# Comparing `tmp/migration_db-1.0.6.tar.gz` & `tmp/migration_db-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migration_db-1.0.6.tar", last modified: Mon May  6 02:21:39 2024, max compression
+gzip compressed data, was "migration_db-1.0.7.tar", last modified: Mon May  6 02:38:09 2024, max compression
```

## Comparing `migration_db-1.0.6.tar` & `migration_db-1.0.7.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:39.036522 migration_db-1.0.6/
--rw-rw-rw-   0        0        0     1091 2023-02-14 02:04:04.000000 migration_db-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       42 2024-04-30 06:49:17.000000 migration_db-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      330 2024-05-06 02:21:39.034529 migration_db-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-04-30 07:55:39.000000 migration_db-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:36.981645 migration_db-1.0.6/migration_db/
--rw-rw-rw-   0        0        0      172 2024-05-06 02:21:26.000000 migration_db-1.0.6/migration_db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:37.399648 migration_db-1.0.6/migration_db/common/
--rw-rw-rw-   0        0        0      564 2023-07-14 03:27:20.000000 migration_db-1.0.6/migration_db/common/calc_time.py
--rw-rw-rw-   0        0        0     2375 2023-07-31 07:46:04.000000 migration_db-1.0.6/migration_db/common/compare_two_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:37.517085 migration_db-1.0.6/migration_db/common/conf/
--rw-rw-rw-   0        0        0     1212 2023-02-23 08:16:11.000000 migration_db-1.0.6/migration_db/common/conf/config.py
--rw-rw-rw-   0        0        0      490 2023-11-20 10:13:23.000000 migration_db-1.0.6/migration_db/common/conf/constant.py
--rw-rw-rw-   0        0        0     1782 2023-07-17 03:00:20.000000 migration_db-1.0.6/migration_db/common/conf/data_source_route.py
--rw-rw-rw-   0        0        0     1942 2023-07-31 03:14:53.000000 migration_db-1.0.6/migration_db/common/conf/datasource.json
--rw-rw-rw-   0        0        0     1242 2023-02-23 08:15:20.000000 migration_db-1.0.6/migration_db/common/conf/study_info_route.py
--rw-rw-rw-   0        0        0     1368 2024-01-17 08:08:39.000000 migration_db-1.0.6/migration_db/common/constant.py
--rw-rw-rw-   0        0        0     1176 2024-02-19 06:49:07.000000 migration_db-1.0.6/migration_db/common/create_folder.py
--rw-rw-rw-   0        0        0      875 2024-04-11 10:28:33.000000 migration_db-1.0.6/migration_db/common/database.py
--rw-rw-rw-   0        0        0     1179 2023-05-31 08:12:05.000000 migration_db-1.0.6/migration_db/common/file.py
--rw-rw-rw-   0        0        0      581 2023-12-14 10:16:04.000000 migration_db-1.0.6/migration_db/common/format_time.py
--rw-rw-rw-   0        0        0     2162 2024-02-05 10:15:53.000000 migration_db-1.0.6/migration_db/common/handle_git.py
--rw-rw-rw-   0        0        0      477 2020-12-24 07:05:06.000000 migration_db-1.0.6/migration_db/common/handle_remove_read_only.py
--rw-rw-rw-   0        0        0     4705 2024-01-17 08:26:53.000000 migration_db-1.0.6/migration_db/common/handle_str.py
--rw-rw-rw-   0        0        0     1503 2023-11-07 08:02:22.000000 migration_db-1.0.6/migration_db/common/lib.py
--rw-rw-rw-   0        0        0     2713 2024-02-19 06:06:43.000000 migration_db-1.0.6/migration_db/common/log.py
--rw-rw-rw-   0        0        0     7702 2023-12-15 09:02:25.000000 migration_db-1.0.6/migration_db/common/my_db.py
--rw-rw-rw-   0        0        0     2055 2024-04-08 03:43:19.000000 migration_db-1.0.6/migration_db/common/path.py
--rw-rw-rw-   0        0        0     2047 2023-07-31 09:19:01.000000 migration_db-1.0.6/migration_db/common/read_file.py
--rw-rw-rw-   0        0        0      408 2021-08-03 02:42:25.000000 migration_db-1.0.6/migration_db/common/template_parse.py
--rw-rw-rw-   0        0        0      951 2024-02-19 06:42:00.000000 migration_db-1.0.6/migration_db/common/write_file.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:36.935712 migration_db-1.0.6/migration_db/migration/
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:37.904646 migration_db-1.0.6/migration_db/migration/core/
--rw-rw-rw-   0        0        0    12740 2024-04-30 08:49:09.000000 migration_db-1.0.6/migration_db/migration/core/_migration.py
--rw-rw-rw-   0        0        0      985 2024-05-06 01:56:25.000000 migration_db-1.0.6/migration_db/migration/core/backup.py
--rw-rw-rw-   0        0        0     1990 2024-01-15 08:02:29.000000 migration_db-1.0.6/migration_db/migration/core/base.py
--rw-rw-rw-   0        0        0    16811 2024-02-19 07:29:21.000000 migration_db-1.0.6/migration_db/migration/core/build_update_sql.py
--rw-rw-rw-   0        0        0     5672 2024-04-30 07:52:21.000000 migration_db-1.0.6/migration_db/migration/core/execute_script.py
--rw-rw-rw-   0        0        0     3087 2024-05-06 02:16:09.000000 migration_db-1.0.6/migration_db/migration/core/handle_archive_file.py
--rw-rw-rw-   0        0        0      754 2023-05-06 06:41:30.000000 migration_db-1.0.6/migration_db/migration/core/handle_external_condition_mapping_data.py
--rw-rw-rw-   0        0        0     1339 2023-03-24 13:30:58.000000 migration_db-1.0.6/migration_db/migration/core/handle_procedures.py
--rw-rw-rw-   0        0        0     1840 2023-03-28 07:10:57.000000 migration_db-1.0.6/migration_db/migration/core/handle_special_field.py
--rw-rw-rw-   0        0        0     1711 2022-08-30 02:56:27.000000 migration_db-1.0.6/migration_db/migration/core/handle_table_action.py
--rw-rw-rw-   0        0        0    10110 2024-04-23 08:01:53.000000 migration_db-1.0.6/migration_db/migration/core/incremental_sql.py
--rw-rw-rw-   0        0        0     5211 2023-09-21 04:39:01.000000 migration_db-1.0.6/migration_db/migration/core/match_ids.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:38.068982 migration_db-1.0.6/migration_db/migration/core/models/
--rw-rw-rw-   0        0        0     1115 2021-03-16 05:40:58.000000 migration_db-1.0.6/migration_db/migration/core/models/config.py
--rw-rw-rw-   0        0        0      709 2023-09-08 02:39:23.000000 migration_db-1.0.6/migration_db/migration/core/models/file_detail.py
--rw-rw-rw-   0        0        0     2436 2023-03-24 13:00:15.000000 migration_db-1.0.6/migration_db/migration/core/models/table_detail.py
--rw-rw-rw-   0        0        0     1574 2024-02-19 07:27:11.000000 migration_db-1.0.6/migration_db/migration/core/redis_biz.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:38.170169 migration_db-1.0.6/migration_db/migration/core/split_sql/
--rw-rw-rw-   0        0        0     5463 2023-09-25 08:55:57.000000 migration_db-1.0.6/migration_db/migration/core/split_sql/split_sql.py
--rw-rw-rw-   0        0        0     2138 2024-05-06 02:11:57.000000 migration_db-1.0.6/migration_db/migration/core/switch_data_source.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:38.303856 migration_db-1.0.6/migration_db/migration/db/
--rw-rw-rw-   0        0        0     8020 2024-01-15 07:44:36.000000 migration_db-1.0.6/migration_db/migration/db/admin_db.py
--rw-rw-rw-   0        0        0     2373 2024-02-27 06:56:06.000000 migration_db-1.0.6/migration_db/migration/db/base_db.py
--rw-rw-rw-   0        0        0      460 2023-03-02 01:37:13.000000 migration_db-1.0.6/migration_db/migration/db/design_db.py
--rw-rw-rw-   0        0        0     1260 2023-03-14 09:20:46.000000 migration_db-1.0.6/migration_db/migration/db/edc_db.py
--rw-rw-rw-   0        0        0      693 2023-09-21 01:31:22.000000 migration_db-1.0.6/migration_db/migration/db/iwrs_db.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:38.337378 migration_db-1.0.6/migration_db/migration/docs/
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:38.412805 migration_db-1.0.6/migration_db/migration/docs/common_sql/
--rw-rw-rw-   0        0        0     2370 2023-03-27 01:40:59.000000 migration_db-1.0.6/migration_db/migration/docs/common_sql/create_procedure.sql
--rw-rw-rw-   0        0        0      128 2023-03-30 06:10:59.000000 migration_db-1.0.6/migration_db/migration/docs/common_sql/drop_procedure.sql
--rw-rw-rw-   0        0        0      871 2022-05-30 09:06:22.000000 migration_db-1.0.6/migration_db/migration/docs/common_sql/eclinical_schema_history.sql
--rw-rw-rw-   0        0        0    29341 2024-04-30 08:08:27.000000 migration_db-1.0.6/migration_db/migration/docs/config_info.json
--rw-rw-rw-   0        0        0      982 2023-07-31 03:14:53.000000 migration_db-1.0.6/migration_db/migration/docs/redis_detail.json
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:38.488657 migration_db-1.0.6/migration_db/migration/docs/template/
--rw-rw-rw-   0        0        0      213 2023-06-07 10:37:29.000000 migration_db-1.0.6/migration_db/migration/docs/template/mysql-shell-dump.j2
--rw-rw-rw-   0        0        0      219 2023-06-07 10:37:27.000000 migration_db-1.0.6/migration_db/migration/docs/template/mysql-shell-load-dump.j2
--rw-rw-rw-   0        0        0      429 2022-06-26 13:22:39.000000 migration_db-1.0.6/migration_db/migration/docs/template/parse.py
--rw-rw-rw-   0        0        0     1146 2023-03-24 13:00:15.000000 migration_db-1.0.6/migration_db/migration/docs/template/update_id_template.j2
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:38.625250 migration_db-1.0.6/migration_db/migration/helper/
--rw-rw-rw-   0        0        0      831 2024-05-06 01:59:04.000000 migration_db-1.0.6/migration_db/migration/helper/backup_by_database.py
--rw-rw-rw-   0        0        0     2388 2024-04-30 07:52:21.000000 migration_db-1.0.6/migration_db/migration/helper/run_edc.py
--rw-rw-rw-   0        0        0     2661 2024-04-30 07:52:21.000000 migration_db-1.0.6/migration_db/migration/helper/run_pv.py
--rw-rw-rw-   0        0        0    11665 2024-04-30 07:52:21.000000 migration_db-1.0.6/migration_db/migration/helper/run_split_sql.py
--rw-rw-rw-   0        0        0     1407 2024-04-30 07:52:21.000000 migration_db-1.0.6/migration_db/migration/helper/run_table_action.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:38.882969 migration_db-1.0.6/migration_db/migration/lib/
--rw-rw-rw-   0        0        0     2282 2020-12-23 14:18:08.000000 migration_db-1.0.6/migration_db/migration/lib/compareTwoDict.py
--rw-rw-rw-   0        0        0     2422 2024-01-18 08:52:06.000000 migration_db-1.0.6/migration_db/migration/lib/constant.py
--rw-rw-rw-   0        0        0     2282 2024-02-19 07:26:01.000000 migration_db-1.0.6/migration_db/migration/lib/handle_redis.py
--rw-rw-rw-   0        0        0      602 2023-08-07 06:38:30.000000 migration_db-1.0.6/migration_db/migration/lib/handle_str.py
--rw-rw-rw-   0        0        0     5757 2024-02-19 07:24:41.000000 migration_db-1.0.6/migration_db/migration/lib/my_db.py
--rw-rw-rw-   0        0        0     2384 2021-08-07 06:57:33.000000 migration_db-1.0.6/migration_db/migration/lib/my_excel.py
--rw-rw-rw-   0        0        0     5867 2024-02-05 12:03:52.000000 migration_db-1.0.6/migration_db/migration/lib/mysql_connector.py
--rw-rw-rw-   0        0        0     3277 2024-02-19 07:29:21.000000 migration_db-1.0.6/migration_db/migration/lib/mysql_shell.py
--rw-rw-rw-   0        0        0     1531 2023-10-29 07:05:46.000000 migration_db-1.0.6/migration_db/migration/lib/mysql_task.py
--rw-rw-rw-   0        0        0     1506 2024-04-30 08:10:52.000000 migration_db-1.0.6/migration_db/migration/lib/path.py
--rw-rw-rw-   0        0        0      376 2024-03-04 09:45:05.000000 migration_db-1.0.6/migration_db/migration/lib/synchronized.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:21:38.973597 migration_db-1.0.6/migration_db.egg-info/
--rw-rw-rw-   0        0        0      330 2024-05-06 02:21:36.000000 migration_db-1.0.6/migration_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6418 2024-05-06 02:21:36.000000 migration_db-1.0.6/migration_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 02:21:36.000000 migration_db-1.0.6/migration_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-05-06 02:21:36.000000 migration_db-1.0.6/migration_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 02:21:36.000000 migration_db-1.0.6/migration_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 02:21:39.037582 migration_db-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      979 2024-04-30 08:58:50.000000 migration_db-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.835863 migration_db-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-02-14 02:04:04.000000 migration_db-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       42 2024-04-30 06:49:17.000000 migration_db-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      330 2024-05-06 02:38:09.834864 migration_db-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-04-30 07:55:39.000000 migration_db-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.271316 migration_db-1.0.7/migration_db/
+-rw-rw-rw-   0        0        0      172 2024-05-06 02:38:00.000000 migration_db-1.0.7/migration_db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.323176 migration_db-1.0.7/migration_db/common/
+-rw-rw-rw-   0        0        0      564 2023-07-14 03:27:20.000000 migration_db-1.0.7/migration_db/common/calc_time.py
+-rw-rw-rw-   0        0        0     2375 2023-07-31 07:46:04.000000 migration_db-1.0.7/migration_db/common/compare_two_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.336141 migration_db-1.0.7/migration_db/common/conf/
+-rw-rw-rw-   0        0        0     1212 2023-02-23 08:16:11.000000 migration_db-1.0.7/migration_db/common/conf/config.py
+-rw-rw-rw-   0        0        0      490 2023-11-20 10:13:23.000000 migration_db-1.0.7/migration_db/common/conf/constant.py
+-rw-rw-rw-   0        0        0     1782 2023-07-17 03:00:20.000000 migration_db-1.0.7/migration_db/common/conf/data_source_route.py
+-rw-rw-rw-   0        0        0     1942 2023-07-31 03:14:53.000000 migration_db-1.0.7/migration_db/common/conf/datasource.json
+-rw-rw-rw-   0        0        0     1242 2023-02-23 08:15:20.000000 migration_db-1.0.7/migration_db/common/conf/study_info_route.py
+-rw-rw-rw-   0        0        0     1368 2024-01-17 08:08:39.000000 migration_db-1.0.7/migration_db/common/constant.py
+-rw-rw-rw-   0        0        0     1176 2024-02-19 06:49:07.000000 migration_db-1.0.7/migration_db/common/create_folder.py
+-rw-rw-rw-   0        0        0      875 2024-04-11 10:28:33.000000 migration_db-1.0.7/migration_db/common/database.py
+-rw-rw-rw-   0        0        0     1179 2023-05-31 08:12:05.000000 migration_db-1.0.7/migration_db/common/file.py
+-rw-rw-rw-   0        0        0      581 2023-12-14 10:16:04.000000 migration_db-1.0.7/migration_db/common/format_time.py
+-rw-rw-rw-   0        0        0     2162 2024-02-05 10:15:53.000000 migration_db-1.0.7/migration_db/common/handle_git.py
+-rw-rw-rw-   0        0        0      477 2020-12-24 07:05:06.000000 migration_db-1.0.7/migration_db/common/handle_remove_read_only.py
+-rw-rw-rw-   0        0        0     4705 2024-01-17 08:26:53.000000 migration_db-1.0.7/migration_db/common/handle_str.py
+-rw-rw-rw-   0        0        0     1503 2023-11-07 08:02:22.000000 migration_db-1.0.7/migration_db/common/lib.py
+-rw-rw-rw-   0        0        0     2713 2024-02-19 06:06:43.000000 migration_db-1.0.7/migration_db/common/log.py
+-rw-rw-rw-   0        0        0     7702 2023-12-15 09:02:25.000000 migration_db-1.0.7/migration_db/common/my_db.py
+-rw-rw-rw-   0        0        0     2055 2024-04-08 03:43:19.000000 migration_db-1.0.7/migration_db/common/path.py
+-rw-rw-rw-   0        0        0     2047 2023-07-31 09:19:01.000000 migration_db-1.0.7/migration_db/common/read_file.py
+-rw-rw-rw-   0        0        0      408 2021-08-03 02:42:25.000000 migration_db-1.0.7/migration_db/common/template_parse.py
+-rw-rw-rw-   0        0        0      951 2024-02-19 06:42:00.000000 migration_db-1.0.7/migration_db/common/write_file.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.253361 migration_db-1.0.7/migration_db/migration/
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.444855 migration_db-1.0.7/migration_db/migration/core/
+-rw-rw-rw-   0        0        0    12740 2024-04-30 08:49:09.000000 migration_db-1.0.7/migration_db/migration/core/_migration.py
+-rw-rw-rw-   0        0        0     1144 2024-05-06 02:36:48.000000 migration_db-1.0.7/migration_db/migration/core/backup.py
+-rw-rw-rw-   0        0        0     1990 2024-01-15 08:02:29.000000 migration_db-1.0.7/migration_db/migration/core/base.py
+-rw-rw-rw-   0        0        0    16811 2024-02-19 07:29:21.000000 migration_db-1.0.7/migration_db/migration/core/build_update_sql.py
+-rw-rw-rw-   0        0        0     5672 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/core/execute_script.py
+-rw-rw-rw-   0        0        0     3087 2024-05-06 02:16:09.000000 migration_db-1.0.7/migration_db/migration/core/handle_archive_file.py
+-rw-rw-rw-   0        0        0      754 2023-05-06 06:41:30.000000 migration_db-1.0.7/migration_db/migration/core/handle_external_condition_mapping_data.py
+-rw-rw-rw-   0        0        0     1339 2023-03-24 13:30:58.000000 migration_db-1.0.7/migration_db/migration/core/handle_procedures.py
+-rw-rw-rw-   0        0        0     1840 2023-03-28 07:10:57.000000 migration_db-1.0.7/migration_db/migration/core/handle_special_field.py
+-rw-rw-rw-   0        0        0     1711 2022-08-30 02:56:27.000000 migration_db-1.0.7/migration_db/migration/core/handle_table_action.py
+-rw-rw-rw-   0        0        0    10110 2024-04-23 08:01:53.000000 migration_db-1.0.7/migration_db/migration/core/incremental_sql.py
+-rw-rw-rw-   0        0        0     5211 2023-09-21 04:39:01.000000 migration_db-1.0.7/migration_db/migration/core/match_ids.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.465795 migration_db-1.0.7/migration_db/migration/core/models/
+-rw-rw-rw-   0        0        0     1115 2021-03-16 05:40:58.000000 migration_db-1.0.7/migration_db/migration/core/models/config.py
+-rw-rw-rw-   0        0        0      709 2023-09-08 02:39:23.000000 migration_db-1.0.7/migration_db/migration/core/models/file_detail.py
+-rw-rw-rw-   0        0        0     2436 2023-03-24 13:00:15.000000 migration_db-1.0.7/migration_db/migration/core/models/table_detail.py
+-rw-rw-rw-   0        0        0     1574 2024-02-19 07:27:11.000000 migration_db-1.0.7/migration_db/migration/core/redis_biz.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.478761 migration_db-1.0.7/migration_db/migration/core/split_sql/
+-rw-rw-rw-   0        0        0     5463 2023-09-25 08:55:57.000000 migration_db-1.0.7/migration_db/migration/core/split_sql/split_sql.py
+-rw-rw-rw-   0        0        0     2138 2024-05-06 02:11:57.000000 migration_db-1.0.7/migration_db/migration/core/switch_data_source.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.520647 migration_db-1.0.7/migration_db/migration/db/
+-rw-rw-rw-   0        0        0     8020 2024-01-15 07:44:36.000000 migration_db-1.0.7/migration_db/migration/db/admin_db.py
+-rw-rw-rw-   0        0        0     2373 2024-02-27 06:56:06.000000 migration_db-1.0.7/migration_db/migration/db/base_db.py
+-rw-rw-rw-   0        0        0      460 2023-03-02 01:37:13.000000 migration_db-1.0.7/migration_db/migration/db/design_db.py
+-rw-rw-rw-   0        0        0     1260 2023-03-14 09:20:46.000000 migration_db-1.0.7/migration_db/migration/db/edc_db.py
+-rw-rw-rw-   0        0        0      693 2023-09-21 01:31:22.000000 migration_db-1.0.7/migration_db/migration/db/iwrs_db.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.557603 migration_db-1.0.7/migration_db/migration/docs/
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.587527 migration_db-1.0.7/migration_db/migration/docs/common_sql/
+-rw-rw-rw-   0        0        0     2370 2023-03-27 01:40:59.000000 migration_db-1.0.7/migration_db/migration/docs/common_sql/create_procedure.sql
+-rw-rw-rw-   0        0        0      128 2023-03-30 06:10:59.000000 migration_db-1.0.7/migration_db/migration/docs/common_sql/drop_procedure.sql
+-rw-rw-rw-   0        0        0      871 2022-05-30 09:06:22.000000 migration_db-1.0.7/migration_db/migration/docs/common_sql/eclinical_schema_history.sql
+-rw-rw-rw-   0        0        0    29341 2024-04-30 08:08:27.000000 migration_db-1.0.7/migration_db/migration/docs/config_info.json
+-rw-rw-rw-   0        0        0      982 2023-07-31 03:14:53.000000 migration_db-1.0.7/migration_db/migration/docs/redis_detail.json
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.608469 migration_db-1.0.7/migration_db/migration/docs/template/
+-rw-rw-rw-   0        0        0      213 2023-06-07 10:37:29.000000 migration_db-1.0.7/migration_db/migration/docs/template/mysql-shell-dump.j2
+-rw-rw-rw-   0        0        0      219 2023-06-07 10:37:27.000000 migration_db-1.0.7/migration_db/migration/docs/template/mysql-shell-load-dump.j2
+-rw-rw-rw-   0        0        0      429 2022-06-26 13:22:39.000000 migration_db-1.0.7/migration_db/migration/docs/template/parse.py
+-rw-rw-rw-   0        0        0     1146 2023-03-24 13:00:15.000000 migration_db-1.0.7/migration_db/migration/docs/template/update_id_template.j2
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.670303 migration_db-1.0.7/migration_db/migration/helper/
+-rw-rw-rw-   0        0        0      831 2024-05-06 01:59:04.000000 migration_db-1.0.7/migration_db/migration/helper/backup_by_database.py
+-rw-rw-rw-   0        0        0     2388 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/helper/run_edc.py
+-rw-rw-rw-   0        0        0     2661 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/helper/run_pv.py
+-rw-rw-rw-   0        0        0    11665 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/helper/run_split_sql.py
+-rw-rw-rw-   0        0        0     1407 2024-04-30 07:52:21.000000 migration_db-1.0.7/migration_db/migration/helper/run_table_action.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.754082 migration_db-1.0.7/migration_db/migration/lib/
+-rw-rw-rw-   0        0        0     2282 2020-12-23 14:18:08.000000 migration_db-1.0.7/migration_db/migration/lib/compareTwoDict.py
+-rw-rw-rw-   0        0        0     2422 2024-01-18 08:52:06.000000 migration_db-1.0.7/migration_db/migration/lib/constant.py
+-rw-rw-rw-   0        0        0     2282 2024-02-19 07:26:01.000000 migration_db-1.0.7/migration_db/migration/lib/handle_redis.py
+-rw-rw-rw-   0        0        0      602 2023-08-07 06:38:30.000000 migration_db-1.0.7/migration_db/migration/lib/handle_str.py
+-rw-rw-rw-   0        0        0     5757 2024-02-19 07:24:41.000000 migration_db-1.0.7/migration_db/migration/lib/my_db.py
+-rw-rw-rw-   0        0        0     2384 2021-08-07 06:57:33.000000 migration_db-1.0.7/migration_db/migration/lib/my_excel.py
+-rw-rw-rw-   0        0        0     5867 2024-02-05 12:03:52.000000 migration_db-1.0.7/migration_db/migration/lib/mysql_connector.py
+-rw-rw-rw-   0        0        0     3277 2024-02-19 07:29:21.000000 migration_db-1.0.7/migration_db/migration/lib/mysql_shell.py
+-rw-rw-rw-   0        0        0     1531 2023-10-29 07:05:46.000000 migration_db-1.0.7/migration_db/migration/lib/mysql_task.py
+-rw-rw-rw-   0        0        0     1506 2024-04-30 08:10:52.000000 migration_db-1.0.7/migration_db/migration/lib/path.py
+-rw-rw-rw-   0        0        0      376 2024-03-04 09:45:05.000000 migration_db-1.0.7/migration_db/migration/lib/synchronized.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:38:09.804945 migration_db-1.0.7/migration_db.egg-info/
+-rw-rw-rw-   0        0        0      330 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6418 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 02:38:09.000000 migration_db-1.0.7/migration_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 02:38:09.836865 migration_db-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      979 2024-04-30 08:58:50.000000 migration_db-1.0.7/setup.py
```

### Comparing `migration_db-1.0.6/LICENSE` & `migration_db-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/calc_time.py` & `migration_db-1.0.7/migration_db/common/calc_time.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/compare_two_dict.py` & `migration_db-1.0.7/migration_db/common/compare_two_dict.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/conf/config.py` & `migration_db-1.0.7/migration_db/common/conf/config.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/conf/data_source_route.py` & `migration_db-1.0.7/migration_db/common/conf/data_source_route.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/conf/datasource.json` & `migration_db-1.0.7/migration_db/common/conf/datasource.json`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/conf/study_info_route.py` & `migration_db-1.0.7/migration_db/common/conf/study_info_route.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/constant.py` & `migration_db-1.0.7/migration_db/common/constant.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/create_folder.py` & `migration_db-1.0.7/migration_db/common/create_folder.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/database.py` & `migration_db-1.0.7/migration_db/common/database.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/file.py` & `migration_db-1.0.7/migration_db/common/file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/format_time.py` & `migration_db-1.0.7/migration_db/common/format_time.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/handle_git.py` & `migration_db-1.0.7/migration_db/common/handle_git.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/handle_str.py` & `migration_db-1.0.7/migration_db/common/handle_str.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/lib.py` & `migration_db-1.0.7/migration_db/common/lib.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/log.py` & `migration_db-1.0.7/migration_db/common/log.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/my_db.py` & `migration_db-1.0.7/migration_db/common/my_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/path.py` & `migration_db-1.0.7/migration_db/common/path.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/read_file.py` & `migration_db-1.0.7/migration_db/common/read_file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/common/write_file.py` & `migration_db-1.0.7/migration_db/common/write_file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/_migration.py` & `migration_db-1.0.7/migration_db/migration/core/_migration.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/backup.py` & `migration_db-1.0.7/migration_db/migration/core/backup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 """
 @Author: xiaodong.li
 @Time: 5/6/2024 9:54 AM
 @Description: Description
 @File: backup.py
 """
 import os
+import sys
 import zipfile
 
+sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.realpath(__file__)))))
 from common.conf.data_source_route import DataSourceRoute
 from migration.lib.mysql_task import MysqlTask
 from migration.lib.path import build_sql_file_path
 
 
-def backup(dir_path, host_alias, db_name, sql_name, _is_compress=False):
+def backup(dir_path, host_alias, db_name, sql_name, _is_compress=False, data_source=None):
     local_sql_path = build_sql_file_path(dir_path, sql_name)
-    data_source = DataSourceRoute().build_config(host_alias, use_config_obj=False)
+    if data_source is None:
+        data_source = DataSourceRoute().build_config(host_alias, use_config_obj=False)
     data_source["db"] = db_name
     MysqlTask(**data_source).mysqldump_task(local_sql_path)
     if _is_compress is True:
         zip_backup_path = os.path.join(dir_path, sql_name + ".zip")
         with zipfile.ZipFile(zip_backup_path, "w", zipfile.ZIP_DEFLATED) as zipf:
             zipf.write(local_sql_path, arcname=sql_name + ".sql")
         if os.path.exists(local_sql_path):
```

