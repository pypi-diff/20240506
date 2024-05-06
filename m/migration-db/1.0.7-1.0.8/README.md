# Comparing `tmp/migration_db-1.0.7.tar.gz` & `tmp/migration_db-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migration_db-1.0.7.tar", last modified: Mon May  6 02:38:09 2024, max compression
+gzip compressed data, was "migration_db-1.0.8.tar", last modified: Mon May  6 09:28:40 2024, max compression
```

## Comparing `migration_db-1.0.7.tar` & `migration_db-1.0.8.tar`

### file list

```diff
@@ -1,97 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.835863 migration_db-1.0.7/
--rw-rw-rw-   0        0        0     1091 2023-02-14 02:04:04.000000 migration_db-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       42 2024-04-30 06:49:17.000000 migration_db-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      330 2024-05-06 02:38:09.834864 migration_db-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-04-30 07:55:39.000000 migration_db-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.271316 migration_db-1.0.7/migration_db/
--rw-rw-rw-   0        0        0      172 2024-05-06 02:38:00.000000 migration_db-1.0.7/migration_db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.323176 migration_db-1.0.7/migration_db/common/
--rw-rw-rw-   0        0        0      564 2023-07-14 03:27:20.000000 migration_db-1.0.7/migration_db/common/calc_time.py
--rw-rw-rw-   0        0        0     2375 2023-07-31 07:46:04.000000 migration_db-1.0.7/migration_db/common/compare_two_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.336141 migration_db-1.0.7/migration_db/common/conf/
--rw-rw-rw-   0        0        0     1212 2023-02-23 08:16:11.000000 migration_db-1.0.7/migration_db/common/conf/config.py
--rw-rw-rw-   0        0        0      490 2023-11-20 10:13:23.000000 migration_db-1.0.7/migration_db/common/conf/constant.py
--rw-rw-rw-   0        0        0     1782 2023-07-17 03:00:20.000000 migration_db-1.0.7/migration_db/common/conf/data_source_route.py
--rw-rw-rw-   0        0        0     1942 2023-07-31 03:14:53.000000 migration_db-1.0.7/migration_db/common/conf/datasource.json
--rw-rw-rw-   0        0        0     1242 2023-02-23 08:15:20.000000 migration_db-1.0.7/migration_db/common/conf/study_info_route.py
--rw-rw-rw-   0        0        0     1368 2024-01-17 08:08:39.000000 migration_db-1.0.7/migration_db/common/constant.py
--rw-rw-rw-   0        0        0     1176 2024-02-19 06:49:07.000000 migration_db-1.0.7/migration_db/common/create_folder.py
--rw-rw-rw-   0        0        0      875 2024-04-11 10:28:33.000000 migration_db-1.0.7/migration_db/common/database.py
--rw-rw-rw-   0        0        0     1179 2023-05-31 08:12:05.000000 migration_db-1.0.7/migration_db/common/file.py
--rw-rw-rw-   0        0        0      581 2023-12-14 10:16:04.000000 migration_db-1.0.7/migration_db/common/format_time.py
--rw-rw-rw-   0        0        0     2162 2024-02-05 10:15:53.000000 migration_db-1.0.7/migration_db/common/handle_git.py
--rw-rw-rw-   0        0        0      477 2020-12-24 07:05:06.000000 migration_db-1.0.7/migration_db/common/handle_remove_read_only.py
--rw-rw-rw-   0        0        0     4705 2024-01-17 08:26:53.000000 migration_db-1.0.7/migration_db/common/handle_str.py
--rw-rw-rw-   0        0        0     1503 2023-11-07 08:02:22.000000 migration_db-1.0.7/migration_db/common/lib.py
--rw-rw-rw-   0        0        0     2713 2024-02-19 06:06:43.000000 migration_db-1.0.7/migration_db/common/log.py
--rw-rw-rw-   0        0        0     7702 2023-12-15 09:02:25.000000 migration_db-1.0.7/migration_db/common/my_db.py
--rw-rw-rw-   0        0        0     2055 2024-04-08 03:43:19.000000 migration_db-1.0.7/migration_db/common/path.py
--rw-rw-rw-   0        0        0     2047 2023-07-31 09:19:01.000000 migration_db-1.0.7/migration_db/common/read_file.py
--rw-rw-rw-   0        0        0      408 2021-08-03 02:42:25.000000 migration_db-1.0.7/migration_db/common/template_parse.py
--rw-rw-rw-   0        0        0      951 2024-02-19 06:42:00.000000 migration_db-1.0.7/migration_db/common/write_file.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.253361 migration_db-1.0.7/migration_db/migration/
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.444855 migration_db-1.0.7/migration_db/migration/core/
--rw-rw-rw-   0        0        0    12740 2024-04-30 08:49:09.000000 migration_db-1.0.7/migration_db/migration/core/_migration.py
--rw-rw-rw-   0        0        0     1144 2024-05-06 02:36:48.000000 migration_db-1.0.7/migration_db/migration/core/backup.py
--rw-rw-rw-   0        0        0     1990 2024-01-15 08:02:29.000000 migration_db-1.0.7/migration_db/migration/core/base.py
--rw-rw-rw-   0        0        0    16811 2024-02-19 07:29:21.000000 migration_db-1.0.7/migration_db/migration/core/build_update_sql.py
--rw-rw-rw-   0        0        0     5672 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/core/execute_script.py
--rw-rw-rw-   0        0        0     3087 2024-05-06 02:16:09.000000 migration_db-1.0.7/migration_db/migration/core/handle_archive_file.py
--rw-rw-rw-   0        0        0      754 2023-05-06 06:41:30.000000 migration_db-1.0.7/migration_db/migration/core/handle_external_condition_mapping_data.py
--rw-rw-rw-   0        0        0     1339 2023-03-24 13:30:58.000000 migration_db-1.0.7/migration_db/migration/core/handle_procedures.py
--rw-rw-rw-   0        0        0     1840 2023-03-28 07:10:57.000000 migration_db-1.0.7/migration_db/migration/core/handle_special_field.py
--rw-rw-rw-   0        0        0     1711 2022-08-30 02:56:27.000000 migration_db-1.0.7/migration_db/migration/core/handle_table_action.py
--rw-rw-rw-   0        0        0    10110 2024-04-23 08:01:53.000000 migration_db-1.0.7/migration_db/migration/core/incremental_sql.py
--rw-rw-rw-   0        0        0     5211 2023-09-21 04:39:01.000000 migration_db-1.0.7/migration_db/migration/core/match_ids.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.465795 migration_db-1.0.7/migration_db/migration/core/models/
--rw-rw-rw-   0        0        0     1115 2021-03-16 05:40:58.000000 migration_db-1.0.7/migration_db/migration/core/models/config.py
--rw-rw-rw-   0        0        0      709 2023-09-08 02:39:23.000000 migration_db-1.0.7/migration_db/migration/core/models/file_detail.py
--rw-rw-rw-   0        0        0     2436 2023-03-24 13:00:15.000000 migration_db-1.0.7/migration_db/migration/core/models/table_detail.py
--rw-rw-rw-   0        0        0     1574 2024-02-19 07:27:11.000000 migration_db-1.0.7/migration_db/migration/core/redis_biz.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.478761 migration_db-1.0.7/migration_db/migration/core/split_sql/
--rw-rw-rw-   0        0        0     5463 2023-09-25 08:55:57.000000 migration_db-1.0.7/migration_db/migration/core/split_sql/split_sql.py
--rw-rw-rw-   0        0        0     2138 2024-05-06 02:11:57.000000 migration_db-1.0.7/migration_db/migration/core/switch_data_source.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.520647 migration_db-1.0.7/migration_db/migration/db/
--rw-rw-rw-   0        0        0     8020 2024-01-15 07:44:36.000000 migration_db-1.0.7/migration_db/migration/db/admin_db.py
--rw-rw-rw-   0        0        0     2373 2024-02-27 06:56:06.000000 migration_db-1.0.7/migration_db/migration/db/base_db.py
--rw-rw-rw-   0        0        0      460 2023-03-02 01:37:13.000000 migration_db-1.0.7/migration_db/migration/db/design_db.py
--rw-rw-rw-   0        0        0     1260 2023-03-14 09:20:46.000000 migration_db-1.0.7/migration_db/migration/db/edc_db.py
--rw-rw-rw-   0        0        0      693 2023-09-21 01:31:22.000000 migration_db-1.0.7/migration_db/migration/db/iwrs_db.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.557603 migration_db-1.0.7/migration_db/migration/docs/
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.587527 migration_db-1.0.7/migration_db/migration/docs/common_sql/
--rw-rw-rw-   0        0        0     2370 2023-03-27 01:40:59.000000 migration_db-1.0.7/migration_db/migration/docs/common_sql/create_procedure.sql
--rw-rw-rw-   0        0        0      128 2023-03-30 06:10:59.000000 migration_db-1.0.7/migration_db/migration/docs/common_sql/drop_procedure.sql
--rw-rw-rw-   0        0        0      871 2022-05-30 09:06:22.000000 migration_db-1.0.7/migration_db/migration/docs/common_sql/eclinical_schema_history.sql
--rw-rw-rw-   0        0        0    29341 2024-04-30 08:08:27.000000 migration_db-1.0.7/migration_db/migration/docs/config_info.json
--rw-rw-rw-   0        0        0      982 2023-07-31 03:14:53.000000 migration_db-1.0.7/migration_db/migration/docs/redis_detail.json
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.608469 migration_db-1.0.7/migration_db/migration/docs/template/
--rw-rw-rw-   0        0        0      213 2023-06-07 10:37:29.000000 migration_db-1.0.7/migration_db/migration/docs/template/mysql-shell-dump.j2
--rw-rw-rw-   0        0        0      219 2023-06-07 10:37:27.000000 migration_db-1.0.7/migration_db/migration/docs/template/mysql-shell-load-dump.j2
--rw-rw-rw-   0        0        0      429 2022-06-26 13:22:39.000000 migration_db-1.0.7/migration_db/migration/docs/template/parse.py
--rw-rw-rw-   0        0        0     1146 2023-03-24 13:00:15.000000 migration_db-1.0.7/migration_db/migration/docs/template/update_id_template.j2
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.670303 migration_db-1.0.7/migration_db/migration/helper/
--rw-rw-rw-   0        0        0      831 2024-05-06 01:59:04.000000 migration_db-1.0.7/migration_db/migration/helper/backup_by_database.py
--rw-rw-rw-   0        0        0     2388 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/helper/run_edc.py
--rw-rw-rw-   0        0        0     2661 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/helper/run_pv.py
--rw-rw-rw-   0        0        0    11665 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/helper/run_split_sql.py
--rw-rw-rw-   0        0        0     1407 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/helper/run_table_action.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.754082 migration_db-1.0.7/migration_db/migration/lib/
--rw-rw-rw-   0        0        0     2282 2020-12-23 14:18:08.000000 migration_db-1.0.7/migration_db/migration/lib/compareTwoDict.py
--rw-rw-rw-   0        0        0     2422 2024-01-18 08:52:06.000000 migration_db-1.0.7/migration_db/migration/lib/constant.py
--rw-rw-rw-   0        0        0     2282 2024-02-19 07:26:01.000000 migration_db-1.0.7/migration_db/migration/lib/handle_redis.py
--rw-rw-rw-   0        0        0      602 2023-08-07 06:38:30.000000 migration_db-1.0.7/migration_db/migration/lib/handle_str.py
--rw-rw-rw-   0        0        0     5757 2024-02-19 07:24:41.000000 migration_db-1.0.7/migration_db/migration/lib/my_db.py
--rw-rw-rw-   0        0        0     2384 2021-08-07 06:57:33.000000 migration_db-1.0.7/migration_db/migration/lib/my_excel.py
--rw-rw-rw-   0        0        0     5867 2024-02-05 12:03:52.000000 migration_db-1.0.7/migration_db/migration/lib/mysql_connector.py
--rw-rw-rw-   0        0        0     3277 2024-02-19 07:29:21.000000 migration_db-1.0.7/migration_db/migration/lib/mysql_shell.py
--rw-rw-rw-   0        0        0     1531 2023-10-29 07:05:46.000000 migration_db-1.0.7/migration_db/migration/lib/mysql_task.py
--rw-rw-rw-   0        0        0     1506 2024-04-30 08:10:52.000000 migration_db-1.0.7/migration_db/migration/lib/path.py
--rw-rw-rw-   0        0        0      376 2024-03-04 09:45:05.000000 migration_db-1.0.7/migration_db/migration/lib/synchronized.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.804945 migration_db-1.0.7/migration_db.egg-info/
--rw-rw-rw-   0        0        0      330 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6418 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 02:38:09.836865 migration_db-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      979 2024-04-30 08:58:50.000000 migration_db-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.389459 migration_db-1.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-02-14 02:04:04.000000 migration_db-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      452 2024-05-06 09:28:27.000000 migration_db-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      330 2024-05-06 09:28:40.388466 migration_db-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-04-30 07:55:39.000000 migration_db-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:39.945440 migration_db-1.0.8/migration_db/
+-rw-rw-rw-   0        0        0      172 2024-05-06 06:32:24.000000 migration_db-1.0.8/migration_db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:39.996307 migration_db-1.0.8/migration_db/common/
+-rw-rw-rw-   0        0        0      564 2023-07-14 03:27:20.000000 migration_db-1.0.8/migration_db/common/calc_time.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.012463 migration_db-1.0.8/migration_db/common/conf/
+-rw-rw-rw-   0        0        0     1212 2023-02-23 08:16:11.000000 migration_db-1.0.8/migration_db/common/conf/config.py
+-rw-rw-rw-   0        0        0      490 2023-11-20 10:13:23.000000 migration_db-1.0.8/migration_db/common/conf/constant.py
+-rw-rw-rw-   0        0        0     1782 2023-07-17 03:00:20.000000 migration_db-1.0.8/migration_db/common/conf/data_source_route.py
+-rw-rw-rw-   0        0        0     1942 2023-07-31 03:14:53.000000 migration_db-1.0.8/migration_db/common/conf/datasource.json
+-rw-rw-rw-   0        0        0     1242 2023-02-23 08:15:20.000000 migration_db-1.0.8/migration_db/common/conf/study_info_route.py
+-rw-rw-rw-   0        0        0     1368 2024-01-17 08:08:39.000000 migration_db-1.0.8/migration_db/common/constant.py
+-rw-rw-rw-   0        0        0     1179 2023-05-31 08:12:05.000000 migration_db-1.0.8/migration_db/common/file.py
+-rw-rw-rw-   0        0        0      581 2023-12-14 10:16:04.000000 migration_db-1.0.8/migration_db/common/format_time.py
+-rw-rw-rw-   0        0        0     4705 2024-01-17 08:26:53.000000 migration_db-1.0.8/migration_db/common/handle_str.py
+-rw-rw-rw-   0        0        0     2713 2024-02-19 06:06:43.000000 migration_db-1.0.8/migration_db/common/log.py
+-rw-rw-rw-   0        0        0     2055 2024-04-08 03:43:19.000000 migration_db-1.0.8/migration_db/common/path.py
+-rw-rw-rw-   0        0        0     2047 2023-07-31 09:19:01.000000 migration_db-1.0.8/migration_db/common/read_file.py
+-rw-rw-rw-   0        0        0      951 2024-02-19 06:42:00.000000 migration_db-1.0.8/migration_db/common/write_file.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:39.930481 migration_db-1.0.8/migration_db/migration/
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.131146 migration_db-1.0.8/migration_db/migration/core/
+-rw-rw-rw-   0        0        0    12856 2024-05-06 08:16:05.000000 migration_db-1.0.8/migration_db/migration/core/_migration.py
+-rw-rw-rw-   0        0        0     1392 2024-05-06 08:16:05.000000 migration_db-1.0.8/migration_db/migration/core/backup.py
+-rw-rw-rw-   0        0        0     1990 2024-01-15 08:02:29.000000 migration_db-1.0.8/migration_db/migration/core/base.py
+-rw-rw-rw-   0        0        0    16811 2024-02-19 07:29:21.000000 migration_db-1.0.8/migration_db/migration/core/build_update_sql.py
+-rw-rw-rw-   0        0        0     5886 2024-05-06 08:16:05.000000 migration_db-1.0.8/migration_db/migration/core/execute_script.py
+-rw-rw-rw-   0        0        0     3087 2024-05-06 02:16:09.000000 migration_db-1.0.8/migration_db/migration/core/handle_archive_file.py
+-rw-rw-rw-   0        0        0      754 2023-05-06 06:41:30.000000 migration_db-1.0.8/migration_db/migration/core/handle_external_condition_mapping_data.py
+-rw-rw-rw-   0        0        0     1339 2023-03-24 13:30:58.000000 migration_db-1.0.8/migration_db/migration/core/handle_procedures.py
+-rw-rw-rw-   0        0        0     1840 2023-03-28 07:10:57.000000 migration_db-1.0.8/migration_db/migration/core/handle_special_field.py
+-rw-rw-rw-   0        0        0     1711 2022-08-30 02:56:27.000000 migration_db-1.0.8/migration_db/migration/core/handle_table_action.py
+-rw-rw-rw-   0        0        0    10110 2024-04-23 08:01:53.000000 migration_db-1.0.8/migration_db/migration/core/incremental_sql.py
+-rw-rw-rw-   0        0        0     5211 2023-09-21 04:39:01.000000 migration_db-1.0.8/migration_db/migration/core/match_ids.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.152093 migration_db-1.0.8/migration_db/migration/core/models/
+-rw-rw-rw-   0        0        0     1115 2021-03-16 05:40:58.000000 migration_db-1.0.8/migration_db/migration/core/models/config.py
+-rw-rw-rw-   0        0        0      709 2023-09-08 02:39:23.000000 migration_db-1.0.8/migration_db/migration/core/models/file_detail.py
+-rw-rw-rw-   0        0        0     2436 2023-03-24 13:00:15.000000 migration_db-1.0.8/migration_db/migration/core/models/table_detail.py
+-rw-rw-rw-   0        0        0     1574 2024-02-19 07:27:11.000000 migration_db-1.0.8/migration_db/migration/core/redis_biz.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.156120 migration_db-1.0.8/migration_db/migration/core/split_sql/
+-rw-rw-rw-   0        0        0     5463 2023-09-25 08:55:57.000000 migration_db-1.0.8/migration_db/migration/core/split_sql/split_sql.py
+-rw-rw-rw-   0        0        0     2004 2024-05-06 09:00:21.000000 migration_db-1.0.8/migration_db/migration/core/switch_data_source.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.178063 migration_db-1.0.8/migration_db/migration/db/
+-rw-rw-rw-   0        0        0     8020 2024-01-15 07:44:36.000000 migration_db-1.0.8/migration_db/migration/db/admin_db.py
+-rw-rw-rw-   0        0        0     2373 2024-02-27 06:56:06.000000 migration_db-1.0.8/migration_db/migration/db/base_db.py
+-rw-rw-rw-   0        0        0      460 2023-03-02 01:37:13.000000 migration_db-1.0.8/migration_db/migration/db/design_db.py
+-rw-rw-rw-   0        0        0     1260 2023-03-14 09:20:46.000000 migration_db-1.0.8/migration_db/migration/db/edc_db.py
+-rw-rw-rw-   0        0        0      693 2023-09-21 01:31:22.000000 migration_db-1.0.8/migration_db/migration/db/iwrs_db.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.192983 migration_db-1.0.8/migration_db/migration/docs/
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.210965 migration_db-1.0.8/migration_db/migration/docs/common_sql/
+-rw-rw-rw-   0        0        0     2370 2023-03-27 01:40:59.000000 migration_db-1.0.8/migration_db/migration/docs/common_sql/create_procedure.sql
+-rw-rw-rw-   0        0        0      128 2023-03-30 06:10:59.000000 migration_db-1.0.8/migration_db/migration/docs/common_sql/drop_procedure.sql
+-rw-rw-rw-   0        0        0      871 2022-05-30 09:06:22.000000 migration_db-1.0.8/migration_db/migration/docs/common_sql/eclinical_schema_history.sql
+-rw-rw-rw-   0        0        0    29341 2024-04-30 08:08:27.000000 migration_db-1.0.8/migration_db/migration/docs/config_info.json
+-rw-rw-rw-   0        0        0      982 2023-07-31 03:14:53.000000 migration_db-1.0.8/migration_db/migration/docs/redis_detail.json
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.242872 migration_db-1.0.8/migration_db/migration/docs/template/
+-rw-rw-rw-   0        0        0      213 2023-06-07 10:37:29.000000 migration_db-1.0.8/migration_db/migration/docs/template/mysql-shell-dump.j2
+-rw-rw-rw-   0        0        0      219 2023-06-07 10:37:27.000000 migration_db-1.0.8/migration_db/migration/docs/template/mysql-shell-load-dump.j2
+-rw-rw-rw-   0        0        0      429 2022-06-26 13:22:39.000000 migration_db-1.0.8/migration_db/migration/docs/template/parse.py
+-rw-rw-rw-   0        0        0     1146 2023-03-24 13:00:15.000000 migration_db-1.0.8/migration_db/migration/docs/template/update_id_template.j2
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.292746 migration_db-1.0.8/migration_db/migration/helper/
+-rw-rw-rw-   0        0        0      831 2024-05-06 01:59:04.000000 migration_db-1.0.8/migration_db/migration/helper/backup_by_database.py
+-rw-rw-rw-   0        0        0     2388 2024-04-30 07:52:21.000000 migration_db-1.0.8/migration_db/migration/helper/run_edc.py
+-rw-rw-rw-   0        0        0     2661 2024-04-30 07:52:21.000000 migration_db-1.0.8/migration_db/migration/helper/run_pv.py
+-rw-rw-rw-   0        0        0    11665 2024-04-30 07:52:21.000000 migration_db-1.0.8/migration_db/migration/helper/run_split_sql.py
+-rw-rw-rw-   0        0        0     1407 2024-04-30 07:52:21.000000 migration_db-1.0.8/migration_db/migration/helper/run_table_action.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:40.383474 migration_db-1.0.8/migration_db/migration/lib/
+-rw-rw-rw-   0        0        0     2282 2020-12-23 14:18:08.000000 migration_db-1.0.8/migration_db/migration/lib/compareTwoDict.py
+-rw-rw-rw-   0        0        0     2422 2024-01-18 08:52:06.000000 migration_db-1.0.8/migration_db/migration/lib/constant.py
+-rw-rw-rw-   0        0        0     2282 2024-02-19 07:26:01.000000 migration_db-1.0.8/migration_db/migration/lib/handle_redis.py
+-rw-rw-rw-   0        0        0      602 2023-08-07 06:38:30.000000 migration_db-1.0.8/migration_db/migration/lib/handle_str.py
+-rw-rw-rw-   0        0        0     5757 2024-02-19 07:24:41.000000 migration_db-1.0.8/migration_db/migration/lib/my_db.py
+-rw-rw-rw-   0        0        0     2384 2021-08-07 06:57:33.000000 migration_db-1.0.8/migration_db/migration/lib/my_excel.py
+-rw-rw-rw-   0        0        0     5867 2024-02-05 12:03:52.000000 migration_db-1.0.8/migration_db/migration/lib/mysql_connector.py
+-rw-rw-rw-   0        0        0     3277 2024-02-19 07:29:21.000000 migration_db-1.0.8/migration_db/migration/lib/mysql_shell.py
+-rw-rw-rw-   0        0        0     1531 2023-10-29 07:05:46.000000 migration_db-1.0.8/migration_db/migration/lib/mysql_task.py
+-rw-rw-rw-   0        0        0     1506 2024-04-30 08:10:52.000000 migration_db-1.0.8/migration_db/migration/lib/path.py
+-rw-rw-rw-   0        0        0      376 2024-03-04 09:45:05.000000 migration_db-1.0.8/migration_db/migration/lib/synchronized.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:28:39.973367 migration_db-1.0.8/migration_db.egg-info/
+-rw-rw-rw-   0        0        0      330 2024-05-06 09:28:39.000000 migration_db-1.0.8/migration_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2957 2024-05-06 09:28:39.000000 migration_db-1.0.8/migration_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:28:39.000000 migration_db-1.0.8/migration_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-06 09:28:39.000000 migration_db-1.0.8/migration_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 09:28:39.000000 migration_db-1.0.8/migration_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:28:40.390455 migration_db-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      962 2024-05-06 08:53:16.000000 migration_db-1.0.8/setup.py
```

### Comparing `migration_db-1.0.7/LICENSE` & `migration_db-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/calc_time.py` & `migration_db-1.0.8/migration_db/common/calc_time.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/compare_two_dict.py` & `migration_db-1.0.8/migration_db/migration/lib/compareTwoDict.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# !/usr/bin/python3
-# -*- coding:utf-8 -*-
 """
-@Author: xiaodong.li
-@Time: 7/31/2023 3:03 PM
-@Description: Description
-@File: compare_two_dict.py
+Created on Nov 8, 2020
+
+@author: xiaodong.li
 """
