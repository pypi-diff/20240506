# Comparing `tmp/orchestrator_core-2.2.2rc2.tar.gz` & `tmp/orchestrator_core-2.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-2.2.2rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-2.3.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-2.2.2rc2.tar` & `orchestrator_core-2.3.0rc1.tar`

### file list

```diff
@@ -1,543 +1,560 @@
--rw-r--r--   0        0        0      342 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.coveragerc
--rw-r--r--   0        0        0     1564 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1149 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      502 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/dependabot.yml
--rw-r--r--   0        0        0     2620 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      346 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      583 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/issues.yml
--rw-r--r--   0        0        0      550 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1215 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2426 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1809 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.gitignore
--rw-r--r--   0        0        0     2599 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.stignore
--rw-r--r--   0        0        0    30927 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/CHANGELOG.md
--rw-r--r--   0        0        0      333 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/Dockerfile
--rw-r--r--   0        0        0    11409 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/LICENSE
--rw-r--r--   0        0        0      150 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/NOTICE
--rw-r--r--   0        0        0     5595 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/README.md
--rw-r--r--   0        0        0      196 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/codecov.yml
--rw-r--r--   0        0        0       45 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/api.md
--rw-r--r--   0        0        0     5505 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/callbacks.md
--rw-r--r--   0        0        0    30737 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0    13882 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    28254 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/graphql.md
--rw-r--r--   0        0        0    48994 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5585 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2500 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11462 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0      668 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/context.md
--rw-r--r--   0        0        0      802 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/introduction.md
--rw-r--r--   0        0        0     1671 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/ip_static.md
--rw-r--r--   0        0        0    84576 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/ip_static.png
--rw-r--r--   0        0        0     1311 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.md
--rw-r--r--   0        0        0    55937 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.png
--rw-r--r--   0        0        0      854 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_vpn.md
--rw-r--r--   0        0        0    29551 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_vpn.png
--rw-r--r--   0        0        0     1398 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/modelling.md
--rw-r--r--   0        0        0     1138 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/node.md
--rw-r--r--   0        0        0    23110 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/node.png
--rw-r--r--   0        0        0     1147 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/port.md
--rw-r--r--   0        0        0    37248 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/port.png
--rw-r--r--   0        0        0     1694 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/product_block_graph.md
--rw-r--r--   0        0        0    78824 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/product_block_graph.png
--rw-r--r--   0        0        0      989 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/standards.md
--rw-r--r--   0        0        0     1114 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/terminology.md
--rw-r--r--   0        0        0     2080 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/contributing/guidelines.md
--rw-r--r--   0        0        0     9997 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/css/custom.css
--rw-r--r--   0        0        0      656 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/css/style.css
--rw-r--r--   0        0        0     2165 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/getting-started/development.md
--rw-r--r--   0        0        0     3438 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/getting-started/prepare-source-folder.md
--rw-r--r--   0        0        0    17905 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/img/WFO-Emblem-White.png
--rw-r--r--   0        0        0      842 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/img/favicon.ico
--rw-r--r--   0        0        0     4020 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/index.md
--rw-r--r--   0        0        0     3897 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/js/termynal.js
--rw-r--r--   0        0        0    11084 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/migration-guide/2.0.md
--rw-r--r--   0        0        0     9063 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/circuit-workflow.md
--rw-r--r--   0        0        0      254 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/database-migration.md
--rw-r--r--   0        0        0     3719 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/docker-installation.md
--rw-r--r--   0        0        0     2563 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/domain-models.md
--rw-r--r--   0        0        0     6048 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/node-workflow.md
--rw-r--r--   0        0        0     3087 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/overview.md
--rw-r--r--   0        0        0     1750 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/scenario.md
--rw-r--r--   0        0        0     4369 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/workflow-introduction.md
--rw-r--r--   0        0        0     5602 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4623 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7447 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3697 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3051 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6156 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1953 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3991 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3596 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2141 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2878 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      785 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3632 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0   983304 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/docs/workshops/images/netbox_devices_active.png
--rw-r--r--   0        0        0     5478 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/mkdocs.yml
--rw-r--r--   0        0        0     1262 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/mutmut_config.py
--rw-r--r--   0        0        0       70 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/nitpick-style.toml
--rw-r--r--   0        0        0     1098 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     3145 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     1034 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1284 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    14585 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     4021 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     4806 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     3657 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     6106 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     3081 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    15675 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      963 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1827 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     2563 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1722 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/ws.py
--rw-r--r--   0        0        0     1502 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    10612 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5996 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/models.py
--rw-r--r--   0        0        0     8721 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/app.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13792 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6775 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     2172 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10474 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9379 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    23981 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1399 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0     7377 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generate.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/__init__.py
--rw-r--r--   0        0        0      173 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/README
--rw-r--r--   0        0        0      307 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
--rw-r--r--   0        0        0      115 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
--rw-r--r--   0        0        0       82 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
--rw-r--r--   0        0        0      307 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
--rw-r--r--   0        0        0      115 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
--rw-r--r--   0        0        0       82 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
--rw-r--r--   0        0        0      234 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
--rw-r--r--   0        0        0      131 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
--rw-r--r--   0        0        0       82 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/__init__.py
--rw-r--r--   0        0        0     2007 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/enums.py
--rw-r--r--   0        0        0     5452 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/helpers.py
--rw-r--r--   0        0        0     6341 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/migration.py
--rw-r--r--   0        0        0     2073 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/product.py
--rw-r--r--   0        0        0     5285 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/product_block.py
--rw-r--r--   0        0        0     1379 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/settings.py
--rw-r--r--   0        0        0     1878 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/translations.py
--rw-r--r--   0        0        0     4541 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/unittest.py
--rw-r--r--   0        0        0     1815 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/validations.py
--rw-r--r--   0        0        0     8026 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/workflow.py
--rw-r--r--   0        0        0      759 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/circuit.yaml
--rw-r--r--   0        0        0      538 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/node.yaml
--rw-r--r--   0        0        0      532 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/user.yaml
--rw-r--r--   0        0        0      361 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/user_group.yaml
--rw-r--r--   0        0        0      431 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_create_imports.j2
--rw-r--r--   0        0        0       25 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_create_steps.j2
--rw-r--r--   0        0        0      394 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_modify_imports.j2
--rw-r--r--   0        0        0       25 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_modify_steps.j2
--rw-r--r--   0        0        0       25 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0      282 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/constrained_int_definitions.j2
--rw-r--r--   0        0        0      361 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/create_data_head.j2
--rw-r--r--   0        0        0     4806 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/create_product.j2
--rw-r--r--   0        0        0      298 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/enums.j2
--rw-r--r--   0        0        0      523 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
--rw-r--r--   0        0        0      277 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/list_definitions.j2
--rw-r--r--   0        0        0      904 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/macros.j2
--rw-r--r--   0        0        0     4719 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/modify_product.j2
--rw-r--r--   0        0        0     2901 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/new_product_migration.j2
--rw-r--r--   0        0        0     1365 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/product.j2
--rw-r--r--   0        0        0     2454 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/product_block.j2
--rw-r--r--   0        0        0      545 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/shared_forms.j2
--rw-r--r--   0        0        0     1274 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/shared_workflows.j2
--rw-r--r--   0        0        0      291 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/subscription_model_registry.j2
--rw-r--r--   0        0        0     1883 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/terminate_product.j2
--rw-r--r--   0        0        0     1802 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_create_workflow.j2
--rw-r--r--   0        0        0     1677 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2
--rw-r--r--   0        0        0     1860 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_product_type.j2
--rw-r--r--   0        0        0     1518 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2
--rw-r--r--   0        0        0      985 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2
--rw-r--r--   0        0        0     2315 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/validate_product.j2
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1139 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      857 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      983 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20371 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8979 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4110 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2970 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10269 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/db/database.py
--rw-r--r--   0        0        0      371 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     5020 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0     4144 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0      899 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0     1089 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/product_block.py
--rw-r--r--   0        0        0      889 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/resource_type.py
--rw-r--r--   0        0        0      562 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/search_filters/__init__.py
--rw-r--r--   0        0        0     5591 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/search_filters/inferred_filter.py
--rw-r--r--   0        0        0     1466 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/subscription.py
--rw-r--r--   0        0        0     1276 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/workflow.py
--rw-r--r--   0        0        0      831 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/helpers.py
--rw-r--r--   0        0        0    24900 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/models.py
--rw-r--r--   0        0        0      162 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     2175 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      353 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0     1987 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      570 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0      617 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/product_block.py
--rw-r--r--   0        0        0      617 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/resource_type.py
--rw-r--r--   0        0        0     4455 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0     1441 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/subscription.py
--rw-r--r--   0        0        0      576 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/workflow.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    18847 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/devtools/scripts/__init__.py
--rw-r--r--   0        0        0     8359 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/devtools/scripts/migrate_20.py
--rw-r--r--   0        0        0     2494 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2508 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3114 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3271 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      894 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    59246 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2732 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/customer_description.py
--rw-r--r--   0        0        0      989 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/helpers.py
--rw-r--r--   0        0        0     2882 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     1268 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0      892 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     1906 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/__init__.py
--rw-r--r--   0        0        0     1505 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/customer_contact_list.py
--rw-r--r--   0        0        0      708 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/customer_id.py
--rw-r--r--   0        0        0      779 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/display_subscription.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/network_type_validators.py
--rw-r--r--   0        0        0     2114 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/product_id.py
--rw-r--r--   0        0        0     1482 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0     6159 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/autoregistration.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4304 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     1746 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/error_collector_extension.py
--rw-r--r--   0        0        0     5826 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/error_handler_extension.py
--rw-r--r--   0        0        0     3100 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/mutations/customer_description.py
--rw-r--r--   0        0        0     1553 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/mutations/start_process.py
--rw-r--r--   0        0        0     2413 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      851 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0      934 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/customer.py
--rw-r--r--   0        0        0      636 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/helpers.py
--rw-r--r--   0        0        0     4491 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2562 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     2748 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/product_block.py
--rw-r--r--   0        0        0     2741 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/resource_type.py
--rw-r--r--   0        0        0     3700 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0     5888 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/subscription.py
--rw-r--r--   0        0        0     2681 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/workflow.py
--rw-r--r--   0        0        0     7736 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schema.py
--rw-r--r--   0        0        0      798 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/__init__.py
--rw-r--r--   0        0        0      147 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/customer.py
--rw-r--r--   0        0        0      213 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/customer_description.py
--rw-r--r--   0        0        0      203 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     3482 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0     2134 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0     1203 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      755 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      999 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0     7838 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/subscription.py
--rw-r--r--   0        0        0     1140 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     4905 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      524 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0     1191 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/create_resolver_error_handler.py
--rw-r--r--   0        0        0     1002 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0     3897 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/get_subscription_product_blocks.py
--rw-r--r--   0        0        0     2156 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/is_query_detailed.py
--rw-r--r--   0        0        0     1370 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/override_class.py
--rw-r--r--   0        0        0      902 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/to_graphql_result_page.py
--rw-r--r--   0        0        0       39 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3382 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40911 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2698 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1265 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    39307 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      950 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1214 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1603 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5106 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7964 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0     1014 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
--rw-r--r--   0        0        0      591 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
--rw-r--r--   0        0        0      755 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
--rw-r--r--   0        0        0      967 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
--rw-r--r--   0        0        0     4491 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
--rw-r--r--   0        0        0     1036 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
--rw-r--r--   0        0        0     5383 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
--rw-r--r--   0        0        0     2246 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/py.typed
--rw-r--r--   0        0        0     1066 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1526 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1234 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2195 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2708 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      888 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1286 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1356 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      802 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     2693 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1698 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1792 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      973 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3366 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1030 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1977 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1744 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/security.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3635 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/celery.py
--rw-r--r--   0        0        0      876 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/fixed_inputs.py
--rw-r--r--   0        0        0     3710 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/process_broadcast_thread.py
--rw-r--r--   0        0        0    26253 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1933 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/products.py
--rw-r--r--   0        0        0      884 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/resource_types.py
--rw-r--r--   0        0        0     2723 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/settings.py
--rw-r--r--   0        0        0    25733 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5867 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1713 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/translations.py
--rw-r--r--   0        0        0     1638 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/workflows.py
--rw-r--r--   0        0        0     3634 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/targets.py
--rw-r--r--   0        0        0    16236 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/types.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5584 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0      875 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/deprecation_logger.py
--rw-r--r--   0        0        0     6172 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     4658 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/enrich_process.py
--rw-r--r--   0        0        0     4250 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     2665 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/fixed_inputs.py
--rw-r--r--   0        0        0     8063 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     1322 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/get_updated_properties.py
--rw-r--r--   0        0        0     3212 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8341 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/json.py
--rw-r--r--   0        0        0     6378 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/utils/redis.py
--rw-r--r--   0        0        0    17039 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/utils/search_query.py
--rw-r--r--   0        0        0    12998 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     1366 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/version.py
--rw-r--r--   0        0        0     4828 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     4596 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3324 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2924 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    42689 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflow.py
--rw-r--r--   0        0        0     4048 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9528 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1614 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2349 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8511 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0    12929 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     5073 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/pyproject.toml
--rw-r--r--   0        0        0     2725 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/setup.cfg
--rw-r--r--   0        0        0      665 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/setup.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1529 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2887 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5160 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1626 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1139 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3055 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    21379 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    15509 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3787 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     8209 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2530 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     3000 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     3038 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    41173 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     3457 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0     3777 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_ws.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/__init__.py
--rw-r--r--   0        0        0      744 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate.sh
--rw-r--r--   0        0        0      885 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/alembic.ini
--rw-r--r--   0        0        0      233 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/main.py
--rw-r--r--   0        0        0     2821 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/env.py
--rw-r--r--   0        0        0       98 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/script.py.mako
--rw-r--r--   0        0        0      315 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
--rw-r--r--   0        0        0     2227 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
--rw-r--r--   0        0        0     3852 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
--rw-r--r--   0        0        0      467 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1995 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
--rw-r--r--   0        0        0      812 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/__init__.py
--rw-r--r--   0        0        0      764 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/example1.py
--rw-r--r--   0        0        0      559 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/example2.py
--rw-r--r--   0        0        0     1499 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
--rw-r--r--   0        0        0     1499 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
--rw-r--r--   0        0        0     2442 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
--rw-r--r--   0        0        0     2014 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
--rw-r--r--   0        0        0     1345 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
--rw-r--r--   0        0        0     1010 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
--rw-r--r--   0        0        0      902 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
--rw-r--r--   0        0        0      872 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
--rw-r--r--   0        0        0      755 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
--rw-r--r--   0        0        0      405 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
--rw-r--r--   0        0        0      415 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/translations/en-GB.json
--rw-r--r--   0        0        0      701 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/__init__.py
--rw-r--r--   0        0        0     3940 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
--rw-r--r--   0        0        0     3602 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
--rw-r--r--   0        0        0      620 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
--rw-r--r--   0        0        0     1560 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
--rw-r--r--   0        0        0     1025 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
--rw-r--r--   0        0        0     2683 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
--rw-r--r--   0        0        0     2508 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
--rw-r--r--   0        0        0        1 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
--rw-r--r--   0        0        0     1220 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
--rw-r--r--   0        0        0     1273 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/shared.py
--rw-r--r--   0        0        0     2656 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config1.yaml
--rw-r--r--   0        0        0      549 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config2.yaml
--rw-r--r--   0        0        0      590 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config3.yaml
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/generator/__init__.py
--rw-r--r--   0        0        0      812 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/generator/test_enums.py
--rw-r--r--   0        0        0     2509 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_cli_generate.py
--rw-r--r--   0        0        0     2930 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_generate_code.py
--rw-r--r--   0        0        0    26343 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27644 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/config.py
--rw-r--r--   0        0        0    23677 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    53002 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8230 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4670 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     1992 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_lifecycle.py
--rw-r--r--   0        0        0     2841 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7794 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1645 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2970 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1606 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2573 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2518 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1194 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1123 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2172 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4217 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3428 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2951 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2272 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2256 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1639 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1838 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      644 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0      451 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/workflows.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     4706 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_customer_contact_list.py
--rw-r--r--   0        0        0      495 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_customer_id.py
--rw-r--r--   0        0        0     1746 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_display_subscription.py
--rw-r--r--   0        0        0     4109 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/__init__.py
--rw-r--r--   0        0        0     1424 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/conftest.py
--rw-r--r--   0        0        0      488 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/helpers.py
--rw-r--r--   0        0        0     6235 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/test_customer_description.py
--rw-r--r--   0        0        0     2449 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/test_start_process.py
--rw-r--r--   0        0        0     2316 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_customer.py
--rw-r--r--   0        0        0    18677 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     8514 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0    10211 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_product_blocks.py
--rw-r--r--   0        0        0     5635 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_resource_types.py
--rw-r--r--   0        0        0     5179 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0     2939 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_sort_and_filter_fields.py
--rw-r--r--   0        0        0     3239 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_subscription.py
--rw-r--r--   0        0        0    48770 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_subscriptions.py
--rw-r--r--   0        0        0     6682 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_workflows.py
--rw-r--r--   0        0        0      608 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_autoregistration.py
--rw-r--r--   0        0        0     7669 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_is_query_detailed.py
--rw-r--r--   0        0        0     3042 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_is_querying_page_data.py
--rw-r--r--   0        0        0     8760 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_override_class.py
--rw-r--r--   0        0        0      631 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/helpers.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    28556 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1155 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     6171 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     6852 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      379 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    17406 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1891 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3486 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3529 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_get_updated_properties.py
--rw-r--r--   0        0        0     3052 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     5867 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_search_query.py
--rw-r--r--   0        0        0    11471 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/websocket/__init__.py
--rw-r--r--   0        0        0     3561 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/websocket/test_broadcast.py
--rw-r--r--   0        0        0    14040 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2094 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2746 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     5378 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_async_workflow.py
--rw-r--r--   0        0        0     3495 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1884 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 orchestrator_core-2.2.2rc2/PKG-INFO
+-rw-r--r--   0        0        0      342 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.coveragerc
+-rw-r--r--   0        0        0     1564 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1149 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      502 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2620 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      346 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      583 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/issues.yml
+-rw-r--r--   0        0        0      550 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1221 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2426 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1809 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.gitignore
+-rw-r--r--   0        0        0     2599 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.stignore
+-rw-r--r--   0        0        0    30927 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/Dockerfile
+-rw-r--r--   0        0        0    11409 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/LICENSE
+-rw-r--r--   0        0        0      150 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/NOTICE
+-rw-r--r--   0        0        0     5595 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/README.md
+-rw-r--r--   0        0        0      196 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/codecov.yml
+-rw-r--r--   0        0        0    10746 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0     9277 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/application/forms-frontend.md
+-rw-r--r--   0        0        0     5514 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0    11462 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0      668 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/context.md
+-rw-r--r--   0        0        0     4226 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/imports.md
+-rw-r--r--   0        0        0      802 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/introduction.md
+-rw-r--r--   0        0        0     1671 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/ip_static.md
+-rw-r--r--   0        0        0    84576 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/ip_static.png
+-rw-r--r--   0        0        0     1311 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_point_to_point.md
+-rw-r--r--   0        0        0    55937 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_point_to_point.png
+-rw-r--r--   0        0        0      854 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_vpn.md
+-rw-r--r--   0        0        0    29551 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_vpn.png
+-rw-r--r--   0        0        0     1398 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/modelling.md
+-rw-r--r--   0        0        0     1138 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/node.md
+-rw-r--r--   0        0        0    23110 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/node.png
+-rw-r--r--   0        0        0     1147 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/port.md
+-rw-r--r--   0        0        0    37248 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/port.png
+-rw-r--r--   0        0        0     1694 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/product_block_graph.md
+-rw-r--r--   0        0        0    78824 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/product_block_graph.png
+-rw-r--r--   0        0        0      989 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/standards.md
+-rw-r--r--   0        0        0     1114 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/terminology.md
+-rw-r--r--   0        0        0     2080 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/tldr.md
+-rw-r--r--   0        0        0      443 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/contributing/documentation.md
+-rw-r--r--   0        0        0     1771 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0     9997 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/css/custom.css
+-rw-r--r--   0        0        0      656 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/css/style.css
+-rw-r--r--   0        0        0     2165 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/getting-started/development.md
+-rw-r--r--   0        0        0     3438 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/getting-started/prepare-source-folder.md
+-rw-r--r--   0        0        0    17905 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/img/WFO-Emblem-White.png
+-rw-r--r--   0        0        0      842 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/img/favicon.ico
+-rw-r--r--   0        0        0     4005 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/index.md
+-rw-r--r--   0        0        0     3897 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/js/termynal.js
+-rw-r--r--   0        0        0    11084 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/migration-guide/2.0.md
+-rw-r--r--   0        0        0      600 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/api.md
+-rw-r--r--   0        0        0     1026 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/app/app.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/app/runtimes.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/auth.md
+-rw-r--r--   0        0        0    29652 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/cli.md
+-rw-r--r--   0        0        0     2241 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/database.md
+-rw-r--r--   0        0        0      359 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/generator.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/instantiating.md
+-rw-r--r--   0        0        0     3867 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/model_attributes.md
+-rw-r--r--   0        0        0      543 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/overview.md
+-rw-r--r--   0        0        0     3863 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/product_blocks.md
+-rw-r--r--   0        0        0     4030 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/product_types.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/properties.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/pydantic_hooks.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/type_casting.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/union_types.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/validation.md
+-rw-r--r--   0        0        0    15366 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/forms.md
+-rw-r--r--   0        0        0    27254 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/graphql.md
+-rw-r--r--   0        0        0     1565 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/python.md
+-rw-r--r--   0        0        0     5585 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/scaling.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/serialization.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/tasks.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/tests.md
+-rw-r--r--   0        0        0      499 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/tldr.md
+-rw-r--r--   0        0        0     2500 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/websockets.md
+-rw-r--r--   0        0        0     5505 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/workflows/callbacks.md
+-rw-r--r--   0        0        0       73 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/workflows/workflow-lifecycles.md
+-rw-r--r--   0        0        0     1472 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/workflows/workflow-steps.md
+-rw-r--r--   0        0        0     9063 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/circuit-workflow.md
+-rw-r--r--   0        0        0      254 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/database-migration.md
+-rw-r--r--   0        0        0     3719 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/docker-installation.md
+-rw-r--r--   0        0        0     2563 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/domain-models.md
+-rw-r--r--   0        0        0     6048 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/node-workflow.md
+-rw-r--r--   0        0        0     3087 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/overview.md
+-rw-r--r--   0        0        0     1750 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/scenario.md
+-rw-r--r--   0        0        0     4369 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/workflow-introduction.md
+-rw-r--r--   0        0        0     5602 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4623 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7447 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3697 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3051 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6157 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1953 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3991 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3596 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2141 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2878 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      785 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3632 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0   983304 2024-05-06 11:29:58.002776 orchestrator_core-2.3.0rc1/docs/workshops/images/netbox_devices_active.png
+-rw-r--r--   0        0        0      312 2024-05-06 11:29:58.002776 orchestrator_core-2.3.0rc1/includes/abbreviations.md
+-rw-r--r--   0        0        0     8030 2024-05-06 11:29:58.002776 orchestrator_core-2.3.0rc1/mkdocs.yml
+-rw-r--r--   0        0        0     1262 2024-05-06 11:29:58.002776 orchestrator_core-2.3.0rc1/mutmut_config.py
+-rw-r--r--   0        0        0       70 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/nitpick-style.toml
+-rw-r--r--   0        0        0     1098 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2415 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     1284 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    12428 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2143 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     6106 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     3081 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0     8861 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      963 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1827 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1722 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/ws.py
+-rw-r--r--   0        0        0     1502 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0     6933 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5996 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/models.py
+-rw-r--r--   0        0        0     8886 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    16226 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6775 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     2172 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10474 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9379 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    23981 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1399 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     7377 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0      173 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/README
+-rw-r--r--   0        0        0      307 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
+-rw-r--r--   0        0        0      115 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      307 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0      115 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0      234 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
+-rw-r--r--   0        0        0      131 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     2007 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/enums.py
+-rw-r--r--   0        0        0     5452 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     6341 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2073 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5285 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1379 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1878 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4541 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1815 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     8026 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      759 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      538 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      532 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      361 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      431 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_create_imports.j2
+-rw-r--r--   0        0        0       25 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      394 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0       25 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0       25 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0      282 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0      361 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/create_data_head.j2
+-rw-r--r--   0        0        0     4806 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      298 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/enums.j2
+-rw-r--r--   0        0        0      523 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
+-rw-r--r--   0        0        0      277 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      904 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4719 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2901 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1365 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2454 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      545 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     1274 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/shared_workflows.j2
+-rw-r--r--   0        0        0      291 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/subscription_model_registry.j2
+-rw-r--r--   0        0        0     1883 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1802 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1677 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      985 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2315 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      857 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20371 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8979 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4110 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2970 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10269 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/database.py
+-rw-r--r--   0        0        0      371 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     5020 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0     4144 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0      899 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0     1089 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/product_block.py
+-rw-r--r--   0        0        0      889 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/resource_type.py
+-rw-r--r--   0        0        0      562 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/search_filters/__init__.py
+-rw-r--r--   0        0        0     5591 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/search_filters/inferred_filter.py
+-rw-r--r--   0        0        0     1466 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/subscription.py
+-rw-r--r--   0        0        0     1276 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/workflow.py
+-rw-r--r--   0        0        0      831 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/helpers.py
+-rw-r--r--   0        0        0    24900 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/models.py
+-rw-r--r--   0        0        0      162 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     2175 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      353 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0     1987 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      570 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0      617 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/product_block.py
+-rw-r--r--   0        0        0      617 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/resource_type.py
+-rw-r--r--   0        0        0     4455 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0     1441 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/subscription.py
+-rw-r--r--   0        0        0      576 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/workflow.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    18847 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/devtools/scripts/__init__.py
+-rw-r--r--   0        0        0     8359 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/devtools/scripts/migrate_20.py
+-rw-r--r--   0        0        0     2494 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2508 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3114 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3271 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      894 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    59707 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2732 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/customer_description.py
+-rw-r--r--   0        0        0      989 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/helpers.py
+-rw-r--r--   0        0        0     2882 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     1268 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     1168 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     1906 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/__init__.py
+-rw-r--r--   0        0        0     1505 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/customer_contact_list.py
+-rw-r--r--   0        0        0      708 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/customer_id.py
+-rw-r--r--   0        0        0      779 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/display_subscription.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/network_type_validators.py
+-rw-r--r--   0        0        0     2114 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/product_id.py
+-rw-r--r--   0        0        0     1482 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0     6413 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/autoregistration.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4304 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     1746 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/error_collector_extension.py
+-rw-r--r--   0        0        0     5826 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/error_handler_extension.py
+-rw-r--r--   0        0        0     3100 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/mutations/customer_description.py
+-rw-r--r--   0        0        0     1553 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/mutations/start_process.py
+-rw-r--r--   0        0        0     2413 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      851 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0      934 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/customer.py
+-rw-r--r--   0        0        0      636 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/helpers.py
+-rw-r--r--   0        0        0     4491 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2562 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     2748 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/product_block.py
+-rw-r--r--   0        0        0     2741 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/resource_type.py
+-rw-r--r--   0        0        0     3700 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0     5888 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/subscription.py
+-rw-r--r--   0        0        0     2681 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/workflow.py
+-rw-r--r--   0        0        0     7736 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schema.py
+-rw-r--r--   0        0        0      798 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/__init__.py
+-rw-r--r--   0        0        0      147 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/customer.py
+-rw-r--r--   0        0        0      213 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/customer_description.py
+-rw-r--r--   0        0        0      203 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     3482 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     2430 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0     2414 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      755 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      999 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0     7838 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/subscription.py
+-rw-r--r--   0        0        0     1140 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     4905 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      524 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0     1191 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/create_resolver_error_handler.py
+-rw-r--r--   0        0        0     1002 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0     4374 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/get_subscription_product_blocks.py
+-rw-r--r--   0        0        0     2156 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/is_query_detailed.py
+-rw-r--r--   0        0        0     1370 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/override_class.py
+-rw-r--r--   0        0        0      902 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/to_graphql_result_page.py
+-rw-r--r--   0        0        0       39 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3382 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40911 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2698 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1265 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    39307 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      950 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1214 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1603 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5106 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7964 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0     1014 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
+-rw-r--r--   0        0        0      591 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
+-rw-r--r--   0        0        0      755 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
+-rw-r--r--   0        0        0      967 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
+-rw-r--r--   0        0        0     4491 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
+-rw-r--r--   0        0        0     1036 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
+-rw-r--r--   0        0        0     5383 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
+-rw-r--r--   0        0        0     2246 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/py.typed
+-rw-r--r--   0        0        0     1066 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1526 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1234 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2195 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2326 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      930 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1286 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1214 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      802 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     2354 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1484 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1428 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      973 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3366 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1030 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1890 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1744 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3635 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/celery.py
+-rw-r--r--   0        0        0      876 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/fixed_inputs.py
+-rw-r--r--   0        0        0     3710 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/process_broadcast_thread.py
+-rw-r--r--   0        0        0    26253 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1933 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/products.py
+-rw-r--r--   0        0        0      884 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/resource_types.py
+-rw-r--r--   0        0        0     2723 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    25733 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5867 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1713 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     1638 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/workflows.py
+-rw-r--r--   0        0        0     3634 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/targets.py
+-rw-r--r--   0        0        0    16236 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5584 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0      875 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/deprecation_logger.py
+-rw-r--r--   0        0        0     6172 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     4658 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/enrich_process.py
+-rw-r--r--   0        0        0     4250 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     2665 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/fixed_inputs.py
+-rw-r--r--   0        0        0     8063 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     1322 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/get_updated_properties.py
+-rw-r--r--   0        0        0     3212 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8341 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     6378 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0    17039 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/search_query.py
+-rw-r--r--   0        0        0    13011 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     1366 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/version.py
+-rw-r--r--   0        0        0     4828 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     4596 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3324 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2924 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    42689 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4048 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2175 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9528 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1614 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2349 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8511 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12929 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     5208 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2725 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/setup.cfg
+-rw-r--r--   0        0        0      665 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/setup.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1529 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1210 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2887 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5160 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1139 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3055 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    19442 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    15509 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     5841 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     3000 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     3038 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    29171 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     3777 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_ws.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/__init__.py
+-rw-r--r--   0        0        0      744 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate.sh
+-rw-r--r--   0        0        0      885 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/alembic.ini
+-rw-r--r--   0        0        0      233 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/main.py
+-rw-r--r--   0        0        0     2821 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/env.py
+-rw-r--r--   0        0        0       98 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/script.py.mako
+-rw-r--r--   0        0        0      315 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
+-rw-r--r--   0        0        0     2227 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
+-rw-r--r--   0        0        0     3852 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
+-rw-r--r--   0        0        0      467 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1995 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
+-rw-r--r--   0        0        0      812 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/example1.py
+-rw-r--r--   0        0        0      559 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/example2.py
+-rw-r--r--   0        0        0     1499 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
+-rw-r--r--   0        0        0     1499 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
+-rw-r--r--   0        0        0     2442 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
+-rw-r--r--   0        0        0     2014 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
+-rw-r--r--   0        0        0     1345 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
+-rw-r--r--   0        0        0     1010 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
+-rw-r--r--   0        0        0      902 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
+-rw-r--r--   0        0        0      872 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
+-rw-r--r--   0        0        0      755 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
+-rw-r--r--   0        0        0      405 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
+-rw-r--r--   0        0        0      415 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/translations/en-GB.json
+-rw-r--r--   0        0        0      701 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/__init__.py
+-rw-r--r--   0        0        0     3940 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
+-rw-r--r--   0        0        0     3602 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
+-rw-r--r--   0        0        0      620 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
+-rw-r--r--   0        0        0     1560 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
+-rw-r--r--   0        0        0     1025 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
+-rw-r--r--   0        0        0     2683 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
+-rw-r--r--   0        0        0     2508 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
+-rw-r--r--   0        0        0        1 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
+-rw-r--r--   0        0        0     1220 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
+-rw-r--r--   0        0        0     1273 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/shared.py
+-rw-r--r--   0        0        0     2656 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config1.yaml
+-rw-r--r--   0        0        0      549 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config2.yaml
+-rw-r--r--   0        0        0      590 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config3.yaml
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/generator/__init__.py
+-rw-r--r--   0        0        0      812 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/generator/test_enums.py
+-rw-r--r--   0        0        0     2509 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_cli_generate.py
+-rw-r--r--   0        0        0     2930 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_generate_code.py
+-rw-r--r--   0        0        0    26343 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27644 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/config.py
+-rw-r--r--   0        0        0    23677 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    53002 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8230 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4670 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     1992 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_lifecycle.py
+-rw-r--r--   0        0        0     2841 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7794 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1645 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2970 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1606 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2573 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2518 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1194 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1123 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2172 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4217 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3428 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2951 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2272 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2256 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1639 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1838 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      644 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0      451 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     4706 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_customer_contact_list.py
+-rw-r--r--   0        0        0      495 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_customer_id.py
+-rw-r--r--   0        0        0     1746 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_display_subscription.py
+-rw-r--r--   0        0        0     4109 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/__init__.py
+-rw-r--r--   0        0        0     1424 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/conftest.py
+-rw-r--r--   0        0        0      488 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/helpers.py
+-rw-r--r--   0        0        0     6235 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/test_customer_description.py
+-rw-r--r--   0        0        0     2449 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/test_start_process.py
+-rw-r--r--   0        0        0     2316 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_customer.py
+-rw-r--r--   0        0        0    18677 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     8514 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0    10211 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_product_blocks.py
+-rw-r--r--   0        0        0     5635 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_resource_types.py
+-rw-r--r--   0        0        0     5179 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0     2939 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_sort_and_filter_fields.py
+-rw-r--r--   0        0        0     3239 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_subscription.py
+-rw-r--r--   0        0        0    48814 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_subscriptions.py
+-rw-r--r--   0        0        0     6682 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_workflows.py
+-rw-r--r--   0        0        0      608 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_autoregistration.py
+-rw-r--r--   0        0        0     7669 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_is_query_detailed.py
+-rw-r--r--   0        0        0     3042 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_is_querying_page_data.py
+-rw-r--r--   0        0        0     8760 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_override_class.py
+-rw-r--r--   0        0        0      631 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    28556 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1155 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     6171 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     6852 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      379 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    17406 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1891 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3486 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3529 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_get_updated_properties.py
+-rw-r--r--   0        0        0     3907 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     5867 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_search_query.py
+-rw-r--r--   0        0        0    11471 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/websocket/__init__.py
+-rw-r--r--   0        0        0     3561 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/websocket/test_broadcast.py
+-rw-r--r--   0        0        0    14040 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2094 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2443 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2746 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     5378 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_async_workflow.py
+-rw-r--r--   0        0        0     3495 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1884 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 orchestrator_core-2.3.0rc1/PKG-INFO
```