### Comparing `migration_db-1.0.6/migration_db/migration/core/base.py` & `migration_db-1.0.7/migration_db/migration/core/base.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/build_update_sql.py` & `migration_db-1.0.7/migration_db/migration/core/build_update_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/execute_script.py` & `migration_db-1.0.7/migration_db/migration/core/execute_script.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/handle_archive_file.py` & `migration_db-1.0.7/migration_db/migration/core/handle_archive_file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/handle_external_condition_mapping_data.py` & `migration_db-1.0.7/migration_db/migration/core/handle_external_condition_mapping_data.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/handle_procedures.py` & `migration_db-1.0.7/migration_db/migration/core/handle_procedures.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/handle_special_field.py` & `migration_db-1.0.7/migration_db/migration/core/handle_special_field.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/handle_table_action.py` & `migration_db-1.0.7/migration_db/migration/core/handle_table_action.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/incremental_sql.py` & `migration_db-1.0.7/migration_db/migration/core/incremental_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/match_ids.py` & `migration_db-1.0.7/migration_db/migration/core/match_ids.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/models/config.py` & `migration_db-1.0.7/migration_db/migration/core/models/config.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/models/file_detail.py` & `migration_db-1.0.7/migration_db/migration/core/models/file_detail.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/models/table_detail.py` & `migration_db-1.0.7/migration_db/migration/core/models/table_detail.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/redis_biz.py` & `migration_db-1.0.7/migration_db/migration/core/redis_biz.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/split_sql/split_sql.py` & `migration_db-1.0.7/migration_db/migration/core/split_sql/split_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/core/switch_data_source.py` & `migration_db-1.0.7/migration_db/migration/core/switch_data_source.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/db/admin_db.py` & `migration_db-1.0.7/migration_db/migration/db/admin_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/db/base_db.py` & `migration_db-1.0.7/migration_db/migration/db/base_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/db/edc_db.py` & `migration_db-1.0.7/migration_db/migration/db/edc_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/db/iwrs_db.py` & `migration_db-1.0.7/migration_db/migration/db/iwrs_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/docs/common_sql/create_procedure.sql` & `migration_db-1.0.7/migration_db/migration/docs/common_sql/create_procedure.sql`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/docs/common_sql/eclinical_schema_history.sql` & `migration_db-1.0.7/migration_db/migration/docs/common_sql/eclinical_schema_history.sql`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/docs/config_info.json` & `migration_db-1.0.7/migration_db/migration/docs/config_info.json`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/docs/redis_detail.json` & `migration_db-1.0.7/migration_db/migration/docs/redis_detail.json`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/docs/template/update_id_template.j2` & `migration_db-1.0.7/migration_db/migration/docs/template/update_id_template.j2`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/helper/backup_by_database.py` & `migration_db-1.0.7/migration_db/migration/helper/backup_by_database.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/helper/run_edc.py` & `migration_db-1.0.7/migration_db/migration/helper/run_edc.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/helper/run_pv.py` & `migration_db-1.0.7/migration_db/migration/helper/run_pv.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/helper/run_split_sql.py` & `migration_db-1.0.7/migration_db/migration/helper/run_split_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/helper/run_table_action.py` & `migration_db-1.0.7/migration_db/migration/helper/run_table_action.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/compareTwoDict.py` & `migration_db-1.0.7/migration_db/migration/lib/compareTwoDict.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/constant.py` & `migration_db-1.0.7/migration_db/migration/lib/constant.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/handle_redis.py` & `migration_db-1.0.7/migration_db/migration/lib/handle_redis.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/handle_str.py` & `migration_db-1.0.7/migration_db/migration/lib/handle_str.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/my_db.py` & `migration_db-1.0.7/migration_db/migration/lib/my_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/my_excel.py` & `migration_db-1.0.7/migration_db/migration/lib/my_excel.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/mysql_connector.py` & `migration_db-1.0.7/migration_db/migration/lib/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/mysql_shell.py` & `migration_db-1.0.7/migration_db/migration/lib/mysql_shell.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/mysql_task.py` & `migration_db-1.0.7/migration_db/migration/lib/mysql_task.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db/migration/lib/path.py` & `migration_db-1.0.7/migration_db/migration/lib/path.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/migration_db.egg-info/SOURCES.txt` & `migration_db-1.0.7/migration_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.6/setup.py` & `migration_db-1.0.7/setup.py`

 * *Files identical despite different names*

