# Comparing `tmp/math_spec_mapping-0.3.1.tar.gz` & `tmp/math_spec_mapping-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_spec_mapping-0.3.1.tar", last modified: Wed Apr 17 18:03:10 2024, max compression
+gzip compressed data, was "math_spec_mapping-0.3.2.tar", last modified: Mon May  6 21:45:46 2024, max compression
```

## Comparing `math_spec_mapping-0.3.1.tar` & `math_spec_mapping-0.3.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.157278 math_spec_mapping-0.3.1/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math_spec_mapping-0.3.1/LICENSE
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-04-17 18:03:10.157049 math_spec_mapping-0.3.1/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/README.md
--rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-04-17 18:01:09.000000 math_spec_mapping-0.3.1/pyproject.toml
--rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-04-17 18:03:10.157329 math_spec_mapping-0.3.1/setup.cfg
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.146304 math_spec_mapping-0.3.1/src/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.147557 math_spec_mapping-0.3.1/src/math_spec_mapping/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.151118 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    17302 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Block.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      476 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/BoundaryAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/ControlAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Entity.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    28854 2024-04-17 14:13:59.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/MathSpec.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Metric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Parameter.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Space.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1538 2024-04-09 05:13:17.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/State.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/StatefulMetric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/__init__.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.151666 math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/
--rw-r--r--   0 seanmcowen   (501) staff       (20)       60 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1607 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/documentation.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)        0 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/starter.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.154552 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/
--rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/action_transmission_channel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2058 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      414 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/displays.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1208 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/entities.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/implementations.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/load.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3434 2024-04-17 16:10:27.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1334 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/state_update_transmission_channels.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/stateful_metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1290 2024-04-09 05:14:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/states.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4330 2024-04-15 15:26:17.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/wiring.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.156612 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     9007 2024-04-09 05:23:11.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/html.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    22479 2024-04-17 16:00:07.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/markdown.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/mechanisms.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/node_map.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/policies.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2321 2024-04-09 05:18:38.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/state.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/tables.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/wiring.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      907 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/schema.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    29352 2024-04-09 05:29:32.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/schema.schema.json
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.156809 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/requires.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.846809 math_spec_mapping-0.3.2/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math_spec_mapping-0.3.2/LICENSE
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-06 21:45:46.846566 math_spec_mapping-0.3.2/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/README.md
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-04-20 18:11:50.000000 math_spec_mapping-0.3.2/pyproject.toml
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-05-06 21:45:46.846855 math_spec_mapping-0.3.2/setup.cfg
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.811201 math_spec_mapping-0.3.2/src/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.812855 math_spec_mapping-0.3.2/src/math_spec_mapping/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.838460 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    17302 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Block.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      476 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/BoundaryAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/ControlAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Entity.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    28854 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/MathSpec.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Metric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Parameter.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Space.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1538 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/State.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/StatefulMetric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/__init__.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.839409 math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      112 2024-05-05 21:14:39.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1625 2024-05-05 21:14:18.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/documentation.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    11010 2024-05-06 05:19:05.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/starter.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.843364 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/action_transmission_channel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2058 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      414 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/displays.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1208 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/entities.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/implementations.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/load.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3434 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1393 2024-05-06 21:03:12.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/state_update_transmission_channels.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/stateful_metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1290 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/states.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4356 2024-05-06 05:20:31.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/wiring.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.846065 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     9007 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/html.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    22505 2024-05-06 02:23:26.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/markdown.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/mechanisms.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/node_map.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/policies.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2321 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/state.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/tables.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/wiring.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      961 2024-05-05 21:12:15.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/schema.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    29400 2024-04-23 15:25:57.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/schema.schema.json
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.846312 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/requires.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/top_level.txt
```

### Comparing `math_spec_mapping-0.3.1/LICENSE` & `math_spec_mapping-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/PKG-INFO` & `math_spec_mapping-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math_spec_mapping-0.3.1/README.md` & `math_spec_mapping-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/pyproject.toml` & `math_spec_mapping-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "math-spec-mapping"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Sean McOwen", email="Sean@Block.Science" },
 ]
 description = "A library for easy mapping of mathematical specifications."
 dependencies = [
   "graphviz>=0.20.1",
   "ipython>=7.7.0",
```

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Block.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Block.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/ControlAction.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/ControlAction.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Entity.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Entity.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/MathSpec.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/MathSpec.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Metric.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Metric.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Parameter.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Parameter.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Policy.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Policy.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/State.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/State.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/StatefulMetric.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/StatefulMetric.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/__init__.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/documentation.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/documentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src import schema
+from src.math_spec_mapping import schema
 
 
 def write_json_description(schema, key, name):
     out = "- **{}**: ".format(name)
 
     out += schema["definitions"][key]["description"]
     out += "\n"
```

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/action_transmission_channel.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/action_transmission_channel.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/boundary_actions.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/control_actions.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/control_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/entities.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/entities.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/general.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/general.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/load.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/load.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/mechanism.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/mechanism.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/metrics.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/metrics.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/parameters.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
     # Convert the parameters
     new_parameters = []
     for param in data["parameters"]:
         if "metadata" not in param:
             param["metadata"] = {}
         check_json_keys(param, "Parameter")
-        assert param["variable_type"] in ms["Types"], "Type not in ms"
+        assert param["variable_type"] in ms["Types"], "Type of {} not in ms".format(
+            param["variable_type"]
+        )
         param["variable_type"] = ms["Types"][param["variable_type"]]
         new_parameters.append(Parameter(param))
     data["parameters"] = new_parameters
 
     # Build the state object
     return ParameterSet(data)
```

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/policy.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/policy.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/spaces.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/spaces.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/state_update_transmission_channels.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/state_update_transmission_channels.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/stateful_metrics.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/stateful_metrics.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/states.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/states.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/type.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/type.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 def load_typescript_type_key(path):
     with open(path, "r") as file:
         type_definitions = file.read()
     type_definitions = type_definitions.split("\n")
     type_definitions = [x for x in type_definitions if len(x) > 0]
     hold = type_definitions[:]
     type_definitions = []
-    type_definitions.append(hold.pop(0))
+    if len(hold) > 0:
+        type_definitions.append(hold.pop(0))
     while len(hold) > 0:
         curr = hold.pop(0)
         if "type" in curr or "interface" in curr:
             type_definitions.append(curr)
         else:
             type_definitions[-1] += "\n" + curr
```

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/wiring.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/wiring.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/__init__.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/boundary_actions.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/control_actions.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/control_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/general.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/general.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/html.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/html.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/markdown.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,15 +581,15 @@
         if var.symbol:
             out += " , symbol: {}".format(var.symbol)
         out += "\n"
     out += "\n"
 
     out += "## Variables Used\n"
     for i, x in enumerate(metric.variables_used):
-        out += "{}. {}.{}".format(i + 1, x[0], x[1])
+        out += "{}. [[{}]].[[{}-{}|{}]]".format(i + 1, x[0], x[0], x[1], x[1])
         var = ms.state[x[0]].variable_map[x[1]]
         if var.symbol:
             out += " , symbol: {}".format(var.symbol)
         out += "\n"
     out += "\n"
 
     out += "## Domain Spaces\n"
```

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/mechanisms.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/mechanisms.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/node_map.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/node_map.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/parameters.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/parameters.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/policies.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/policies.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/spaces.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/spaces.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/state.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/state.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/tables.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/tables.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/wiring.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/wiring.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/__init__.py` & `math_spec_mapping-0.3.2/src/math_spec_mapping/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,9 +22,10 @@
     write_control_action_markdown_report,
     write_wiring_markdown_report,
     write_parameter_markdown_report,
     write_stateful_metrics_markdown_report,
     write_all_markdown_reports,
 )
 from .schema import schema
+from .Convenience import remove_dummy_repo_components
 
 # from .Convenience import write_top_level_json_description
```

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping/schema.schema.json` & `math_spec_mapping-0.3.2/src/math_spec_mapping/schema.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999779541446209%*

 * *Differences: {"'definitions'": "{'Wiring': {'properties': {'metadata': OrderedDict([('type', 'object')])}}}"}*

```diff
@@ -769,14 +769,17 @@
                 },
                 "loop": {
                     "type": "boolean"
                 },
                 "mermaid_show_name": {
                     "type": "boolean"
                 },
+                "metadata": {
+                    "type": "object"
+                },
                 "name": {
                     "type": "string"
                 },
                 "optional_indices": {
                     "items": {
                         "type": "integer"
                     },
```

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/PKG-INFO` & `math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/SOURCES.txt` & `math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