+
 from enum import Enum, unique
 
 
 @unique
 class CompareConst(Enum):
     equal = '='  # Equal value
     diff = '!'  # Value varies
@@ -28,15 +26,15 @@
     def compare(self, key):
         v1 = self.dict1.get(key)
         v2 = self.dict2.get(key)
         if (type(v1) == dict) and (type(v2) == dict):
             if v1 == v2 == dict():
                 self.result[key] = CompareConst.equal.value
             else:
-                self.result[key] = CompareTwoDict(v1, v2).run()
+                self.result[key] = CompareTwoDict(v1, v2).main()
         else:
             self.result[key] = self.diff(v1, v2)
 
     @staticmethod
     def diff(v1, v2):
         if (v1 is not None) and (v2 is not None):
             if isinstance(v1, str) and isinstance(v2, str):
@@ -51,15 +49,15 @@
         elif (v1 is None) and (v2 is None):
             return CompareConst.equal.value
         elif v1 is not None:
             return CompareConst.more.value
         else:
             return CompareConst.lack.value
 
-    def run(self):
+    def main(self):
         for k in self.key_list:
             self.compare(k)
         return self.result
 
 
 class FilterDict(object):
 
@@ -67,17 +65,17 @@
         self.dict1 = dict1
         self.key_list = list(dict1.keys())
         self.result = {}
 
     def filter(self, key):
         v1 = self.dict1.get(key)
         if type(v1) == dict:
