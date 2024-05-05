# Comparing `tmp/graphlit_client-1.0.20240429002.tar.gz` & `tmp/graphlit_client-1.0.20240505001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240429002.tar", last modified: Mon Apr 29 19:19:38 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240505001.tar", last modified: Sun May  5 22:14:26 2024, max compression
```

## Comparing `graphlit_client-1.0.20240429002.tar` & `graphlit_client-1.0.20240505001.tar`

### file list

```diff
@@ -1,166 +1,184 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 19:19:38.582396 graphlit_client-1.0.20240429002/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-29 19:19:38.582396 graphlit_client-1.0.20240429002/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 19:19:38.506395 graphlit_client-1.0.20240429002/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2689 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 19:19:38.582396 graphlit_client-1.0.20240429002/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    72910 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    77051 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16975 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7261 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4502 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    69307 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53809 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      750 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/publish_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_content_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8887 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      727 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4953 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/update_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/graphlit_api/usage.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 19:19:38.582396 graphlit_client-1.0.20240429002/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-29 19:19:38.000000 graphlit_client-1.0.20240429002/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4997 2024-04-29 19:19:38.000000 graphlit_client-1.0.20240429002/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-29 19:19:38.000000 graphlit_client-1.0.20240429002/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-29 19:19:38.000000 graphlit_client-1.0.20240429002/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-29 19:19:38.000000 graphlit_client-1.0.20240429002/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-29 19:19:38.582396 graphlit_client-1.0.20240429002/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-29 19:19:19.000000 graphlit_client-1.0.20240429002/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 22:14:26.212003 graphlit_client-1.0.20240505001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-05 22:14:26.212003 graphlit_client-1.0.20240505001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 22:14:26.180003 graphlit_client-1.0.20240505001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1878 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 22:14:26.212003 graphlit_client-1.0.20240505001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    82101 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    95409 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/count_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8528 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      506 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17117 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9686 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4286 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5193 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7962 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    78479 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    66376 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3382 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2390 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/publish_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10533 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11920 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_contents_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_contents_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4895 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1004 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5666 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1502 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8940 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8528 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/graphlit_api/update_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 22:14:26.212003 graphlit_client-1.0.20240505001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-05 22:14:26.000000 graphlit_client-1.0.20240505001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5600 2024-05-05 22:14:26.000000 graphlit_client-1.0.20240505001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 22:14:26.000000 graphlit_client-1.0.20240505001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-05 22:14:26.000000 graphlit_client-1.0.20240505001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-05 22:14:26.000000 graphlit_client-1.0.20240505001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-05 22:14:26.212003 graphlit_client-1.0.20240505001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-05-05 22:14:08.000000 graphlit_client-1.0.20240505001/setup.py
```

### Comparing `graphlit_client-1.0.20240429002/LICENSE` & `graphlit_client-1.0.20240505001/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/PKG-INFO` & `graphlit_client-1.0.20240505001/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240429002
+Version: 1.0.20240505001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240429002/README.md` & `graphlit_client-1.0.20240505001/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/__init__.py` & `graphlit_client-1.0.20240505001/graphlit_api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,39 @@
     AddContentsToCollectionsAddContentsToCollectionsContents,
 )
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel, Upload
 from .clear_conversation import ClearConversation, ClearConversationClearConversation
 from .client import Client
 from .close_conversation import CloseConversation, CloseConversationCloseConversation
+from .count_alerts import CountAlerts, CountAlertsCountAlerts
+from .count_categories import CountCategories, CountCategoriesCountCategories
+from .count_collections import CountCollections, CountCollectionsCountCollections
+from .count_contents import CountContents, CountContentsCountContents
+from .count_conversations import (
+    CountConversations,
+    CountConversationsCountConversations,
+)
+from .count_events import CountEvents, CountEventsCountEvents
+from .count_feeds import CountFeeds, CountFeedsCountFeeds
+from .count_labels import CountLabels, CountLabelsCountLabels
+from .count_organizations import (
+    CountOrganizations,
+    CountOrganizationsCountOrganizations,
+)
+from .count_persons import CountPersons, CountPersonsCountPersons
+from .count_places import CountPlaces, CountPlacesCountPlaces
+from .count_products import CountProducts, CountProductsCountProducts
+from .count_repos import CountRepos, CountReposCountRepos
+from .count_softwares import CountSoftwares, CountSoftwaresCountSoftwares
+from .count_specifications import (
+    CountSpecifications,
+    CountSpecificationsCountSpecifications,
+)
+from .count_workflows import CountWorkflows, CountWorkflowsCountWorkflows
 from .create_alert import CreateAlert, CreateAlertCreateAlert
 from .create_category import CreateCategory, CreateCategoryCreateCategory
 from .create_collection import CreateCollection, CreateCollectionCreateCollection
 from .create_conversation import (
     CreateConversation,
     CreateConversationCreateConversation,
 )
@@ -61,15 +86,14 @@
     CreateWorkflowCreateWorkflowPreparationJobsConnectorAzureDocument,
     CreateWorkflowCreateWorkflowPreparationJobsConnectorDeepgram,
     CreateWorkflowCreateWorkflowPreparationJobsConnectorDocument,
     CreateWorkflowCreateWorkflowPreparationJobsConnectorEmail,
     CreateWorkflowCreateWorkflowPreparationSummarizations,
     CreateWorkflowCreateWorkflowPreparationSummarizationsSpecification,
 )
-from .credits import Credits, CreditsCredits
 from .delete_alert import DeleteAlert, DeleteAlertDeleteAlert
 from .delete_alerts import DeleteAlerts, DeleteAlertsDeleteAlerts
 from .delete_all_alerts import DeleteAllAlerts, DeleteAllAlertsDeleteAllAlerts
 from .delete_all_categories import (
     DeleteAllCategories,
     DeleteAllCategoriesDeleteAllCategories,
 )
@@ -93,14 +117,18 @@
 from .delete_all_places import DeleteAllPlaces, DeleteAllPlacesDeleteAllPlaces
 from .delete_all_products import DeleteAllProducts, DeleteAllProductsDeleteAllProducts
 from .delete_all_repos import DeleteAllRepos, DeleteAllReposDeleteAllRepos
 from .delete_all_softwares import (
     DeleteAllSoftwares,
     DeleteAllSoftwaresDeleteAllSoftwares,
 )
+from .delete_all_specifications import (
+    DeleteAllSpecifications,
+    DeleteAllSpecificationsDeleteAllSpecifications,
+)
 from .delete_all_workflows import (
     DeleteAllWorkflows,
     DeleteAllWorkflowsDeleteAllWorkflows,
 )
 from .delete_categories import DeleteCategories, DeleteCategoriesDeleteCategories
 from .delete_category import DeleteCategory, DeleteCategoryDeleteCategory
 from .delete_collection import DeleteCollection, DeleteCollectionDeleteCollection
@@ -140,14 +168,18 @@
 from .delete_repos import DeleteRepos, DeleteReposDeleteRepos
 from .delete_software import DeleteSoftware, DeleteSoftwareDeleteSoftware
 from .delete_softwares import DeleteSoftwares, DeleteSoftwaresDeleteSoftwares
 from .delete_specification import (
     DeleteSpecification,
     DeleteSpecificationDeleteSpecification,
 )
