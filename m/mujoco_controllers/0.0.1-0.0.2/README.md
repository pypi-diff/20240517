# Comparing `tmp/mujoco_controllers-0.0.1.tar.gz` & `tmp/mujoco_controllers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mujoco_controllers-0.0.1.tar", max compression
+gzip compressed data, was "mujoco_controllers-0.0.2.tar", max compression
```

## Comparing `mujoco_controllers-0.0.1.tar` & `mujoco_controllers-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,136 @@
--rw-r--r--   0        0        0    11357 2024-05-13 12:33:16.770188 mujoco_controllers-0.0.1/LICENSE
--rw-r--r--   0        0        0      798 2024-05-13 12:33:16.770188 mujoco_controllers-0.0.1/README.md
--rw-r--r--   0        0        0     1212 2024-05-13 12:33:16.770188 mujoco_controllers-0.0.1/mujoco_controllers/README.md
--rw-r--r--   0        0        0      296 2024-05-13 12:33:16.770188 mujoco_controllers-0.0.1/mujoco_controllers/__init__.py
--rw-r--r--   0        0        0     9731 2024-05-13 12:33:16.770188 mujoco_controllers-0.0.1/mujoco_controllers/build_env.py
--rw-r--r--   0        0        0      500 2024-05-13 12:33:16.770188 mujoco_controllers-0.0.1/mujoco_controllers/config/arena/cameras/transporter_data_collection.yaml
--rw-r--r--   0        0        0      251 2024-05-13 12:33:16.770188 mujoco_controllers-0.0.1/mujoco_controllers/config/arena/props/default.yaml
--rw-r--r--   0        0        0      224 2024-05-13 12:33:16.770188 mujoco_controllers-0.0.1/mujoco_controllers/config/arena/props/single_block.yaml
--rw-r--r--   0        0        0       70 2024-05-13 12:33:16.770188 mujoco_controllers-0.0.1/mujoco_controllers/config/arena/rearrangement_table.yaml
--rw-r--r--   0        0        0      310 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/itl_rearrangement.yaml
--rw-r--r--   0        0        0     1465 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/actuator_config/intvelocity.yaml
--rw-r--r--   0        0        0      326 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/actuator_config/motor.yaml
--rw-r--r--   0        0        0     1029 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/actuator_config/velocity.yaml
--rw-r--r--   0        0        0      315 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/controller_config/diffik.yaml
--rw-r--r--   0        0        0      603 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/controller_config/osc.yaml
--rw-r--r--   0        0        0      630 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/franka_emika_panda.yaml
--rw-r--r--   0        0        0      531 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/sensor_config/position.yaml
--rw-r--r--   0        0        0       25 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/end_effector/actuator_config/default.yaml
--rw-r--r--   0        0        0       90 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/end_effector/controller_config/min_max.yaml
--rw-r--r--   0        0        0      419 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/end_effector/robotiq_2f85.yaml
--rw-r--r--   0        0        0       25 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/end_effector/sensor_config/default.yaml
--rw-r--r--   0        0        0       69 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/robots/franka_robotiq_2f85.yaml
--rw-r--r--   0        0        0      207 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/config/task/itl_rearrangement.yaml
--rw-r--r--   0        0        0     9612 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/diffik.py
--rw-r--r--   0        0        0      901 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/min_max.py
--rw-r--r--   0        0        0       30 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/arenas/__init__.py
--rw-r--r--   0        0        0     1647 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/arenas/empty.py
--rw-r--r--   0        0        0      934 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/arenas/empty_assets/arena.xml
--rw-r--r--   0        0        0       23 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/arms/__init__.py
--rw-r--r--   0        0        0     5000 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/arms/franka_emika.py
--rw-r--r--   0        0        0     1970 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/arms/robot_arm.py
--rw-r--r--   0        0        0        0 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/end_effectors/__init__.py
--rw-r--r--   0        0        0     2686 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/end_effectors/robot_hand.py
--rw-r--r--   0        0        0     2080 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/end_effectors/robotiq_2f85.py
--rw-r--r--   0        0        0     3309 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/models/robot_arm.py
--rw-r--r--   0        0        0    11547 2024-05-13 12:33:16.774188 mujoco_controllers-0.0.1/mujoco_controllers/osc.py
--rw-r--r--   0        0        0     1140 2024-05-13 14:50:34.765605 mujoco_controllers-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 mujoco_controllers-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-17 09:01:34.017960 mujoco_controllers-0.0.2/LICENSE
+-rw-r--r--   0        0        0      798 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/README.md
+-rw-r--r--   0        0        0     1212 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/README.md
+-rw-r--r--   0        0        0      296 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/__init__.py
+-rw-r--r--   0        0        0     9731 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/build_env.py
+-rw-r--r--   0        0        0      500 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/arena/cameras/transporter_data_collection.yaml
+-rw-r--r--   0        0        0      251 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/arena/props/default.yaml
+-rw-r--r--   0        0        0      224 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/arena/props/single_block.yaml
+-rw-r--r--   0        0        0       70 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/arena/rearrangement_table.yaml
+-rw-r--r--   0        0        0      310 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/itl_rearrangement.yaml
+-rw-r--r--   0        0        0     1465 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/actuator_config/intvelocity.yaml
+-rw-r--r--   0        0        0      326 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/actuator_config/motor.yaml
+-rw-r--r--   0        0        0     1029 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/actuator_config/velocity.yaml
+-rw-r--r--   0        0        0      315 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/controller_config/diffik.yaml
+-rw-r--r--   0        0        0      603 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/controller_config/osc.yaml
+-rw-r--r--   0        0        0      630 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/franka_emika_panda.yaml
+-rw-r--r--   0        0        0      531 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/sensor_config/position.yaml
+-rw-r--r--   0        0        0       25 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/end_effector/actuator_config/default.yaml
+-rw-r--r--   0        0        0       90 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/end_effector/controller_config/min_max.yaml
+-rw-r--r--   0        0        0      419 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/end_effector/robotiq_2f85.yaml
+-rw-r--r--   0        0        0       25 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/end_effector/sensor_config/default.yaml
+-rw-r--r--   0        0        0       69 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/robots/franka_robotiq_2f85.yaml
+-rw-r--r--   0        0        0      207 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/config/task/itl_rearrangement.yaml
+-rw-r--r--   0        0        0     9612 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/diffik.py
+-rw-r--r--   0        0        0      901 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/min_max.py
+-rw-r--r--   0        0        0       30 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/arenas/__init__.py
+-rw-r--r--   0        0        0     1647 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/arenas/empty.py
+-rw-r--r--   0        0        0      934 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/arenas/empty_assets/arena.xml
+-rw-r--r--   0        0        0       23 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/arms/__init__.py
+-rw-r--r--   0        0        0     5000 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/arms/franka_emika.py
+-rw-r--r--   0        0        0     1970 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/arms/robot_arm.py
+-rw-r--r--   0        0        0        0 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/end_effectors/__init__.py
+-rw-r--r--   0        0        0     2686 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/end_effectors/robot_hand.py
+-rw-r--r--   0        0        0     2080 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/end_effectors/robotiq_2f85.py
+-rw-r--r--   0        0        0     3309 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/models/robot_arm.py
+-rw-r--r--   0        0        0       63 2024-05-17 09:04:10.406508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/.git
+-rw-r--r--   0        0        0      293 2024-05-17 09:04:10.418507 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      600 2024-05-17 09:04:10.418507 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/.github/ISSUE_TEMPLATE/model_addition.md
+-rw-r--r--   0        0        0      632 2024-05-17 09:04:10.418507 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/.github/workflows/build.yml
+-rw-r--r--   0        0        0      243 2024-05-17 09:04:10.418507 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/CITATION.cff
+-rw-r--r--   0        0        0     3234 2024-05-17 09:04:10.418507 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1688 2024-05-17 09:04:10.418507 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/FAQ.md
+-rw-r--r--   0        0        0   123264 2024-05-17 09:04:10.418507 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/LICENSE
+-rw-r--r--   0        0        0    10074 2024-05-17 09:04:10.418507 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/README.md
+-rw-r--r--   0        0        0   118412 2024-05-17 09:04:10.630508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/banner.png
+-rw-r--r--   0        0        0    10173 2024-05-17 09:04:10.630508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/LICENSE
+-rw-r--r--   0        0        0     2236 2024-05-17 09:04:10.630508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/README.md
+-rw-r--r--   0        0        0    87872 2024-05-17 09:04:10.630508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/finger_0.obj
+-rw-r--r--   0        0        0    64651 2024-05-17 09:04:10.630508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/finger_1.obj
+-rw-r--r--   0        0        0    10084 2024-05-17 09:04:10.630508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/hand.stl
+-rw-r--r--   0        0        0     9091 2024-05-17 09:04:10.630508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/hand_0.obj
+-rw-r--r--   0        0        0   121863 2024-05-17 09:04:10.630508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/hand_1.obj
+-rw-r--r--   0        0        0   596001 2024-05-17 09:04:10.630508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/hand_2.obj
+-rw-r--r--   0        0        0   902145 2024-05-17 09:04:10.634508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/hand_3.obj
+-rw-r--r--   0        0        0   151988 2024-05-17 09:04:10.634508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/hand_4.obj
+-rw-r--r--   0        0        0    10084 2024-05-17 09:04:10.634508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0.stl
+-rw-r--r--   0        0        0   296497 2024-05-17 09:04:10.634508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_0.obj
+-rw-r--r--   0        0        0   103978 2024-05-17 09:04:10.634508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_1.obj
+-rw-r--r--   0        0        0   343308 2024-05-17 09:04:10.634508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_10.obj
+-rw-r--r--   0        0        0    22295 2024-05-17 09:04:10.634508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_11.obj
+-rw-r--r--   0        0        0   590892 2024-05-17 09:04:10.638508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_2.obj
+-rw-r--r--   0        0        0    47588 2024-05-17 09:04:10.638508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_3.obj
+-rw-r--r--   0        0        0   211200 2024-05-17 09:04:10.638508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_4.obj
+-rw-r--r--   0        0        0    17023 2024-05-17 09:04:10.638508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_5.obj
+-rw-r--r--   0        0        0    30699 2024-05-17 09:04:10.638508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_7.obj
+-rw-r--r--   0        0        0  3263194 2024-05-17 09:04:10.646508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_8.obj
+-rw-r--r--   0        0        0   105629 2024-05-17 09:04:10.646508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link0_9.obj
+-rw-r--r--   0        0        0  3274995 2024-05-17 09:04:10.654508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link1.obj
+-rw-r--r--   0        0        0    15084 2024-05-17 09:04:10.654508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link1.stl
+-rw-r--r--   0        0        0  3295608 2024-05-17 09:04:10.662509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link2.obj
+-rw-r--r--   0        0        0    15084 2024-05-17 09:04:10.662509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link2.stl
+-rw-r--r--   0        0        0    15084 2024-05-17 09:04:10.662509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link3.stl
+-rw-r--r--   0        0        0  3046804 2024-05-17 09:04:10.670508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link3_0.obj
+-rw-r--r--   0        0        0    65260 2024-05-17 09:04:10.670508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link3_1.obj
+-rw-r--r--   0        0        0    83591 2024-05-17 09:04:10.670508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link3_2.obj
+-rw-r--r--   0        0        0   457684 2024-05-17 09:04:10.670508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link3_3.obj
+-rw-r--r--   0        0        0    15084 2024-05-17 09:04:10.670508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link4.stl
+-rw-r--r--   0        0        0    83486 2024-05-17 09:04:10.670508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link4_0.obj
+-rw-r--r--   0        0        0  3148001 2024-05-17 09:04:10.678509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link4_1.obj
+-rw-r--r--   0        0        0   455522 2024-05-17 09:04:10.678509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link4_2.obj
+-rw-r--r--   0        0        0    67497 2024-05-17 09:04:10.678509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link4_3.obj
+-rw-r--r--   0        0        0   824158 2024-05-17 09:04:10.682509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link5_0.obj
+-rw-r--r--   0        0        0    63174 2024-05-17 09:04:10.682509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link5_1.obj
+-rw-r--r--   0        0        0  3856621 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link5_2.obj
+-rw-r--r--   0        0        0     3861 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link5_collision_0.obj
+-rw-r--r--   0        0        0     2412 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link5_collision_1.obj
+-rw-r--r--   0        0        0     3786 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link5_collision_2.obj
+-rw-r--r--   0        0        0    10084 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6.stl
+-rw-r--r--   0        0        0   157563 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_0.obj
+-rw-r--r--   0        0        0    27106 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_1.obj
+-rw-r--r--   0        0        0   368502 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_10.obj
+-rw-r--r--   0        0        0    32653 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_11.obj
+-rw-r--r--   0        0        0     3894 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_12.obj
+-rw-r--r--   0        0        0     3798 2024-05-17 09:04:10.690508 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_13.obj
+-rw-r--r--   0        0        0   444469 2024-05-17 09:04:10.694509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_14.obj
+-rw-r--r--   0        0        0   668552 2024-05-17 09:04:10.694509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_15.obj
+-rw-r--r--   0        0        0  3675358 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_16.obj
+-rw-r--r--   0        0        0     9916 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_2.obj
+-rw-r--r--   0        0        0    11943 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_3.obj
+-rw-r--r--   0        0        0    13846 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_4.obj
+-rw-r--r--   0        0        0    11841 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_5.obj
+-rw-r--r--   0        0        0    12597 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_6.obj
+-rw-r--r--   0        0        0     4382 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_7.obj
+-rw-r--r--   0        0        0     9131 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_8.obj
+-rw-r--r--   0        0        0    17616 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link6_9.obj
+-rw-r--r--   0        0        0    10084 2024-05-17 09:04:10.702509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link7.stl
+-rw-r--r--   0        0        0  1362355 2024-05-17 09:04:10.706509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link7_0.obj
+-rw-r--r--   0        0        0   121358 2024-05-17 09:04:10.706509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link7_1.obj
+-rw-r--r--   0        0        0   208907 2024-05-17 09:04:10.706509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link7_2.obj
+-rw-r--r--   0        0        0   123684 2024-05-17 09:04:10.706509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link7_3.obj
+-rw-r--r--   0        0        0    85732 2024-05-17 09:04:10.706509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link7_4.obj
+-rw-r--r--   0        0        0   226402 2024-05-17 09:04:10.706509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link7_5.obj
+-rw-r--r--   0        0        0    99900 2024-05-17 09:04:10.706509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link7_6.obj
+-rw-r--r--   0        0        0   792162 2024-05-17 09:04:10.710509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/assets/link7_7.obj
+-rw-r--r--   0        0        0     4547 2024-05-17 09:04:10.710509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/hand.xml
+-rw-r--r--   0        0        0  2192427 2024-05-17 09:04:10.718509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/panda.png
+-rw-r--r--   0        0        0    14369 2024-05-17 09:04:10.718509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/panda.xml
+-rw-r--r--   0        0        0     9699 2024-05-17 09:04:10.718509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/panda_nohand.xml
+-rw-r--r--   0        0        0      867 2024-05-17 09:04:10.718509 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/franka_emika_panda/scene.xml
+-rw-r--r--   0        0        0  1140430 2024-05-17 09:04:11.122510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/2f85.png
+-rw-r--r--   0        0        0     9463 2024-05-17 09:04:11.122510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/2f85.xml
+-rw-r--r--   0        0        0     1297 2024-05-17 09:04:11.122510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/LICENSE
+-rw-r--r--   0        0        0     1269 2024-05-17 09:04:11.122510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/README.md
+-rw-r--r--   0        0        0  1712484 2024-05-17 09:04:11.126510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/assets/base.stl
+-rw-r--r--   0        0        0  1091784 2024-05-17 09:04:11.126510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/assets/base_mount.stl
+-rw-r--r--   0        0        0    89084 2024-05-17 09:04:11.126510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/assets/coupler.stl
+-rw-r--r--   0        0        0    67084 2024-05-17 09:04:11.126510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/assets/driver.stl
+-rw-r--r--   0        0        0   110484 2024-05-17 09:04:11.130510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/assets/follower.stl
+-rw-r--r--   0        0        0    15084 2024-05-17 09:04:11.130510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/assets/pad.stl
+-rw-r--r--   0        0        0    15084 2024-05-17 09:04:11.130510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/assets/silicone_pad.stl
+-rw-r--r--   0        0        0    84884 2024-05-17 09:04:11.130510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/assets/spring_link.stl
+-rw-r--r--   0        0        0     1442 2024-05-17 09:04:11.130510 mujoco_controllers-0.0.2/mujoco_controllers/mujoco_menagerie/robotiq_2f85/scene.xml
+-rw-r--r--   0        0        0    11547 2024-05-17 09:01:34.021960 mujoco_controllers-0.0.2/mujoco_controllers/osc.py
+-rw-r--r--   0        0        0     1143 2024-05-17 09:04:59.630693 mujoco_controllers-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 mujoco_controllers-0.0.2/PKG-INFO
```

### Comparing `mujoco_controllers-0.0.1/LICENSE` & `mujoco_controllers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/README.md` & `mujoco_controllers-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/README.md` & `mujoco_controllers-0.0.2/mujoco_controllers/README.md`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/build_env.py` & `mujoco_controllers-0.0.2/mujoco_controllers/build_env.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/actuator_config/intvelocity.yaml` & `mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/actuator_config/intvelocity.yaml`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/actuator_config/velocity.yaml` & `mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/actuator_config/velocity.yaml`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/controller_config/osc.yaml` & `mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/controller_config/osc.yaml`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/franka_emika_panda.yaml` & `mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/franka_emika_panda.yaml`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/config/robots/arm/sensor_config/position.yaml` & `mujoco_controllers-0.0.2/mujoco_controllers/config/robots/arm/sensor_config/position.yaml`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/diffik.py` & `mujoco_controllers-0.0.2/mujoco_controllers/diffik.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/min_max.py` & `mujoco_controllers-0.0.2/mujoco_controllers/min_max.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/models/arenas/empty.py` & `mujoco_controllers-0.0.2/mujoco_controllers/models/arenas/empty.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/models/arenas/empty_assets/arena.xml` & `mujoco_controllers-0.0.2/mujoco_controllers/models/arenas/empty_assets/arena.xml`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/models/arms/franka_emika.py` & `mujoco_controllers-0.0.2/mujoco_controllers/models/arms/franka_emika.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/models/arms/robot_arm.py` & `mujoco_controllers-0.0.2/mujoco_controllers/models/arms/robot_arm.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/models/end_effectors/robot_hand.py` & `mujoco_controllers-0.0.2/mujoco_controllers/models/end_effectors/robot_hand.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/models/end_effectors/robotiq_2f85.py` & `mujoco_controllers-0.0.2/mujoco_controllers/models/end_effectors/robotiq_2f85.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/models/robot_arm.py` & `mujoco_controllers-0.0.2/mujoco_controllers/models/robot_arm.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/mujoco_controllers/osc.py` & `mujoco_controllers-0.0.2/mujoco_controllers/osc.py`

 * *Files identical despite different names*