-            if FilterDict(v1).run():
-                self.result[key] = FilterDict(v1).run()
+            if FilterDict(v1).main():
+                self.result[key] = FilterDict(v1).main()
         else:
             if v1 in ['-', '+', '!']:
                 self.result[key] = v1
 
-    def run(self):
+    def main(self):
         for key in self.key_list:
             self.filter(key)
         return self.result
```

### Comparing `migration_db-1.0.7/migration_db/common/conf/config.py` & `migration_db-1.0.8/migration_db/common/conf/config.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/conf/data_source_route.py` & `migration_db-1.0.8/migration_db/common/conf/data_source_route.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/conf/datasource.json` & `migration_db-1.0.8/migration_db/common/conf/datasource.json`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/conf/study_info_route.py` & `migration_db-1.0.8/migration_db/common/conf/study_info_route.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/constant.py` & `migration_db-1.0.8/migration_db/common/constant.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/file.py` & `migration_db-1.0.8/migration_db/common/file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/format_time.py` & `migration_db-1.0.8/migration_db/common/format_time.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/handle_str.py` & `migration_db-1.0.8/migration_db/common/handle_str.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/log.py` & `migration_db-1.0.8/migration_db/common/log.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/my_db.py` & `migration_db-1.0.8/migration_db/migration/lib/my_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,118 @@
 """
 Created on Nov 27, 2019
 
 @author: xiaodong.li
 """
+import traceback
 
 import pymysql
+from common.log import Logger
+from pymysql import cursors
 
-from .log import Logger
 
-
-class MyDB(object):
+class MyDB:
     """
     define my database
     """
 
     def __init__(self, config):
         """
         initialization parameters
         :param config: object
         """
-        self.connect_params = dict(host=config.host, port=int(config.port), user=config.user_name,
-                                   password=config.password, db=config.database, charset='utf8mb4',
-                                   cursorclass=pymysql.cursors.DictCursor)
-        self.env = f"{config.host} / {config.database}"
+        self.connect_params = dict(host=config.host, port=config.port, user=config.user,
+                                   password=config.password, db=config.db, charset='utf8mb4',
+                                   cursorclass=cursors.DictCursor)
+        self.env = f"{config.host} / {config.db}"
         self.conn = None
         self.cur = None
         self.connect()
 
     def connect(self):
         """
         : 获取连接对象和执行对象
         :return:
         """
         try:
             self.conn = pymysql.Connect(**self.connect_params)
             self.cur = self.conn.cursor()
             Logger().debug(f"Connect Database ({self.env}) successfully.")
         except Exception as e:
-            Logger().error(f"Connect Database ({self.env}): Mysql Error{e}.")
-            raise BaseException(e)
+            traceback.print_exc()
+            return Logger().error(f"Connect Database ({self.env}): Mysql Error{e}.")
 
-    def fetchone(self, sql, params=None):
+    def fetchone(self, sql, params=None) -> dict or list:
         """
         : 根据sql和参数获取一行数据
         :param sql: sql语句
         :param params: sql语句对象的参数元祖，默认值为None
         :return: 查询的一行数据
         """
         data_one = None
         try:
             count = self.cur.execute(sql, params)
-            Logger().debug(f"SQL>>>{self.cur._executed}")
+            Logger().debug(f"SQL>>>\n\t\t\t\t{self.cur._executed}")
             if count != 0:
                 data_one = self.cur.fetchone()
             else:
                 Logger().debug("The SQL query data is empty.")
         except Exception as ex:
-            self.close()
             Logger().error(ex)
+        finally:
+            self.close()
         return data_one
 
-    def fetchall(self, sql, params=None):
+    def fetchall(self, sql, params=None) -> list:
         """
         : 根据sql和参数获取一行数据
         :param sql: sql语句
         :param params: sql语句对象的参数列表，默认值为None
         :return: 查询的一行数据
         """
         data_all = None
         try:
             count = self.cur.execute(sql, params)
-            Logger().debug(f"SQL>>>{self.cur._executed}")
+            Logger().debug(f"SQL>>>\n\t\t\t\t{self.cur._executed}")
             if count != 0:
                 data_all = self.cur.fetchall()
             else:
                 Logger().debug("The SQL query data is empty.")
         except Exception as ex:
-            Logger().error(sql)
             Logger().error(ex)
+        finally:
             self.close()
         return data_all
 
     def execute(self, sql, params=None):
         """
         : 执行sql
         :param sql: sql语句
         :param params: sql语句对象的参数列表，默认值为None
         :return:
         """
-        Logger().debug(f"SQL>>>{sql}")
         try:
             self.cur.execute(sql, params)
-            return True
+            Logger().debug(f"SQL>>>\n\t\t\t\t{self.cur._executed}")
         except Exception as ex:
-            Logger().error(ex)
-            return False
+            return Logger().error(ex)
+        return self
 
-    def execute_many(self, stmts):
-        """
-        : 执行多条sql
-        """
-        Logger().debug(f"SQL_STATEMENTS>>>{stmts}")
-        try:
-            sqls = stmts.split(";")
-            self.cur.execute("SET FOREIGN_KEY_CHECKS = 0;")
-            for sql in sqls:
-                sql = sql.strip().replace("\n", "").replace(";", "").replace("  ", " ")
-                if not sql:
-                    continue
-                sql = f"{sql};"
-                self.cur.execute(sql)
-                Logger().info(f"SQL>>>{sql}")
-            self.cur.execute("SET FOREIGN_KEY_CHECKS = 1;")
-        except Exception as ex:
-            Logger().error(ex)
-        finally:
-            self.close()
+    def commit(self):
+        self.conn.commit()
+        return self
 
     def _items(self, sql, params=None):
         """
         : 执行增删改
         :param sql: sql语句
         :param params: sql语句对象的参数列表，默认值为None
         :return: 受影响的行数
         """
         try:
-            Logger().debug(f"SQL>>>{self.cur._executed}")
             self.cur.execute(sql, params)
             self.conn.commit()
         except Exception as ex:
             Logger().error(ex)
 
     def update(self, sql, params=None):
         """
@@ -145,83 +128,52 @@
         : 执行新增
         :param table_name: 表名
         :param table_data: 数据字典
         :return: 受影响的行数
         """
         keys = ','.join(table_data.keys())
         values = ','.join(['%s'] * len(table_data))
-        sql = f"INSERT INTO {table_name}({keys}) VALUES ({values});"
+        sql = 'INSERT INTO {table}({keys}) VALUES ({values});'.format(
+            table=table_name, keys=keys, values=values)
         try:
             self._items(sql, params=tuple(table_data.values()))
-            Logger().debug("插入数据成功.")
+            Logger().info("插入数据成功.")
         except:
-            self.db.rollback()
+            self.cur.rollback()
             self.close()
             Logger().error("插入数据失败.")
 
-    def delete(self, table_name, table_data, params=None):
+    def delete(self, table_name, table_data):
         """
         : 执行删除
         :param table_name: 表名
         :param table_data: 数据字典
         :return: 受影响的行数
         """
-        condition = ""
-        if params is None:
-            for keys in table_data.keys():
-                if keys == list(table_data.keys())[-1]:
-                    condition = condition + keys + ' = %s'
-                    break
-                condition = condition + keys + " = %s and "
-        elif params == 'in':
-            for keys, values in table_data.items():
-                if values is None:
-                    table_data[keys] = (None,)
-                condition = f"{keys} in %s"
-        sql = f"DELETE FROM {table_name} WHERE {condition};"
+        params = ""
+        for keys in table_data.keys():
+            if keys == list(table_data.keys())[-1]:
+                params = params + keys + ' = %s'
+                break
+            params = params + keys + " = %s and "
+        sql = 'DELETE FROM {table} WHERE {params};'.format(table=table_name,
+                                                           params=params)
         try:
             self._items(sql, params=tuple(table_data.values()))
-        except:
+            Logger().info(
+                f"The data in the table ({table_name}) has been deleted."
+            )
+        finally:
             self.close()
 
     def close(self):
         """
-        : Close the execution tool and the connected object.
+        : 关闭执行工具和连接对象
         """
         try:
             if self.cur is not None:
                 self.cur.close()
             if self.conn is not None:
                 self.conn.close()
-                Logger().debug(f"Database ({self.env}) closed.")
-        except Exception as e:
-            return Logger().error(f"Mysql Error {e}")
-
-    def insert_many(self, table_name, data: list):
-        try:
-            length = len(data)
-            print(f"insert_many start: {length}")
-            slice_size = 10000
-            if length > 0:
-                first_row = data[0]
-                fields = ','.join(list(data[0].keys()))
-                values = ','.join(['%s'] * len(first_row))
-                sql = f"INSERT INTO {table_name}({fields}) VALUES ({values})"
-                slice_count = length // slice_size
-                remainder = len(data) % slice_size
-                if remainder > 0:
-                    slice_count += 1
-                start = 0
-                for count in range(1, slice_count + 1):
-                    if count < slice_count:
-                        end = slice_size * count
-                    else:
-                        end = length
-                    items = data[start: end]
-                    partial_data = [tuple(item.values()) for item in items]
-                    self.cur.executemany(sql, partial_data)
-                    start = end
-                    print(end)
-                self.conn.commit()
-            print(f"insert_many end: {length}")
+                Logger().debug("Database closed.")
         except Exception as e:
-            raise Exception(str(e))
+            return Logger().error("Mysql Error {0}".format(e))
```

