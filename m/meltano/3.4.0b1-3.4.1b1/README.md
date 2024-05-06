# Comparing `tmp/meltano-3.4.0b1.tar.gz` & `tmp/meltano-3.4.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltano-3.4.0b1.tar", max compression
+gzip compressed data, was "meltano-3.4.1b1.tar", max compression
```

## Comparing `meltano-3.4.0b1.tar` & `meltano-3.4.1b1.tar`

### file list

```diff
@@ -1,298 +1,298 @@
--rw-r--r--   0        0        0     1048 2024-04-16 15:52:52.147721 meltano-3.4.0b1/LICENSE
--rw-r--r--   0        0        0     5237 2024-04-16 15:52:52.147721 meltano-3.4.0b1/README.md
--rw-r--r--   0        0        0    19419 2024-04-16 15:52:52.275722 meltano-3.4.0b1/pyproject.toml
--rw-r--r--   0        0        0      100 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/__init__.py
--rw-r--r--   0        0        0     3631 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/__init__.py
--rw-r--r--   0        0        0       73 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/__main__.py
--rw-r--r--   0        0        0     6770 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/add.py
--rw-r--r--   0        0        0     6006 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/cli.py
--rw-r--r--   0        0        0     3806 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/compile.py
--rw-r--r--   0        0        0    14489 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/config.py
--rw-r--r--   0        0        0      406 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/docs.py
--rw-r--r--   0        0        0      507 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/dragon.py
--rw-r--r--   0        0        0    17244 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/elt.py
--rw-r--r--   0        0        0     2548 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/environment.py
--rw-r--r--   0        0        0     1671 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/hub.py
--rw-r--r--   0        0        0     2221 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/initialize.py
--rw-r--r--   0        0        0     4100 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/install.py
--rw-r--r--   0        0        0      181 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/interactive/__init__.py
--rw-r--r--   0        0        0    16395 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/interactive/config.py
--rw-r--r--   0        0        0      241 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/interactive/utils.py
--rw-r--r--   0        0        0     6275 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/invoke.py
--rw-r--r--   0        0        0    10060 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/job.py
--rw-r--r--   0        0        0     3804 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/lock.py
--rw-r--r--   0        0        0     2242 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/params.py
--rw-r--r--   0        0        0     2789 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/remove.py
--rw-r--r--   0        0        0     7299 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/run.py
--rw-r--r--   0        0        0    12993 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/schedule.py
--rw-r--r--   0        0        0      770 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/schema.py
--rw-r--r--   0        0        0     4446 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/select.py
--rw-r--r--   0        0        0    10590 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/state.py
--rw-r--r--   0        0        0     4344 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/upgrade.py
--rw-r--r--   0        0        0    23965 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/utils.py
--rw-r--r--   0        0        0     4185 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/validate.py
--rw-r--r--   0        0        0        0 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/__init__.py
--rw-r--r--   0        0        0       64 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/__init__.py
--rw-r--r--   0        0        0    13060 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/canonical.py
--rw-r--r--   0        0        0     3962 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/hookable.py
--rw-r--r--   0        0        0      192 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/name_eq.py
--rw-r--r--   0        0        0     1187 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/versioned.py
--rw-r--r--   0        0        0      406 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/visitor.py
--rw-r--r--   0        0        0      117 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/__init__.py
--rw-r--r--   0        0        0     1582 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/blockset.py
--rw-r--r--   0        0        0    29706 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/extract_load.py
--rw-r--r--   0        0        0     2705 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/future_utils.py
--rw-r--r--   0        0        0     3946 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/ioblock.py
--rw-r--r--   0        0        0    11236 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/parser.py
--rw-r--r--   0        0        0     5745 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/plugin_command.py
--rw-r--r--   0        0        0    12176 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/singer.py
--rw-r--r--   0        0        0      128 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/bundle/__init__.py
--rw-r--r--   0        0        0      460 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/bundle/initialize.yml
--rw-r--r--   0        0        0     2773 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/bundle/settings.yml
--rw-r--r--   0        0        0    10326 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/cli_messages.py
--rw-r--r--   0        0        0     3094 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/config_service.py
--rw-r--r--   0        0        0       81 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/container/__init__.py
--rw-r--r--   0        0        0     2130 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/container/container_service.py
--rw-r--r--   0        0        0     2997 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/container/container_spec.py
--rw-r--r--   0        0        0     7391 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/db.py
--rw-r--r--   0        0        0    14930 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/elt_context.py
--rw-r--r--   0        0        0     6924 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/environment.py
--rw-r--r--   0        0        0     2797 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/environment_service.py
--rw-r--r--   0        0        0     3747 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/error.py
--rw-r--r--   0        0        0      181 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/hub/__init__.py
--rw-r--r--   0        0        0    11085 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/hub/client.py
--rw-r--r--   0        0        0      896 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/hub/schema.py
--rw-r--r--   0        0        0      103 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job/__init__.py
--rw-r--r--   0        0        0     5940 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job/finder.py
--rw-r--r--   0        0        0    11544 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job/job.py
--rw-r--r--   0        0        0     1036 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job/stale_job_failer.py
--rw-r--r--   0        0        0     6015 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job_state.py
--rw-r--r--   0        0        0     2974 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/locked_definition_service.py
--rw-r--r--   0        0        0      699 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/__init__.py
--rw-r--r--   0        0        0     4530 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/formatters.py
--rw-r--r--   0        0        0     5573 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/job_logging_service.py
--rw-r--r--   0        0        0     7367 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/output_logger.py
--rw-r--r--   0        0        0     7084 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/utils.py
--rw-r--r--   0        0        0     3453 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/__init__.py
--rw-r--r--   0        0        0      365 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/cache.py
--rw-r--r--   0        0        0     4835 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/contexts.py
--rw-r--r--   0        0        0     4867 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/jsonschema.py
--rw-r--r--   0        0        0    18190 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/manifest.py
--rw-r--r--   0        0        0     5137 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/meltano_file.py
--rw-r--r--   0        0        0     2679 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/meltano_invoker.py
--rw-r--r--   0        0        0     3665 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/migration_service.py
--rw-r--r--   0        0        0      481 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/models.py
--rw-r--r--   0        0        0      188 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/plugin/__init__.py
--rw-r--r--   0        0        0     5707 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/airflow.py
--rw-r--r--   0        0        0    27344 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/base.py
--rw-r--r--   0        0        0     3638 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/command.py
--rw-r--r--   0        0        0     1422 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/config_service.py
--rw-r--r--   0        0        0      139 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/dbt/__init__.py
--rw-r--r--   0        0        0     4072 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/dbt/base.py
--rw-r--r--   0        0        0     2703 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/error.py
--rw-r--r--   0        0        0     1849 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/factory.py
--rw-r--r--   0        0        0     9890 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/file.py
--rw-r--r--   0        0        0     2708 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/meltano_file.py
--rw-r--r--   0        0        0    14822 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/project_plugin.py
--rw-r--r--   0        0        0     1135 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/requirements.py
--rw-r--r--   0        0        0     7651 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/settings_service.py
--rw-r--r--   0        0        0      282 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/__init__.py
--rw-r--r--   0        0        0     2552 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/base.py
--rw-r--r--   0        0        0    19585 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/catalog.py
--rw-r--r--   0        0        0     2362 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/mapper.py
--rw-r--r--   0        0        0    23896 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/tap.py
--rw-r--r--   0        0        0     5573 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/target.py
--rw-r--r--   0        0        0     5850 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/superset.py
--rw-r--r--   0        0        0      269 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/utility.py
--rw-r--r--   0        0        0    17350 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_install_service.py
--rw-r--r--   0        0        0    17248 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_invoker.py
--rw-r--r--   0        0        0     6473 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_location_remove.py
--rw-r--r--   0        0        0     3931 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_lock_service.py
--rw-r--r--   0        0        0     2817 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_remove_service.py
--rw-r--r--   0        0        0     2180 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_repository.py
--rw-r--r--   0        0        0     3289 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_test_service.py
--rw-r--r--   0        0        0    20306 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project.py
--rw-r--r--   0        0        0     3999 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_add_service.py
--rw-r--r--   0        0        0    14180 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_files.py
--rw-r--r--   0        0        0     6581 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_init_service.py
--rw-r--r--   0        0        0    18330 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_plugins_service.py
--rw-r--r--   0        0        0     5118 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_settings_service.py
--rw-r--r--   0        0        0      262 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/runner/__init__.py
--rw-r--r--   0        0        0     2149 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/runner/dbt.py
--rw-r--r--   0        0        0    10141 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/runner/singer.py
--rw-r--r--   0        0        0     3769 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/schedule.py
--rw-r--r--   0        0        0    10918 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/schedule_service.py
--rw-r--r--   0        0        0     3384 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/select_service.py
--rw-r--r--   0        0        0      926 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/setting.py
--rw-r--r--   0        0        0    15809 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/setting_definition.py
--rw-r--r--   0        0        0    21245 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/settings_service.py
--rw-r--r--   0        0        0    46397 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/settings_store.py
--rw-r--r--   0        0        0     2573 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/sqlalchemy.py
--rw-r--r--   0        0        0     7282 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_service.py
--rw-r--r--   0        0        0     3728 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/__init__.py
--rw-r--r--   0        0        0     5482 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/azure.py
--rw-r--r--   0        0        0     2134 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/base.py
--rw-r--r--   0        0        0     3831 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/db.py
--rw-r--r--   0        0        0    17948 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/filesystem.py
--rw-r--r--   0        0        0     4170 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/google.py
--rw-r--r--   0        0        0     4860 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/s3.py
--rw-r--r--   0        0        0     4461 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/task_sets.py
--rw-r--r--   0        0        0     3993 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/task_sets_service.py
--rw-r--r--   0        0        0        0 2024-04-16 15:53:10.131913 meltano-3.4.0b1/src/meltano/core/tracking/.release_marker
--rw-r--r--   0        0        0     3614 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/README.md
--rw-r--r--   0        0        0      125 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/__init__.py
--rw-r--r--   0        0        0      470 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/cli.py
--rw-r--r--   0        0        0     6044 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/environment.py
--rw-r--r--   0        0        0     3790 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/exception.py
--rw-r--r--   0        0        0     4948 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/plugins.py
--rw-r--r--   0        0        0     4128 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/project.py
--rw-r--r--   0        0        0      918 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1051 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1194 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
--rw-r--r--   0        0        0      720 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      748 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     6002 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     6501 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     6963 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
--rw-r--r--   0        0        0     7408 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
--rw-r--r--   0        0        0     4449 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1403 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1462 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     3920 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2109 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2812 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     1202 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      404 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu.json
--rw-r--r--   0        0        0     9688 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/micro.conf
--rw-r--r--   0        0        0     1112 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/schemas.py
--rw-r--r--   0        0        0    18604 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/tracker.py
--rw-r--r--   0        0        0     3562 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/transform_add_service.py
--rw-r--r--   0        0        0     7708 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/upgrade_service.py
--rw-r--r--   0        0        0    25155 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/utils/__init__.py
--rw-r--r--   0        0        0     1451 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/utils/pidfile.py
--rw-r--r--   0        0        0     4105 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/validation_service.py
--rw-r--r--   0        0        0    23733 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/venv_service.py
--rw-r--r--   0        0        0     1521 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/yaml.py
--rw-r--r--   0        0        0      508 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/__init__.py
--rw-r--r--   0        0        0       12 2024-04-16 15:53:10.055912 meltano-3.4.0b1/src/meltano/migrations/db.lock
--rw-r--r--   0        0        0     1490 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/env.py
--rw-r--r--   0        0        0      495 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/script.py.mako
--rw-r--r--   0        0        0       67 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/utils/__init__.py
--rw-r--r--   0        0        0     1261 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/utils/dialect_typing.py
--rw-r--r--   0        0        0     1814 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
--rw-r--r--   0        0        0      972 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
--rw-r--r--   0        0        0      674 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
--rw-r--r--   0        0        0      802 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
--rw-r--r--   0        0        0      563 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
--rw-r--r--   0        0        0    11827 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
--rw-r--r--   0        0        0     2877 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/6ef30ab7b8e5_.py
--rw-r--r--   0        0        0     1095 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
--rw-r--r--   0        0        0      643 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
--rw-r--r--   0        0        0      786 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
--rw-r--r--   0        0        0     2026 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/b4c05e463b53_.py
--rw-r--r--   0        0        0      972 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
--rw-r--r--   0        0        0      699 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
--rw-r--r--   0        0        0      679 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
--rw-r--r--   0        0        0      486 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
--rw-r--r--   0        0        0    37569 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/schemas/meltano.schema.json
--rw-r--r--   0        0        0      438 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/asserts.py
--rw-r--r--   0        0        0     7479 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/conftest.py
--rw-r--r--   0        0        0     2174 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/cli.py
--rw-r--r--   0        0        0   125876 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/core.py
--rw-r--r--   0        0        0     2829 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/__init__.py
--rw-r--r--   0        0        0     2510 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/mssql.py
--rw-r--r--   0        0        0     1227 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/postgresql.py
--rw-r--r--   0        0        0     1222 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/postgresql_psycopg3.py
--rw-r--r--   0        0        0      328 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/sqlite.py
--rw-r--r--   0        0        0      752 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/docker/__init__.py
--rw-r--r--   0        0        0      276 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/docker/docker-compose.yml
--rw-r--r--   0        0        0     4132 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/docker/snowplow.py
--rw-r--r--   0        0        0     1535 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/fs.py
--rw-r--r--   0        0        0     3135 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/large_config_project/meltano.yml
--rw-r--r--   0        0        0    30013 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/large_config_project/schedule.yml
--rw-r--r--   0        0        0     1086 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/multifile_project/meltano.yml
--rw-r--r--   0        0        0      469 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/multifile_project/subconfig_2.yml
--rw-r--r--   0        0        0      394 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
--rw-r--r--   0        0        0      631 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/plugins/extractors/tap-custom/test.yml
--rw-r--r--   0        0        0     1136 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/utils.py
--rw-r--r--   0        0        0    31067 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_add.py
--rw-r--r--   0        0        0    15154 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_cli.py
--rw-r--r--   0        0        0     5174 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_compile.py
--rw-r--r--   0        0        0     8595 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_config.py
--rw-r--r--   0        0        0    42025 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_elt.py
--rw-r--r--   0        0        0     1585 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_hub.py
--rw-r--r--   0        0        0     3577 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_initialize.py
--rw-r--r--   0        0        0    12665 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_install.py
--rw-r--r--   0        0        0     9285 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_invoke.py
--rw-r--r--   0        0        0     6777 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_job_cmd.py
--rw-r--r--   0        0        0     3771 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_lock.py
--rw-r--r--   0        0        0     1864 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_remove.py
--rw-r--r--   0        0        0    47456 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_run.py
--rw-r--r--   0        0        0     8502 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_schedule.py
--rw-r--r--   0        0        0     1140 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_select.py
--rw-r--r--   0        0        0    11532 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_state.py
--rw-r--r--   0        0        0     8268 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_upgrade.py
--rw-r--r--   0        0        0     5381 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/behavior/test_canonical.py
--rw-r--r--   0        0        0     2155 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/behavior/test_hookable.py
--rw-r--r--   0        0        0    21766 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/block/test_extract_load.py
--rw-r--r--   0        0        0      241 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/block/test_parser.py
--rw-r--r--   0        0        0      933 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/block/test_plugin_command.py
--rw-r--r--   0        0        0     7736 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/block/test_singer.py
--rw-r--r--   0        0        0     2302 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/container/test_container_spec.py
--rw-r--r--   0        0        0     6783 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/hub/test_meltano_hub_service.py
--rw-r--r--   0        0        0     2076 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/job/test_finder.py
--rw-r--r--   0        0        0     6240 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/job/test_job.py
--rw-r--r--   0        0        0     2579 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/job/test_stale_job_failer.py
--rw-r--r--   0        0        0     3357 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/logging/test_formatters.py
--rw-r--r--   0        0        0      806 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/logging/test_logging_utils.py
--rw-r--r--   0        0        0     7398 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/logging/test_output_logger.py
--rw-r--r--   0        0        0    32051 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_catalog.py
--rw-r--r--   0        0        0      562 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_mapper.py
--rw-r--r--   0        0        0    37590 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_tap.py
--rw-r--r--   0        0        0     3690 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_target.py
--rw-r--r--   0        0        0     3921 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_airflow.py
--rw-r--r--   0        0        0     2396 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_command.py
--rw-r--r--   0        0        0    22146 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin.py
--rw-r--r--   0        0        0      174 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin_config_service.py
--rw-r--r--   0        0        0    35208 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin_settings.py
--rw-r--r--   0        0        0     5963 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_superset.py
--rw-r--r--   0        0        0     7999 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/runner/test_runner.py
--rw-r--r--   0        0        0     2807 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/state_store/test_db.py
--rw-r--r--   0        0        0    21574 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/state_store/test_filesystem.py
--rw-r--r--   0        0        0     6765 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/state_store/test_state_store.py
--rw-r--r--   0        0        0     1558 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_db_compat.py
--rw-r--r--   0        0        0     1813 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_db_connection.py
--rw-r--r--   0        0        0     5217 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_elt_context.py
--rw-r--r--   0        0        0     2610 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_environment_service.py
--rw-r--r--   0        0        0    13772 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_environment_variables.py
--rw-r--r--   0        0        0     2274 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_locked_definition_service.py
--rw-r--r--   0        0        0     2108 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_meltano_file.py
--rw-r--r--   0        0        0     3128 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_meltano_invoker.py
--rw-r--r--   0        0        0     4094 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_install_service.py
--rw-r--r--   0        0        0     6101 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_invoker.py
--rw-r--r--   0        0        0     3127 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_lock_service.py
--rw-r--r--   0        0        0     5749 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_remove_service.py
--rw-r--r--   0        0        0     5776 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_test_service.py
--rw-r--r--   0        0        0     4319 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project.py
--rw-r--r--   0        0        0     8892 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_add_service.py
--rw-r--r--   0        0        0    16326 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_files.py
--rw-r--r--   0        0        0     3281 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_init_service.py
--rw-r--r--   0        0        0     8071 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_plugins_service.py
--rw-r--r--   0        0        0     7238 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_settings_service.py
--rw-r--r--   0        0        0     9759 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_schedule_service.py
--rw-r--r--   0        0        0     5865 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_setting_definition.py
--rw-r--r--   0        0        0    22226 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_settings_store.py
--rw-r--r--   0        0        0     3665 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_state_service.py
--rw-r--r--   0        0        0     2430 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_task_sets.py
--rw-r--r--   0        0        0     2645 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_task_sets_service.py
--rw-r--r--   0        0        0     7126 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_utils.py
--rw-r--r--   0        0        0     1813 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_validation_service.py
--rw-r--r--   0        0        0    12257 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_venv_service.py
--rw-r--r--   0        0        0     1980 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_environment_context.py
--rw-r--r--   0        0        0     5708 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_exception.py
--rw-r--r--   0        0        0     3061 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_plugins.py
--rw-r--r--   0        0        0     1271 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_project_context.py
--rw-r--r--   0        0        0      684 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_schemas.py
--rw-r--r--   0        0        0    19704 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_tracker.py
--rw-r--r--   0        0        0     9032 1970-01-01 00:00:00.000000 meltano-3.4.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1048 2024-05-06 16:59:49.770012 meltano-3.4.1b1/LICENSE
+-rw-r--r--   0        0        0     5237 2024-05-06 16:59:49.770012 meltano-3.4.1b1/README.md
+-rw-r--r--   0        0        0    20170 2024-05-06 16:59:49.906013 meltano-3.4.1b1/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/__main__.py
+-rw-r--r--   0        0        0     6770 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/add.py
+-rw-r--r--   0        0        0     6018 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/cli.py
+-rw-r--r--   0        0        0     3806 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/compile.py
+-rw-r--r--   0        0        0    14501 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/config.py
+-rw-r--r--   0        0        0      406 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/docs.py
+-rw-r--r--   0        0        0      507 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/dragon.py
+-rw-r--r--   0        0        0    17244 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/elt.py
+-rw-r--r--   0        0        0     2548 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/environment.py
+-rw-r--r--   0        0        0     1671 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/hub.py
+-rw-r--r--   0        0        0     2232 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/initialize.py
+-rw-r--r--   0        0        0     4099 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/install.py
+-rw-r--r--   0        0        0      181 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/interactive/__init__.py
+-rw-r--r--   0        0        0    16395 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/interactive/config.py
+-rw-r--r--   0        0        0      241 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/interactive/utils.py
+-rw-r--r--   0        0        0     6287 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/invoke.py
+-rw-r--r--   0        0        0    10060 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/job.py
+-rw-r--r--   0        0        0     3804 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/lock.py
+-rw-r--r--   0        0        0     2242 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/params.py
+-rw-r--r--   0        0        0     2789 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/remove.py
+-rw-r--r--   0        0        0     7804 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/run.py
+-rw-r--r--   0        0        0    12993 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/schedule.py
+-rw-r--r--   0        0        0      770 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/schema.py
+-rw-r--r--   0        0        0     4446 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/select.py
+-rw-r--r--   0        0        0    10590 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/state.py
+-rw-r--r--   0        0        0     4344 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/upgrade.py
+-rw-r--r--   0        0        0    24048 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/utils.py
+-rw-r--r--   0        0        0     4185 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/validate.py
+-rw-r--r--   0        0        0        0 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/__init__.py
+-rw-r--r--   0        0        0    13060 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/canonical.py
+-rw-r--r--   0        0        0     3975 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/hookable.py
+-rw-r--r--   0        0        0      192 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/name_eq.py
+-rw-r--r--   0        0        0     1187 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/versioned.py
+-rw-r--r--   0        0        0      406 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/visitor.py
+-rw-r--r--   0        0        0      117 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/block/__init__.py
+-rw-r--r--   0        0        0     1582 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/block/blockset.py
+-rw-r--r--   0        0        0    30262 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/extract_load.py
+-rw-r--r--   0        0        0     2753 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/future_utils.py
+-rw-r--r--   0        0        0     3946 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/ioblock.py
+-rw-r--r--   0        0        0    11405 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/parser.py
+-rw-r--r--   0        0        0     5745 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/plugin_command.py
+-rw-r--r--   0        0        0    12260 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/singer.py
+-rw-r--r--   0        0        0      128 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/bundle/__init__.py
+-rw-r--r--   0        0        0      460 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/bundle/initialize.yml
+-rw-r--r--   0        0        0     2773 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/bundle/settings.yml
+-rw-r--r--   0        0        0    10326 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/cli_messages.py
+-rw-r--r--   0        0        0     3106 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/config_service.py
+-rw-r--r--   0        0        0       81 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/container/__init__.py
+-rw-r--r--   0        0        0     2130 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/container/container_service.py
+-rw-r--r--   0        0        0     2997 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/container/container_spec.py
+-rw-r--r--   0        0        0     7435 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/db.py
+-rw-r--r--   0        0        0    14979 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/elt_context.py
+-rw-r--r--   0        0        0     6924 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/environment.py
+-rw-r--r--   0        0        0     2797 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/environment_service.py
+-rw-r--r--   0        0        0     3747 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/error.py
+-rw-r--r--   0        0        0      181 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/hub/__init__.py
+-rw-r--r--   0        0        0    11085 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/hub/client.py
+-rw-r--r--   0        0        0      896 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/hub/schema.py
+-rw-r--r--   0        0        0      103 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job/__init__.py
+-rw-r--r--   0        0        0     5940 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job/finder.py
+-rw-r--r--   0        0        0    11544 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job/job.py
+-rw-r--r--   0        0        0     1049 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job/stale_job_failer.py
+-rw-r--r--   0        0        0     6015 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job_state.py
+-rw-r--r--   0        0        0     2974 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/locked_definition_service.py
+-rw-r--r--   0        0        0      699 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/__init__.py
+-rw-r--r--   0        0        0     4530 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/formatters.py
+-rw-r--r--   0        0        0     5622 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/job_logging_service.py
+-rw-r--r--   0        0        0     7383 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/output_logger.py
+-rw-r--r--   0        0        0     7100 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/utils.py
+-rw-r--r--   0        0        0     3453 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/cache.py
+-rw-r--r--   0        0        0     4835 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/contexts.py
+-rw-r--r--   0        0        0     4867 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/jsonschema.py
+-rw-r--r--   0        0        0    18190 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/manifest.py
+-rw-r--r--   0        0        0     5137 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/meltano_file.py
+-rw-r--r--   0        0        0     2679 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/meltano_invoker.py
+-rw-r--r--   0        0        0     3744 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/migration_service.py
+-rw-r--r--   0        0        0      481 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/models.py
+-rw-r--r--   0        0        0      188 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/__init__.py
+-rw-r--r--   0        0        0     5751 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/airflow.py
+-rw-r--r--   0        0        0    27362 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/base.py
+-rw-r--r--   0        0        0     3638 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/command.py
+-rw-r--r--   0        0        0     1472 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/config_service.py
+-rw-r--r--   0        0        0      139 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/dbt/__init__.py
+-rw-r--r--   0        0        0     4085 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/dbt/base.py
+-rw-r--r--   0        0        0     2703 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/error.py
+-rw-r--r--   0        0        0     1849 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/factory.py
+-rw-r--r--   0        0        0     9890 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/file.py
+-rw-r--r--   0        0        0     2708 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/meltano_file.py
+-rw-r--r--   0        0        0    14849 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/project_plugin.py
+-rw-r--r--   0        0        0     1135 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/requirements.py
+-rw-r--r--   0        0        0     7651 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/settings_service.py
+-rw-r--r--   0        0        0      282 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/__init__.py
+-rw-r--r--   0        0        0     2601 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/base.py
+-rw-r--r--   0        0        0    19824 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/catalog.py
+-rw-r--r--   0        0        0     2512 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/mapper.py
+-rw-r--r--   0        0        0    23895 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/tap.py
+-rw-r--r--   0        0        0     5592 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/target.py
+-rw-r--r--   0        0        0     5831 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/superset.py
+-rw-r--r--   0        0        0      269 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/utility.py
+-rw-r--r--   0        0        0    17363 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin_install_service.py
+-rw-r--r--   0        0        0    17290 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin_invoker.py
+-rw-r--r--   0        0        0     6473 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_location_remove.py
+-rw-r--r--   0        0        0     3931 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_lock_service.py
+-rw-r--r--   0        0        0     2817 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_remove_service.py
+-rw-r--r--   0        0        0     2180 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_repository.py
+-rw-r--r--   0        0        0     3264 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_test_service.py
+-rw-r--r--   0        0        0    20318 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project.py
+-rw-r--r--   0        0        0     3999 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_add_service.py
+-rw-r--r--   0        0        0    14192 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_files.py
+-rw-r--r--   0        0        0     6581 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_init_service.py
+-rw-r--r--   0        0        0    18330 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_plugins_service.py
+-rw-r--r--   0        0        0     5118 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_settings_service.py
+-rw-r--r--   0        0        0      262 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/runner/__init__.py
+-rw-r--r--   0        0        0     2149 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/runner/dbt.py
+-rw-r--r--   0        0        0    10225 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/runner/singer.py
+-rw-r--r--   0        0        0     3769 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/schedule.py
+-rw-r--r--   0        0        0    10967 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/schedule_service.py
+-rw-r--r--   0        0        0     3384 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/select_service.py
+-rw-r--r--   0        0        0      926 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/setting.py
+-rw-r--r--   0        0        0    15809 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/setting_definition.py
+-rw-r--r--   0        0        0    21258 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/settings_service.py
+-rw-r--r--   0        0        0    46409 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/settings_store.py
+-rw-r--r--   0        0        0     2573 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/sqlalchemy.py
+-rw-r--r--   0        0        0     7282 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_service.py
+-rw-r--r--   0        0        0     3728 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/__init__.py
+-rw-r--r--   0        0        0     5482 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/azure.py
+-rw-r--r--   0        0        0     2116 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/base.py
+-rw-r--r--   0        0        0     3831 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/db.py
+-rw-r--r--   0        0        0    17960 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/filesystem.py
+-rw-r--r--   0        0        0     4170 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/google.py
+-rw-r--r--   0        0        0     4860 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/s3.py
+-rw-r--r--   0        0        0     4461 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/task_sets.py
+-rw-r--r--   0        0        0     3993 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/task_sets_service.py
+-rw-r--r--   0        0        0        0 2024-05-06 17:00:07.430114 meltano-3.4.1b1/src/meltano/core/tracking/.release_marker
+-rw-r--r--   0        0        0     3614 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/README.md
+-rw-r--r--   0        0        0      125 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/__init__.py
+-rw-r--r--   0        0        0      470 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/cli.py
+-rw-r--r--   0        0        0     6044 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/environment.py
+-rw-r--r--   0        0        0     3790 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/exception.py
+-rw-r--r--   0        0        0     4942 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/plugins.py
+-rw-r--r--   0        0        0     4128 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/project.py
+-rw-r--r--   0        0        0      918 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1051 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1194 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0      720 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      748 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     6002 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     6501 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     6963 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
+-rw-r--r--   0        0        0     7408 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
+-rw-r--r--   0        0        0     4449 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1403 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1462 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     3920 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2109 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2812 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     1202 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      404 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu.json
+-rw-r--r--   0        0        0     9688 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/micro.conf
+-rw-r--r--   0        0        0     1112 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/schemas.py
+-rw-r--r--   0        0        0    18604 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/tracking/tracker.py
+-rw-r--r--   0        0        0     3562 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/transform_add_service.py
+-rw-r--r--   0        0        0     7708 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/upgrade_service.py
+-rw-r--r--   0        0        0    25167 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/utils/__init__.py
+-rw-r--r--   0        0        0     1463 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/utils/pidfile.py
+-rw-r--r--   0        0        0     4095 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/validation_service.py
+-rw-r--r--   0        0        0    23746 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/venv_service.py
+-rw-r--r--   0        0        0     1521 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/yaml.py
+-rw-r--r--   0        0        0      508 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/__init__.py
+-rw-r--r--   0        0        0       12 2024-05-06 17:00:07.346114 meltano-3.4.1b1/src/meltano/migrations/db.lock
+-rw-r--r--   0        0        0     1490 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/env.py
+-rw-r--r--   0        0        0      495 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/script.py.mako
+-rw-r--r--   0        0        0       67 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/utils/__init__.py
+-rw-r--r--   0        0        0     1261 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/utils/dialect_typing.py
+-rw-r--r--   0        0        0     1814 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
+-rw-r--r--   0        0        0      972 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
+-rw-r--r--   0        0        0      674 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
+-rw-r--r--   0        0        0      802 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
+-rw-r--r--   0        0        0      563 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
+-rw-r--r--   0        0        0    11827 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
+-rw-r--r--   0        0        0     2877 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/6ef30ab7b8e5_.py
+-rw-r--r--   0        0        0     1095 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
+-rw-r--r--   0        0        0      643 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
+-rw-r--r--   0        0        0      786 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
+-rw-r--r--   0        0        0     2026 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/b4c05e463b53_.py
+-rw-r--r--   0        0        0      972 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
+-rw-r--r--   0        0        0      699 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
+-rw-r--r--   0        0        0      679 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
+-rw-r--r--   0        0        0      486 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
+-rw-r--r--   0        0        0    37573 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/schemas/meltano.schema.json
+-rw-r--r--   0        0        0      438 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/asserts.py
+-rw-r--r--   0        0        0     7479 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/conftest.py
+-rw-r--r--   0        0        0     2190 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/cli.py
+-rw-r--r--   0        0        0   125892 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/core.py
+-rw-r--r--   0        0        0     2845 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/__init__.py
+-rw-r--r--   0        0        0     2518 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/mssql.py
+-rw-r--r--   0        0        0     1227 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/postgresql.py
+-rw-r--r--   0        0        0     1222 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/postgresql_psycopg3.py
+-rw-r--r--   0        0        0      328 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/sqlite.py
+-rw-r--r--   0        0        0      752 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/docker/__init__.py
+-rw-r--r--   0        0        0      276 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/docker/docker-compose.yml
+-rw-r--r--   0        0        0     4132 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/docker/snowplow.py
+-rw-r--r--   0        0        0     1535 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/fs.py
+-rw-r--r--   0        0        0     3135 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/large_config_project/meltano.yml
+-rw-r--r--   0        0        0    30013 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/large_config_project/schedule.yml
+-rw-r--r--   0        0        0     1086 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/multifile_project/meltano.yml
+-rw-r--r--   0        0        0      469 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/multifile_project/subconfig_2.yml
+-rw-r--r--   0        0        0      394 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
+-rw-r--r--   0        0        0      631 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/plugins/extractors/tap-custom/test.yml
+-rw-r--r--   0        0        0     1152 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/utils.py
+-rw-r--r--   0        0        0    31067 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_add.py
+-rw-r--r--   0        0        0    15154 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_cli.py
+-rw-r--r--   0        0        0     5174 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_compile.py
+-rw-r--r--   0        0        0     8634 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_config.py
+-rw-r--r--   0        0        0    42021 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_elt.py
+-rw-r--r--   0        0        0     1585 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_hub.py
+-rw-r--r--   0        0        0     3577 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_initialize.py
+-rw-r--r--   0        0        0    12665 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_install.py
+-rw-r--r--   0        0        0     9285 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_invoke.py
+-rw-r--r--   0        0        0     6777 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_job_cmd.py
+-rw-r--r--   0        0        0     3771 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_lock.py
+-rw-r--r--   0        0        0     1864 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_remove.py
+-rw-r--r--   0        0        0    48146 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_run.py
+-rw-r--r--   0        0        0     8502 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_schedule.py
+-rw-r--r--   0        0        0     1140 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_select.py
+-rw-r--r--   0        0        0    11532 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_state.py
+-rw-r--r--   0        0        0     8268 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_upgrade.py
+-rw-r--r--   0        0        0     5381 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/behavior/test_canonical.py
+-rw-r--r--   0        0        0     2155 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/behavior/test_hookable.py
+-rw-r--r--   0        0        0    22553 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/block/test_extract_load.py
+-rw-r--r--   0        0        0      241 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/block/test_parser.py
+-rw-r--r--   0        0        0      933 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/block/test_plugin_command.py
+-rw-r--r--   0        0        0     7736 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/block/test_singer.py
+-rw-r--r--   0        0        0     2302 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/container/test_container_spec.py
+-rw-r--r--   0        0        0     6783 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/hub/test_meltano_hub_service.py
+-rw-r--r--   0        0        0     2076 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/job/test_finder.py
+-rw-r--r--   0        0        0     6240 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/job/test_job.py
+-rw-r--r--   0        0        0     2579 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/job/test_stale_job_failer.py
+-rw-r--r--   0        0        0     3357 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/logging/test_formatters.py
+-rw-r--r--   0        0        0      806 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/logging/test_logging_utils.py
+-rw-r--r--   0        0        0     7590 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/logging/test_output_logger.py
+-rw-r--r--   0        0        0    32646 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_catalog.py
+-rw-r--r--   0        0        0     3185 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_mapper.py
+-rw-r--r--   0        0        0    37606 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_tap.py
+-rw-r--r--   0        0        0     3690 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_target.py
+-rw-r--r--   0        0        0     3921 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_airflow.py
+-rw-r--r--   0        0        0     2396 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_command.py
+-rw-r--r--   0        0        0    22146 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin.py
+-rw-r--r--   0        0        0      174 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin_config_service.py
+-rw-r--r--   0        0        0    35208 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin_settings.py
+-rw-r--r--   0        0        0     5963 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_superset.py
+-rw-r--r--   0        0        0     7999 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/runner/test_runner.py
+-rw-r--r--   0        0        0     2807 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/state_store/test_db.py
+-rw-r--r--   0        0        0    21574 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/state_store/test_filesystem.py
+-rw-r--r--   0        0        0     6765 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/state_store/test_state_store.py
+-rw-r--r--   0        0        0     1558 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_db_compat.py
+-rw-r--r--   0        0        0     1813 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_db_connection.py
+-rw-r--r--   0        0        0     5217 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_elt_context.py
+-rw-r--r--   0        0        0     2610 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_environment_service.py
+-rw-r--r--   0        0        0    13772 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_environment_variables.py
+-rw-r--r--   0        0        0     2274 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_locked_definition_service.py
+-rw-r--r--   0        0        0     2108 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_meltano_file.py
+-rw-r--r--   0        0        0     3128 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_meltano_invoker.py
+-rw-r--r--   0        0        0     4094 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_install_service.py
+-rw-r--r--   0        0        0     6101 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_invoker.py
+-rw-r--r--   0        0        0     3127 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_lock_service.py
+-rw-r--r--   0        0        0     5749 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_remove_service.py
+-rw-r--r--   0        0        0     5815 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_test_service.py
+-rw-r--r--   0        0        0     4319 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project.py
+-rw-r--r--   0        0        0     8892 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_add_service.py
+-rw-r--r--   0        0        0    16326 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_files.py
+-rw-r--r--   0        0        0     3281 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_init_service.py
+-rw-r--r--   0        0        0     8071 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_plugins_service.py
+-rw-r--r--   0        0        0     7238 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_settings_service.py
+-rw-r--r--   0        0        0     9759 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_schedule_service.py
+-rw-r--r--   0        0        0     5865 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_setting_definition.py
+-rw-r--r--   0        0        0    22226 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_settings_store.py
+-rw-r--r--   0        0        0     3665 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_state_service.py
+-rw-r--r--   0        0        0     2430 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_task_sets.py
+-rw-r--r--   0        0        0     2645 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_task_sets_service.py
+-rw-r--r--   0        0        0     7126 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_utils.py
+-rw-r--r--   0        0        0     1813 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_validation_service.py
+-rw-r--r--   0        0        0    12257 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_venv_service.py
+-rw-r--r--   0        0        0     1980 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/tracking/test_environment_context.py
+-rw-r--r--   0        0        0     5708 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_exception.py
+-rw-r--r--   0        0        0     3061 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_plugins.py
+-rw-r--r--   0        0        0     1271 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_project_context.py
+-rw-r--r--   0        0        0      684 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_schemas.py
+-rw-r--r--   0        0        0    19720 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_tracker.py
+-rw-r--r--   0        0        0     9032 1970-01-01 00:00:00.000000 meltano-3.4.1b1/PKG-INFO
```

### Comparing `meltano-3.4.0b1/LICENSE` & `meltano-3.4.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/README.md` & `meltano-3.4.1b1/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/pyproject.toml` & `meltano-3.4.1b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltano"
-version = "3.4.0b1"
+version = "3.4.1b1"
 description = "Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love."
 authors = ["Meltano <hello@meltano.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/meltano/meltano"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -43,28 +43,28 @@
 aiodocker = "^0.21.0"
 alembic = "^1.13.1"
 atomicwrites = "^1.2.1"
 azure-common = {version = "^1.1.28", optional = true}
 azure-core = {version = "^1.30.1", optional = true}
 azure-identity = {version = "^1.16.0", optional = true}
 azure-storage-blob = {version = "^12.19.1", optional = true}
-boto3 = {version = "^1.34.84", optional = true}
+boto3 = {version = "^1.34.98", optional = true}
 check-jsonschema = "^0.28.2"
 click = "^8.1"
 click-default-group = "^1.2.4"
 click-didyoumean = "^0.3.1"
-croniter = "^2.0.3"
+croniter = "^2.0.5"
 fasteners = "^0.19"
 flatten-dict = "^0"
 google-cloud-storage = {version = ">=1.31.0", optional = true}
 importlib-resources = "^6.4.0"
-jinja2 = "^3.1.3"
-jsonschema = "^4.21"
+jinja2 = "^3.1.4"
+jsonschema = "^4.22"
 packaging = "^24.0"
-platformdirs = "^4.2.0"
+platformdirs = "^4.2.1"
 psutil = "^5.9.8"
 psycopg = {version = "^3.1.18", extras = ["binary"], optional = true}
 psycopg2-binary = {version="^2.9.9", optional=true}
 pyjwt = "^2.6.0"
 pymssql = {version = "^2.3.0", optional = true}
 python = ">=3.8,<3.13"
 python-dateutil = "^2.9.0"
@@ -75,62 +75,62 @@
 questionary = "^2.0.1"
 requests = "^2.31.0"
 rich = "^13.7.1"
 "ruamel.yaml" = "^0.18.6"
 setuptools = {version = "^69.5.1", python = ">=3.12"}
 smart-open = "^7.0.4"
 snowplow-tracker = "^1.0.2"
-sqlalchemy = "^2.0.29"
+sqlalchemy = "^2.0.30"
 structlog = "^24.1.0"
 tabulate = "^0.9.0"
 typing-extensions = "^4.11.0"
 tzlocal = "^5.2"
 # Compatibility issues with boto: https://github.com/boto/botocore/pull/3034
 urllib3 = "<2"
 uv = { version = ">=0.1.24,<0.2", optional = true }
-virtualenv = "^20.25.1"
+virtualenv = "^20.26.1"
 yaspin = "^2.3.0"
 
 [tool.poetry.extras]
 azure = ["azure-storage-blob", "azure-common", "azure-core", "azure-identity"]
 gcs = ["google-cloud-storage"]
 mssql = ["pymssql"]
 postgres = ["psycopg"]
 psycopg2 = ["psycopg2-binary"]
 s3 = ["boto3"]
 uv = ["uv"]
 
 [tool.poetry.group.dev.dependencies]
 backoff = "^2.1.2"
-black = "^24.4.0"
-boto3-stubs = {extras = ["essential"], version = "1.34.84"}
+black = "^24.4.2"
+boto3-stubs = {extras = ["essential"], version = "1.34.98"}
 bumpversion = "^0.6.0"
 colorama = "^0.4.4"
 coverage = {extras = ["toml"], version = ">=7.3.2,!=7.3.3"}
-freezegun = "^1.4.0"
-hypothesis = "^6.100.1"
+freezegun = "^1.5.0"
+hypothesis = "^6.100.4"
 mock = "^5.0.2"
-moto = "^5.0.5"
-mypy = "^1.9.0"
+moto = "^5.0.6"
+mypy = "^1.10.0"
 pre-commit = "^3.5.0"
-pytest = "^8.1.1"
+pytest = "^8.2.0"
 pytest-asyncio = "^0.23.6"
 pytest-cov = "^5.0.0"
 pytest-docker = "^3.1"
 pytest-httpserver = "^1.0.10"
 pytest-order = "^1.2"
 pytest-randomly = "^3.12"
 pytest-rerunfailures = "^14.0"
 pytest-structlog = "^0.8"
-pytest-xdist = "^3.5"
+pytest-xdist = "^3.6"
 requests-mock = "^1.12.1"
 setproctitle = "^1.3" # Used by pytest-xdist to aid with handling resource intensive processes.
 types-croniter = "^2.0.0"
-types-jsonschema = "^4.21.0.20240331"
-types-psutil = "^5.9.5.20240316"
+types-jsonschema = "^4.22.0.20240501"
+types-psutil = "^5.9.5.20240423"
 types-python-dateutil = "^2.9.0.20240316"
 types-python-slugify = "^8.0.2.20240310"
 types-pyyaml = "^6.0.12.20240311"
 types-requests = "^2.31.0"
 types-tabulate = "^0.9.0.20240106"
 
 [tool.poetry.scripts]
@@ -470,15 +470,15 @@
 skip_covered = true
 
 [tool.commitizen]
 name = "cz_version_bump"
 prerelease_offset = 1
 tag_format = "v$major.$minor.$patch$prerelease"
 changelog_merge_prerelease = true
-version = "3.4.0b1"
+version = "3.4.1b1"
 version_files = [
   "pyproject.toml:^version =",
   "src/meltano/__init__.py:^__version__ =",
   'docs/package.json:^  "version":',
 ]
 
 [tool.mypy]
@@ -643,9 +643,19 @@
 known-first-party = ["asserts", "fixtures", "meltano"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.ruff.lint.flake8-tidy-imports.banned-api]
+"logging.getLogger".msg = "Use `structlog.stdlib.get_logger` instead"
+"logging.critical".msg = "Create a logger with `structlog.stdlib.get_logger`"
+"logging.fatal".msg = "Create a logger with `structlog.stdlib.get_logger`"
+"logging.error".msg = "Create a logger with `structlog.stdlib.get_logger`"
+"logging.exception".msg = "Create a logger with `structlog.stdlib.get_logger`"
+"logging.warning".msg = "Create a logger with `structlog.stdlib.get_logger`"
+"logging.warn".msg = "Create a logger with `structlog.stdlib.get_logger`"
+"logging.info".msg = "Create a logger with `structlog.stdlib.get_logger`"
+"logging.debug".msg = "Create a logger with `structlog.stdlib.get_logger`"
+"logging.log".msg = "Create a logger with `structlog.stdlib.get_logger`"
 "meltano.cli.cli.command".msg = "Use `click.command` and `meltano.cli.cli.add_command` instead"
 "meltano.cli.cli.group".msg = "Use `click.group` and `meltano.cli.cli.add_command` instead"
```

### Comparing `meltano-3.4.0b1/src/meltano/cli/__init__.py` & `meltano-3.4.1b1/src/meltano/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Main entry point for the meltano CLI."""
 
 from __future__ import annotations
 
-import logging
 import os
 import sys
 import typing as t
 
+import structlog
+
 from meltano.cli import (  # noqa: WPS235
     add,
     config,
     docs,
     dragon,
     elt,
     environment,
@@ -67,15 +68,15 @@
 
 atexit_handler_registered = False
 exit_code_reported = False
 exit_event_tracker: Tracker | None = None
 
 setup_logging()
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 troubleshooting_message = """\
 Need help fixing this problem? Visit http://melta.no/ for troubleshooting steps, or to
 join our friendly Slack community.
 """
```

### Comparing `meltano-3.4.0b1/src/meltano/cli/add.py` & `meltano-3.4.1b1/src/meltano/cli/add.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/cli.py` & `meltano-3.4.1b1/src/meltano/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """Definition of the top-level Click group for the Meltano CLI."""
 
 from __future__ import annotations
 
-import logging
 import os
 import platform
 import sys
 import typing as t
 from pathlib import Path
 
 import click
+import structlog
 
 from meltano import (
     __version__,
 )
 from meltano.cli.utils import InstrumentedGroup
 from meltano.core.behavior.versioned import IncompatibleVersionError
 from meltano.core.error import EmptyMeltanoFileException, ProjectNotFound
 from meltano.core.logging import LEVELS, setup_logging
 from meltano.core.project import PROJECT_ENVIRONMENT_ENV, Project
 from meltano.core.project_settings_service import ProjectSettingsService
 from meltano.core.tracking import Tracker
 from meltano.core.tracking.contexts import CliContext
 from meltano.core.utils import get_no_color_flag
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class NoWindowsGlobbingGroup(InstrumentedGroup):
     """A instrumented Click group that does not perform glob expansion on Windows.
 
     This restores the behaviour of Click's globbing to how it was before v8.
     Click (as of version 8.1.3) ignores quotes around an asterisk, which makes
```

### Comparing `meltano-3.4.0b1/src/meltano/cli/compile.py` & `meltano-3.4.1b1/src/meltano/cli/compile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/config.py` & `meltano-3.4.1b1/src/meltano/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Config management CLI."""
 
 from __future__ import annotations
 
 import asyncio
 import json
-import logging
 import tempfile
 import typing as t
 from functools import wraps
 from pathlib import Path
 
 import click
 import dotenv
+import structlog
 
 from meltano.cli.interactive import InteractiveConfig
 from meltano.cli.params import pass_project
 from meltano.cli.utils import (
     CliEnvironmentBehavior,
     CliError,
     InstrumentedGroup,
@@ -30,15 +30,15 @@
 from meltano.core.settings_service import SettingValueStore
 from meltano.core.settings_store import StoreNotSupportedError
 from meltano.core.tracking.contexts import CliEvent, PluginsTrackingContext
 
 if t.TYPE_CHECKING:
     from meltano.core.project import Project
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 def _get_ctx_arg(*args: t.Any) -> click.core.Context:
     """Get the click.core.Context arg from a set of args.
 
     Args:
         args: the args to get Context from
```

### Comparing `meltano-3.4.0b1/src/meltano/cli/elt.py` & `meltano-3.4.1b1/src/meltano/cli/elt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/environment.py` & `meltano-3.4.1b1/src/meltano/cli/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/hub.py` & `meltano-3.4.1b1/src/meltano/cli/hub.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/initialize.py` & `meltano-3.4.1b1/src/meltano/cli/initialize.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """New Project Initialization CLI."""
 
 from __future__ import annotations
 
-import logging
 from pathlib import Path
 
 import click
+import structlog
 
 from meltano.cli.params import database_uri_option
 from meltano.cli.utils import InstrumentedCmd
 from meltano.core.project_init_service import ProjectInitService
 from meltano.core.project_settings_service import ProjectSettingsService
 from meltano.core.tracking import Tracker
 from meltano.core.tracking.contexts import CliContext, CliEvent
 
 EXTRACTORS = "extractors"
 LOADERS = "loaders"
 ALL = "all"
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 path_type = click.Path(file_okay=False, path_type=Path)
 
 
 @click.command(cls=InstrumentedCmd, short_help="Create a new Meltano project.")
 @click.pass_context
 @click.argument("project_directory", required=False, type=path_type)
 @click.option(
@@ -48,15 +48,15 @@
         project_directory = click.prompt(
             "Enter a name now to create a Meltano project",
             type=path_type,
         )
 
     if ctx.obj["project"]:
         root = ctx.obj["project"].root
-        logging.warning(f"Found meltano project at: {root}")  # noqa: G004
+        logger.warning(f"Found meltano project at: {root}")  # noqa: G004
 
     if no_usage_stats:
         ProjectSettingsService.config_override["send_anonymous_usage_stats"] = False
 
     init_service = ProjectInitService(project_directory)
 
     project = init_service.init(force=force)
```

### Comparing `meltano-3.4.0b1/src/meltano/cli/install.py` & `meltano-3.4.1b1/src/meltano/cli/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 schedule_name,
             )
             plugins = list(set(plugins) & set(schedule_plugins))
     except Exception:
         tracker.track_command_event(CliEvent.aborted)
         raise
 
-    click.echo(f"Installing {len(plugins)} plugins...")
+    logger.info("Installing %d plugins", len(plugins))
     tracker.add_contexts(
         PluginsTrackingContext([(candidate, None) for candidate in plugins]),
     )
     tracker.track_command_event(CliEvent.inflight)
 
     success = install_plugins(
         project,
```

### Comparing `meltano-3.4.0b1/src/meltano/cli/interactive/config.py` & `meltano-3.4.1b1/src/meltano/cli/interactive/config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/invoke.py` & `meltano-3.4.1b1/src/meltano/cli/invoke.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """CLI command `meltano invoke`."""
 
 from __future__ import annotations
 
 import asyncio
-import logging
 import sys
 import typing as t
 
 import click
+import structlog
 
 from meltano.cli.params import pass_project
 from meltano.cli.utils import (
     CliEnvironmentBehavior,
     CliError,
     PartialInstrumentedCmd,
     propagate_stop_signals,
@@ -29,15 +29,15 @@
 
 if t.TYPE_CHECKING:
     from sqlalchemy.orm import sessionmaker
 
     from meltano.core.project import Project
     from meltano.core.tracking import Tracker
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 @click.command(
     cls=PartialInstrumentedCmd,
     context_settings={"ignore_unknown_options": True, "allow_interspersed_args": False},
     short_help="Invoke a plugin.",
     environment_behavior=CliEnvironmentBehavior.environment_optional_use_default,
```

### Comparing `meltano-3.4.0b1/src/meltano/cli/job.py` & `meltano-3.4.1b1/src/meltano/cli/job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/lock.py` & `meltano-3.4.1b1/src/meltano/cli/lock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/params.py` & `meltano-3.4.1b1/src/meltano/cli/params.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/remove.py` & `meltano-3.4.1b1/src/meltano/cli/remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/run.py` & `meltano-3.4.1b1/src/meltano/cli/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Meltano run command and supporting functions."""
 
 from __future__ import annotations
 
 import typing as t
+import uuid
 
 import click
 import structlog
 
 from meltano.cli.params import pass_project
 from meltano.cli.utils import CliEnvironmentBehavior, CliError, PartialInstrumentedCmd
 from meltano.core.block.blockset import BlockSet
@@ -22,14 +23,27 @@
 
 if t.TYPE_CHECKING:
     from meltano.core.project import Project
 
 logger = structlog.getLogger(__name__)
 
 
+class UUIDParamType(click.ParamType):
+    """A custom click parameter type for UUIDs."""
+
+    name = "uuid"
+
+    def convert(self, value, param, ctx):
+        """Convert an input value to a UUID."""
+        try:
+            return uuid.UUID(value)
+        except ValueError:
+            self.fail(f"{value} is not a valid UUID.", param, ctx)
+
+
 @click.command(
     cls=PartialInstrumentedCmd,
     short_help="Run a set of plugins in series.",
     environment_behavior=CliEnvironmentBehavior.environment_required,
 )
 @click.option(
     "--dry-run",
@@ -66,14 +80,19 @@
     help="Define a custom suffix to autogenerate state IDs with.",
 )
 @click.option(
     "--merge-state",
     is_flag=True,
     help="Merges state with that of previous runs.",
 )
+@click.option(
+    "--run-id",
+    type=UUIDParamType(),
+    help="Use a custom run ID.",
+)
 @click.argument(
     "blocks",
     nargs=-1,
 )
 @pass_project(migrate=True)
 @click.pass_context
 @run_async
@@ -82,14 +101,15 @@
     project: Project,
     dry_run: bool,
     full_refresh: bool,
     no_state_update: bool,
     force: bool,
     state_id_suffix: str,
     merge_state: bool,
+    run_id: uuid.UUID | None,
     blocks: list[str],
 ):
     """
     Run a set of command blocks in series.
 
     Blocks are specified as either:\n
       - a list of plugin names\n
@@ -123,14 +143,15 @@
             project,
             blocks,
             full_refresh=full_refresh,
             no_state_update=no_state_update,
             force=force,
             state_id_suffix=state_id_suffix,
             merge_state=merge_state,
+            run_id=run_id,
         )
         parsed_blocks = list(parser.find_blocks(0))
         if not parsed_blocks:
             tracker.track_command_event(CliEvent.aborted)
             logger.info("No valid blocks found.")
             return
     except Exception as parser_err:
```

### Comparing `meltano-3.4.0b1/src/meltano/cli/schedule.py` & `meltano-3.4.1b1/src/meltano/cli/schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/schema.py` & `meltano-3.4.1b1/src/meltano/cli/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/select.py` & `meltano-3.4.1b1/src/meltano/cli/select.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/state.py` & `meltano-3.4.1b1/src/meltano/cli/state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/upgrade.py` & `meltano-3.4.1b1/src/meltano/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/cli/utils.py` & `meltano-3.4.1b1/src/meltano/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 import os
 import signal
 import typing as t
 from contextlib import contextmanager
 from enum import Enum, auto
 
 import click
+import structlog
 from click_default_group import DefaultGroup
 from click_didyoumean import DYMGroup
 
 from meltano.core.error import MeltanoConfigurationError
 from meltano.core.logging import setup_logging
 from meltano.core.plugin.base import PluginDefinition, PluginType
 from meltano.core.plugin.error import InvalidPluginDefinitionError, PluginNotFoundError
 from meltano.core.plugin_install_service import (
     PluginInstallReason,
     PluginInstallService,
+    PluginInstallState,
     PluginInstallStatus,
 )
 from meltano.core.plugin_lock_service import LockfileAlreadyExistsError
 from meltano.core.project_add_service import (
     PluginAddedReason,
     PluginAlreadyAddedException,
     ProjectAddService,
@@ -35,15 +37,15 @@
     from meltano.core.plugin.base import PluginRef
     from meltano.core.plugin.project_plugin import ProjectPlugin
     from meltano.core.project import Project
     from meltano.core.project_plugins_service import ProjectPluginsService
 
 setup_logging()
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class CliError(Exception):
     """CLI Error."""
 
     def __init__(self, *args, **kwargs):
         """Instantiate custom CLI Error exception."""
@@ -398,36 +400,34 @@
             click.echo()
 
         added_plugins.extend(required_plugins)
 
     return added_plugins
 
 
-def install_status_update(install_state):
+def install_status_update(install_state: PluginInstallState):
     """
     Print the status of plugin installation.
 
     Used as the callback for PluginInstallService.
     """
     plugin = install_state.plugin
     desc = plugin.type.descriptor
     if install_state.status in {
         PluginInstallStatus.RUNNING,
         PluginInstallStatus.SKIPPED,
     }:
-        msg = f"{install_state.verb} {desc} '{plugin.name}'..."
-        click.secho(msg)
+        logger.info("%s %s '%s'", install_state.verb, desc, plugin.name)
     elif install_state.status is PluginInstallStatus.ERROR:
-        click.secho(install_state.message, fg="red")
-        click.secho(install_state.details, err=True)
-    elif install_state.status is PluginInstallStatus.WARNING:
-        click.secho(f"Warning! {install_state.message}.", fg="yellow")
+        logger.error(install_state.message)
+        logger.info(install_state.details)
+    elif install_state.status is PluginInstallStatus.WARNING:  # pragma: no cover
+        logger.warning(install_state.message)
     elif install_state.status is PluginInstallStatus.SUCCESS:
-        msg = f"{install_state.verb} {desc} '{plugin.name}'"
-        click.secho(msg, fg="green")
+        logger.info("%s %s '%s'", install_state.verb, desc, plugin.name)
 
 
 def install_plugins(
     project,
     plugins,
     reason=PluginInstallReason.INSTALL,
     parallelism=None,
@@ -443,31 +443,34 @@
         force=force,
     )
     install_results = install_service.install_plugins(plugins, reason=reason)
     num_successful = len([status for status in install_results if status.successful])
     num_skipped = len([status for status in install_results if status.skipped])
     num_failed = len(install_results) - num_successful
 
-    fg = "green"
+    level = logging.INFO
     if num_failed >= 0 and num_successful == 0:
-        fg = "red"
+        level = logging.ERROR
     elif num_failed > 0 and num_successful > 0:
-        fg = "yellow"
+        level = logging.WARNING
 
     if len(plugins) > 1:
-        verb = "Updated" if reason == PluginInstallReason.UPGRADE else "Installed"
-        click.secho(
-            f"{verb} {num_successful-num_skipped}/{num_successful+num_failed} plugins",
-            fg=fg,
-        )
-    if num_skipped:
-        verb = "Skipped installing"
-        click.secho(
-            f"{verb} {num_skipped}/{num_successful+num_failed} plugins",
-            fg=fg,
+        logger.log(
+            level,
+            "%s %d/%d plugins",
+            "Updated" if reason == PluginInstallReason.UPGRADE else "Installed",
+            num_successful - num_skipped,
+            num_successful + num_failed,
+        )
+    if num_skipped:  # pragma: no cover
+        logger.log(
+            level,
+            "Skipped installing %d/%d plugins",
+            num_skipped,
+            num_successful + num_failed,
         )
 
     return num_failed == 0
 
 
 @contextmanager
 def propagate_stop_signals(proc):
```

### Comparing `meltano-3.4.0b1/src/meltano/cli/validate.py` & `meltano-3.4.1b1/src/meltano/cli/validate.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/behavior/canonical.py` & `meltano-3.4.1b1/src/meltano/core/behavior/canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/behavior/hookable.py` & `meltano-3.4.1b1/src/meltano/core/behavior/hookable.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 This module contains the Hookable class which allows for implementation of a
 classic before/after hook pattern. Allowing you to register functions to be
 called before or after given trigger.
 """
 
 from __future__ import annotations
 
-import logging
 from collections import OrderedDict
 from contextlib import asynccontextmanager
 
-logger = logging.getLogger(__name__)
+import structlog
+
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class hook:  # noqa: N801
     """This decorator marks a function as a `__hook__`.
 
     It will be found by the `Hookable` metaclass and registered to be triggered
     accordingly.
```

### Comparing `meltano-3.4.0b1/src/meltano/core/behavior/versioned.py` & `meltano-3.4.1b1/src/meltano/core/behavior/versioned.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/block/blockset.py` & `meltano-3.4.1b1/src/meltano/core/block/blockset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/block/extract_load.py` & `meltano-3.4.1b1/src/meltano/core/block/extract_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from meltano.core.state_service import StateService
 
 from .blockset import BlockSet, BlockSetValidationError
 from .future_utils import first_failed_future, handle_producer_line_length_limit_error
 from .singer import SingerBlock
 
 if t.TYPE_CHECKING:
+    import uuid
     from pathlib import Path
 
     from sqlalchemy.orm import Session
 
     from meltano.core.plugin.project_plugin import ProjectPlugin
     from meltano.core.project import Project
 
@@ -52,36 +53,39 @@
         job: Job | None = None,
         full_refresh: bool | None = False,
         force: bool | None = False,
         update_state: bool | None = True,
         state_id_suffix: str | None = None,
         base_output_logger: OutputLogger | None = None,
         merge_state: bool | None = False,
+        run_id: uuid.UUID | None = None,
     ):
         """Use an ELBContext to pass information on to ExtractLoadBlocks.
 
         Args:
             project: The project to use.
             session: The session to use.
             job: The job within this context should run.
             full_refresh: Whether this is a full refresh.
             force: Whether to force the execution of the job if it is stale.
             update_state: Whether to update the state of the job.
             state_id_suffix: The state ID suffix to use.
             base_output_logger: The base logger to use.
             merge_state: Whether to merge state at the end of run.
+            run_id: The run ID to use.
         """
         self.project = project
         self.session = session
         self.job = job
         self.full_refresh = full_refresh
         self.force = force
         self.update_state = update_state
         self.state_id_suffix = state_id_suffix
         self.merge_state = merge_state
+        self.run_id = run_id
 
         # not yet used but required to satisfy the interface
         self.dry_run = False
         self.state = None
         self.select_filter = []
         self.catalog = None
 
@@ -118,14 +122,15 @@
         self._full_refresh = False
         self._state_update = True
         self._force = False
         self._state_id_suffix = None
         self._env = {}
         self._blocks = []
         self._merge_state = False
+        self._run_id: uuid.UUID | None = None
 
         self._base_output_logger = None
 
     def with_job(self, job: Job):
         """Set the associated job for the context.
 
         Args:
@@ -197,14 +202,26 @@
 
         Returns:
             self
         """
         self._state_id_suffix = state_id_suffix
         return self
 
+    def with_run_id(self, run_id: uuid.UUID | None):
+        """Set a run ID for this run.
+
+        Args:
+            run_id: The run ID value.
+
+        Returns:
+            self
+        """
+        self._run_id = run_id
+        return self
+
     def make_block(
         self,
         plugin: ProjectPlugin,
         plugin_args: list[str] | None = None,
     ) -> SingerBlock:
         """Create a new `SingerBlock` object, from a plugin.
 
@@ -217,15 +234,15 @@
         """
         ctx = self.plugin_context(plugin, env=self._env.copy())
 
         block = SingerBlock(
             block_ctx=ctx,
             project=self.project,
             plugin_invoker=self.invoker_for(ctx),
-            plugin_args=plugin_args,
+            plugin_args=plugin_args or (),
         )
         self._blocks.append(block)
         self._env.update(ctx.env)
         return block
 
     def plugin_context(
         self,
@@ -293,24 +310,25 @@
             job=self._job,
             full_refresh=self._full_refresh,
             force=self._force,
             update_state=self._state_update,
             state_id_suffix=self._state_id_suffix,
             base_output_logger=self._base_output_logger,
             merge_state=self._merge_state,
+            run_id=self._run_id,
         )
 
 
 class ExtractLoadBlocks(BlockSet):  # noqa: WPS214
     """`BlockSet` that supports basic EL (extract, load) patterns."""
 
     def __init__(
         self,
         context: ELBContext,
-        blocks: tuple[IOBlock],
+        blocks: tuple[IOBlock, ...],
     ):
         """Initialize a basic BlockSet suitable for executing ELT tasks.
 
         Args:
             context: the elt context to use for this elt run.
             blocks: the IOBlocks that should be used for this elt run.
         """
@@ -326,14 +344,17 @@
             state_id = generate_state_id(
                 self.context.project,
                 self.context.state_id_suffix,
                 self.head,
                 self.tail,
             )
             self.context.job = Job(job_name=state_id)
+            if self.context.run_id:
+                self.context.job.run_id = self.context.run_id
+
             job_logging_service = JobLoggingService(self.context.project)
             log_file = job_logging_service.generate_log_name(
                 self.context.job.job_name,
                 self.context.job.run_id,
             )
             self.output_logger = OutputLogger(log_file)
```

### Comparing `meltano-3.4.0b1/src/meltano/core/block/future_utils.py` & `meltano-3.4.1b1/src/meltano/core/block/future_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Various small utilities for working with futures."""
 
 from __future__ import annotations
 
 import asyncio
-import logging
 from asyncio import Task
 
+import structlog
+
 from meltano.core.runner import RunnerError
 from meltano.core.utils import human_size
 
+logger = structlog.stdlib.get_logger(__name__)
+
 
 def all_done(tasks: list[Task], done: set[Task]) -> bool:
     """Iterate through a task list checking if ALL tasks are in the done set."""
     return all(idx in done for idx in tasks)
 
 
 def first_failed_future(exception_future: Task, done: set[Task]) -> Task | None:
@@ -57,22 +60,22 @@
     if not isinstance(exception, ValueError):
         return
 
     exception = exception.__context__  # noqa: WPS609
     if not isinstance(exception, asyncio.LimitOverrunError):
         return
 
-    logging.error(
+    logger.error(
         "The extractor generated a message exceeding the message size limit "  # noqa: G004
         f"of {human_size(line_length_limit)} (half the buffer size "
         f"of {human_size(stream_buffer_size)}).",
     )
-    logging.error(
+    logger.error(
         "To let this message be processed, increase the 'elt.buffer_size' "
         "setting to at least double the size of the largest expected message, "
         "and try again.",
     )
-    logging.error(
+    logger.error(
         "To learn more, visit "
         "https://docs.meltano.com/reference/settings#eltbuffer_size",
     )
     raise RunnerError("Output line length limit exceeded") from exception  # noqa: EM101
```

### Comparing `meltano-3.4.0b1/src/meltano/core/block/ioblock.py` & `meltano-3.4.1b1/src/meltano/core/block/ioblock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/block/parser.py` & `meltano-3.4.1b1/src/meltano/core/block/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from meltano.core.block.plugin_command import PluginCommandBlock, plugin_command_invoker
 from meltano.core.block.singer import CONSUMERS, SingerBlock
 from meltano.core.plugin import PluginType
 from meltano.core.plugin.error import PluginNotFoundError
 from meltano.core.task_sets_service import TaskSetsService
 
 if t.TYPE_CHECKING:
+    import uuid
+
     import structlog
 
     from meltano.core.plugin.project_plugin import ProjectPlugin
 
 
 def is_command_block(plugin: ProjectPlugin) -> bool:
     """Check if a plugin is a command block.
@@ -70,14 +72,15 @@
         project,
         blocks: list[str],
         full_refresh: bool | None = False,
         no_state_update: bool | None = False,
         force: bool | None = False,
         state_id_suffix: str | None = None,
         merge_state: bool | None = False,
+        run_id: uuid.UUID | None = None,
     ):
         """
         Parse a meltano run command invocation into a list of blocks.
 
         Args:
             log: Logger to use.
             project: Project to use.
@@ -85,14 +88,15 @@
             full_refresh: Whether to perform a full refresh (applies to all
                 found sets).
             no_state_update: Whether to run with or without state updates.
             force: Whether to force a run if a job is already running (applies
                 to all found sets).
             state_id_suffix: State ID suffix to use.
             merge_state: Whether to merge state at end of run.
+            run_id: Custom run ID to use.
 
         Raises:
             ClickException: If a block name is not found.
         """
         self.log = log
         self.project = project
 
@@ -100,14 +104,15 @@
         self._no_state_update = no_state_update
         self._force = force
         self._state_id_suffix = state_id_suffix
         self._plugins: list[ProjectPlugin] = []
         self._commands: dict[int, str] = {}
         self._mappings_ref: dict[int, str] = {}
         self._merge_state = merge_state
+        self._run_id = run_id
 
         task_sets_service: TaskSetsService = TaskSetsService(project)
 
         blocks = self._expand_jobs(blocks, task_sets_service)
 
         for idx, name in enumerate(blocks):
             try:
@@ -240,14 +245,15 @@
         builder = (
             ELBContextBuilder(self.project)
             .with_force(self._force)
             .with_full_refresh(self._full_refresh)
             .with_no_state_update(self._no_state_update)
             .with_state_id_suffix(self._state_id_suffix)
             .with_merge_state(self._merge_state)
+            .with_run_id(self._run_id)
         )
 
         if self._plugins[offset].type != PluginType.EXTRACTORS:
             self.log.debug(
                 "next block not extractor",
                 offset=offset,
                 plugin_type=self._plugins[offset].type,
```

### Comparing `meltano-3.4.0b1/src/meltano/core/block/plugin_command.py` & `meltano-3.4.1b1/src/meltano/core/block/plugin_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/block/singer.py` & `meltano-3.4.1b1/src/meltano/core/block/singer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from meltano.core.logging import capture_subprocess_output
 from meltano.core.plugin import PluginType
 from meltano.core.runner import RunnerError
 
 if t.TYPE_CHECKING:
     from asyncio.subprocess import Process
 
+    from meltano.core.elt_context import PluginContext
     from meltano.core.logging.utils import SubprocessOutputWriter
     from meltano.core.plugin_invoker import PluginInvoker
     from meltano.core.project import Project
 
 PRODUCERS = (PluginType.EXTRACTORS, PluginType.MAPPERS)
 CONSUMERS = (PluginType.LOADERS, PluginType.MAPPERS)
 
@@ -31,15 +32,15 @@
 
 
 class InvokerBase:  # noqa: WPS230, WPS214
     """Base class for creating IOBlock's built on top of existing Meltano plugins."""
 
     def __init__(
         self,
-        block_ctx,
+        block_ctx: PluginContext,
         project: Project,
         plugin_invoker: PluginInvoker,
         command: str | None,
     ):
         """Init a wrapped plugin invoker for use as an IOBlock or PluginCommandBlock.
 
         Args:
@@ -261,18 +262,18 @@
 
 
 class SingerBlock(InvokerBase, IOBlock):
     """SingerBlock wraps singer plugins to implement the IOBlock interface."""
 
     def __init__(
         self,
-        block_ctx: dict,
+        block_ctx: PluginContext,
         project: Project,
         plugin_invoker: PluginInvoker,
-        plugin_args: tuple[str],
+        plugin_args: t.Sequence[str],
     ):
         """Configure and return a Singer plugin wrapped as an IOBlock.
 
         Args:
             block_ctx: the block context.
             project:  the project to use to obtain project settings.
             plugin_invoker: the plugin invoker.
```

### Comparing `meltano-3.4.0b1/src/meltano/core/bundle/settings.yml` & `meltano-3.4.1b1/src/meltano/core/bundle/settings.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/cli_messages.py` & `meltano-3.4.1b1/src/meltano/core/cli_messages.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/config_service.py` & `meltano-3.4.1b1/src/meltano/core/config_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Service to manage meltano.yml."""
 
 from __future__ import annotations
 
-import logging
 import os
 import typing as t
 from contextlib import contextmanager
 from functools import cached_property
 
+import structlog
 import yaml
 
 from meltano.core import bundle
 from meltano.core.setting_definition import SettingDefinition
 
 if t.TYPE_CHECKING:
     from meltano.core.meltano_file import MeltanoFile
     from meltano.core.project import Project
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class ConfigService:
     """Service to manage meltano.yml."""
 
     def __init__(self, project: Project):
         """Create a new project configuration service.
```

### Comparing `meltano-3.4.0b1/src/meltano/core/container/container_service.py` & `meltano-3.4.1b1/src/meltano/core/container/container_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/container/container_spec.py` & `meltano-3.4.1b1/src/meltano/core/container/container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/db.py` & `meltano-3.4.1b1/src/meltano/core/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Defines helpers related to the system database."""
 
 from __future__ import annotations
 
-import logging
 import time
 import typing as t
 from urllib.parse import urlparse
 
+import structlog
 from sqlalchemy import create_engine
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.pool import NullPool
 from sqlalchemy.sql import text
 
 from meltano.core.error import MeltanoError
@@ -19,14 +19,15 @@
     from sqlalchemy.engine import Connection, Engine
 
     from meltano.core.project import Project
 
 # Keep a Project → Engine mapping to serve
 # the same engine for the same Project
 _engines = {}
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class MeltanoDatabaseCompatibilityError(MeltanoError):
     """Raised when the database is not compatible with Meltano."""
 
     INSTRUCTION = (
         "Upgrade your database to be compatible with Meltano or use a different "
@@ -85,15 +86,15 @@
             if parsed_db_uri.password
             else "********@"  # token auth case
             if parsed_db_uri.username
             else ""  # no auth case
         )
         + (parsed_db_uri.hostname or ""),
     ).geturl()
-    logging.debug(
+    logger.debug(
         f"Creating DB engine for project at {str(project.root)!r} "  # noqa: G004
         f"with DB URI {sanitized_db_uri!r}",
     )
 
     if database_uri is None:
         raise NullConnectionStringError
 
@@ -138,21 +139,21 @@
     """
     attempt = 0
     while True:
         try:
             return engine.connect()
         except OperationalError:
             if attempt >= max_retries:
-                logging.error(
+                logger.error(
                     f"Could not connect to the database after {attempt} "  # noqa: G004
                     "attempts. Max retries exceeded.",
                 )
                 raise
             attempt += 1
-            logging.info(
+            logger.info(
                 f"DB connection failed. Will retry after {retry_timeout}s. "  # noqa: G004
                 f"Attempt {attempt}/{max_retries}",
             )
             time.sleep(retry_timeout)
 
 
 init_hooks: dict[str, t.Callable[[Connection], None]] = {
@@ -206,17 +207,17 @@
 
     with engine.connect() as conn, conn.begin():
         conn.execute(create_schema)
         if grant_roles:
             conn.execute(grant_select_schema)
             conn.execute(grant_usage_schema)
 
-    logging.info(f"Schema {schema_name} has been created successfully.")  # noqa: G004
+    logger.info(f"Schema {schema_name} has been created successfully.")  # noqa: G004
     for role in grant_roles:
-        logging.info(f"Usage has been granted for role: {role}.")  # noqa: G004
+        logger.info(f"Usage has been granted for role: {role}.")  # noqa: G004
 
 
 def check_database_compatibility(engine: Engine) -> None:
     """Check that the database is compatible with Meltano.
 
     Args:
         engine: The DB engine to be used. This should already be connected to
```

### Comparing `meltano-3.4.0b1/src/meltano/core/elt_context.py` & `meltano-3.4.1b1/src/meltano/core/elt_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """ELT Context."""
 
 from __future__ import annotations
 
 import typing as t
-from collections import namedtuple
 
 from meltano.core.plugin import PluginRef, PluginType
 from meltano.core.plugin.error import PluginNotFoundError
 from meltano.core.plugin.settings_service import PluginSettingsService
 from meltano.core.plugin_invoker import PluginInvoker, invoker_factory
 
 if t.TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
     from meltano.core.job import Job
     from meltano.core.logging.output_logger import OutputLogger
+    from meltano.core.plugin.project_plugin import ProjectPlugin
     from meltano.core.project import Project
 
 
-class PluginContext(
-    namedtuple("PluginContext", "plugin settings_service session"),  # noqa: WPS606
-):
+class PluginContext(t.NamedTuple):
     """Plugin Context container."""
 
+    plugin: ProjectPlugin
+    settings_service: PluginSettingsService
+    session: Session
+
     def __getattr__(self, attr: str) -> t.Any:
         """Get plugin attribute.
 
         Args:
             attr: Attribute name.
 
         Returns:
```

### Comparing `meltano-3.4.0b1/src/meltano/core/environment.py` & `meltano-3.4.1b1/src/meltano/core/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/environment_service.py` & `meltano-3.4.1b1/src/meltano/core/environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/error.py` & `meltano-3.4.1b1/src/meltano/core/error.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/hub/client.py` & `meltano-3.4.1b1/src/meltano/core/hub/client.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/hub/schema.py` & `meltano-3.4.1b1/src/meltano/core/hub/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/job/finder.py` & `meltano-3.4.1b1/src/meltano/core/job/finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/job/job.py` & `meltano-3.4.1b1/src/meltano/core/job/job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/job/stale_job_failer.py` & `meltano-3.4.1b1/src/meltano/core/job/stale_job_failer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Defines `fail_stale_jobs`."""
 
 from __future__ import annotations
 
-import logging
 import typing as t
 
+import structlog
+
 from .finder import JobFinder
 
 if t.TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 def fail_stale_jobs(session: Session, state_id: str | None = None) -> None:
     """Mark stale jobs as failed.
 
     Args:
         session: An ORM DB session.
```

### Comparing `meltano-3.4.0b1/src/meltano/core/job_state.py` & `meltano-3.4.1b1/src/meltano/core/job_state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/locked_definition_service.py` & `meltano-3.4.1b1/src/meltano/core/locked_definition_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/logging/__init__.py` & `meltano-3.4.1b1/src/meltano/core/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/logging/formatters.py` & `meltano-3.4.1b1/src/meltano/core/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/logging/job_logging_service.py` & `meltano-3.4.1b1/src/meltano/core/logging/job_logging_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
-import logging
 import os
 import typing as t
 from contextlib import contextmanager
 
+import structlog
+
 from meltano.core.utils import makedirs, slugify
 
 if t.TYPE_CHECKING:
     from pathlib import Path
 
     from meltano.core.project import Project
 
+logger = structlog.stdlib.get_logger(__name__)
 MAX_FILE_SIZE = 2097152  # 2MB max
 
 
 class MissingJobLogException(Exception):
     """Occurs when `JobLoggingService` can not find a requested log."""
 
 
@@ -70,15 +72,15 @@
 
         try:
             with open(log_file_name, "w") as log_file:
                 yield log_file
         except OSError:
             # Don't stop the Job running if you can not open the log file
             # for writing: just return /dev/null
-            logging.error(
+            logger.error(
                 f"Could open log file {log_file_name!r} for writing. "  # noqa: G004
                 "Using `/dev/null`",
             )
             with open(os.devnull, "w") as log_file:
                 yield log_file
 
     def get_latest_log(self, state_id) -> str:
```

### Comparing `meltano-3.4.0b1/src/meltano/core/logging/output_logger.py` & `meltano-3.4.1b1/src/meltano/core/logging/output_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
         Args:
             ignore_errors: A tuple of Error classes to ignore.
 
         Yields:
             With the side-effect of redirecting logging.
         """  # noqa: DAR401
-        logger = logging.getLogger()
+        logger = logging.getLogger()  # noqa: TID251
         logger.addHandler(self.redirect_log_handler)
         ignored_errors = (
             KeyboardInterrupt,
             asyncio.CancelledError,
             *ignore_errors,
         )
         try:
```

### Comparing `meltano-3.4.0b1/src/meltano/core/logging/utils.py` & `meltano-3.4.1b1/src/meltano/core/logging/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     output, but want to respect other aspects of any potential `logging.yaml`
     sourced configs. Note that if a `logging.yaml` config without a 'console'
     handler is used, this will not override the log level.
 
     Args:
         log_level: set log levels to provided level.
     """
-    root_logger = logging.getLogger()
+    root_logger = logging.getLogger()  # noqa: TID251
     root_logger.setLevel(log_level)
     for handler in root_logger.handlers:
         if handler.name == "console":
             handler.setLevel(log_level)
 
 
 class SubprocessOutputWriter(t.Protocol):
```

### Comparing `meltano-3.4.0b1/src/meltano/core/manifest/__init__.py` & `meltano-3.4.1b1/src/meltano/core/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/manifest/contexts.py` & `meltano-3.4.1b1/src/meltano/core/manifest/contexts.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/manifest/jsonschema.py` & `meltano-3.4.1b1/src/meltano/core/manifest/jsonschema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/manifest/manifest.py` & `meltano-3.4.1b1/src/meltano/core/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/meltano_file.py` & `meltano-3.4.1b1/src/meltano/core/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/meltano_invoker.py` & `meltano-3.4.1b1/src/meltano/core/meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/migration_service.py` & `meltano-3.4.1b1/src/meltano/core/migration_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 from __future__ import annotations
 
 import logging
 import typing as t
 
 import click
+import structlog
 from alembic import command
 from alembic.config import Config
 from alembic.runtime.migration import MigrationContext
 from alembic.script import ScriptDirectory
 
 from meltano.migrations import LOCK_PATH, MIGRATION_DIR
 
 if t.TYPE_CHECKING:
     from sqlalchemy.engine import Engine
 
+logger = structlog.stdlib.get_logger(__name__)
 SPLAT = "*"
 
 
 class MigrationError(Exception):
     """Generic class for migration errors."""
 
 
@@ -77,15 +79,15 @@
 
             # this connection is used in `env.py` for the migrations
             cfg.attributes["connection"] = conn
             cfg.set_main_option("script_location", str(MIGRATION_DIR))
             script = ScriptDirectory.from_config(cfg)
             # let's make sure we actually need to migrate
 
-            migration_logger = logging.getLogger("alembic.runtime.migration")
+            migration_logger = logging.getLogger("alembic.runtime.migration")  # noqa: TID251
             original_log_level = migration_logger.getEffectiveLevel()
             if silent:
                 migration_logger.setLevel(logging.ERROR)
 
             context = MigrationContext.configure(conn)
 
             try:
@@ -103,12 +105,12 @@
                 raise MigrationError(
                     "Cannot upgrade the system database, revision lock not found.",  # noqa: EM101
                 ) from ex
             except MigrationUneededException:
                 if not silent:
                     click.secho("System database up-to-date.")
             except Exception as ex:
-                logging.exception(str(ex))
+                logger.exception(str(ex))
                 raise MigrationError(
                     "Cannot upgrade the system database. It might be corrupted or "  # noqa: EM101
                     "was created before database migrations where introduced (v0.34.0)",
                 ) from ex
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/airflow.py` & `meltano-3.4.1b1/src/meltano/core/plugin/airflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Plugin glue code for Airflow."""
 
 from __future__ import annotations
 
 import configparser
-import logging
 import os
 import subprocess
 from contextlib import suppress
 
+import structlog
 from packaging.version import Version
 
 from meltano.core.behavior.hookable import hook
 from meltano.core.error import AsyncSubprocessError
 from meltano.core.plugin import BasePlugin, PluginType
 from meltano.core.plugin_invoker import PluginInvoker
 from meltano.core.utils import nest
 
+logger = structlog.stdlib.get_logger(__name__)
+
 
 class AirflowInvoker(PluginInvoker):
     """Invoker that prepares env for Airflow."""
 
     def env(self):
         """Environment variables for Airflow.
 
@@ -68,32 +70,32 @@
     def update_config_file(invoker: AirflowInvoker) -> None:
         """Update airflow.cfg with plugin configuration.
 
         Args:
             invoker: the active PluginInvoker
         """
         airflow_cfg_path = invoker.files["config"]
-        logging.debug(f"Generated default '{str(airflow_cfg_path)}'")  # noqa: G004
+        logger.debug(f"Generated default '{str(airflow_cfg_path)}'")  # noqa: G004
 
         # open the configuration and update it
         # now we let's update the config to use our stubs
         airflow_cfg = configparser.ConfigParser()
 
         with airflow_cfg_path.open() as airflow_cfg_file_to_read:
             airflow_cfg.read_file(airflow_cfg_file_to_read)
-            logging.debug(f"Loaded '{str(airflow_cfg_path)}'")  # noqa: G004
+            logger.debug(f"Loaded '{str(airflow_cfg_path)}'")  # noqa: G004
 
         config = invoker.plugin_config_processed
         for section, section_config in config.items():
             airflow_cfg[section].update(section_config)
-            logging.debug(f"\tUpdated section [{section}] with {section_config}")  # noqa: G004
+            logger.debug(f"\tUpdated section [{section}] with {section_config}")  # noqa: G004
 
         with airflow_cfg_path.open("w") as airflow_cfg_file_to_write:
             airflow_cfg.write(airflow_cfg_file_to_write)
-            logging.debug(f"Saved '{str(airflow_cfg_path)}'")  # noqa: G004
+            logger.debug(f"Saved '{str(airflow_cfg_path)}'")  # noqa: G004
 
     @hook("before_install")
     async def setup_env(self, *args, **kwargs):  # noqa: ARG002
         """Configure the env to make airflow installable without GPL deps.
 
         Args:
             args: Arbitrary args
@@ -167,20 +169,20 @@
                 (
                     "Airflow metadata database could not be initialized: "  # noqa: EM101
                     "`airflow initdb` failed"
                 ),
                 handle,
             )
 
-        logging.debug("Completed `airflow initdb`")
+        logger.debug("Completed `airflow initdb`")
 
     @hook("before_cleanup")
     async def before_cleanup(self, invoker: PluginInvoker):
         """Delete the config file.
 
         Args:
             invoker: the active PluginInvoker
         """
         config_file = invoker.files["config"]
         with suppress(FileNotFoundError):
             config_file.unlink()
-            logging.debug(f"Deleted configuration at {config_file}")  # noqa: G004
+            logger.debug(f"Deleted configuration at {config_file}")  # noqa: G004
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/base.py` & `meltano-3.4.1b1/src/meltano/core/plugin/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Base class for all Meltano plugins."""
 
 from __future__ import annotations
 
-import logging
 import re
 from collections import defaultdict
 
 import yaml
+from structlog.stdlib import get_logger
 
 from meltano.core.behavior import NameEq
 from meltano.core.behavior.canonical import Canonical
 from meltano.core.behavior.hookable import HookObject
 from meltano.core.job_state import STATE_ID_COMPONENT_DELIMITER
 from meltano.core.plugin.command import Command
 from meltano.core.plugin.requirements import PluginRequirement
 from meltano.core.setting_definition import SettingDefinition, SettingKind, YAMLEnum
 from meltano.core.utils import NotFound, find_named
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class VariantNotFoundError(Exception):
     """Raised when a variant is not found."""
 
     def __init__(self, plugin: PluginDefinition, variant_name: str):
         """Create a new VariantNotFoundError.
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/command.py` & `meltano-3.4.1b1/src/meltano/core/plugin/command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/config_service.py` & `meltano-3.4.1b1/src/meltano/core/plugin/config_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
-import logging
 import os
 import shutil
 import typing as t
 from pathlib import Path
 
+import structlog
+
 if t.TYPE_CHECKING:
     from meltano.core.plugin.project_plugin import ProjectPlugin
 
+logger = structlog.stdlib.get_logger(__name__)
+
 
 class PluginConfigService:
     """Manage the plugin configuration files.
 
     Each plugin can expose a set of files that should be stubbed using
     environment variables.
     """
@@ -43,12 +46,12 @@
         stubbed = []
         # stub the files from the env
         for dst, src in stubs:
             try:
                 shutil.copy(src, dst)
                 stubbed.append(dst)
             except FileNotFoundError:
-                logging.debug(
+                logger.debug(
                     f"Could not find {src.name} in {src.resolve()}, skipping.",  # noqa: G004
                 )
 
         return stubbed
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/dbt/base.py` & `meltano-3.4.1b1/src/meltano/core/plugin/dbt/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Defines DBT-specific plugins."""
 
 from __future__ import annotations
 
-import logging
 import typing as t
 from pathlib import Path
 
+import structlog
+
 from meltano.core.error import PluginInstallError
 from meltano.core.plugin import BasePlugin, PluginType
 from meltano.core.plugin.error import PluginNotFoundError
 from meltano.core.plugin_install_service import PluginInstaller, PluginInstallReason
 from meltano.core.plugin_invoker import PluginInvoker
 from meltano.core.setting_definition import SettingDefinition, SettingKind
 from meltano.core.transform_add_service import TransformAddService
 
 if t.TYPE_CHECKING:
     from meltano.core.plugin.project_plugin import ProjectPlugin
     from meltano.core.project import Project
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class DbtInvoker(PluginInvoker):
     """dbt plugin invoker."""
 
     def Popen_options(self):  # noqa: N802
         """Get options for `subprocess.Popen`.
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/error.py` & `meltano-3.4.1b1/src/meltano/core/plugin/error.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/factory.py` & `meltano-3.4.1b1/src/meltano/core/plugin/factory.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/file.py` & `meltano-3.4.1b1/src/meltano/core/plugin/file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/meltano_file.py` & `meltano-3.4.1b1/src/meltano/core/plugin/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/project_plugin.py` & `meltano-3.4.1b1/src/meltano/core/plugin/project_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Project Plugin Class."""
 
 from __future__ import annotations
 
 import copy
-import logging
 import typing as t
 
+import structlog
+
 from meltano.core.plugin.base import PluginDefinition, PluginRef, PluginType, Variant
 from meltano.core.plugin.command import Command
 from meltano.core.plugin.factory import base_plugin_factory
 from meltano.core.plugin.requirements import PluginRequirement
 from meltano.core.setting_definition import SettingDefinition
 from meltano.core.utils import flatten, uniques_in
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class CyclicInheritanceError(Exception):
     """Exception raised when project plugin inherits from itself cyclicly."""
 
     def __init__(self, plugin: ProjectPlugin, ancestor: ProjectPlugin):
         """Initialize cyclic inheritance error.
@@ -45,14 +46,15 @@
 
 
 class ProjectPlugin(PluginRef):  # noqa: WPS230, WPS214 # too many attrs and methods
     """ProjectPlugin class."""
 
     VARIANT_ATTR = "variant"
 
+    name: str
     variant: str | None
 
     def __init__(
         self,
         plugin_type: PluginType,
         name: str,
         inherit_from: str | None = None,
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/requirements.py` & `meltano-3.4.1b1/src/meltano/core/plugin/requirements.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/settings_service.py` & `meltano-3.4.1b1/src/meltano/core/plugin/settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/singer/base.py` & `meltano-3.4.1b1/src/meltano/core/plugin/singer/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 import json
-import logging
 from uuid import uuid4
 
+import structlog
+
 from meltano.core.behavior.hookable import hook
 from meltano.core.plugin import BasePlugin
 from meltano.core.utils import nest_object
 
+logger = structlog.stdlib.get_logger(__name__)
+
 
 class SingerPlugin(BasePlugin):
     def __init__(self, *args, **kwargs) -> None:
         """Initialize a `SingerPlugin`.
 
         Args:
             args: Positional arguments for the super class.
@@ -48,22 +51,22 @@
     ):
         """Create configuration file."""  # noqa: DAR101
         config_path = invoker.files["config"]
         with open(config_path, "w") as config_file:
             config = invoker.plugin_config_processed
             json.dump(config, config_file, indent=2)
 
-        logging.debug(f"Created configuration at {config_path}")  # noqa: G004
+        logger.debug(f"Created configuration at {config_path}")  # noqa: G004
 
     @hook("before_cleanup")
     async def before_cleanup(self, invoker):
         """Delete configuration file."""
         config_path = invoker.files["config"]
         config_path.unlink()
-        logging.debug(f"Deleted configuration at {config_path}")  # noqa: G004
+        logger.debug(f"Deleted configuration at {config_path}")  # noqa: G004
 
     @property
     def instance_uuid(self):
         """Multiple processes running at the same time have a unique value to use."""
         if not self._instance_uuid:
             self._instance_uuid = str(uuid4())
         return self._instance_uuid
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/singer/catalog.py` & `meltano-3.4.1b1/src/meltano/core/plugin/singer/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 from __future__ import annotations
 
 import fnmatch
-import logging
 import re
+import sys
 import typing as t
 from collections import OrderedDict
 from enum import Enum, auto
 from functools import singledispatch
 
+import structlog
+
 from meltano.core.behavior.visitor import visit_with
 
+if sys.version_info < (3, 11):
+    ReprEnum = Enum
+else:
+    from enum import ReprEnum
+
+logger = structlog.stdlib.get_logger(__name__)
+
 Node = t.Dict[str, t.Any]
 T = t.TypeVar("T", bound="CatalogRule")
 
+
 UNESCAPED_DOT = re.compile(r"(?<!\\)\.")
 
 
 class CatalogDict(t.TypedDict):
     """A catalog dictionary."""
 
     streams: list[dict[str, t.Any]]
@@ -285,15 +295,16 @@
 
 class CatalogNode(Enum):
     STREAM = auto()
     PROPERTY = auto()
     METADATA = auto()
 
 
-class SelectionType(str, Enum):
+# TODO: Move to `enum.StrEnum` when support for Python 3.8 is dropped
+class SelectionType(str, ReprEnum):
     """A valid stream or property selection type."""
 
     SELECTED = "selected"
     EXCLUDED = "excluded"
     AUTOMATIC = "automatic"
 
     def __bool__(self):
@@ -311,15 +322,15 @@
 
 @singledispatch
 def visit(  # noqa: D103
     node,  # noqa: ARG001
     executor,  # noqa: ARG001
     path: str = "",
 ):
-    logging.debug("Skipping node at '%s'", path)  # noqa: WPS323
+    logger.debug("Skipping node at '%s'", path)  # noqa: WPS323
 
 
 @visit.register(dict)
 def _(node: dict, executor, path=""):
     node_type = None
 
     if re.search(r"streams\[\d+\]$", path):
@@ -328,15 +339,15 @@
     if re.search(r"schema(\.properties\.\w*)+$", path):
         node_type = CatalogNode.PROPERTY
 
     if re.search(r"metadata\[\d+\]$", path) and "breadcrumb" in node:
         node_type = CatalogNode.METADATA
 
     if node_type:
-        logging.debug("Visiting %s at '%s'.", node_type, path)  # noqa: WPS323
+        logger.debug("Visiting %s at '%s'.", node_type, path)  # noqa: WPS323
         executor(node_type, node, path)
 
     for child_path, child_node in node.items():
         if node_type is CatalogNode.PROPERTY and child_path in {"anyOf", "type"}:
             continue
 
         # TODO mbergeron: refactor this to use a dynamic visitor per CatalogNode
@@ -357,16 +368,16 @@
             CatalogNode.STREAM: self.stream_node,
             CatalogNode.PROPERTY: self.property_node,
             CatalogNode.METADATA: self.metadata_node,
         }
 
         try:
             dispatch[node_type](node, path)
-        except KeyError:
-            logging.debug("Unknown node type '%s'.", node_type)  # noqa: WPS323
+        except KeyError:  # pragma: no cover
+            logger.debug("Unknown node type '%s'.", node_type)  # noqa: WPS323
 
     def stream_node(self, node: Node, path: str):
         """Process stream node."""
 
     def property_node(self, node: Node, path: str):
         """Process property node."""
 
@@ -448,15 +459,15 @@
         self.ensure_metadata(breadcrumb)
 
     def metadata_node(self, node: Node, path: str):
         """Process metadata node."""
         tap_stream_id = self._stream["tap_stream_id"]
         breadcrumb = node["breadcrumb"]
 
-        logging.debug(
+        logger.debug(
             "Visiting metadata node for tap_stream_id '%s', breadcrumb '%s'",  # noqa: WPS323, E501
             tap_stream_id,
             breadcrumb,
         )
 
         for rule in MetadataRule.matching(self._rules, tap_stream_id, breadcrumb):
             self.set_metadata(
@@ -473,15 +484,15 @@
             key == "selected"
             and value is True
             and node.get("inclusion") == "unsupported"
         ):
             return
 
         node[key] = value
-        logging.debug("Setting '%s.%s' to '%s'", path, key, value)  # noqa: WPS323
+        logger.debug("Setting '%s.%s' to '%s'", path, key, value)  # noqa: WPS323
 
 
 class SelectExecutor(MetadataExecutor):
     def __init__(self, patterns: list[str]):
         super().__init__(select_metadata_rules(patterns))
 
 
@@ -538,15 +549,15 @@
         for rule in SchemaRule.matching(self._rules, tap_stream_id, breadcrumb):
             self.set_payload(node, path, rule.payload)
 
     def set_payload(self, node: Node, path: str, payload: dict):
         """Set node payload from a clean mapping."""
         node.clear()
         node.update(payload)
-        logging.debug("Setting '%s' to %r", path, payload)  # noqa: WPS323
+        logger.debug("Setting '%s' to %r", path, payload)  # noqa: WPS323
 
 
 class ListExecutor(CatalogExecutor):
     def __init__(self):
         # properties per stream
         self.properties: dict[str, set[str]] = OrderedDict()
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/singer/mapper.py` & `meltano-3.4.1b1/src/meltano/core/plugin/singer/mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,23 +54,31 @@
         session,  # noqa: ARG002
     ):
         """Create configuration file."""  # noqa: DAR101
         config_path = invoker.files["config"]
 
         config_payload: dict = {}
         with open(config_path, "w") as config_file:
-            config_payload = self._get_mapping_config(invoker.plugin.extra_config)
+            config_payload = {
+                **invoker.plugin_config_processed,
+                **self._get_mapping_config(invoker.plugin.extra_config),
+            }
             json.dump(config_payload, config_file, indent=2)
 
         logger.debug(
             "Created configuration",
             config_path=config_path,
             plugin_name=invoker.plugin.name,
             mapping_name=invoker.plugin_config_extras["_mapping_name"],
             mapping_config=config_payload,
         )
 
     @staticmethod
-    def _get_mapping_config(extra_config: dict) -> dict | None:
-        for mapping in extra_config.get("_mappings", []):  # noqa: RET503
-            if mapping.get("name") == extra_config.get("_mapping_name"):
-                return mapping["config"]
+    def _get_mapping_config(extra_config: dict) -> dict:
+        return next(
+            (
+                mapping.get("config", {})
+                for mapping in extra_config.get("_mappings", [])
+                if mapping.get("name") == extra_config.get("_mapping_name")
+            ),
+            {},
+        )
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/singer/tap.py` & `meltano-3.4.1b1/src/meltano/core/plugin/singer/tap.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
             with suppress(FileNotFoundError):
                 cached_key = catalog_cache_key_path.read_text()
                 new_cache_key = self.catalog_cache_key(plugin_invoker)
 
                 if cached_key == new_cache_key:
                     logger.debug("Using cached catalog file")
                     return
-            logging.debug("Cached catalog is outdated, running discovery...")
+            logger.debug("Cached catalog is outdated, running discovery...")
 
         # We're gonna generate a new catalog, so delete the cache key.
         with suppress(FileNotFoundError):
             catalog_cache_key_path.unlink()
 
         if custom_catalog_filename := plugin_invoker.plugin_config_extras["_catalog"]:
             custom_catalog_path = plugin_invoker.project.root.joinpath(
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/singer/target.py` & `meltano-3.4.1b1/src/meltano/core/plugin/singer/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """SingerTarget and supporting classes."""
 
 from __future__ import annotations
 
 import json
-import logging
 import typing as t
 from datetime import datetime
 
+from structlog.stdlib import get_logger
+
 from meltano.core.behavior.hookable import hook
 from meltano.core.job import Job, Payload
 from meltano.core.setting_definition import SettingDefinition
 from meltano.core.state_service import SINGER_STATE_KEY, StateService
 
 from . import PluginType, SingerPlugin
 
 if t.TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
     from meltano.core.plugin_invoker import PluginInvoker
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class BookmarkWriter:
     """A basic bookmark writer suitable for use as an output handler.
 
     Has a writelines method to support ingesting and persisting state messages.
     """
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin/superset.py` & `meltano-3.4.1b1/src/meltano/core/plugin/superset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Plugin glue code for Superset."""
 
 from __future__ import annotations
 
-import logging
 import subprocess
 from contextlib import suppress
 
 import structlog
 
 from meltano.core.behavior.hookable import hook
 from meltano.core.error import AsyncSubprocessError
@@ -102,15 +101,15 @@
                 ],
             )
 
             logger.info(f"Merged in config from {custom_config_path}")  # noqa: G004
         config_path = invoker.files["config"]
         with open(config_path, "w") as config_file:
             config_file.write("\n".join(config_script_lines))
-        logging.debug(f"Created configuration at {config_path}")  # noqa: G004
+        logger.debug(f"Created configuration at {config_path}")  # noqa: G004
 
     @hook("before_invoke")
     async def db_upgrade_hook(
         self,
         invoker: PluginInvoker,
         exec_args: list[str],  # noqa: ARG002
     ):
@@ -136,15 +135,15 @@
                 (
                     "Superset metadata database could not be initialized: "  # noqa: EM101
                     "`superset db upgrade` failed"
                 ),
                 handle,
             )
 
-        logging.debug("Completed `superset db upgrade`")
+        logger.debug("Completed `superset db upgrade`")
 
     @hook("before_invoke")
     async def init_hook(
         self,
         invoker: PluginInvoker,
         exec_args: list[str],  # noqa: ARG002
     ):
@@ -169,20 +168,20 @@
                 (
                     "Superset default roles and permissions could not be "  # noqa: EM101
                     "created: `superset init` failed"
                 ),
                 handle,
             )
 
-        logging.debug("Completed `superset init`")
+        logger.debug("Completed `superset init`")
 
     @hook("before_cleanup")
     async def before_cleanup(self, invoker: PluginInvoker):
         """Delete the config file.
 
         Args:
             invoker: the active PluginInvoker
         """
         config_file = invoker.files["config"]
         with suppress(FileNotFoundError):
             config_file.unlink()
-            logging.debug(f"Deleted configuration at {config_file}")  # noqa: G004
+            logger.debug(f"Deleted configuration at {config_file}")  # noqa: G004
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin_install_service.py` & `meltano-3.4.1b1/src/meltano/core/plugin_install_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Install plugins into the project, using pip in separate venv by default."""
 
 from __future__ import annotations
 
 import asyncio
 import functools
-import logging
 import os
 import shlex
 import sys
 import typing as t
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 from multiprocessing import cpu_count
 
+import structlog
+
 from meltano.core.error import (
     AsyncSubprocessError,
     PluginInstallError,
     PluginInstallWarning,
 )
 from meltano.core.plugin import PluginType
 from meltano.core.plugin.settings_service import PluginSettingsService
@@ -25,15 +26,15 @@
 from meltano.core.utils import EnvVarMissingBehavior, expand_env_vars, noop
 from meltano.core.venv_service import UvVenvService, VenvService
 
 if t.TYPE_CHECKING:
     from meltano.core.plugin.project_plugin import ProjectPlugin
     from meltano.core.project import Project
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class PluginInstallReason(str, Enum):
     """Plugin install reason enum."""
 
     ADD = "add"
     INSTALL = "install"
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin_invoker.py` & `meltano-3.4.1b1/src/meltano/core/plugin_invoker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Plugin invoker class."""
 
 from __future__ import annotations
 
 import asyncio
 import enum
-import logging
 import os
 import typing as t
 import uuid
 from contextlib import asynccontextmanager
 
 from structlog.stdlib import get_logger
 
@@ -20,14 +19,16 @@
 from meltano.core.tracking import Tracker
 from meltano.core.utils import EnvVarMissingBehavior, expand_env_vars
 from meltano.core.venv_service import VenvService, VirtualEnv
 
 if t.TYPE_CHECKING:
     from pathlib import Path
 
+    from sqlalchemy.orm import Session
+
     from meltano.core.logging.utils import SubprocessOutputWriter
     from meltano.core.plugin import PluginRef
     from meltano.core.plugin.project_plugin import ProjectPlugin
     from meltano.core.project import Project
 
 logger = get_logger(__name__)
 
@@ -202,15 +203,15 @@
         """
         plugin_files = {**self.plugin.config_files, **self.plugin.output_files}
         return {
             _key: self.plugin_config_service.run_dir.joinpath(filename)
             for _key, filename in plugin_files.items()
         }
 
-    async def prepare(self, session):
+    async def prepare(self, session: Session):
         """Prepare plugin config.
 
         Args:
             session: Database session.
         """
         self.plugin_config = self.settings_service.as_dict(
             extras=False,
@@ -237,15 +238,15 @@
         self.plugin_config_extras = {}
         self.plugin_config_env = {}
 
         async with self.plugin.trigger_hooks("cleanup", self):
             self._prepared = False
 
     @asynccontextmanager
-    async def prepared(self, session):
+    async def prepared(self, session: Session):
         """Context manager that prepares plugin config.
 
         Args:
             session: Database session.
 
         Yields:
             Yields to the caller, then resetting the config.
@@ -424,15 +425,15 @@
         if require_preparation and not self._prepared:
             raise InvokerNotPreparedError
 
         async with self.plugin.trigger_hooks("invoke", self, args):
             popen_options = {**self.Popen_options(), **kwargs}
             popen_env = {**self.env(), **env}
             popen_args = self.exec_args(*args, command=command, env=popen_env)
-            logging.debug(f"Invoking: {popen_args}")  # noqa: G004
+            logger.debug(f"Invoking: {popen_args}")  # noqa: G004
 
             try:
                 yield (popen_args, popen_options, popen_env)
             except FileNotFoundError as err:
                 raise ExecutableNotFoundError(
                     self.plugin,
                     self.plugin.executable,
```

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin_location_remove.py` & `meltano-3.4.1b1/src/meltano/core/plugin_location_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin_lock_service.py` & `meltano-3.4.1b1/src/meltano/core/plugin_lock_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin_remove_service.py` & `meltano-3.4.1b1/src/meltano/core/plugin_remove_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin_repository.py` & `meltano-3.4.1b1/src/meltano/core/plugin_repository.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/plugin_test_service.py` & `meltano-3.4.1b1/src/meltano/core/plugin_test_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Defines PluginTestService."""
 
 from __future__ import annotations
 
 import asyncio
 import json
-import logging
 import typing as t
 from abc import ABC, abstractmethod
 
+import structlog
+
 from meltano.core.plugin.base import PluginType
 from meltano.core.plugin.error import PluginNotSupportedError
 
 if t.TYPE_CHECKING:
     from meltano.core.plugin_invoker import PluginInvoker
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class PluginTestServiceFactory:
     """Factory class to resolve a plugin test service."""
 
     def __init__(self, plugin_invoker: PluginInvoker):
         """Construct a PluginTestServiceFactory instance.
@@ -76,33 +77,34 @@
             process = await self.plugin_invoker.invoke_async(
                 stdout=asyncio.subprocess.PIPE,
                 stderr=asyncio.subprocess.STDOUT,
             )
         except Exception as exc:
             return False, str(exc)
 
-        last_line = None
+        record_message_received: bool = False
+        last_line: str | None = None
+
         while process.stdout and not process.stdout.at_eof():
             data = await process.stdout.readline()
             line = data.decode("utf-8").strip()
             if line:
                 logger.debug(line)
                 last_line = line
 
             try:
                 message_type = json.loads(line)["type"]
             except (json.decoder.JSONDecodeError, KeyError):
                 continue
 
-            if message_type == "RECORD":
+            record_message_received = message_type == "RECORD"
+            if record_message_received:
                 process.terminate()
                 break
 
         returncode = await process.wait()
+        logger.debug("Process return code: %s", returncode)
 
-        # Considered valid if subprocess is terminated (exit status < 0) on
-        # RECORD message received. See
-        # https://docs.python.org/3/library/subprocess.html#subprocess.CompletedProcess.returncode  # noqa: E501
         return (
-            returncode < 0,
+            record_message_received,
             last_line if returncode else "No RECORD message received",
         )
```

### Comparing `meltano-3.4.0b1/src/meltano/core/project.py` & `meltano-3.4.1b1/src/meltano/core/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Meltano Projects."""
 
 from __future__ import annotations
 
 import errno
-import logging
 import os
 import sys
 import threading
 import typing as t
 from contextlib import contextmanager
 from functools import cached_property
 from pathlib import Path
 
 import fasteners  # type: ignore[import-untyped]
+import structlog
 from dotenv import dotenv_values
 
 from meltano.core import yaml
 from meltano.core.behavior.versioned import Versioned
 from meltano.core.config_service import ConfigService
 from meltano.core.environment import Environment
 from meltano.core.error import (
@@ -38,15 +38,15 @@
         from typing import TypeAlias
     else:
         from typing_extensions import TypeAlias
 
 
 StrPath: TypeAlias = t.Union[str, os.PathLike]
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 PROJECT_ROOT_ENV = "MELTANO_PROJECT_ROOT"
 PROJECT_ENVIRONMENT_ENV = "MELTANO_ENVIRONMENT"
 PROJECT_READONLY_ENV = "MELTANO_PROJECT_READONLY"
 PROJECT_SYS_DIR_ROOT_ENV = "MELTANO_SYS_DIR_ROOT"
```

### Comparing `meltano-3.4.0b1/src/meltano/core/project_add_service.py` & `meltano-3.4.1b1/src/meltano/core/project_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/project_files.py` & `meltano-3.4.1b1/src/meltano/core/project_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Module for handling multiple project .yml files."""
 
 from __future__ import annotations
 
-import logging
 import typing as t
 from collections import OrderedDict
 from copy import copy
 
+import structlog
 from atomicwrites import atomic_write
 from ruamel.yaml import CommentedMap, CommentedSeq, YAMLError
 
 from meltano.core import yaml
 from meltano.core.utils import deep_merge
 
 if t.TYPE_CHECKING:
     from os import PathLike
     from pathlib import Path
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 BLANK_SUBFILE = CommentedMap(
     [
         ("plugins", {}),
         ("schedules", []),
         ("jobs", []),
         ("environments", []),
```

### Comparing `meltano-3.4.0b1/src/meltano/core/project_init_service.py` & `meltano-3.4.1b1/src/meltano/core/project_init_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/project_plugins_service.py` & `meltano-3.4.1b1/src/meltano/core/project_plugins_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/project_settings_service.py` & `meltano-3.4.1b1/src/meltano/core/project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/runner/dbt.py` & `meltano-3.4.1b1/src/meltano/core/runner/dbt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/runner/singer.py` & `meltano-3.4.1b1/src/meltano/core/runner/singer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from __future__ import annotations
 
 import asyncio
-import logging
 import subprocess
 import sys
 import typing as t
 
+import structlog
+
 from meltano.core.logging import capture_subprocess_output
 from meltano.core.plugin import PluginType
 from meltano.core.runner import Runner, RunnerError
 from meltano.core.utils import human_size
 
 if t.TYPE_CHECKING:
     from meltano.core.elt_context import ELTContext
     from meltano.core.plugin_invoker import PluginInvoker
 
 
+logger = structlog.stdlib.get_logger(__name__)
+
+
 class SingerRunner(Runner):
     def __init__(self, elt_context: ELTContext):
         self.context = elt_context
 
     def stop(self, process, **wait_args):
-        while True:
+        while True:  # pragma: no cover
             try:
                 code = process.wait(**wait_args)
-                logging.debug(f"{process} exited with {code}")  # noqa: G004
+                logger.debug(f"{process} exited with {code}")  # noqa: G004
                 return code
             except subprocess.TimeoutExpired:
                 process.kill()
-                logging.error(f"{process} was killed.")  # noqa: G004
+                logger.error(f"{process} was killed.")  # noqa: G004
 
     async def invoke(  # noqa: WPS210, WPS213, WPS217, WPS231, WPS238
         self,
         tap: PluginInvoker,
         target: PluginInvoker,
         extractor_log=None,
         loader_log=None,
@@ -197,17 +201,17 @@
             )
         if tap_code:
             raise RunnerError("Extractor failed", {PluginType.EXTRACTORS: tap_code})  # noqa: EM101
         if target_code:
             raise RunnerError("Loader failed", {PluginType.LOADERS: target_code})  # noqa: EM101
 
     def dry_run(self, tap: PluginInvoker, target: PluginInvoker):
-        logging.info("Dry run:")
-        logging.info(f"\textractor: {tap.plugin.name} at '{tap.exec_path()}'")  # noqa: G004
-        logging.info(f"\tloader: {target.plugin.name} at '{target.exec_path()}'")  # noqa: G004
+        logger.info("Dry run:")
+        logger.info(f"\textractor: {tap.plugin.name} at '{tap.exec_path()}'")  # noqa: G004
+        logger.info(f"\tloader: {target.plugin.name} at '{target.exec_path()}'")  # noqa: G004
 
     async def run(
         self,
         extractor_log=None,
         loader_log=None,
         extractor_out=None,
         loader_out=None,
@@ -238,25 +242,25 @@
     ):
         # StreamReader.readline can raise a ValueError wrapping a LimitOverrunError:
         # https://github.com/python/cpython/blob/v3.8.7/Lib/asyncio/streams.py#L549
         if not isinstance(exception, ValueError):
             return
 
         exception = exception.__context__  # noqa: WPS609
-        if not isinstance(exception, asyncio.LimitOverrunError):
+        if not isinstance(exception, asyncio.LimitOverrunError):  # pragma: no cover
             return
 
-        logging.error(
+        logger.error(
             f"The extractor generated a message exceeding the message size "  # noqa: G004
             f"limit of {human_size(line_length_limit)} (half the buffer size "
             f"of {human_size(stream_buffer_size)}).",
         )
-        logging.error(
+        logger.error(
             "To let this message be processed, increase the 'elt.buffer_size' "
             "setting to at least double the size of the largest expected "
             "message, and try again.",
         )
-        logging.error(
+        logger.error(
             "To learn more, visit "
             "https://docs.meltano.com/reference/settings#eltbuffer_size",
         )
         raise RunnerError("Output line length limit exceeded") from exception  # noqa: EM101
```

### Comparing `meltano-3.4.0b1/src/meltano/core/schedule.py` & `meltano-3.4.1b1/src/meltano/core/schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/schedule_service.py` & `meltano-3.4.1b1/src/meltano/core/schedule_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Service for managing meltano schedules."""
 
 from __future__ import annotations
 
-import logging
 import typing as t
 from datetime import date, datetime
 
+import structlog
 from croniter import croniter
 
 from meltano.core.error import MeltanoError
 from meltano.core.locked_definition_service import PluginNotFoundError
 from meltano.core.meltano_invoker import MeltanoInvoker
 from meltano.core.plugin import PluginType
 from meltano.core.plugin.settings_service import PluginSettingsService
@@ -19,14 +19,16 @@
 from meltano.core.utils import NotFound, coerce_datetime, find_named, iso8601_datetime
 
 if t.TYPE_CHECKING:
     import subprocess
 
     from meltano.core.project import Project
 
+logger = structlog.stdlib.get_logger(__name__)
+
 
 class ScheduleAlreadyExistsError(MeltanoError):
     """A schedule already exists."""
 
     def __init__(self, schedule: Schedule):
         """Initialize the exception.
 
@@ -188,15 +190,15 @@
             plugin_type=PluginType.EXTRACTORS,
         )
         start_date: str | datetime | date | None = None
         try:
             settings_service = PluginSettingsService(self.project, extractor_plugin)
             start_date = settings_service.get("start_date", session=session)
         except SettingMissingError:
-            logging.debug(f"`start_date` not found in {extractor_plugin}.")  # noqa: G004
+            logger.debug(f"`start_date` not found in {extractor_plugin}.")  # noqa: G004
 
         # TODO: this coercion should be handled by the `kind` attribute
         # on the actual setting
         if isinstance(start_date, date):
             return coerce_datetime(start_date)
 
         if isinstance(start_date, datetime):
```

### Comparing `meltano-3.4.0b1/src/meltano/core/select_service.py` & `meltano-3.4.1b1/src/meltano/core/select_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/setting.py` & `meltano-3.4.1b1/src/meltano/core/setting.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/setting_definition.py` & `meltano-3.4.1b1/src/meltano/core/setting_definition.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/settings_service.py` & `meltano-3.4.1b1/src/meltano/core/settings_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Module for managing settings."""
 
 from __future__ import annotations
 
-import logging
 import os
 import typing as t
 import warnings
 from abc import ABCMeta, abstractmethod
 from contextlib import contextmanager, suppress
 from enum import Enum
 
+import structlog
+
 from meltano.core.setting_definition import (
     SettingDefinition,
     SettingKind,
     SettingMissingError,
 )
 from meltano.core.settings_store import SettingValueStore
 from meltano.core.utils import EnvVarMissingBehavior, flatten
 from meltano.core.utils import expand_env_vars as do_expand_env_vars
 
 if t.TYPE_CHECKING:
     from meltano.core.project import Project
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 # sentinel value to use to prevent leaking sensitive data
 REDACTED_VALUE = "(redacted)"
 
 # magic string used as feature flag setting for experimental features
 EXPERIMENTAL = "experimental"
```

### Comparing `meltano-3.4.0b1/src/meltano/core/settings_store.py` & `meltano-3.4.1b1/src/meltano/core/settings_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Storage Managers for Meltano Configuration."""
 
 from __future__ import annotations
 
-import logging
 import typing as t
 from abc import ABC, abstractmethod
 from contextlib import contextmanager, suppress
 from copy import deepcopy
 from enum import Enum
 from functools import reduce
 from operator import eq
 
 import dotenv
 import sqlalchemy
+import structlog
 
 from meltano.core.environment import NoActiveEnvironment
 from meltano.core.error import Error, ProjectReadonly
 from meltano.core.setting import Setting
 from meltano.core.setting_definition import SettingDefinition, SettingMissingError
 from meltano.core.utils import flatten, pop_at_path, set_at_path
 
 if t.TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
     from meltano.core.settings_service import SettingsService
 
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class ConflictingSettingValueException(Exception):  # noqa: N818
     """A setting has multiple conflicting values via aliases."""
 
     def __init__(self, setting_names):
         """Instantiate the error.
```

### Comparing `meltano-3.4.0b1/src/meltano/core/sqlalchemy.py` & `meltano-3.4.1b1/src/meltano/core/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/state_service.py` & `meltano-3.4.1b1/src/meltano/core/state_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/state_store/__init__.py` & `meltano-3.4.1b1/src/meltano/core/state_store/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/state_store/azure.py` & `meltano-3.4.1b1/src/meltano/core/state_store/azure.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/state_store/base.py` & `meltano-3.4.1b1/src/meltano/core/state_store/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,22 +20,20 @@
 class StateIDLockedError(Exception):
     """A job attempted to acquire a lock on an already-locked state ID."""
 
 
 class StateStoreManager(ABC):
     """Base state store manager."""
 
-    @abstractmethod
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs):  # noqa: B027
         """Initialize state store manager.
 
         Args:
             kwargs: additional keyword arguments
         """
-        ...
 
     @abstractproperty
     def label(self) -> str:
         """Get the label for the StateStoreManager."""
         ...
 
     @abstractmethod
```

### Comparing `meltano-3.4.0b1/src/meltano/core/state_store/db.py` & `meltano-3.4.1b1/src/meltano/core/state_store/db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/state_store/filesystem.py` & `meltano-3.4.1b1/src/meltano/core/state_store/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """StateStoreManagers for filesystems."""
 
 from __future__ import annotations
 
 import glob
-import logging
 import os
 import re
 import shutil
 import typing as t
 from abc import abstractmethod, abstractproperty
 from base64 import b64decode, b64encode
 from contextlib import contextmanager
 from datetime import datetime, timedelta
 from functools import reduce
 from pathlib import Path
 from time import sleep
 from urllib.parse import urlparse
 
+import structlog
 from smart_open import open  # type: ignore
 
 from meltano.core.job_state import JobState
 from meltano.core.state_store.base import StateStoreManager
 from meltano.core.utils import remove_suffix
 
 if t.TYPE_CHECKING:
     from collections.abc import Iterator
     from io import TextIOWrapper
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class InvalidStateBackendConfigurationException(Exception):
     """State backend configuration is invalid."""
 
 
 class BaseFilesystemStateStoreManager(StateStoreManager):  # noqa: WPS214
```

### Comparing `meltano-3.4.0b1/src/meltano/core/state_store/google.py` & `meltano-3.4.1b1/src/meltano/core/state_store/google.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/state_store/s3.py` & `meltano-3.4.1b1/src/meltano/core/state_store/s3.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/task_sets.py` & `meltano-3.4.1b1/src/meltano/core/task_sets.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/task_sets_service.py` & `meltano-3.4.1b1/src/meltano/core/task_sets_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/README.md` & `meltano-3.4.1b1/src/meltano/core/tracking/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/contexts/cli.py` & `meltano-3.4.1b1/src/meltano/core/tracking/contexts/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/contexts/environment.py` & `meltano-3.4.1b1/src/meltano/core/tracking/contexts/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/contexts/exception.py` & `meltano-3.4.1b1/src/meltano/core/tracking/contexts/exception.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/contexts/plugins.py` & `meltano-3.4.1b1/src/meltano/core/tracking/contexts/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Tracking plugin context for the Snowplow tracker."""
 
 from __future__ import annotations
 
 import typing as t
 import uuid
 
+import structlog
 from snowplow_tracker import SelfDescribingJson
-from structlog.stdlib import get_logger
 
 from meltano.core.block.blockset import BlockSet
 from meltano.core.block.plugin_command import PluginCommandBlock
 from meltano.core.tracking.schemas import PluginsContextSchema
 from meltano.core.utils import hash_sha256, safe_hasattr
 
 if t.TYPE_CHECKING:
     from meltano.core.elt_context import ELTContext
     from meltano.core.plugin.project_plugin import ProjectPlugin
 
-logger = get_logger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 def _from_plugin(plugin: ProjectPlugin, cmd: str | None) -> dict:
     if not plugin or not safe_hasattr(plugin, "info"):
         # Don't try to snag any info for this plugin, we're somehow badly
         # malformed (unittest?), or where passed None. This event will be
         # routed to the "bad" bucket on the snowplow side. That makes it
```

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/contexts/project.py` & `meltano-3.4.1b1/src/meltano/core/tracking/contexts/project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0` & `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/micro.conf` & `meltano-3.4.1b1/src/meltano/core/tracking/micro.conf`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/schemas.py` & `meltano-3.4.1b1/src/meltano/core/tracking/schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/tracking/tracker.py` & `meltano-3.4.1b1/src/meltano/core/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/transform_add_service.py` & `meltano-3.4.1b1/src/meltano/core/transform_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/upgrade_service.py` & `meltano-3.4.1b1/src/meltano/core/upgrade_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/core/utils/__init__.py` & `meltano-3.4.1b1/src/meltano/core/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from __future__ import annotations
 
 import asyncio
 import collections
 import functools
 import hashlib
-import logging
 import math
 import os
 import platform
 import re
 import sys
 import traceback
 import typing as t
@@ -20,19 +19,20 @@
 from datetime import date, datetime, time
 from enum import IntEnum
 from functools import reduce
 from operator import setitem
 from pathlib import Path
 
 import flatten_dict
+import structlog
 from requests.auth import HTTPBasicAuth
 
 from meltano.core.error import MeltanoError
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 TRUTHY = ("true", "1", "yes", "on")
 REGEX_EMAIL = r"(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$)"
 
 
 try:
     # asyncio.Task.all_tasks() is fully moved to asyncio.all_tasks() starting
```

### Comparing `meltano-3.4.0b1/src/meltano/core/utils/pidfile.py` & `meltano-3.4.1b1/src/meltano/core/utils/pidfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-import logging
 from pathlib import Path
 
 import psutil
+import structlog
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 
 class PIDFile:
     def __init__(self, path: str | Path):
         self.path = Path(path)
         self._pid = None
```

### Comparing `meltano-3.4.0b1/src/meltano/core/validation_service.py` & `meltano-3.4.1b1/src/meltano/core/validation_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from abc import ABCMeta, abstractmethod
 from enum import Enum
 
 from meltano.core.plugin import PluginType
 from meltano.core.plugin_invoker import PluginInvoker, invoker_factory
 
 if t.TYPE_CHECKING:
-    from sqlalchemy.orm.session import sessionmaker
+    from sqlalchemy.orm.session import Session
 
     from meltano.core.project import Project
 
 EXIT_CODE_OK = 0
 
 T = t.TypeVar("T", bound="ValidationsRunner")  # noqa: WPS111
 
@@ -90,15 +90,15 @@
             ) from exc
 
     def select_all(self) -> None:
         """Mark all plugin validators as selected."""
         for name in self.tests_selection:
             self.tests_selection[name] = True
 
-    async def run_all(self, session: sessionmaker) -> dict[str, int]:
+    async def run_all(self, session: Session) -> dict[str, int]:
         """Run all validators defined in a plugin.
 
         Args:
             session: A SQLAlchemy ORM session.
 
         Returns:
             A mapping of validator names to exit codes.
```

### Comparing `meltano-3.4.0b1/src/meltano/core/venv_service.py` & `meltano-3.4.1b1/src/meltano/core/venv_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Manage Python virtual environments."""
 
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import hashlib
-import logging
 import os
 import platform
 import shlex
 import shutil
 import subprocess
 import sys
 import typing as t
 from asyncio.subprocess import Process
 from functools import cached_property, lru_cache
 from numbers import Number
 from pathlib import Path
 
+import structlog
+
 from meltano.core.error import AsyncSubprocessError, MeltanoError
 
 if t.TYPE_CHECKING:
     from collections.abc import Iterable
 
     from meltano.core.project import Project
 
@@ -32,15 +33,15 @@
 
 if sys.version_info < (3, 12):
     from typing_extensions import override
 else:
     from typing import override
 
 
-logger = logging.getLogger(__name__)
+logger = structlog.stdlib.get_logger(__name__)
 
 StdErrExtractor: TypeAlias = t.Callable[[Process], t.Awaitable[t.Union[str, None]]]
 
 
 @lru_cache(maxsize=None)
 def find_uv() -> str:
     """Find the `uv` executable.
```

### Comparing `meltano-3.4.0b1/src/meltano/core/yaml.py` & `meltano-3.4.1b1/src/meltano/core/yaml.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/env.py` & `meltano-3.4.1b1/src/meltano/migrations/env.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/utils/dialect_typing.py` & `meltano-3.4.1b1/src/meltano/migrations/utils/dialect_typing.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/6ef30ab7b8e5_.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/6ef30ab7b8e5_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/b4c05e463b53_.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/b4c05e463b53_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py` & `meltano-3.4.1b1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/src/meltano/schemas/meltano.schema.json` & `meltano-3.4.1b1/src/meltano/schemas/meltano.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999975887345679%*

 * *Differences: {"'$defs'": "{'schedules': {'properties': {'interval': {'pattern': "*

 * *            "'^((@(hourly|daily|weekly|monthly|yearly|once))|((((\\\\d+,)+\\\\d+|(\\\\d+|\\\\*)(\\\\/|-)\\\\d+|\\\\d+|\\\\*) "*

 * *            "?){5,6}))$'}}}}"}*

```diff
@@ -863,15 +863,15 @@
                     "description": "A UNIX cron expression to represent the frequency the scheduled job should execute",
                     "examples": [
                         "@hourly",
                         "@daily",
                         "@weekly",
                         "0 0 * * *"
                     ],
-                    "pattern": "^((@(hourly|daily|weekly|monthly|yearly|once))|((((\\d+,)+\\d+|(\\d+(\\/|-)\\d+)|\\d+|\\*) ?){5,6}))$",
+                    "pattern": "^((@(hourly|daily|weekly|monthly|yearly|once))|((((\\d+,)+\\d+|(\\d+|\\*)(\\/|-)\\d+|\\d+|\\*) ?){5,6}))$",
                     "type": "string"
                 },
                 "job": {
                     "description": "The name of a meltano job",
                     "examples": [
                         "some-custom-job"
                     ],
```

### Comparing `meltano-3.4.0b1/tests/conftest.py` & `meltano-3.4.1b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/cli.py` & `meltano-3.4.1b1/tests/fixtures/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             assert not self.snowplow.bad()  # pragma: no cover
         return results
 
 
 @pytest.fixture()
 def cli_runner(pushd, snowplow_optional: SnowplowMicro | None):
     pushd(os.getcwd())  # Ensure we return to the CWD after the test
-    root_logger = logging.getLogger()
+    root_logger = logging.getLogger()  # noqa: TID251
     log_level = root_logger.level
     try:
         yield MeltanoCliRunner(mix_stderr=False, snowplow=snowplow_optional)
     finally:
         root_logger.setLevel(log_level)
```

### Comparing `meltano-3.4.0b1/tests/fixtures/core.py` & `meltano-3.4.1b1/tests/fixtures/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2068,30 +2068,30 @@
 def job_logging_service(project):
     return JobLoggingService(project)
 
 
 @contextmanager
 def project_directory(project_init_service):
     project = project_init_service.init()
-    logging.debug(f"Created new project at {project.root}")  # noqa: G004
+    logging.debug(f"Created new project at {project.root}")  # noqa: G004, TID251
 
     # empty out the `plugins`
     with project.meltano_update() as meltano:
         meltano.plugins = Canonical()
 
     ProjectSettingsService(project).set("snowplow.collector_endpoints", "[]")
 
     # cd into the new project root
     os.chdir(project.root)
 
     try:
         yield project
     finally:
         Project.deactivate()
-        logging.debug(f"Cleaned project at {project.root}")  # noqa: G004
+        logging.debug(f"Cleaned project at {project.root}")  # noqa: G004, TID251
 
 
 @pytest.fixture(scope="class")
 def project(project_init_service, tmp_path_factory: pytest.TempPathFactory):
     with cd(tmp_path_factory.mktemp("meltano-project-dir")), project_directory(
         project_init_service,
     ) as project:
```

### Comparing `meltano-3.4.0b1/tests/fixtures/db/__init__.py` & `meltano-3.4.1b1/tests/fixtures/db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 @pytest.fixture(scope="class", autouse=True)
 def vacuum_db(engine_sessionmaker):
     try:
         yield
     finally:
-        logging.debug("Cleaning system database...")
+        logging.debug("Cleaning system database...")  # noqa: TID251
         engine, _ = engine_sessionmaker
         close_all_sessions()
         metadata = MetaData()
         metadata.reflect(bind=engine)
         metadata.drop_all(bind=engine)
```

### Comparing `meltano-3.4.0b1/tests/fixtures/db/mssql.py` & `meltano-3.4.1b1/tests/fixtures/db/mssql.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,8 +87,8 @@
 @pytest.fixture()
 def pg_stats(request, session):
     yield
 
     from meltano.core.job import Job
 
     jobs = session.query(Job).all()
-    logging.info("%s created %d Job.", request.node.name, len(jobs))  # noqa: WPS323
+    logging.info("%s created %d Job.", request.node.name, len(jobs))  # noqa: TID251, WPS323
```

### Comparing `meltano-3.4.0b1/tests/fixtures/db/postgresql.py` & `meltano-3.4.1b1/tests/fixtures/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/db/postgresql_psycopg3.py` & `meltano-3.4.1b1/tests/fixtures/db/postgresql_psycopg3.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/docker/__init__.py` & `meltano-3.4.1b1/tests/fixtures/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/docker/snowplow.py` & `meltano-3.4.1b1/tests/fixtures/docker/snowplow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/fs.py` & `meltano-3.4.1b1/tests/fixtures/fs.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/large_config_project/meltano.yml` & `meltano-3.4.1b1/tests/fixtures/large_config_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/large_config_project/schedule.yml` & `meltano-3.4.1b1/tests/fixtures/large_config_project/schedule.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/multifile_project/meltano.yml` & `meltano-3.4.1b1/tests/fixtures/multifile_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/plugins/extractors/tap-custom/test.yml` & `meltano-3.4.1b1/tests/fixtures/plugins/extractors/tap-custom/test.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/fixtures/utils.py` & `meltano-3.4.1b1/tests/fixtures/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
         os.chdir(prev_dir)
 
 
 @contextmanager
 def tmp_project(name: str, source: Path, compatible_copy_tree) -> Project:
     project_init_service = ProjectInitService(name)
     blank_project = project_init_service.init()
-    logging.debug(f"Created new project at {blank_project.root}")  # noqa: G004
+    logging.debug(f"Created new project at {blank_project.root}")  # noqa: G004, TID251
     os.remove(blank_project.meltanofile)
     compatible_copy_tree(source, blank_project.root)
     Project._default = None
     project = Project(blank_project.root)
     with cd(project.root):
         try:
             project.refresh()
             yield project
         finally:
             Project.deactivate()
-            logging.debug(f"Cleaned project at {project.root}")  # noqa: G004
+            logging.debug(f"Cleaned project at {project.root}")  # noqa: G004, TID251
```

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_add.py` & `meltano-3.4.1b1/tests/meltano/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_cli.py` & `meltano-3.4.1b1/tests/meltano/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_compile.py` & `meltano-3.4.1b1/tests/meltano/cli/test_compile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_config.py` & `meltano-3.4.1b1/tests/meltano/cli/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import json
 import platform
 import typing as t
+from signal import SIGTERM
 
 import pytest
 from mock import AsyncMock, mock
 
 from asserts import assert_cli_runner
 from meltano.cli import cli
 from meltano.core.settings_service import REDACTED_VALUE, SettingValueStore
@@ -71,16 +72,16 @@
         ) in result.stdout
 
     @pytest.mark.usefixtures("project")
     def test_config_test(self, cli_runner, tap):
         mock_invoke = mock.Mock()
         mock_invoke.sterr.at_eof.side_effect = True
         mock_invoke.stdout.at_eof.side_effect = (False, True)
-        mock_invoke.wait = AsyncMock(return_value=-1)
-        mock_invoke.returncode = -1
+        mock_invoke.wait = AsyncMock(return_value=-SIGTERM)
+        mock_invoke.returncode = -SIGTERM
         payload = json.dumps({"type": "RECORD"}).encode()
         mock_invoke.stdout.readline = AsyncMock(return_value=b"%b" % payload)
 
         with mock.patch(
             "meltano.core.plugin_invoker.PluginInvoker.invoke_async",
             return_value=mock_invoke,
         ) as mocked_invoke:
```

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_elt.py` & `meltano-3.4.1b1/tests/meltano/cli/test_elt.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     """
     seen_lines: list[dict] = []
     for line in result_output.splitlines():
         parsed_line = json.loads(line)
         seen_lines.append(parsed_line)
 
     for line in seen_lines:
-        if line.get("exc_info") and repr(exc) in line.get("exc_info"):
+        if line.get("event") and exc.args[0] in line.get("event"):
             return True
     return False
 
 
 def assert_log_lines(result_output: str, expected: list[LogEntry]):
     seen_lines: list[dict] = []
     for line in result_output.splitlines():
```

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_hub.py` & `meltano-3.4.1b1/tests/meltano/cli/test_hub.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_initialize.py` & `meltano-3.4.1b1/tests/meltano/cli/test_initialize.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_install.py` & `meltano-3.4.1b1/tests/meltano/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_invoke.py` & `meltano-3.4.1b1/tests/meltano/cli/test_invoke.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_job_cmd.py` & `meltano-3.4.1b1/tests/meltano/cli/test_job_cmd.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_lock.py` & `meltano-3.4.1b1/tests/meltano/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_remove.py` & `meltano-3.4.1b1/tests/meltano/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_run.py` & `meltano-3.4.1b1/tests/meltano/cli/test_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import asyncio
 import json
 import re
 import typing as t
+import uuid
 
+import click
 import pytest
 from mock import AsyncMock, mock
 
 from meltano.cli import cli
+from meltano.cli.run import UUIDParamType
 from meltano.core.block.ioblock import IOBlock
 from meltano.core.logging.utils import default_config
 from meltano.core.plugin import PluginType
 from meltano.core.plugin.singer import SingerTap
 from meltano.core.plugin_invoker import PluginInvoker
 from meltano.core.project_plugins_service import (
     AmbiguousMappingName,
@@ -1297,7 +1300,26 @@
             result = cli_runner.invoke(cli, args)
             ansi_color_escape = re.compile(r"\x1b\[[0-9;]+m")
             match = ansi_color_escape.search(result.stderr)
             if colors:
                 assert match
             else:
                 assert not match
+
+
+class TestUUIDParamType:
+    @pytest.mark.parametrize(
+        "value",
+        (
+            pytest.param("123e4567-e89b-12d3-a456-426614174000", id="with hyphens"),
+            pytest.param("123e4567e89b12d3a456426614174000", id="without hyphens"),
+        ),
+    )
+    def test_valid_uuid(self, value: str):
+        param = UUIDParamType()
+        assert param.convert(value, None, None) == uuid.UUID(value)
+
+    def test_invalid_uuid(self):
+        param = UUIDParamType()
+        value = "zzz"
+        with pytest.raises(click.BadParameter, match="is not a valid UUID"):
+            param.convert(value, None, None)
```

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_schedule.py` & `meltano-3.4.1b1/tests/meltano/cli/test_schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_select.py` & `meltano-3.4.1b1/tests/meltano/cli/test_select.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_state.py` & `meltano-3.4.1b1/tests/meltano/cli/test_state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/cli/test_upgrade.py` & `meltano-3.4.1b1/tests/meltano/cli/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/behavior/test_canonical.py` & `meltano-3.4.1b1/tests/meltano/core/behavior/test_canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/behavior/test_hookable.py` & `meltano-3.4.1b1/tests/meltano/core/behavior/test_hookable.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/block/test_extract_load.py` & `meltano-3.4.1b1/tests/meltano/core/block/test_extract_load.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
 import tempfile
 import typing as t
+import uuid
 from pathlib import Path
 
 import mock
 import pytest
 from mock import AsyncMock
 
 from meltano.core.block.blockset import BlockSetValidationError
@@ -28,14 +29,15 @@
 from meltano.core.plugin_invoker import PluginInvoker
 from meltano.core.project_plugins_service import PluginAlreadyAddedException
 from meltano.core.runner import RunnerError
 from meltano.core.runner.singer import SingerRunner
 
 if t.TYPE_CHECKING:
     from meltano.core.plugin.project_plugin import ProjectPlugin
+    from meltano.core.project import Project
 
 TEST_STATE_ID = "test_job"
 MOCK_STATE_MESSAGE = json.dumps({"type": "STATE"})
 MOCK_RECORD_MESSAGE = json.dumps({"type": "RECORD"})
 
 
 def create_plugin_files(config_dir: Path, plugin: ProjectPlugin):
@@ -165,15 +167,15 @@
             == target_env["MELTANO_EXTRACTOR_NAMESPACE"]
         )
 
 
 class TestExtractLoadBlocks:
     @pytest.fixture()
     def log_level_debug(self):
-        root_logger = logging.getLogger()
+        root_logger = logging.getLogger()  # noqa: TID251
         log_level = root_logger.level
         try:
             root_logger.setLevel(logging.DEBUG)
             yield
         finally:
             root_logger.setLevel(log_level)
 
@@ -573,14 +575,32 @@
                 assert block.context.job.job_name == "test:tap-mock-to-target-mock"
 
             elb.run_with_job = AsyncMock()
 
             await elb.run()
             assert elb.run_with_job.call_count == 1
 
+    def test_custom_run_id(
+        self,
+        tap,
+        target,
+        project_with_environment: Project,
+    ):
+        run_id = uuid.UUID("12345678-1234-5678-1234-567812345678")
+        builder = ELBContextBuilder(project_with_environment).with_run_id(run_id)
+        assert builder._run_id == run_id
+
+        elb_context = builder.context()
+        tap_block = builder.make_block(tap)
+        target_block = builder.make_block(target)
+        extract_load_blocks = ExtractLoadBlocks(elb_context, (tap_block, target_block))
+        assert extract_load_blocks.context.update_state
+        assert extract_load_blocks.context.job is not None
+        assert extract_load_blocks.context.job.run_id == run_id
+
 
 class TestExtractLoadUtils:
     def test_generate_state_id(self):
         block1 = mock.Mock(spec=IOBlock)
         block1.string_id = "block1"
 
         block2 = mock.Mock(spec=IOBlock)
```

### Comparing `meltano-3.4.0b1/tests/meltano/core/block/test_plugin_command.py` & `meltano-3.4.1b1/tests/meltano/core/block/test_plugin_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/block/test_singer.py` & `meltano-3.4.1b1/tests/meltano/core/block/test_singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/container/test_container_spec.py` & `meltano-3.4.1b1/tests/meltano/core/container/test_container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/hub/test_meltano_hub_service.py` & `meltano-3.4.1b1/tests/meltano/core/hub/test_meltano_hub_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/job/test_finder.py` & `meltano-3.4.1b1/tests/meltano/core/job/test_finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/job/test_job.py` & `meltano-3.4.1b1/tests/meltano/core/job/test_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/job/test_stale_job_failer.py` & `meltano-3.4.1b1/tests/meltano/core/job/test_stale_job_failer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/logging/test_formatters.py` & `meltano-3.4.1b1/tests/meltano/core/logging/test_formatters.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/logging/test_logging_utils.py` & `meltano-3.4.1b1/tests/meltano/core/logging/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/logging/test_output_logger.py` & `meltano-3.4.1b1/tests/meltano/core/logging/test_output_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 import logging
 import platform
 import sys
 import tempfile
+import typing as t
 
 import mock
 import pytest
 import structlog
 from structlog.testing import LogCapture
 
 from meltano.core.logging.output_logger import Out, OutputLogger
@@ -18,15 +19,17 @@
     for line in lines:
         assert line in output
 
 
 class TestOutputLogger:
     @pytest.fixture()
     def log(self, tmp_path):
-        return tempfile.NamedTemporaryFile(mode="w+", dir=tmp_path)
+        file = tempfile.NamedTemporaryFile(mode="w+", dir=tmp_path)
+        yield file
+        file.close()
 
     @pytest.fixture()
     def subject(self, log):
         return OutputLogger(log.name)
 
     @pytest.fixture(name="log_output")
     def fixture_log_output(self):
@@ -42,22 +45,26 @@
         )
         try:
             yield
         finally:
             structlog.configure(**original_config)
 
     @pytest.fixture(name="redirect_handler")
-    def redirect_handler(self, subject: OutputLogger) -> logging.Handler:
+    def redirect_handler(
+        self,
+        subject: OutputLogger,
+    ) -> t.Generator[logging.Handler, None, None]:
         formatter = structlog.stdlib.ProcessorFormatter(
             # use a json renderer so output is easier to verify
             processor=structlog.processors.JSONRenderer(),
         )
         handler = logging.FileHandler(subject.file)
         handler.setFormatter(formatter)
-        return handler
+        yield handler
+        handler.close()
 
     @pytest.mark.asyncio()
     @pytest.mark.usefixtures("log")
     async def test_stdio_capture(self, subject, log_output):
         if platform.system() == "Windows":
             pytest.xfail(
                 "Fails on Windows: https://github.com/meltano/meltano/issues/3444",
@@ -182,30 +189,30 @@
 
     @pytest.mark.skipif(
         platform.system() == "Windows",
         reason="Test fails if even attempted to be run, xfail can't save us here.",
     )
     @pytest.mark.asyncio()
     @pytest.mark.usefixtures("log", "log_output")
-    async def test_logging_redirect(self, subject, redirect_handler):
+    async def test_logging_redirect(self, subject: OutputLogger, redirect_handler):
         if platform.system() == "Windows":
             pytest.xfail(
                 "Fails on Windows: https://github.com/meltano/meltano/issues/3444",
             )
 
         logging_out = subject.out("logging")
 
         with mock.patch.object(
             Out,
             "redirect_log_handler",
             redirect_handler,
         ), logging_out.redirect_logging():
-            logging.info("info")
-            logging.warning("warning")
-            logging.error("error")
+            logging.info("info")  # noqa: TID251
+            logging.warning("warning")  # noqa: TID251
+            logging.error("error")  # noqa: TID251
 
         with open(subject.file) as logf:
             log_file_contents = [json.loads(line) for line in logf.readlines()]
 
         assert_lines(
             log_file_contents,
             {"event": "info"},
```

### Comparing `meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_catalog.py` & `meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1089,14 +1089,29 @@
         ],
     )
     def test_node_selection(self, node: dict, selection_type: SelectionType):
         """Test that selection metadata produces the expected selection type member."""
         assert ListSelectedExecutor.node_selection(node) == selection_type
 
 
+class TestSelectionType:
+    def test_selection_type_addition(self):
+        st = SelectionType
+        assert st.EXCLUDED + st.EXCLUDED == st.EXCLUDED
+        assert st.SELECTED + st.EXCLUDED == st.EXCLUDED
+        assert st.AUTOMATIC + st.EXCLUDED == st.EXCLUDED
+        assert st.SELECTED + st.AUTOMATIC == st.AUTOMATIC
+        assert st.SELECTED + st.SELECTED == st.SELECTED
+
+    def test_selection_type_repr(self):
+        assert f"{SelectionType.EXCLUDED}" == "excluded"
+        assert f"{SelectionType.AUTOMATIC}" == "automatic"
+        assert f"{SelectionType.SELECTED}" == "selected"
+
+
 class TestMetadataExecutor:
     @pytest.fixture()
     def catalog(self, request):
         return json.loads(globals()[request.param])  # noqa: WPS421
 
     @pytest.mark.parametrize(
         "catalog",
```

### Comparing `meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_tap.py` & `meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_tap.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,15 +849,15 @@
         ), mock.patch(
             "meltano.core.plugin.singer.tap._stream_redirect",
         ) as stream_mock2:
             await subject.run_discovery(invoker, catalog_path)
             assert stream_mock2.call_count == 2
 
         # ensure stderr is redirected to devnull if we don't need it
-        discovery_logger = logging.getLogger("meltano.core.plugin.singer.tap")
+        discovery_logger = logging.getLogger("meltano.core.plugin.singer.tap")  # noqa: TID251
         original_level = discovery_logger.getEffectiveLevel()
         discovery_logger.setLevel(logging.INFO)
         with mock.patch(
             "meltano.core.plugin.singer.tap.logger.isEnabledFor",
             return_value=True,
         ), mock.patch(
             "meltano.core.plugin.singer.tap._stream_redirect",
```

### Comparing `meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_target.py` & `meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_target.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/plugin/test_airflow.py` & `meltano-3.4.1b1/tests/meltano/core/plugin/test_airflow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/plugin/test_command.py` & `meltano-3.4.1b1/tests/meltano/core/plugin/test_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin.py` & `meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin_settings.py` & `meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin_settings.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/plugin/test_superset.py` & `meltano-3.4.1b1/tests/meltano/core/plugin/test_superset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/runner/test_runner.py` & `meltano-3.4.1b1/tests/meltano/core/runner/test_runner.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/state_store/test_db.py` & `meltano-3.4.1b1/tests/meltano/core/state_store/test_db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/state_store/test_filesystem.py` & `meltano-3.4.1b1/tests/meltano/core/state_store/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/state_store/test_state_store.py` & `meltano-3.4.1b1/tests/meltano/core/state_store/test_state_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_db_compat.py` & `meltano-3.4.1b1/tests/meltano/core/test_db_compat.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_db_connection.py` & `meltano-3.4.1b1/tests/meltano/core/test_db_connection.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_elt_context.py` & `meltano-3.4.1b1/tests/meltano/core/test_elt_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_environment_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_environment_variables.py` & `meltano-3.4.1b1/tests/meltano/core/test_environment_variables.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_locked_definition_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_locked_definition_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_meltano_file.py` & `meltano-3.4.1b1/tests/meltano/core/test_meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_meltano_invoker.py` & `meltano-3.4.1b1/tests/meltano/core/test_meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_plugin_install_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_plugin_install_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_plugin_invoker.py` & `meltano-3.4.1b1/tests/meltano/core/test_plugin_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_plugin_lock_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_plugin_lock_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_plugin_remove_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_plugin_remove_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_plugin_test_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_plugin_test_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import json
 import typing as t
+from signal import SIGTERM
 
 import pytest
 from mock import AsyncMock, Mock, patch
 
 from meltano.core.plugin.error import PluginNotSupportedError
 from meltano.core.plugin_test_service import (
     ExtractorTestService,
@@ -45,16 +46,16 @@
 
 class TestExtractorTestService:
     @pytest.fixture(autouse=True)
     @patch("meltano.core.plugin_invoker.PluginInvoker")
     def setup(self, mock_invoker):
         self.mock_invoke = Mock()
         self.mock_invoke.name = "utility-mock"
-        self.mock_invoke.wait = AsyncMock(return_value=-1)
-        self.mock_invoke.returncode = -1
+        self.mock_invoke.wait = AsyncMock(return_value=-SIGTERM)
+        self.mock_invoke.returncode = -SIGTERM
         self.mock_invoker = mock_invoker
         self.mock_invoker.invoke_async = AsyncMock(return_value=self.mock_invoke)
 
     @pytest.mark.asyncio()
     async def test_validate_success(self):
         self.mock_invoke.sterr.at_eof.side_effect = True
         self.mock_invoke.stdout.at_eof.side_effect = (False, True)
```

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_project.py` & `meltano-3.4.1b1/tests/meltano/core/test_project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_project_add_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_project_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_project_files.py` & `meltano-3.4.1b1/tests/meltano/core/test_project_files.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_project_init_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_project_init_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_project_plugins_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_project_plugins_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_project_settings_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_schedule_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_schedule_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_setting_definition.py` & `meltano-3.4.1b1/tests/meltano/core/test_setting_definition.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_settings_store.py` & `meltano-3.4.1b1/tests/meltano/core/test_settings_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_state_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_state_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_task_sets.py` & `meltano-3.4.1b1/tests/meltano/core/test_task_sets.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_task_sets_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_task_sets_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_utils.py` & `meltano-3.4.1b1/tests/meltano/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_validation_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_validation_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/test_venv_service.py` & `meltano-3.4.1b1/tests/meltano/core/test_venv_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/tracking/test_environment_context.py` & `meltano-3.4.1b1/tests/meltano/core/tracking/test_environment_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/tracking/test_exception.py` & `meltano-3.4.1b1/tests/meltano/core/tracking/test_exception.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/tracking/test_plugins.py` & `meltano-3.4.1b1/tests/meltano/core/tracking/test_plugins.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/tracking/test_project_context.py` & `meltano-3.4.1b1/tests/meltano/core/tracking/test_project_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/tracking/test_schemas.py` & `meltano-3.4.1b1/tests/meltano/core/tracking/test_schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0b1/tests/meltano/core/tracking/test_tracker.py` & `meltano-3.4.1b1/tests/meltano/core/tracking/test_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,15 @@
                 "notvalid:8080",
                 "https://valid.endpoint:8080",
                 "file://bad.scheme",
                 "https://other.endpoint/path/to/collector"
             ]
         """
         monkeypatch.setenv("MELTANO_SNOWPLOW_COLLECTOR_ENDPOINTS", endpoints)
-        logging.getLogger().setLevel(logging.DEBUG)
+        logging.getLogger().setLevel(logging.DEBUG)  # noqa: TID251
 
         with caplog.at_level(logging.WARNING, logger="snowplow_tracker.emitters"):
             tracker = Tracker(project)
 
         try:
             assert caplog.records[0].levelname == "WARNING"
             assert caplog.records[0].msg["event"] == "invalid_snowplow_endpoint"
```

### Comparing `meltano-3.4.0b1/PKG-INFO` & `meltano-3.4.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltano
-Version: 3.4.0b1
+Version: 3.4.1b1
 Summary: Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love.
 Home-page: https://meltano.com
 License: MIT
 Keywords: Meltano,ELT,Data integration,singer-io,dbt
 Author: Meltano
 Author-email: hello@meltano.com
 Requires-Python: >=3.8,<3.13
@@ -28,28 +28,28 @@
 Requires-Dist: aiodocker (>=0.21.0,<0.22.0)
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: atomicwrites (>=1.2.1,<2.0.0)
 Requires-Dist: azure-common (>=1.1.28,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-core (>=1.30.1,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-identity (>=1.16.0,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0) ; extra == "azure"
-Requires-Dist: boto3 (>=1.34.84,<2.0.0) ; extra == "s3"
+Requires-Dist: boto3 (>=1.34.98,<2.0.0) ; extra == "s3"
 Requires-Dist: check-jsonschema (>=0.28.2,<0.29.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: click-default-group (>=1.2.4,<2.0.0)
 Requires-Dist: click-didyoumean (>=0.3.1,<0.4.0)
-Requires-Dist: croniter (>=2.0.3,<3.0.0)
+Requires-Dist: croniter (>=2.0.5,<3.0.0)
 Requires-Dist: fasteners (>=0.19,<0.20)
 Requires-Dist: flatten-dict (>=0,<1)
 Requires-Dist: google-cloud-storage (>=1.31.0) ; extra == "gcs"
 Requires-Dist: importlib-resources (>=6.4.0,<7.0.0)
-Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
-Requires-Dist: jsonschema (>=4.21,<5.0)
+Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
+Requires-Dist: jsonschema (>=4.22,<5.0)
 Requires-Dist: packaging (>=24.0,<25.0)
-Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
+Requires-Dist: platformdirs (>=4.2.1,<5.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) ; extra == "psycopg2"
 Requires-Dist: psycopg[binary] (>=3.1.18,<4.0.0) ; extra == "postgres"
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: pymssql (>=2.3.0,<3.0.0) ; extra == "mssql"
 Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
@@ -59,22 +59,22 @@
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: ruamel.yaml (>=0.18.6,<0.19.0)
 Requires-Dist: setuptools (>=69.5.1,<70.0.0) ; python_version >= "3.12"
 Requires-Dist: smart-open (>=7.0.4,<8.0.0)
 Requires-Dist: snowplow-tracker (>=1.0.2,<2.0.0)
-Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Requires-Dist: tzlocal (>=5.2,<6.0)
 Requires-Dist: urllib3 (<2)
 Requires-Dist: uv (>=0.1.24,<0.2) ; extra == "uv"
-Requires-Dist: virtualenv (>=20.25.1,<21.0.0)
+Requires-Dist: virtualenv (>=20.26.1,<21.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Project-URL: Changelog, https://github.com/meltano/meltano/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://docs.meltano.com
 Project-URL: Issue Tracker, https://github.com/meltano/meltano/issues
 Project-URL: Repository, https://github.com/meltano/meltano
 Project-URL: Slack, https://meltano.com/slack
 Project-URL: Twitter, https://twitter.com/meltanodata/
```