### Comparing `orchestrator_core-2.2.2rc2/.github/ISSUE_TEMPLATE/bug-report.yml` & `orchestrator_core-2.3.0rc1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.github/ISSUE_TEMPLATE/feature-request.yml` & `orchestrator_core-2.3.0rc1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.github/workflows/README.md` & `orchestrator_core-2.3.0rc1/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.github/workflows/build-push-container.yml` & `orchestrator_core-2.3.0rc1/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.github/workflows/codeql-analysis.yml` & `orchestrator_core-2.3.0rc1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.github/workflows/issues.yml` & `orchestrator_core-2.3.0rc1/.github/workflows/issues.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.github/workflows/publish-package.yml` & `orchestrator_core-2.3.0rc1/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.github/workflows/run-linting-tests.yml` & `orchestrator_core-2.3.0rc1/.github/workflows/run-linting-tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -31,13 +31,13 @@
           flit install --deps develop --symlink
       - name: Check formatting
         run: |
           black --check .
       - name: Lint with ruff
         run: |
           # stop the build if there are Python syntax errors or undefined names
-          ruff .
+          ruff check .
       - name: Check with mypy
         run: |
           mypy .
       - name: Run remaining pre-commit hooks
         uses: pre-commit/action@v3.0.1
```

### Comparing `orchestrator_core-2.2.2rc2/.github/workflows/run-unit-tests.yml` & `orchestrator_core-2.3.0rc1/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.github/workflows/scheduled-build.yml` & `orchestrator_core-2.3.0rc1/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.gitignore` & `orchestrator_core-2.3.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.pre-commit-config.yaml` & `orchestrator_core-2.3.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/.stignore` & `orchestrator_core-2.3.0rc1/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/CHANGELOG.md` & `orchestrator_core-2.3.0rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/LICENSE` & `orchestrator_core-2.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/README.md` & `orchestrator_core-2.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/callbacks.md` & `orchestrator_core-2.3.0rc1/docs/reference-docs/workflows/callbacks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/cli.md` & `orchestrator_core-2.3.0rc1/docs/reference-docs/cli.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,51 @@
-# Command line interface commands
+# Command Line Interface Commands
 
 Top level options:
 