### Comparing `migration_db-1.0.7/migration_db/common/path.py` & `migration_db-1.0.8/migration_db/common/path.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/read_file.py` & `migration_db-1.0.8/migration_db/common/read_file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/common/write_file.py` & `migration_db-1.0.8/migration_db/common/write_file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/_migration.py` & `migration_db-1.0.8/migration_db/migration/core/_migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,16 @@
     def _restore_database(self):
         if self.migration_type == MigrationTypeEnum.MYSQL.code and self.local_sql_path:
             return MysqlTask(**self.app_db_route).mysql_task(self.local_sql_path)
         elif self.migration_type == MigrationTypeEnum.MYSQL_SHELL.code:
             return MysqlShellTask(**self.app_db_route).restore_task(self.local_path_dir)
         elif self.migration_type == MigrationTypeEnum.MYSQL_CONNECTOR.code:
             return MysqlConnector(**self.app_db_route).restore_from_slice_path(self.slice_path,
-                self.is_restore_all_tables, self.restore_tables)
+                                                                               self.is_restore_all_tables,
+                                                                               self.restore_tables)
 
     @calc_func_time
     def _update_database(self, config_info):
         self.set_update_sql_path(config_info)
         if self.update_sql_path is None:
             print("sql path is none.")
         else:
@@ -256,16 +257,15 @@
     def count_table(self, table_name):
         return BaseDb(self.app_db_route).count_table(table_name)
 
     def fetchall(self, sql, params=None):
         return BaseDb(self.app_db_route).fetchall(sql, params) or dict()
 
     def init_schema_history_and_latest_sql_version(self, latest_version_id):