+from .delete_specifications import (
+    DeleteSpecifications,
+    DeleteSpecificationsDeleteSpecifications,
+)
 from .delete_workflow import DeleteWorkflow, DeleteWorkflowDeleteWorkflow
 from .delete_workflows import DeleteWorkflows, DeleteWorkflowsDeleteWorkflows
 from .disable_alert import DisableAlert, DisableAlertDisableAlert
 from .disable_feed import DisableFeed, DisableFeedDisableFeed
 from .enable_alert import EnableAlert, EnableAlertEnableAlert
 from .enable_feed import EnableFeed, EnableFeedEnableFeed
 from .enums import (
@@ -270,33 +302,39 @@
     GetCollectionCollection,
     GetCollectionCollectionContents,
     GetCollectionCollectionOwner,
 )
 from .get_content import (
     GetContent,
     GetContentContent,
+    GetContentContentAddress,
     GetContentContentAudio,
     GetContentContentChildren,
     GetContentContentCollections,
     GetContentContentDocument,
     GetContentContentEmail,
     GetContentContentEmailBcc,
     GetContentContentEmailCc,
     GetContentContentEmailFrom,
     GetContentContentEmailTo,
     GetContentContentFeed,
     GetContentContentImage,
     GetContentContentIssue,
     GetContentContentLinks,
+    GetContentContentLocation,
     GetContentContentObservations,
     GetContentContentObservationsObservable,
     GetContentContentObservationsOccurrences,
     GetContentContentObservationsOccurrencesBoundingBox,
     GetContentContentOwner,
+    GetContentContentPackage,
+    GetContentContentPages,
+    GetContentContentPagesChunks,
     GetContentContentParent,
+    GetContentContentSegments,
     GetContentContentVideo,
     GetContentContentWorkflow,
 )
 from .get_conversation import (
     GetConversation,
     GetConversationConversation,
     GetConversationConversationFilter,
@@ -363,14 +401,15 @@
 from .get_repo import GetRepo, GetRepoRepo
 from .get_software import GetSoftware, GetSoftwareSoftware
 from .get_specification import (
     GetSpecification,
     GetSpecificationSpecification,
     GetSpecificationSpecificationAnthropic,
     GetSpecificationSpecificationAzureOpenAi,
+    GetSpecificationSpecificationCohere,
     GetSpecificationSpecificationOpenAi,
     GetSpecificationSpecificationOwner,
     GetSpecificationSpecificationPromptStrategy,
     GetSpecificationSpecificationReplicate,
     GetSpecificationSpecificationRerankingStrategy,
     GetSpecificationSpecificationRetrievalStrategy,
     GetSpecificationSpecificationStrategy,
@@ -404,30 +443,39 @@
     GetWorkflowWorkflowPreparationJobsConnectorAzureDocument,
     GetWorkflowWorkflowPreparationJobsConnectorDeepgram,
     GetWorkflowWorkflowPreparationJobsConnectorDocument,
     GetWorkflowWorkflowPreparationJobsConnectorEmail,
     GetWorkflowWorkflowPreparationSummarizations,
     GetWorkflowWorkflowPreparationSummarizationsSpecification,
 )
-from .ingest_encoded_file import IngestEncodedFile, IngestEncodedFileIngestEncodedFile
-from .ingest_text import IngestText, IngestTextIngestText
-from .ingest_uri import IngestUri, IngestUriIngestUri
+from .ingest_encoded_file import (
+    IngestEncodedFile,
+    IngestEncodedFileIngestEncodedFile,
+    IngestEncodedFileIngestEncodedFileCollections,
+)
+from .ingest_text import (
+    IngestText,
+    IngestTextIngestText,
+    IngestTextIngestTextCollections,
+)
+from .ingest_uri import IngestUri, IngestUriIngestUri, IngestUriIngestUriCollections
 from .input_types import (
     AddressFilter,
     AddressInput,
     AlertFilter,
     AlertInput,
     AlertSchedulePolicyInput,
     AlertUpdateInput,
     AmazonFeedPropertiesInput,
     AmazonFeedPropertiesUpdateInput,
     AnthropicModelPropertiesInput,
     AnthropicModelPropertiesUpdateInput,
     AtlassianJiraFeedPropertiesInput,
     AtlassianJiraFeedPropertiesUpdateInput,
+    AudioMetadataInput,
     AzureBlobFeedPropertiesInput,
     AzureBlobFeedPropertiesUpdateInput,
     AzureDocumentPreparationPropertiesInput,
     AzureFileFeedPropertiesInput,
     AzureFileFeedPropertiesUpdateInput,
     AzureImageExtractionPropertiesInput,
     AzureOpenAIModelPropertiesInput,
@@ -442,32 +490,36 @@
     CohereModelPropertiesUpdateInput,
     CollectionFilter,
     CollectionInput,
     CollectionUpdateInput,
     ContentCriteriaInput,
     ContentFacetInput,
     ContentFilter,
+    ContentGraphInput,
     ContentInput,
     ContentPublishingConnectorInput,
     ContentPublishingConnectorUpdateInput,
     ContentUpdateInput,
     ConversationFilter,
     ConversationInput,
     ConversationStrategyInput,
     ConversationStrategyUpdateInput,
     ConversationUpdateInput,
     DateRangeFilter,
     DateRangeInput,
     DeepgramAudioPreparationPropertiesInput,
     DiscordFeedPropertiesInput,
     DiscordFeedPropertiesUpdateInput,
+    DocumentMetadataInput,
     DocumentPreparationPropertiesInput,
+    DrawingMetadataInput,
     ElevenLabsPublishingPropertiesInput,
     EmailFeedPropertiesInput,
     EmailFeedPropertiesUpdateInput,
+    EmailMetadataInput,
     EmailPreparationPropertiesInput,
     EnrichmentWorkflowJobInput,
     EnrichmentWorkflowStageInput,
     EntityEnrichmentConnectorInput,
     EntityExtractionConnectorInput,
     EntityReferenceFilter,
     EntityReferenceInput,
@@ -478,45 +530,50 @@
     ExtractionWorkflowJobInput,
     ExtractionWorkflowStageInput,
     FeedFilter,
     FeedInput,
     FeedSchedulePolicyInput,
     FeedUpdateInput,
     FilePreparationConnectorInput,
+    GeometryMetadataInput,
     GitHubIssuesFeedPropertiesInput,
     GitHubIssuesFeedPropertiesUpdateInput,
     GoogleDriveFeedPropertiesInput,
     GoogleDriveFeedPropertiesUpdateInput,
     GoogleEmailFeedPropertiesInput,
     GoogleEmailFeedPropertiesUpdateInput,
     GoogleFeedPropertiesInput,
     GoogleFeedPropertiesUpdateInput,
     GroqModelPropertiesInput,
     GroqModelPropertiesUpdateInput,
     H3Filter,
     H3IndexFilter,
+    ImageMetadataInput,
     IngestionContentFilterInput,
     IngestionWorkflowStageInput,
     Int64RangeFilter,
     IntegrationConnectorInput,
     IntegrationConnectorUpdateInput,
     IssueFeedPropertiesInput,
     IssueFeedPropertiesUpdateInput,
+    IssueMetadataInput,
     LabelFacetInput,
     LabelFilter,
     LabelInput,
     LabelUpdateInput,
     LinearFeedPropertiesInput,
     LinearFeedPropertiesUpdateInput,
     LinkStrategyInput,
     MetadataFilter,
     MetadataInput,
     MetadataUpdateInput,
     MicrosoftEmailFeedPropertiesInput,
     MicrosoftEmailFeedPropertiesUpdateInput,
+    MicrosoftTeamsFeedPropertiesInput,
+    MicrosoftTeamsFeedPropertiesUpdateInput,
     MistralModelPropertiesInput,
     MistralModelPropertiesUpdateInput,
     ModelTextExtractionPropertiesInput,
     NamedEntityReferenceInput,
     NotionFeedPropertiesInput,
     NotionFeedPropertiesUpdateInput,
     ObservationCriteriaInput,
@@ -529,22 +586,24 @@
     OpenAIImageExtractionPropertiesInput,
     OpenAIModelPropertiesInput,
     OpenAIModelPropertiesUpdateInput,
     OrganizationFacetInput,
     OrganizationFilter,
     OrganizationInput,
     OrganizationUpdateInput,
+    PackageMetadataInput,
     PersonFacetInput,
     PersonFilter,
     PersonInput,
     PersonUpdateInput,
     PlaceFacetInput,
     PlaceFilter,
     PlaceInput,
     PlaceUpdateInput,
+    PointCloudMetadataInput,
     PointFilter,
     PointInput,
     PreparationWorkflowJobInput,
     PreparationWorkflowStageInput,
     ProductFacetInput,
     ProductFilter,
     ProductInput,
@@ -565,14 +624,15 @@
     RepoUpdateInput,
     RerankingStrategyInput,
     RerankingStrategyUpdateInput,
     RetrievalStrategyInput,
     RetrievalStrategyUpdateInput,
     RSSFeedPropertiesInput,
     RSSFeedPropertiesUpdateInput,
+    ShapeMetadataInput,
     SharePointFeedPropertiesInput,
     SharePointFeedPropertiesUpdateInput,
     SharePointLibrariesInput,
     SiteFeedPropertiesInput,
     SiteFeedPropertiesUpdateInput,
     SlackFeedPropertiesInput,
     SlackFeedPropertiesUpdateInput,
@@ -583,14 +643,15 @@
     SoftwareUpdateInput,
     SpecificationFilter,
     SpecificationInput,
     SpecificationUpdateInput,
     SummarizationStrategyInput,
     ToolDefinitionInput,
     ToolDefinitionUpdateInput,
+    VideoMetadataInput,
     WebFeedPropertiesInput,
     WebFeedPropertiesUpdateInput,
     WorkflowActionInput,
     WorkflowFilter,
     WorkflowInput,
     WorkflowUpdateInput,
     YouTubeFeedPropertiesInput,
@@ -600,14 +661,30 @@
 from .is_feed_done import IsFeedDone, IsFeedDoneIsFeedDone
 from .lookup_credits import LookupCredits, LookupCreditsLookupCredits
 from .lookup_usage import LookupUsage, LookupUsageLookupUsage
 from .operations import (
     ADD_CONTENTS_TO_COLLECTIONS_GQL,
     CLEAR_CONVERSATION_GQL,
     CLOSE_CONVERSATION_GQL,
+    COUNT_ALERTS_GQL,
+    COUNT_CATEGORIES_GQL,
+    COUNT_COLLECTIONS_GQL,
+    COUNT_CONTENTS_GQL,
+    COUNT_CONVERSATIONS_GQL,
+    COUNT_EVENTS_GQL,
+    COUNT_FEEDS_GQL,
+    COUNT_LABELS_GQL,
+    COUNT_ORGANIZATIONS_GQL,
+    COUNT_PERSONS_GQL,
+    COUNT_PLACES_GQL,
+    COUNT_PRODUCTS_GQL,
+    COUNT_REPOS_GQL,
+    COUNT_SOFTWARES_GQL,
+    COUNT_SPECIFICATIONS_GQL,
+    COUNT_WORKFLOWS_GQL,
     CREATE_ALERT_GQL,
     CREATE_CATEGORY_GQL,
     CREATE_COLLECTION_GQL,
     CREATE_CONVERSATION_GQL,
     CREATE_EVENT_GQL,
     CREATE_FEED_GQL,
     CREATE_LABEL_GQL,
@@ -616,15 +693,14 @@
     CREATE_PERSON_GQL,
     CREATE_PLACE_GQL,
     CREATE_PRODUCT_GQL,
     CREATE_REPO_GQL,
     CREATE_SOFTWARE_GQL,
     CREATE_SPECIFICATION_GQL,
     CREATE_WORKFLOW_GQL,
-    CREDITS_GQL,
     DELETE_ALERT_GQL,
     DELETE_ALERTS_GQL,
     DELETE_ALL_ALERTS_GQL,
     DELETE_ALL_CATEGORIES_GQL,
     DELETE_ALL_COLLECTIONS_GQL,
     DELETE_ALL_CONTENTS_GQL,
     DELETE_ALL_CONVERSATIONS_GQL,
@@ -633,14 +709,15 @@
     DELETE_ALL_LABELS_GQL,
     DELETE_ALL_ORGANIZATIONS_GQL,
     DELETE_ALL_PERSONS_GQL,
     DELETE_ALL_PLACES_GQL,
     DELETE_ALL_PRODUCTS_GQL,
     DELETE_ALL_REPOS_GQL,
     DELETE_ALL_SOFTWARES_GQL,
+    DELETE_ALL_SPECIFICATIONS_GQL,
     DELETE_ALL_WORKFLOWS_GQL,
     DELETE_CATEGORIES_GQL,
     DELETE_CATEGORY_GQL,
     DELETE_COLLECTION_GQL,
     DELETE_COLLECTIONS_GQL,
     DELETE_CONTENT_GQL,
     DELETE_CONTENTS_GQL,
@@ -662,14 +739,15 @@
     DELETE_PRODUCT_GQL,
     DELETE_PRODUCTS_GQL,
     DELETE_REPO_GQL,
     DELETE_REPOS_GQL,
     DELETE_SOFTWARE_GQL,
     DELETE_SOFTWARES_GQL,
     DELETE_SPECIFICATION_GQL,
+    DELETE_SPECIFICATIONS_GQL,
     DELETE_WORKFLOW_GQL,
     DELETE_WORKFLOWS_GQL,
     DISABLE_ALERT_GQL,
     DISABLE_FEED_GQL,
     ENABLE_ALERT_GQL,
     ENABLE_FEED_GQL,
     EXTRACT_CONTENTS_GQL,
@@ -701,27 +779,30 @@
     PROMPT_SPECIFICATIONS_GQL,
     PUBLISH_CONTENTS_GQL,
     PUBLISH_CONVERSATION_GQL,
     PUBLISH_TEXT_GQL,
     QUERY_ALERTS_GQL,
     QUERY_CATEGORIES_GQL,
     QUERY_COLLECTIONS_GQL,
-    QUERY_CONTENT_FACETS_GQL,
+    QUERY_CONTENTS_FACETS_GQL,
     QUERY_CONTENTS_GQL,
+    QUERY_CONTENTS_GRAPH_GQL,
     QUERY_CONVERSATIONS_GQL,
+    QUERY_CREDITS_GQL,
     QUERY_EVENTS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_LABELS_GQL,
     QUERY_ORGANIZATIONS_GQL,
     QUERY_PERSONS_GQL,
     QUERY_PLACES_GQL,
     QUERY_PRODUCTS_GQL,
     QUERY_REPOS_GQL,
     QUERY_SOFTWARES_GQL,
     QUERY_SPECIFICATIONS_GQL,
+    QUERY_USAGE_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
     SUGGEST_CONVERSATION_GQL,
     SUMMARIZE_CONTENTS_GQL,
     UPDATE_ALERT_GQL,
     UPDATE_CATEGORY_GQL,
     UPDATE_COLLECTION_GQL,
@@ -736,15 +817,14 @@
     UPDATE_PLACE_GQL,
     UPDATE_PRODUCT_GQL,
     UPDATE_PROJECT_GQL,
     UPDATE_REPO_GQL,
     UPDATE_SOFTWARE_GQL,
     UPDATE_SPECIFICATION_GQL,
     UPDATE_WORKFLOW_GQL,
-    USAGE_GQL,
 )
 from .prompt_conversation import (
     PromptConversation,
     PromptConversationPromptConversation,
     PromptConversationPromptConversationConversation,
     PromptConversationPromptConversationFacets,
     PromptConversationPromptConversationFacetsObservable,
@@ -758,20 +838,29 @@
     PromptSpecifications,
     PromptSpecificationsPromptSpecifications,
     PromptSpecificationsPromptSpecificationsMessages,
     PromptSpecificationsPromptSpecificationsMessagesCitations,
     PromptSpecificationsPromptSpecificationsMessagesCitationsContent,
     PromptSpecificationsPromptSpecificationsSpecification,
 )
-from .publish_contents import PublishContents, PublishContentsPublishContents
+from .publish_contents import (
+    PublishContents,
+    PublishContentsPublishContents,
+    PublishContentsPublishContentsCollections,
+)
 from .publish_conversation import (
     PublishConversation,
     PublishConversationPublishConversation,
+    PublishConversationPublishConversationCollections,
+)
+from .publish_text import (
+    PublishText,
+    PublishTextPublishText,
+    PublishTextPublishTextCollections,
 )
-from .publish_text import PublishText, PublishTextPublishText
 from .query_alerts import (
     QueryAlerts,
     QueryAlertsAlerts,
     QueryAlertsAlertsResults,
     QueryAlertsAlertsResultsFilter,
     QueryAlertsAlertsResultsFilterCollections,
     QueryAlertsAlertsResultsFilterContents,
@@ -797,50 +886,89 @@
 from .query_collections import (
     QueryCollections,
     QueryCollectionsCollections,
     QueryCollectionsCollectionsResults,
     QueryCollectionsCollectionsResultsContents,
     QueryCollectionsCollectionsResultsOwner,
 )
-from .query_content_facets import (
-    QueryContentFacets,
-    QueryContentFacetsContents,
-    QueryContentFacetsContentsFacets,
-    QueryContentFacetsContentsFacetsObservable,
-    QueryContentFacetsContentsFacetsObservableObservable,
-)
 from .query_contents import (
     QueryContents,
     QueryContentsContents,
     QueryContentsContentsResults,
+    QueryContentsContentsResultsAddress,
     QueryContentsContentsResultsAudio,
     QueryContentsContentsResultsChildren,
     QueryContentsContentsResultsCollections,
     QueryContentsContentsResultsDocument,
     QueryContentsContentsResultsEmail,
     QueryContentsContentsResultsEmailBcc,
     QueryContentsContentsResultsEmailCc,
     QueryContentsContentsResultsEmailFrom,
     QueryContentsContentsResultsEmailTo,
     QueryContentsContentsResultsFeed,
     QueryContentsContentsResultsImage,
     QueryContentsContentsResultsIssue,
     QueryContentsContentsResultsLinks,
+    QueryContentsContentsResultsLocation,
     QueryContentsContentsResultsObservations,
     QueryContentsContentsResultsObservationsObservable,
     QueryContentsContentsResultsObservationsOccurrences,
     QueryContentsContentsResultsObservationsOccurrencesBoundingBox,
     QueryContentsContentsResultsOwner,
+    QueryContentsContentsResultsPackage,
     QueryContentsContentsResultsPages,
     QueryContentsContentsResultsPagesChunks,
     QueryContentsContentsResultsParent,
     QueryContentsContentsResultsSegments,
     QueryContentsContentsResultsVideo,
     QueryContentsContentsResultsWorkflow,
 )
+from .query_contents_facets import (
+    QueryContentsFacets,
+    QueryContentsFacetsContents,
+    QueryContentsFacetsContentsFacets,
+    QueryContentsFacetsContentsFacetsObservable,
+    QueryContentsFacetsContentsFacetsObservableObservable,
+    QueryContentsFacetsContentsFacetsRange,
+    QueryContentsFacetsContentsResults,
+    QueryContentsFacetsContentsResultsAddress,
+    QueryContentsFacetsContentsResultsAudio,
+    QueryContentsFacetsContentsResultsChildren,
+    QueryContentsFacetsContentsResultsCollections,
+    QueryContentsFacetsContentsResultsDocument,
+    QueryContentsFacetsContentsResultsEmail,
+    QueryContentsFacetsContentsResultsEmailBcc,
+    QueryContentsFacetsContentsResultsEmailCc,
+    QueryContentsFacetsContentsResultsEmailFrom,
+    QueryContentsFacetsContentsResultsEmailTo,
+    QueryContentsFacetsContentsResultsFeed,
+    QueryContentsFacetsContentsResultsImage,
+    QueryContentsFacetsContentsResultsIssue,
+    QueryContentsFacetsContentsResultsLinks,
+    QueryContentsFacetsContentsResultsLocation,
+    QueryContentsFacetsContentsResultsObservations,
+    QueryContentsFacetsContentsResultsObservationsObservable,
+    QueryContentsFacetsContentsResultsObservationsOccurrences,
+    QueryContentsFacetsContentsResultsObservationsOccurrencesBoundingBox,
+    QueryContentsFacetsContentsResultsOwner,
+    QueryContentsFacetsContentsResultsPackage,
+    QueryContentsFacetsContentsResultsPages,
+    QueryContentsFacetsContentsResultsPagesChunks,
+    QueryContentsFacetsContentsResultsParent,
+    QueryContentsFacetsContentsResultsSegments,
+    QueryContentsFacetsContentsResultsVideo,
+    QueryContentsFacetsContentsResultsWorkflow,
+)
+from .query_contents_graph import (
+    QueryContentsGraph,
+    QueryContentsGraphContents,
+    QueryContentsGraphContentsGraph,
+    QueryContentsGraphContentsGraphEdges,
+    QueryContentsGraphContentsGraphNodes,
+)
 from .query_conversations import (
     QueryConversations,
     QueryConversationsConversations,
     QueryConversationsConversationsResults,
     QueryConversationsConversationsResultsFilter,
     QueryConversationsConversationsResultsFilterCollections,
     QueryConversationsConversationsResultsFilterContents,
@@ -852,14 +980,15 @@
     QueryConversationsConversationsResultsFilterWorkflows,
     QueryConversationsConversationsResultsMessages,
     QueryConversationsConversationsResultsMessagesCitations,
     QueryConversationsConversationsResultsMessagesCitationsContent,
     QueryConversationsConversationsResultsOwner,
     QueryConversationsConversationsResultsSpecification,
 )
+from .query_credits import QueryCredits, QueryCreditsCredits
 from .query_events import (
     QueryEvents,
     QueryEventsEvents,
     QueryEventsEventsResults,
     QueryEventsEventsResultsAddress,
 )
 from .query_feeds import (
@@ -925,23 +1054,25 @@
 )
 from .query_specifications import (
     QuerySpecifications,
     QuerySpecificationsSpecifications,
     QuerySpecificationsSpecificationsResults,
     QuerySpecificationsSpecificationsResultsAnthropic,
     QuerySpecificationsSpecificationsResultsAzureOpenAi,
+    QuerySpecificationsSpecificationsResultsCohere,
     QuerySpecificationsSpecificationsResultsOpenAi,
     QuerySpecificationsSpecificationsResultsOwner,
     QuerySpecificationsSpecificationsResultsPromptStrategy,
     QuerySpecificationsSpecificationsResultsReplicate,
     QuerySpecificationsSpecificationsResultsRerankingStrategy,
     QuerySpecificationsSpecificationsResultsRetrievalStrategy,
     QuerySpecificationsSpecificationsResultsStrategy,
     QuerySpecificationsSpecificationsResultsTools,
 )
+from .query_usage import QueryUsage, QueryUsageUsage
 from .query_workflows import (
     QueryWorkflows,
     QueryWorkflowsWorkflows,
     QueryWorkflowsWorkflowsResults,
     QueryWorkflowsWorkflowsResultsActions,
     QueryWorkflowsWorkflowsResultsActionsConnector,
     QueryWorkflowsWorkflowsResultsActionsConnectorSlack,
@@ -986,15 +1117,19 @@
     SummarizeContentsSummarizeContentsContent,
     SummarizeContentsSummarizeContentsItems,
     SummarizeContentsSummarizeContentsSpecification,
 )
 from .update_alert import UpdateAlert, UpdateAlertUpdateAlert
 from .update_category import UpdateCategory, UpdateCategoryUpdateCategory
 from .update_collection import UpdateCollection, UpdateCollectionUpdateCollection
-from .update_content import UpdateContent, UpdateContentUpdateContent
+from .update_content import (
+    UpdateContent,
+    UpdateContentUpdateContent,
+    UpdateContentUpdateContentCollections,
+)
 from .update_conversation import (
     UpdateConversation,
     UpdateConversationUpdateConversation,
 )
 from .update_event import UpdateEvent, UpdateEventUpdateEvent
 from .update_feed import UpdateFeed, UpdateFeedUpdateFeed
 from .update_label import UpdateLabel, UpdateLabelUpdateLabel
@@ -1040,15 +1175,14 @@
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorAzureDocument,
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDeepgram,
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDocument,
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorEmail,
     UpdateWorkflowUpdateWorkflowPreparationSummarizations,
     UpdateWorkflowUpdateWorkflowPreparationSummarizationsSpecification,
 )
-from .usage import Usage, UsageUsage
 
 __all__ = [
     "ADD_CONTENTS_TO_COLLECTIONS_GQL",
     "AddContentsToCollections",
     "AddContentsToCollectionsAddContentsToCollections",
     "AddContentsToCollectionsAddContentsToCollectionsContents",
     "AddressFilter",
@@ -1063,14 +1197,15 @@
     "AnthropicModelPropertiesInput",
     "AnthropicModelPropertiesUpdateInput",
     "AnthropicModels",
     "ApplyPolicy",
     "AsyncBaseClient",
     "AtlassianJiraFeedPropertiesInput",
     "AtlassianJiraFeedPropertiesUpdateInput",
+    "AudioMetadataInput",
     "AzureBlobFeedPropertiesInput",
     "AzureBlobFeedPropertiesUpdateInput",
     "AzureDocumentIntelligenceModels",
     "AzureDocumentPreparationPropertiesInput",
     "AzureFileFeedPropertiesInput",
     "AzureFileFeedPropertiesUpdateInput",
     "AzureImageExtractionPropertiesInput",
@@ -1079,14 +1214,30 @@
     "AzureOpenAIModels",
     "AzureTextExtractionPropertiesInput",
     "BaseModel",
     "BillableMetrics",
     "BoundingBoxInput",
     "CLEAR_CONVERSATION_GQL",
     "CLOSE_CONVERSATION_GQL",
+    "COUNT_ALERTS_GQL",
+    "COUNT_CATEGORIES_GQL",
+    "COUNT_COLLECTIONS_GQL",
+    "COUNT_CONTENTS_GQL",
+    "COUNT_CONVERSATIONS_GQL",
+    "COUNT_EVENTS_GQL",
+    "COUNT_FEEDS_GQL",
+    "COUNT_LABELS_GQL",
+    "COUNT_ORGANIZATIONS_GQL",
+    "COUNT_PERSONS_GQL",
+    "COUNT_PLACES_GQL",
+    "COUNT_PRODUCTS_GQL",
+    "COUNT_REPOS_GQL",
+    "COUNT_SOFTWARES_GQL",
+    "COUNT_SPECIFICATIONS_GQL",
+    "COUNT_WORKFLOWS_GQL",
     "CREATE_ALERT_GQL",
     "CREATE_CATEGORY_GQL",
     "CREATE_COLLECTION_GQL",
     "CREATE_CONVERSATION_GQL",
     "CREATE_EVENT_GQL",
     "CREATE_FEED_GQL",
     "CREATE_LABEL_GQL",
@@ -1095,15 +1246,14 @@
     "CREATE_PERSON_GQL",
     "CREATE_PLACE_GQL",
     "CREATE_PRODUCT_GQL",
     "CREATE_REPO_GQL",
     "CREATE_SOFTWARE_GQL",
     "CREATE_SPECIFICATION_GQL",
     "CREATE_WORKFLOW_GQL",
-    "CREDITS_GQL",
     "CategoryFacetInput",
     "CategoryFacetTypes",
     "CategoryFilter",
     "CategoryInput",
     "CategoryUpdateInput",
     "ClearConversation",
     "ClearConversationClearConversation",
@@ -1117,14 +1267,15 @@
     "CollectionInput",
     "CollectionTypes",
     "CollectionUpdateInput",
     "ContentCriteriaInput",
     "ContentFacetInput",
     "ContentFacetTypes",
     "ContentFilter",
+    "ContentGraphInput",
     "ContentInput",
     "ContentPublishingConnectorInput",
     "ContentPublishingConnectorUpdateInput",
     "ContentPublishingFormats",
     "ContentPublishingServiceTypes",
     "ContentTypes",
     "ContentUpdateInput",
@@ -1133,14 +1284,46 @@
     "ConversationRoleTypes",
     "ConversationSearchTypes",
     "ConversationStrategyInput",
     "ConversationStrategyTypes",
     "ConversationStrategyUpdateInput",
     "ConversationTypes",
     "ConversationUpdateInput",
+    "CountAlerts",
+    "CountAlertsCountAlerts",
+    "CountCategories",
+    "CountCategoriesCountCategories",
+    "CountCollections",
+    "CountCollectionsCountCollections",
+    "CountContents",
+    "CountContentsCountContents",
+    "CountConversations",
+    "CountConversationsCountConversations",
+    "CountEvents",
+    "CountEventsCountEvents",
+    "CountFeeds",
+    "CountFeedsCountFeeds",
+    "CountLabels",
+    "CountLabelsCountLabels",
+    "CountOrganizations",
+    "CountOrganizationsCountOrganizations",
+    "CountPersons",
+    "CountPersonsCountPersons",
+    "CountPlaces",
+    "CountPlacesCountPlaces",
+    "CountProducts",
+    "CountProductsCountProducts",
+    "CountRepos",
+    "CountReposCountRepos",
+    "CountSoftwares",
+    "CountSoftwaresCountSoftwares",
+    "CountSpecifications",
+    "CountSpecificationsCountSpecifications",
+    "CountWorkflows",
+    "CountWorkflowsCountWorkflows",
     "CreateAlert",
     "CreateAlertCreateAlert",
     "CreateCategory",
     "CreateCategoryCreateCategory",
     "CreateCollection",
     "CreateCollectionCreateCollection",
     "CreateConversation",
@@ -1192,16 +1375,14 @@
     "CreateWorkflowCreateWorkflowPreparationJobsConnector",
     "CreateWorkflowCreateWorkflowPreparationJobsConnectorAzureDocument",
     "CreateWorkflowCreateWorkflowPreparationJobsConnectorDeepgram",
     "CreateWorkflowCreateWorkflowPreparationJobsConnectorDocument",
     "CreateWorkflowCreateWorkflowPreparationJobsConnectorEmail",
     "CreateWorkflowCreateWorkflowPreparationSummarizations",
     "CreateWorkflowCreateWorkflowPreparationSummarizationsSpecification",
-    "Credits",
-    "CreditsCredits",
     "DELETE_ALERTS_GQL",
     "DELETE_ALERT_GQL",
     "DELETE_ALL_ALERTS_GQL",
     "DELETE_ALL_CATEGORIES_GQL",
     "DELETE_ALL_COLLECTIONS_GQL",
     "DELETE_ALL_CONTENTS_GQL",
     "DELETE_ALL_CONVERSATIONS_GQL",
@@ -1210,14 +1391,15 @@
     "DELETE_ALL_LABELS_GQL",
     "DELETE_ALL_ORGANIZATIONS_GQL",
     "DELETE_ALL_PERSONS_GQL",
     "DELETE_ALL_PLACES_GQL",
     "DELETE_ALL_PRODUCTS_GQL",
     "DELETE_ALL_REPOS_GQL",
     "DELETE_ALL_SOFTWARES_GQL",
+    "DELETE_ALL_SPECIFICATIONS_GQL",
     "DELETE_ALL_WORKFLOWS_GQL",
     "DELETE_CATEGORIES_GQL",
     "DELETE_CATEGORY_GQL",
     "DELETE_COLLECTIONS_GQL",
     "DELETE_COLLECTION_GQL",
     "DELETE_CONTENTS_GQL",
     "DELETE_CONTENT_GQL",
@@ -1238,14 +1420,15 @@
     "DELETE_PLACE_GQL",
     "DELETE_PRODUCTS_GQL",
     "DELETE_PRODUCT_GQL",
     "DELETE_REPOS_GQL",
     "DELETE_REPO_GQL",
     "DELETE_SOFTWARES_GQL",
     "DELETE_SOFTWARE_GQL",
+    "DELETE_SPECIFICATIONS_GQL",
     "DELETE_SPECIFICATION_GQL",
     "DELETE_WORKFLOWS_GQL",
     "DELETE_WORKFLOW_GQL",
     "DISABLE_ALERT_GQL",
     "DISABLE_FEED_GQL",
     "DateRangeFilter",
     "DateRangeInput",
@@ -1279,14 +1462,16 @@
     "DeleteAllPlacesDeleteAllPlaces",
     "DeleteAllProducts",
     "DeleteAllProductsDeleteAllProducts",
     "DeleteAllRepos",
     "DeleteAllReposDeleteAllRepos",
     "DeleteAllSoftwares",
     "DeleteAllSoftwaresDeleteAllSoftwares",
+    "DeleteAllSpecifications",
+    "DeleteAllSpecificationsDeleteAllSpecifications",
     "DeleteAllWorkflows",
     "DeleteAllWorkflowsDeleteAllWorkflows",
     "DeleteCategories",
     "DeleteCategoriesDeleteCategories",
     "DeleteCategory",
     "DeleteCategoryDeleteCategory",
     "DeleteCollection",
@@ -1337,34 +1522,39 @@
     "DeleteReposDeleteRepos",
     "DeleteSoftware",
     "DeleteSoftwareDeleteSoftware",
     "DeleteSoftwares",
     "DeleteSoftwaresDeleteSoftwares",
     "DeleteSpecification",
     "DeleteSpecificationDeleteSpecification",
+    "DeleteSpecifications",
+    "DeleteSpecificationsDeleteSpecifications",
     "DeleteWorkflow",
     "DeleteWorkflowDeleteWorkflow",
     "DeleteWorkflows",
     "DeleteWorkflowsDeleteWorkflows",
     "DeviceTypes",
     "DisableAlert",
     "DisableAlertDisableAlert",
     "DisableFeed",
     "DisableFeedDisableFeed",
     "DiscordFeedPropertiesInput",
     "DiscordFeedPropertiesUpdateInput",
+    "DocumentMetadataInput",
     "DocumentPreparationPropertiesInput",
+    "DrawingMetadataInput",
     "ENABLE_ALERT_GQL",
     "ENABLE_FEED_GQL",
     "EXTRACT_CONTENTS_GQL",
     "ElevenLabsModels",
     "ElevenLabsPublishingPropertiesInput",
     "EmailFeedPropertiesInput",
     "EmailFeedPropertiesUpdateInput",
     "EmailListingTypes",
+    "EmailMetadataInput",
     "EmailPreparationPropertiesInput",
     "EnableAlert",
     "EnableAlertEnableAlert",
     "EnableFeed",
     "EnableFeedEnableFeed",
     "EnrichmentWorkflowJobInput",
     "EnrichmentWorkflowStageInput",
@@ -1413,14 +1603,15 @@
     "GET_PLACE_GQL",
     "GET_PRODUCT_GQL",
     "GET_PROJECT_GQL",
     "GET_REPO_GQL",
     "GET_SOFTWARE_GQL",
     "GET_SPECIFICATION_GQL",
     "GET_WORKFLOW_GQL",
+    "GeometryMetadataInput",
     "GetAlert",
     "GetAlertAlert",
     "GetAlertAlertFilter",
     "GetAlertAlertFilterCollections",
     "GetAlertAlertFilterContents",
     "GetAlertAlertFilterCreationDateRange",
     "GetAlertAlertFilterDateRange",
@@ -1439,33 +1630,39 @@
     "GetCategoryCategory",
     "GetCollection",
     "GetCollectionCollection",
     "GetCollectionCollectionContents",
     "GetCollectionCollectionOwner",
     "GetContent",
     "GetContentContent",
+    "GetContentContentAddress",
     "GetContentContentAudio",
     "GetContentContentChildren",
     "GetContentContentCollections",
     "GetContentContentDocument",
     "GetContentContentEmail",
     "GetContentContentEmailBcc",
     "GetContentContentEmailCc",
     "GetContentContentEmailFrom",
     "GetContentContentEmailTo",
     "GetContentContentFeed",
     "GetContentContentImage",
     "GetContentContentIssue",
     "GetContentContentLinks",
+    "GetContentContentLocation",
     "GetContentContentObservations",
     "GetContentContentObservationsObservable",
     "GetContentContentObservationsOccurrences",
     "GetContentContentObservationsOccurrencesBoundingBox",
     "GetContentContentOwner",
+    "GetContentContentPackage",
+    "GetContentContentPages",
+    "GetContentContentPagesChunks",
     "GetContentContentParent",
+    "GetContentContentSegments",
     "GetContentContentVideo",
     "GetContentContentWorkflow",
     "GetConversation",
     "GetConversationConversation",
     "GetConversationConversationFilter",
     "GetConversationConversationFilterCollections",
     "GetConversationConversationFilterContents",
@@ -1533,14 +1730,15 @@
     "GetRepoRepo",
     "GetSoftware",
     "GetSoftwareSoftware",
     "GetSpecification",
     "GetSpecificationSpecification",
     "GetSpecificationSpecificationAnthropic",
     "GetSpecificationSpecificationAzureOpenAi",
+    "GetSpecificationSpecificationCohere",
     "GetSpecificationSpecificationOpenAi",
     "GetSpecificationSpecificationOwner",
     "GetSpecificationSpecificationPromptStrategy",
     "GetSpecificationSpecificationReplicate",
     "GetSpecificationSpecificationRerankingStrategy",
     "GetSpecificationSpecificationRetrievalStrategy",
     "GetSpecificationSpecificationStrategy",
@@ -1595,33 +1793,38 @@
     "H3IndexFilter",
     "H3ResolutionTypes",
     "INGEST_ENCODED_FILE_GQL",
     "INGEST_TEXT_GQL",
     "INGEST_URI_GQL",
     "IS_CONTENT_DONE_GQL",
     "IS_FEED_DONE_GQL",
+    "ImageMetadataInput",
     "ImageProjectionTypes",
     "IngestEncodedFile",
     "IngestEncodedFileIngestEncodedFile",
+    "IngestEncodedFileIngestEncodedFileCollections",
     "IngestText",
     "IngestTextIngestText",
+    "IngestTextIngestTextCollections",
     "IngestUri",
     "IngestUriIngestUri",
+    "IngestUriIngestUriCollections",
     "IngestionContentFilterInput",
     "IngestionWorkflowStageInput",
     "Int64RangeFilter",
     "IntegrationConnectorInput",
     "IntegrationConnectorUpdateInput",
     "IntegrationServiceTypes",
     "IsContentDone",
     "IsContentDoneIsContentDone",
     "IsFeedDone",
     "IsFeedDoneIsFeedDone",
     "IssueFeedPropertiesInput",
     "IssueFeedPropertiesUpdateInput",
+    "IssueMetadataInput",
     "LOOKUP_CREDITS_GQL",
     "LOOKUP_USAGE_GQL",
     "LabelFacetInput",
     "LabelFacetTypes",
     "LabelFilter",
     "LabelInput",
     "LabelUpdateInput",
@@ -1638,14 +1841,16 @@
     "MailSensitivity",
     "MetadataFilter",
     "MetadataInput",
     "MetadataTypes",
     "MetadataUpdateInput",
     "MicrosoftEmailFeedPropertiesInput",
     "MicrosoftEmailFeedPropertiesUpdateInput",
+    "MicrosoftTeamsFeedPropertiesInput",
+    "MicrosoftTeamsFeedPropertiesUpdateInput",
     "MistralModelPropertiesInput",
     "MistralModelPropertiesUpdateInput",
     "MistralModels",
     "ModelServiceTypes",
     "ModelTextExtractionPropertiesInput",
     "NamedEntityReferenceInput",
     "NotionFeedPropertiesInput",
@@ -1674,24 +1879,26 @@
     "OrganizationUpdateInput",
     "OrientationTypes",
     "PROMPT_CONVERSATION_GQL",
     "PROMPT_SPECIFICATIONS_GQL",
     "PUBLISH_CONTENTS_GQL",
     "PUBLISH_CONVERSATION_GQL",
     "PUBLISH_TEXT_GQL",
+    "PackageMetadataInput",
     "PersonFacetInput",
     "PersonFacetTypes",
     "PersonFilter",
     "PersonInput",
     "PersonUpdateInput",
     "PlaceFacetInput",
     "PlaceFacetTypes",
     "PlaceFilter",
     "PlaceInput",
     "PlaceUpdateInput",
+    "PointCloudMetadataInput",
     "PointFilter",
     "PointInput",
     "PolicyTimeTypes",
     "PreparationWorkflowJobInput",
     "PreparationWorkflowStageInput",
     "ProductFacetInput",
     "ProductFacetTypes",
@@ -1719,34 +1926,40 @@
     "PromptSpecificationsPromptSpecificationsMessagesCitationsContent",
     "PromptSpecificationsPromptSpecificationsSpecification",
     "PromptStrategyInput",
     "PromptStrategyTypes",
     "PromptStrategyUpdateInput",
     "PublishContents",
     "PublishContentsPublishContents",
+    "PublishContentsPublishContentsCollections",
     "PublishConversation",
     "PublishConversationPublishConversation",
+    "PublishConversationPublishConversationCollections",
     "PublishText",
     "PublishTextPublishText",
+    "PublishTextPublishTextCollections",
     "QUERY_ALERTS_GQL",
     "QUERY_CATEGORIES_GQL",
     "QUERY_COLLECTIONS_GQL",
+    "QUERY_CONTENTS_FACETS_GQL",
     "QUERY_CONTENTS_GQL",
-    "QUERY_CONTENT_FACETS_GQL",
+    "QUERY_CONTENTS_GRAPH_GQL",
     "QUERY_CONVERSATIONS_GQL",
+    "QUERY_CREDITS_GQL",
     "QUERY_EVENTS_GQL",
     "QUERY_FEEDS_GQL",
     "QUERY_LABELS_GQL",
     "QUERY_ORGANIZATIONS_GQL",
     "QUERY_PERSONS_GQL",
     "QUERY_PLACES_GQL",
     "QUERY_PRODUCTS_GQL",
     "QUERY_REPOS_GQL",
     "QUERY_SOFTWARES_GQL",
     "QUERY_SPECIFICATIONS_GQL",
+    "QUERY_USAGE_GQL",
     "QUERY_WORKFLOWS_GQL",
     "QueryAlerts",
     "QueryAlertsAlerts",
     "QueryAlertsAlertsResults",
     "QueryAlertsAlertsResultsFilter",
     "QueryAlertsAlertsResultsFilterCollections",
     "QueryAlertsAlertsResultsFilterContents",
@@ -1767,46 +1980,83 @@
     "QueryCategoriesCategories",
     "QueryCategoriesCategoriesResults",
     "QueryCollections",
     "QueryCollectionsCollections",
     "QueryCollectionsCollectionsResults",
     "QueryCollectionsCollectionsResultsContents",
     "QueryCollectionsCollectionsResultsOwner",
-    "QueryContentFacets",
-    "QueryContentFacetsContents",
-    "QueryContentFacetsContentsFacets",
-    "QueryContentFacetsContentsFacetsObservable",
-    "QueryContentFacetsContentsFacetsObservableObservable",
     "QueryContents",
     "QueryContentsContents",
     "QueryContentsContentsResults",
+    "QueryContentsContentsResultsAddress",
     "QueryContentsContentsResultsAudio",
     "QueryContentsContentsResultsChildren",
     "QueryContentsContentsResultsCollections",
     "QueryContentsContentsResultsDocument",
     "QueryContentsContentsResultsEmail",
     "QueryContentsContentsResultsEmailBcc",
     "QueryContentsContentsResultsEmailCc",
     "QueryContentsContentsResultsEmailFrom",
     "QueryContentsContentsResultsEmailTo",
     "QueryContentsContentsResultsFeed",
     "QueryContentsContentsResultsImage",
     "QueryContentsContentsResultsIssue",
     "QueryContentsContentsResultsLinks",
+    "QueryContentsContentsResultsLocation",
     "QueryContentsContentsResultsObservations",
     "QueryContentsContentsResultsObservationsObservable",
     "QueryContentsContentsResultsObservationsOccurrences",
     "QueryContentsContentsResultsObservationsOccurrencesBoundingBox",
     "QueryContentsContentsResultsOwner",
+    "QueryContentsContentsResultsPackage",
     "QueryContentsContentsResultsPages",
     "QueryContentsContentsResultsPagesChunks",
     "QueryContentsContentsResultsParent",
     "QueryContentsContentsResultsSegments",
     "QueryContentsContentsResultsVideo",
     "QueryContentsContentsResultsWorkflow",
+    "QueryContentsFacets",
+    "QueryContentsFacetsContents",
+    "QueryContentsFacetsContentsFacets",
+    "QueryContentsFacetsContentsFacetsObservable",
+    "QueryContentsFacetsContentsFacetsObservableObservable",
+    "QueryContentsFacetsContentsFacetsRange",
+    "QueryContentsFacetsContentsResults",
+    "QueryContentsFacetsContentsResultsAddress",
+    "QueryContentsFacetsContentsResultsAudio",
+    "QueryContentsFacetsContentsResultsChildren",
+    "QueryContentsFacetsContentsResultsCollections",
+    "QueryContentsFacetsContentsResultsDocument",
+    "QueryContentsFacetsContentsResultsEmail",
+    "QueryContentsFacetsContentsResultsEmailBcc",
+    "QueryContentsFacetsContentsResultsEmailCc",
+    "QueryContentsFacetsContentsResultsEmailFrom",
+    "QueryContentsFacetsContentsResultsEmailTo",
+    "QueryContentsFacetsContentsResultsFeed",
+    "QueryContentsFacetsContentsResultsImage",
+    "QueryContentsFacetsContentsResultsIssue",
+    "QueryContentsFacetsContentsResultsLinks",
+    "QueryContentsFacetsContentsResultsLocation",
+    "QueryContentsFacetsContentsResultsObservations",
+    "QueryContentsFacetsContentsResultsObservationsObservable",
+    "QueryContentsFacetsContentsResultsObservationsOccurrences",
+    "QueryContentsFacetsContentsResultsObservationsOccurrencesBoundingBox",
+    "QueryContentsFacetsContentsResultsOwner",
+    "QueryContentsFacetsContentsResultsPackage",
+    "QueryContentsFacetsContentsResultsPages",
+    "QueryContentsFacetsContentsResultsPagesChunks",
+    "QueryContentsFacetsContentsResultsParent",
+    "QueryContentsFacetsContentsResultsSegments",
+    "QueryContentsFacetsContentsResultsVideo",
+    "QueryContentsFacetsContentsResultsWorkflow",
+    "QueryContentsGraph",
+    "QueryContentsGraphContents",
+    "QueryContentsGraphContentsGraph",
+    "QueryContentsGraphContentsGraphEdges",
+    "QueryContentsGraphContentsGraphNodes",
     "QueryConversations",
     "QueryConversationsConversations",
     "QueryConversationsConversationsResults",
     "QueryConversationsConversationsResultsFilter",
     "QueryConversationsConversationsResultsFilterCollections",
     "QueryConversationsConversationsResultsFilterContents",
     "QueryConversationsConversationsResultsFilterCreationDateRange",
@@ -1816,14 +2066,16 @@
     "QueryConversationsConversationsResultsFilterObservationsObservable",
     "QueryConversationsConversationsResultsFilterWorkflows",
     "QueryConversationsConversationsResultsMessages",
     "QueryConversationsConversationsResultsMessagesCitations",
     "QueryConversationsConversationsResultsMessagesCitationsContent",
     "QueryConversationsConversationsResultsOwner",
     "QueryConversationsConversationsResultsSpecification",
+    "QueryCredits",
+    "QueryCreditsCredits",
     "QueryEvents",
     "QueryEventsEvents",
     "QueryEventsEventsResults",
     "QueryEventsEventsResultsAddress",
     "QueryFeeds",
     "QueryFeedsFeeds",
     "QueryFeedsFeedsResults",
@@ -1878,22 +2130,25 @@
     "QuerySoftwaresSoftwares",
     "QuerySoftwaresSoftwaresResults",
     "QuerySpecifications",
     "QuerySpecificationsSpecifications",
     "QuerySpecificationsSpecificationsResults",
     "QuerySpecificationsSpecificationsResultsAnthropic",
     "QuerySpecificationsSpecificationsResultsAzureOpenAi",
+    "QuerySpecificationsSpecificationsResultsCohere",
     "QuerySpecificationsSpecificationsResultsOpenAi",
     "QuerySpecificationsSpecificationsResultsOwner",
     "QuerySpecificationsSpecificationsResultsPromptStrategy",
     "QuerySpecificationsSpecificationsResultsReplicate",
     "QuerySpecificationsSpecificationsResultsRerankingStrategy",
     "QuerySpecificationsSpecificationsResultsRetrievalStrategy",
     "QuerySpecificationsSpecificationsResultsStrategy",
     "QuerySpecificationsSpecificationsResultsTools",
+    "QueryUsage",
+    "QueryUsageUsage",
     "QueryWorkflows",
     "QueryWorkflowsWorkflows",
     "QueryWorkflowsWorkflowsResults",
     "QueryWorkflowsWorkflowsResultsActions",
     "QueryWorkflowsWorkflowsResultsActionsConnector",
     "QueryWorkflowsWorkflowsResultsActionsConnectorSlack",
     "QueryWorkflowsWorkflowsResultsEnrichment",
@@ -1945,14 +2200,15 @@
     "RetrievalStrategyInput",
     "RetrievalStrategyTypes",
     "RetrievalStrategyUpdateInput",
     "SUGGEST_CONVERSATION_GQL",
     "SUMMARIZE_CONTENTS_GQL",
     "SearchQueryTypes",
     "SearchTypes",
+    "ShapeMetadataInput",
     "SharePointAuthenticationTypes",
     "SharePointFeedPropertiesInput",
     "SharePointFeedPropertiesUpdateInput",
     "SharePointLibrariesInput",
     "SiteFeedPropertiesInput",
     "SiteFeedPropertiesUpdateInput",
     "SiteTypes",
@@ -1997,24 +2253,24 @@
     "UPDATE_PLACE_GQL",
     "UPDATE_PRODUCT_GQL",
     "UPDATE_PROJECT_GQL",
     "UPDATE_REPO_GQL",
     "UPDATE_SOFTWARE_GQL",
     "UPDATE_SPECIFICATION_GQL",
     "UPDATE_WORKFLOW_GQL",
-    "USAGE_GQL",
     "UnitTypes",
     "UpdateAlert",
     "UpdateAlertUpdateAlert",
     "UpdateCategory",
     "UpdateCategoryUpdateCategory",
     "UpdateCollection",
     "UpdateCollectionUpdateCollection",
     "UpdateContent",
     "UpdateContentUpdateContent",
+    "UpdateContentUpdateContentCollections",
     "UpdateConversation",
     "UpdateConversationUpdateConversation",
     "UpdateEvent",
     "UpdateEventUpdateEvent",
     "UpdateFeed",
     "UpdateFeedUpdateFeed",
     "UpdateLabel",
@@ -2063,16 +2319,15 @@
     "UpdateWorkflowUpdateWorkflowPreparationJobsConnectorAzureDocument",
     "UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDeepgram",
     "UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDocument",
     "UpdateWorkflowUpdateWorkflowPreparationJobsConnectorEmail",
     "UpdateWorkflowUpdateWorkflowPreparationSummarizations",
     "UpdateWorkflowUpdateWorkflowPreparationSummarizationsSpecification",
     "Upload",
-    "Usage",
-    "UsageUsage",
+    "VideoMetadataInput",
     "WebFeedPropertiesInput",
     "WebFeedPropertiesUpdateInput",
     "WorkflowActionInput",
     "WorkflowFilter",
     "WorkflowInput",
     "WorkflowUpdateInput",
     "YouTubeFeedPropertiesInput",
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240505001/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240505001/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/base_model.py` & `graphlit_client-1.0.20240505001/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240505001/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/client.py` & `graphlit_client-1.0.20240505001/graphlit_api/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 from typing import Any, Dict, List, Optional, Union
 
 from .add_contents_to_collections import AddContentsToCollections
 from .async_base_client import AsyncBaseClient
 from .base_model import UNSET, UnsetType
 from .clear_conversation import ClearConversation
 from .close_conversation import CloseConversation
+from .count_alerts import CountAlerts
+from .count_categories import CountCategories
+from .count_collections import CountCollections
+from .count_contents import CountContents
+from .count_conversations import CountConversations
+from .count_events import CountEvents
+from .count_feeds import CountFeeds
+from .count_labels import CountLabels
+from .count_organizations import CountOrganizations
+from .count_persons import CountPersons
+from .count_places import CountPlaces
+from .count_products import CountProducts
+from .count_repos import CountRepos
+from .count_softwares import CountSoftwares
+from .count_specifications import CountSpecifications
+from .count_workflows import CountWorkflows
 from .create_alert import CreateAlert
 from .create_category import CreateCategory
 from .create_collection import CreateCollection
 from .create_conversation import CreateConversation
 from .create_event import CreateEvent
 from .create_feed import CreateFeed
 from .create_label import CreateLabel
@@ -20,15 +36,14 @@
 from .create_person import CreatePerson
 from .create_place import CreatePlace
 from .create_product import CreateProduct
 from .create_repo import CreateRepo
 from .create_software import CreateSoftware
 from .create_specification import CreateSpecification
 from .create_workflow import CreateWorkflow
-from .credits import Credits
 from .delete_alert import DeleteAlert
 from .delete_alerts import DeleteAlerts
 from .delete_all_alerts import DeleteAllAlerts
 from .delete_all_categories import DeleteAllCategories
 from .delete_all_collections import DeleteAllCollections
 from .delete_all_contents import DeleteAllContents
 from .delete_all_conversations import DeleteAllConversations
@@ -37,14 +52,15 @@
 from .delete_all_labels import DeleteAllLabels
 from .delete_all_organizations import DeleteAllOrganizations
 from .delete_all_persons import DeleteAllPersons
 from .delete_all_places import DeleteAllPlaces
 from .delete_all_products import DeleteAllProducts
 from .delete_all_repos import DeleteAllRepos
 from .delete_all_softwares import DeleteAllSoftwares
+from .delete_all_specifications import DeleteAllSpecifications
 from .delete_all_workflows import DeleteAllWorkflows
 from .delete_categories import DeleteCategories
 from .delete_category import DeleteCategory
 from .delete_collection import DeleteCollection
 from .delete_collections import DeleteCollections
 from .delete_content import DeleteContent
 from .delete_contents import DeleteContents
@@ -66,14 +82,15 @@
 from .delete_product import DeleteProduct
 from .delete_products import DeleteProducts
 from .delete_repo import DeleteRepo
 from .delete_repos import DeleteRepos
 from .delete_software import DeleteSoftware
 from .delete_softwares import DeleteSoftwares
 from .delete_specification import DeleteSpecification
+from .delete_specifications import DeleteSpecifications
 from .delete_workflow import DeleteWorkflow
 from .delete_workflows import DeleteWorkflows
 from .disable_alert import DisableAlert
 from .disable_feed import DisableFeed
 from .enable_alert import EnableAlert
 from .enable_feed import EnableFeed
 from .enums import TextTypes
@@ -106,14 +123,15 @@
     CategoryInput,
     CategoryUpdateInput,
     CollectionFilter,
     CollectionInput,
     CollectionUpdateInput,
     ContentFacetInput,
     ContentFilter,
+    ContentGraphInput,
     ContentPublishingConnectorInput,
     ContentUpdateInput,
     ConversationFilter,
     ConversationInput,
     ConversationUpdateInput,
     EntityReferenceInput,
     EventFilter,
@@ -158,14 +176,30 @@
 from .is_feed_done import IsFeedDone
 from .lookup_credits import LookupCredits
 from .lookup_usage import LookupUsage
 from .operations import (
     ADD_CONTENTS_TO_COLLECTIONS_GQL,
     CLEAR_CONVERSATION_GQL,
     CLOSE_CONVERSATION_GQL,
+    COUNT_ALERTS_GQL,
+    COUNT_CATEGORIES_GQL,
+    COUNT_COLLECTIONS_GQL,
+    COUNT_CONTENTS_GQL,
+    COUNT_CONVERSATIONS_GQL,
+    COUNT_EVENTS_GQL,
+    COUNT_FEEDS_GQL,
+    COUNT_LABELS_GQL,
+    COUNT_ORGANIZATIONS_GQL,
+    COUNT_PERSONS_GQL,
+    COUNT_PLACES_GQL,
+    COUNT_PRODUCTS_GQL,
+    COUNT_REPOS_GQL,
+    COUNT_SOFTWARES_GQL,
+    COUNT_SPECIFICATIONS_GQL,
+    COUNT_WORKFLOWS_GQL,
     CREATE_ALERT_GQL,
     CREATE_CATEGORY_GQL,
     CREATE_COLLECTION_GQL,
     CREATE_CONVERSATION_GQL,
     CREATE_EVENT_GQL,
     CREATE_FEED_GQL,
     CREATE_LABEL_GQL,
@@ -174,15 +208,14 @@
     CREATE_PERSON_GQL,
     CREATE_PLACE_GQL,
     CREATE_PRODUCT_GQL,
     CREATE_REPO_GQL,
     CREATE_SOFTWARE_GQL,
     CREATE_SPECIFICATION_GQL,
     CREATE_WORKFLOW_GQL,
-    CREDITS_GQL,
     DELETE_ALERT_GQL,
     DELETE_ALERTS_GQL,
     DELETE_ALL_ALERTS_GQL,
     DELETE_ALL_CATEGORIES_GQL,
     DELETE_ALL_COLLECTIONS_GQL,
     DELETE_ALL_CONTENTS_GQL,
     DELETE_ALL_CONVERSATIONS_GQL,
@@ -191,14 +224,15 @@
     DELETE_ALL_LABELS_GQL,
     DELETE_ALL_ORGANIZATIONS_GQL,
     DELETE_ALL_PERSONS_GQL,
     DELETE_ALL_PLACES_GQL,
     DELETE_ALL_PRODUCTS_GQL,
     DELETE_ALL_REPOS_GQL,
     DELETE_ALL_SOFTWARES_GQL,
+    DELETE_ALL_SPECIFICATIONS_GQL,
     DELETE_ALL_WORKFLOWS_GQL,
     DELETE_CATEGORIES_GQL,
     DELETE_CATEGORY_GQL,
     DELETE_COLLECTION_GQL,
     DELETE_COLLECTIONS_GQL,
     DELETE_CONTENT_GQL,
     DELETE_CONTENTS_GQL,
@@ -220,14 +254,15 @@
     DELETE_PRODUCT_GQL,
     DELETE_PRODUCTS_GQL,
     DELETE_REPO_GQL,
     DELETE_REPOS_GQL,
     DELETE_SOFTWARE_GQL,
     DELETE_SOFTWARES_GQL,
     DELETE_SPECIFICATION_GQL,
+    DELETE_SPECIFICATIONS_GQL,
     DELETE_WORKFLOW_GQL,
     DELETE_WORKFLOWS_GQL,
     DISABLE_ALERT_GQL,
     DISABLE_FEED_GQL,
     ENABLE_ALERT_GQL,
     ENABLE_FEED_GQL,
     EXTRACT_CONTENTS_GQL,
@@ -259,27 +294,30 @@
     PROMPT_SPECIFICATIONS_GQL,
     PUBLISH_CONTENTS_GQL,
     PUBLISH_CONVERSATION_GQL,
     PUBLISH_TEXT_GQL,
     QUERY_ALERTS_GQL,
     QUERY_CATEGORIES_GQL,
     QUERY_COLLECTIONS_GQL,
-    QUERY_CONTENT_FACETS_GQL,
+    QUERY_CONTENTS_FACETS_GQL,
     QUERY_CONTENTS_GQL,
+    QUERY_CONTENTS_GRAPH_GQL,
     QUERY_CONVERSATIONS_GQL,
+    QUERY_CREDITS_GQL,
     QUERY_EVENTS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_LABELS_GQL,
     QUERY_ORGANIZATIONS_GQL,
     QUERY_PERSONS_GQL,
     QUERY_PLACES_GQL,
     QUERY_PRODUCTS_GQL,
     QUERY_REPOS_GQL,
     QUERY_SOFTWARES_GQL,
     QUERY_SPECIFICATIONS_GQL,
+    QUERY_USAGE_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
     SUGGEST_CONVERSATION_GQL,
     SUMMARIZE_CONTENTS_GQL,
     UPDATE_ALERT_GQL,
     UPDATE_CATEGORY_GQL,
     UPDATE_COLLECTION_GQL,
@@ -294,37 +332,39 @@
     UPDATE_PLACE_GQL,
     UPDATE_PRODUCT_GQL,
     UPDATE_PROJECT_GQL,
     UPDATE_REPO_GQL,
     UPDATE_SOFTWARE_GQL,
     UPDATE_SPECIFICATION_GQL,
     UPDATE_WORKFLOW_GQL,
-    USAGE_GQL,
 )
 from .prompt_conversation import PromptConversation
 from .prompt_specifications import PromptSpecifications
 from .publish_contents import PublishContents
 from .publish_conversation import PublishConversation
 from .publish_text import PublishText
 from .query_alerts import QueryAlerts
 from .query_categories import QueryCategories
 from .query_collections import QueryCollections
-from .query_content_facets import QueryContentFacets
 from .query_contents import QueryContents
+from .query_contents_facets import QueryContentsFacets
+from .query_contents_graph import QueryContentsGraph
 from .query_conversations import QueryConversations
+from .query_credits import QueryCredits
 from .query_events import QueryEvents
 from .query_feeds import QueryFeeds
 from .query_labels import QueryLabels
 from .query_organizations import QueryOrganizations
 from .query_persons import QueryPersons
 from .query_places import QueryPlaces
 from .query_products import QueryProducts
 from .query_repos import QueryRepos
 from .query_softwares import QuerySoftwares
 from .query_specifications import QuerySpecifications
+from .query_usage import QueryUsage
 from .query_workflows import QueryWorkflows
 from .remove_contents_from_collection import RemoveContentsFromCollection
 from .suggest_conversation import SuggestConversation
 from .summarize_contents import SummarizeContents
 from .update_alert import UpdateAlert
 from .update_category import UpdateCategory
 from .update_collection import UpdateCollection
@@ -339,22 +379,34 @@
 from .update_place import UpdatePlace
 from .update_product import UpdateProduct
 from .update_project import UpdateProject
 from .update_repo import UpdateRepo
 from .update_software import UpdateSoftware
 from .update_specification import UpdateSpecification
 from .update_workflow import UpdateWorkflow
-from .usage import Usage
 
 
 def gql(q: str) -> str:
     return q
 
 
 class Client(AsyncBaseClient):
+    async def count_alerts(
+        self, filter: Union[Optional[AlertFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountAlerts:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_ALERTS_GQL,
+            operation_name="CountAlerts",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountAlerts.model_validate(data)
+
     async def create_alert(
         self,
         alert: AlertInput,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> CreateAlert:
         variables: Dict[str, object] = {"alert": alert, "correlationId": correlation_id}
@@ -374,27 +426,42 @@
             operation_name="DeleteAlert",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteAlert.model_validate(data)
 
-    async def delete_alerts(self, ids: List[str], **kwargs: Any) -> DeleteAlerts:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_alerts(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteAlerts:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_ALERTS_GQL,
             operation_name="DeleteAlerts",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteAlerts.model_validate(data)
 
-    async def delete_all_alerts(self, **kwargs: Any) -> DeleteAllAlerts:
-        variables: Dict[str, object] = {}
+    async def delete_all_alerts(
+        self,
+        filter: Union[Optional[AlertFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteAllAlerts:
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_ALERTS_GQL,
             operation_name="DeleteAllAlerts",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -453,44 +520,68 @@
             operation_name="UpdateAlert",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateAlert.model_validate(data)
 
+    async def count_categories(
+        self, filter: Union[Optional[CategoryFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountCategories:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_CATEGORIES_GQL,
+            operation_name="CountCategories",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountCategories.model_validate(data)
+
     async def create_category(
         self, category: CategoryInput, **kwargs: Any
     ) -> CreateCategory:
         variables: Dict[str, object] = {"category": category}
         response = await self.execute(
             query=CREATE_CATEGORY_GQL,
             operation_name="CreateCategory",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateCategory.model_validate(data)
 
     async def delete_all_categories(
-        self, filter: CategoryFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[CategoryFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteAllCategories:
-        variables: Dict[str, object] = {"filter": filter}
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_CATEGORIES_GQL,
             operation_name="DeleteAllCategories",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteAllCategories.model_validate(data)
 
     async def delete_categories(
-        self, ids: List[str], **kwargs: Any
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteCategories:
-        variables: Dict[str, object] = {"ids": ids}
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_CATEGORIES_GQL,
             operation_name="DeleteCategories",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -515,15 +606,15 @@
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return GetCategory.model_validate(data)
 
     async def query_categories(
-        self, filter: CategoryFilter, **kwargs: Any
+        self, filter: Union[Optional[CategoryFilter], UnsetType] = UNSET, **kwargs: Any
     ) -> QueryCategories:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_CATEGORIES_GQL,
             operation_name="QueryCategories",
             variables=variables,
             **kwargs
@@ -559,29 +650,54 @@
             operation_name="AddContentsToCollections",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return AddContentsToCollections.model_validate(data)
 
+    async def count_collections(
+        self,
+        filter: Union[Optional[CollectionFilter], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> CountCollections:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_COLLECTIONS_GQL,
+            operation_name="CountCollections",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountCollections.model_validate(data)
+
     async def create_collection(
         self, collection: CollectionInput, **kwargs: Any
     ) -> CreateCollection:
         variables: Dict[str, object] = {"collection": collection}
         response = await self.execute(
             query=CREATE_COLLECTION_GQL,
             operation_name="CreateCollection",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateCollection.model_validate(data)
 
-    async def delete_all_collections(self, **kwargs: Any) -> DeleteAllCollections:
-        variables: Dict[str, object] = {}
+    async def delete_all_collections(
+        self,
+        filter: Union[Optional[CollectionFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteAllCollections:
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_COLLECTIONS_GQL,
             operation_name="DeleteAllCollections",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -595,17 +711,20 @@
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteCollection.model_validate(data)
 
     async def delete_collections(
-        self, ids: List[str], **kwargs: Any
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteCollections:
-        variables: Dict[str, object] = {"ids": ids}
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_COLLECTIONS_GQL,
             operation_name="DeleteCollections",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -662,16 +781,39 @@
             operation_name="UpdateCollection",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateCollection.model_validate(data)
 
-    async def delete_all_contents(self, **kwargs: Any) -> DeleteAllContents:
-        variables: Dict[str, object] = {}
+    async def count_contents(
+        self, filter: Union[Optional[ContentFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountContents:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_CONTENTS_GQL,
+            operation_name="CountContents",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountContents.model_validate(data)
+
+    async def delete_all_contents(
+        self,
+        filter: Union[Optional[ContentFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteAllContents:
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_CONTENTS_GQL,
             operation_name="DeleteAllContents",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -684,16 +826,21 @@
             operation_name="DeleteContent",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteContent.model_validate(data)
 
-    async def delete_contents(self, ids: List[str], **kwargs: Any) -> DeleteContents:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_contents(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteContents:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_CONTENTS_GQL,
             operation_name="DeleteContents",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -768,28 +915,28 @@
         self,
         name: str,
         text: str,
         text_type: Union[Optional[TextTypes], UnsetType] = UNSET,
         uri: Union[Optional[Any], UnsetType] = UNSET,
         id: Union[Optional[str], UnsetType] = UNSET,
         is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
-        collections: Union[Optional[List[EntityReferenceInput]], UnsetType] = UNSET,
         workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
+        collections: Union[Optional[List[EntityReferenceInput]], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> IngestText:
         variables: Dict[str, object] = {
             "name": name,
             "text": text,
             "textType": text_type,
             "uri": uri,
             "id": id,
             "isSynchronous": is_synchronous,
-            "collections": collections,
             "workflow": workflow,
+            "collections": collections,
             "correlationId": correlation_id,
         }
         response = await self.execute(
             query=INGEST_TEXT_GQL,
             operation_name="IngestText",
             variables=variables,
             **kwargs
@@ -799,26 +946,26 @@
 
     async def ingest_uri(
         self,
         uri: Any,
         name: Union[Optional[str], UnsetType] = UNSET,
         id: Union[Optional[str], UnsetType] = UNSET,
         is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
-        collections: Union[Optional[List[EntityReferenceInput]], UnsetType] = UNSET,
         workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
+        collections: Union[Optional[List[EntityReferenceInput]], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> IngestUri:
         variables: Dict[str, object] = {
             "name": name,
             "uri": uri,
             "id": id,
             "isSynchronous": is_synchronous,
-            "collections": collections,
             "workflow": workflow,
+            "collections": collections,
             "correlationId": correlation_id,
         }
         response = await self.execute(
             query=INGEST_URI_GQL,
             operation_name="IngestUri",
             variables=variables,
             **kwargs
@@ -837,102 +984,118 @@
         data = self.get_data(response)
         return IsContentDone.model_validate(data)
 
     async def publish_contents(
         self,
         publish_prompt: str,
         connector: ContentPublishingConnectorInput,
-        is_synchronous: bool,
         summary_prompt: Union[Optional[str], UnsetType] = UNSET,
         filter: Union[Optional[ContentFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         name: Union[Optional[str], UnsetType] = UNSET,
         summary_specification: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         publish_specification: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         **kwargs: Any
     ) -> PublishContents:
         variables: Dict[str, object] = {
             "summaryPrompt": summary_prompt,
             "publishPrompt": publish_prompt,
             "connector": connector,
             "filter": filter,
+            "isSynchronous": is_synchronous,
             "correlationId": correlation_id,
             "name": name,
             "summarySpecification": summary_specification,
             "publishSpecification": publish_specification,
             "workflow": workflow,
-            "isSynchronous": is_synchronous,
         }
         response = await self.execute(
             query=PUBLISH_CONTENTS_GQL,
             operation_name="PublishContents",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return PublishContents.model_validate(data)
 
     async def publish_text(
         self,
         text: str,
         connector: ContentPublishingConnectorInput,
-        is_synchronous: bool,
         text_type: Union[Optional[TextTypes], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         name: Union[Optional[str], UnsetType] = UNSET,
         workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         **kwargs: Any
     ) -> PublishText:
         variables: Dict[str, object] = {
             "text": text,
             "textType": text_type,
             "connector": connector,
+            "isSynchronous": is_synchronous,
             "correlationId": correlation_id,
             "name": name,
             "workflow": workflow,
-            "isSynchronous": is_synchronous,
         }
         response = await self.execute(
             query=PUBLISH_TEXT_GQL,
             operation_name="PublishText",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return PublishText.model_validate(data)
 
-    async def query_content_facets(
+    async def query_contents(
+        self, filter: ContentFilter, **kwargs: Any
+    ) -> QueryContents:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=QUERY_CONTENTS_GQL,
+            operation_name="QueryContents",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryContents.model_validate(data)
+
+    async def query_contents_facets(
         self,
-        filter: Union[Optional[ContentFilter], UnsetType] = UNSET,
+        filter: ContentFilter,
         facets: Union[Optional[List[ContentFacetInput]], UnsetType] = UNSET,
         **kwargs: Any
-    ) -> QueryContentFacets:
+    ) -> QueryContentsFacets:
         variables: Dict[str, object] = {"filter": filter, "facets": facets}
         response = await self.execute(
-            query=QUERY_CONTENT_FACETS_GQL,
-            operation_name="QueryContentFacets",
+            query=QUERY_CONTENTS_FACETS_GQL,
+            operation_name="QueryContentsFacets",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
-        return QueryContentFacets.model_validate(data)
+        return QueryContentsFacets.model_validate(data)
 
-    async def query_contents(
-        self, filter: Union[Optional[ContentFilter], UnsetType] = UNSET, **kwargs: Any
-    ) -> QueryContents:
-        variables: Dict[str, object] = {"filter": filter}
+    async def query_contents_graph(
+        self,
+        filter: ContentFilter,
+        graph: Union[Optional[ContentGraphInput], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> QueryContentsGraph:
+        variables: Dict[str, object] = {"filter": filter, "graph": graph}
         response = await self.execute(
-            query=QUERY_CONTENTS_GQL,
-            operation_name="QueryContents",
+            query=QUERY_CONTENTS_GRAPH_GQL,
+            operation_name="QueryContentsGraph",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
-        return QueryContents.model_validate(data)
+        return QueryContentsGraph.model_validate(data)
 
     async def summarize_contents(
         self,
         summarizations: List[SummarizationStrategyInput],
         filter: Union[Optional[ContentFilter], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
@@ -982,14 +1145,29 @@
             operation_name="CloseConversation",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CloseConversation.model_validate(data)
 
+    async def count_conversations(
+        self,
+        filter: Union[Optional[ConversationFilter], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> CountConversations:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_CONVERSATIONS_GQL,
+            operation_name="CountConversations",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountConversations.model_validate(data)
+
     async def create_conversation(
         self,
         conversation: ConversationInput,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> CreateConversation:
         variables: Dict[str, object] = {
@@ -1001,16 +1179,26 @@
             operation_name="CreateConversation",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateConversation.model_validate(data)
 
-    async def delete_all_conversations(self, **kwargs: Any) -> DeleteAllConversations:
-        variables: Dict[str, object] = {}
+    async def delete_all_conversations(
+        self,
+        filter: Union[Optional[ConversationFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteAllConversations:
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_CONVERSATIONS_GQL,
             operation_name="DeleteAllConversations",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1024,17 +1212,20 @@
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteConversation.model_validate(data)
 
     async def delete_conversations(
-        self, ids: List[str], **kwargs: Any
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteConversations:
-        variables: Dict[str, object] = {"ids": ids}
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_CONVERSATIONS_GQL,
             operation_name="DeleteConversations",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1073,22 +1264,24 @@
         return PromptConversation.model_validate(data)
 
     async def publish_conversation(
         self,
         id: str,
         connector: ContentPublishingConnectorInput,
         name: Union[Optional[str], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
         workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> PublishConversation:
         variables: Dict[str, object] = {
             "id": id,
             "connector": connector,
             "name": name,
+            "isSynchronous": is_synchronous,
             "workflow": workflow,
             "correlationId": correlation_id,
         }
         response = await self.execute(
             query=PUBLISH_CONVERSATION_GQL,
             operation_name="PublishConversation",
             variables=variables,
@@ -1142,29 +1335,50 @@
             operation_name="UpdateConversation",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateConversation.model_validate(data)
 
+    async def count_events(
+        self, filter: Union[Optional[EventFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountEvents:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_EVENTS_GQL,
+            operation_name="CountEvents",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountEvents.model_validate(data)
+
     async def create_event(self, event: EventInput, **kwargs: Any) -> CreateEvent:
         variables: Dict[str, object] = {"event": event}
         response = await self.execute(
             query=CREATE_EVENT_GQL,
             operation_name="CreateEvent",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateEvent.model_validate(data)
 
     async def delete_all_events(
-        self, filter: EventFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[EventFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteAllEvents:
-        variables: Dict[str, object] = {"filter": filter}
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_EVENTS_GQL,
             operation_name="DeleteAllEvents",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1177,16 +1391,21 @@
             operation_name="DeleteEvent",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteEvent.model_validate(data)
 
-    async def delete_events(self, ids: List[str], **kwargs: Any) -> DeleteEvents:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_events(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteEvents:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_EVENTS_GQL,
             operation_name="DeleteEvents",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1199,15 +1418,17 @@
             operation_name="GetEvent",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return GetEvent.model_validate(data)
 
-    async def query_events(self, filter: EventFilter, **kwargs: Any) -> QueryEvents:
+    async def query_events(
+        self, filter: Union[Optional[EventFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> QueryEvents:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_EVENTS_GQL,
             operation_name="QueryEvents",
             variables=variables,
             **kwargs
         )
@@ -1221,14 +1442,27 @@
             operation_name="UpdateEvent",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateEvent.model_validate(data)
 
+    async def count_feeds(
+        self, filter: Union[Optional[FeedFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountFeeds:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_FEEDS_GQL,
+            operation_name="CountFeeds",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountFeeds.model_validate(data)
+
     async def create_feed(
         self,
         feed: FeedInput,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> CreateFeed:
         variables: Dict[str, object] = {"feed": feed, "correlationId": correlation_id}
@@ -1237,16 +1471,26 @@
             operation_name="CreateFeed",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateFeed.model_validate(data)
 
-    async def delete_all_feeds(self, **kwargs: Any) -> DeleteAllFeeds:
-        variables: Dict[str, object] = {}
+    async def delete_all_feeds(
+        self,
+        filter: Union[Optional[FeedFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteAllFeeds:
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_FEEDS_GQL,
             operation_name="DeleteAllFeeds",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1259,16 +1503,21 @@
             operation_name="DeleteFeed",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteFeed.model_validate(data)
 
-    async def delete_feeds(self, ids: List[str], **kwargs: Any) -> DeleteFeeds:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_feeds(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteFeeds:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_FEEDS_GQL,
             operation_name="DeleteFeeds",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1335,29 +1584,50 @@
             operation_name="UpdateFeed",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateFeed.model_validate(data)
 
+    async def count_labels(
+        self, filter: Union[Optional[LabelFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountLabels:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_LABELS_GQL,
+            operation_name="CountLabels",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountLabels.model_validate(data)
+
     async def create_label(self, label: LabelInput, **kwargs: Any) -> CreateLabel:
         variables: Dict[str, object] = {"label": label}
         response = await self.execute(
             query=CREATE_LABEL_GQL,
             operation_name="CreateLabel",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateLabel.model_validate(data)
 
     async def delete_all_labels(
-        self, filter: LabelFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[LabelFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteAllLabels:
-        variables: Dict[str, object] = {"filter": filter}
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_LABELS_GQL,
             operation_name="DeleteAllLabels",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1370,16 +1640,21 @@
             operation_name="DeleteLabel",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteLabel.model_validate(data)
 
-    async def delete_labels(self, ids: List[str], **kwargs: Any) -> DeleteLabels:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_labels(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteLabels:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_LABELS_GQL,
             operation_name="DeleteLabels",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1392,15 +1667,17 @@
             operation_name="GetLabel",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return GetLabel.model_validate(data)
 
-    async def query_labels(self, filter: LabelFilter, **kwargs: Any) -> QueryLabels:
+    async def query_labels(
+        self, filter: Union[Optional[LabelFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> QueryLabels:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_LABELS_GQL,
             operation_name="QueryLabels",
             variables=variables,
             **kwargs
         )
@@ -1451,31 +1728,54 @@
             operation_name="UpdateObservation",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateObservation.model_validate(data)
 
+    async def count_organizations(
+        self,
+        filter: Union[Optional[OrganizationFilter], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> CountOrganizations:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_ORGANIZATIONS_GQL,
+            operation_name="CountOrganizations",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountOrganizations.model_validate(data)
+
     async def create_organization(
         self, organization: OrganizationInput, **kwargs: Any
     ) -> CreateOrganization:
         variables: Dict[str, object] = {"organization": organization}
         response = await self.execute(
             query=CREATE_ORGANIZATION_GQL,
             operation_name="CreateOrganization",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateOrganization.model_validate(data)
 
     async def delete_all_organizations(
-        self, filter: OrganizationFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[OrganizationFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteAllOrganizations:
-        variables: Dict[str, object] = {"filter": filter}
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_ORGANIZATIONS_GQL,
             operation_name="DeleteAllOrganizations",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1489,17 +1789,20 @@
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteOrganization.model_validate(data)
 
     async def delete_organizations(
-        self, ids: List[str], **kwargs: Any
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteOrganizations:
-        variables: Dict[str, object] = {"ids": ids}
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_ORGANIZATIONS_GQL,
             operation_name="DeleteOrganizations",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1513,15 +1816,17 @@
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return GetOrganization.model_validate(data)
 
     async def query_organizations(
-        self, filter: OrganizationFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[OrganizationFilter], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> QueryOrganizations:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_ORGANIZATIONS_GQL,
             operation_name="QueryOrganizations",
             variables=variables,
             **kwargs
@@ -1538,29 +1843,50 @@
             operation_name="UpdateOrganization",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateOrganization.model_validate(data)
 
+    async def count_persons(
+        self, filter: Union[Optional[PersonFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountPersons:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_PERSONS_GQL,
+            operation_name="CountPersons",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountPersons.model_validate(data)
+
     async def create_person(self, person: PersonInput, **kwargs: Any) -> CreatePerson:
         variables: Dict[str, object] = {"person": person}
         response = await self.execute(
             query=CREATE_PERSON_GQL,
             operation_name="CreatePerson",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreatePerson.model_validate(data)
 
     async def delete_all_persons(
-        self, filter: PersonFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[PersonFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteAllPersons:
-        variables: Dict[str, object] = {"filter": filter}
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_PERSONS_GQL,
             operation_name="DeleteAllPersons",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1573,16 +1899,21 @@
             operation_name="DeletePerson",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeletePerson.model_validate(data)
 
-    async def delete_persons(self, ids: List[str], **kwargs: Any) -> DeletePersons:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_persons(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeletePersons:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_PERSONS_GQL,
             operation_name="DeletePersons",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1595,15 +1926,17 @@
             operation_name="GetPerson",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return GetPerson.model_validate(data)
 
-    async def query_persons(self, filter: PersonFilter, **kwargs: Any) -> QueryPersons:
+    async def query_persons(
+        self, filter: Union[Optional[PersonFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> QueryPersons:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_PERSONS_GQL,
             operation_name="QueryPersons",
             variables=variables,
             **kwargs
         )
@@ -1619,29 +1952,50 @@
             operation_name="UpdatePerson",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdatePerson.model_validate(data)
 
+    async def count_places(
+        self, filter: Union[Optional[PlaceFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountPlaces:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_PLACES_GQL,
+            operation_name="CountPlaces",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountPlaces.model_validate(data)
+
     async def create_place(self, place: PlaceInput, **kwargs: Any) -> CreatePlace:
         variables: Dict[str, object] = {"place": place}
         response = await self.execute(
             query=CREATE_PLACE_GQL,
             operation_name="CreatePlace",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreatePlace.model_validate(data)
 
     async def delete_all_places(
-        self, filter: PlaceFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[PlaceFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteAllPlaces:
-        variables: Dict[str, object] = {"filter": filter}
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_PLACES_GQL,
             operation_name="DeleteAllPlaces",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1654,16 +2008,21 @@
             operation_name="DeletePlace",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeletePlace.model_validate(data)
 
-    async def delete_places(self, ids: List[str], **kwargs: Any) -> DeletePlaces:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_places(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeletePlaces:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_PLACES_GQL,
             operation_name="DeletePlaces",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1676,15 +2035,17 @@
             operation_name="GetPlace",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return GetPlace.model_validate(data)
 
-    async def query_places(self, filter: PlaceFilter, **kwargs: Any) -> QueryPlaces:
+    async def query_places(
+        self, filter: Union[Optional[PlaceFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> QueryPlaces:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_PLACES_GQL,
             operation_name="QueryPlaces",
             variables=variables,
             **kwargs
         )
@@ -1698,31 +2059,52 @@
             operation_name="UpdatePlace",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdatePlace.model_validate(data)
 
+    async def count_products(
+        self, filter: Union[Optional[ProductFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountProducts:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_PRODUCTS_GQL,
+            operation_name="CountProducts",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountProducts.model_validate(data)
+
     async def create_product(
         self, product: ProductInput, **kwargs: Any
     ) -> CreateProduct:
         variables: Dict[str, object] = {"product": product}
         response = await self.execute(
             query=CREATE_PRODUCT_GQL,
             operation_name="CreateProduct",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateProduct.model_validate(data)
 
     async def delete_all_products(
-        self, filter: ProductFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[ProductFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteAllProducts:
-        variables: Dict[str, object] = {"filter": filter}
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_PRODUCTS_GQL,
             operation_name="DeleteAllProducts",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1735,16 +2117,21 @@
             operation_name="DeleteProduct",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteProduct.model_validate(data)
 
-    async def delete_products(self, ids: List[str], **kwargs: Any) -> DeleteProducts:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_products(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteProducts:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_PRODUCTS_GQL,
             operation_name="DeleteProducts",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1758,15 +2145,15 @@
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return GetProduct.model_validate(data)
 
     async def query_products(
-        self, filter: ProductFilter, **kwargs: Any
+        self, filter: Union[Optional[ProductFilter], UnsetType] = UNSET, **kwargs: Any
     ) -> QueryProducts:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_PRODUCTS_GQL,
             operation_name="QueryProducts",
             variables=variables,
             **kwargs
@@ -1783,22 +2170,14 @@
             operation_name="UpdateProduct",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateProduct.model_validate(data)
 
-    async def credits(self, start_date: Any, duration: Any, **kwargs: Any) -> Credits:
-        variables: Dict[str, object] = {"startDate": start_date, "duration": duration}
-        response = await self.execute(
-            query=CREDITS_GQL, operation_name="Credits", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return Credits.model_validate(data)
-
     async def get_project(self, **kwargs: Any) -> GetProject:
         variables: Dict[str, object] = {}
         response = await self.execute(
             query=GET_PROJECT_GQL,
             operation_name="GetProject",
             variables=variables,
             **kwargs
@@ -1824,50 +2203,89 @@
             operation_name="LookupUsage",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return LookupUsage.model_validate(data)
 
+    async def query_credits(
+        self, start_date: Any, duration: Any, **kwargs: Any
+    ) -> QueryCredits:
+        variables: Dict[str, object] = {"startDate": start_date, "duration": duration}
+        response = await self.execute(
+            query=QUERY_CREDITS_GQL,
+            operation_name="QueryCredits",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryCredits.model_validate(data)
+
+    async def query_usage(
+        self, start_date: Any, duration: Any, **kwargs: Any
+    ) -> QueryUsage:
+        variables: Dict[str, object] = {"startDate": start_date, "duration": duration}
+        response = await self.execute(
+            query=QUERY_USAGE_GQL,
+            operation_name="QueryUsage",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryUsage.model_validate(data)
+
     async def update_project(
         self, project: ProjectUpdateInput, **kwargs: Any
     ) -> UpdateProject:
         variables: Dict[str, object] = {"project": project}
         response = await self.execute(
             query=UPDATE_PROJECT_GQL,
             operation_name="UpdateProject",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateProject.model_validate(data)
 
-    async def usage(self, start_date: Any, duration: Any, **kwargs: Any) -> Usage:
-        variables: Dict[str, object] = {"startDate": start_date, "duration": duration}
+    async def count_repos(
+        self, filter: Union[Optional[RepoFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountRepos:
+        variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
-            query=USAGE_GQL, operation_name="Usage", variables=variables, **kwargs
+            query=COUNT_REPOS_GQL,
+            operation_name="CountRepos",
+            variables=variables,
+            **kwargs
         )
         data = self.get_data(response)
-        return Usage.model_validate(data)
+        return CountRepos.model_validate(data)
 
     async def create_repo(self, repo: RepoInput, **kwargs: Any) -> CreateRepo:
         variables: Dict[str, object] = {"repo": repo}
         response = await self.execute(
             query=CREATE_REPO_GQL,
             operation_name="CreateRepo",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateRepo.model_validate(data)
 
     async def delete_all_repos(
-        self, filter: RepoFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[RepoFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteAllRepos:
-        variables: Dict[str, object] = {"filter": filter}
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_REPOS_GQL,
             operation_name="DeleteAllRepos",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1880,16 +2298,21 @@
             operation_name="DeleteRepo",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteRepo.model_validate(data)
 
-    async def delete_repos(self, ids: List[str], **kwargs: Any) -> DeleteRepos:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_repos(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteRepos:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_REPOS_GQL,
             operation_name="DeleteRepos",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1899,15 +2322,17 @@
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
             query=GET_REPO_GQL, operation_name="GetRepo", variables=variables, **kwargs
         )
         data = self.get_data(response)
         return GetRepo.model_validate(data)
 
-    async def query_repos(self, filter: RepoFilter, **kwargs: Any) -> QueryRepos:
+    async def query_repos(
+        self, filter: Union[Optional[RepoFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> QueryRepos:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_REPOS_GQL,
             operation_name="QueryRepos",
             variables=variables,
             **kwargs
         )
@@ -1921,31 +2346,52 @@
             operation_name="UpdateRepo",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateRepo.model_validate(data)
 
+    async def count_softwares(
+        self, filter: Union[Optional[SoftwareFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountSoftwares:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_SOFTWARES_GQL,
+            operation_name="CountSoftwares",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountSoftwares.model_validate(data)
+
     async def create_software(
         self, software: SoftwareInput, **kwargs: Any
     ) -> CreateSoftware:
         variables: Dict[str, object] = {"software": software}
         response = await self.execute(
             query=CREATE_SOFTWARE_GQL,
             operation_name="CreateSoftware",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateSoftware.model_validate(data)
 
     async def delete_all_softwares(
-        self, filter: SoftwareFilter, **kwargs: Any
+        self,
+        filter: Union[Optional[SoftwareFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
     ) -> DeleteAllSoftwares:
-        variables: Dict[str, object] = {"filter": filter}
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_SOFTWARES_GQL,
             operation_name="DeleteAllSoftwares",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1958,16 +2404,21 @@
             operation_name="DeleteSoftware",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteSoftware.model_validate(data)
 
-    async def delete_softwares(self, ids: List[str], **kwargs: Any) -> DeleteSoftwares:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_softwares(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteSoftwares:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_SOFTWARES_GQL,
             operation_name="DeleteSoftwares",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -1981,15 +2432,15 @@
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return GetSoftware.model_validate(data)
 
     async def query_softwares(
-        self, filter: SoftwareFilter, **kwargs: Any
+        self, filter: Union[Optional[SoftwareFilter], UnsetType] = UNSET, **kwargs: Any
     ) -> QuerySoftwares:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_SOFTWARES_GQL,
             operation_name="QuerySoftwares",
             variables=variables,
             **kwargs
@@ -2006,38 +2457,90 @@
             operation_name="UpdateSoftware",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateSoftware.model_validate(data)
 
+    async def count_specifications(
+        self,
+        filter: Union[Optional[SpecificationFilter], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> CountSpecifications:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_SPECIFICATIONS_GQL,
+            operation_name="CountSpecifications",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountSpecifications.model_validate(data)
+
     async def create_specification(
         self, specification: SpecificationInput, **kwargs: Any
     ) -> CreateSpecification:
         variables: Dict[str, object] = {"specification": specification}
         response = await self.execute(
             query=CREATE_SPECIFICATION_GQL,
             operation_name="CreateSpecification",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateSpecification.model_validate(data)
 
+    async def delete_all_specifications(
+        self,
+        filter: Union[Optional[SpecificationFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteAllSpecifications:
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
+        response = await self.execute(
+            query=DELETE_ALL_SPECIFICATIONS_GQL,
+            operation_name="DeleteAllSpecifications",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteAllSpecifications.model_validate(data)
+
     async def delete_specification(self, id: str, **kwargs: Any) -> DeleteSpecification:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
             query=DELETE_SPECIFICATION_GQL,
             operation_name="DeleteSpecification",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteSpecification.model_validate(data)
 
+    async def delete_specifications(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteSpecifications:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
+        response = await self.execute(
+            query=DELETE_SPECIFICATIONS_GQL,
+            operation_name="DeleteSpecifications",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return DeleteSpecifications.model_validate(data)
+
     async def get_specification(self, id: str, **kwargs: Any) -> GetSpecification:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
             query=GET_SPECIFICATION_GQL,
             operation_name="GetSpecification",
             variables=variables,
             **kwargs
@@ -2082,29 +2585,52 @@
             operation_name="UpdateSpecification",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return UpdateSpecification.model_validate(data)
 
+    async def count_workflows(
+        self, filter: Union[Optional[WorkflowFilter], UnsetType] = UNSET, **kwargs: Any
+    ) -> CountWorkflows:
+        variables: Dict[str, object] = {"filter": filter}
+        response = await self.execute(
+            query=COUNT_WORKFLOWS_GQL,
+            operation_name="CountWorkflows",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return CountWorkflows.model_validate(data)
+
     async def create_workflow(
         self, workflow: WorkflowInput, **kwargs: Any
     ) -> CreateWorkflow:
         variables: Dict[str, object] = {"workflow": workflow}
         response = await self.execute(
             query=CREATE_WORKFLOW_GQL,
             operation_name="CreateWorkflow",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return CreateWorkflow.model_validate(data)
 
-    async def delete_all_workflows(self, **kwargs: Any) -> DeleteAllWorkflows:
-        variables: Dict[str, object] = {}
+    async def delete_all_workflows(
+        self,
+        filter: Union[Optional[WorkflowFilter], UnsetType] = UNSET,
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteAllWorkflows:
+        variables: Dict[str, object] = {
+            "filter": filter,
+            "isSynchronous": is_synchronous,
+            "correlationId": correlation_id,
+        }
         response = await self.execute(
             query=DELETE_ALL_WORKFLOWS_GQL,
             operation_name="DeleteAllWorkflows",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
@@ -2117,16 +2643,21 @@
             operation_name="DeleteWorkflow",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteWorkflow.model_validate(data)
 
-    async def delete_workflows(self, ids: List[str], **kwargs: Any) -> DeleteWorkflows:
-        variables: Dict[str, object] = {"ids": ids}
+    async def delete_workflows(
+        self,
+        ids: List[str],
+        is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> DeleteWorkflows:
+        variables: Dict[str, object] = {"ids": ids, "isSynchronous": is_synchronous}
         response = await self.execute(
             query=DELETE_WORKFLOWS_GQL,
             operation_name="DeleteWorkflows",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240505001/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240505001/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240505001/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240505001/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240505001/graphlit_api/create_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 class CreateWorkflowCreateWorkflowExtractionJobsConnectorAzureImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
 
 
 class CreateWorkflowCreateWorkflowExtractionJobsConnectorOpenAiImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
     detail_level: Optional[OpenAIVisionDetailLevels] = Field(alias="detailLevel")
+    custom_instructions: Optional[str] = Field(alias="customInstructions")
 
 
 class CreateWorkflowCreateWorkflowExtractionJobsConnectorModelText(BaseModel):
     specification: Optional[
         "CreateWorkflowCreateWorkflowExtractionJobsConnectorModelTextSpecification"
     ]
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/credits.py` & `graphlit_client-1.0.20240505001/graphlit_api/lookup_credits.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
-from typing import Any, List, Optional
+from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
-class Credits(BaseModel):
-    credits: Optional[List[Optional["CreditsCredits"]]]
+class LookupCredits(BaseModel):
+    lookup_credits: Optional["LookupCreditsLookupCredits"] = Field(
+        alias="lookupCredits"
+    )
 
 
-class CreditsCredits(BaseModel):
+class LookupCreditsLookupCredits(BaseModel):
     correlation_id: Optional[str] = Field(alias="correlationId")
     owner_id: Optional[str] = Field(alias="ownerId")
     credits: Optional[Any]
     storage_ratio: Optional[Any] = Field(alias="storageRatio")
     compute_ratio: Optional[Any] = Field(alias="computeRatio")
     preparation_ratio: Optional[Any] = Field(alias="preparationRatio")
     extraction_ratio: Optional[Any] = Field(alias="extractionRatio")
     enrichment_ratio: Optional[Any] = Field(alias="enrichmentRatio")
     publishing_ratio: Optional[Any] = Field(alias="publishingRatio")
     search_ratio: Optional[Any] = Field(alias="searchRatio")
     conversation_ratio: Optional[Any] = Field(alias="conversationRatio")
 
 
-Credits.model_rebuild()
+LookupCredits.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240505001/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/delete_all_organizations.py` & `graphlit_client-1.0.20240505001/graphlit_api/delete_all_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/enums.py` & `graphlit_client-1.0.20240505001/graphlit_api/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 class ConversationTypes(str, Enum):
     CONTENT = "CONTENT"
 
 
 class FeedTypes(str, Enum):
     NOTION = "NOTION"
     SLACK = "SLACK"
+    MICROSOFT_TEAMS = "MICROSOFT_TEAMS"
     DISCORD = "DISCORD"
     REDDIT = "REDDIT"
     WEB = "WEB"
     RSS = "RSS"
     SITE = "SITE"
     YOU_TUBE = "YOU_TUBE"
     EMAIL = "EMAIL"
@@ -284,14 +285,15 @@
     RELATIVE_TIME = "RELATIVE_TIME"
     ABSOLUTE_TIME = "ABSOLUTE_TIME"
 
 
 class LinkTypes(str, Enum):
     TYPE_FORM = "TYPE_FORM"
     AIRTABLE = "AIRTABLE"
+    MICROSOFT_TEAMS = "MICROSOFT_TEAMS"
     DISCORD = "DISCORD"
     APPLE = "APPLE"
     SLACK = "SLACK"
     ANGEL_LIST = "ANGEL_LIST"
     CRUNCHBASE = "CRUNCHBASE"
     LINKED_IN = "LINKED_IN"
     DIFFBOT = "DIFFBOT"
@@ -459,27 +461,29 @@
     WINDOWED = "WINDOWED"
     SUMMARIZED = "SUMMARIZED"
 
 
 class PromptStrategyTypes(str, Enum):
     OPTIMIZE_SEARCH = "OPTIMIZE_SEARCH"
     REWRITE = "REWRITE"
+    REWRITE_QUESTION = "REWRITE_QUESTION"
     REWRITE_MULTIPLE = "REWRITE_MULTIPLE"
     NONE = "NONE"
 
 
 class RetrievalStrategyTypes(str, Enum):
     CONTENT = "CONTENT"
     CHUNK = "CHUNK"
     SECTION = "SECTION"
 
 
 class RerankingModelServiceTypes(str, Enum):
     COHERE = "COHERE"
     JINA = "JINA"
+    PONGO = "PONGO"
 
 
 class OpenAIModels(str, Enum):
     GPT35_TURBO = "GPT35_TURBO"
     GPT35_TURBO_0613 = "GPT35_TURBO_0613"
     GPT35_TURBO_16K = "GPT35_TURBO_16K"
     GPT35_TURBO_16K_0613 = "GPT35_TURBO_16K_0613"
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240505001/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240505001/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_alert.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_alert.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_collection.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_content.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_content.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,38 +6,44 @@
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
     ContentTypes,
     EntityState,
     FileTypes,
+    ImageProjectionTypes,
     LinkTypes,
     MailImportance,
     MailPriority,
     MailSensitivity,
     ObservableTypes,
     OccurrenceTypes,
+    OrientationTypes,
+    TextRoles,
 )
 
 
 class GetContent(BaseModel):
     content: Optional["GetContentContent"]
 
 
 class GetContentContent(BaseModel):
     id: str
     name: str
-    description: Optional[str]
     creation_date: Any = Field(alias="creationDate")
     owner: "GetContentContentOwner"
     state: EntityState
     original_date: Optional[Any] = Field(alias="originalDate")
     finished_date: Optional[Any] = Field(alias="finishedDate")
     workflow_duration: Optional[Any] = Field(alias="workflowDuration")
     uri: Optional[Any]
+    description: Optional[str]
+    markdown: Optional[str]
+    address: Optional["GetContentContentAddress"]
+    location: Optional["GetContentContentLocation"]
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
     mime_type: Optional[str] = Field(alias="mimeType")
     file_name: Optional[str] = Field(alias="fileName")
     file_size: Optional[Any] = Field(alias="fileSize")
     master_uri: Optional[Any] = Field(alias="masterUri")
     image_uri: Optional[Any] = Field(alias="imageUri")
@@ -46,191 +52,258 @@
     transcript_uri: Optional[Any] = Field(alias="transcriptUri")
     video: Optional["GetContentContentVideo"]
     audio: Optional["GetContentContentAudio"]
     image: Optional["GetContentContentImage"]
     document: Optional["GetContentContentDocument"]
     email: Optional["GetContentContentEmail"]
     issue: Optional["GetContentContentIssue"]
-    observations: Optional[List[Optional["GetContentContentObservations"]]]
+    package: Optional["GetContentContentPackage"]
     parent: Optional["GetContentContentParent"]
     children: Optional[List[Optional["GetContentContentChildren"]]]
-    collections: Optional[List[Optional["GetContentContentCollections"]]]
     feed: Optional["GetContentContentFeed"]
-    workflow: Optional["GetContentContentWorkflow"]
-    markdown: Optional[str]
+    collections: Optional[List[Optional["GetContentContentCollections"]]]
     links: Optional[List["GetContentContentLinks"]]
+    observations: Optional[List[Optional["GetContentContentObservations"]]]
+    workflow: Optional["GetContentContentWorkflow"]
+    pages: Optional[List["GetContentContentPages"]]
+    segments: Optional[List["GetContentContentSegments"]]
     error: Optional[str]
 
 
 class GetContentContentOwner(BaseModel):
     id: str
 
 
+class GetContentContentAddress(BaseModel):
+    street_address: Optional[str] = Field(alias="streetAddress")
+    city: Optional[str]
+    region: Optional[str]
+    country: Optional[str]
+    postal_code: Optional[str] = Field(alias="postalCode")
+
+
+class GetContentContentLocation(BaseModel):
+    latitude: Optional[float]
+    longitude: Optional[float]
+
+
 class GetContentContentVideo(BaseModel):
     width: Optional[int]
     height: Optional[int]
     duration: Optional[str]
-    software: Optional[str]
     make: Optional[str]
     model: Optional[str]
+    software: Optional[str]
+    title: Optional[str]
+    description: Optional[str]
+    keywords: Optional[List[Optional[str]]]
+    author: Optional[str]
 
 
 class GetContentContentAudio(BaseModel):
     keywords: Optional[List[Optional[str]]]
     author: Optional[str]
     series: Optional[str]
     episode: Optional[str]
     episode_type: Optional[str] = Field(alias="episodeType")
     season: Optional[str]
     publisher: Optional[str]
     copyright: Optional[str]
     language: Optional[str]
     genre: Optional[str]
     title: Optional[str]
+    description: Optional[str]
     bitrate: Optional[int]
     channels: Optional[int]
     sample_rate: Optional[int] = Field(alias="sampleRate")
     bits_per_sample: Optional[int] = Field(alias="bitsPerSample")
     duration: Optional[str]
 
 
 class GetContentContentImage(BaseModel):
     width: Optional[int]
     height: Optional[int]
+    resolution_x: Optional[int] = Field(alias="resolutionX")
+    resolution_y: Optional[int] = Field(alias="resolutionY")
+    bits_per_component: Optional[int] = Field(alias="bitsPerComponent")
+    components: Optional[int]
+    projection_type: Optional[ImageProjectionTypes] = Field(alias="projectionType")
+    orientation: Optional[OrientationTypes]
     description: Optional[str]
-    software: Optional[str]
-    identifier: Optional[str]
     make: Optional[str]
     model: Optional[str]
+    software: Optional[str]
+    lens: Optional[str]
+    focal_length: Optional[float] = Field(alias="focalLength")
+    exposure_time: Optional[str] = Field(alias="exposureTime")
+    f_number: Optional[str] = Field(alias="fNumber")
+    iso: Optional[str]
+    heading: Optional[float]
+    pitch: Optional[float]
 
 
 class GetContentContentDocument(BaseModel):
     title: Optional[str]
     subject: Optional[str]
+    summary: Optional[str]
     author: Optional[str]
-    software: Optional[str]
     publisher: Optional[str]
     description: Optional[str]
-    summary: Optional[str]
     keywords: Optional[List[Optional[str]]]
     page_count: Optional[int] = Field(alias="pageCount")
     worksheet_count: Optional[int] = Field(alias="worksheetCount")
     slide_count: Optional[int] = Field(alias="slideCount")
     word_count: Optional[int] = Field(alias="wordCount")
     line_count: Optional[int] = Field(alias="lineCount")
     paragraph_count: Optional[int] = Field(alias="paragraphCount")
-    character_count: Optional[int] = Field(alias="characterCount")
     is_encrypted: Optional[bool] = Field(alias="isEncrypted")
     has_digital_signature: Optional[bool] = Field(alias="hasDigitalSignature")
 
 
 class GetContentContentEmail(BaseModel):
-    subject: Optional[str]
     identifier: Optional[str]
+    subject: Optional[str]
+    labels: Optional[List[Optional[str]]]
     sensitivity: Optional[MailSensitivity]
     priority: Optional[MailPriority]
     importance: Optional[MailImportance]
-    labels: Optional[List[Optional[str]]]
     from_: Optional[List[Optional["GetContentContentEmailFrom"]]] = Field(alias="from")
     to: Optional[List[Optional["GetContentContentEmailTo"]]]
     cc: Optional[List[Optional["GetContentContentEmailCc"]]]
     bcc: Optional[List[Optional["GetContentContentEmailBcc"]]]
 
 
 class GetContentContentEmailFrom(BaseModel):
     name: Optional[str]
-    family_name: Optional[str] = Field(alias="familyName")
-    given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
+    given_name: Optional[str] = Field(alias="givenName")
+    family_name: Optional[str] = Field(alias="familyName")
 
 
 class GetContentContentEmailTo(BaseModel):
     name: Optional[str]
-    family_name: Optional[str] = Field(alias="familyName")
-    given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
+    given_name: Optional[str] = Field(alias="givenName")
+    family_name: Optional[str] = Field(alias="familyName")
 
 
 class GetContentContentEmailCc(BaseModel):
     name: Optional[str]
-    family_name: Optional[str] = Field(alias="familyName")
-    given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
+    given_name: Optional[str] = Field(alias="givenName")
+    family_name: Optional[str] = Field(alias="familyName")
 
 
 class GetContentContentEmailBcc(BaseModel):
     name: Optional[str]
-    family_name: Optional[str] = Field(alias="familyName")
-    given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
+    given_name: Optional[str] = Field(alias="givenName")
+    family_name: Optional[str] = Field(alias="familyName")
 
 
 class GetContentContentIssue(BaseModel):
+    identifier: Optional[str]
     title: Optional[str]
     project: Optional[str]
     team: Optional[str]
     status: Optional[str]
     priority: Optional[str]
     type: Optional[str]
-    identifier: Optional[str]
     labels: Optional[List[Optional[str]]]
 
 
+class GetContentContentPackage(BaseModel):
+    file_count: Optional[int] = Field(alias="fileCount")
+    folder_count: Optional[int] = Field(alias="folderCount")
+    is_encrypted: Optional[bool] = Field(alias="isEncrypted")
+
+
+class GetContentContentParent(BaseModel):
+    id: str
+    name: str
+
+
+class GetContentContentChildren(BaseModel):
+    id: str
+    name: str
+
+
+class GetContentContentFeed(BaseModel):
+    id: str
+    name: str
+
+
+class GetContentContentCollections(BaseModel):
+    id: str
+    name: str
+
+
+class GetContentContentLinks(BaseModel):
+    uri: Optional[Any]
+    link_type: Optional[LinkTypes] = Field(alias="linkType")
+
+
 class GetContentContentObservations(BaseModel):
+    id: str
     type: ObservableTypes
     observable: "GetContentContentObservationsObservable"
     occurrences: Optional[List[Optional["GetContentContentObservationsOccurrences"]]]
+    state: EntityState
 
 
 class GetContentContentObservationsObservable(BaseModel):
     id: str
     name: Optional[str]
 
 
 class GetContentContentObservationsOccurrences(BaseModel):
     type: Optional[OccurrenceTypes]
     confidence: Optional[float]
+    start_time: Optional[Any] = Field(alias="startTime")
+    end_time: Optional[Any] = Field(alias="endTime")
+    page_index: Optional[int] = Field(alias="pageIndex")
     bounding_box: Optional["GetContentContentObservationsOccurrencesBoundingBox"] = (
         Field(alias="boundingBox")
     )
-    page_index: Optional[int] = Field(alias="pageIndex")
-    start_time: Optional[Any] = Field(alias="startTime")
-    end_time: Optional[Any] = Field(alias="endTime")
 
 
 class GetContentContentObservationsOccurrencesBoundingBox(BaseModel):
     left: Optional[float]
     top: Optional[float]
     width: Optional[float]
     height: Optional[float]
 
 
-class GetContentContentParent(BaseModel):
-    id: str
-
-
-class GetContentContentChildren(BaseModel):
-    id: str
-
-
-class GetContentContentCollections(BaseModel):
+class GetContentContentWorkflow(BaseModel):
     id: str
+    name: str
 
 
-class GetContentContentFeed(BaseModel):
-    id: str
+class GetContentContentPages(BaseModel):
+    index: Optional[int]
+    chunks: Optional[List[Optional["GetContentContentPagesChunks"]]]
 
 
-class GetContentContentWorkflow(BaseModel):
-    id: str
+class GetContentContentPagesChunks(BaseModel):
+    index: Optional[int]
+    page_index: Optional[int] = Field(alias="pageIndex")
+    row_index: Optional[int] = Field(alias="rowIndex")
+    column_index: Optional[int] = Field(alias="columnIndex")
+    confidence: Optional[float]
+    text: Optional[str]
+    role: Optional[TextRoles]
+    relevance: Optional[float]
 
 
-class GetContentContentLinks(BaseModel):
-    uri: Optional[Any]
-    link_type: Optional[LinkTypes] = Field(alias="linkType")
+class GetContentContentSegments(BaseModel):
+    start_time: Optional[Any] = Field(alias="startTime")
+    end_time: Optional[Any] = Field(alias="endTime")
+    text: Optional[str]
+    relevance: Optional[float]
 
 
 GetContent.model_rebuild()
 GetContentContent.model_rebuild()
 GetContentContentEmail.model_rebuild()
 GetContentContentObservations.model_rebuild()
 GetContentContentObservationsOccurrences.model_rebuild()
+GetContentContentPages.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_conversation.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,14 +59,21 @@
     end_time: Optional[Any] = Field(alias="endTime")
     page_number: Optional[int] = Field(alias="pageNumber")
     frame_number: Optional[int] = Field(alias="frameNumber")
 
 
 class GetConversationConversationMessagesCitationsContent(BaseModel):
     id: str
+    name: str
+    state: EntityState
+    type: Optional[ContentTypes]
+    file_type: Optional[FileTypes] = Field(alias="fileType")
+    file_name: Optional[str] = Field(alias="fileName")
+    original_date: Optional[Any] = Field(alias="originalDate")
+    uri: Optional[Any]
 
 
 class GetConversationConversationSpecification(BaseModel):
     id: str
     name: str
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_event.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_event.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_feed.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_organization.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_organization.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_person.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_person.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_place.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_place.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_product.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_product.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_project.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_software.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_software.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_specification.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
     AnthropicModels,
     AzureOpenAIModels,
+    CohereModels,
+    ConversationSearchTypes,
     ConversationStrategyTypes,
     EntityState,
     ModelServiceTypes,
     OpenAIModels,
     PromptStrategyTypes,
     ReplicateModels,
     RerankingModelServiceTypes,
@@ -31,28 +33,32 @@
     creation_date: Any = Field(alias="creationDate")
     owner: "GetSpecificationSpecificationOwner"
     state: EntityState
     type: Optional[SpecificationTypes]
     service_type: Optional[ModelServiceTypes] = Field(alias="serviceType")
     system_prompt: Optional[str] = Field(alias="systemPrompt")
     custom_guidance: Optional[str] = Field(alias="customGuidance")
+    custom_instructions: Optional[str] = Field(alias="customInstructions")
+    search_type: Optional[ConversationSearchTypes] = Field(alias="searchType")
+    number_similar: Optional[int] = Field(alias="numberSimilar")
     strategy: Optional["GetSpecificationSpecificationStrategy"]
     prompt_strategy: Optional["GetSpecificationSpecificationPromptStrategy"] = Field(
         alias="promptStrategy"
     )
     retrieval_strategy: Optional["GetSpecificationSpecificationRetrievalStrategy"] = (
         Field(alias="retrievalStrategy")
     )
     reranking_strategy: Optional["GetSpecificationSpecificationRerankingStrategy"] = (
         Field(alias="rerankingStrategy")
     )
     open_ai: Optional["GetSpecificationSpecificationOpenAi"] = Field(alias="openAI")
     azure_open_ai: Optional["GetSpecificationSpecificationAzureOpenAi"] = Field(
         alias="azureOpenAI"
     )
+    cohere: Optional["GetSpecificationSpecificationCohere"]
     anthropic: Optional["GetSpecificationSpecificationAnthropic"]
     replicate: Optional["GetSpecificationSpecificationReplicate"]
     tools: Optional[List["GetSpecificationSpecificationTools"]]
 
 
 class GetSpecificationSpecificationOwner(BaseModel):
     id: str
@@ -97,14 +103,24 @@
     key: Optional[str]
     endpoint: Optional[Any]
     deployment_name: Optional[str] = Field(alias="deploymentName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
+class GetSpecificationSpecificationCohere(BaseModel):
+    token_limit: Optional[int] = Field(alias="tokenLimit")
+    completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
+    model: CohereModels
+    key: Optional[str]
+    model_name: Optional[str] = Field(alias="modelName")
+    temperature: Optional[float]
+    probability: Optional[float]
+
+
 class GetSpecificationSpecificationAnthropic(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: AnthropicModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240505001/graphlit_api/get_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 class GetWorkflowWorkflowExtractionJobsConnectorAzureImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
 
 
 class GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
     detail_level: Optional[OpenAIVisionDetailLevels] = Field(alias="detailLevel")
+    custom_instructions: Optional[str] = Field(alias="customInstructions")
 
 
 class GetWorkflowWorkflowExtractionJobsConnectorModelText(BaseModel):
     specification: Optional[
         "GetWorkflowWorkflowExtractionJobsConnectorModelTextSpecification"
     ]
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240505001/graphlit_api/ingest_encoded_file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ContentTypes, EntityState, FileTypes
 
 
@@ -19,10 +19,19 @@
     id: str
     name: str
     state: EntityState
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
     mime_type: Optional[str] = Field(alias="mimeType")
     uri: Optional[Any]
+    collections: Optional[
+        List[Optional["IngestEncodedFileIngestEncodedFileCollections"]]
+    ]
+
+
+class IngestEncodedFileIngestEncodedFileCollections(BaseModel):
+    id: str
+    name: str
 
 
 IngestEncodedFile.model_rebuild()
+IngestEncodedFileIngestEncodedFile.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240505001/graphlit_api/ingest_text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ContentTypes, EntityState, FileTypes
 
 
@@ -17,10 +17,17 @@
     id: str
     name: str
     state: EntityState
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
     mime_type: Optional[str] = Field(alias="mimeType")
     uri: Optional[Any]
+    collections: Optional[List[Optional["IngestTextIngestTextCollections"]]]
+
+
+class IngestTextIngestTextCollections(BaseModel):
+    id: str
+    name: str
 
 
 IngestText.model_rebuild()
+IngestTextIngestText.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240505001/graphlit_api/ingest_uri.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ContentTypes, EntityState, FileTypes
 
 
@@ -17,10 +17,17 @@
     id: str
     name: str
     state: EntityState
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
     mime_type: Optional[str] = Field(alias="mimeType")
     uri: Optional[Any]
+    collections: Optional[List[Optional["IngestUriIngestUriCollections"]]]
+
+
+class IngestUriIngestUriCollections(BaseModel):
+    id: str
+    name: str
 
 
 IngestUri.model_rebuild()
+IngestUriIngestUri.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/input_types.py` & `graphlit_client-1.0.20240505001/graphlit_api/input_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,33 @@
     FeedListingTypes,
     FeedServiceTypes,
     FeedTypes,
     FilePreparationServiceTypes,
     FileTypes,
     GroqModels,
     H3ResolutionTypes,
+    ImageProjectionTypes,
     IntegrationServiceTypes,
     LabelFacetTypes,
     LinkTypes,
+    MailImportance,
+    MailPriority,
+    MailSensitivity,
     MetadataTypes,
     MistralModels,
     ModelServiceTypes,
     NotionTypes,
     ObservableTypes,
     OccurrenceTypes,
     OpenAIModels,
     OpenAIVisionDetailLevels,
     OrderByTypes,
     OrderDirectionTypes,
     OrganizationFacetTypes,
+    OrientationTypes,
     PersonFacetTypes,
     PlaceFacetTypes,
     PolicyTimeTypes,
     ProductFacetTypes,
     PromptStrategyTypes,
     ReplicateModels,
     RepoFacetTypes,
@@ -64,14 +69,15 @@
     SearchTypes,
     SharePointAuthenticationTypes,
     SoftwareFacetTypes,
     SpecificationTypes,
     SummarizationTypes,
     TimedPolicyRecurrenceTypes,
     TimeIntervalTypes,
+    UnitTypes,
     YouTubeTypes,
 )
 
 
 class AlertFilter(BaseModel):
     search: Optional[str] = None
     order_by: Optional[OrderByTypes] = Field(alias="orderBy", default=None)
@@ -513,14 +519,17 @@
     issue: Optional["IssueFeedPropertiesInput"] = None
     rss: Optional["RSSFeedPropertiesInput"] = None
     web: Optional["WebFeedPropertiesInput"] = None
     reddit: Optional["RedditFeedPropertiesInput"] = None
     youtube: Optional["YouTubeFeedPropertiesInput"] = None
     notion: Optional["NotionFeedPropertiesInput"] = None
     slack: Optional["SlackFeedPropertiesInput"] = None
+    microsoft_teams: Optional["MicrosoftTeamsFeedPropertiesInput"] = Field(
+        alias="microsoftTeams", default=None
+    )
     discord: Optional["DiscordFeedPropertiesInput"] = None
     schedule_policy: Optional["FeedSchedulePolicyInput"] = Field(
         alias="schedulePolicy", default=None
     )
     workflow: Optional["EntityReferenceInput"] = None
 
 
@@ -751,14 +760,17 @@
     issue: Optional["IssueFeedPropertiesUpdateInput"] = None
     rss: Optional["RSSFeedPropertiesUpdateInput"] = None
     web: Optional["WebFeedPropertiesUpdateInput"] = None
     reddit: Optional["RedditFeedPropertiesUpdateInput"] = None
     youtube: Optional["YouTubeFeedPropertiesUpdateInput"] = None
     notion: Optional["NotionFeedPropertiesUpdateInput"] = None
     slack: Optional["SlackFeedPropertiesUpdateInput"] = None
+    microsoft_teams: Optional["MicrosoftTeamsFeedPropertiesUpdateInput"] = Field(
+        alias="microsoftTeams", default=None
+    )
     discord: Optional["DiscordFeedPropertiesUpdateInput"] = None
     schedule_policy: Optional["FeedSchedulePolicyInput"] = Field(
         alias="schedulePolicy", default=None
     )
     workflow: Optional["EntityReferenceInput"] = None
 
 
@@ -1093,14 +1105,23 @@
     channel: str
     include_attachments: Optional[bool] = Field(
         alias="includeAttachments", default=None
     )
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
+class MicrosoftTeamsFeedPropertiesInput(BaseModel):
+    type: Optional[FeedListingTypes] = None
+    tenant_id: str = Field(alias="tenantId")
+    refresh_token: str = Field(alias="refreshToken")
+    team: str
+    channel: str
+    read_limit: Optional[int] = Field(alias="readLimit", default=None)
+
+
 class DiscordFeedPropertiesInput(BaseModel):
     type: Optional[FeedListingTypes] = None
     token: str
     channel: str
     include_attachments: Optional[bool] = Field(
         alias="includeAttachments", default=None
     )
@@ -1371,14 +1392,23 @@
     channel: Optional[str] = None
     include_attachments: Optional[bool] = Field(
         alias="includeAttachments", default=None
     )
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
+class MicrosoftTeamsFeedPropertiesUpdateInput(BaseModel):
+    type: Optional[FeedListingTypes] = None
+    tenant_id: Optional[str] = Field(alias="tenantId", default=None)
+    refresh_token: Optional[str] = Field(alias="refreshToken", default=None)
+    team: str
+    channel: str
+    read_limit: Optional[int] = Field(alias="readLimit", default=None)
+
+
 class DiscordFeedPropertiesUpdateInput(BaseModel):
     type: Optional[FeedListingTypes] = None
     token: Optional[str] = None
     channel: Optional[str] = None
     include_attachments: Optional[bool] = Field(
         alias="includeAttachments", default=None
     )
@@ -1846,14 +1876,18 @@
     time_interval: Optional[TimeIntervalTypes] = Field(
         alias="timeInterval", default=None
     )
     time_offset: Optional[int] = Field(alias="timeOffset", default=None)
     facet: Optional[ContentFacetTypes] = None
 
 
+class ContentGraphInput(BaseModel):
+    types: Optional[List[Optional[ObservableTypes]]] = None
+
+
 class EventFacetInput(BaseModel):
     time_interval: Optional[TimeIntervalTypes] = Field(
         alias="timeInterval", default=None
     )
     time_offset: Optional[int] = Field(alias="timeOffset", default=None)
     facet: Optional[EventFacetTypes] = None
 
@@ -1922,7 +1956,187 @@
     facet: Optional[SoftwareFacetTypes] = None
 
 
 class ContentUpdateInput(BaseModel):
     id: str
     name: Optional[str] = None
     description: Optional[str] = None
+    video: Optional["VideoMetadataInput"] = None
+    audio: Optional["AudioMetadataInput"] = None
+    image: Optional["ImageMetadataInput"] = None
+    document: Optional["DocumentMetadataInput"] = None
+    email: Optional["EmailMetadataInput"] = None
+    issue: Optional["IssueMetadataInput"] = None
+    drawing: Optional["DrawingMetadataInput"] = None
+    shape: Optional["ShapeMetadataInput"] = None
+    geometry: Optional["GeometryMetadataInput"] = None
+    point_cloud: Optional["PointCloudMetadataInput"] = Field(
+        alias="pointCloud", default=None
+    )
+    package: Optional["PackageMetadataInput"] = None
+
+
+class VideoMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    width: Optional[int] = None
+    height: Optional[int] = None
+    duration: Optional[str] = None
+    software: Optional[str] = None
+    make: Optional[str] = None
+    model: Optional[str] = None
+
+
+class AudioMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    keywords: Optional[List[Optional[str]]] = None
+    author: Optional[str] = None
+    series: Optional[str] = None
+    episode: Optional[str] = None
+    episode_type: Optional[str] = Field(alias="episodeType", default=None)
+    season: Optional[str] = None
+    publisher: Optional[str] = None
+    copyright: Optional[str] = None
+    language: Optional[str] = None
+    genre: Optional[str] = None
+    title: Optional[str] = None
+    bitrate: Optional[int] = None
+    channels: Optional[int] = None
+    sample_rate: Optional[int] = Field(alias="sampleRate", default=None)
+    bits_per_sample: Optional[int] = Field(alias="bitsPerSample", default=None)
+    duration: Optional[str] = None
+
+
+class ImageMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    width: Optional[int] = None
+    height: Optional[int] = None
+    bits_per_component: Optional[int] = Field(alias="bitsPerComponent", default=None)
+    components: Optional[int] = None
+    projection_type: Optional[ImageProjectionTypes] = Field(
+        alias="projectionType", default=None
+    )
+    orientation: Optional[OrientationTypes] = None
+    resolution_x: Optional[int] = Field(alias="resolutionX", default=None)
+    resolution_y: Optional[int] = Field(alias="resolutionY", default=None)
+    description: Optional[str] = None
+    software: Optional[str] = None
+    identifier: Optional[str] = None
+    make: Optional[str] = None
+    model: Optional[str] = None
+    lens: Optional[str] = None
+    lens_specification: Optional[str] = Field(alias="lensSpecification", default=None)
+    focal_length: Optional[float] = Field(alias="focalLength", default=None)
+    exposure_time: Optional[str] = Field(alias="exposureTime", default=None)
+    f_number: Optional[str] = Field(alias="fNumber", default=None)
+    iso: Optional[str] = None
+    color_space: Optional[str] = Field(alias="colorSpace", default=None)
+    heading: Optional[float] = None
+    pitch: Optional[float] = None
+
+
+class DocumentMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    title: Optional[str] = None
+    subject: Optional[str] = None
+    author: Optional[str] = None
+    software: Optional[str] = None
+    publisher: Optional[str] = None
+    description: Optional[str] = None
+    summary: Optional[str] = None
+    comments: Optional[str] = None
+    identifier: Optional[str] = None
+    keywords: Optional[List[Optional[str]]] = None
+    links: Optional[List[Optional[Any]]] = None
+    page_count: Optional[int] = Field(alias="pageCount", default=None)
+    worksheet_count: Optional[int] = Field(alias="worksheetCount", default=None)
+    slide_count: Optional[int] = Field(alias="slideCount", default=None)
+    word_count: Optional[int] = Field(alias="wordCount", default=None)
+    line_count: Optional[int] = Field(alias="lineCount", default=None)
+    paragraph_count: Optional[int] = Field(alias="paragraphCount", default=None)
+    character_count: Optional[int] = Field(alias="characterCount", default=None)
+    total_editing_time: Optional[str] = Field(alias="totalEditingTime", default=None)
+    is_encrypted: Optional[bool] = Field(alias="isEncrypted", default=None)
+    has_digital_signature: Optional[bool] = Field(
+        alias="hasDigitalSignature", default=None
+    )
+
+
+class EmailMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    subject: Optional[str] = None
+    identifier: Optional[str] = None
+    sensitivity: Optional[MailSensitivity] = None
+    priority: Optional[MailPriority] = None
+    importance: Optional[MailImportance] = None
+    labels: Optional[List[Optional[str]]] = None
+    links: Optional[List[Optional[Any]]] = None
+
+
+class IssueMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    title: Optional[str] = None
+    project: Optional[str] = None
+    team: Optional[str] = None
+    status: Optional[str] = None
+    priority: Optional[str] = None
+    type: Optional[str] = None
+    identifier: Optional[str] = None
+    labels: Optional[List[Optional[str]]] = None
+    links: Optional[List[Optional[Any]]] = None
+
+
+class DrawingMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    x: Optional[float] = None
+    y: Optional[float] = None
+    width: Optional[float] = None
+    height: Optional[float] = None
+    depth: Optional[float] = None
+    unit_type: Optional[UnitTypes] = Field(alias="unitType", default=None)
+
+
+class ShapeMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    feature_count: Optional[int] = Field(alias="featureCount", default=None)
+    attribute_count: Optional[int] = Field(alias="attributeCount", default=None)
+
+
+class GeometryMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    triangle_count: Optional[Any] = Field(alias="triangleCount", default=None)
+    vertex_count: Optional[Any] = Field(alias="vertexCount", default=None)
+
+
+class PointCloudMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    software: Optional[str] = None
+    description: Optional[str] = None
+    identifier: Optional[str] = None
+    point_count: Optional[Any] = Field(alias="pointCount", default=None)
+
+
+class PackageMetadataInput(BaseModel):
+    creation_date: Optional[Any] = Field(alias="creationDate", default=None)
+    modified_date: Optional[Any] = Field(alias="modifiedDate", default=None)
+    location: Optional["PointInput"] = None
+    file_count: Optional[int] = Field(alias="fileCount", default=None)
+    folder_count: Optional[int] = Field(alias="folderCount", default=None)
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_credits.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
-class LookupCredits(BaseModel):
-    lookup_credits: Optional["LookupCreditsLookupCredits"] = Field(
-        alias="lookupCredits"
-    )
+class QueryCredits(BaseModel):
+    credits: Optional[List[Optional["QueryCreditsCredits"]]]
 
 
-class LookupCreditsLookupCredits(BaseModel):
+class QueryCreditsCredits(BaseModel):
     correlation_id: Optional[str] = Field(alias="correlationId")
     owner_id: Optional[str] = Field(alias="ownerId")
     credits: Optional[Any]
     storage_ratio: Optional[Any] = Field(alias="storageRatio")
     compute_ratio: Optional[Any] = Field(alias="computeRatio")
     preparation_ratio: Optional[Any] = Field(alias="preparationRatio")
     extraction_ratio: Optional[Any] = Field(alias="extractionRatio")
     enrichment_ratio: Optional[Any] = Field(alias="enrichmentRatio")
     publishing_ratio: Optional[Any] = Field(alias="publishingRatio")
     search_ratio: Optional[Any] = Field(alias="searchRatio")
     conversation_ratio: Optional[Any] = Field(alias="conversationRatio")
 
 
-LookupCredits.model_rebuild()
+QueryCredits.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240505001/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/operations.py` & `graphlit_client-1.0.20240505001/graphlit_api/operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
 __all__ = [
     "ADD_CONTENTS_TO_COLLECTIONS_GQL",
     "CLEAR_CONVERSATION_GQL",
     "CLOSE_CONVERSATION_GQL",
+    "COUNT_ALERTS_GQL",
+    "COUNT_CATEGORIES_GQL",
+    "COUNT_COLLECTIONS_GQL",
+    "COUNT_CONTENTS_GQL",
+    "COUNT_CONVERSATIONS_GQL",
+    "COUNT_EVENTS_GQL",
+    "COUNT_FEEDS_GQL",
+    "COUNT_LABELS_GQL",
+    "COUNT_ORGANIZATIONS_GQL",
+    "COUNT_PERSONS_GQL",
+    "COUNT_PLACES_GQL",
+    "COUNT_PRODUCTS_GQL",
+    "COUNT_REPOS_GQL",
+    "COUNT_SOFTWARES_GQL",
+    "COUNT_SPECIFICATIONS_GQL",
+    "COUNT_WORKFLOWS_GQL",
     "CREATE_ALERT_GQL",
     "CREATE_CATEGORY_GQL",
     "CREATE_COLLECTION_GQL",
     "CREATE_CONVERSATION_GQL",
     "CREATE_EVENT_GQL",
     "CREATE_FEED_GQL",
     "CREATE_LABEL_GQL",
@@ -17,15 +33,14 @@
     "CREATE_PERSON_GQL",
     "CREATE_PLACE_GQL",
     "CREATE_PRODUCT_GQL",
     "CREATE_REPO_GQL",
     "CREATE_SOFTWARE_GQL",
     "CREATE_SPECIFICATION_GQL",
     "CREATE_WORKFLOW_GQL",
-    "CREDITS_GQL",
     "DELETE_ALERTS_GQL",
     "DELETE_ALERT_GQL",
     "DELETE_ALL_ALERTS_GQL",
     "DELETE_ALL_CATEGORIES_GQL",
     "DELETE_ALL_COLLECTIONS_GQL",
     "DELETE_ALL_CONTENTS_GQL",
     "DELETE_ALL_CONVERSATIONS_GQL",
@@ -34,14 +49,15 @@
     "DELETE_ALL_LABELS_GQL",
     "DELETE_ALL_ORGANIZATIONS_GQL",
     "DELETE_ALL_PERSONS_GQL",
     "DELETE_ALL_PLACES_GQL",
     "DELETE_ALL_PRODUCTS_GQL",
     "DELETE_ALL_REPOS_GQL",
     "DELETE_ALL_SOFTWARES_GQL",
+    "DELETE_ALL_SPECIFICATIONS_GQL",
     "DELETE_ALL_WORKFLOWS_GQL",
     "DELETE_CATEGORIES_GQL",
     "DELETE_CATEGORY_GQL",
     "DELETE_COLLECTIONS_GQL",
     "DELETE_COLLECTION_GQL",
     "DELETE_CONTENTS_GQL",
     "DELETE_CONTENT_GQL",
@@ -62,14 +78,15 @@
     "DELETE_PLACE_GQL",
     "DELETE_PRODUCTS_GQL",
     "DELETE_PRODUCT_GQL",
     "DELETE_REPOS_GQL",
     "DELETE_REPO_GQL",
     "DELETE_SOFTWARES_GQL",
     "DELETE_SOFTWARE_GQL",
+    "DELETE_SPECIFICATIONS_GQL",
     "DELETE_SPECIFICATION_GQL",
     "DELETE_WORKFLOWS_GQL",
     "DELETE_WORKFLOW_GQL",
     "DISABLE_ALERT_GQL",
     "DISABLE_FEED_GQL",
     "ENABLE_ALERT_GQL",
     "ENABLE_FEED_GQL",
@@ -102,27 +119,30 @@
     "PROMPT_SPECIFICATIONS_GQL",
     "PUBLISH_CONTENTS_GQL",
     "PUBLISH_CONVERSATION_GQL",
     "PUBLISH_TEXT_GQL",
     "QUERY_ALERTS_GQL",
     "QUERY_CATEGORIES_GQL",
     "QUERY_COLLECTIONS_GQL",
+    "QUERY_CONTENTS_FACETS_GQL",
     "QUERY_CONTENTS_GQL",
-    "QUERY_CONTENT_FACETS_GQL",
+    "QUERY_CONTENTS_GRAPH_GQL",
     "QUERY_CONVERSATIONS_GQL",
+    "QUERY_CREDITS_GQL",
     "QUERY_EVENTS_GQL",
     "QUERY_FEEDS_GQL",
     "QUERY_LABELS_GQL",
     "QUERY_ORGANIZATIONS_GQL",
     "QUERY_PERSONS_GQL",
     "QUERY_PLACES_GQL",
     "QUERY_PRODUCTS_GQL",
     "QUERY_REPOS_GQL",
     "QUERY_SOFTWARES_GQL",
     "QUERY_SPECIFICATIONS_GQL",
+    "QUERY_USAGE_GQL",
     "QUERY_WORKFLOWS_GQL",
     "REMOVE_CONTENTS_FROM_COLLECTION_GQL",
     "SUGGEST_CONVERSATION_GQL",
     "SUMMARIZE_CONTENTS_GQL",
     "UPDATE_ALERT_GQL",
     "UPDATE_CATEGORY_GQL",
     "UPDATE_COLLECTION_GQL",
@@ -137,17 +157,24 @@
     "UPDATE_PLACE_GQL",
     "UPDATE_PRODUCT_GQL",
     "UPDATE_PROJECT_GQL",
     "UPDATE_REPO_GQL",
     "UPDATE_SOFTWARE_GQL",
     "UPDATE_SPECIFICATION_GQL",
     "UPDATE_WORKFLOW_GQL",
-    "USAGE_GQL",
 ]
 
+COUNT_ALERTS_GQL = """
+query CountAlerts($filter: AlertFilter) {
+  countAlerts(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_ALERT_GQL = """
 mutation CreateAlert($alert: AlertInput!, $correlationId: String) {
   createAlert(alert: $alert, correlationId: $correlationId) {
     id
     name
     state
     type
@@ -161,25 +188,29 @@
     id
     state
   }
 }
 """
 
 DELETE_ALERTS_GQL = """
-mutation DeleteAlerts($ids: [ID!]!) {
-  deleteAlerts(ids: $ids) {
+mutation DeleteAlerts($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteAlerts(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 DELETE_ALL_ALERTS_GQL = """
-mutation DeleteAllAlerts {
-  deleteAllAlerts {
+mutation DeleteAllAlerts($filter: AlertFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllAlerts(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DISABLE_ALERT_GQL = """
@@ -351,35 +382,47 @@
     name
     state
     type
   }
 }
 """
 
+COUNT_CATEGORIES_GQL = """
+query CountCategories($filter: CategoryFilter) {
+  countCategories(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_CATEGORY_GQL = """
 mutation CreateCategory($category: CategoryInput!) {
   createCategory(category: $category) {
     id
     name
   }
 }
 """
 
 DELETE_ALL_CATEGORIES_GQL = """
-mutation DeleteAllCategories($filter: CategoryFilter!) {
-  deleteAllCategories(filter: $filter) {
+mutation DeleteAllCategories($filter: CategoryFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllCategories(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_CATEGORIES_GQL = """
-mutation DeleteCategories($ids: [ID!]!) {
-  deleteCategories(ids: $ids) {
+mutation DeleteCategories($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteCategories(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 DELETE_CATEGORY_GQL = """
@@ -399,15 +442,15 @@
     description
     creationDate
   }
 }
 """
 
 QUERY_CATEGORIES_GQL = """
-query QueryCategories($filter: CategoryFilter!) {
+query QueryCategories($filter: CategoryFilter) {
   categories(filter: $filter) {
     results {
       id
       name
       description
       creationDate
     }
@@ -435,28 +478,40 @@
       id
       name
     }
   }
 }
 """
 
+COUNT_COLLECTIONS_GQL = """
+query CountCollections($filter: CollectionFilter) {
+  countCollections(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_COLLECTION_GQL = """
 mutation CreateCollection($collection: CollectionInput!) {
   createCollection(collection: $collection) {
     id
     name
     state
     type
   }
 }
 """
 
 DELETE_ALL_COLLECTIONS_GQL = """
-mutation DeleteAllCollections {
-  deleteAllCollections {
+mutation DeleteAllCollections($filter: CollectionFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllCollections(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_COLLECTION_GQL = """
@@ -465,16 +520,16 @@
     id
     state
   }
 }
 """
 
 DELETE_COLLECTIONS_GQL = """
-mutation DeleteCollections($ids: [ID!]!) {
-  deleteCollections(ids: $ids) {
+mutation DeleteCollections($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteCollections(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_COLLECTION_GQL = """
@@ -539,17 +594,29 @@
     name
     state
     type
   }
 }
 """
 
+COUNT_CONTENTS_GQL = """
+query CountContents($filter: ContentFilter) {
+  countContents(filter: $filter) {
+    count
+  }
+}
+"""
+
 DELETE_ALL_CONTENTS_GQL = """
-mutation DeleteAllContents {
-  deleteAllContents {
+mutation DeleteAllContents($filter: ContentFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllContents(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_CONTENT_GQL = """
@@ -558,16 +625,16 @@
     id
     state
   }
 }
 """
 
 DELETE_CONTENTS_GQL = """
-mutation DeleteContents($ids: [ID!]!) {
-  deleteContents(ids: $ids) {
+mutation DeleteContents($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteContents(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 EXTRACT_CONTENTS_GQL = """
@@ -594,169 +661,226 @@
 """
 
 GET_CONTENT_GQL = """
 query GetContent($id: ID!) {
   content(id: $id) {
     id
     name
-    description
     creationDate
     owner {
       id
     }
     state
     originalDate
     finishedDate
     workflowDuration
     uri
+    description
+    markdown
+    address {
+      streetAddress
+      city
+      region
+      country
+      postalCode
+    }
+    location {
+      latitude
+      longitude
+    }
     type
     fileType
     mimeType
     fileName
     fileSize
     masterUri
     imageUri
     textUri
     audioUri
     transcriptUri
     video {
       width
       height
       duration
-      software
       make
       model
+      software
+      title
+      description
+      keywords
+      author
     }
     audio {
       keywords
       author
       series
       episode
       episodeType
       season
       publisher
       copyright
       language
       genre
       title
+      description
       bitrate
       channels
       sampleRate
       bitsPerSample
       duration
     }
     image {
       width
       height
+      resolutionX
+      resolutionY
+      bitsPerComponent
+      components
+      projectionType
+      orientation
       description
-      software
-      identifier
       make
       model
+      software
+      lens
+      focalLength
+      exposureTime
+      fNumber
+      iso
+      heading
+      pitch
     }
     document {
       title
       subject
+      summary
       author
-      software
       publisher
       description
-      summary
       keywords
       pageCount
       worksheetCount
       slideCount
       wordCount
       lineCount
       paragraphCount
-      characterCount
       isEncrypted
       hasDigitalSignature
     }
     email {
-      subject
       identifier
+      subject
+      labels
       sensitivity
       priority
       importance
-      labels
       from {
         name
-        familyName
-        givenName
         email
+        givenName
+        familyName
       }
       to {
         name
-        familyName
-        givenName
         email
+        givenName
+        familyName
       }
       cc {
         name
-        familyName
-        givenName
         email
+        givenName
+        familyName
       }
       bcc {
         name
-        familyName
-        givenName
         email
+        givenName
+        familyName
       }
     }
     issue {
+      identifier
       title
       project
       team
       status
       priority
       type
-      identifier
       labels
     }
+    package {
+      fileCount
+      folderCount
+      isEncrypted
+    }
+    parent {
+      id
+      name
+    }
+    children {
+      id
+      name
+    }
+    feed {
+      id
+      name
+    }
+    collections {
+      id
+      name
+    }
+    links {
+      uri
+      linkType
+    }
     observations {
+      id
       type
       observable {
         id
         name
       }
       occurrences {
         type
         confidence
+        startTime
+        endTime
+        pageIndex
         boundingBox {
           left
           top
           width
           height
         }
-        pageIndex
-        startTime
-        endTime
       }
-    }
-    parent {
-      id
-    }
-    children {
-      id
-    }
-    collections {
-      id
-    }
-    feed {
-      id
+      state
     }
     workflow {
       id
+      name
     }
-    markdown
-    links {
-      uri
-      linkType
+    pages {
+      index
+      chunks {
+        index
+        pageIndex
+        rowIndex
+        columnIndex
+        confidence
+        text
+        role
+        relevance
+      }
+    }
+    segments {
+      startTime
+      endTime
+      text
+      relevance
     }
     error
   }
 }
 """
 
 INGEST_ENCODED_FILE_GQL = """
@@ -774,169 +898,345 @@
     id
     name
     state
     type
     fileType
     mimeType
     uri
+    collections {
+      id
+      name
+    }
   }
 }
 """
 
 INGEST_TEXT_GQL = """
-mutation IngestText($name: String!, $text: String!, $textType: TextTypes, $uri: URL, $id: ID, $isSynchronous: Boolean, $collections: [EntityReferenceInput!], $workflow: EntityReferenceInput, $correlationId: String) {
+mutation IngestText($name: String!, $text: String!, $textType: TextTypes, $uri: URL, $id: ID, $isSynchronous: Boolean, $workflow: EntityReferenceInput, $collections: [EntityReferenceInput!], $correlationId: String) {
   ingestText(
     name: $name
     text: $text
     textType: $textType
     uri: $uri
     id: $id
     isSynchronous: $isSynchronous
-    collections: $collections
     workflow: $workflow
+    collections: $collections
     correlationId: $correlationId
   ) {
     id
     name
     state
     type
     fileType
     mimeType
     uri
+    collections {
+      id
+      name
+    }
   }
 }
 """
 
 INGEST_URI_GQL = """
-mutation IngestUri($name: String, $uri: URL!, $id: ID, $isSynchronous: Boolean, $collections: [EntityReferenceInput!], $workflow: EntityReferenceInput, $correlationId: String) {
+mutation IngestUri($name: String, $uri: URL!, $id: ID, $isSynchronous: Boolean, $workflow: EntityReferenceInput, $collections: [EntityReferenceInput!], $correlationId: String) {
   ingestUri(
     name: $name
     uri: $uri
     id: $id
-    collections: $collections
     workflow: $workflow
+    collections: $collections
     isSynchronous: $isSynchronous
     correlationId: $correlationId
   ) {
     id
     name
     state
     type
     fileType
     mimeType
     uri
+    collections {
+      id
+      name
+    }
   }
 }
 """
 
 IS_CONTENT_DONE_GQL = """
 query IsContentDone($id: ID!) {
   isContentDone(id: $id) {
     result
   }
 }
 """
 
 PUBLISH_CONTENTS_GQL = """
-mutation PublishContents($summaryPrompt: String, $publishPrompt: String!, $connector: ContentPublishingConnectorInput!, $filter: ContentFilter, $correlationId: String, $name: String, $summarySpecification: EntityReferenceInput, $publishSpecification: EntityReferenceInput, $workflow: EntityReferenceInput, $isSynchronous: Boolean!) {
+mutation PublishContents($summaryPrompt: String, $publishPrompt: String!, $connector: ContentPublishingConnectorInput!, $filter: ContentFilter, $isSynchronous: Boolean, $correlationId: String, $name: String, $summarySpecification: EntityReferenceInput, $publishSpecification: EntityReferenceInput, $workflow: EntityReferenceInput) {
   publishContents(
     summaryPrompt: $summaryPrompt
     publishPrompt: $publishPrompt
     connector: $connector
     filter: $filter
+    isSynchronous: $isSynchronous
     correlationId: $correlationId
     name: $name
     summarySpecification: $summarySpecification
     publishSpecification: $publishSpecification
     workflow: $workflow
-    isSynchronous: $isSynchronous
   ) {
     id
     name
     state
     type
     fileType
     mimeType
     uri
+    collections {
+      id
+      name
+    }
     textUri
     audioUri
     markdown
   }
 }
 """
 
 PUBLISH_TEXT_GQL = """
-mutation PublishText($text: String!, $textType: TextTypes, $connector: ContentPublishingConnectorInput!, $correlationId: String, $name: String, $workflow: EntityReferenceInput, $isSynchronous: Boolean!) {
+mutation PublishText($text: String!, $textType: TextTypes, $connector: ContentPublishingConnectorInput!, $isSynchronous: Boolean, $correlationId: String, $name: String, $workflow: EntityReferenceInput) {
   publishText(
     text: $text
     textType: $textType
     connector: $connector
+    isSynchronous: $isSynchronous
     correlationId: $correlationId
     name: $name
     workflow: $workflow
-    isSynchronous: $isSynchronous
   ) {
     id
     name
     state
     type
     fileType
     mimeType
     uri
+    collections {
+      id
+      name
+    }
     textUri
     audioUri
     markdown
   }
 }
 """
 
-QUERY_CONTENT_FACETS_GQL = """
-query QueryContentFacets($filter: ContentFilter, $facets: [ContentFacetInput!]) {
-  contents(filter: $filter, facets: $facets) {
-    facets {
-      facet
-      type
-      observable {
-        type
-        observable {
-          id
-          name
-        }
-      }
-      count
-    }
-  }
-}
-"""
-
 QUERY_CONTENTS_GQL = """
-query QueryContents($filter: ContentFilter) {
+query QueryContents($filter: ContentFilter!) {
   contents(filter: $filter) {
     results {
       id
       name
       creationDate
       owner {
         id
       }
       state
       originalDate
       finishedDate
       workflowDuration
       uri
+      description
+      markdown
+      address {
+        streetAddress
+        city
+        region
+        country
+        postalCode
+      }
+      location {
+        latitude
+        longitude
+      }
       type
       fileType
       mimeType
       fileName
       fileSize
       masterUri
       imageUri
       textUri
       audioUri
       transcriptUri
+      video {
+        width
+        height
+        duration
+        make
+        model
+        software
+        title
+        description
+        keywords
+        author
+      }
+      audio {
+        keywords
+        author
+        series
+        episode
+        episodeType
+        season
+        publisher
+        copyright
+        language
+        genre
+        title
+        description
+        bitrate
+        channels
+        sampleRate
+        bitsPerSample
+        duration
+      }
+      image {
+        width
+        height
+        resolutionX
+        resolutionY
+        bitsPerComponent
+        components
+        projectionType
+        orientation
+        description
+        make
+        model
+        software
+        lens
+        focalLength
+        exposureTime
+        fNumber
+        iso
+        heading
+        pitch
+      }
+      document {
+        title
+        subject
+        summary
+        author
+        publisher
+        description
+        keywords
+        pageCount
+        worksheetCount
+        slideCount
+        wordCount
+        lineCount
+        paragraphCount
+        isEncrypted
+        hasDigitalSignature
+      }
+      email {
+        identifier
+        subject
+        labels
+        sensitivity
+        priority
+        importance
+        from {
+          name
+          email
+          givenName
+          familyName
+        }
+        to {
+          name
+          email
+          givenName
+          familyName
+        }
+        cc {
+          name
+          email
+          givenName
+          familyName
+        }
+        bcc {
+          name
+          email
+          givenName
+          familyName
+        }
+      }
+      issue {
+        identifier
+        title
+        project
+        team
+        status
+        priority
+        type
+        labels
+      }
+      package {
+        fileCount
+        folderCount
+        isEncrypted
+      }
+      parent {
+        id
+        name
+      }
+      children {
+        id
+        name
+      }
+      feed {
+        id
+        name
+      }
+      collections {
+        id
+        name
+      }
+      links {
+        uri
+        linkType
+      }
+      observations {
+        id
+        type
+        observable {
+          id
+          name
+        }
+        occurrences {
+          type
+          confidence
+          startTime
+          endTime
+          pageIndex
+          boundingBox {
+            left
+            top
+            width
+            height
+          }
+        }
+        state
+      }
+      workflow {
+        id
+        name
+      }
       pages {
         index
         chunks {
           index
           pageIndex
           rowIndex
           columnIndex
@@ -948,151 +1248,276 @@
       }
       segments {
         startTime
         endTime
         text
         relevance
       }
+      error
+    }
+  }
+}
+"""
+
+QUERY_CONTENTS_FACETS_GQL = """
+query QueryContentsFacets($filter: ContentFilter!, $facets: [ContentFacetInput!]) {
+  contents(filter: $filter, facets: $facets) {
+    results {
+      id
+      name
+      creationDate
+      owner {
+        id
+      }
+      state
+      originalDate
+      finishedDate
+      workflowDuration
+      uri
+      description
+      markdown
+      address {
+        streetAddress
+        city
+        region
+        country
+        postalCode
+      }
+      location {
+        latitude
+        longitude
+      }
+      type
+      fileType
+      mimeType
+      fileName
+      fileSize
+      masterUri
+      imageUri
+      textUri
+      audioUri
+      transcriptUri
       video {
         width
         height
         duration
-        software
         make
         model
+        software
+        title
+        description
+        keywords
+        author
       }
       audio {
         keywords
         author
         series
         episode
         episodeType
         season
         publisher
         copyright
         language
         genre
         title
+        description
         bitrate
         channels
         sampleRate
         bitsPerSample
         duration
       }
       image {
         width
         height
+        resolutionX
+        resolutionY
+        bitsPerComponent
+        components
+        projectionType
+        orientation
         description
-        software
-        identifier
         make
         model
+        software
+        lens
+        focalLength
+        exposureTime
+        fNumber
+        iso
+        heading
+        pitch
       }
       document {
         title
         subject
+        summary
         author
-        software
         publisher
         description
-        summary
         keywords
         pageCount
         worksheetCount
         slideCount
         wordCount
         lineCount
         paragraphCount
-        characterCount
         isEncrypted
         hasDigitalSignature
       }
       email {
-        subject
         identifier
+        subject
+        labels
         sensitivity
         priority
         importance
-        labels
         from {
           name
-          familyName
-          givenName
           email
+          givenName
+          familyName
         }
         to {
           name
-          familyName
-          givenName
           email
+          givenName
+          familyName
         }
         cc {
           name
-          familyName
-          givenName
           email
+          givenName
+          familyName
         }
         bcc {
           name
-          familyName
-          givenName
           email
+          givenName
+          familyName
         }
       }
       issue {
+        identifier
         title
         project
         team
         status
         priority
         type
-        identifier
         labels
       }
+      package {
+        fileCount
+        folderCount
+        isEncrypted
+      }
+      parent {
+        id
+        name
+      }
+      children {
+        id
+        name
+      }
+      feed {
+        id
+        name
+      }
+      collections {
+        id
+        name
+      }
+      links {
+        uri
+        linkType
+      }
       observations {
+        id
         type
         observable {
           id
           name
         }
         occurrences {
           type
           confidence
+          startTime
+          endTime
+          pageIndex
           boundingBox {
             left
             top
             width
             height
           }
-          pageIndex
-          startTime
-          endTime
         }
+        state
       }
-      parent {
+      workflow {
         id
+        name
       }
-      children {
-        id
+      pages {
+        index
+        chunks {
+          index
+          pageIndex
+          rowIndex
+          columnIndex
+          confidence
+          text
+          role
+          relevance
+        }
       }
-      collections {
-        id
+      segments {
+        startTime
+        endTime
+        text
+        relevance
       }
-      feed {
-        id
+      error
+    }
+    facets {
+      facet
+      count
+      type
+      value
+      range {
+        from
+        to
       }
-      workflow {
+      observable {
+        type
+        observable {
+          id
+          name
+        }
+      }
+    }
+  }
+}
+"""
+
+QUERY_CONTENTS_GRAPH_GQL = """
+query QueryContentsGraph($filter: ContentFilter!, $graph: ContentGraphInput) {
+  contents(filter: $filter, graph: $graph) {
+    graph {
+      nodes {
         id
+        name
+        type
+        metadata
       }
-      markdown
-      links {
-        uri
-        linkType
+      edges {
+        from
+        to
       }
-      error
     }
   }
 }
 """
 
 SUMMARIZE_CONTENTS_GQL = """
 mutation SummarizeContents($summarizations: [SummarizationStrategyInput!]!, $filter: ContentFilter, $correlationId: String) {
@@ -1124,14 +1549,18 @@
     id
     name
     state
     type
     fileType
     mimeType
     uri
+    collections {
+      id
+      name
+    }
   }
 }
 """
 
 CLEAR_CONVERSATION_GQL = """
 mutation ClearConversation($id: ID!) {
   clearConversation(id: $id) {
@@ -1150,28 +1579,40 @@
     name
     state
     type
   }
 }
 """
 
+COUNT_CONVERSATIONS_GQL = """
+query CountConversations($filter: ConversationFilter) {
+  countConversations(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_CONVERSATION_GQL = """
 mutation CreateConversation($conversation: ConversationInput!, $correlationId: String) {
   createConversation(conversation: $conversation, correlationId: $correlationId) {
     id
     name
     state
     type
   }
 }
 """
 
 DELETE_ALL_CONVERSATIONS_GQL = """
-mutation DeleteAllConversations {
-  deleteAllConversations {
+mutation DeleteAllConversations($filter: ConversationFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllConversations(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_CONVERSATION_GQL = """
@@ -1180,16 +1621,16 @@
     id
     state
   }
 }
 """
 
 DELETE_CONVERSATIONS_GQL = """
-mutation DeleteConversations($ids: [ID!]!) {
-  deleteConversations(ids: $ids) {
+mutation DeleteConversations($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteConversations(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_CONVERSATION_GQL = """
@@ -1207,14 +1648,21 @@
     messages {
       role
       author
       message
       citations {
         content {
           id
+          name
+          state
+          type
+          fileType
+          fileName
+          originalDate
+          uri
         }
         index
         text
         startTime
         endTime
         pageNumber
         frameNumber
@@ -1275,17 +1723,20 @@
       role
       author
       message
       citations {
         content {
           id
           name
+          state
           type
           fileType
           fileName
+          originalDate
+          uri
         }
         index
         text
         startTime
         endTime
         pageNumber
         frameNumber
@@ -1316,29 +1767,34 @@
       }
     }
   }
 }
 """
 
 PUBLISH_CONVERSATION_GQL = """
-mutation PublishConversation($id: ID!, $connector: ContentPublishingConnectorInput!, $name: String, $workflow: EntityReferenceInput, $correlationId: String) {
+mutation PublishConversation($id: ID!, $connector: ContentPublishingConnectorInput!, $name: String, $isSynchronous: Boolean, $workflow: EntityReferenceInput, $correlationId: String) {
   publishConversation(
     id: $id
     connector: $connector
     name: $name
+    isSynchronous: $isSynchronous
     workflow: $workflow
     correlationId: $correlationId
   ) {
     id
     name
     state
     type
     fileType
     mimeType
     uri
+    collections {
+      id
+      name
+    }
     textUri
     audioUri
     markdown
   }
 }
 """
 
@@ -1358,14 +1814,21 @@
       messages {
         role
         author
         message
         citations {
           content {
             id
+            name
+            state
+            type
+            fileType
+            fileName
+            originalDate
+            uri
           }
           index
           text
           startTime
           endTime
           pageNumber
           frameNumber
@@ -1432,26 +1895,38 @@
     name
     state
     type
   }
 }
 """
 
+COUNT_EVENTS_GQL = """
+query CountEvents($filter: EventFilter) {
+  countEvents(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_EVENT_GQL = """
 mutation CreateEvent($event: EventInput!) {
   createEvent(event: $event) {
     id
     name
   }
 }
 """
 
 DELETE_ALL_EVENTS_GQL = """
-mutation DeleteAllEvents($filter: EventFilter!) {
-  deleteAllEvents(filter: $filter) {
+mutation DeleteAllEvents($filter: EventFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllEvents(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_EVENT_GQL = """
@@ -1460,16 +1935,16 @@
     id
     state
   }
 }
 """
 
 DELETE_EVENTS_GQL = """
-mutation DeleteEvents($ids: [ID!]!) {
-  deleteEvents(ids: $ids) {
+mutation DeleteEvents($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteEvents(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_EVENT_GQL = """
@@ -1497,15 +1972,15 @@
     isAccessibleForFree
     typicalAgeRange
   }
 }
 """
 
 QUERY_EVENTS_GQL = """
-query QueryEvents($filter: EventFilter!) {
+query QueryEvents($filter: EventFilter) {
   events(filter: $filter) {
     results {
       id
       name
       alternateNames
       creationDate
       address {
@@ -1535,28 +2010,40 @@
   updateEvent(event: $event) {
     id
     name
   }
 }
 """
 
+COUNT_FEEDS_GQL = """
+query CountFeeds($filter: FeedFilter) {
+  countFeeds(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_FEED_GQL = """
 mutation CreateFeed($feed: FeedInput!, $correlationId: String) {
   createFeed(feed: $feed, correlationId: $correlationId) {
     id
     name
     state
     type
   }
 }
 """
 
 DELETE_ALL_FEEDS_GQL = """
-mutation DeleteAllFeeds {
-  deleteAllFeeds {
+mutation DeleteAllFeeds($filter: FeedFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllFeeds(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_FEED_GQL = """
@@ -1565,16 +2052,16 @@
     id
     state
   }
 }
 """
 
 DELETE_FEEDS_GQL = """
-mutation DeleteFeeds($ids: [ID!]!) {
-  deleteFeeds(ids: $ids) {
+mutation DeleteFeeds($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteFeeds(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 DISABLE_FEED_GQL = """
@@ -1906,26 +2393,38 @@
     name
     state
     type
   }
 }
 """
 
+COUNT_LABELS_GQL = """
+query CountLabels($filter: LabelFilter) {
+  countLabels(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_LABEL_GQL = """
 mutation CreateLabel($label: LabelInput!) {
   createLabel(label: $label) {
     id
     name
   }
 }
 """
 
 DELETE_ALL_LABELS_GQL = """
-mutation DeleteAllLabels($filter: LabelFilter!) {
-  deleteAllLabels(filter: $filter) {
+mutation DeleteAllLabels($filter: LabelFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllLabels(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_LABEL_GQL = """
@@ -1934,16 +2433,16 @@
     id
     state
   }
 }
 """
 
 DELETE_LABELS_GQL = """
-mutation DeleteLabels($ids: [ID!]!) {
-  deleteLabels(ids: $ids) {
+mutation DeleteLabels($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteLabels(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_LABEL_GQL = """
@@ -1954,15 +2453,15 @@
     description
     creationDate
   }
 }
 """
 
 QUERY_LABELS_GQL = """
-query QueryLabels($filter: LabelFilter!) {
+query QueryLabels($filter: LabelFilter) {
   labels(filter: $filter) {
     results {
       id
       name
       description
       creationDate
     }
@@ -2002,26 +2501,38 @@
   updateObservation(observation: $observation) {
     id
     state
   }
 }
 """
 
+COUNT_ORGANIZATIONS_GQL = """
+query CountOrganizations($filter: OrganizationFilter) {
+  countOrganizations(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_ORGANIZATION_GQL = """
 mutation CreateOrganization($organization: OrganizationInput!) {
   createOrganization(organization: $organization) {
     id
     name
   }
 }
 """
 
 DELETE_ALL_ORGANIZATIONS_GQL = """
-mutation DeleteAllOrganizations($filter: OrganizationFilter!) {
-  deleteAllOrganizations(filter: $filter) {
+mutation DeleteAllOrganizations($filter: OrganizationFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllOrganizations(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_ORGANIZATION_GQL = """
@@ -2030,16 +2541,16 @@
     id
     state
   }
 }
 """
 
 DELETE_ORGANIZATIONS_GQL = """
-mutation DeleteOrganizations($ids: [ID!]!) {
-  deleteOrganizations(ids: $ids) {
+mutation DeleteOrganizations($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteOrganizations(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_ORGANIZATION_GQL = """
@@ -2063,15 +2574,15 @@
     investment
     investmentCurrency
   }
 }
 """
 
 QUERY_ORGANIZATIONS_GQL = """
-query QueryOrganizations($filter: OrganizationFilter!) {
+query QueryOrganizations($filter: OrganizationFilter) {
   organizations(filter: $filter) {
     results {
       id
       name
       alternateNames
       creationDate
       address {
@@ -2097,26 +2608,38 @@
   updateOrganization(organization: $organization) {
     id
     name
   }
 }
 """
 
+COUNT_PERSONS_GQL = """
+query CountPersons($filter: PersonFilter) {
+  countPersons(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_PERSON_GQL = """
 mutation CreatePerson($person: PersonInput!) {
   createPerson(person: $person) {
     id
     name
   }
 }
 """
 
 DELETE_ALL_PERSONS_GQL = """
-mutation DeleteAllPersons($filter: PersonFilter!) {
-  deleteAllPersons(filter: $filter) {
+mutation DeleteAllPersons($filter: PersonFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllPersons(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_PERSON_GQL = """
@@ -2125,16 +2648,16 @@
     id
     state
   }
 }
 """
 
 DELETE_PERSONS_GQL = """
-mutation DeletePersons($ids: [ID!]!) {
-  deletePersons(ids: $ids) {
+mutation DeletePersons($ids: [ID!]!, $isSynchronous: Boolean) {
+  deletePersons(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_PERSON_GQL = """
@@ -2160,15 +2683,15 @@
     occupation
     education
   }
 }
 """
 
 QUERY_PERSONS_GQL = """
-query QueryPersons($filter: PersonFilter!) {
+query QueryPersons($filter: PersonFilter) {
   persons(filter: $filter) {
     results {
       id
       name
       alternateNames
       creationDate
       address {
@@ -2196,26 +2719,38 @@
   updatePerson(person: $person) {
     id
     name
   }
 }
 """
 
+COUNT_PLACES_GQL = """
+query CountPlaces($filter: PlaceFilter) {
+  countPlaces(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_PLACE_GQL = """
 mutation CreatePlace($place: PlaceInput!) {
   createPlace(place: $place) {
     id
     name
   }
 }
 """
 
 DELETE_ALL_PLACES_GQL = """
-mutation DeleteAllPlaces($filter: PlaceFilter!) {
-  deleteAllPlaces(filter: $filter) {
+mutation DeleteAllPlaces($filter: PlaceFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllPlaces(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_PLACE_GQL = """
@@ -2224,16 +2759,16 @@
     id
     state
   }
 }
 """
 
 DELETE_PLACES_GQL = """
-mutation DeletePlaces($ids: [ID!]!) {
-  deletePlaces(ids: $ids) {
+mutation DeletePlaces($ids: [ID!]!, $isSynchronous: Boolean) {
+  deletePlaces(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_PLACE_GQL = """
@@ -2251,15 +2786,15 @@
       postalCode
     }
   }
 }
 """
 
 QUERY_PLACES_GQL = """
-query QueryPlaces($filter: PlaceFilter!) {
+query QueryPlaces($filter: PlaceFilter) {
   places(filter: $filter) {
     results {
       id
       name
       alternateNames
       creationDate
       address {
@@ -2279,26 +2814,38 @@
   updatePlace(place: $place) {
     id
     name
   }
 }
 """
 
+COUNT_PRODUCTS_GQL = """
+query CountProducts($filter: ProductFilter) {
+  countProducts(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_PRODUCT_GQL = """
 mutation CreateProduct($product: ProductInput!) {
   createProduct(product: $product) {
     id
     name
   }
 }
 """
 
 DELETE_ALL_PRODUCTS_GQL = """
-mutation DeleteAllProducts($filter: ProductFilter!) {
-  deleteAllProducts(filter: $filter) {
+mutation DeleteAllProducts($filter: ProductFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllProducts(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_PRODUCT_GQL = """
@@ -2307,16 +2854,16 @@
     id
     state
   }
 }
 """
 
 DELETE_PRODUCTS_GQL = """
-mutation DeleteProducts($ids: [ID!]!) {
-  deleteProducts(ids: $ids) {
+mutation DeleteProducts($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteProducts(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_PRODUCT_GQL = """
@@ -2341,15 +2888,15 @@
     releaseDate
     productionDate
   }
 }
 """
 
 QUERY_PRODUCTS_GQL = """
-query QueryProducts($filter: ProductFilter!) {
+query QueryProducts($filter: ProductFilter) {
   products(filter: $filter) {
     results {
       id
       name
       alternateNames
       creationDate
       address {
@@ -2376,32 +2923,14 @@
   updateProduct(product: $product) {
     id
     name
   }
 }
 """
 
-CREDITS_GQL = """
-query Credits($startDate: DateTime!, $duration: TimeSpan!) {
-  credits(startDate: $startDate, duration: $duration) {
-    correlationId
-    ownerId
-    credits
-    storageRatio
-    computeRatio
-    preparationRatio
-    extractionRatio
-    enrichmentRatio
-    publishingRatio
-    searchRatio
-    conversationRatio
-  }
-}
-"""
-
 GET_PROJECT_GQL = """
 query GetProject {
   project {
     id
     name
     creationDate
     modifiedDate
@@ -2477,25 +3006,34 @@
     request
     variables
     response
   }
 }
 """
 
-UPDATE_PROJECT_GQL = """
-mutation UpdateProject($project: ProjectUpdateInput!) {
-  updateProject(project: $project) {
-    id
-    name
+QUERY_CREDITS_GQL = """
+query QueryCredits($startDate: DateTime!, $duration: TimeSpan!) {
+  credits(startDate: $startDate, duration: $duration) {
+    correlationId
+    ownerId
+    credits
+    storageRatio
+    computeRatio
+    preparationRatio
+    extractionRatio
+    enrichmentRatio
+    publishingRatio
+    searchRatio
+    conversationRatio
   }
 }
 """
 
-USAGE_GQL = """
-query Usage($startDate: DateTime!, $duration: TimeSpan!) {
+QUERY_USAGE_GQL = """
+query QueryUsage($startDate: DateTime!, $duration: TimeSpan!) {
   usage(startDate: $startDate, duration: $duration) {
     correlationId
     date
     credits
     name
     metric
     workflow
@@ -2520,26 +3058,47 @@
     request
     variables
     response
   }
 }
 """
 
+UPDATE_PROJECT_GQL = """
+mutation UpdateProject($project: ProjectUpdateInput!) {
+  updateProject(project: $project) {
+    id
+    name
+  }
+}
+"""
+
+COUNT_REPOS_GQL = """
+query CountRepos($filter: RepoFilter) {
+  countRepos(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_REPO_GQL = """
 mutation CreateRepo($repo: RepoInput!) {
   createRepo(repo: $repo) {
     id
     name
   }
 }
 """
 
 DELETE_ALL_REPOS_GQL = """
-mutation DeleteAllRepos($filter: RepoFilter!) {
-  deleteAllRepos(filter: $filter) {
+mutation DeleteAllRepos($filter: RepoFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllRepos(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_REPO_GQL = """
@@ -2548,16 +3107,16 @@
     id
     state
   }
 }
 """
 
 DELETE_REPOS_GQL = """
-mutation DeleteRepos($ids: [ID!]!) {
-  deleteRepos(ids: $ids) {
+mutation DeleteRepos($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteRepos(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_REPO_GQL = """
@@ -2568,15 +3127,15 @@
     alternateNames
     creationDate
   }
 }
 """
 
 QUERY_REPOS_GQL = """
-query QueryRepos($filter: RepoFilter!) {
+query QueryRepos($filter: RepoFilter) {
   repos(filter: $filter) {
     results {
       id
       name
       alternateNames
       creationDate
     }
@@ -2589,26 +3148,38 @@
   updateRepo(repo: $repo) {
     id
     name
   }
 }
 """
 
+COUNT_SOFTWARES_GQL = """
+query CountSoftwares($filter: SoftwareFilter) {
+  countSoftwares(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_SOFTWARE_GQL = """
 mutation CreateSoftware($software: SoftwareInput!) {
   createSoftware(software: $software) {
     id
     name
   }
 }
 """
 
 DELETE_ALL_SOFTWARES_GQL = """
-mutation DeleteAllSoftwares($filter: SoftwareFilter!) {
-  deleteAllSoftwares(filter: $filter) {
+mutation DeleteAllSoftwares($filter: SoftwareFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllSoftwares(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_SOFTWARE_GQL = """
@@ -2617,16 +3188,16 @@
     id
     state
   }
 }
 """
 
 DELETE_SOFTWARES_GQL = """
-mutation DeleteSoftwares($ids: [ID!]!) {
-  deleteSoftwares(ids: $ids) {
+mutation DeleteSoftwares($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteSoftwares(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_SOFTWARE_GQL = """
@@ -2639,15 +3210,15 @@
     releaseDate
     developer
   }
 }
 """
 
 QUERY_SOFTWARES_GQL = """
-query QuerySoftwares($filter: SoftwareFilter!) {
+query QuerySoftwares($filter: SoftwareFilter) {
   softwares(filter: $filter) {
     results {
       id
       name
       alternateNames
       creationDate
       releaseDate
@@ -2662,49 +3233,82 @@
   updateSoftware(software: $software) {
     id
     name
   }
 }
 """
 
+COUNT_SPECIFICATIONS_GQL = """
+query CountSpecifications($filter: SpecificationFilter) {
+  countSpecifications(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_SPECIFICATION_GQL = """
 mutation CreateSpecification($specification: SpecificationInput!) {
   createSpecification(specification: $specification) {
     id
     name
     state
     type
     serviceType
   }
 }
 """
 
+DELETE_ALL_SPECIFICATIONS_GQL = """
+mutation DeleteAllSpecifications($filter: SpecificationFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllSpecifications(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
+    id
+    state
+  }
+}
+"""
+
 DELETE_SPECIFICATION_GQL = """
 mutation DeleteSpecification($id: ID!) {
   deleteSpecification(id: $id) {
     id
     state
   }
 }
 """
 
+DELETE_SPECIFICATIONS_GQL = """
+mutation DeleteSpecifications($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteSpecifications(ids: $ids, isSynchronous: $isSynchronous) {
+    id
+    state
+  }
+}
+"""
+
 GET_SPECIFICATION_GQL = """
 query GetSpecification($id: ID!) {
   specification(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
     state
     type
     serviceType
     systemPrompt
     customGuidance
+    customInstructions
+    searchType
+    numberSimilar
     strategy {
       type
       messageLimit
       embedCitations
       enableFacets
       messagesWeight
       contentsWeight
@@ -2734,14 +3338,23 @@
       model
       key
       endpoint
       deploymentName
       temperature
       probability
     }
+    cohere {
+      tokenLimit
+      completionTokenLimit
+      model
+      key
+      modelName
+      temperature
+      probability
+    }
     anthropic {
       tokenLimit
       completionTokenLimit
       model
       key
       modelName
       temperature
@@ -2775,14 +3388,21 @@
     messages {
       role
       author
       message
       citations {
         content {
           id
+          name
+          state
+          type
+          fileType
+          fileName
+          originalDate
+          uri
         }
         index
         text
         startTime
         endTime
         pageNumber
         frameNumber
@@ -2810,14 +3430,17 @@
         id
       }
       state
       type
       serviceType
       systemPrompt
       customGuidance
+      customInstructions
+      searchType
+      numberSimilar
       strategy {
         type
         messageLimit
         embedCitations
         enableFacets
         messagesWeight
         contentsWeight
@@ -2847,14 +3470,23 @@
         model
         key
         endpoint
         deploymentName
         temperature
         probability
       }
+      cohere {
+        tokenLimit
+        completionTokenLimit
+        model
+        key
+        modelName
+        temperature
+        probability
+      }
       anthropic {
         tokenLimit
         completionTokenLimit
         model
         key
         modelName
         temperature
@@ -2888,14 +3520,22 @@
     state
     type
     serviceType
   }
 }
 """
 
+COUNT_WORKFLOWS_GQL = """
+query CountWorkflows($filter: WorkflowFilter) {
+  countWorkflows(filter: $filter) {
+    count
+  }
+}
+"""
+
 CREATE_WORKFLOW_GQL = """
 mutation CreateWorkflow($workflow: WorkflowInput!) {
   createWorkflow(workflow: $workflow) {
     id
     name
     state
     ingestion {
@@ -2952,14 +3592,15 @@
           }
           azureImage {
             confidenceThreshold
           }
           openAIImage {
             confidenceThreshold
             detailLevel
+            customInstructions
           }
           modelText {
             specification {
               id
             }
           }
         }
@@ -2995,16 +3636,20 @@
       }
     }
   }
 }
 """
 
 DELETE_ALL_WORKFLOWS_GQL = """
-mutation DeleteAllWorkflows {
-  deleteAllWorkflows {
+mutation DeleteAllWorkflows($filter: WorkflowFilter, $isSynchronous: Boolean, $correlationId: String) {
+  deleteAllWorkflows(
+    filter: $filter
+    isSynchronous: $isSynchronous
+    correlationId: $correlationId
+  ) {
     id
     state
   }
 }
 """
 
 DELETE_WORKFLOW_GQL = """
@@ -3013,16 +3658,16 @@
     id
     state
   }
 }
 """
 
 DELETE_WORKFLOWS_GQL = """
-mutation DeleteWorkflows($ids: [ID!]!) {
-  deleteWorkflows(ids: $ids) {
+mutation DeleteWorkflows($ids: [ID!]!, $isSynchronous: Boolean) {
+  deleteWorkflows(ids: $ids, isSynchronous: $isSynchronous) {
     id
     state
   }
 }
 """
 
 GET_WORKFLOW_GQL = """
@@ -3089,14 +3734,15 @@
           }
           azureImage {
             confidenceThreshold
           }
           openAIImage {
             confidenceThreshold
             detailLevel
+            customInstructions
           }
           modelText {
             specification {
               id
             }
           }
         }
@@ -3200,14 +3846,15 @@
             }
             azureImage {
               confidenceThreshold
             }
             openAIImage {
               confidenceThreshold
               detailLevel
+              customInstructions
             }
             modelText {
               specification {
                 id
               }
             }
           }
@@ -3307,14 +3954,15 @@
           }
           azureImage {
             confidenceThreshold
           }
           openAIImage {
             confidenceThreshold
             detailLevel
+            customInstructions
           }
           modelText {
             specification {
               id
             }
           }
         }
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240505001/graphlit_api/prompt_conversation.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
     ContentFacetTypes,
     ContentTypes,
     ConversationRoleTypes,
+    EntityState,
     FacetValueTypes,
     FileTypes,
     ModelServiceTypes,
     ObservableTypes,
 )
 
 
@@ -58,17 +59,20 @@
     page_number: Optional[int] = Field(alias="pageNumber")
     frame_number: Optional[int] = Field(alias="frameNumber")
 
 
 class PromptConversationPromptConversationMessageCitationsContent(BaseModel):
     id: str
     name: str
+    state: EntityState
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
     file_name: Optional[str] = Field(alias="fileName")
+    original_date: Optional[Any] = Field(alias="originalDate")
+    uri: Optional[Any]
 
 
 class PromptConversationPromptConversationFacets(BaseModel):
     type: Optional[FacetValueTypes]
     value: Optional[str]
     range: Optional["PromptConversationPromptConversationFacetsRange"]
     count: Optional[Any]
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240505001/graphlit_api/prompt_specifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 # Source: ./documents
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .enums import ConversationRoleTypes, ModelServiceTypes
+from .enums import (
+    ContentTypes,
+    ConversationRoleTypes,
+    EntityState,
+    FileTypes,
+    ModelServiceTypes,
+)
 
 
 class PromptSpecifications(BaseModel):
     prompt_specifications: Optional[
         List[Optional["PromptSpecificationsPromptSpecifications"]]
     ] = Field(alias="promptSpecifications")
 
@@ -52,13 +58,20 @@
     end_time: Optional[Any] = Field(alias="endTime")
     page_number: Optional[int] = Field(alias="pageNumber")
     frame_number: Optional[int] = Field(alias="frameNumber")
 
 
 class PromptSpecificationsPromptSpecificationsMessagesCitationsContent(BaseModel):
     id: str
+    name: str
+    state: EntityState
+    type: Optional[ContentTypes]
+    file_type: Optional[FileTypes] = Field(alias="fileType")
+    file_name: Optional[str] = Field(alias="fileName")
+    original_date: Optional[Any] = Field(alias="originalDate")
+    uri: Optional[Any]
 
 
 PromptSpecifications.model_rebuild()
 PromptSpecificationsPromptSpecifications.model_rebuild()
 PromptSpecificationsPromptSpecificationsMessages.model_rebuild()
 PromptSpecificationsPromptSpecificationsMessagesCitations.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240505001/graphlit_api/publish_text.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ContentTypes, EntityState, FileTypes
 
 
-class PublishContents(BaseModel):
-    publish_contents: Optional["PublishContentsPublishContents"] = Field(
-        alias="publishContents"
-    )
+class PublishText(BaseModel):
+    publish_text: Optional["PublishTextPublishText"] = Field(alias="publishText")
 
 
-class PublishContentsPublishContents(BaseModel):
+class PublishTextPublishText(BaseModel):
     id: str
     name: str
     state: EntityState
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
     mime_type: Optional[str] = Field(alias="mimeType")
     uri: Optional[Any]
+    collections: Optional[List[Optional["PublishTextPublishTextCollections"]]]
     text_uri: Optional[Any] = Field(alias="textUri")
     audio_uri: Optional[Any] = Field(alias="audioUri")
     markdown: Optional[str]
 
 
-PublishContents.model_rebuild()
+class PublishTextPublishTextCollections(BaseModel):
+    id: str
+    name: str
+
+
+PublishText.model_rebuild()
+PublishTextPublishText.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240505001/graphlit_api/publish_contents.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ContentTypes, EntityState, FileTypes
 
 
-class PublishConversation(BaseModel):
-    publish_conversation: Optional["PublishConversationPublishConversation"] = Field(
-        alias="publishConversation"
+class PublishContents(BaseModel):
+    publish_contents: Optional["PublishContentsPublishContents"] = Field(
+        alias="publishContents"
     )
 
 
-class PublishConversationPublishConversation(BaseModel):
+class PublishContentsPublishContents(BaseModel):
     id: str
     name: str
     state: EntityState
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
     mime_type: Optional[str] = Field(alias="mimeType")
     uri: Optional[Any]
+    collections: Optional[List[Optional["PublishContentsPublishContentsCollections"]]]
     text_uri: Optional[Any] = Field(alias="textUri")
     audio_uri: Optional[Any] = Field(alias="audioUri")
     markdown: Optional[str]
 
 
-PublishConversation.model_rebuild()
+class PublishContentsPublishContentsCollections(BaseModel):
+    id: str
+    name: str
+
+
+PublishContents.model_rebuild()
+PublishContentsPublishContents.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_categories.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_categories.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_contents.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
     ContentTypes,
     EntityState,
     FileTypes,
+    ImageProjectionTypes,
     LinkTypes,
     MailImportance,
     MailPriority,
     MailSensitivity,
     ObservableTypes,
     OccurrenceTypes,
+    OrientationTypes,
     TextRoles,
 )
 
 
 class QueryContents(BaseModel):
     contents: Optional["QueryContentsContents"]
 
@@ -34,238 +36,283 @@
     creation_date: Any = Field(alias="creationDate")
     owner: "QueryContentsContentsResultsOwner"
     state: EntityState
     original_date: Optional[Any] = Field(alias="originalDate")
     finished_date: Optional[Any] = Field(alias="finishedDate")
     workflow_duration: Optional[Any] = Field(alias="workflowDuration")
     uri: Optional[Any]
+    description: Optional[str]
+    markdown: Optional[str]
+    address: Optional["QueryContentsContentsResultsAddress"]
+    location: Optional["QueryContentsContentsResultsLocation"]
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
     mime_type: Optional[str] = Field(alias="mimeType")
     file_name: Optional[str] = Field(alias="fileName")
     file_size: Optional[Any] = Field(alias="fileSize")
     master_uri: Optional[Any] = Field(alias="masterUri")
     image_uri: Optional[Any] = Field(alias="imageUri")
     text_uri: Optional[Any] = Field(alias="textUri")
     audio_uri: Optional[Any] = Field(alias="audioUri")
     transcript_uri: Optional[Any] = Field(alias="transcriptUri")
-    pages: Optional[List["QueryContentsContentsResultsPages"]]
-    segments: Optional[List["QueryContentsContentsResultsSegments"]]
     video: Optional["QueryContentsContentsResultsVideo"]
     audio: Optional["QueryContentsContentsResultsAudio"]
     image: Optional["QueryContentsContentsResultsImage"]
     document: Optional["QueryContentsContentsResultsDocument"]
     email: Optional["QueryContentsContentsResultsEmail"]
     issue: Optional["QueryContentsContentsResultsIssue"]
-    observations: Optional[List[Optional["QueryContentsContentsResultsObservations"]]]
+    package: Optional["QueryContentsContentsResultsPackage"]
     parent: Optional["QueryContentsContentsResultsParent"]
     children: Optional[List[Optional["QueryContentsContentsResultsChildren"]]]
-    collections: Optional[List[Optional["QueryContentsContentsResultsCollections"]]]
     feed: Optional["QueryContentsContentsResultsFeed"]
-    workflow: Optional["QueryContentsContentsResultsWorkflow"]
-    markdown: Optional[str]
+    collections: Optional[List[Optional["QueryContentsContentsResultsCollections"]]]
     links: Optional[List["QueryContentsContentsResultsLinks"]]
+    observations: Optional[List[Optional["QueryContentsContentsResultsObservations"]]]
+    workflow: Optional["QueryContentsContentsResultsWorkflow"]
+    pages: Optional[List["QueryContentsContentsResultsPages"]]
+    segments: Optional[List["QueryContentsContentsResultsSegments"]]
     error: Optional[str]
 
 
 class QueryContentsContentsResultsOwner(BaseModel):
     id: str
 
 
-class QueryContentsContentsResultsPages(BaseModel):
-    index: Optional[int]
-    chunks: Optional[List[Optional["QueryContentsContentsResultsPagesChunks"]]]
+class QueryContentsContentsResultsAddress(BaseModel):
+    street_address: Optional[str] = Field(alias="streetAddress")
+    city: Optional[str]
+    region: Optional[str]
+    country: Optional[str]
+    postal_code: Optional[str] = Field(alias="postalCode")
 
 
-class QueryContentsContentsResultsPagesChunks(BaseModel):
-    index: Optional[int]
-    page_index: Optional[int] = Field(alias="pageIndex")
-    row_index: Optional[int] = Field(alias="rowIndex")
-    column_index: Optional[int] = Field(alias="columnIndex")
-    confidence: Optional[float]
-    text: Optional[str]
-    role: Optional[TextRoles]
-    relevance: Optional[float]
-
-
-class QueryContentsContentsResultsSegments(BaseModel):
-    start_time: Optional[Any] = Field(alias="startTime")
-    end_time: Optional[Any] = Field(alias="endTime")
-    text: Optional[str]
-    relevance: Optional[float]
+class QueryContentsContentsResultsLocation(BaseModel):
+    latitude: Optional[float]
+    longitude: Optional[float]
 
 
 class QueryContentsContentsResultsVideo(BaseModel):
     width: Optional[int]
     height: Optional[int]
     duration: Optional[str]
-    software: Optional[str]
     make: Optional[str]
     model: Optional[str]
+    software: Optional[str]
+    title: Optional[str]
+    description: Optional[str]
+    keywords: Optional[List[Optional[str]]]
+    author: Optional[str]
 
 
 class QueryContentsContentsResultsAudio(BaseModel):
     keywords: Optional[List[Optional[str]]]
     author: Optional[str]
     series: Optional[str]
     episode: Optional[str]
     episode_type: Optional[str] = Field(alias="episodeType")
     season: Optional[str]
     publisher: Optional[str]
     copyright: Optional[str]
     language: Optional[str]
     genre: Optional[str]
     title: Optional[str]
+    description: Optional[str]
     bitrate: Optional[int]
     channels: Optional[int]
     sample_rate: Optional[int] = Field(alias="sampleRate")
     bits_per_sample: Optional[int] = Field(alias="bitsPerSample")
     duration: Optional[str]
 
 
 class QueryContentsContentsResultsImage(BaseModel):
     width: Optional[int]
     height: Optional[int]
+    resolution_x: Optional[int] = Field(alias="resolutionX")
+    resolution_y: Optional[int] = Field(alias="resolutionY")
+    bits_per_component: Optional[int] = Field(alias="bitsPerComponent")
+    components: Optional[int]
+    projection_type: Optional[ImageProjectionTypes] = Field(alias="projectionType")
+    orientation: Optional[OrientationTypes]
     description: Optional[str]
-    software: Optional[str]
-    identifier: Optional[str]
     make: Optional[str]
     model: Optional[str]
+    software: Optional[str]
+    lens: Optional[str]
+    focal_length: Optional[float] = Field(alias="focalLength")
+    exposure_time: Optional[str] = Field(alias="exposureTime")
+    f_number: Optional[str] = Field(alias="fNumber")
+    iso: Optional[str]
+    heading: Optional[float]
+    pitch: Optional[float]
 
 
 class QueryContentsContentsResultsDocument(BaseModel):
     title: Optional[str]
     subject: Optional[str]
+    summary: Optional[str]
     author: Optional[str]
-    software: Optional[str]
     publisher: Optional[str]
     description: Optional[str]
-    summary: Optional[str]
     keywords: Optional[List[Optional[str]]]
     page_count: Optional[int] = Field(alias="pageCount")
     worksheet_count: Optional[int] = Field(alias="worksheetCount")
     slide_count: Optional[int] = Field(alias="slideCount")
     word_count: Optional[int] = Field(alias="wordCount")
     line_count: Optional[int] = Field(alias="lineCount")
     paragraph_count: Optional[int] = Field(alias="paragraphCount")
-    character_count: Optional[int] = Field(alias="characterCount")
     is_encrypted: Optional[bool] = Field(alias="isEncrypted")
     has_digital_signature: Optional[bool] = Field(alias="hasDigitalSignature")
 
 
 class QueryContentsContentsResultsEmail(BaseModel):
-    subject: Optional[str]
     identifier: Optional[str]
+    subject: Optional[str]
+    labels: Optional[List[Optional[str]]]
     sensitivity: Optional[MailSensitivity]
     priority: Optional[MailPriority]
     importance: Optional[MailImportance]
-    labels: Optional[List[Optional[str]]]
     from_: Optional[List[Optional["QueryContentsContentsResultsEmailFrom"]]] = Field(
         alias="from"
     )
     to: Optional[List[Optional["QueryContentsContentsResultsEmailTo"]]]
     cc: Optional[List[Optional["QueryContentsContentsResultsEmailCc"]]]
     bcc: Optional[List[Optional["QueryContentsContentsResultsEmailBcc"]]]
 
 
 class QueryContentsContentsResultsEmailFrom(BaseModel):
     name: Optional[str]
-    family_name: Optional[str] = Field(alias="familyName")
-    given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
+    given_name: Optional[str] = Field(alias="givenName")
+    family_name: Optional[str] = Field(alias="familyName")
 
 
 class QueryContentsContentsResultsEmailTo(BaseModel):
     name: Optional[str]
-    family_name: Optional[str] = Field(alias="familyName")
-    given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
+    given_name: Optional[str] = Field(alias="givenName")
+    family_name: Optional[str] = Field(alias="familyName")
 
 
 class QueryContentsContentsResultsEmailCc(BaseModel):
     name: Optional[str]
-    family_name: Optional[str] = Field(alias="familyName")
-    given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
+    given_name: Optional[str] = Field(alias="givenName")
+    family_name: Optional[str] = Field(alias="familyName")
 
 
 class QueryContentsContentsResultsEmailBcc(BaseModel):
     name: Optional[str]
-    family_name: Optional[str] = Field(alias="familyName")
-    given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
+    given_name: Optional[str] = Field(alias="givenName")
+    family_name: Optional[str] = Field(alias="familyName")
 
 
 class QueryContentsContentsResultsIssue(BaseModel):
+    identifier: Optional[str]
     title: Optional[str]
     project: Optional[str]
     team: Optional[str]
     status: Optional[str]
     priority: Optional[str]
     type: Optional[str]
-    identifier: Optional[str]
     labels: Optional[List[Optional[str]]]
 
 
+class QueryContentsContentsResultsPackage(BaseModel):
+    file_count: Optional[int] = Field(alias="fileCount")
+    folder_count: Optional[int] = Field(alias="folderCount")
+    is_encrypted: Optional[bool] = Field(alias="isEncrypted")
+
+
+class QueryContentsContentsResultsParent(BaseModel):
+    id: str
+    name: str
+
+
+class QueryContentsContentsResultsChildren(BaseModel):
+    id: str
+    name: str
+
+
+class QueryContentsContentsResultsFeed(BaseModel):
+    id: str
+    name: str
+
+
+class QueryContentsContentsResultsCollections(BaseModel):
+    id: str
+    name: str
+
+
+class QueryContentsContentsResultsLinks(BaseModel):
+    uri: Optional[Any]
+    link_type: Optional[LinkTypes] = Field(alias="linkType")
+
+
 class QueryContentsContentsResultsObservations(BaseModel):
+    id: str
     type: ObservableTypes
     observable: "QueryContentsContentsResultsObservationsObservable"
     occurrences: Optional[
         List[Optional["QueryContentsContentsResultsObservationsOccurrences"]]
     ]
+    state: EntityState
 
 
 class QueryContentsContentsResultsObservationsObservable(BaseModel):
     id: str
     name: Optional[str]
 
 
 class QueryContentsContentsResultsObservationsOccurrences(BaseModel):
     type: Optional[OccurrenceTypes]
     confidence: Optional[float]
+    start_time: Optional[Any] = Field(alias="startTime")
+    end_time: Optional[Any] = Field(alias="endTime")
+    page_index: Optional[int] = Field(alias="pageIndex")
     bounding_box: Optional[
         "QueryContentsContentsResultsObservationsOccurrencesBoundingBox"
     ] = Field(alias="boundingBox")
-    page_index: Optional[int] = Field(alias="pageIndex")
-    start_time: Optional[Any] = Field(alias="startTime")
-    end_time: Optional[Any] = Field(alias="endTime")
 
 
 class QueryContentsContentsResultsObservationsOccurrencesBoundingBox(BaseModel):
     left: Optional[float]
     top: Optional[float]
     width: Optional[float]
     height: Optional[float]
 
 
-class QueryContentsContentsResultsParent(BaseModel):
-    id: str
-
-
-class QueryContentsContentsResultsChildren(BaseModel):
-    id: str
-
-
-class QueryContentsContentsResultsCollections(BaseModel):
+class QueryContentsContentsResultsWorkflow(BaseModel):
     id: str
+    name: str
 
 
-class QueryContentsContentsResultsFeed(BaseModel):
-    id: str
+class QueryContentsContentsResultsPages(BaseModel):
+    index: Optional[int]
+    chunks: Optional[List[Optional["QueryContentsContentsResultsPagesChunks"]]]
 
 
-class QueryContentsContentsResultsWorkflow(BaseModel):
-    id: str
+class QueryContentsContentsResultsPagesChunks(BaseModel):
+    index: Optional[int]
+    page_index: Optional[int] = Field(alias="pageIndex")
+    row_index: Optional[int] = Field(alias="rowIndex")
+    column_index: Optional[int] = Field(alias="columnIndex")
+    confidence: Optional[float]
+    text: Optional[str]
+    role: Optional[TextRoles]
+    relevance: Optional[float]
 
 
-class QueryContentsContentsResultsLinks(BaseModel):
-    uri: Optional[Any]
-    link_type: Optional[LinkTypes] = Field(alias="linkType")
+class QueryContentsContentsResultsSegments(BaseModel):
+    start_time: Optional[Any] = Field(alias="startTime")
+    end_time: Optional[Any] = Field(alias="endTime")
+    text: Optional[str]
+    relevance: Optional[float]
 
 
 QueryContents.model_rebuild()
 QueryContentsContents.model_rebuild()
 QueryContentsContentsResults.model_rebuild()
-QueryContentsContentsResultsPages.model_rebuild()
 QueryContentsContentsResultsEmail.model_rebuild()
 QueryContentsContentsResultsObservations.model_rebuild()
 QueryContentsContentsResultsObservationsOccurrences.model_rebuild()
+QueryContentsContentsResultsPages.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_conversations.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,14 +65,21 @@
     end_time: Optional[Any] = Field(alias="endTime")
     page_number: Optional[int] = Field(alias="pageNumber")
     frame_number: Optional[int] = Field(alias="frameNumber")
 
 
 class QueryConversationsConversationsResultsMessagesCitationsContent(BaseModel):
     id: str
+    name: str
+    state: EntityState
+    type: Optional[ContentTypes]
+    file_type: Optional[FileTypes] = Field(alias="fileType")
+    file_name: Optional[str] = Field(alias="fileName")
+    original_date: Optional[Any] = Field(alias="originalDate")
+    uri: Optional[Any]
 
 
 class QueryConversationsConversationsResultsSpecification(BaseModel):
     id: str
     name: str
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_events.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_events.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_labels.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_labels.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_organizations.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_persons.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_persons.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_places.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_places.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_products.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_products.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_repos.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_repos.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_software.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_softwares.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
-class QuerySoftware(BaseModel):
-    softwares: Optional["QuerySoftwareSoftwares"]
+class QuerySoftwares(BaseModel):
+    softwares: Optional["QuerySoftwaresSoftwares"]
 
 
-class QuerySoftwareSoftwares(BaseModel):
-    results: Optional[List[Optional["QuerySoftwareSoftwaresResults"]]]
+class QuerySoftwaresSoftwares(BaseModel):
+    results: Optional[List[Optional["QuerySoftwaresSoftwaresResults"]]]
 
 
-class QuerySoftwareSoftwaresResults(BaseModel):
+class QuerySoftwaresSoftwaresResults(BaseModel):
     id: str
     name: str
     alternate_names: Optional[List[Optional[str]]] = Field(alias="alternateNames")
     creation_date: Any = Field(alias="creationDate")
     release_date: Optional[Any] = Field(alias="releaseDate")
     developer: Optional[str]
 
 
-QuerySoftware.model_rebuild()
-QuerySoftwareSoftwares.model_rebuild()
+QuerySoftwares.model_rebuild()
+QuerySoftwaresSoftwares.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_specifications.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
     AnthropicModels,
     AzureOpenAIModels,
+    CohereModels,
+    ConversationSearchTypes,
     ConversationStrategyTypes,
     EntityState,
     ModelServiceTypes,
     OpenAIModels,
     PromptStrategyTypes,
     ReplicateModels,
     RerankingModelServiceTypes,
@@ -35,14 +37,17 @@
     creation_date: Any = Field(alias="creationDate")
     owner: "QuerySpecificationsSpecificationsResultsOwner"
     state: EntityState
     type: Optional[SpecificationTypes]
     service_type: Optional[ModelServiceTypes] = Field(alias="serviceType")
     system_prompt: Optional[str] = Field(alias="systemPrompt")
     custom_guidance: Optional[str] = Field(alias="customGuidance")
+    custom_instructions: Optional[str] = Field(alias="customInstructions")
+    search_type: Optional[ConversationSearchTypes] = Field(alias="searchType")
+    number_similar: Optional[int] = Field(alias="numberSimilar")
     strategy: Optional["QuerySpecificationsSpecificationsResultsStrategy"]
     prompt_strategy: Optional[
         "QuerySpecificationsSpecificationsResultsPromptStrategy"
     ] = Field(alias="promptStrategy")
     retrieval_strategy: Optional[
         "QuerySpecificationsSpecificationsResultsRetrievalStrategy"
     ] = Field(alias="retrievalStrategy")
@@ -51,14 +56,15 @@
     ] = Field(alias="rerankingStrategy")
     open_ai: Optional["QuerySpecificationsSpecificationsResultsOpenAi"] = Field(
         alias="openAI"
     )
     azure_open_ai: Optional["QuerySpecificationsSpecificationsResultsAzureOpenAi"] = (
         Field(alias="azureOpenAI")
     )
+    cohere: Optional["QuerySpecificationsSpecificationsResultsCohere"]
     anthropic: Optional["QuerySpecificationsSpecificationsResultsAnthropic"]
     replicate: Optional["QuerySpecificationsSpecificationsResultsReplicate"]
     tools: Optional[List["QuerySpecificationsSpecificationsResultsTools"]]
 
 
 class QuerySpecificationsSpecificationsResultsOwner(BaseModel):
     id: str
@@ -103,14 +109,24 @@
     key: Optional[str]
     endpoint: Optional[Any]
     deployment_name: Optional[str] = Field(alias="deploymentName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
+class QuerySpecificationsSpecificationsResultsCohere(BaseModel):
+    token_limit: Optional[int] = Field(alias="tokenLimit")
+    completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
+    model: CohereModels
+    key: Optional[str]
+    model_name: Optional[str] = Field(alias="modelName")
+    temperature: Optional[float]
+    probability: Optional[float]
+
+
 class QuerySpecificationsSpecificationsResultsAnthropic(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: AnthropicModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
 class QueryWorkflowsWorkflowsResultsExtractionJobsConnectorAzureImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
 
 
 class QueryWorkflowsWorkflowsResultsExtractionJobsConnectorOpenAiImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
     detail_level: Optional[OpenAIVisionDetailLevels] = Field(alias="detailLevel")
+    custom_instructions: Optional[str] = Field(alias="customInstructions")
 
 
 class QueryWorkflowsWorkflowsResultsExtractionJobsConnectorModelText(BaseModel):
     specification: Optional[
         "QueryWorkflowsWorkflowsResultsExtractionJobsConnectorModelTextSpecification"
     ]
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240505001/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240505001/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240505001/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/update_content.py` & `graphlit_client-1.0.20240505001/graphlit_api/update_content.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ContentTypes, EntityState, FileTypes
 
 
@@ -19,10 +19,17 @@
     id: str
     name: str
     state: EntityState
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
     mime_type: Optional[str] = Field(alias="mimeType")
     uri: Optional[Any]
+    collections: Optional[List[Optional["UpdateContentUpdateContentCollections"]]]
+
+
+class UpdateContentUpdateContentCollections(BaseModel):
+    id: str
+    name: str
 
 
 UpdateContent.model_rebuild()
+UpdateContentUpdateContent.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240505001/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240505001/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240505001/graphlit_api/update_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 class UpdateWorkflowUpdateWorkflowExtractionJobsConnectorAzureImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
 
 
 class UpdateWorkflowUpdateWorkflowExtractionJobsConnectorOpenAiImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
     detail_level: Optional[OpenAIVisionDetailLevels] = Field(alias="detailLevel")
+    custom_instructions: Optional[str] = Field(alias="customInstructions")
 
 
 class UpdateWorkflowUpdateWorkflowExtractionJobsConnectorModelText(BaseModel):
     specification: Optional[
         "UpdateWorkflowUpdateWorkflowExtractionJobsConnectorModelTextSpecification"
     ]
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_api/usage.py` & `graphlit_client-1.0.20240505001/graphlit_api/query_usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import BillableMetrics, ContentTypes, EntityTypes, FileTypes
 
 
-class Usage(BaseModel):
-    usage: Optional[List[Optional["UsageUsage"]]]
+class QueryUsage(BaseModel):
+    usage: Optional[List[Optional["QueryUsageUsage"]]]
 
 
-class UsageUsage(BaseModel):
+class QueryUsageUsage(BaseModel):
     correlation_id: Optional[str] = Field(alias="correlationId")
     date: Any
     credits: Optional[Any]
     name: str
     metric: Optional[BillableMetrics]
     workflow: Optional[str]
     entity_type: Optional[EntityTypes] = Field(alias="entityType")
@@ -39,8 +39,8 @@
     tokens: Optional[int]
     count: Optional[int]
     request: Optional[str]
     variables: Optional[str]
     response: Optional[str]
 
 
-Usage.model_rebuild()
+QueryUsage.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240505001/graphlit_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240429002
+Version: 1.0.20240505001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240429002/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240505001/graphlit_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,30 @@
 graphlit_api/__init__.py
 graphlit_api/add_contents_to_collections.py
 graphlit_api/async_base_client.py
 graphlit_api/base_model.py
 graphlit_api/clear_conversation.py
 graphlit_api/client.py
 graphlit_api/close_conversation.py
+graphlit_api/count_alerts.py
+graphlit_api/count_categories.py
+graphlit_api/count_collections.py
+graphlit_api/count_contents.py
+graphlit_api/count_conversations.py
+graphlit_api/count_events.py
+graphlit_api/count_feeds.py
+graphlit_api/count_labels.py
+graphlit_api/count_organizations.py
+graphlit_api/count_persons.py
+graphlit_api/count_places.py
+graphlit_api/count_products.py
+graphlit_api/count_repos.py
+graphlit_api/count_softwares.py
+graphlit_api/count_specifications.py
+graphlit_api/count_workflows.py
 graphlit_api/create_alert.py
 graphlit_api/create_category.py
 graphlit_api/create_collection.py
 graphlit_api/create_conversation.py
 graphlit_api/create_event.py
 graphlit_api/create_feed.py
 graphlit_api/create_label.py
@@ -23,15 +39,14 @@
 graphlit_api/create_person.py
 graphlit_api/create_place.py
 graphlit_api/create_product.py
 graphlit_api/create_repo.py
 graphlit_api/create_software.py
 graphlit_api/create_specification.py
 graphlit_api/create_workflow.py
-graphlit_api/credits.py
 graphlit_api/delete_alert.py
 graphlit_api/delete_alerts.py
 graphlit_api/delete_all_alerts.py
 graphlit_api/delete_all_categories.py
 graphlit_api/delete_all_collections.py
 graphlit_api/delete_all_contents.py
 graphlit_api/delete_all_conversations.py
@@ -40,14 +55,15 @@
 graphlit_api/delete_all_labels.py
 graphlit_api/delete_all_organizations.py
 graphlit_api/delete_all_persons.py
 graphlit_api/delete_all_places.py
 graphlit_api/delete_all_products.py
 graphlit_api/delete_all_repos.py
 graphlit_api/delete_all_softwares.py
+graphlit_api/delete_all_specifications.py
 graphlit_api/delete_all_workflows.py
 graphlit_api/delete_categories.py
 graphlit_api/delete_category.py
 graphlit_api/delete_collection.py
 graphlit_api/delete_collections.py
 graphlit_api/delete_content.py
 graphlit_api/delete_contents.py
@@ -69,14 +85,15 @@
 graphlit_api/delete_product.py
 graphlit_api/delete_products.py
 graphlit_api/delete_repo.py
 graphlit_api/delete_repos.py
 graphlit_api/delete_software.py
 graphlit_api/delete_softwares.py
 graphlit_api/delete_specification.py
+graphlit_api/delete_specifications.py
 graphlit_api/delete_workflow.py
 graphlit_api/delete_workflows.py
 graphlit_api/disable_alert.py
 graphlit_api/disable_feed.py
 graphlit_api/enable_alert.py
 graphlit_api/enable_feed.py
 graphlit_api/enums.py
@@ -112,28 +129,30 @@
 graphlit_api/prompt_specifications.py
 graphlit_api/publish_contents.py
 graphlit_api/publish_conversation.py
 graphlit_api/publish_text.py
 graphlit_api/query_alerts.py
 graphlit_api/query_categories.py
 graphlit_api/query_collections.py
-graphlit_api/query_content_facets.py
 graphlit_api/query_contents.py
+graphlit_api/query_contents_facets.py
+graphlit_api/query_contents_graph.py
 graphlit_api/query_conversations.py
+graphlit_api/query_credits.py
 graphlit_api/query_events.py
 graphlit_api/query_feeds.py
 graphlit_api/query_labels.py
 graphlit_api/query_organizations.py
 graphlit_api/query_persons.py
 graphlit_api/query_places.py
 graphlit_api/query_products.py
 graphlit_api/query_repos.py
-graphlit_api/query_software.py
 graphlit_api/query_softwares.py
 graphlit_api/query_specifications.py
+graphlit_api/query_usage.py
 graphlit_api/query_workflows.py
 graphlit_api/remove_contents_from_collection.py
 graphlit_api/suggest_conversation.py
 graphlit_api/summarize_contents.py
 graphlit_api/update_alert.py
 graphlit_api/update_category.py
 graphlit_api/update_collection.py
@@ -148,13 +167,12 @@
 graphlit_api/update_place.py
 graphlit_api/update_product.py
 graphlit_api/update_project.py
 graphlit_api/update_repo.py
 graphlit_api/update_software.py
 graphlit_api/update_specification.py
 graphlit_api/update_workflow.py
-graphlit_api/usage.py
 graphlit_client.egg-info/PKG-INFO
 graphlit_client.egg-info/SOURCES.txt
 graphlit_client.egg-info/dependency_links.txt
 graphlit_client.egg-info/requires.txt
 graphlit_client.egg-info/top_level.txt
```

### Comparing `graphlit_client-1.0.20240429002/setup.py` & `graphlit_client-1.0.20240505001/setup.py`

 * *Files identical despite different names*