### Comparing `mujoco_controllers-0.0.1/pyproject.toml` & `mujoco_controllers-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mujoco_controllers"
-version = "0.0.1"
+version = "0.0.2"
 description = "A repository for debugging controller implementations applied to mujoco models."
 authors = [
 	{ name = "Peter David Fagan", email = "peterdavidfagan@gmail.com" }
 ]
 readme = "README.md"
 
 [tool.poetry]
 name = "mujoco_controllers"
-version = "0.0.1"
+version = "0.0.2"
 description = "A repository for debugging controller implementations applied to mujoco models."
 license = "Apache-2.0"
 authors = [
 	"Peter David Fagan <peterdavidfagan@gmail.com>"
 ]
 readme = "README.md"
 packages = [
 	{include = "mujoco_controllers"}
 ]
 
 [tool.setuptools]
 py-modules=["mujoco_controllers"]
 
 [tool.poetry.dependencies]
-python = "3.10.6"
+python = "^3.10.6"
 numpy = "^1.16.0"
-mujoco = "3.1.1"
-dm-control = "1.0.16"
+mujoco = "^3.1.1"
+dm-control = "^1.0.16"
 pillow = "10.0.0"
 jax = "^0.4.14"
 matplotlib = "^3.7.2"
 hydra-core = "^1.3.2"
 pytest = "^7.4.2"
 lark = "^1.1.7"
 profilehooks = "^1.12.0"