-        return ExecuteScript(self.app_db_route, self.system).init_schema_history_and_latest_sql_version(
-            latest_version_id)
+        return ExecuteScript(self.app_db_route).init_schema_history_and_latest_sql_version(latest_version_id)
 
     def _kill_db_process(self):
         data_source = copy.deepcopy(self.app_db_route)
         data_source["db"] = None
         items = BaseDb(data_source).get_all_process_id(self.database)
         n = 1
         while items:
```

### Comparing `migration_db-1.0.7/migration_db/migration/core/backup.py` & `migration_db-1.0.8/migration_db/migration/core/backup.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,25 +6,31 @@
 @Description: Description
 @File: backup.py
 """
 import os
 import sys
 import zipfile
 
+from migration.core.execute_script import ExecuteScript
+
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.realpath(__file__)))))
 from common.conf.data_source_route import DataSourceRoute
 from migration.lib.mysql_task import MysqlTask
 from migration.lib.path import build_sql_file_path
 
 
-def backup(dir_path, host_alias, db_name, sql_name, _is_compress=False, data_source=None):
+def backup(dir_path: str, host_alias, db_name, sql_name, _is_compress=False, data_source=None):
     local_sql_path = build_sql_file_path(dir_path, sql_name)
     if data_source is None:
         data_source = DataSourceRoute().build_config(host_alias, use_config_obj=False)
     data_source["db"] = db_name
     MysqlTask(**data_source).mysqldump_task(local_sql_path)
     if _is_compress is True:
-        zip_backup_path = os.path.join(dir_path, sql_name + ".zip")
+        zip_backup_path: str = os.path.join(dir_path, sql_name + ".zip")
         with zipfile.ZipFile(zip_backup_path, "w", zipfile.ZIP_DEFLATED) as zipf:
             zipf.write(local_sql_path, arcname=sql_name + ".sql")
         if os.path.exists(local_sql_path):
             os.remove(local_sql_path)
+
+
+def init_schema_history_and_latest_sql_version(data_source, latest_version_id):
+    ExecuteScript(data_source).init_schema_history_and_latest_sql_version(latest_version_id)
```

### Comparing `migration_db-1.0.7/migration_db/migration/core/base.py` & `migration_db-1.0.8/migration_db/migration/core/base.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/build_update_sql.py` & `migration_db-1.0.8/migration_db/migration/core/build_update_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/execute_script.py` & `migration_db-1.0.8/migration_db/migration/core/execute_script.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,37 +6,43 @@
 @Description: Description
 @File: execute_script.py
 """
 import os
 import time
 
 from common.format_time import now_utc