---install-completion [bash|zsh|fish|powershell|pwsh]
+`--install-completion [bash|zsh|fish|powershell|pwsh]`
 
 Install completion for the specified shell. [default: None]
 
---show-completion [bash|zsh|fish|powershell|pwsh]
+`--show-completion [bash|zsh|fish|powershell|pwsh]`
 
 Show completion for the specified shell, to copy it or customize the
 installation. [default: None]
 
 ## db
 
-Interact with the application database.
+Interact with the application database. By default, does nothing, specify `main.py db --help` for more information.
 
-### downgrade
-
-The `main.py db downgrade` command will downgrade the database to the previous
-revision or to the optionally specified revision.
-
-Arguments
-
-revision - Rev id to upgrade to [default: -1]
-
-### heads
-
-The `main.py db heads` command shows the Alembic database heads.
-
-### history
-
-The `main.py db history` command lists Alembic revision history in
-chronological order.
-
-Options
-
---verbose - Verbose output
---current - Indicate current revision
-
-### init
-
-The `main.py db init` command initialises an empty migrations environment.
-This command will throw an exception when it detects conflicting files and
-directories.
-
-### merge
-
-The `main.py db merge` command merges database revisions.
-
-Arguments
-
-revisions - Add the revision you would like to merge to this command
-[default: None]
-
-Options
-
---message TEXT - The revision message
+::: orchestrator.cli.database
+    options:
+      show_signature: false
+      show_root_heading: false
+      docstring_style: google
+      show_docstring_parameters: false
+      show_docstring_returns: false
+      show_root_toc_entry: false
+      show_symbol_type_toc: false
+      show_symbol_type_heading: false
+      members:
+        - init
+        - revision
+        - upgrade
+        - downgrade
+        - heads
+        - history
+        - merge
+        - migrate_workflows
+        - heads
+        - history
+        - init
+        - merge
+        - migrate_workflows
+        - revision
+        - upgrade
+      heading_level: 3
 
 ### migrate-domain-models
 
 The `main.py db migrate-domain-models` command creates a revision based on the
 difference between domain models in the source code and those that are defined
 in the database.
 
@@ -417,51 +403,14 @@
 2022-10-27 11:45:10 [info] Version Locations [orchestrator.cli.database] locations=/home/tjeerddie/projects_surf/example-orchestrator/migrations/versions/schema /home/tjeerddie/projects_surf/example-orchestrator/.venv/lib/python3.10/site-packages/orchestrator/migrations/versions/schema
   Generating /home/tjeerddie/projects_surf/example-orchestrator/migrations/versions/schema/2022-10-27_a8946b2d1647_test.py ...  done
 Migration generated. Don't forget to create a database backup before migrating!
 ```
 
 If you are running with `--test`, the SQL file will not be generated.
 
-### migrate-workflows
-
-The `main.py db migrate-workflows` command creates a migration file based on
-the difference between de worfklows code and the workflows that are registered
-in the database.
-
-Arguments
-
-message - Migration name [default: None] [required]
-
-Options
-
---test | --no-test - Optional boolean if you don't want to generate a
-migration file [default: no-test]
-
-### revision
-
-The `main.py db revision` command creates a new Alembic revision file.
-
-Arguments
-
---message - The revision message [default: None]
---version-path - Specify specific path from config for version file
-[default: None]
---autogenerate | --no-autogenerate - Detect schema changes and add
-migrations [default: no-autogenerate]
---head - Determine the head you need to add your migration to. [default: None]
-
-### upgrade
-
-The `main.py db upgrade` command will upgrade the database to the specified
-revision
-
-Arguments
-
-revision - Rev id to upgrade to [default: none]
-
 ## generate
 
 Generate products, workflows and other artifacts.
 
 Products can be described in a YAML configuration file which makes it easy to
 generate product and product block domain models, and skeleton workflows and
 unit tests. Note that this is a one time thing, the generate commands do not
@@ -483,15 +432,14 @@
 
 The generate command should be called from the top level folder of your orchestrator
 implementation, this is the folder that contains the `products` sub folder, amongst others, except when
 the `--prefix` is used to point to that folder. In case there are product blocks defined that use other
 generated product blocks, the order in which `generate product-blocks` is run is important,
 the code for the blocks used in other blocks should be generated first.
 
-
 ### config file
 
 An example of a simple product configuration:
 
 ```yaml
 config:
   summary_forms: true
```

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/domainmodels.md` & `orchestrator_core-2.3.0rc1/docs/architecture/application/domainmodels.md`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 this product block model must have all resource_types filled in except for `auto_negotiation` to function correctly.
 
 !!! Tip
     The stricter you are in defining your product block models the more you are able to leverage the built in validation
     of`Pydantic`.
 
 #### Product Model a.k.a SubscriptionModel
-Product models are very similar to Prodblock Models in that they adhere to the same principles as explained above. However
+Product models are very similar to Product Block Models in that they adhere to the same principles as explained above. However
 the difference to Product Block models is that they create `Subscriptions` in the database. They must always have a reference
 to a customer and instead of containing other `ProductBlockModel` or `resource_types` they contain either `fixed_inputs`
 which basically describe fixed product attributes or other `ProductBlockModels.`
 
 ##### Product Model - Inactive
 ```python hl_lines="2 5 7"
 class ServicePortInitial(
@@ -217,15 +217,15 @@
     >>> second_service_port.port.subscription == second_service_port.subscription
     False
     ```
 This is valid use of the domain models. The code will detect that `port` is part of `first_service_port` and respect
 ownership. It basically will treat it as a `read-only` property.
 
 #### Union types
-There may also be a case where a user would like to define two different types to a `ProductBlockModel` propery.
+There may also be a case where a user would like to define two different types to a `ProductBlockModel` property.
 This can be achieved by using the `Union` type decorator.
 
 !!! danger
     When using this method be sure as to declare the **Most** specific type first. This is how Pydantic attempts to cast
     types to the property. For more background as to why, [read here](https://pydantic-docs.helpmanual.io/usage/types/#unions)
 
 ```python hl_lines="4"
```

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/forms.md` & `orchestrator_core-2.3.0rc1/docs/reference-docs/forms.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,77 @@
-# Form input logic
+# Pydantic Forms
 
-In the orchestrator core, form input elements are now class based and subclass the `FormPage` class in the core.
+In the orchestrator core, the forms a user will use in the web UI are created by defining your form input elements as a class that is a subclass of the `FormPage` class in the core. This allows you to write your form data for your WFO instance as simple python classes, but still have a useful form rendered in the frontend Web UI. This is achieved by using the library [pydantic-forms](https://github.com/workfloworchestrator/pydantic-forms). One benefit of this model is that it lets WFO developers not have to understand much about frontend technologies to build complex form structures. It's definitely worth poking around in that module to see the various input types the core library exposes.
+
+## Form Examples
+
+### Importing Form Elements
+
+To use the pydantic forms, you must import the `FormPage` class:
 
 ```python
 from orchestrator.forms import FormPage, ReadOnlyField
 ```
 
-And the validators module exposes validators that also function as "input type widgets":
+Additionally, the validators module exposes validators that also function as "input type widgets". Here is an example of importing some of the built-in validators for use in a workflow:
 
 ```python
 from orchestrator.forms.validators import CustomerId, choice_list, Choice
 ```
 
-It's worth poking around in that module to see the various input types the core library exposes.
+You can, of course, define you own validators as well simply by using pydantic validators, as described in the [pydantic documentation.](https://docs.pydantic.dev/latest/concepts/validators/)
 
-## Form examples
+### Writing Forms
 
-Here is a relatively simple input form:
+Writing forms is quite straight forward, here is a relatively simple input form:
 
 ```python
-equipment = get_planned_equipment()
+equipment = get_planned_equipment() # grab available equipment from inventory system
 choices = [f"{eq['name']}" for eq in equipment]
 
 EquipmentList = choice_list(
     Choice("EquipmentEnum", zip(choices, choices)),
     min_items=1,
     max_items=1,
     unique_items=True,
 )
 
 
 class CreateNodeEnrollmentForm(FormPage):
     class Config:
         title = product_name
 
-    customer_id: CustomerId = ReadOnlyField(CustomerId(ESNET_ORG_UUID))
+    customer_id: CustomerId = ReadOnlyField(CustomerId(DEFAULT_ORG_UUID))
     select_node_choice: EquipmentList
 
 
 # Don't call like this CreateNodeEnrollmentForm() or you'll
 # get a vague error.
 user_input = yield CreateNodeEnrollmentForm
 ```
 
-It has a read only ORG ID and exposes a list of devices pulled from ESDB for the user to choose from.
+The only real data gathered with this form are `customer_id`, which is read-only, so the user cannot modify it, and the form exposes a list of devices pulled from a network inventory system for the user to choose from.
 
-### Choice widgets
+#### Choice Widgets
 
-Of note: `min_items` and `max_items` do not refer to the number of elements in the list. This UI construct allows for an arbitrary number of choices to be made - there are `+` and `-` options exposed in the UI allowing for multiple choices selected by the user. So `min 1 / max 1` tells the UI to display one pull down list of choices one of which must be selected, and additional choices can not be added.
+Of note: `min_items` and `max_items` do not refer to the number of elements in the list. This UI construct allows for an arbitrary number of choices to be made. There are `+` and `-` options exposed in the UI allowing for multiple choices selected by the user. So `min 1 / max 1` tells the UI to display one pull down list of choices one of which must be selected, and additional choices can not be added.
 
 If one defined something like `min 1 / max 3` it would display one pulldown box by default and expose a `+` element in the UI. The user could click on it to arbitrarily add a second or a third pulldown list. `min 0` would not display any list by default but the user could use `+` to add some, etc.
 
 Since multiple choices are allowed, the results are returned as a list even if there is only a single choice element:
 
 ```python
 eq_name = user_input.select_node_choice[0]
 ```
 
-The `zip()` maneuver takes the list and makes it into a dict with the same keys and values. So the display text doesn't have to be the same as the value returned.
+The `zip()` maneuver takes the list and makes it into a dict with the same keys and values so that the display text doesn't have to be the same as the value returned.
 
-### Accept actions
+#### Accept Actions
 
-Confirming actions is a common bit of functionality. This bit of code displays some read only NSO payload and lets the user ok the dry run:
+Confirming actions is a common bit of functionality. This bit of code displays a read only payload from an external system, lets the user check that value and then approve that the payload is correct as a form of a dry run:
 
 ```python
 from orchestrator.forms import FormPage, ReadOnlyField
 from orchestrator.forms.validators import Accept, LongText
 
 
 def confirm_dry_run_results(dry_run_results: str) -> State:
@@ -74,15 +80,15 @@
         confirm_dry_run_results: Accept
 
     user_input = yield ConfirmDryRun
 
     return user_input
 ```
 
-### Generic python types
+#### Generic Python Types
 
 It is possible to mix generic python types in the with the defined validation fields:
 
 ```python
 class CreateLightPathForm(FormPage):
     class Config:
         title = product_name
@@ -92,52 +98,55 @@
     ticket_id: JiraTicketId = ""  # type: ignore
     service_ports: ListOfTwo[ServicePort]  # type: ignore
     service_speed: bandwidth("service_ports")  # type: ignore # noqa: F821
     speed_policer: bool = False
     remote_port_shutdown: bool = True
 ```
 
-### Multi step form input
+#### Multi-step Form Input
 
-Similar to the original "list based" form `Input` elements, to do a multistep form flow yield multiple times and then combine the results at the end:
+To do a multistep form in your workflow, you simply yield multiple times and then combine the results at the end:
 
 ```python
 def initial_input_form_generator(product: UUIDstr, product_name: str) -> FormGenerator:
     class CreateNodeForm(FormPage):
         class Config:
             title = product_name
 
         customer_id: CustomerId = ReadOnlyField(CustomerId(SURFNET_NETWORK_UUID))
         location_code: LocationCode
         ticket_id: JiraTicketId = ""  # type:ignore
 
     user_input = yield CreateNodeForm
 
-    class NodeIdForm(FormPage):
+    class NodeIdForm(SubmitFormPage):
         class Config:
             title = product_name
 
         ims_node_id: ims_node_id(
             user_input.location_code, node_status="PL"
         )  # type:ignore # noqa: F821
 
     user_input_node = yield NodeIdForm
 
     return {**user_input.dict(), **user_input_node.dict()}
 ```
 
-## custom form field
+For multistep forms especially, it can be useful to use the `orchestrator.forms.SubmitFormPage` class, which is just a subclass of `orchestrator.forms.FormPage` that has some metadata informing the frontend that this form is the last page in the flow so it can style the submit button differently. This is entirely optional.
+
+### Custom Form Fields
 
 You can create a custom field component in the frontend. The components in `orchestrator-gui/src/lib/uniforms-surfnet/src` can be used to study reference implementations for a couple of custom form field types.
 
 For it to show up in the form, you have to do 2 things, a pydantic type/class in the backend and add the component to the `AutoFieldLoader.tsx`.
 
 as an example I will create a custom field with name field and group select field.
 
-### pydantic type/class in backend
+
+#### Pydantic Type/Class In Backend
 
 Create a pydantic type/class.
 
 ``` python
 from uuid import UUID
 
 
@@ -183,15 +192,15 @@
             title = product_name
 
         user: user_choice("group_id_1") = "user_id_1"
 
     user_input = yield ChoseUserForm
 ```
 
-### auto field loader
+#### Auto Field Loader
 
 The auto field loader is for loading the correct field component in the form.
 It has switches that check the field type and the field format.
 You have to add your new form field here.
 
 for this example, we would need to add to a `ChooseUser` case to the String switch:
 
@@ -215,15 +224,15 @@
     }
 
     ...
 }
 
 ```
 
-### custom field example
+#### Custom Field Example
 
 example custom field to select a user by group.
 
 ``` js
 import { EuiFlexItem, EuiFormRow, EuiText } from "@elastic/eui";
 import { FieldProps } from "lib/uniforms-surfnet/src/types";
 import React, { useCallback, useContext, useEffect, useState } from "react";
@@ -423,9 +432,7 @@
             </section>
         </EuiFlexItem>
     );
 }
 
 export default connectField(injectIntl(ChoosePerson), { kind: "leaf" });
 ```
-
-## TBA
```

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/graphql.md` & `orchestrator_core-2.3.0rc1/docs/reference-docs/graphql.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,10 @@
 # GraphQL documentation
 