```

### Comparing `mujoco_controllers-0.0.1/PKG-INFO` & `mujoco_controllers-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: mujoco_controllers
-Version: 0.0.1
+Version: 0.0.2
 Summary: A repository for debugging controller implementations applied to mujoco models.
 License: Apache-2.0
 Author: Peter David Fagan
 Author-email: peterdavidfagan@gmail.com
-Requires-Python: ==3.10.6
+Requires-Python: >=3.10.6,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: dm-control (==1.0.16)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dm-control (>=1.0.16,<2.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: ipywidgets (>=8.1.1,<9.0.0)
 Requires-Dist: jax (>=0.4.14,<0.5.0)
 Requires-Dist: jaxopt (>=0.8.2,<0.9.0)
 Requires-Dist: jupyterlab (>=4.0.9,<5.0.0)
 Requires-Dist: lark (>=1.1.7,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
-Requires-Dist: mujoco (==3.1.1)
+Requires-Dist: mujoco (>=3.1.1,<4.0.0)
 Requires-Dist: notebook (>=7.0.6,<8.0.0)
 Requires-Dist: numpy (>=1.16.0,<2.0.0)
 Requires-Dist: pandas (>=2.1.3,<3.0.0)
 Requires-Dist: pillow (==10.0.0)
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: profilehooks (>=1.12.0,<2.0.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
```