-from common.handle_str import ParseBizSqlForAppInfo
+from common.handle_str import ParseBizSqlForAppInfo, ParseNameForAppInfo
 from common.path import incremental_sql_dir_path
 from migration.db.base_db import BaseDb
 from migration.lib.constant import TABLE_SCHEMA_HISTORY
 from migration.lib.mysql_task import MysqlTask
 from migration.lib.path import common_sql_path
 
 
 class ExecuteScript:
 
-    def __init__(self, app_db_route, app):
-        self.app_db_route = app_db_route
-        self.app = app
+    def __init__(self, data_source):
+        self.data_source = data_source
+        db = self.data_source.get("db")
+        if db is not None:
+            p = ParseNameForAppInfo().parse(db)
+            app = p.app
+        else:
+            raise Exception("The db is empty.")
+        self.app: str = app
 
     def execute_incremental_sql(self, ignore_error=False, latest_version=None):
         sql_dir = os.path.join(incremental_sql_dir_path(), self.app)
-        all_tables = BaseDb(self.app_db_route).get_all_tables()
+        all_tables = BaseDb(self.data_source).get_all_tables()
         if TABLE_SCHEMA_HISTORY not in all_tables:
             table_schema_path = os.path.join(common_sql_path(), "{0}.sql".format(TABLE_SCHEMA_HISTORY))
