# Comparing `tmp/math_spec_mapping-0.3.3.tar.gz` & `tmp/math_spec_mapping-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_spec_mapping-0.3.3.tar", last modified: Wed May 15 18:33:39 2024, max compression
+gzip compressed data, was "math_spec_mapping-0.3.4.tar", last modified: Fri May 17 04:40:05 2024, max compression
```

## Comparing `math_spec_mapping-0.3.3.tar` & `math_spec_mapping-0.3.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.512143 math_spec_mapping-0.3.3/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math_spec_mapping-0.3.3/LICENSE
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-15 18:33:39.511880 math_spec_mapping-0.3.3/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/README.md
--rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-05-12 21:07:44.000000 math_spec_mapping-0.3.3/pyproject.toml
--rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-05-15 18:33:39.512187 math_spec_mapping-0.3.3/setup.cfg
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.500648 math_spec_mapping-0.3.3/src/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.502078 math_spec_mapping-0.3.3/src/math_spec_mapping/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.505586 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    17437 2024-05-15 17:30:11.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Block.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      476 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/BoundaryAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/ControlAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Entity.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    28854 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/MathSpec.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Metric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Parameter.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Space.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1599 2024-05-14 15:58:35.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/State.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/StatefulMetric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/__init__.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.506081 math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      112 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1625 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/documentation.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    11010 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/starter.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.509261 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/
--rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/action_transmission_channel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2142 2024-05-14 16:01:16.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      414 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/displays.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1289 2024-05-14 15:59:52.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/entities.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/implementations.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/load.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3434 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1393 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/state_update_transmission_channels.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/stateful_metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1313 2024-05-12 21:08:43.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/states.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4356 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/wiring.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.511448 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     9007 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/html.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    22881 2024-05-15 17:34:54.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/markdown.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/mechanisms.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/node_map.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/policies.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2321 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/state.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/tables.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/wiring.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      961 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/schema.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    29400 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/schema.schema.json
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.511653 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/requires.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.897089 math_spec_mapping-0.3.4/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math_spec_mapping-0.3.4/LICENSE
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-17 04:40:05.896818 math_spec_mapping-0.3.4/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/README.md
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-05-17 04:30:03.000000 math_spec_mapping-0.3.4/pyproject.toml
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-05-17 04:40:05.897134 math_spec_mapping-0.3.4/setup.cfg
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.886456 math_spec_mapping-0.3.4/src/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.887733 math_spec_mapping-0.3.4/src/math_spec_mapping/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.890972 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    17437 2024-05-15 18:36:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Block.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      593 2024-05-17 03:51:16.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/BoundaryAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/ControlAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Entity.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    32143 2024-05-17 04:00:15.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/MathSpec.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Metric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Parameter.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Space.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1599 2024-05-15 18:36:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/State.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/StatefulMetric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/__init__.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.891408 math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      112 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1625 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/documentation.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    11010 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/starter.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.894121 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/action_transmission_channel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2625 2024-05-17 03:54:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      480 2024-05-17 02:56:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/displays.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1289 2024-05-15 18:36:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/entities.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/implementations.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/load.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3434 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1393 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/state_update_transmission_channels.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/stateful_metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1365 2024-05-17 00:59:42.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/states.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4356 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Load/wiring.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.896332 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     9007 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/html.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    22871 2024-05-16 16:23:01.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/markdown.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/mechanisms.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/node_map.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/policies.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2321 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/state.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/tables.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/wiring.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      961 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/schema.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    30916 2024-05-16 16:43:09.000000 math_spec_mapping-0.3.4/src/math_spec_mapping/schema.schema.json
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-17 04:40:05.896571 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/requires.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-05-17 04:40:05.000000 math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/top_level.txt
```

### Comparing `math_spec_mapping-0.3.3/LICENSE` & `math_spec_mapping-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/PKG-INFO` & `math_spec_mapping-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.3
+Version: 0.3.4
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math_spec_mapping-0.3.3/README.md` & `math_spec_mapping-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/pyproject.toml` & `math_spec_mapping-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "math-spec-mapping"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Sean McOwen", email="Sean@Block.Science" },
 ]
 description = "A library for easy mapping of mathematical specifications."
 dependencies = [
   "graphviz>=0.20.1",
   "ipython>=7.7.0",
```

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Block.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Block.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/ControlAction.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/ControlAction.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Entity.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Entity.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/MathSpec.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/MathSpec.py`

 * *Files 3% similar despite different names*

```diff
@@ -360,15 +360,15 @@
         opts = [
             (x, x.policy_options)
             for x in self.policies.values()
             if len(x.policy_options) > 1
         ]
         opts.extend(
             [
-                (x, x.boundary_actions)
+                (x, x.boundary_action_options)
                 for x in self.boundary_actions.values()
                 if len(x.boundary_action_options) > 1
             ]
         )
         opts.extend(
             [
                 (x, x.control_actions)
@@ -600,14 +600,42 @@
         out += "\n\n"
 
         out += "parameters: Parameters = {**behavioral_parameters, **functional_parameters, **system_parameters}"
 
         with open(path, "w") as f:
             f.write(out)
 
+    def metaprogramming_boundary_actions(
+        self, model_directory, overwrite=False, default_values=None
+    ):
+        path = model_directory + "/boundary_actions.py"
+        if not overwrite:
+            assert "boundary_actions.py" not in os.listdir(
+                model_directory
+            ), "The boundary actions file is already written, either delete it or switch to overwrite mode"
+        out = ""
+
+        unique_spaces = set().union(
+            *[x.all_spaces_used for x in self.boundary_actions.values()]
+        )
+        unique_spaces = [x.name_variable for x in unique_spaces]
+
+        out += "from .spaces import {}".format(", ".join(unique_spaces))
+        out += "\n\n"
+        for x in self.boundary_actions.values():
+            out += "def "
+            out += x.model_name
+            out += "(state, params) -> ({}):".format(
+                ", ".join([y.name_variable for y in x.codomain])
+            )
+            out += "\n\n"
+
+        with open(path, "w") as f:
+            f.write(out)
+
     def metaprogramming_julia_types(self, model_directory, overwrite=False):
         path = model_directory + "/types.jl"
         if not overwrite:
             assert "types.jl" not in os.listdir(
                 model_directory
             ), "The types file is already written, either delete it or switch to overwrite mode"
 
@@ -648,15 +676,15 @@
 
 
 class MathSpecImplementation:
     def __init__(self, ms: MathSpec, params):
         self.ms = deepcopy(ms)
         self.params = params
         self.control_actions = self.load_control_actions()
-        self.boundary_actions = {}
+        self.boundary_actions = self.load_boundary_actions()
         self.policies = self.load_policies()
         self.mechanisms = self.load_mechanisms()
         self.load_wiring()
 
     def load_control_actions(self):
         control_actions = {}
         for ca in self.ms.control_actions:
@@ -666,32 +694,72 @@
                 print("{} has no control action options".format(ca.name))
             else:
                 if len(opts) == 1:
                     opt = opts[0]
                 else:
                     assert (
                         "FP {}".format(ca.name) in self.params
-                    ), "No functional parameterization for {}".format(ca.name)
+                    ), "No functional parameterization for {}. To fix this error, add {} to the parameters passed to ms.build_implementation. Option can be: {}".format(
+                        ca.name, "FP " + ca.name, [x.name for x in opts]
+                    )
                     opt = self.ms.functional_parameters["FP {}".format(ca.name)][
                         self.params["FP {}".format(ca.name)]
                     ]
 
-                assert (
-                    "python" in opt.implementations
-                ), "No python implementation for {} / {}".format(ca.name, opt.name)
-
-                control_actions[ca.name] = opt.implementations["python"]
+                if "python" not in opt.implementations:
+                    print(
+                        "No python implementation for {} / {}. To fix this, go to Implementations/Python/ControlActions and add {}".format(
+                            ca.name, opt.name, opt.name
+                        )
+                    )
+                else:
+                    control_actions[ca.name] = opt.implementations["python"]
         return control_actions
 
+    def load_boundary_actions(self):
+        boundary_actions = {}
+        for ba in self.ms.boundary_actions:
+            ba = self.ms.boundary_actions[ba]
+            opts = ba.boundary_action_options
+            if len(opts) == 0:
+                print("{} has no boundary action options".format(ba.name))
+            else:
+                if len(opts) == 1:
+                    opt = opts[0]
+                else:
+                    assert (
+                        "FP {}".format(ba.name) in self.params
+                    ), "No functional parameterization for {}. To fix this error, add {} to the parameters passed to ms.build_implementation. Option can be: {}".format(
+                        ba.name, ba.name, [x.name for x in opts]
+                    )
+
+                    opt = self.ms.functional_parameters["FP {}".format(ba.name)][
+                        self.params["FP {}".format(ba.name)]
+                    ]
+
+                if "python" not in opt.implementations:
+                    print(
+                        "No python implementation for {} / {}. To fix this, go to Implementations/Python/BoundaryActions and add {}".format(
+                            ba.name, opt.name, opt.name
+                        )
+                    )
+                else:
+                    boundary_actions[ba.name] = opt.implementations["python"]
+        return boundary_actions
+
     def load_mechanisms(self):
         mechanisms = {}
         for m in self.ms.mechanisms:
             m = self.ms.mechanisms[m]
             if "python" not in m.implementations:
-                print("No python implementation for {}".format(m.name))
+                print(
+                    "No python implementation for {}. To fix this, go to Implementations/Python/Mechanisms and add {}".format(
+                        m.name, m.name
+                    )
+                )
             else:
                 mechanisms[m.name] = m.implementations["python"]
         return mechanisms
 
     def load_single_wiring(self, wiring):
         components = [x.name for x in wiring.components]
         if wiring.block_type == "Stack Block":
@@ -733,22 +801,26 @@
                 print("{} has no policy options".format(p.name))
             else:
                 if len(opts) == 1:
                     opt = opts[0]
                 else:
                     assert (
                         "FP {}".format(p.name) in self.params
-                    ), "No functional parameterization for {}".format(p.name)
+                    ), "No functional parameterization for {}. To fix this error, add {} to the parameters passed to ms.build_implementation. Option can be: {}".format(
+                        p.name, p.name, [x.name for x in opts]
+                    )
                     opt = self.ms.functional_parameters["FP {}".format(p.name)][
                         self.params["FP {}".format(p.name)]
                     ]
 
                 if "python" not in opt.implementations:
                     print(
-                        "No python implementation for {} / {}".format(p.name, opt.name)
+                        "No python implementation for {} / {}. To fix this, go to Implementations/Python/Policies and add {}".format(
+                            p.name, opt.name, opt.name
+                        )
                     )
                 else:
                     policies[p.name] = opt.implementations["python"]
         return policies
 
     def load_wiring(
         self,
```

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Metric.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Metric.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Parameter.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Parameter.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Policy.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/Policy.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/State.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/State.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/StatefulMetric.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/StatefulMetric.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/__init__.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Classes/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/documentation.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/documentation.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/starter.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Convenience/starter.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/action_transmission_channel.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/action_transmission_channel.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/boundary_actions.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/boundary_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,25 @@
     # Copy
     data = data.copy()
 
     # Convert the boundary action options
     new_bao = []
     for ba in data["boundary_action_options"]:
         check_json_keys(ba, "Boundary Action Option")
+
+        ba["implementations"] = {}
+        if "python" in ms["Implementations"]:
+            if "boundary_action_options" in ms["Implementations"]["python"]:
+                if (
+                    ba["name"]
+                    in ms["Implementations"]["python"]["boundary_action_options"]
+                ):
+                    ba["implementations"]["python"] = ms["Implementations"]["python"][
+                        "boundary_action_options"
+                    ][ba["name"]]
         new_bao.append(BoundaryActionOption(ba))
     data["boundary_action_options"] = new_bao
 
     # Assert that the entities in called_by are in math spec
     if data["called_by"]:
         for name in data["called_by"]:
             assert (
```

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/control_actions.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/control_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/entities.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/entities.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/general.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/general.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/load.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/load.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/mechanism.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/mechanism.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/metrics.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/metrics.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/parameters.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/parameters.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/policy.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/policy.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/spaces.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/spaces.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/state_update_transmission_channels.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/state_update_transmission_channels.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/stateful_metrics.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/stateful_metrics.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/states.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/states.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,15 +21,17 @@
     # Copy
     data = data.copy()
 
     # Convert the variables
     new_variables = []
     for var in data["variables"]:
         check_json_keys(var, "State Variable")
-        assert var["type"] in ms["Types"], "Type {} not in ms".format(var["name"])
+        assert var["type"] in ms["Types"], "Type {} referenced by {} not in ms".format(
+            var["type"], var["name"]
+        )
         var["type"] = ms["Types"][var["type"]]
         if "metadata" not in var:
             var["metadata"] = {}
         new_variables.append(StateVariable(var))
     data["variables"] = new_variables
 
     # Build the state object
```

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/type.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/type.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/wiring.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Load/wiring.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/__init__.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/boundary_actions.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/control_actions.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/control_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/general.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/general.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/html.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/html.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/markdown.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,15 +573,15 @@
     out += "Symbol: {}\n\n".format(metric.symbol)
 
     out += "## Logic\n"
     out += metric.logic
     out += "\n\n"
 
     out += "## Parameters Used\n"
-    for i, x in enumerate(sorted(metric.parameters_used, key=lambda x: x.name)):
+    for i, x in enumerate(sorted(metric.parameters_used, key=lambda x: x)):
         out += "{}. [[{}]]".format(i + 1, x)
         var = ms.parameters.parameter_map[x]
         if var.symbol:
             out += " , symbol: {}".format(var.symbol)
         out += "\n"
     out += "\n"
 
@@ -707,15 +707,15 @@
         out += "\n"
     out += "\n"""
 
     parameters = [set(x.parameters_used) for x in wirings]
     parameters = set().union(*parameters)
     parameters = sorted(parameters, key=lambda x: x)
     out += "## Unique Parameters Used\n"
-    for i, x in enumerate(sorted(parameters, key=lambda x: x.name)):
+    for i, x in enumerate(sorted(parameters, key=lambda x: x)):
         out += "{}. [[{}]]".format(i + 1, x)
         out += "\n"
     out += "\n"
 
     with open("{}/Displays/Wiring/{}.md".format(path, wiring["name"]), "w") as f:
         f.write(out)
```

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/mechanisms.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/mechanisms.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/node_map.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/node_map.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/parameters.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/parameters.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/policies.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/policies.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/spaces.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/spaces.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/state.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/state.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/tables.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/tables.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/wiring.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/Reports/wiring.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/__init__.py` & `math_spec_mapping-0.3.4/src/math_spec_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping/schema.schema.json` & `math_spec_mapping-0.3.4/src/math_spec_mapping/schema.schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9912996750632621%*

 * *Differences: {"'definitions'": "{'ControlAction': {'properties': {'control_action_options': {'items': {replace: "*

 * *                  "OrderedDict([('$ref', "*

 * *                  "'./schema.schema.json/#/definitions/ControlActionOption')])}}}}, "*

 * *                  "'BoundaryAction': {'properties': {'boundary_action_options': {'items': "*

 * *                  "{replace: OrderedDict([('$ref', "*

 * *                  "'./schema.schema.json/#/definitions/BoundaryActionOption')])}}}}, "*

 * *                  "'BoundaryActionOption': Ordered […]*

```diff
@@ -5,15 +5,17 @@
     "definitions": {
         "BoundaryAction": {
             "additionalProperties": true,
             "description": "The definition of different actions that might happen outside of the system such as customers coming into a shop. Generally will be called by entities.",
             "properties": {
                 "boundary_action_options": {
                     "description": "The options for implementation of the boundary action",
-                    "items": {},
+                    "items": {
+                        "$ref": "./schema.schema.json/#/definitions/BoundaryActionOption"
+                    },
                     "type": "array"
                 },
                 "called_by": {
                     "description": "The entities which are allowed to call this boundary action",
                     "items": {
                         "type": "string"
                     },
@@ -57,14 +59,42 @@
                 "description",
                 "name",
                 "parameters_used"
             ],
             "title": "Boundary Action",
             "type": "object"
         },
+        "BoundaryActionOption": {
+            "additionalProperties": false,
+            "description": "Specific implementations of a control action which are in the same form of the underlying control action definition.",
+            "properties": {
+                "description": {
+                    "description": "A description of what this implementation does",
+                    "type": "string"
+                },
+                "logic": {
+                    "description": "The logic related to the implementation",
+                    "type": "string"
+                },
+                "metadata": {
+                    "type": "object"
+                },
+                "name": {
+                    "description": "The name of the boundary action option",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "name",
+                "description",
+                "logic"
+            ],
+            "title": "BoundaryActionOption",
+            "type": "object"
+        },
         "ControlAction": {
             "additionalProperties": false,
             "description": "The definition of actions that the system might call, such as an action to refill the stock of an item when reserves run too low or something that could get triggered from a sensor. The key differentiator from boundary actions is that there is no entity calling it and it is not done with randomness.",
             "properties": {
                 "codomain": {
                     "description": "The output spaces of the control action",
                     "items": {
@@ -77,15 +107,17 @@
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "control_action_options": {
                     "description": "Possible implementations of the control action",
-                    "items": {},
+                    "items": {
+                        "$ref": "./schema.schema.json/#/definitions/ControlActionOption"
+                    },
                     "type": "array"
                 },
                 "description": {
                     "description": "The description of the control action",
                     "type": "string"
                 },
                 "name": {
@@ -107,14 +139,42 @@
                 "description",
                 "name",
                 "parameters_used"
             ],
             "title": "ControlAction",
             "type": "object"
         },
+        "ControlActionOption": {
+            "additionalProperties": false,
+            "description": "Specific implementations of a control action which are in the same form of the underlying control action definition.",
+            "properties": {
+                "description": {
+                    "description": "A description of what this implementation does",
+                    "type": "string"
+                },
+                "logic": {
+                    "description": "The logic related to the implementation",
+                    "type": "string"
+                },
+                "metadata": {
+                    "type": "object"
+                },
+                "name": {
+                    "description": "The name of the control action option",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "name",
+                "description",
+                "logic"
+            ],
+            "title": "ControlActionOption",
+            "type": "object"
+        },
         "Entity": {
             "additionalProperties": false,
             "description": "Entities are any class of user or infrastructure that should have their own state and potentially ability to call boundary actions. Examples could be a customer or a company (for which a simulation might assume it is acting as one cohesive unit)",
             "properties": {
                 "metadata": {
                     "type": "object"
                 },
```

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/PKG-INFO` & `math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.3
+Version: 0.3.4
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/SOURCES.txt` & `math_spec_mapping-0.3.4/src/math_spec_mapping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