-- [Extending the Query and Mutation](#extending-the-query-and-mutation)
-- [Add Json schema for metadata](#add-json-schema-for-metadata)
-- [Domain Models Auto Registration for GraphQL](#domain-models-auto-registration-for-graphql)
-  - [Scalars for Auto Registration](#scalars-for-auto-registration)
-  - [Federating with Autogenerated Types](#federating-with-autogenerated-types)
-    - [Federating with Specific Subscriptions](#federating-with-specific-subscriptions)
-    - [Federating with Specific Subscription Product Blocks](#federating-with-specific-subscription-product-blocks)
-  - [Usage of USE_PYDANTIC_ALIAS_MODEL_MAPPING](#usage-of-use_pydantic_alias_model_mapping)
-- [Overriding types](#overriding-types)
-  - [Overriding CustomerType and Resolvers](#overriding-customertype-and-resolvers)
-    - [CustomerType Override](#customertype-override)
-    - [CustomerType Resolver Override](#customertype-resolver-override)
-    - [CustomerType Related Type Overrides](#customertype-related-type-overrides)
-
-OrchestratorCore comes with a graphql interface that can to be registered after you create your OrchestratorApp.
+The `orchestrator-core` comes with a graphql interface that can to be registered after you create your OrchestratorApp.
 If you add it after registering your `SUBSCRIPTION_MODEL_REGISTRY` it will automatically create graphql types for them.
 
 example:
 
 ```python
 app = OrchestratorCore(base_settings=AppSettings())
 # register SUBSCRIPTION_MODEL_REGISTRY
```

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/python.md` & `orchestrator_core-2.3.0rc1/docs/reference-docs/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/scaling.md` & `orchestrator_core-2.3.0rc1/docs/reference-docs/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/tasks.md` & `orchestrator_core-2.3.0rc1/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/websockets.md` & `orchestrator_core-2.3.0rc1/docs/reference-docs/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/application/workflow.md` & `orchestrator_core-2.3.0rc1/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/context.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/context.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/introduction.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/ip_static.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/ip_static.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/ip_static.png` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/ip_static.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_point_to_point.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.png` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_point_to_point.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_vpn.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_vpn.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_vpn.png` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_vpn.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/modelling.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/modelling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/node.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/node.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/node.png` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/node.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/port.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/port.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/port.png` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/port.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/product_block_graph.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/product_block_graph.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/product_block_graph.png` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/product_block_graph.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/standards.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/standards.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/terminology.md` & `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/terminology.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/architecture/tldr.md` & `orchestrator_core-2.3.0rc1/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/contributing/guidelines.md` & `orchestrator_core-2.3.0rc1/docs/contributing/guidelines.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Contributing
 The workflow orchestrator projects welcomes any contributions from any party. If you are interested in contributing
 or have questions about the project please contact the board: workfloworchestrator.board@commonsconservancy.org or feel
 free to raise an issue in the project. We will strive to reply to your enquiry A.S.A.P.
 
 ## Documentation
-We use [**MKDOCS**](https://www.mkdocs.org) as a documentation tool. Please create a PR if you have any additions or
-contributions to make. All docs can be written in MD or html.
+We use [**MKDOCS**](https://www.mkdocs.org) as a documentation tool. Please create a PR if you have any additions or contributions to make. All docs can be written in MD or html. Full guidelines on how to set this up can be found [here](documentation.md).
 
 ## Orchestrator release
 The `orchestrator-core` has no release schedule but is actively used and maintained by the workflow orchestrator group.
 Creating a new release is done by the developers of the project and the procedure is as follows.
 
 ### Release candidates
 When creating new features they can be released in so-called `pre-releases` on github. Depending on the feature type the
```

### Comparing `orchestrator_core-2.2.2rc2/docs/contributing/testing.md` & `orchestrator_core-2.3.0rc1/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/css/style.css` & `orchestrator_core-2.3.0rc1/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/css/termynal.css` & `orchestrator_core-2.3.0rc1/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/getting-started/base.md` & `orchestrator_core-2.3.0rc1/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/getting-started/development.md` & `orchestrator_core-2.3.0rc1/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/getting-started/prepare-source-folder.md` & `orchestrator_core-2.3.0rc1/docs/getting-started/prepare-source-folder.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/img/WFO-Emblem-White.png` & `orchestrator_core-2.3.0rc1/docs/img/WFO-Emblem-White.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/img/favicon.ico` & `orchestrator_core-2.3.0rc1/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/index.md` & `orchestrator_core-2.3.0rc1/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     <a href="https://pypi.org/project/orchestrator-core" target="_blank">
     <img src="https://img.shields.io/pypi/v/orchestrator-core?color=%2334D058&label=pypi%20package" alt="Pypi">
     </a>
 </p>
 <br>
 <br>
 __The orchestrator core is a project developed by [SURF](https://www.surf.nl) to facilitate the orchestration of services.
-Together with [ESnet](https://www.es.net) this project has been opensourced in [the commons conservancy](https://commonsconservancy.org)
+Together with [ESnet](https://www.es.net) this project has been open-sourced in [the commons conservancy](https://commonsconservancy.org)
 to help facilitate collaboration. We invite all who are interested to take a look and to contribute!__
 
 ## Orchestration
 When do you orchestrate and when do you automate? The answer is you probably need both. Automation helps you execute repetitive
 tasks reliably and easily, Orchestration adds a layer and allows you to add more intelligence to the tasks you need to automate and
 to have a complete audit log of changes.
 
@@ -59,19 +59,19 @@
         >> arbitrary_step_func_1
         >> arbitrary_step_func_2
         >> arbitrary_step_func_3
         >> done
     )
 ```
 
-## I'm conviced! Show me more!
+## I'm convinced! Show me more!
 
 There are a number of options for getting started:
 
 - For those of you who would like to see it working, take a look at [this repo](https://github.com/workfloworchestrator/example-orchestrator) and follow the README to setup a
   docker-compose so you can experiment on your localhost.
-- For those who are more adventurous, follow the guide on the [next page](/orchestrator-core/getting-started/base) to
-  start codeing right away.
+- For those who are more adventurous, follow the guide on the [next page](getting-started/base.md) to
+  start coding right away.
 
 [//]: # (- If you would like to see the workflow engine in action, click [here]&#40;https://demo.workfloworchestrator.org&#41; this )
 
 [//]: # (will take you to our demo environment, where you can see some of our examples in action.)
```

### Comparing `orchestrator_core-2.2.2rc2/docs/js/custom.js` & `orchestrator_core-2.3.0rc1/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/js/termynal.js` & `orchestrator_core-2.3.0rc1/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/migration-guide/2.0.md` & `orchestrator_core-2.3.0rc1/docs/migration-guide/2.0.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/advanced/circuit-workflow.md` & `orchestrator_core-2.3.0rc1/docs/workshops/advanced/circuit-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/advanced/docker-installation.md` & `orchestrator_core-2.3.0rc1/docs/workshops/advanced/docker-installation.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/advanced/domain-models.md` & `orchestrator_core-2.3.0rc1/docs/workshops/advanced/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/advanced/node-workflow.md` & `orchestrator_core-2.3.0rc1/docs/workshops/advanced/node-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/advanced/overview.md` & `orchestrator_core-2.3.0rc1/docs/workshops/advanced/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/advanced/scenario.md` & `orchestrator_core-2.3.0rc1/docs/workshops/advanced/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/advanced/workflow-introduction.md` & `orchestrator_core-2.3.0rc1/docs/workshops/advanced/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/create-user.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/database-migration.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/debian.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/docker.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/domain-models.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/domain-models.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Domain models
 
 ## Introduction
 
-First read the [Architecture; TLDR](/orchestrator-core/architecture/tldr/)
+First read the [Architecture; TL;DR](/orchestrator-core/architecture/tldr/)
 section of the orchestrator core documentation to get an overview of the
 concepts that will be covered.
 
 To put a part of the terminology in context, products are modeled using a set
 of product blocks. The product attributes are modeled by resource types.  By
 default all resource types are mutable and can be changed over the lifetime of
 a subscription. Fixed inputs are used to model immutable attributes.
```

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/explore.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/input-forms.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/macos.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/modify-user.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/overview.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/scenario.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/start-applications.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-2.3.0rc1/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/images/metadata_products.png` & `orchestrator_core-2.3.0rc1/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/docs/workshops/images/netbox_devices_active.png` & `orchestrator_core-2.3.0rc1/docs/workshops/images/netbox_devices_active.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/mutmut_config.py` & `orchestrator_core-2.3.0rc1/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "2.2.2rc2"
+__version__ = "2.3.0rc1"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/api.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,59 +13,36 @@
 
 """Module that implements process related API endpoints."""
 
 from fastapi.param_functions import Depends
 from fastapi.routing import APIRouter
 
 from orchestrator.api.api_v1.endpoints import (
-    fixed_input,
     health,
     processes,
-    product_blocks,
     products,
-    resource_types,
     settings,
     subscription_customer_descriptions,
     subscriptions,
     translations,
     user,
-    workflows,
     ws,
 )
 from orchestrator.security import opa_security_default
 
 api_router = APIRouter()
-api_router.include_router(
-    fixed_input.router,
-    prefix="/fixed_inputs",
-    tags=["Core", "Fixed Inputs"],
-    dependencies=[Depends(opa_security_default)],
-)
 
 api_router.include_router(
     processes.router, prefix="/processes", tags=["Core", "Processes"], dependencies=[Depends(opa_security_default)]
 )
 api_router.include_router(processes.ws_router, prefix="/processes", tags=["Core", "Processes"])
-
-api_router.include_router(
-    product_blocks.router,
-    prefix="/product_blocks",
-    tags=["Core", "Product Blocks"],
-    dependencies=[Depends(opa_security_default)],
-)
 api_router.include_router(
     products.router, prefix="/products", tags=["Core", "Product"], dependencies=[Depends(opa_security_default)]
 )
 api_router.include_router(
-    resource_types.router,
-    prefix="/resource_types",
-    tags=["Core", "Resource Types"],
-    dependencies=[Depends(opa_security_default)],
-)
-api_router.include_router(
     subscriptions.router,
     prefix="/subscriptions",
     tags=["Core", "Subscriptions"],
     dependencies=[Depends(opa_security_default)],
 )
 api_router.include_router(
     subscription_customer_descriptions.router,
@@ -73,17 +50,14 @@
     tags=["Core", "Subscription Customer Descriptions"],
     dependencies=[Depends(opa_security_default)],
 )
 api_router.include_router(
     user.router, prefix="/user", tags=["Core", "User"], dependencies=[Depends(opa_security_default)]
 )
 api_router.include_router(
-    workflows.router, prefix="/workflows", tags=["Core", "Workflows"], dependencies=[Depends(opa_security_default)]
-)
-api_router.include_router(
     settings.router, prefix="/settings", tags=["Core", "Settings"], dependencies=[Depends(opa_security_default)]
 )
 api_router.include_router(settings.ws_router, prefix="/settings", tags=["Core", "Settings"])
 api_router.include_router(health.router, prefix="/health", tags=["Core"])
 api_router.include_router(
     translations.router,
     prefix="/translations",
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/health.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,21 +7,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from http import HTTPStatus
+
 import structlog
 from fastapi.routing import APIRouter
+from sqlalchemy import select
+from sqlalchemy.exc import OperationalError
 
-from orchestrator.schemas import FixedInputConfigurationSchema
-from orchestrator.utils.fixed_inputs import fixed_input_configuration
-
-router = APIRouter()
+from orchestrator.api.error_handling import raise_status
+from orchestrator.db import ProductTable, db
 
 logger = structlog.get_logger(__name__)
 
+router = APIRouter()
+
 
-@router.get("/configuration", response_model=FixedInputConfigurationSchema)
-def get_fixed_input_configuration_schema() -> FixedInputConfigurationSchema:
-    return fixed_input_configuration()  # type: ignore
+@router.get("/", response_model=str)
+def get_health() -> str:
+    try:
+        stmt = select(ProductTable.name).limit(1)
+        db.session.execute(stmt)
+    except OperationalError as e:
+        logger.warning("Health endpoint returned: notok!")
+        logger.debug("Health endpoint error details", error=str(e))
+        raise_status(HTTPStatus.INTERNAL_SERVER_ERROR)
+    return "OK"
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_health.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,31 +8,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from http import HTTPStatus
+from unittest import mock
 
-import structlog
-from fastapi.routing import APIRouter
-from sqlalchemy import select
 from sqlalchemy.exc import OperationalError
 
-from orchestrator.api.error_handling import raise_status
-from orchestrator.db import ProductTable, db
 
-logger = structlog.get_logger(__name__)
+def test_get_health(test_client):
+    response = test_client.get("/api/health/")
+    assert HTTPStatus.OK == response.status_code
+    assert response.json() == "OK"
 
-router = APIRouter()
 
-
-@router.get("/", response_model=str)
-def get_health() -> str:
-    try:
-        stmt = select(ProductTable.name).limit(1)
-        db.session.execute(stmt)
-    except OperationalError as e:
-        logger.warning("Health endpoint returned: notok!")
-        logger.debug("Health endpoint error details", error=str(e))
-        raise_status(HTTPStatus.INTERNAL_SERVER_ERROR)
-    return "OK"
+@mock.patch("orchestrator.db.db.session")
+def test_get_health_no_connection(mock_session, test_client):
+    mock_session.execute.side_effect = OperationalError("THIS", "IS", "KABOOM")
+    response = test_client.get("/api/health/")
+    assert response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,34 +24,31 @@
 from fastapi.param_functions import Body, Depends, Header
 from fastapi.routing import APIRouter
 from fastapi.websockets import WebSocket
 from fastapi_etag.dependency import CacheHit
 from more_itertools import chunked
 from sentry_sdk.tracing import trace
 from sqlalchemy import CompoundSelect, Select, select
-from sqlalchemy.orm import contains_eager, defer, joinedload
+from sqlalchemy.orm import defer, joinedload
 from sqlalchemy.sql.functions import count
 from starlette.responses import Response
 
 from oauth2_lib.fastapi import OIDCUserModel
 from orchestrator.api.error_handling import raise_status
 from orchestrator.api.helpers import add_response_range
-from orchestrator.config.assignee import Assignee
 from orchestrator.db import ProcessSubscriptionTable, ProcessTable, SubscriptionTable, db
 from orchestrator.db.filters import Filter
 from orchestrator.db.filters.process import filter_processes
 from orchestrator.db.sorting import Sort, SortOrder
 from orchestrator.db.sorting.process import sort_processes
 from orchestrator.schemas import (
     ProcessIdSchema,
     ProcessResumeAllSchema,
     ProcessSchema,
     ProcessStatusCounts,
-    ProcessSubscriptionBaseSchema,
-    ProcessSubscriptionSchema,
     Reporter,
 )
 from orchestrator.security import oidc_user
 from orchestrator.services.process_broadcast_thread import api_broadcast_process_data
 from orchestrator.services.processes import (
     SYSTEM_USER,
     _async_resume_processes,
@@ -61,15 +58,14 @@
     load_process,
     resume_process,
     start_process,
 )
 from orchestrator.services.settings import get_engine_settings
 from orchestrator.settings import app_settings
 from orchestrator.types import JSON, State
-from orchestrator.utils.deprecation_logger import deprecated_endpoint
 from orchestrator.utils.enrich_process import enrich_process
 from orchestrator.websocket import WS_CHANNELS, send_process_data_to_websocket, websocket_manager
 from orchestrator.workflow import ProcessStatus
 
 router = APIRouter()
 
 logger = structlog.get_logger(__name__)
@@ -226,54 +222,14 @@
     try:
         abort_process(process, user, broadcast_func=broadcast_func)
         return
     except Exception as e:
         raise_status(HTTPStatus.INTERNAL_SERVER_ERROR, str(e))
 
 
-@router.get(
-    "/process-subscriptions-by-subscription-id/{subscription_id}",
-    response_model=list[ProcessSubscriptionSchema],
-    deprecated=True,
-    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
-    dependencies=[Depends(deprecated_endpoint)],
-)
-def process_subscriptions_by_subscription_id(subscription_id: UUID) -> list[ProcessSubscriptionSchema]:
-    stmt = (
-        select(ProcessSubscriptionTable)
-        .options(contains_eager(ProcessSubscriptionTable.process))
-        .join(ProcessTable)
-        .filter(ProcessSubscriptionTable.subscription_id == subscription_id)
-        .order_by(ProcessTable.started_at.asc())
-    )
-    return list(db.session.scalars(stmt))
-
-
-@router.get(
-    "/process-subscriptions-by-process_id/{process_id}",
-    response_model=list[ProcessSubscriptionBaseSchema],
-    deprecated=True,
-    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
-    dependencies=[Depends(deprecated_endpoint)],
-)
-def process_subscriptions_by_process_process_id(process_id: UUID) -> list[ProcessSubscriptionTable]:
-    return list(db.session.scalars(select(ProcessSubscriptionTable).filter_by(process_id=process_id)))
-
-
-@router.get(
-    "/statuses",
-    response_model=list[ProcessStatus],
-    deprecated=True,
-    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
-    dependencies=[Depends(deprecated_endpoint)],
-)
-def statuses() -> list[str]:
-    return [status.value for status in ProcessStatus]
-
-
 @router.get("/status-counts", response_model=ProcessStatusCounts)
 def status_counts() -> ProcessStatusCounts:
     """Retrieve status counts for processes and tasks."""
 
     stmt = (
         select(ProcessTable)
         .with_only_columns(ProcessTable.is_task, ProcessTable.last_status, count(ProcessTable.last_status))
@@ -282,25 +238,14 @@
     rows = db.session.execute(stmt).all()
     return ProcessStatusCounts(
         process_counts={status: num_processes for is_task, status, num_processes in rows if not is_task},
         task_counts={status: num_processes for is_task, status, num_processes in rows if is_task},
     )
 
 
-@router.get(
-    "/assignees",
-    response_model=list[Assignee],
-    deprecated=True,
-    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
-    dependencies=[Depends(deprecated_endpoint)],
-)
-def assignees() -> list[str]:
-    return [assignee.value for assignee in Assignee]
-
-
 @router.get("/{process_id}", response_model=ProcessSchema)
 def show(process_id: UUID) -> dict[str, Any]:
     process = _get_process(process_id)
     p = load_process(process)
 
     return enrich_process(process, p)
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/ws.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/error_handling.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from datetime import datetime
 from http import HTTPStatus
 from shlex import shlex
 from typing import Any
 from uuid import UUID
 
 from more_itertools import chunked
-from sqlalchemy import Select, String, cast, func, select
+from sqlalchemy import Select, func, select
 from sqlalchemy.sql import expression
 from starlette.responses import Response
 from structlog import get_logger
 
 from orchestrator.api.error_handling import raise_status
 from orchestrator.db import ProductTable, SubscriptionTable, db
 from orchestrator.db.models import SubscriptionSearchView
@@ -70,77 +70,14 @@
             if col:
                 query = query.order_by(order_by_expr(col))
             else:
                 raise_status(HTTPStatus.BAD_REQUEST, f"Unable to sort on unknown field: {item[0]}")
     return query
 
 
-def query_with_filters(  # noqa: C901
-    stmt: Select,
-    sort: list[str] | None = None,
-    filters: list[str] | None = None,
-) -> Select:
-    if filters is not None:
-        for filter_ in chunked(filters, 2):
-            if filter_ and len(filter_) == 2:
-                field = filter_[0]
-                value = filter_[1]
-                value_as_bool = value.lower() in ("yes", "y", "ye", "true", "1", "insync")
-                if value is not None:
-                    if field.endswith("_gt"):
-                        stmt = stmt.filter(SubscriptionTable.__dict__[field[:-3]] > value)
-                    elif field.endswith("_gte"):
-                        stmt = stmt.filter(SubscriptionTable.__dict__[field[:-4]] >= value)
-                    elif field.endswith("_lte"):
-                        stmt = stmt.filter(SubscriptionTable.__dict__[field[:-4]] <= value)
-                    elif field.endswith("_lt"):
-                        stmt = stmt.filter(SubscriptionTable.__dict__[field[:-3]] < value)
-                    elif field.endswith("_ne"):
-                        stmt = stmt.filter(SubscriptionTable.__dict__[field[:-3]] != value)
-                    elif field == "insync":
-                        stmt = stmt.filter(SubscriptionTable.insync.is_(value_as_bool))
-                    elif field == "tags":
-                        # For node and port selector form widgets
-                        sub_values = value.split("-")
-                        stmt = stmt.filter(func.lower(ProductTable.tag).in_([s.lower() for s in sub_values]))
-                    elif field == "tag":
-                        # For React table 7
-                        sub_values = value.split("-")
-                        stmt = stmt.filter(func.lower(ProductTable.tag).in_([s.lower() for s in sub_values]))
-                    elif field == "product":
-                        sub_values = value.split("-")
-                        stmt = stmt.filter(func.lower(ProductTable.name).in_([s.lower() for s in sub_values]))
-                    elif field == "status":
-                        # For React table 7
-                        statuses = value.split("-")
-                        stmt = stmt.filter(SubscriptionTable.status.in_([s.lower() for s in statuses]))
-                    elif field == "statuses":
-                        # For port subscriptions
-                        sub_values = value.split("-")
-                        stmt = stmt.filter(SubscriptionTable.status.in_([s.lower() for s in sub_values]))
-                    elif field == "organisation" or field == "customer" or field == "customer_id":
-                        stmt = stmt.filter(SubscriptionTable.customer_id == value)
-                    elif field == "tsv":
-                        # Quote key:value tokens. This will use the FOLLOWED BY operator (https://www.postgresql.org/docs/13/textsearch-controls.html)
-                        processed_text_query = _process_text_query(value)
-
-                        logger.debug("Running full-text search query:", value=processed_text_query)
-                        # TODO: Make 'websearch_to_tsquery' into a sqlalchemy extension
-                        stmt = stmt.join(SubscriptionSearchView).filter(
-                            func.websearch_to_tsquery("simple", processed_text_query).op("@@")(
-                                SubscriptionSearchView.tsv
-                            )
-                        )
-
-                    elif field in SubscriptionTable.__dict__:
-                        stmt = stmt.filter(cast(SubscriptionTable.__dict__[field], String).ilike("%" + value + "%"))
-
-    return _add_sort_to_query(stmt, sort)
-
-
 def add_response_range(
     stmt: Selectable, range_: list[int] | None, response: Response, unit: str = "items"
 ) -> Selectable:
     if range_ is not None and len(range_) == 2:
         total = db.session.scalar(select(func.count()).select_from(stmt.subquery()))
         range_start, range_end = range_
         try:
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/api/models.py` & `orchestrator_core-2.3.0rc1/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/app.py` & `orchestrator_core-2.3.0rc1/orchestrator/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 #!/usr/bin/env python3
+"""The main application module.
 
-# Copyright 2019-2020 SURF.
+This module contains the main `OrchestratorCore` class for the `FastAPI` backend and
+provides the ability to run the CLI.
+"""
+
+# Copyright 2019-2020 SURF, ESnet
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/database.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2020 SURF.
+# Copyright 2019-2020 SURF, ESnet
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -56,19 +56,22 @@
 @app.command(
     help="Initialize an empty migrations environment. This command will throw an exception when it detects conflicting files and directories."
 )
 def init() -> None:
     """Initialize the `migrations` directory.
 
     This command will initialize a migration directory for the orchestrator core application and setup a correct
-    migration environment.
+    migration environment. It will also throw an exception when it detects conflicting files and directories.
 
     Returns:
         None
 
+    CLI Options:
+        None
+
     """
 
     if os.access(migration_dir, os.F_OK) and os.listdir(migration_dir):
         raise OSError(f"Directory {migration_dir} already exists and is not empty")
 
     logger.info("Creating directory", directory=os.path.abspath(migration_dir))
     os.makedirs(migration_dir)
@@ -102,99 +105,150 @@
             alembic_ini.write(template.render(migrations_dir=migration_dir))
     else:
         logger.info("Skipping Alembic.ini file. It already exists")
 
 
 @app.command(help="Get the database heads")
 def heads() -> None:
+    """The `heads` command command shows the Alembic database heads.
+
+    CLI Options:
+        None
+
+    """
     command.heads(alembic_cfg())  # type: ignore[no-untyped-call]
 
 
 @app.command(help="Merge database revisions.")
 def merge(
     revisions: str = typer.Argument(default=None, help="Add the revision you would like to merge to this command."),
     message: str = typer.Option(None, "--message", "-m", help="The revision message"),
 ) -> None:
     """Merge database revisions.
 
+    It is possible when using multiple git branches in your WFO development lifecycle to have
+    multiple Alembic heads emerge. This command will allow you to merge those two (or more)
+    heads to resolve the issue. You also might need to run this after updating your version
+    of orchestrator-core if there have been schema changes.
+
+    [Read More Here](https://alembic.sqlalchemy.org/en/latest/branches.html#merging-branches)
+
     Args:
         revisions: List of revisions to merge
         message: Optional message for the revision.
 
     Returns:
         None
 
+    CLI Options:
+        ```sh
+        Arguments:
+            [REVISIONS]  Add the revision you would like to merge to this command.
+
+        Options:
+            -m, --message TEXT  The revision message
+        ```
     """
     command.merge(alembic_cfg(), revisions, message=message)
 
 
 @app.command()
 def upgrade(revision: str = typer.Argument(default=None, help="Rev id to upgrade to")) -> None:
-    """Upgrade the database.
+    """The `upgrade` command will upgrade the database to the specified revision.
 
     Args:
         revision: Optional argument to indicate where to upgrade to.
 
     Returns:
         None
 
+    CLI Options:
+        ```sh
+        Arguments:
+            [REVISION]  Rev id to upgrade to
+
+        Options:
+            --help  Show this message and exit.
+        ```
+
     """
     command.upgrade(alembic_cfg(), revision)
 
 
 @app.command()
-def downgrade(revision: str = typer.Argument("-1", help="Rev id to upgrade to")) -> None:
-    """Downgrade the database.
+def downgrade(revision: str = typer.Argument("-1", help="Rev id to downgrade to")) -> None:
+    """The `downgrade` command will downgrade the database to the previous revision or to the optionally specified revision.
 
     Args:
-        revision: Optional argument to indicate where to downgrade to.
+        revision (str, optional): Optional argument to indicate where to downgrade to. [default: -1]
 
     Returns:
         None
 
+    CLI Options:
+        ```sh
+        Arguments:
+            [REVISION]  Rev id to upgrade to  [default: -1]
+        ```
+
     """
     command.downgrade(alembic_cfg(), revision)
 
 
 @app.command()
 def revision(
     message: str = typer.Option(None, "--message", "-m", help="The revision message"),
     version_path: str = typer.Option(None, "--version-path", help="Specify specific path from config for version file"),
     autogenerate: bool = typer.Option(False, help="Detect schema changes and add migrations"),
     head: str = typer.Option(None, help="Determine the head you need to add your migration to."),
 ) -> None:
-    """Create a new revision file.
+    """The `revision` command creates a new Alembic revision file.
 
     Args:
         message: The revision message
         version_path: Specify specific path from config for version file
         autogenerate: Whether to detect schema changes.
         head: To which head the migration applies
 
     Returns:
         None
 
+    CLI Options:
+        ```sh
+        Options:
+            -m, --message TEXT              The revision message
+            --version-path TEXT             Specify specific path from config for version file
+            --autogenerate / --no-autogenerate
+                                            Detect schema changes and add migrations [default: no-autogenerate]
+            --head TEXT                     Determine the head you need to add your migration to.
+        ```
     """
     command.revision(alembic_cfg(), message, version_path=version_path, autogenerate=autogenerate, head=head)
 
 
 @app.command()
 def history(
     verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose output"),
     indicate_current: bool = typer.Option(False, "--current", "-c", help="Indicate current revision"),
 ) -> None:
-    """List changeset scripts in chronological order.
+    """The `history` command lists Alembic revision history/changeset scripts in chronological order.
 
     Args:
-        verbose: Verbose output
-        indicate_current: Indicate current revision
+        verbose (bool, optional): Verbose output
+        indicate_current (bool, optional): Indicate current revision
 
     Returns:
         None
 
+    CLI Options:
+        ```sh
+        Options:
+            -v, --verbose  Verbose output
+            -c, --current  Indicate current revision
+        ```
     """
     command.history(alembic_cfg(), verbose=verbose, indicate_current=indicate_current)
 
 
 @app.command(help="Create revision based on diff_product_in_database.")
 def migrate_domain_models(
     message: str = typer.Argument(..., help="Migration name"),
@@ -265,27 +319,39 @@
 
 
 @app.command(help="Create migration file based on diff workflows in db")
 def migrate_workflows(
     message: str = typer.Argument(..., help="Migration name"),
     test: bool = typer.Option(False, help="Optional boolean if you don't want to generate a migration file"),
 ) -> tuple[list[dict], list[dict]] | None:
-    """Create a migration file based on the difference between workflows in the database and registered WorkflowInstances. BACKUP DATABASE BEFORE USING THE MIGRATION!.
+    """The `migrate-workflows` commanad creates a migration file based on the difference between workflows in the database and registered WorkflowInstances in your codebase.
+
+    !!! warning "BACKUP YOUR DATABASE BEFORE USING THE MIGRATION!"
 
     You will be prompted with inputs for new models and resource type updates.
     Resource type updates are only handled when it's renamed in all product blocks.
 
     Args:
         message: Message/description of the generated migration.
         test: Optional boolean if you don't want to generate a migration file.
 
     Returns None unless `--test` is used, in which case it returns:
         - tuple:
             - list of upgrade SQL statements in string format.
             - list of downgrade SQL statements in string format.
+
+    CLI Arguments:
+        ```sh
+        Arguments:
+            MESSAGE  Migration name  [required]
+
+        Options:
+            --test / --no-test  Optional boolean if you don't want to generate a migration
+            file  [default: no-test]
+        ```
     """
     if not app_settings.TESTING:
         init_database(app_settings)
 
     if test:
         print(  # noqa: T001, T201
             f"{str_fmt('NOTE:', flags=[COLOR.BOLD, COLOR.CYAN])} Running in test mode. No migration file will be generated.\n"
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generate.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/enums.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/migration.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/product.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/product_block.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/settings.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/translations.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/unittest.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/unittest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/validations.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/validations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/workflow.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/circuit.yaml` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/circuit.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/node.yaml` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/node.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/user.yaml` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/user.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/create_product.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/create_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/lazy_workflow_instance.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/macros.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/modify_product.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/modify_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/new_product_migration.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/new_product_migration.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/product.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/product_block.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/product_block.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/shared_forms.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/shared_forms.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/shared_workflows.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/shared_workflows.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/terminate_product.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/terminate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_create_workflow.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_create_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_product_type.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_product_type.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/validate_product.j2` & `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/validate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/main.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/migration_helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/cli/scheduler.py` & `orchestrator_core-2.3.0rc1/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/config/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/config/assignee.py` & `orchestrator_core-2.3.0rc1/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/database.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/filters/filters.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/filters/filters.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/filters/process.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/filters/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/filters/product.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/filters/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/filters/product_block.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/filters/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/filters/resource_type.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/filters/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/filters/search_filters/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/filters/search_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/filters/search_filters/inferred_filter.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/filters/search_filters/inferred_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/filters/subscription.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/filters/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/filters/workflow.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/filters/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/models.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/range/range.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/process.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/product.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/product_block.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/resource_type.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/sorting.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/sorting.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/subscription.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/workflow.py` & `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/devtools/populator.py` & `orchestrator_core-2.3.0rc1/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/devtools/scripts/migrate_20.py` & `orchestrator_core-2.3.0rc1/orchestrator/devtools/scripts/migrate_20.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/distlock/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-2.3.0rc1/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/domain/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/domain/base.py` & `orchestrator_core-2.3.0rc1/orchestrator/domain/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2020 SURF.
+# Copyright 2019-2020 SURF, ESnet.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -438,48 +438,53 @@
     if product_blocks_types_in_model and isinstance(first(product_blocks_types_in_model), tuple):
         return one(product_blocks_types_in_model)
 
     return product_blocks_types_in_model
 
 
 class ProductBlockModel(DomainModel):
-    r"""Base class for all product block models.
+    r"""This is the base class for all product block models.
 
     This class should have been called SubscriptionInstanceModel.
 
     ProductTable Blocks are represented as dataclasses with pydantic runtime validation.
 
-    Different stages of a subscription lifecycle could require different product block definition. Mainly to support
-    mandatory fields when a subscription is active. To support this a lifecycle specific product block definition can
-    be created by subclassing the generic product block with keyword argument 'lifecycle' and overriding its fields.
+    Different stages of a subscription lifecycle could require different product block
+    definition.Mainly to support mandatory fields when a subscription is active. To support
+    this a lifecycle specific product block definition can be created by subclassing the
+    generic product block with keyword argument 'lifecycle' and overriding its fields.
 
-    All product blocks are related to a database ProductBlockTable object through the `product_block_name` that is given
-    as class keyword argument.
+    All product blocks are related to a database ProductBlockTable object through the `product_block_name`
+    that is given as class keyword argument.
 
     Define a product block:
-    >>> class BlockInactive(ProductBlockModel, product_block_name="Virtual Circuit"):
-    ...    int_field: Optional[int] = None
-    ...    str_field: Optional[str] = None
-
-    >>> class Block(BlockInactive, lifecycle=[SubscriptionLifecycle.ACTIVE]):
-    ...    int_field: int
-    ...    str_field: str
+
+        >>> class BlockInactive(ProductBlockModel, product_block_name="Virtual Circuit"):
+        ...    int_field: Optional[int] = None
+        ...    str_field: Optional[str] = None
+
+        >>> class Block(BlockInactive, lifecycle=[SubscriptionLifecycle.ACTIVE]):
+        ...    int_field: int
+        ...    str_field: str
 
     This example defines a product_block with two different contraints based on lifecycle. `Block` is valid only for `ACTIVE`
     And `BlockInactive` for all other states.
     `product_block_name` must be defined on the base class and need not to be defined on the others
 
-    Create a new empty product block
-    >>> example1 = BlockInactive()  # doctest:+SKIP
+    Create a new empty product block:
+
+        >>> example1 = BlockInactive()  # doctest: +SKIP
 
     Create a new instance based on a dict in the state:
-    >>> example2 = BlockInactive(**state)  # doctest:+SKIP
 
-    To retrieve a ProductBlockModel from the database.:
-    >>> BlockInactive.from_db(subscription_instance_id)  # doctest:+SKIP
+        >>> example2 = BlockInactive(**state)  # doctest:+SKIP
+
+    To retrieve a ProductBlockModel from the database:
+
+        >>> BlockInactive.from_db(subscription_instance_id)  # doctest:+SKIP
     """
 
     registry: ClassVar[dict[str, type["ProductBlockModel"]]] = {}  # pragma: no mutate
     __names__: ClassVar[set[str]] = set()
     product_block_id: ClassVar[UUID]
     description: ClassVar[str]
     tag: ClassVar[str]
@@ -706,18 +711,18 @@
         subscription_instance: SubscriptionInstanceTable | None = None,
         status: SubscriptionLifecycle | None = None,
     ) -> B:
         """Create a product block based on a subscription instance from the database.
 
         This function is similar to `from_subscription()`
 
-        >>> subscription_instance_id = KNOWN_UUID_IN_DB  # doctest:+SKIP
-        >>> si_from_db = db.SubscriptionInstanceTable.query.get(subscription_instance_id)  # doctest:+SKIP
-        >>> example3 = ProductBlockModel.from_db(subscription_instance=si_from_db)  # doctest:+SKIP
-        >>> example4 = ProductBlockModel.from_db(subscription_instance_id=subscription_instance_id)  # doctest:+SKIP
+            >>> subscription_instance_id = KNOWN_UUID_IN_DB  # doctest:+SKIP
+            >>> si_from_db = db.SubscriptionInstanceTable.query.get(subscription_instance_id)  # doctest:+SKIP
+            >>> example3 = ProductBlockModel.from_db(subscription_instance=si_from_db)  # doctest:+SKIP
+            >>> example4 = ProductBlockModel.from_db(subscription_instance_id=subscription_instance_id)  # doctest:+SKIP
         """
         # Fill values from actual subscription
         if subscription_instance_id:
             subscription_instance = db.session.get(SubscriptionInstanceTable, subscription_instance_id)
         if subscription_instance:
             subscription_instance_id = subscription_instance.subscription_instance_id
         assert subscription_instance_id  # noqa: S101
@@ -838,15 +843,17 @@
         subscription_instance.depends_on_block_relations = depends_on_block_relations
 
     def save(
         self, *, subscription_id: UUID, status: SubscriptionLifecycle
     ) -> tuple[list[SubscriptionInstanceTable], SubscriptionInstanceTable]:
         """Save the current model instance to the database.
 
-        This means saving the whole tree of subscription instances and separately saving all instance values for this instance.
+        This means saving the whole tree of subscription instances and separately saving all instance
+        values for this instance. This is called automatically when you return a subscription to the state
+        in a workflow step.
 
         Args:
             status: current SubscriptionLifecycle to check if all constraints match
             subscription_id: Optional subscription id needed if this is a new model
 
         Returns:
             List of saved instances
@@ -904,18 +911,20 @@
 
     @property
     def db_model(self) -> SubscriptionInstanceTable:
         return self._db_model
 
     @property
     def in_use_by(self) -> list[SubscriptionInstanceTable]:
+        """This provides a list of product blocks that depend on this product block."""
         return self._db_model.in_use_by
 
     @property
     def depends_on(self) -> list[SubscriptionInstanceTable]:
+        """This provides a list of product blocks that this product block depends on."""
         return self._db_model.depends_on
 
 
 class ProductModel(BaseModel):
     """Represent the product as defined in the database as a dataclass."""
 
     model_config = ConfigDict(validate_assignment=True, validate_default=True)
@@ -927,36 +936,41 @@
     tag: str
     status: ProductLifecycle
     created_at: datetime | None = None
     end_date: datetime | None = None
 
 
 class SubscriptionModel(DomainModel):
-    r"""Base class for all product subscription models.
+    r"""This is the base class for all product subscription models.
 
-    Define a subscription model:
-    >>> class SubscriptionInactive(SubscriptionModel, product_type="SP"):  # doctest:+SKIP
-    ...    block: Optional[ProductBlockModelInactive] = None
+    To use this class, see the examples below:
 
-    >>> class Subscription(BlockInactive, lifecycle=[SubscriptionLifecycle.ACTIVE]):  # doctest:+SKIP
-    ...    block: ProductBlockModel
+    Definining a subscription model:
 
+        >>> class SubscriptionInactive(SubscriptionModel, product_type="SP"):  # doctest:+SKIP
+        ...    block: Optional[ProductBlockModelInactive] = None
+
+        >>> class Subscription(BlockInactive, lifecycle=[SubscriptionLifecycle.ACTIVE]):  # doctest:+SKIP
+        ...    block: ProductBlockModel
 
     This example defines a subscription model with two different contraints based on lifecycle. `Subscription` is valid only for `ACTIVE`
     And `SubscriptionInactive` for all other states.
     `product_type` must be defined on the base class and need not to be defined on the others
 
-    Create a new empty subscription
-    >>> example1 = SubscriptionInactive.from_product_id(product_id, customer_id)  # doctest:+SKIP
+    Create a new empty subscription:
+
+        >>> example1 = SubscriptionInactive.from_product_id(product_id, customer_id)  # doctest:+SKIP
 
     Create a new instance based on a dict in the state:
-    >>> example2 = SubscriptionInactive(**state)  # doctest:+SKIP
+
+        >>> example2 = SubscriptionInactive(**state)  # doctest:+SKIP
 
     To retrieve a ProductBlockModel from the database:
-    >>> SubscriptionInactive.from_subscription(subscription_id)  # doctest:+SKIP
+
+        >>> SubscriptionInactive.from_subscription(subscription_id)  # doctest:+SKIP
     """
 
     product: ProductModel
     customer_id: str
     _db_model: SubscriptionTable = PrivateAttr()
     subscription_id: UUID = Field(default_factory=uuid4)  # pragma: no mutate
     description: str = "Initial subscription"  # pragma: no mutate
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/domain/customer_description.py` & `orchestrator_core-2.3.0rc1/orchestrator/domain/customer_description.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/domain/helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/domain/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/domain/lifecycle.py` & `orchestrator_core-2.3.0rc1/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/exception_handlers.py` & `orchestrator_core-2.3.0rc1/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/forms/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/forms/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,20 +6,31 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import ClassVar
 
-from pydantic_forms.core import DisplayOnlyFieldType, FormPage, generate_form, post_form
+from pydantic_forms.core import DisplayOnlyFieldType, generate_form, post_form
+from pydantic_forms.core import FormPage as PydanticFormsFormPage
 from pydantic_forms.types import JSON, InputForm, StateInputFormGenerator
 
 __all__ = [
     "DisplayOnlyFieldType",
     "FormPage",
+    "SubmitFormPage",
     "InputForm",
     "JSON",
     "StateInputFormGenerator",
     "generate_form",
     "post_form",
 ]
+
+
+class FormPage(PydanticFormsFormPage):
+    meta__: ClassVar[JSON] = {"hasNext": True}
+
+
+class SubmitFormPage(FormPage):
+    meta__: ClassVar[JSON] = {"hasNext": False}
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/customer_contact_list.py` & `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/customer_contact_list.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/customer_id.py` & `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/customer_id.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/display_subscription.py` & `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/display_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/network_type_validators.py` & `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/product_id.py` & `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/product_id.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/autoregistration.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/autoregistration.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from more_itertools import one
 from strawberry.experimental.pydantic.conversion_types import StrawberryTypeFromPydantic
 from strawberry.federation.schema_directives import Key
 from strawberry.unset import UNSET
 
 from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY
 from orchestrator.domain.base import DomainModel, get_depends_on_product_block_type_list
+from orchestrator.graphql.schemas.product_block import BaseProductBlockType
 from orchestrator.graphql.types import StrawberryModelType
 from orchestrator.types import filter_nonetype, is_of_type, is_optional_type
 from orchestrator.utils.helpers import to_camel
 
 logger = structlog.get_logger(__name__)
 
 EnumDict = dict[str, EnumMeta]
@@ -77,21 +78,25 @@
 ) -> type[StrawberryTypeFromPydantic[DomainModel]]:
     from strawberry.federation.schema_directives import Key
     from strawberry.unset import UNSET
 
     federation_key_directives = [Key(fields="subscriptionInstanceId", resolvable=UNSET)]
 
     if keys := [key for key in model.__annotations__.keys() if "_id" in key]:
-        federation_key_directives.extend([Key(fields=to_camel(key), resolvable=UNSET) for key in keys])
+        federation_key_directives.extend([Key(fields=to_camel(key), resolvable=True) for key in keys])
 
-    new_type = type(strawberry_name, (), {})
-    strawberry_wrapper = strawberry.experimental.pydantic.type(
-        model, name=strawberry_name, all_fields=True, directives=federation_key_directives
+    base_type = type(strawberry_name, (BaseProductBlockType,), {})
+    pydantic_wrapper = strawberry.experimental.pydantic.type(
+        model,
+        all_fields=True,
+        directives=federation_key_directives,
+        description=f"{strawberry_name} Type",
+        use_pydantic_alias=USE_PYDANTIC_ALIAS_MODEL_MAPPING.get(strawberry_name, True),
     )
-    return strawberry_wrapper(new_type)
+    return type(strawberry_name, (pydantic_wrapper(base_type),), {})
 
 
 def create_subscription_strawberry_type(strawberry_name: str, model: type[DomainModel], interface: type) -> type:
     base_type = type(strawberry_name, (interface,), {})
     directives = [Key(fields="subscriptionId", resolvable=UNSET)]
 
     pydantic_wrapper = strawberry.experimental.pydantic.type(
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/error_collector_extension.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/error_collector_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/error_handler_extension.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/error_handler_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/mutations/customer_description.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/mutations/customer_description.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/mutations/start_process.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/mutations/start_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/pagination.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/customer.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/product_block.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/resource_type.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/subscription.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/workflow.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/schema.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/schema.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/process.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/product.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     tag: strawberry.auto
     created_at: strawberry.auto
     end_date: strawberry.auto
     product_blocks: list[ProductBlock]
     fixed_inputs: list[FixedInput]
     workflows: list[Workflow]
 
+    @strawberry.field(description="Returns the product type")  # type: ignore
+    async def type(self) -> str:
+        return self.product_type
+
     @authenticated_field(description="Returns list of subscriptions of the product type")  # type: ignore
     async def subscriptions(
         self,
         info: OrchestratorInfo,
         filter_by: list[GraphqlFilter] | None = None,
         sort_by: list[GraphqlSort] | None = None,
         first: int = 10,
@@ -47,8 +51,10 @@
 
         filter_by_with_related_subscriptions = (filter_by or []) + [GraphqlFilter(field="product", value=self.name)]
         return await resolve_subscriptions(info, filter_by_with_related_subscriptions, sort_by, first, after)
 
 
 @strawberry.experimental.pydantic.type(model=ProductModel, all_fields=True)
 class ProductModelGraphql:
-    pass
+    @strawberry.field(description="Returns the product type")  # type: ignore
+    async def type(self) -> str:
+        return self.product_type  # type: ignore
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/resource_type.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/subscription.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/workflow.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/types.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/create_resolver_error_handler.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/create_resolver_error_handler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/get_subscription_product_blocks.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/get_subscription_product_blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from collections.abc import Generator
 from itertools import count
-from typing import Any
+from typing import TYPE_CHECKING, Annotated, Any
 from uuid import UUID
 
 import strawberry
 from pydantic.alias_generators import to_camel as to_lower_camel
 from strawberry.scalars import JSON
 
 from orchestrator.domain.base import SubscriptionModel
+from orchestrator.graphql.schemas.product_block import owner_subscription_resolver
 from orchestrator.services.subscriptions import build_extended_domain_model
 from orchestrator.utils.redis import from_redis
 
+if TYPE_CHECKING:
+    from orchestrator.graphql.schemas.subscription import SubscriptionInterface
+
 
 @strawberry.type
 class ProductBlockInstance:
     id: int
     parent: int | None
     subscription_instance_id: UUID
     owner_subscription_id: UUID
     in_use_by_relations: list[JSON]
     product_block_instance_values: JSON
+    subscription: (
+        Annotated["SubscriptionInterface", strawberry.lazy("orchestrator.graphql.schemas.subscription")] | None
+    ) = strawberry.field(
+        description="resolve to subscription of the product block", resolver=owner_subscription_resolver
+    )
 
 
 def is_product_block(candidate: Any) -> bool:
     if isinstance(candidate, dict):
         # TODO: also filter on tag (needs addition of tag in orchestrator endpoint)
         # NOTE: this crosses subscription boundaries. If needed we can add an additional filter to limit that.
         return candidate.get("owner_subscription_id", None)
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/is_query_detailed.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/override_class.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/to_graphql_result_page.py` & `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/to_graphql_result_page.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/alembic.ini` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/env.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py` & `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schedules/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-2.3.0rc1/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schedules/scheduling.py` & `orchestrator_core-2.3.0rc1/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-2.3.0rc1/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schedules/validate_products.py` & `orchestrator_core-2.3.0rc1/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-2.3.0rc1/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,67 +13,58 @@
 
 from orchestrator.schemas.engine_settings import (
     EngineSettingsBaseSchema,
     EngineSettingsSchema,
     GlobalStatusEnum,
     WorkerStatus,
 )
-from orchestrator.schemas.fixed_input import FixedInputConfigurationSchema, FixedInputSchema
+from orchestrator.schemas.fixed_input import FixedInputSchema
 from orchestrator.schemas.problem_detail import ProblemDetailSchema
 from orchestrator.schemas.process import (
     ProcessBaseSchema,
     ProcessIdSchema,
     ProcessResumeAllSchema,
     ProcessSchema,
     ProcessStatusCounts,
-    ProcessSubscriptionBaseSchema,
-    ProcessSubscriptionSchema,
     Reporter,
 )
-from orchestrator.schemas.product import ProductBaseSchema, ProductCRUDSchema, ProductSchema
-from orchestrator.schemas.product_block import ProductBlockBaseSchema, ProductBlockEnrichedSchema
+from orchestrator.schemas.product import ProductBaseSchema, ProductSchema
+from orchestrator.schemas.product_block import ProductBlockBaseSchema
 from orchestrator.schemas.resource_type import ResourceTypeBaseSchema, ResourceTypeSchema
 from orchestrator.schemas.subscription import SubscriptionDomainModelSchema, SubscriptionIdSchema, SubscriptionSchema
 from orchestrator.schemas.subscription_descriptions import (
     SubscriptionDescriptionBaseSchema,
     SubscriptionDescriptionSchema,
 )
 from orchestrator.schemas.workflow import (
     StepSchema,
     SubscriptionWorkflowListsSchema,
     WorkflowSchema,
-    WorkflowWithProductTagsSchema,
 )
 
 __all__ = (
     "EngineSettingsSchema",
     "EngineSettingsBaseSchema",
-    "FixedInputConfigurationSchema",
     "GlobalStatusEnum",
     "ProblemDetailSchema",
     "FixedInputSchema",
-    "ProductBlockEnrichedSchema",
     "ProductBlockBaseSchema",
-    "ProductCRUDSchema",
     "ProductBaseSchema",
     "ProductSchema",
-    "ProcessSubscriptionSchema",
     "ProcessResumeAllSchema",
     "ProcessBaseSchema",
     "ProcessSchema",
     "ProcessIdSchema",
-    "ProcessSubscriptionBaseSchema",
     "StepSchema",
+    "SubscriptionDomainModelSchema",
     "SubscriptionDescriptionBaseSchema",
     "SubscriptionDescriptionSchema",
     "SubscriptionSchema",
-    "SubscriptionDomainModelSchema",
     "SubscriptionWorkflowListsSchema",
     "SubscriptionIdSchema",
     "ResourceTypeSchema",
     "ResourceTypeBaseSchema",
     "WorkerStatus",
     "WorkflowSchema",
-    "WorkflowWithProductTagsSchema",
     "Reporter",
     "ProcessStatusCounts",
 )
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/base.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 
 from datetime import datetime
 
 from pydantic import BaseModel, ConfigDict
 
 
 class OrchestratorBaseModel(BaseModel):
-    # TODO #429 json_encoders is deprecated and will be removed in Pydantic 3.x
+    # Unable to refactor in a neat way without using an ugly recursive function. Leaving Pydantic v1 functionality intact
     model_config = ConfigDict(
         json_encoders={
             datetime: lambda dt: dt.timestamp(),
         }
     )
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/engine_settings.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/fixed_input.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/fixed_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,12 +35,7 @@
     model_config = ConfigDict(from_attributes=True)
 
 
 class FixedInputConfigurationItemSchema(OrchestratorBaseModel):
     name: str
     description: str
     values: list[str]
-
-
-class FixedInputConfigurationSchema(OrchestratorBaseModel):
-    fixed_inputs: list[FixedInputConfigurationItemSchema]
-    by_tag: TagConfig
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/problem_detail.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/process.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/process.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,28 +61,14 @@
     workflow_target: Target | None = None
     subscriptions: list[SubscriptionSchema]
     current_state: dict[str, Any] | None = None
     steps: list[ProcessStepSchema] | None = None
     form: dict[str, Any] | None = None
 
 
-class ProcessSubscriptionBaseSchema(OrchestratorBaseModel):
-    id: UUID
-    process_id: UUID
-    subscription_id: UUID
-    workflow_target: Target | None = None
-    created_at: datetime
-
-    model_config = ConfigDict(from_attributes=True)
-
-
-class ProcessSubscriptionSchema(ProcessSubscriptionBaseSchema):
-    process: ProcessBaseSchema
-
-
 class ProcessResumeAllSchema(OrchestratorBaseModel):
     count: int
 
 
 class ProcessStatusCounts(OrchestratorBaseModel):
     process_counts: dict[ProcessStatus, int]
     task_counts: dict[ProcessStatus, int]
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/resource_type.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/subscription.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/schemas/workflow.py` & `orchestrator_core-2.3.0rc1/orchestrator/schemas/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,14 @@
     workflow_id: UUID
     created_at: datetime
     steps: list[StepSchema] | None = None
 
     model_config = ConfigDict(from_attributes=True)
 
 
-class WorkflowWithProductTagsSchema(WorkflowBaseSchema):
-    product_tags: list[str]
-
-
 class WorkflowListItemSchema(OrchestratorBaseModel):
     name: str
     description: str | None = None
     reason: str | None = None
     usable_when: list[Any] | None = None
     status: str | None = None
     action: str | None = None
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/security.py` & `orchestrator_core-2.3.0rc1/orchestrator/security.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/celery.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/fixed_inputs.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/process_broadcast_thread.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/process_broadcast_thread.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/processes.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/products.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/resource_types.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/settings.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/subscriptions.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/tasks.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/translations.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/services/workflows.py` & `orchestrator_core-2.3.0rc1/orchestrator/services/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/settings.py` & `orchestrator_core-2.3.0rc1/orchestrator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/targets.py` & `orchestrator_core-2.3.0rc1/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/types.py` & `orchestrator_core-2.3.0rc1/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/crypt.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/datetime.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/deprecation_logger.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/deprecation_logger.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/docs.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/enrich_process.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/enrich_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/errors.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/fixed_inputs.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/functional.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/get_updated_properties.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/helpers.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/json.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/redis.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/search_query.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/search_query.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/state.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2020 SURF.
+# Copyright 2019-2020 SURF, ESnet
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -209,15 +209,16 @@
                     ) from key_error
     return arguments
 
 
 def inject_args(func: StepFunc) -> Callable[[State], State]:
     """Allow functions to specify values from the state dict as parameters named after the state keys.
 
-    .. note:: domain models are subject to special processing (see: :ref:`domain models processing
+    !!! note
+        Domain models are subject to special processing (see: :ref:`domain models processing
         <domain-models-processing>`)
 
     What this decorator does is better explained with an example than lots of text. So normally we do this::
 
         def load_initial_state_for_modify(state: State) -> State:
             customer_id = state["customer_id"]
             subscription_id = state["subscription_id"]
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/utils/strings.py` & `orchestrator_core-2.3.0rc1/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/version.py` & `orchestrator_core-2.3.0rc1/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/websocket/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-2.3.0rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-2.3.0rc1/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-2.3.0rc1/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflow.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/modify_note.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/modify_note.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from orchestrator.db import db
+from orchestrator.forms import SubmitFormPage
 from orchestrator.services import subscriptions
 from orchestrator.settings import app_settings
 from orchestrator.targets import Target
 from orchestrator.types import UUIDstr
 from orchestrator.utils.json import to_serializable
 from orchestrator.workflow import StepList, conditional, done, init, workflow
 from orchestrator.workflows.steps import cache_domain_models, store_process_subscription
 from orchestrator.workflows.utils import wrap_modify_initial_input_form
-from pydantic_forms.core import FormPage
 from pydantic_forms.types import FormGenerator
 from pydantic_forms.validators import LongText
 
 
 def initial_input_form(subscription_id: UUIDstr) -> FormGenerator:
     subscription = subscriptions.get_subscription(subscription_id)
     subscription_backup = {subscription_id: to_serializable(subscription)}
     old_note = subscription.note
 
-    class ModifyNoteForm(FormPage):
+    class ModifyNoteForm(SubmitFormPage):
         note: LongText = old_note
 
     user_input = yield ModifyNoteForm
     subscription.note = user_input.note
     db.session.add(subscription)
     return {
         "old_note": old_note,
```

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/steps.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/orchestrator/workflows/utils.py` & `orchestrator_core-2.3.0rc1/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/pyproject.toml` & `orchestrator_core-2.3.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,64 +36,64 @@
 ]
 dependencies = [
     "alembic==1.13.1",
     "anyio>=3.7.0",
     "click==8.*",
     "deprecated",
     "deepmerge==1.1.1",
-    "fastapi~=0.110.0",
+    "fastapi~=0.111.0",
     "fastapi-etag==0.4.0",
     "more-itertools~=10.2.0",
     "itsdangerous",
     "Jinja2==3.1.3",
     "orjson==3.10.0",
     "psycopg2-binary==2.9.9",
     "pydantic[email]~=2.5.1",
     "pydantic-settings~=2.2.1",
     "python-dateutil==2.8.2",
     "python-rapidjson>=1.9,<1.17",
     "pytz==2024.1",
     "redis==5.0.3",
     "schedule==1.1.0",
-    "sentry-sdk[fastapi]==1.44.0",
+    "sentry-sdk[fastapi]==2.0.1",
     "SQLAlchemy==2.0.29",
     "SQLAlchemy-Utils==0.41.2",
     "structlog",
-    "typer==0.12.0",
+    "typer==0.12.3",
     "uvicorn[standard]~=0.29.0",
     "nwa-stdlib~=1.7.0",
     "oauth2-lib~=1.5.0",
     "tabulate==0.9.0",
     "strawberry-graphql==0.210.0",
-    "pydantic-forms==1.0.2",
+    "pydantic-forms~=1.0.3",
     "ruff",
 ]
 
 description-file = "README.md"
 requires-python = ">=3.11,<3.13"
 
 [project.urls]
 Documentation = "https://workfloworchestrator.org/orchestrator-core/"
 Source = "https://github.com/workfloworchestrator/orchestrator-core"
 
 [project.optional-dependencies]
 celery = [
-    "celery~=5.3.1"
+    "celery~=5.4.0"
 ]
 
 test = [
     "apache-license-check",
     "black",
     "blinker",
     "deepdiff",
     "dirty-equals",
     "jsonref",
-    "mypy",
-    "pytest",
-    "pytest-asyncio==0.21.0",
+    "mypy==1.9",
+    "pytest==8.2.0",
+    "pytest-asyncio==0.21.2",
     "pytest-cov",
     "pytest-httpx",
     "pytest-xdist",
     "requests-mock",
     "sqlalchemy[mypy]",
     "urllib3-mock",
     "types-Deprecated",
@@ -114,14 +114,17 @@
     "types-PyYAML",
 ]
 doc = [
     "mkdocs",
     "mkdocs-material[imaging]",
     "mkdocs-render-swagger-plugin",
     "mkdocs-include-markdown-plugin",
+    "mkdocstrings[python]",
+    "mkdocs-open-in-new-tab",
+    "mkdocs-macros-plugin",
 ]
 dev = [
     "toml",
     "bumpversion",
     "mypy_extensions",
     "pre-commit",
     "pydocstyle",
@@ -169,14 +172,18 @@
     "crypt.py",
     "venv",
     ".venv",
     "docs",
     "test/unit_tests/cli/data/generate",
     "orchestrator/vendor",
 ]
+line-length = 120
+target-version = "py39"
+
+[tool.ruff.lint]
 ignore = [
     "C417",
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
@@ -190,32 +197,30 @@
     "N805",
     "B904",
     "N803",
     "N801",
     "N815",
     "N802",
 ]
-line-length = 120
 select = ["B", "C", "D", "E", "F", "I", "N", "RET", "S", "T", "W"]
-target-version = "py39"
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "orchestrator/api/*" = ["B008"]
 "orchestrator/cli/*" = ["B008"]
 "orchestrator/devtools/scripts/*" = ["S101", "T201"]
 "test/*" = ["S101", "B033", "N816", "N802"]
 "orchestrator/__init__.py" = ["E402"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-third-party = ["pynso", "pydantic"]
 known-first-party = [
     "migrations",
     "test",
     "nwastdlib",
     "oauth2_lib",
     "pydantic_forms",
```

### Comparing `orchestrator_core-2.2.2rc2/setup.cfg` & `orchestrator_core-2.3.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/setup.py` & `orchestrator_core-2.3.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/acceptance_tests/conftest.py` & `orchestrator_core-2.3.0rc1/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/acceptance_tests/test_test_product.py` & `orchestrator_core-2.3.0rc1/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_caching.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_helpers.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_models.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_processes.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_processes.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     ProcessTable,
     SubscriptionTable,
     db,
 )
 from orchestrator.services.processes import shutdown_thread_pool
 from orchestrator.services.settings import get_engine_settings
 from orchestrator.settings import app_settings
-from orchestrator.targets import Target
 from orchestrator.workflow import ProcessStatus, done, init, step, workflow
 from test.unit_tests.helpers import URL_STR_TYPE
 from test.unit_tests.workflows import WorkflowInstanceForTests
 
 test_condition = Condition()
 
 
@@ -251,44 +250,14 @@
     response = test_client.put(f"/api/processes/{started_process}/abort")
     assert HTTPStatus.NO_CONTENT == response.status_code
 
     aborted_process = test_client.get(f"/api/processes/{started_process}").json()
     assert "aborted" == aborted_process["last_status"]
 
 
-def test_process_subscription_by_subscription_id(test_client, started_process, generic_subscription_1):
-    response = test_client.get(f"/api/processes/process-subscriptions-by-subscription-id/{generic_subscription_1}")
-    assert HTTPStatus.OK == response.status_code
-    process_subscriptions = response.json()
-    assert 1 == len(process_subscriptions)
-    assert process_subscriptions[0]["subscription_id"].lower(), generic_subscription_1
-    assert process_subscriptions[0]["process_id"].lower(), started_process
-    assert process_subscriptions[0]["workflow_target"], Target.CREATE
-    assert process_subscriptions[0]["process"]["workflow_name"], "workflow_for_testing_processes_py"
-
-
-def test_process_subscription_by_process_id(test_client, started_process, generic_subscription_1):
-    response = test_client.get(f"/api/processes/process-subscriptions-by-process_id/{started_process}")
-    assert HTTPStatus.OK == response.status_code
-    process_subscriptions = response.json()
-    assert 1 == len(process_subscriptions)
-    assert process_subscriptions[0]["subscription_id"].lower(), generic_subscription_1
-    assert process_subscriptions[0]["workflow_target"], Target.CREATE
-
-
-def test_process_subscription_by_process_id_404(test_client):
-    response = test_client.get(f"/api/processes/process-subscriptions-by-process_id/{uuid4()}")
-    assert 0 == len(response.json())
-
-
-def test_process_subscription_by_subscription_id_404(test_client):
-    response = test_client.get(f"/api/processes/process-subscriptions-by-subscription-id/{uuid4()}")
-    assert 0 == len(response.json())
-
-
 def test_new_process_invalid_body(test_client, long_running_workflow):
     response = test_client.post(f"/api/processes/{long_running_workflow}", json=[{"wrong": "body"}])
     assert HTTPStatus.BAD_REQUEST == response.status_code
 
 
 def test_new_process_invalid_Content_Type(test_client):
     response = test_client.post("/api/processes/terminate_sn8_light_path")
@@ -466,24 +435,14 @@
     process = processes[0]
 
     assert len(process["subscriptions"]) == 1
     assert process["subscriptions"][0]["product"]["tag"] == "GEN1"
     assert process["subscriptions"][0]["product"]["name"] == "Product 1"
 
 
-def test_processes_assignees(test_client):
-    response = test_client.get("/api/processes/assignees")
-    assert HTTPStatus.OK == response.status_code
-
-
-def test_processes_statuses(test_client):
-    response = test_client.get("/api/processes/statuses")
-    assert HTTPStatus.OK == response.status_code
-
-
 def test_resume_all_processes(test_client, mocked_processes_resumeall):
     """Test resuming all processes."""
     response = test_client.put("/api/processes/resume-all")
     assert HTTPStatus.OK == response.status_code
     assert response.json()["count"] == 3
```

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_products.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_products.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from http import HTTPStatus
 from uuid import uuid4
 
 import pytest
-from sqlalchemy import delete, select
+from sqlalchemy import delete
 
 from orchestrator.db import (
     FixedInputTable,
     ProductBlockTable,
     ProductTable,
     ResourceTypeTable,
     SubscriptionInstanceTable,
     SubscriptionInstanceValueTable,
     SubscriptionTable,
     db,
 )
-from orchestrator.services.fixed_inputs import get_fixed_inputs
 from test.unit_tests.config import CITY_TYPE, DOMAIN, IMS_CIRCUIT_ID, PORT_SPEED, PORT_SUBSCRIPTION_ID, SERVICE_SPEED
 from test.unit_tests.fixtures.workflows import add_soft_deleted_workflows  # noqa: F401
 
 PRODUCT_ID = uuid4()
 MSP_PRODUCT_ID = uuid4()
 UNPROTECTED_MSP_SSP_ID = uuid4()
 PROTECTED_MSP_SSP_ID = uuid4()
@@ -167,83 +166,7 @@
     assert "1000" == expected_value
     assert "Ethernet" == product["product_blocks"][0]["name"]
 
 
 def test_product_by_id_404(seed, test_client):
     response = test_client.get(f"/api/products/{str(uuid4())}")
     assert HTTPStatus.NOT_FOUND == response.status_code
-
-
-def test_save(seed, test_client):
-    p_id = uuid4()
-    body = {
-        "product_id": p_id,
-        "name": "MSP_2",
-        "description": "MSP",
-        "product_type": "Port",
-        "tag": "Port",
-        "status": "active",
-        "fixed_inputs": [{"name": "help", "value": "val"}],
-        "product_blocks": [
-            {"name": "name", "description": "desc", "status": "active", "resource_types": [{"resource_type": "test"}]}
-        ],
-    }
-
-    fi = get_fixed_inputs()
-    response = test_client.post("/api/products/", json=body)
-    assert HTTPStatus.NO_CONTENT == response.status_code
-    products = test_client.get("/api/products").json()
-    assert 10 == len(products)
-
-    fi2 = get_fixed_inputs()
-    assert len(fi) + 1 == len(fi2)
-
-
-def test_delete(seed, test_client):
-    p_id = uuid4()
-    body = {
-        "product_id": p_id,
-        "name": "DEL",
-        "description": "DEL",
-        "product_type": "Port",
-        "tag": "Port",
-        "status": "active",
-    }
-    test_client.post("/api/products/", json=body)
-
-    response = test_client.delete(f"/api/products/{p_id}")
-    assert HTTPStatus.NO_CONTENT == response.status_code
-
-
-def test_delete_with_subscriptions(seed, test_client):
-    response = test_client.delete(f"/api/products/{PRODUCT_ID}")
-
-    assert HTTPStatus.BAD_REQUEST == response.status_code
-    assert f"Product {PRODUCT_ID} is used in Subscriptions: desc" == response.json()["detail"]
-
-
-def test_tags_all(seed, test_client):
-    response = test_client.get("/api/products/tags/all")
-
-    assert HTTPStatus.OK == response.status_code
-    tags = response.json()
-
-    tags_db = db.session.scalars(select(ProductTable.tag))
-    assert sorted(tags) == sorted(set(tags_db))
-
-
-def test_types_all(seed, test_client):
-    response = test_client.get("/api/products/types/all")
-
-    assert HTTPStatus.OK == response.status_code
-    types = response.json()
-    types_db = db.session.scalars(select(ProductTable.product_type))
-
-    assert sorted(types) == sorted(set(types_db))
-
-
-def test_statuses_all(seed, test_client):
-    response = test_client.get("/api/products/statuses/all")
-
-    assert HTTPStatus.OK == response.status_code
-    statuses = response.json()
-    assert {"active", "phase out", "pre production", "end of life"}.issubset(set(statuses))
```

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_settings.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_subscriptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from http import HTTPStatus
 from ipaddress import IPv4Address
 from os import getenv
 from unittest import mock
 from uuid import uuid4
 
 import pytest
-from redis import Redis
-from sqlalchemy import select
+from redis.client import Redis
 
 from nwastdlib.url import URL
+from orchestrator import app_settings
 from orchestrator.api.helpers import product_block_paths
 from orchestrator.db import (
     FixedInputTable,
     ProcessSubscriptionTable,
     ProcessTable,
     ProductBlockTable,
     ProductTable,
@@ -27,15 +27,14 @@
 from orchestrator.services.subscriptions import (
     RELATION_RESOURCE_TYPES,
     _generate_etag,
     build_extended_domain_model,
     get_subscription,
     unsync,
 )
-from orchestrator.settings import app_settings
 from orchestrator.targets import Target
 from orchestrator.utils.json import json_dumps, json_loads
 from orchestrator.utils.redis import to_redis
 from orchestrator.workflow import ProcessStatus
 from test.unit_tests.config import (
     IMS_CIRCUIT_ID,
     INTERNETPINNEN_PREFIX_SUBSCRIPTION_ID,
@@ -484,196 +483,14 @@
             PEER_GROUP_SUBSCRIPTION_ID,
         ]
     )
 
     return ip_prefix_product
 
 
-def test_subscriptions_all(seed, test_client):
-    product_fields = [
-        "name",
-        "created_at",
-        "description",
-        "end_date",
-        "status",
-        "product_type",
-        "product_id",
-        "tag",
-    ]
-    subscription_fields = [
-        "customer_id",
-        "description",
-        "status",
-        "end_date",
-        "insync",
-        "start_date",
-        "subscription_id",
-        "product",
-        "name",
-        "note",
-        "customer_descriptions",
-        "product_id",
-        "tag",
-    ]
-    response = test_client.get("/api/subscriptions/all")
-
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-    for item in response.json():
-        # Todo: determine if we want to let the test fail when extra fields are detected?
-        product = item["product"]
-        # test for extra fields in the response that are not listed in the YAML
-        assert set(product.keys()) == set(product_fields)
-        assert set(item.keys()) == set(subscription_fields)
-
-        # Check if all listed YAML fields are also available in Response
-        for field in product_fields:
-            assert field in product
-        for field in subscription_fields:
-            assert field in item
-
-
-def test_subscriptions_paginated(seed, test_client):
-    product_fields = [
-        "name",
-        "created_at",
-        "description",
-        "end_date",
-        "status",
-        "product_type",
-        "product_id",
-        "tag",
-    ]
-    subscription_fields = [
-        "customer_id",
-        "description",
-        "status",
-        "end_date",
-        "insync",
-        "start_date",
-        "subscription_id",
-        "product",
-        "name",
-        "note",
-        "customer_descriptions",
-        "product_id",
-        "tag",
-    ]
-    response = test_client.get("/api/subscriptions")
-
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-
-    response = test_client.get("/api/subscriptions/all")
-
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-    for item in response.json():
-        product = item["product"]
-        # test for extra fields in the response that are not listed in the YAML
-        assert set(product.keys()) == set(product_fields)
-        assert set(item.keys()) == set(subscription_fields)
-
-        # Check if all listed YAML fields are also available in Response
-        for field in product_fields:
-            assert field in product
-        for field in subscription_fields:
-            assert field in item
-
-
-def test_filtering_subscriptions(seed, test_client):
-    response = test_client.get("/api/subscriptions?filter=status,active")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 5
-
-    response = test_client.get("/api/subscriptions?filter=insync,no")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 2
-
-    response = test_client.get("/api/subscriptions?filter=insync,Y")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 5
-
-    response = test_client.get("/api/subscriptions?filter=insync,no,status,provisioning")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 1
-
-    response = test_client.get("/api/subscriptions?filter=status_gt,active")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 2
-
-    response = test_client.get("/api/subscriptions?filter=status_gte,active")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-
-    response = test_client.get("/api/subscriptions?filter=status_lt,initial")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 5
-
-    response = test_client.get("/api/subscriptions?filter=status_lte,initial")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 6
-
-    response = test_client.get("/api/subscriptions?filter=status,active,product,LightPathProduct")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 1
-
-    response = test_client.get("/api/subscriptions?filter=status,active,product,LightPathProduct-PortBProduct")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 2
-
-
-def test_sorting_subscriptions(seed, test_client):
-    response = test_client.get("/api/subscriptions?sort=status,asc")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-    assert response.json()[0]["status"] == "active"
-    assert response.json()[6]["status"] == "provisioning"
-
-    response = test_client.get("/api/subscriptions?sort=status,desc")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-    assert response.json()[0]["status"] == "provisioning"
-    assert response.json()[6]["status"] == "active"
-
-    response = test_client.get("/api/subscriptions?sort=tag,asc")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-    assert response.json()[0]["product"]["tag"] == "IP_PREFIX"
-    assert response.json()[6]["product"]["tag"] == "SP"
-
-    response = test_client.get("/api/subscriptions?sort=tag,desc")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-    assert response.json()[0]["product"]["tag"] == "SP"
-    assert response.json()[6]["product"]["tag"] == "IP_PREFIX"
-
-    response = test_client.get("/api/subscriptions?sort=product,asc")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-    assert response.json()[0]["product"]["name"] == "INVALID_PRODUCT"
-    assert response.json()[6]["product"]["name"] == "PortBProduct"
-
-    response = test_client.get("/api/subscriptions?sort=product,desc")
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 7
-    assert response.json()[0]["product"]["name"] == "PortBProduct"
-    assert response.json()[6]["product"]["name"] == "INVALID_PRODUCT"
-
-
-def test_range_subscriptions(seed, test_client):
-    response = test_client.get("/api/subscriptions?range=0,3")
-
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 3
-
-    response = test_client.get("/api/subscriptions?sort=status,asc&range=5,5")
-    assert response.status_code == HTTPStatus.BAD_REQUEST
-
-
 def test_insync_404(seed, test_client):
     response = test_client.get(f"/api/subscriptions/workflows/{str(uuid4())}")
     assert response.status_code == HTTPStatus.NOT_FOUND
 
 
 def test_insync_invalid_tagged(seed, test_client):
     response = test_client.get(f"/api/subscriptions/workflows/{INVALID_PORT_SUBSCRIPTION_ID}")
@@ -683,40 +500,14 @@
         "create": [],
         "modify": [],
         "terminate": [],
         "system": [],
     }
 
 
-def test_in_use_by_subscriptions(seed, test_client):
-    response = test_client.get(f"/api/subscriptions/in_use_by/{PORT_A_SUBSCRIPTION_ID}")
-    in_use_by_subs = response.json()
-    assert len(in_use_by_subs) == 1
-    assert SERVICE_SUBSCRIPTION_ID == in_use_by_subs[0]["subscription_id"]
-
-
-def test_subscriptions_for_in_used_by_ids(seed, test_client, caplog):
-    instance_id = str(db.session.scalar(select(SubscriptionInstanceTable)).subscription_instance_id)
-    response = test_client.post("/api/subscriptions/subscriptions_for_in_used_by_ids", json=[instance_id])
-    in_use_by_subs = response.json()
-    assert in_use_by_subs[instance_id]
-    assert in_use_by_subs[instance_id]["product"]["product_type"] == "IP_PREFIX"
-    assert "Not all subscription_instance_id's could be resolved." not in caplog.text
-
-
-def test_subscriptions_for_in_used_by_ids_with_wrong_instance_ids(seed, test_client, caplog):
-    response = test_client.post(
-        "/api/subscriptions/subscriptions_for_in_used_by_ids", json=["5373600d-c9ee-4ceb-96bd-1d3256baccec"]
-    )
-    in_use_by_subs = response.json()
-    assert len(in_use_by_subs) == 0
-    assert "Not all subscription_instance_id's could be resolved." in caplog.text
-    assert "[UUID('5373600d-c9ee-4ceb-96bd-1d3256baccec')]" in caplog.text
-
-
 def test_in_use_by_subscriptions_not_insync(seed, test_client):
     # ensure that the used subscription of the MSP is out of sync
     service = get_subscription(SERVICE_SUBSCRIPTION_ID)
     service.insync = False
     db.session.commit()
 
     # test the api endpoint
@@ -733,31 +524,14 @@
     assert response.status_code == HTTPStatus.OK
 
     insync_info = response.json()
     assert "reason" not in insync_info
     assert "locked_relations" not in insync_info
 
 
-def test_depends_on_subscriptions(seed, test_client):
-    response = test_client.get(
-        f"/api/subscriptions/depends_on/{SERVICE_SUBSCRIPTION_ID}?filter_statuses=initial,provisioning,active"
-    )
-    depends_on_subs = list(map(lambda sub: sub["subscription_id"], response.json()))
-    assert len(depends_on_subs) == 2
-
-    assert PORT_A_SUBSCRIPTION_ID in depends_on_subs
-    assert SSP_SUBSCRIPTION_ID in depends_on_subs
-
-
-def test_depends_on_subscriptions_bogus_status(seed, test_client):
-    response = test_client.get(f"/api/subscriptions/depends_on/{SERVICE_SUBSCRIPTION_ID}?filter_statuses=NOT_VALID")
-    assert response.status_code == 422
-    assert response.json()["detail"] == "Status NOT_VALID, is not a valid `SubscriptionLifecycle`"
-
-
 def test_depends_on_subscriptions_not_insync(seed, test_client):
     # ensure that the depends on subscription of the LP is out of sync
     msp = db.session.get(SubscriptionTable, PORT_A_SUBSCRIPTION_ID, with_for_update=True)
     msp.insync = False
     db.session.commit()
 
     # test the api endpoint
@@ -774,30 +548,14 @@
     assert response.status_code == HTTPStatus.OK
 
     insync_info = response.json()
     assert "reason" not in insync_info
     assert "locked_relations" not in insync_info
 
 
-def test_in_use_by_subscriptions_direct_relations(seed_with_direct_relations, test_client):
-    response = test_client.get(f"/api/subscriptions/in_use_by/{PORT_A_SUBSCRIPTION_ID}")
-    in_use_by_subs = response.json()
-    assert len(in_use_by_subs) == 1
-    assert SERVICE_SUBSCRIPTION_ID == in_use_by_subs[0]["subscription_id"]
-
-
-def test_subscriptions_for_in_used_by_ids_direct_relations(seed_with_direct_relations, test_client, caplog):
-    instance_id = str(db.session.scalar(select(SubscriptionInstanceTable)).subscription_instance_id)
-    response = test_client.post("/api/subscriptions/subscriptions_for_in_used_by_ids", json=[instance_id])
-    depends_subs = response.json()
-    assert depends_subs[instance_id]
-    assert depends_subs[instance_id]["product"]["product_type"] == "IP_PREFIX"
-    assert "Not all subscription_instance_id's could be resolved." not in caplog.text
-
-
 def test_in_use_by_subscriptions_not_insync_direct_relations(seed_with_direct_relations, test_client):
     # ensure that the used subscription of the MSP is out of sync
     service = get_subscription(SERVICE_SUBSCRIPTION_ID)
     service.insync = False
     db.session.commit()
 
     # test the api endpoint
@@ -805,34 +563,14 @@
     assert response.status_code == HTTPStatus.OK
     insync_info = response.json()
     assert "reason" in insync_info
     assert len(insync_info["locked_relations"]) == 1
     assert insync_info["locked_relations"][0] == SERVICE_SUBSCRIPTION_ID
 
 
-def test_in_use_by_subscriptions_insync_direct_relations(seed_with_direct_relations, test_client):
-    response = test_client.get(f"/api/subscriptions/workflows/{PORT_A_SUBSCRIPTION_ID}")
-    assert response.status_code == HTTPStatus.OK
-
-    insync_info = response.json()
-    assert "reason" not in insync_info
-    assert "locked_relations" not in insync_info
-
-
-def test_depends_on_subscriptions_direct_relations(seed_with_direct_relations, test_client):
-    response = test_client.get(
-        f"/api/subscriptions/depends_on/{SERVICE_SUBSCRIPTION_ID}?filter_statuses=initial,provisioning,active"
-    )
-    depends_on_subs = list(map(lambda sub: sub["subscription_id"], response.json()))
-    assert len(depends_on_subs) == 2
-
-    assert PORT_A_SUBSCRIPTION_ID in depends_on_subs
-    assert SSP_SUBSCRIPTION_ID in depends_on_subs
-
-
 def test_depends_on_subscriptions_not_insync_direct_relations(seed_with_direct_relations, test_client):
     # ensure that the depends on subscription of the LP is out of sync
     msp = get_subscription(PORT_A_SUBSCRIPTION_ID, for_update=True)
     msp.insync = False
     db.session.commit()
 
     # test the api endpoint
@@ -849,37 +587,87 @@
     assert response.status_code == HTTPStatus.OK
 
     insync_info = response.json()
     assert "reason" not in insync_info
     assert "locked_relations" not in insync_info
 
 
-def test_delete_subscription(responses, seed, test_client):
-    wf = WorkflowTable(
-        workflow_id=uuid4(), name="statisch_lichtpad_aanvragen", target=Target.CREATE, description="Test"
+def test_delete_subscription_404(responses, seed, test_client):
+    sub_id = uuid4()
+
+    response = test_client.delete(f"/api/subscriptions/{sub_id}")
+    assert response.status_code == HTTPStatus.NOT_FOUND
+
+
+def test_set_in_sync(seed, test_client):
+    subscription_id = IP_PREFIX_SUBSCRIPTION_ID
+    unsync(subscription_id)
+    db.session.commit()
+
+    response = test_client.put(f"/api/subscriptions/{subscription_id}/set_in_sync")
+    assert response.status_code == HTTPStatus.OK
+
+    subscription = get_subscription(subscription_id)
+    assert subscription.insync
+
+
+def _create_failed_process(subscription_id):
+    wf = WorkflowTable(workflow_id=uuid4(), name="validate_ip_prefix", target=Target.SYSTEM)
+    process_id = uuid4()
+    process = ProcessTable(
+        process_id=process_id,
+        workflow_id=wf.workflow_id,
+        last_status=ProcessStatus.FAILED,
+        last_step="Verify references in NSO",
+        assignee="NOC",
+        is_task=False,
     )
+    process_subscription = ProcessSubscriptionTable(process_id=process_id, subscription_id=subscription_id)
     db.session.add(wf)
+    db.session.add(process)
+    db.session.add(process_subscription)
 
-    process_id = str(uuid4())
-    db.session.add(ProcessTable(process_id=process_id, workflow_id=wf.workflow_id, last_status=ProcessStatus.CREATED))
-    db.session.add(ProcessSubscriptionTable(process_id=process_id, subscription_id=PORT_A_SUBSCRIPTION_ID))
     db.session.commit()
 
-    response = test_client.delete(f"/api/subscriptions/{PORT_A_SUBSCRIPTION_ID}")
-    assert response.status_code == HTTPStatus.OK
 
-    response = test_client.get("/api/processes")
-    assert len(response.json()) == 0
+def test_try_set_failed_task_in_sync(seed, test_client):
+    subscription_id = IP_PREFIX_SUBSCRIPTION_ID
+    unsync(IP_PREFIX_SUBSCRIPTION_ID)
+    db.session.commit()
+
+    _create_failed_process(subscription_id)
 
+    response = test_client.put(f"/api/subscriptions/{subscription_id}/set_in_sync")
+    assert response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY
 
-def test_delete_subscription_404(responses, seed, test_client):
-    sub_id = uuid4()
+    subscription = get_subscription(subscription_id)
+    assert not subscription.insync
 
-    response = test_client.delete(f"/api/subscriptions/{sub_id}")
-    assert response.status_code == HTTPStatus.NOT_FOUND
+
+def test_product_block_paths(generic_subscription_1, generic_subscription_2):
+    subscription_1 = SubscriptionModel.from_subscription(generic_subscription_1)
+    subscription_2 = SubscriptionModel.from_subscription(generic_subscription_2)
+    assert product_block_paths(subscription_1) == ["product", "pb_1", "pb_2"]
+    assert product_block_paths(subscription_2) == ["product", "pb_3"]
+
+
+@pytest.mark.parametrize(
+    "query, num_matches",
+    [
+        ("id", 7),
+        ("tag:(POR* | LP)", 1),
+        ("tag:SP", 3),
+        ("tag:(POR* | LP) | tag:SP", 4),
+        ("tag:(POR* | LP) | tag:SP -status:initial", 3),
+    ],
+)
+def test_subscriptions_search(query, num_matches, seed, test_client, refresh_subscriptions_search_view):
+    response = test_client.get(f"/api/subscriptions/search?query={query}")
+    result = response.json()
+    assert len(result) == num_matches
 
 
 def test_subscription_detail_with_domain_model(test_client, generic_subscription_1):
     # test with a subscription that has domain model and without
     response = test_client.get(URL("api/subscriptions/domain-model") / generic_subscription_1)
     assert response.status_code == HTTPStatus.OK
     # Check hierarchy
@@ -1004,100 +792,7 @@
 
 def test_subscription_detail_with_in_use_by_ids_not_filtered_self(test_client, product_one_subscription_1):
     response = test_client.get(
         URL("api/subscriptions/domain-model") / product_one_subscription_1 / "?filter_owner_relations=false"
     )
     assert response.status_code == HTTPStatus.OK
     assert response.json()["block"]["sub_block"]["in_use_by_ids"]
-
-
-def test_other_subscriptions(test_client, generic_subscription_2, generic_product_type_2):
-    _, GenericProductTwo = generic_product_type_2
-    response = test_client.get(URL("api/subscriptions/instance/other_subscriptions/") / uuid4())
-    assert response.status_code == HTTPStatus.NOT_FOUND
-
-    subscription = GenericProductTwo.from_subscription(generic_subscription_2)
-    response = test_client.get(
-        URL("api/subscriptions/instance/other_subscriptions/") / subscription.pb_3.subscription_instance_id
-    )
-    assert response.status_code == HTTPStatus.OK
-    assert len(response.json()) == 0
-
-
-def test_set_in_sync(seed, test_client):
-    subscription_id = IP_PREFIX_SUBSCRIPTION_ID
-    unsync(subscription_id)
-    db.session.commit()
-
-    response = test_client.put(f"/api/subscriptions/{subscription_id}/set_in_sync")
-    assert response.status_code == HTTPStatus.OK
-
-    subscription = get_subscription(subscription_id)
-    assert subscription.insync
-
-
-def _create_failed_process(subscription_id):
-    wf = WorkflowTable(workflow_id=uuid4(), name="validate_ip_prefix", target=Target.SYSTEM)
-    process_id = uuid4()
-    process = ProcessTable(
-        process_id=process_id,
-        workflow_id=wf.workflow_id,
-        last_status=ProcessStatus.FAILED,
-        last_step="Verify references in NSO",
-        assignee="NOC",
-        is_task=False,
-    )
-    process_subscription = ProcessSubscriptionTable(process_id=process_id, subscription_id=subscription_id)
-    db.session.add(wf)
-    db.session.add(process)
-    db.session.add(process_subscription)
-
-    db.session.commit()
-
-
-def test_try_set_failed_task_in_sync(seed, test_client):
-    subscription_id = IP_PREFIX_SUBSCRIPTION_ID
-    unsync(IP_PREFIX_SUBSCRIPTION_ID)
-    db.session.commit()
-
-    _create_failed_process(subscription_id)
-
-    response = test_client.put(f"/api/subscriptions/{subscription_id}/set_in_sync")
-    assert response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY
-
-    subscription = get_subscription(subscription_id)
-    assert not subscription.insync
-
-
-def test_product_block_paths(generic_subscription_1, generic_subscription_2):
-    subscription_1 = SubscriptionModel.from_subscription(generic_subscription_1)
-    subscription_2 = SubscriptionModel.from_subscription(generic_subscription_2)
-    assert product_block_paths(subscription_1) == ["product", "pb_1", "pb_2"]
-    assert product_block_paths(subscription_2) == ["product", "pb_3"]
-
-
-@pytest.mark.parametrize(
-    "query, num_matches",
-    [
-        ("id", 7),
-        ("tag:(POR* | LP)", 1),
-        ("tag:SP", 3),
-        ("tag:(POR* | LP) | tag:SP", 4),
-        ("tag:(POR* | LP) | tag:SP -status:initial", 3),
-    ],
-)
-def test_subscriptions_search(query, num_matches, seed, test_client, refresh_subscriptions_search_view):
-    response = test_client.get(f"/api/subscriptions/search?query={query}")
-    result = response.json()
-    assert len(result) == num_matches
-
-
-def test_get_subscription_metadata(test_client, generic_subscription_1):
-    response = test_client.get(f"/api/subscriptions/{generic_subscription_1}/metadata")
-    result = response.json()
-    assert result == {"description": "Some metadata description"}
-
-
-def test_get_subscription_metadata_empty(test_client, generic_subscription_2):
-    response = test_client.get(f"/api/subscriptions/{generic_subscription_2}/metadata")
-    result = response.json()
-    assert result is None
```

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_ws.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate.sh` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate.sh`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/alembic.ini` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/env.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/__init__.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/shared.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config1.yaml` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config1.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config2.yaml` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config2.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config3.yaml` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config3.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/generator/test_enums.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/generator/test_enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_cli_generate.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_cli_generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_generate_code.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_generate_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/conftest.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_lifecycle.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/processes.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_customer_contact_list.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_customer_contact_list.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_display_subscription.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_display_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/conftest.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/test_customer_description.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/test_customer_description.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/test_start_process.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/test_start_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_customer.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_product.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_product_blocks.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_resource_types.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_sort_and_filter_fields.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_sort_and_filter_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_subscription.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_subscriptions.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -836,14 +836,16 @@
 )
 def test_single_subscription(test_client, product_type_1_subscriptions_factory, generic_product_type_1, query_args):
     # given
 
     _, GenericProductOne = generic_product_type_1
     subscription_ids = product_type_1_subscriptions_factory(30)
 
+    do_refresh_subscriptions_search_view()
+
     subscription_id = subscription_ids[10]
     subscription = db.session.execute(
         select(SubscriptionTable).filter(SubscriptionTable.subscription_id == subscription_id)
     ).scalar_one_or_none()
     subscription.customer_id = CUSTOMER_ID
     subscription.customer_descriptions = [
         SubscriptionCustomerDescriptionTable(
```

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_workflows.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_autoregistration.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_autoregistration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_is_query_detailed.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_is_querying_page_data.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_is_querying_page_data.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_override_class.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/helpers.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/services/test_processes.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/services/test_products.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/services/test_translations.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/test_db.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/test_workflow.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_errors.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_functional.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_get_updated_properties.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_search_query.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_search_query.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_state.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/websocket/test_broadcast.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/websocket/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/__init__.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_async_workflow.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_async_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc2/PKG-INFO` & `orchestrator_core-2.3.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 2.2.2rc2
+Version: 2.3.0rc1
 Summary: This is the orchestrator workflow engine.
 Requires-Python: >=3.11,<3.13
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -27,61 +27,64 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: alembic==1.13.1
 Requires-Dist: anyio>=3.7.0
 Requires-Dist: click==8.*
 Requires-Dist: deprecated
 Requires-Dist: deepmerge==1.1.1
-Requires-Dist: fastapi~=0.110.0
+Requires-Dist: fastapi~=0.111.0
 Requires-Dist: fastapi-etag==0.4.0
 Requires-Dist: more-itertools~=10.2.0
 Requires-Dist: itsdangerous
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: orjson==3.10.0
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pydantic[email]~=2.5.1
 Requires-Dist: pydantic-settings~=2.2.1
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-rapidjson>=1.9,<1.17
 Requires-Dist: pytz==2024.1
 Requires-Dist: redis==5.0.3
 Requires-Dist: schedule==1.1.0
-Requires-Dist: sentry-sdk[fastapi]==1.44.0
+Requires-Dist: sentry-sdk[fastapi]==2.0.1
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: SQLAlchemy-Utils==0.41.2
 Requires-Dist: structlog
-Requires-Dist: typer==0.12.0
+Requires-Dist: typer==0.12.3
 Requires-Dist: uvicorn[standard]~=0.29.0
 Requires-Dist: nwa-stdlib~=1.7.0
 Requires-Dist: oauth2-lib~=1.5.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: strawberry-graphql==0.210.0
-Requires-Dist: pydantic-forms==1.0.2
+Requires-Dist: pydantic-forms~=1.0.3
 Requires-Dist: ruff
-Requires-Dist: celery~=5.3.1 ; extra == "celery"
+Requires-Dist: celery~=5.4.0 ; extra == "celery"
 Requires-Dist: toml ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: mypy_extensions ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pydocstyle ; extra == "dev"
 Requires-Dist: python-dotenv ; extra == "dev"
 Requires-Dist: watchdog ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "doc"
 Requires-Dist: mkdocs-material[imaging] ; extra == "doc"
 Requires-Dist: mkdocs-render-swagger-plugin ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin ; extra == "doc"
+Requires-Dist: mkdocstrings[python] ; extra == "doc"
+Requires-Dist: mkdocs-open-in-new-tab ; extra == "doc"
+Requires-Dist: mkdocs-macros-plugin ; extra == "doc"
 Requires-Dist: apache-license-check ; extra == "test"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: blinker ; extra == "test"
 Requires-Dist: deepdiff ; extra == "test"
 Requires-Dist: dirty-equals ; extra == "test"
 Requires-Dist: jsonref ; extra == "test"
-Requires-Dist: mypy ; extra == "test"
-Requires-Dist: pytest ; extra == "test"
-Requires-Dist: pytest-asyncio==0.21.0 ; extra == "test"
+Requires-Dist: mypy==1.9 ; extra == "test"
+Requires-Dist: pytest==8.2.0 ; extra == "test"
+Requires-Dist: pytest-asyncio==0.21.2 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-httpx ; extra == "test"
 Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: requests-mock ; extra == "test"
 Requires-Dist: sqlalchemy[mypy] ; extra == "test"
 Requires-Dist: urllib3-mock ; extra == "test"
 Requires-Dist: types-Deprecated ; extra == "test"
```