-            MysqlTask(**self.app_db_route).mysql_task(table_schema_path)
+            MysqlTask(**self.data_source).mysql_task(table_schema_path)
         sql = "SELECT script FROM eclinical_schema_history WHERE type='SQL' " \
               "AND success=TRUE ORDER BY installed_rank DESC LIMIT 1;"
-        item = BaseDb(self.app_db_route).fetchone(sql)
+        item = BaseDb(self.data_source).fetchone(sql)
         db_max_version = None
         if item is not None:
             script = item.get("script")
             p = ParseBizSqlForAppInfo().parse(script)
             db_max_version = p.version_id
         if db_max_version is None or db_max_version == latest_version:
             return
@@ -50,56 +56,56 @@
                 if (latest_version is not None and version > latest_version) or version <= db_max_version:
                     continue
                 version_file_mapping.update({version: sql_name})
         version_file_mapping = sorted(version_file_mapping.items(), key=lambda s: s[0])
         for version, sql_name in version_file_mapping:
             is_execute = False
             try:
-                item = BaseDb(self.app_db_route).fetchone(
+                item = BaseDb(self.data_source).fetchone(
                     f"SELECT * FROM eclinical_schema_history WHERE script='{sql_name}';")
             except Exception as e:
                 raise Exception(e)
             if not item:
                 if db_max_version and version > db_max_version:
                     is_execute = True
                 elif db_max_version is None:
                     is_execute = True
                 try:
                     if is_execute:
                         sql_path = os.path.join(sql_dir, sql_name)
-                        MysqlTask(**self.app_db_route).mysql_task(sql_path)
+                        MysqlTask(**self.data_source).mysql_task(sql_path)
                         success = True
                     else:
                         continue
                 except Exception as e:
                     success = False
                     if ignore_error is False:
                         raise Exception(e)
                 # insert the sql executed record
                 if success is False:
                     continue
-                max_item = BaseDb(self.app_db_route).fetchone(
+                max_item = BaseDb(self.data_source).fetchone(
                     f"SELECT installed_rank FROM eclinical_schema_history ORDER BY installed_rank DESC LIMIT 1;")
                 max_id = max_item.get('installed_rank') if max_item else 0
-                BaseDb(self.app_db_route).insert(
+                BaseDb(self.data_source).insert(
                     "eclinical_schema_history",
                     dict(installed_rank=max_id + 1, version=version, type="SQL", script=sql_name, checksum=0,
                          execution_time=0, description=f"{self.app} business schema incremental sql",
                          installed_by="test_platform", installed_on=now_utc(time.time()), success=1))
 
     def init_schema_history_and_latest_sql_version(self, latest_version_id):
         if latest_version_id is None:
             return
-        all_tables = BaseDb(self.app_db_route).get_all_tables()
+        all_tables = BaseDb(self.data_source).get_all_tables()
         if TABLE_SCHEMA_HISTORY not in all_tables:
             table_schema_path = os.path.join(common_sql_path(), "{0}.sql".format(TABLE_SCHEMA_HISTORY))
-            MysqlTask(**self.app_db_route).mysql_task(table_schema_path)
+            MysqlTask(**self.data_source).mysql_task(table_schema_path)
         sql = "SELECT * FROM eclinical_schema_history WHERE type='SQL' " \
               "AND success=TRUE ORDER BY installed_rank DESC LIMIT 1;"
-        item = BaseDb(self.app_db_route).fetchone(sql)
+        item = BaseDb(self.data_source).fetchone(sql)
         db_max_version = None
         installed_rank = 0
         if item is not None:
             script = item.get("script")
             installed_rank = item.get("installed_rank")
             p = ParseBizSqlForAppInfo().parse(script)
             db_max_version = p.version_id
@@ -107,12 +113,12 @@
         if db_max_version is None:
             flag = True
         elif db_max_version < latest_version_id:
             flag = True
         if flag:
             # insert the latest sql_version
             sql_name = f"V{latest_version_id}__{self.app}_business_schema_incremental_sql.sql"
-            BaseDb(self.app_db_route).insert(
+            BaseDb(self.data_source).insert(
                 "eclinical_schema_history",
                 dict(installed_rank=installed_rank + 1, version=latest_version_id, type="SQL", script=sql_name,
                      checksum=0, execution_time=0, description=f"{self.app} business schema incremental sql",
                      installed_by="test_platform", installed_on=now_utc(time.time()), success=1))
```

### Comparing `migration_db-1.0.7/migration_db/migration/core/handle_archive_file.py` & `migration_db-1.0.8/migration_db/migration/core/handle_archive_file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/handle_external_condition_mapping_data.py` & `migration_db-1.0.8/migration_db/migration/core/handle_external_condition_mapping_data.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/handle_procedures.py` & `migration_db-1.0.8/migration_db/migration/core/handle_procedures.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/handle_special_field.py` & `migration_db-1.0.8/migration_db/migration/core/handle_special_field.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/handle_table_action.py` & `migration_db-1.0.8/migration_db/migration/core/handle_table_action.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/incremental_sql.py` & `migration_db-1.0.8/migration_db/migration/core/incremental_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/match_ids.py` & `migration_db-1.0.8/migration_db/migration/core/match_ids.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/models/config.py` & `migration_db-1.0.8/migration_db/migration/core/models/config.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/models/file_detail.py` & `migration_db-1.0.8/migration_db/migration/core/models/file_detail.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/models/table_detail.py` & `migration_db-1.0.8/migration_db/migration/core/models/table_detail.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/redis_biz.py` & `migration_db-1.0.8/migration_db/migration/core/redis_biz.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/core/split_sql/split_sql.py` & `migration_db-1.0.8/migration_db/migration/core/split_sql/split_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/db/admin_db.py` & `migration_db-1.0.8/migration_db/migration/db/admin_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/db/base_db.py` & `migration_db-1.0.8/migration_db/migration/db/base_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/db/edc_db.py` & `migration_db-1.0.8/migration_db/migration/db/edc_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/db/iwrs_db.py` & `migration_db-1.0.8/migration_db/migration/db/iwrs_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/docs/common_sql/create_procedure.sql` & `migration_db-1.0.8/migration_db/migration/docs/common_sql/create_procedure.sql`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/docs/common_sql/eclinical_schema_history.sql` & `migration_db-1.0.8/migration_db/migration/docs/common_sql/eclinical_schema_history.sql`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/docs/config_info.json` & `migration_db-1.0.8/migration_db/migration/docs/config_info.json`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/docs/redis_detail.json` & `migration_db-1.0.8/migration_db/migration/docs/redis_detail.json`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/docs/template/update_id_template.j2` & `migration_db-1.0.8/migration_db/migration/docs/template/update_id_template.j2`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/helper/backup_by_database.py` & `migration_db-1.0.8/migration_db/migration/helper/backup_by_database.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/helper/run_edc.py` & `migration_db-1.0.8/migration_db/migration/helper/run_edc.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/helper/run_pv.py` & `migration_db-1.0.8/migration_db/migration/helper/run_pv.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/helper/run_split_sql.py` & `migration_db-1.0.8/migration_db/migration/helper/run_split_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/helper/run_table_action.py` & `migration_db-1.0.8/migration_db/migration/helper/run_table_action.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/lib/constant.py` & `migration_db-1.0.8/migration_db/migration/lib/constant.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/lib/handle_redis.py` & `migration_db-1.0.8/migration_db/migration/lib/handle_redis.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/lib/handle_str.py` & `migration_db-1.0.8/migration_db/migration/lib/handle_str.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/lib/my_excel.py` & `migration_db-1.0.8/migration_db/migration/lib/my_excel.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/lib/mysql_connector.py` & `migration_db-1.0.8/migration_db/migration/lib/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/lib/mysql_shell.py` & `migration_db-1.0.8/migration_db/migration/lib/mysql_shell.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/lib/mysql_task.py` & `migration_db-1.0.8/migration_db/migration/lib/mysql_task.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/migration_db/migration/lib/path.py` & `migration_db-1.0.8/migration_db/migration/lib/path.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.7/setup.py` & `migration_db-1.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python
 
 import re
 import setuptools
+from setuptools import find_packages
 
 version = ""
 with open('migration_db/__init__.py', 'r') as fd:
     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
                         fd.read(), re.MULTILINE).group(1)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+
 setuptools.setup(
     name="migration_db",
     version=version,
     author="xiaodong.li",
     author_email="",
     description="Migrate database files",
     long_description=long_description,
@@ -23,13 +25,13 @@
     install_requires=[
         'lxml>=4.8.0',
         'redis>=4.3.1',
         'jinja2>=3.1.2',
         'mysql-connector-python>=8.3.0',
         'slicing>=1.0.6',
     ],
-    packages=setuptools.find_namespace_packages(exclude=("test")),
-    classifiers=(
+    packages=find_packages(),
+    classifiers=[
         "Programming Language :: Python :: 3.9",
-    ),
-    package_data={'': ['*.sql', '*.json', "*.j2"]}
+    ],
+    include_package_data=True,
 )
```

