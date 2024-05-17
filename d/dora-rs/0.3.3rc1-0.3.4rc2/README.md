# Comparing `tmp/dora_rs-0.3.3rc1.tar.gz` & `tmp/dora_rs-0.3.4rc2.tar.gz`

## Comparing `dora_rs-0.3.3rc1.tar` & `dora_rs-0.3.4rc2.tar`

### file list

```diff
@@ -1,117 +1,120 @@
--rw-r--r--   0     1001      127      323 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/Cargo.toml
--rw-r--r--   0     1001      127     5495 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/src/from_impls.rs
--rw-r--r--   0     1001      127     3744 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/src/into_impls.rs
--rw-r--r--   0     1001      127      485 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/src/lib.rs
--rw-r--r--   0     1001      127      452 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/download/Cargo.toml
--rw-r--r--   0     1001      127     1285 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/download/src/lib.rs
--rw-r--r--   0     1001      127      461 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/operator/types/Cargo.toml
--rw-r--r--   0     1001      127     4911 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/operator/types/src/lib.rs
--rw-r--r--   0     1001      127      288 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/Cargo.toml
--rw-r--r--   0     1001      127      787 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/build.rs
--rw-r--r--   0     1001      127    10910 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs
--rw-r--r--   0     1001      127     3703 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs
--rw-r--r--   0     1001      127     2848 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs
--rw-r--r--   0     1001      127      776 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs
--rw-r--r--   0     1001      127     2257 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs
--rw-r--r--   0     1001      127     9363 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs
--rw-r--r--   0     1001      127     4376 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs
--rw-r--r--   0     1001      127     4024 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs
--rw-r--r--   0     1001      127      191 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/mod.rs
--rw-r--r--   0     1001      127     4327 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs
--rw-r--r--   0     1001      127     2607 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs
--rw-r--r--   0     1001      127    10849 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs
--rw-r--r--   0     1001      127     7208 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs
--rw-r--r--   0     1001      127     1942 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs
--rw-r--r--   0     1001      127     4429 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs
--rw-r--r--   0     1001      127    20805 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs
--rw-r--r--   0     1001      127      299 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/mod.rs
--rw-r--r--   0     1001      127     3789 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs
--rw-r--r--   0     1001      127    12158 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs
--rw-r--r--   0     1001      127     3382 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs
--rw-r--r--   0     1001      127    11907 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs
--rw-r--r--   0     1001      127      100 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/action/Fibonacci.action
--rw-r--r--   0     1001      127     1271 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg
--rw-r--r--   0     1001      127      240 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BasicTypes.msg
--rw-r--r--   0     1001      127     1346 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg
--rw-r--r--   0     1001      127      315 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Constants.msg
--rw-r--r--   0     1001      127      315 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Defaults.msg
--rw-r--r--   0     1001      127        0 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Empty.msg
--rw-r--r--   0     1001      127      484 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/MultiNested.msg
--rw-r--r--   0     1001      127       29 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Nested.msg
--rw-r--r--   0     1001      127      591 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg
--rw-r--r--   0     1001      127     1255 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg
--rw-r--r--   0     1001      127      415 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/WStrings.msg
--rw-r--r--   0     1001      127     2282 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv
--rw-r--r--   0     1001      127      524 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv
--rw-r--r--   0     1001      127        4 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Empty.srv
--rw-r--r--   0     1001      127      593 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/Cargo.toml
--rw-r--r--   0     1001      127     3249 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/src/bin/bench.rs
--rw-r--r--   0     1001      127     7343 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/src/channel.rs
--rw-r--r--   0     1001      127     2019 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/src/lib.rs
--rw-r--r--   0     1001      127      733 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/Cargo.toml
--rw-r--r--   0     1001      127     2429 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/mod.rs
--rw-r--r--   0     1001      127     2149 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/tcp.rs
--rw-r--r--   0     1001      127     3457 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/event.rs
--rw-r--r--   0     1001      127     3100 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/merged.rs
--rw-r--r--   0     1001      127     8375 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/mod.rs
--rw-r--r--   0     1001      127     9280 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/thread.rs
--rw-r--r--   0     1001      127      764 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/lib.rs
--rw-r--r--   0     1001      127     2553 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/arrow_utils.rs
--rw-r--r--   0     1001      127     3654 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/control_channel.rs
--rw-r--r--   0     1001      127     5795 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/drop_stream.rs
--rw-r--r--   0     1001      127    14352 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/mod.rs
--rw-r--r--   0     1001      127      561 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/Cargo.toml
--rw-r--r--   0     1001      127     1836 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/src/lib.rs
--rw-r--r--   0     1001      127      424 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/Cargo.toml
--rw-r--r--   0     1001      127     9105 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/lib.rs
--rw-r--r--   0     1001      127     3515 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/qos.rs
--rw-r--r--   0     1001      127      729 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs
--rw-r--r--   0     1001      127     6330 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs
--rw-r--r--   0     1001      127     4726 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs
--rw-r--r--   0     1001      127     6326 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs
--rw-r--r--   0     1001      127     1154 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs
--rw-r--r--   0     1001      127     4263 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/mod.rs
--rw-r--r--   0     1001      127     9390 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs
--rw-r--r--   0     1001      127     9481 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs
--rw-r--r--   0     1001      127     7776 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs
--rw-r--r--   0     1001      127     3086 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs
--rw-r--r--   0     1001      127     9552 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs
--rw-r--r--   0     1001      127    11898 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/test_utils.py
--rw-r--r--   0     1001      127      451 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/message/Cargo.toml
--rw-r--r--   0     1001      127     4223 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/message/src/lib.rs
--rw-r--r--   0     1001      127      549 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/operator/Cargo.toml
--rw-r--r--   0     1001      127     7968 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/operator/src/lib.rs
--rw-r--r--   0     1001      127      665 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/Cargo.toml
--rw-r--r--   0     1001      127     9127 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/config.rs
--rw-r--r--   0     1001      127      957 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/coordinator_messages.rs
--rw-r--r--   0     1001      127     6944 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/daemon_messages.rs
--rw-r--r--   0     1001      127    10351 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/descriptor/mod.rs
--rw-r--r--   0     1001      127     7260 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/descriptor/validate.rs
--rw-r--r--   0     1001      127     7349 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/descriptor/visualize.rs
--rw-r--r--   0     1001      127     2397 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/lib.rs
--rw-r--r--   0     1001      127     2066 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/topics.rs
--rw-r--r--   0     1001      127     1431 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/Cargo.toml
--rw-r--r--   0     1001      127    13120 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/lib.rs
--rw-r--r--   0     1001      127     4296 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/channel.rs
--rw-r--r--   0     1001      127     2639 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/mod.rs
--rw-r--r--   0     1001      127    15169 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/python.rs
--rw-r--r--   0     1001      127    10280 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/shared_lib.rs
--rw-r--r--   0     1001      127      583 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/Cargo.toml
--rw-r--r--   0     1001      127     1620 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/lib.rs
--rw-r--r--   0     1001      127     2388 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/telemetry.rs
--rw-r--r--   0     1001      127     1364 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/Cargo.toml
--rw-r--r--   0     1001      127     1493 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/build.rs
--rw-r--r--   0     1001      127      276 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/mod.rs
--rw-r--r--   0     1001      127     4114 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/sequence.rs
--rw-r--r--   0     1001      127     5495 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/string.rs
--rw-r--r--   0     1001      127     2337 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/traits.rs
--rw-r--r--   0     1001      127      223 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/lib.rs
--rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/apis/python/node/Cargo.toml
--rw-r--r--   0     1001      127      201 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/node/README.md
--rw-r--r--   0     1001      127      518 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/node/dora/__init__.py
--rw-r--r--   0     1001      127     6852 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/node/src/lib.rs
--rw-r--r--   0     1001      127   169924 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/Cargo.lock
--rw-r--r--   0        0        0     3959 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/Cargo.toml
--rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/pyproject.toml
--rw-r--r--   0     1001      127      518 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/dora/__init__.py
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/PKG-INFO
+-rw-r--r--   0     1001      127      549 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/operator/Cargo.toml
+-rw-r--r--   0     1001      127     8166 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/operator/src/lib.rs
+-rw-r--r--   0     1001      127     1213 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/Cargo.toml
+-rw-r--r--   0     1001      127     1483 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/build.rs
+-rw-r--r--   0     1001      127      276 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/mod.rs
+-rw-r--r--   0     1001      127     4114 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/sequence.rs
+-rw-r--r--   0     1001      127     5540 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/string.rs
+-rw-r--r--   0     1001      127     2337 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/traits.rs
+-rw-r--r--   0     1001      127      262 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/lib.rs
+-rw-r--r--   0     1001      127      665 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/Cargo.toml
+-rw-r--r--   0     1001      127     9127 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/config.rs
+-rw-r--r--   0     1001      127      922 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/coordinator_messages.rs
+-rw-r--r--   0     1001      127     7006 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/daemon_messages.rs
+-rw-r--r--   0     1001      127    11553 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/descriptor/mod.rs
+-rw-r--r--   0     1001      127     7331 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/descriptor/validate.rs
+-rw-r--r--   0     1001      127     7349 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/descriptor/visualize.rs
+-rw-r--r--   0     1001      127     2397 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/lib.rs
+-rw-r--r--   0     1001      127     2170 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/topics.rs
+-rw-r--r--   0     1001      127      452 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/download/Cargo.toml
+-rw-r--r--   0     1001      127     1285 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/download/src/lib.rs
+-rw-r--r--   0     1001      127      561 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/metrics/Cargo.toml
+-rw-r--r--   0     1001      127     1828 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/metrics/src/lib.rs
+-rw-r--r--   0     1001      127      322 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/Cargo.toml
+-rw-r--r--   0     1001      127      787 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/build.rs
+-rw-r--r--   0     1001      127    11235 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs
+-rw-r--r--   0     1001      127     3703 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs
+-rw-r--r--   0     1001      127     2848 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs
+-rw-r--r--   0     1001      127      776 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs
+-rw-r--r--   0     1001      127     2257 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs
+-rw-r--r--   0     1001      127     9397 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs
+-rw-r--r--   0     1001      127     4376 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs
+-rw-r--r--   0     1001      127     4024 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs
+-rw-r--r--   0     1001      127      191 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/mod.rs
+-rw-r--r--   0     1001      127     3354 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs
+-rw-r--r--   0     1001      127     2607 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs
+-rw-r--r--   0     1001      127    10878 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs
+-rw-r--r--   0     1001      127     7208 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs
+-rw-r--r--   0     1001      127     1910 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs
+-rw-r--r--   0     1001      127     4429 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs
+-rw-r--r--   0     1001      127    20805 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs
+-rw-r--r--   0     1001      127      299 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/mod.rs
+-rw-r--r--   0     1001      127     3790 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs
+-rw-r--r--   0     1001      127    12149 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs
+-rw-r--r--   0     1001      127     3382 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs
+-rw-r--r--   0     1001      127    11907 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs
+-rw-r--r--   0     1001      127      100 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/action/Fibonacci.action
+-rw-r--r--   0     1001      127     1271 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg
+-rw-r--r--   0     1001      127      240 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BasicTypes.msg
+-rw-r--r--   0     1001      127     1346 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg
+-rw-r--r--   0     1001      127      315 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Constants.msg
+-rw-r--r--   0     1001      127      315 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Defaults.msg
+-rw-r--r--   0     1001      127        0 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Empty.msg
+-rw-r--r--   0     1001      127      484 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/MultiNested.msg
+-rw-r--r--   0     1001      127       29 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Nested.msg
+-rw-r--r--   0     1001      127      591 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg
+-rw-r--r--   0     1001      127     1255 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg
+-rw-r--r--   0     1001      127      415 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/WStrings.msg
+-rw-r--r--   0     1001      127     2282 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv
+-rw-r--r--   0     1001      127      524 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv
+-rw-r--r--   0     1001      127        4 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Empty.srv
+-rw-r--r--   0     1001      127      733 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/Cargo.toml
+-rw-r--r--   0     1001      127     2429 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/daemon_connection/mod.rs
+-rw-r--r--   0     1001      127     2149 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/daemon_connection/tcp.rs
+-rw-r--r--   0     1001      127     3457 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/event.rs
+-rw-r--r--   0     1001      127     3100 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/merged.rs
+-rw-r--r--   0     1001      127     8375 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/mod.rs
+-rw-r--r--   0     1001      127     9280 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/thread.rs
+-rw-r--r--   0     1001      127      764 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/lib.rs
+-rw-r--r--   0     1001      127     2553 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/node/arrow_utils.rs
+-rw-r--r--   0     1001      127     3654 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/node/control_channel.rs
+-rw-r--r--   0     1001      127     5795 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/node/drop_stream.rs
+-rw-r--r--   0     1001      127    14339 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/node/mod.rs
+-rw-r--r--   0     1001      127      583 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/Cargo.toml
+-rw-r--r--   0     1001      127     1620 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/src/lib.rs
+-rw-r--r--   0     1001      127     2388 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/src/telemetry.rs
+-rw-r--r--   0     1001      127      424 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/Cargo.toml
+-rw-r--r--   0     1001      127    13680 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/lib.rs
+-rw-r--r--   0     1001      127     4140 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/qos.rs
+-rw-r--r--   0     1001      127      729 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs
+-rw-r--r--   0     1001      127     6330 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs
+-rw-r--r--   0     1001      127     4726 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs
+-rw-r--r--   0     1001      127     6326 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs
+-rw-r--r--   0     1001      127     1154 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs
+-rw-r--r--   0     1001      127     4263 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/mod.rs
+-rw-r--r--   0     1001      127     9390 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs
+-rw-r--r--   0     1001      127     9481 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs
+-rw-r--r--   0     1001      127     7776 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs
+-rw-r--r--   0     1001      127     3086 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs
+-rw-r--r--   0     1001      127     9552 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs
+-rw-r--r--   0     1001      127    11898 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/test_utils.py
+-rw-r--r--   0     1001      127     1431 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/Cargo.toml
+-rw-r--r--   0     1001      127    13120 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/lib.rs
+-rw-r--r--   0     1001      127     4296 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/operator/channel.rs
+-rw-r--r--   0     1001      127     2639 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/operator/mod.rs
+-rw-r--r--   0     1001      127    15299 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/operator/python.rs
+-rw-r--r--   0     1001      127    10280 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/operator/shared_lib.rs
+-rw-r--r--   0     1001      127      461 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/operator/types/Cargo.toml
+-rw-r--r--   0     1001      127     4949 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/operator/types/src/lib.rs
+-rw-r--r--   0     1001      127      323 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/arrow-convert/Cargo.toml
+-rw-r--r--   0     1001      127     5495 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/arrow-convert/src/from_impls.rs
+-rw-r--r--   0     1001      127     3744 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/arrow-convert/src/into_impls.rs
+-rw-r--r--   0     1001      127      485 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/arrow-convert/src/lib.rs
+-rw-r--r--   0     1001      127      451 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/message/Cargo.toml
+-rw-r--r--   0     1001      127     4262 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/message/src/lib.rs
+-rw-r--r--   0     1001      127      593 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/shared-memory-server/Cargo.toml
+-rw-r--r--   0     1001      127     3249 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/shared-memory-server/src/bin/bench.rs
+-rw-r--r--   0     1001      127     7343 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/shared-memory-server/src/channel.rs
+-rw-r--r--   0     1001      127     2058 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/shared-memory-server/src/lib.rs
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 dora_rs-0.3.4rc2/apis/python/node/Cargo.toml
+-rw-r--r--   0     1001      127      339 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/README.md
+-rw-r--r--   0     1001      127      723 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/dora/__init__.py
+-rw-r--r--   0     1001      127     8425 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/dora/__init__.pyi
+-rw-r--r--   0     1001      127    17717 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/generate_stubs.py
+-rw-r--r--   0     1001      127     7897 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/src/lib.rs
+-rw-r--r--   0     1001      127   262901 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/Cargo.lock
+-rw-r--r--   0        0        0     3955 1970-01-01 00:00:00.000000 dora_rs-0.3.4rc2/Cargo.toml
+-rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 dora_rs-0.3.4rc2/pyproject.toml
+-rw-r--r--   0     1001      127      723 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/dora/__init__.py
+-rw-r--r--   0     1001      127     8425 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/dora/__init__.pyi
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 dora_rs-0.3.4rc2/PKG-INFO
```

### Comparing `dora_rs-0.3.3rc1/libraries/arrow-convert/src/from_impls.rs` & `dora_rs-0.3.4rc2/libraries/arrow-convert/src/from_impls.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/arrow-convert/src/into_impls.rs` & `dora_rs-0.3.4rc2/libraries/arrow-convert/src/into_impls.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/download/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/extensions/download/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/operator/types/src/lib.rs` & `dora_rs-0.3.4rc2/apis/rust/operator/types/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #![deny(elided_lifetimes_in_paths)] // required for safer-ffi
 #![allow(improper_ctypes_definitions)]
+#![allow(clippy::missing_safety_doc)]
 
 pub use arrow;
 use dora_arrow_convert::{ArrowData, IntoArrow};
 pub use safer_ffi;
 
 use arrow::{
     array::Array,
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/build.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/build.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,18 @@
                 impl Ros2Context {
                     fn new_node(&self, name_space: &str, base_name: &str) -> eyre::Result<Box<Ros2Node>> {
                         use futures::task::SpawnExt as _;
                         use eyre::WrapErr as _;
 
                         let name = ros2_client::NodeName::new(name_space, base_name).map_err(|e| eyre::eyre!(e))?;
                         let options = ros2_client::NodeOptions::new().enable_rosout(true);
-                        let mut node = self.context.new_node(name, options)?;
+                        let mut node = self.context.new_node(name, options)
+                            .map_err(|e| eyre::eyre!("failed to create ROS2 node: {e:?}"))?;
 
-                        let spinner = node.spinner();
+                        let spinner = node.spinner().context("failed to create spinner")?;
                         self.executor.spawn(async {
                             if let Err(err) = spinner.spin().await {
                                 eprintln!("ros2 spinner failed: {err:?}");
                             }
                         })
                         .context("failed to spawn ros2 spinner")?;
 
@@ -243,28 +244,34 @@
     quote! {
         #attributes
         mod ffi {
             #imports_and_functions
 
             #[derive(Debug, Default, Clone, PartialEq, Eq, Serialize, Deserialize)]
             pub struct U16String {
-                chars: Vec<u16>,
+                pub chars: Vec<u16>,
             }
 
             #(#shared_type_defs)*
             #(#service_defs)*
         }
 
 
         impl crate::_core::InternalDefault for ffi::U16String {
             fn _default() -> Self {
                 Default::default()
             }
         }
 
+        impl ffi::U16String {
+            fn from_str(arg: &str) -> Self {
+                Self { chars: crate::_core::widestring::U16String::from_str(arg).into_vec()}
+            }
+        }
+
         #(#message_struct_impls)*
 
         #cxx_bridge_impls
         #(#message_topic_impls)*
         #(#service_creation_impls)*
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 fn bool_literal(s: &str) -> IResult<&str, bool> {
     alt((
         value(true, alt((tag("true"), tag("1")))),
         value(false, alt((tag("false"), tag("0")))),
     ))(s)
 }
 
+#[allow(clippy::type_complexity)]
 pub fn get_string_literal_parser(
     string_type: GenericString,
 ) -> Box<dyn FnMut(&str) -> IResult<&str, String>> {
     match string_type {
         GenericString::String | GenericString::WString => Box::new(string_literal),
         GenericString::BoundedString(max_size) | GenericString::BoundedWString(max_size) => {
             Box::new(move |s| verify(string_literal, |s: &str| s.len() <= max_size)(s))
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,19 @@
 pub fn parse_constant_type(s: &str) -> IResult<&str, ConstantType> {
     map(
         tuple((
             primitive_type,
             opt(delimited(char('['), usize_literal, char(']'))),
             peek(alt((space1, eof))),
         )),
-        |(value_type, size, _)| match size {
-            None => value_type.into(),
-            Some(size) => PrimitiveArray { value_type, size }.into(),
+        |(value_type, size, _)| {
+            size.map_or_else(
+                || value_type.into(),
+                |size| PrimitiveArray { value_type, size }.into(),
+            )
         },
     )(s)
 }
 
 fn basic_type(s: &str) -> IResult<&str, BasicType> {
     map(
         alt((
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs`

 * *Files 16% similar despite different names*

```diff
@@ -21,33 +21,33 @@
     PrimitiveType(PrimitiveType),
     PrimitiveArray(PrimitiveArray),
 }
 
 impl ConstantType {
     pub fn type_tokens(&self) -> impl ToTokens {
         match self {
-            ConstantType::PrimitiveType(t) => {
+            Self::PrimitiveType(t) => {
                 let token = t.type_tokens();
                 quote! { #token }
             }
-            ConstantType::PrimitiveArray(t) => {
+            Self::PrimitiveArray(t) => {
                 let token = t.type_tokens();
                 quote! { #token }
             }
         }
     }
 
     pub fn value_tokens(&self, values: &[String]) -> impl ToTokens {
         match self {
-            ConstantType::PrimitiveType(t) => {
+            Self::PrimitiveType(t) => {
                 assert_eq!(values.len(), 1);
                 let token = t.value_tokens(&values[0]);
                 quote! { #token }
             }
-            ConstantType::PrimitiveArray(t) => {
+            Self::PrimitiveArray(t) => {
                 assert_eq!(values.len(), t.size);
                 let tokens = values.iter().map(|v| t.value_type.value_tokens(v));
                 quote! { [#(#tokens,)*] }
             }
         }
     }
 }
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             pub mod #package_name {
                 #aliases
                 #service_aliases
             }
         }
     }
 
-    pub fn token_stream(&self, gen_cxx_bridge: bool) -> impl ToTokens {
+    pub fn token_stream(&self, _gen_cxx_bridge: bool) -> impl ToTokens {
         let name = Ident::new(&self.name, Span::call_site());
         let services_block = self.services_block();
         let actions_block = self.actions_block();
 
         quote! {
             pub mod #name {
                 #services_block
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         }
     }
 
     fn value_tokens(self, value: &str) -> impl ToTokens {
         // TODO: Assertion
         let value = Literal::string(value);
         if self.is_wide() {
-            quote! { ::widestring::U16String::from_str(#value) }
+            quote! { ffi::U16String::from_str(#value) }
         } else {
             quote! { ::std::string::String::from(#value) }
         }
     }
 }
 
 impl From<GenericUnboundedString> for GenericString {
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/shared-memory-server/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/shared-memory-server/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/shared-memory-server/src/bin/bench.rs` & `dora_rs-0.3.4rc2/libraries/shared-memory-server/src/bin/bench.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/shared-memory-server/src/channel.rs` & `dora_rs-0.3.4rc2/libraries/shared-memory-server/src/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/shared-memory-server/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/shared-memory-server/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#![allow(clippy::missing_safety_doc)]
+
 use self::channel::ShmemChannel;
 use eyre::{eyre, Context};
 use serde::{Deserialize, Serialize};
 pub use shared_memory_extended::{Shmem, ShmemConf};
 use std::marker::PhantomData;
 use std::time::Duration;
```

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/Cargo.toml` & `dora_rs-0.3.4rc2/apis/rust/node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/mod.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/daemon_connection/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/tcp.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/daemon_connection/tcp.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/event.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/event.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/merged.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/merged.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/mod.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/thread.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/thread.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/lib.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/node/arrow_utils.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/node/arrow_utils.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/node/control_channel.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/node/control_channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/node/drop_stream.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/node/drop_stream.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/rust/node/src/node/mod.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/node/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 .wrap_err("failed to init drop stream")?;
         let control_channel =
             ControlChannel::init(dataflow_id, &node_id, &daemon_communication, clock.clone())
                 .wrap_err("failed to init control channel")?;
 
         let node = Self {
             id: node_id,
-            dataflow_id: dataflow_id,
+            dataflow_id,
             node_config: run_config,
             control_channel,
             clock,
             sent_out_shared_memory: HashMap::new(),
             drop_stream,
             cache: VecDeque::new(),
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/metrics/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/metrics/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
         .with_period(Duration::from_secs(10))
         .build()
 }
 
 pub fn init_meter_provider(meter_id: String) -> Result<SdkMeterProvider> {
     let meter_provider = init_metrics().context("Could not create opentelemetry meter")?;
     let meter = meter_provider.meter(meter_id);
-    let _ = init_process_observer(meter).context("could not initiale system metrics observer")?;
+    init_process_observer(meter).context("could not initiale system metrics observer")?;
     Ok(meter_provider)
 }
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/qos.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/qos.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 use ::dora_ros2_bridge::rustdds::{self, policy};
 use pyo3::prelude::{pyclass, pymethods};
 
+/// ROS2 QoS Policy
+///
+/// :type durability: dora.Ros2Durability, optional
+/// :type liveliness: dora.Ros2Liveliness, optional
+/// :type reliable: bool, optional
+/// :type keep_all: bool, optional
+/// :type lease_duration: float, optional
+/// :type max_blocking_time: float, optional
+/// :type keep_last: int, optional
+/// :rtype: dora.Ros2QoSPolicies
+///
 #[derive(Debug, Clone)]
-#[pyclass(get_all, set_all)]
+#[pyclass]
 #[non_exhaustive]
 pub struct Ros2QosPolicies {
     pub durability: Ros2Durability,
     pub liveliness: Ros2Liveliness,
     pub lease_duration: f64,
     pub reliable: bool,
     pub max_blocking_time: f64,
@@ -60,44 +71,53 @@
                 }
             })
             .build()
     }
 }
 
 /// DDS 2.2.3.4 DURABILITY
+///
+/// :rtype: dora.Ros2Durability
 #[derive(Copy, Clone, Debug, PartialEq, Eq, PartialOrd, Ord, Hash)]
 #[pyclass]
 pub enum Ros2Durability {
     Volatile,
     TransientLocal,
     Transient,
     Persistent,
 }
 
+/// :type value: dora.Ros2Durability
+/// :rtype: dora.Ros2Durability
 impl From<Ros2Durability> for policy::Durability {
+    /// :type value: dora.Ros2Durability
+    /// :rtype: dora.Ros2Durability
     fn from(value: Ros2Durability) -> Self {
         match value {
             Ros2Durability::Volatile => policy::Durability::Volatile,
             Ros2Durability::TransientLocal => policy::Durability::TransientLocal,
             Ros2Durability::Transient => policy::Durability::Transient,
             Ros2Durability::Persistent => policy::Durability::Persistent,
         }
     }
 }
 
 /// DDS 2.2.3.11 LIVELINESS
+/// :rtype: dora.Ros2Liveliness
 #[derive(Copy, Clone, Debug, PartialEq)]
 #[pyclass]
 pub enum Ros2Liveliness {
     Automatic,
     ManualByParticipant,
     ManualByTopic,
 }
 
 impl Ros2Liveliness {
+    /// :type lease_duration: float
+    /// :rtype: dora.Ros2Liveliness
     fn convert(self, lease_duration: f64) -> policy::Liveliness {
         let lease_duration = if lease_duration.is_infinite() {
             rustdds::Duration::INFINITE
         } else {
             rustdds::Duration::from_frac_seconds(lease_duration)
         };
         match self {
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/mod.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/test_utils.py` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/message/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/message/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 //! Enable serialisation and deserialisation of capnproto messages
 //!
 
+#![allow(clippy::missing_safety_doc)]
+
 use arrow_data::ArrayData;
 use arrow_schema::DataType;
 use eyre::Context;
 use serde::{Deserialize, Serialize};
 pub use uhlc;
 
 #[derive(Debug, Clone, PartialEq, Eq, Serialize, Deserialize)]
```

### Comparing `dora_rs-0.3.3rc1/apis/python/operator/Cargo.toml` & `dora_rs-0.3.4rc2/apis/python/operator/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/python/operator/src/lib.rs` & `dora_rs-0.3.4rc2/apis/python/operator/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 use arrow::{array::ArrayRef, pyarrow::ToPyArrow};
 use dora_node_api::{merged::MergedEvent, Event, Metadata, MetadataParameters};
 use eyre::{Context, Result};
 use pyo3::{exceptions::PyLookupError, prelude::*, types::PyDict};
 
+/// Dora Event
 #[pyclass]
 pub struct PyEvent {
     event: MergedEvent<PyObject>,
     data: Option<ArrayRef>,
 }
 
+// Dora Event
 #[pymethods]
 impl PyEvent {
+    ///
+    /// :rtype: dora.PyObject
     pub fn __getitem__(&self, key: &str, py: Python<'_>) -> PyResult<Option<PyObject>> {
         if key == "kind" {
             let kind = match &self.event {
                 MergedEvent::Dora(_) => "dora",
                 MergedEvent::External(_) => "external",
             };
             return Ok(Some(kind.to_object(py)));
@@ -31,15 +35,22 @@
                         return Err(PyLookupError::new_err(format!(
                             "event has no property `{other}`"
                         )))
                     }
                 };
                 Ok(value)
             }
-            MergedEvent::External(event) => event.call_method1(py, "__getitem__", (key,)).map(Some),
+            MergedEvent::External(event) => {
+                let value = match key {
+                    "value" => event,
+                    _ => todo!(),
+                };
+
+                Ok(Some(value.clone()))
+            }
         }
     }
 
     pub fn inner(&mut self) -> Option<&PyObject> {
         match &self.event {
             MergedEvent::Dora(_) => None,
             MergedEvent::External(event) => Some(event),
```

### Comparing `dora_rs-0.3.3rc1/libraries/core/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/core/src/config.rs` & `dora_rs-0.3.4rc2/libraries/core/src/config.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/core/src/coordinator_messages.rs` & `dora_rs-0.3.4rc2/libraries/core/src/coordinator_messages.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 use crate::daemon_messages::DataflowId;
 use eyre::eyre;
-use std::net::SocketAddr;
 
 #[derive(Debug, serde::Serialize, serde::Deserialize)]
 pub enum CoordinatorRequest {
     Register {
         dora_version: String,
         machine_id: String,
-        listen_socket: SocketAddr,
+        listen_port: u16,
     },
     Event {
         machine_id: String,
         event: DaemonEvent,
     },
 }
```

### Comparing `dora_rs-0.3.3rc1/libraries/core/src/daemon_messages.rs` & `dora_rs-0.3.4rc2/libraries/core/src/daemon_messages.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use std::{
     collections::{BTreeMap, BTreeSet},
     fmt,
     net::SocketAddr,
     path::PathBuf,
+    time::Duration,
 };
 
 use crate::{
     config::{DataId, NodeId, NodeRunConfig, OperatorId},
     descriptor::{Descriptor, OperatorDefinition, ResolvedNode},
 };
 use aligned_vec::{AVec, ConstAlign};
@@ -209,14 +210,15 @@
     Spawn(SpawnDataflowNodes),
     AllNodesReady {
         dataflow_id: DataflowId,
         success: bool,
     },
     StopDataflow {
         dataflow_id: DataflowId,
+        grace_duration: Option<Duration>,
     },
     ReloadDataflow {
         dataflow_id: DataflowId,
         node_id: NodeId,
         operator_id: Option<OperatorId>,
     },
     Logs {
```

### Comparing `dora_rs-0.3.3rc1/libraries/core/src/descriptor/mod.rs` & `dora_rs-0.3.4rc2/libraries/core/src/descriptor/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 use tracing::warn;
 pub use visualize::collect_dora_timers;
 
 mod validate;
 mod visualize;
 pub const SHELL_SOURCE: &str = "shell";
 
+/// Dataflow description
 #[derive(Debug, Clone, Serialize, Deserialize)]
 #[serde(deny_unknown_fields)]
 pub struct Descriptor {
     #[serde(default)]
     pub communication: CommunicationConfig,
     // deprecated
     pub daemon_config: Option<serde_yaml::Value>,
@@ -256,17 +257,61 @@
     pub send_stdout_as: Option<String>,
 }
 
 #[derive(Debug, Serialize, Deserialize, Clone)]
 #[serde(rename_all = "kebab-case")]
 pub enum OperatorSource {
     SharedLibrary(String),
-    Python(String),
+    Python(PythonSource),
     Wasm(String),
 }
+#[derive(Debug, Clone, PartialEq, Eq, Serialize, Deserialize)]
+#[serde(
+    deny_unknown_fields,
+    from = "PythonSourceDef",
+    into = "PythonSourceDef"
+)]
+pub struct PythonSource {
+    pub source: String,
+    pub conda_env: Option<String>,
+}
+
+#[derive(Debug, Clone, PartialEq, Eq, Serialize, Deserialize)]
+#[serde(untagged)]
+pub enum PythonSourceDef {
+    SourceOnly(String),
+    WithOptions {
+        source: String,
+        conda_env: Option<String>,
+    },
+}
+
+impl From<PythonSource> for PythonSourceDef {
+    fn from(input: PythonSource) -> Self {
+        match input {
+            PythonSource {
+                source,
+                conda_env: None,
+            } => Self::SourceOnly(source),
+            PythonSource { source, conda_env } => Self::WithOptions { source, conda_env },
+        }
+    }
+}
+
+impl From<PythonSourceDef> for PythonSource {
+    fn from(value: PythonSourceDef) -> Self {
+        match value {
+            PythonSourceDef::SourceOnly(source) => Self {
+                source,
+                conda_env: None,
+            },
+            PythonSourceDef::WithOptions { source, conda_env } => Self { source, conda_env },
+        }
+    }
+}
 
 pub fn source_is_url(source: &str) -> bool {
     source.contains("://")
 }
 
 pub fn resolve_path(source: &str, working_dir: &Path) -> Result<PathBuf> {
     let path = Path::new(&source);
```

### Comparing `dora_rs-0.3.3rc1/libraries/core/src/descriptor/validate.rs` & `dora_rs-0.3.4rc2/libraries/core/src/descriptor/validate.rs`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,17 @@
                             } else {
                                 let path = adjust_shared_library_path(Path::new(&path))?;
                                 if !working_dir.join(&path).exists() {
                                     bail!("no shared library at `{}`", path.display());
                                 }
                             }
                         }
-                        OperatorSource::Python(path) => {
+                        OperatorSource::Python(python_source) => {
                             has_python_operator = true;
+                            let path = &python_source.source;
                             if source_is_url(path) {
                                 info!("{path} is a URL."); // TODO: Implement url check.
                             } else if !working_dir.join(path).exists() {
                                 bail!("no Python library at `{path}`");
                             }
                         }
                         OperatorSource::Wasm(path) => {
```

### Comparing `dora_rs-0.3.3rc1/libraries/core/src/descriptor/visualize.rs` & `dora_rs-0.3.4rc2/libraries/core/src/descriptor/visualize.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/core/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/core/src/topics.rs` & `dora_rs-0.3.4rc2/libraries/core/src/topics.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use std::{
     collections::BTreeSet,
     fmt::Display,
     net::{Ipv4Addr, SocketAddr},
     path::PathBuf,
+    time::Duration,
 };
 use uuid::Uuid;
 
 use crate::{
     config::{NodeId, OperatorId},
     descriptor::Descriptor,
 };
@@ -34,17 +35,19 @@
         operator_id: Option<OperatorId>,
     },
     Check {
         dataflow_uuid: Uuid,
     },
     Stop {
         dataflow_uuid: Uuid,
+        grace_duration: Option<Duration>,
     },
     StopByName {
         name: String,
+        grace_duration: Option<Duration>,
     },
     Logs {
         uuid: Option<Uuid>,
         name: Option<String>,
         node: String,
     },
     Destroy,
```

### Comparing `dora_rs-0.3.3rc1/binaries/runtime/Cargo.toml` & `dora_rs-0.3.4rc2/binaries/runtime/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/binaries/runtime/src/lib.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/binaries/runtime/src/operator/channel.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/operator/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/binaries/runtime/src/operator/mod.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/binaries/runtime/src/operator/python.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/operator/python.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #![allow(clippy::borrow_deref_ref)] // clippy warns about code generated by #[pymethods]
 
 use super::{OperatorEvent, StopReason};
 use dora_core::{
     config::{NodeId, OperatorId},
-    descriptor::{source_is_url, Descriptor},
+    descriptor::{source_is_url, Descriptor, PythonSource},
 };
 use dora_download::download_file;
 use dora_node_api::Event;
 use dora_operator_api_python::PyEvent;
 use dora_operator_api_types::DoraStatus;
 use eyre::{bail, eyre, Context, Result};
 use pyo3::{
@@ -31,33 +31,33 @@
     }
 }
 
 #[tracing::instrument(skip(events_tx, incoming_events), level = "trace")]
 pub fn run(
     node_id: &NodeId,
     operator_id: &OperatorId,
-    source: &str,
+    python_source: &PythonSource,
     events_tx: Sender<OperatorEvent>,
     incoming_events: flume::Receiver<Event>,
     init_done: oneshot::Sender<Result<()>>,
     dataflow_descriptor: &Descriptor,
 ) -> eyre::Result<()> {
-    let path = if source_is_url(source) {
+    let path = if source_is_url(&python_source.source) {
         let target_path = Path::new("build")
             .join(node_id.to_string())
             .join(format!("{}.py", operator_id));
         // try to download the shared library
         let rt = tokio::runtime::Builder::new_current_thread()
             .enable_all()
             .build()?;
-        rt.block_on(download_file(source, &target_path))
+        rt.block_on(download_file(&python_source.source, &target_path))
             .wrap_err("failed to download Python operator")?;
         target_path
     } else {
-        Path::new(source).to_owned()
+        Path::new(&python_source.source).to_owned()
     };
 
     if !path.exists() {
         bail!("No python file exists at {}", path.display());
     }
     let path = path
         .canonicalize()
@@ -126,14 +126,15 @@
             let Ok(mut event) = incoming_events.recv() else {
                 break StopReason::InputsClosed;
             };
 
             if let Event::Reload { .. } = event {
                 reload = true;
                 // Reloading method
+                #[allow(clippy::blocks_in_conditions)]
                 match Python::with_gil(|py| -> Result<Py<PyAny>> {
                     // Saving current state
                     let current_state = operator
                         .getattr(py, "__dict__")
                         .wrap_err("Could not retrieve current operator state")?;
                     let current_state = current_state
                         .extract::<&PyDict>(py)
```

### Comparing `dora_rs-0.3.3rc1/binaries/runtime/src/operator/shared_lib.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/operator/shared_lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/telemetry.rs` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 ros2-examples = ["dep:eyre", "tokio", "dora-daemon"]
 
 [dependencies]
 array-init = "2.1.0"
 serde = { version = "1.0.164", features = ["derive"] }
 serde-big-array = "0.5.1"
 widestring = "1.0.2"
-ros2-client = { git = "https://github.com/dora-rs/ros2-client.git", branch = "deserialize-seed-2" }
-rustdds = { git = "https://github.com/dora-rs/RustDDS.git", branch = "deserialize-seed-2" }
+ros2-client = "0.7.1"
+rustdds = "0.10.0"
 eyre = { version = "0.6.8", optional = true }
 tokio = { version = "1.29.1", features = ["full"], optional = true }
 dora-daemon = { path = "../../../binaries/daemon", optional = true }
 tracing = "0.1.37"
 tracing-subscriber = "0.3.17"
 flume = "0.11.0"
 futures = { version = "0.3.21", features = ["thread-pool"] }
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/build.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/build.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#[cfg(feature = "generate-messages")]
 use std::path::PathBuf;
 
 #[cfg(not(feature = "generate-messages"))]
 fn main() {}
 
 #[cfg(feature = "generate-messages")]
 fn main() {
@@ -11,19 +12,17 @@
     let generated_string = rust_format::PrettyPlease::default()
         .format_tokens(generated)
         .unwrap();
     let out_dir = PathBuf::from(std::env::var("OUT_DIR").unwrap());
     let target_file = out_dir.join("messages.rs");
     std::fs::write(&target_file, generated_string).unwrap();
     println!("cargo:rustc-env=MESSAGES_PATH={}", target_file.display());
-
-    #[cfg(feature = "cxx-bridge")]
-    let _build = cxx_build::bridge(&target_file);
 }
 
+#[cfg(feature = "generate-messages")]
 fn ament_prefix_paths() -> Vec<PathBuf> {
     let ament_prefix_path: String = match std::env::var("AMENT_PREFIX_PATH") {
         Ok(path) => path,
         Err(std::env::VarError::NotPresent) => {
             println!("cargo:warning='AMENT_PREFIX_PATH not set'");
             String::new()
         }
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/sequence.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/string.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/string.rs`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 pub struct U16String(widestring::U16String);
 
 impl U16String {
     pub fn new() -> Self {
         Self(widestring::U16String::new())
     }
 
+    #[allow(clippy::should_implement_trait)]
     pub fn from_str(arg: &str) -> U16String {
         Self(widestring::U16String::from_str(arg))
     }
 }
 
 impl Deref for U16String {
     type Target = widestring::U16String;
```

### Comparing `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/traits.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/traits.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/python/node/Cargo.toml` & `dora_rs-0.3.4rc2/apis/python/node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3rc1/apis/python/node/src/lib.rs` & `dora_rs-0.3.4rc2/apis/python/node/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             events: Events::Dora(events),
             node,
         })
     }
 
     /// `.next()` gives you the next input that the node has received.
     /// It blocks until the next event becomes available.
+    /// You can use timeout in seconds to return if no input is available.
     /// It will return `None` when all senders has been dropped.
     ///
     /// ```python
     /// event = node.next()
     /// ```
     ///
     /// You can also iterate over the event stream with a loop
@@ -54,42 +55,73 @@
     /// ```python
     /// for event in node:
     ///    match event["type"]:
     ///        case "INPUT":
     ///            match event["id"]:
     ///                 case "image":
     /// ```
+    ///
+    /// :type timeout: float, optional
+    /// :rtype: dora.PyEvent
     #[allow(clippy::should_implement_trait)]
     pub fn next(&mut self, py: Python, timeout: Option<f32>) -> PyResult<Option<PyEvent>> {
         let event = py.allow_threads(|| self.events.recv(timeout.map(Duration::from_secs_f32)));
         Ok(event)
     }
 
+    /// You can iterate over the event stream with a loop
+    ///
+    /// ```python
+    /// for event in node:
+    ///    match event["type"]:
+    ///        case "INPUT":
+    ///            match event["id"]:
+    ///                 case "image":
+    /// ```
+    ///
+    /// :rtype: dora.PyEvent
     pub fn __next__(&mut self, py: Python) -> PyResult<Option<PyEvent>> {
         let event = py.allow_threads(|| self.events.recv(None));
         Ok(event)
     }
 
+    /// You can iterate over the event stream with a loop
+    ///
+    /// ```python
+    /// for event in node:
+    ///    match event["type"]:
+    ///        case "INPUT":
+    ///            match event["id"]:
+    ///                 case "image":
+    /// ```
+    ///
+    /// :rtype: dora.PyEvent
     fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
         slf
     }
 
     /// `send_output` send data from the node.
     ///
     /// ```python
     /// Args:
     ///    output_id: str,
-    ///    data: Bytes|Arrow,
+    ///    data: pyarrow.Array,
     ///    metadata: Option[Dict],
     /// ```
     ///
+    /// ex:
+    ///
     /// ```python
     /// node.send_output("string", b"string", {"open_telemetry_context": "7632e76"})
     /// ```
     ///
+    /// :type output_id: str
+    /// :type data: pyarrow.Array
+    /// :type metadata: dict, optional
+    /// :rtype: None
     pub fn send_output(
         &mut self,
         output_id: String,
         data: PyObject,
         metadata: Option<&PyDict>,
         py: Python,
     ) -> eyre::Result<()> {
@@ -112,18 +144,25 @@
 
         Ok(())
     }
 
     /// Returns the full dataflow descriptor that this node is part of.
     ///
     /// This method returns the parsed dataflow YAML file.
+    ///
+    /// :rtype: dict
     pub fn dataflow_descriptor(&self, py: Python) -> pythonize::Result<PyObject> {
         pythonize::pythonize(py, self.node.dataflow_descriptor())
     }
 
+    /// Merge an external event stream with dora main loop.
+    /// This currently only work with ROS2.
+    ///
+    /// :type subscription: dora.Ros2Subscription
+    /// :rtype: None
     pub fn merge_external_events(
         &mut self,
         subscription: &mut Ros2Subscription,
     ) -> eyre::Result<()> {
         let subscription = subscription.into_stream()?;
         let stream = futures::stream::poll_fn(move |cx| {
             let s = subscription.as_stream().map(|item| {
@@ -193,25 +232,25 @@
 impl Node {
     pub fn id(&self) -> String {
         self.node.id().to_string()
     }
 }
 
 /// Start a runtime for Operators
+///
+/// :rtype: None
 #[pyfunction]
 pub fn start_runtime() -> eyre::Result<()> {
     dora_runtime::main().wrap_err("Dora Runtime raised an error.")
 }
 
 #[pymodule]
-fn dora(py: Python, m: &PyModule) -> PyResult<()> {
+fn dora(_py: Python, m: &PyModule) -> PyResult<()> {
+    dora_ros2_bridge_python::create_dora_ros2_bridge_module(m)?;
     m.add_function(wrap_pyfunction!(start_runtime, m)?)?;
-    m.add_class::<Node>().unwrap();
-
-    let ros2_bridge = PyModule::new(py, "ros2_bridge")?;
-    dora_ros2_bridge_python::create_dora_ros2_bridge_module(ros2_bridge)?;
-    let experimental = PyModule::new(py, "experimental")?;
-    experimental.add_submodule(ros2_bridge)?;
-    m.add_submodule(experimental)?;
+    m.add_class::<Node>()?;
+    m.add_class::<PyEvent>()?;
+    m.setattr("__version__", env!("CARGO_PKG_VERSION"))?;
+    m.setattr("__author__", "Dora-rs Authors")?;
 
     Ok(())
 }
```

### Comparing `dora_rs-0.3.3rc1/Cargo.lock` & `dora_rs-0.3.4rc2/Cargo.lock`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,103 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "ab_glyph"
+version = "0.2.25"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f90148830dac590fac7ccfe78ec4a8ea404c60f75a24e16407a71f0f40de775"
+dependencies = [
+ "ab_glyph_rasterizer",
+ "owned_ttf_parser",
+]
+
+[[package]]
+name = "ab_glyph_rasterizer"
+version = "0.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c71b1793ee61086797f5c80b6efa2b8ffa6d5dd703f118545808a7f2e27f7046"
+
+[[package]]
+name = "accesskit"
+version = "0.12.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "74a4b14f3d99c1255dcba8f45621ab1a2e7540a0009652d33989005a4d0bfc6b"
+dependencies = [
+ "enumn",
+ "serde",
+]
+
+[[package]]
+name = "accesskit_consumer"
+version = "0.16.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8c17cca53c09fbd7288667b22a201274b9becaa27f0b91bf52a526db95de45e6"
+dependencies = [
+ "accesskit",
+]
+
+[[package]]
+name = "accesskit_macos"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cd3b6ae1eabbfbced10e840fd3fce8a93ae84f174b3e4ba892ab7bcb42e477a7"
+dependencies = [
+ "accesskit",
+ "accesskit_consumer",
+ "objc2 0.3.0-beta.3.patch-leaks.3",
+ "once_cell",
+]
+
+[[package]]
+name = "accesskit_unix"
+version = "0.6.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09f46c18d99ba61ad7123dd13eeb0c104436ab6af1df6a1cd8c11054ed394a08"
+dependencies = [
+ "accesskit",
+ "accesskit_consumer",
+ "async-channel 2.1.1",
+ "async-once-cell",
+ "atspi",
+ "futures-lite 1.13.0",
+ "once_cell",
+ "serde",
+ "zbus",
+]
+
+[[package]]
+name = "accesskit_windows"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "afcae27ec0974fc7c3b0b318783be89fd1b2e66dd702179fe600166a38ff4a0b"
+dependencies = [
+ "accesskit",
+ "accesskit_consumer",
+ "once_cell",
+ "paste",
+ "static_assertions",
+ "windows 0.48.0",
+]
+
+[[package]]
+name = "accesskit_winit"
+version = "0.16.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5284218aca17d9e150164428a0ebc7b955f70e3a9a78b4c20894513aabf98a67"
+dependencies = [
+ "accesskit",
+ "accesskit_macos",
+ "accesskit_unix",
+ "accesskit_windows",
+ "winit",
+]
+
+[[package]]
 name = "addr2line"
 version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
 dependencies = [
  "gimli",
 ]
@@ -34,14 +125,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77c3a9648d43b9cd48db467b3f87fdd6e146bcc88ab0180006cef2179fe11d01"
 dependencies = [
  "cfg-if 1.0.0",
  "const-random",
  "getrandom",
  "once_cell",
+ "serde",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
 version = "1.1.1"
@@ -72,14 +164,47 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
+name = "allocator-api2"
+version = "0.2.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
+
+[[package]]
+name = "android-activity"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee91c0c2905bae44f84bfa4e044536541df26b7703fd0888deeb9060fcc44289"
+dependencies = [
+ "android-properties",
+ "bitflags 2.4.0",
+ "cc",
+ "cesu8",
+ "jni",
+ "jni-sys",
+ "libc",
+ "log",
+ "ndk",
+ "ndk-context",
+ "ndk-sys",
+ "num_enum",
+ "thiserror",
+]
+
+[[package]]
+name = "android-properties"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fc7eb209b1518d6bb87b283c20095f5228ecda460da70b44f0802523dea6da04"
+
+[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
@@ -150,20 +275,51 @@
 [[package]]
 name = "anyhow"
 version = "1.0.75"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4668cab20f66d8d020e1fbc0ebe47217433c1b6c8f2040faf858554e394ace6"
 
 [[package]]
+name = "arboard"
+version = "3.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a2041f1943049c7978768d84e6d0fd95de98b76d6c4727b09e78ec253d29fa58"
+dependencies = [
+ "clipboard-win",
+ "core-graphics",
+ "image",
+ "log",
+ "objc",
+ "objc-foundation",
+ "objc_id",
+ "parking_lot",
+ "thiserror",
+ "windows-sys 0.48.0",
+ "x11rb",
+]
+
+[[package]]
 name = "array-init"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d62b7694a562cdf5a74227903507c56ab2cc8bdd1f781ed5cb4cf9c9f810bfc"
 
 [[package]]
+name = "array-init-cursor"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
+
+[[package]]
+name = "arrayvec"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
+
+[[package]]
 name = "arrow"
 version = "48.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "edb738d83750ec705808f6d44046d165e6bb8623f64e29a4d53fcb136ab22dfb"
 dependencies = [
  "ahash",
  "arrow-arith",
@@ -269,14 +425,24 @@
  "arrow-buffer",
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
+name = "arrow-format"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07884ea216994cdc32a2d5f8274a8bee979cfe90274b83f86f440866ee3132c7"
+dependencies = [
+ "planus",
+ "serde",
+]
+
+[[package]]
 name = "arrow-ipc"
 version = "48.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e36bf091502ab7e37775ff448413ef1ffff28ff93789acb669fffdd51b394d51"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
@@ -295,15 +461,15 @@
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
- "indexmap 2.0.2",
+ "indexmap 2.2.6",
  "lexical-core",
  "num",
  "serde",
  "serde_json",
 ]
 
 [[package]]
@@ -373,24 +539,68 @@
  "arrow-select",
  "num",
  "regex",
  "regex-syntax 0.8.2",
 ]
 
 [[package]]
+name = "as-raw-xcb-connection"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "175571dd1d178ced59193a6fc02dde1b972eb0bc56c892cde9beeceac5bf0f6b"
+
+[[package]]
+name = "ash"
+version = "0.37.3+1.3.251"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "39e9c3835d686b0a6084ab4234fcd1b07dbf6e4767dce60874b12356a25ecd4a"
+dependencies = [
+ "libloading 0.7.4",
+]
+
+[[package]]
+name = "ashpd"
+version = "0.6.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4ac22eda5891cc086690cb6fa10121c0390de0e3b04eb269f2d766b00d3f2d81"
+dependencies = [
+ "async-fs 2.1.1",
+ "async-net",
+ "enumflags2",
+ "futures-channel",
+ "futures-util",
+ "once_cell",
+ "rand",
+ "serde",
+ "serde_repr",
+ "url",
+ "zbus",
+]
+
+[[package]]
 name = "async-attributes"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3203e79f4dd9bdda415ed03cf14dae5a2bf775c683a00f94e9cd1faf0f596e5"
 dependencies = [
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "async-broadcast"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7c48ccdbf6ca6b121e0f586cbc0e73ae440e56c67c30fa0873b4e110d9c26d2b"
+dependencies = [
+ "event-listener 2.5.3",
+ "futures-core",
+]
+
+[[package]]
 name = "async-channel"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81953c529336010edd6d8e358f886d9581267795c61b19475b71314bffa46d35"
 dependencies = [
  "concurrent-queue",
  "event-listener 2.5.3",
@@ -412,86 +622,167 @@
 
 [[package]]
 name = "async-executor"
 version = "1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c1da3ae8dabd9c00f453a329dfe1fb28da3c0a72e2478cdcd93171740c20499"
 dependencies = [
- "async-lock",
+ "async-lock 2.8.0",
  "async-task",
  "concurrent-queue",
  "fastrand 2.0.1",
  "futures-lite 1.13.0",
  "slab",
 ]
 
 [[package]]
+name = "async-fs"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "279cf904654eeebfa37ac9bb1598880884924aab82e290aa65c9e77a0e142e06"
+dependencies = [
+ "async-lock 2.8.0",
+ "autocfg",
+ "blocking",
+ "futures-lite 1.13.0",
+]
+
+[[package]]
+name = "async-fs"
+version = "2.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc19683171f287921f2405677dd2ed2549c3b3bda697a563ebc3a121ace2aba1"
+dependencies = [
+ "async-lock 3.3.0",
+ "blocking",
+ "futures-lite 2.2.0",
+]
+
+[[package]]
 name = "async-global-executor"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1b6f5d7df27bd294849f8eec66ecfc63d11814df7a4f5d74168a2394467b776"
 dependencies = [
  "async-channel 1.9.0",
  "async-executor",
- "async-io",
- "async-lock",
+ "async-io 1.13.0",
+ "async-lock 2.8.0",
  "blocking",
  "futures-lite 1.13.0",
  "once_cell",
  "tokio",
 ]
 
 [[package]]
 name = "async-io"
 version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fc5b45d93ef0529756f812ca52e44c221b35341892d3dcc34132ac02f3dd2af"
 dependencies = [
- "async-lock",
+ "async-lock 2.8.0",
  "autocfg",
  "cfg-if 1.0.0",
  "concurrent-queue",
  "futures-lite 1.13.0",
  "log",
  "parking",
- "polling",
+ "polling 2.8.0",
  "rustix 0.37.25",
  "slab",
  "socket2 0.4.9",
  "waker-fn",
 ]
 
 [[package]]
+name = "async-io"
+version = "2.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dcccb0f599cfa2f8ace422d3555572f47424da5648a4382a9dd0310ff8210884"
+dependencies = [
+ "async-lock 3.3.0",
+ "cfg-if 1.0.0",
+ "concurrent-queue",
+ "futures-io",
+ "futures-lite 2.2.0",
+ "parking",
+ "polling 3.5.0",
+ "rustix 0.38.32",
+ "slab",
+ "tracing",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "async-lock"
 version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "287272293e9d8c41773cec55e365490fe034813a2f172f502d6ddcf75b2f582b"
 dependencies = [
  "event-listener 2.5.3",
 ]
 
 [[package]]
+name = "async-lock"
+version = "3.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d034b430882f8381900d3fe6f0aaa3ad94f2cb4ac519b429692a1bc2dda4ae7b"
+dependencies = [
+ "event-listener 4.0.0",
+ "event-listener-strategy",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "async-net"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b948000fad4873c1c9339d60f2623323a0cfd3816e5181033c6a5cb68b2accf7"
+dependencies = [
+ "async-io 2.3.2",
+ "blocking",
+ "futures-lite 2.2.0",
+]
+
+[[package]]
+name = "async-once-cell"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9338790e78aa95a416786ec8389546c4b6a1dfc3dc36071ed9518a9413a542eb"
+
+[[package]]
 name = "async-process"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a9d28b1d97e08915212e2e45310d47854eafa69600756fc735fb788f75199c9"
 dependencies = [
- "async-io",
- "async-lock",
+ "async-io 1.13.0",
+ "async-lock 2.8.0",
  "autocfg",
  "blocking",
  "cfg-if 1.0.0",
  "event-listener 2.5.3",
  "futures-lite 1.13.0",
  "rustix 0.37.25",
  "signal-hook",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "async-recursion"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "30c5ef0ede93efbf733c1a727f3b6b5a1060bbedd5600183e66f6e4be4af0ec5"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
 name = "async-rustls"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93b21a03b7c21702a0110f9f8d228763a533570deb376119042dabf33c37a01a"
 dependencies = [
  "futures-io",
  "rustls 0.20.9",
@@ -503,16 +794,16 @@
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62565bb4402e926b29953c785397c6dc0391b7b446e45008b0049eb43cec6f5d"
 dependencies = [
  "async-attributes",
  "async-channel 1.9.0",
  "async-global-executor",
- "async-io",
- "async-lock",
+ "async-io 1.13.0",
+ "async-lock 2.8.0",
  "async-process",
  "crossbeam-utils",
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-lite 1.13.0",
  "gloo-timers",
@@ -574,14 +865,62 @@
 [[package]]
 name = "atomic-waker"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
 
 [[package]]
+name = "atspi"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6059f350ab6f593ea00727b334265c4dfc7fd442ee32d264794bd9bdc68e87ca"
+dependencies = [
+ "atspi-common",
+ "atspi-connection",
+ "atspi-proxies",
+]
+
+[[package]]
+name = "atspi-common"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92af95f966d2431f962bc632c2e68eda7777330158bf640c4af4249349b2cdf5"
+dependencies = [
+ "enumflags2",
+ "serde",
+ "static_assertions",
+ "zbus",
+ "zbus_names",
+ "zvariant",
+]
+
+[[package]]
+name = "atspi-connection"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0c65e7d70f86d4c0e3b2d585d9bf3f979f0b19d635a336725a88d279f76b939"
+dependencies = [
+ "atspi-common",
+ "atspi-proxies",
+ "futures-lite 1.13.0",
+ "zbus",
+]
+
+[[package]]
+name = "atspi-proxies"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6495661273703e7a229356dcbe8c8f38223d697aacfaf0e13590a9ac9977bb52"
+dependencies = [
+ "atspi-common",
+ "serde",
+ "zbus",
+]
+
+[[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
  "hermit-abi 0.1.19",
  "libc",
@@ -601,15 +940,15 @@
 checksum = "3b829e4e32b91e643de6eafe82b1d90675f5874230191a4ffbc1b336dec4d6bf"
 dependencies = [
  "async-trait",
  "axum-core",
  "bitflags 1.3.2",
  "bytes",
  "futures-util",
- "http",
+ "http 0.2.9",
  "http-body",
  "hyper",
  "itoa",
  "matchit",
  "memchr",
  "mime",
  "percent-encoding",
@@ -627,23 +966,29 @@
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "759fa577a247914fd3f7f76d62972792636412fbfd634cd452f6a385a74d2d2c"
 dependencies = [
  "async-trait",
  "bytes",
  "futures-util",
- "http",
+ "http 0.2.9",
  "http-body",
  "mime",
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
+name = "az"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
+
+[[package]]
 name = "backtrace"
 version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
 dependencies = [
  "addr2line",
  "cc",
@@ -707,28 +1052,28 @@
  "unicode-width",
  "walkdir",
  "wild",
 ]
 
 [[package]]
 name = "benchmark-example-node"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "benchmark-example-sink"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
  "tracing",
  "tracing-subscriber",
 ]
 
@@ -738,14 +1083,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "bit-set"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0700ddab506f33b20a03b13996eccd309a48e5ff77d0d95926aa0210fb4e95f1"
+dependencies = [
+ "bit-vec",
+]
+
+[[package]]
 name = "bit-vec"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "349f9b6a179ed607305526ca489b34ad0a41aed5f7980fa90eb03160b69598fb"
 
 [[package]]
 name = "bitflags"
@@ -754,44 +1108,92 @@
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4682ae6287fcf752ecaabbfcc7b6f9b72aa33933dc23a554d853aea8eea8635"
+dependencies = [
+ "bytemuck",
+ "serde",
+]
 
 [[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
  "funty",
  "radium",
  "tap",
  "wyz",
 ]
 
 [[package]]
+name = "block"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0d8c1fef690941d3e7788d328517591fecc684c084084702d6ff1641e993699a"
+
+[[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
+name = "block-sys"
+version = "0.1.0-beta.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0fa55741ee90902547802152aaf3f8e5248aab7e21468089560d4c8840561146"
+dependencies = [
+ "objc-sys 0.2.0-beta.2",
+]
+
+[[package]]
+name = "block-sys"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae85a0696e7ea3b835a453750bf002770776609115e6d25c6d2ff28a8200f7e7"
+dependencies = [
+ "objc-sys 0.3.3",
+]
+
+[[package]]
+name = "block2"
+version = "0.2.0-alpha.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8dd9e63c1744f755c2f60332b88de39d341e5e86239014ad839bd71c106dec42"
+dependencies = [
+ "block-sys 0.1.0-beta.1",
+ "objc2-encode 2.0.0-pre.2",
+]
+
+[[package]]
+name = "block2"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "15b55663a85f33501257357e6421bb33e769d5c9ffb5ba0921c975a123e35e68"
+dependencies = [
+ "block-sys 0.2.1",
+ "objc2 0.4.1",
+]
+
+[[package]]
 name = "blocking"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94c4ef1f913d78636d78d538eec1f18de81e481f44b1be0a81060090530846e1"
 dependencies = [
  "async-channel 1.9.0",
- "async-lock",
+ "async-lock 2.8.0",
  "async-task",
  "fastrand 2.0.1",
  "futures-io",
  "futures-lite 1.13.0",
  "piper",
  "tracing",
 ]
@@ -815,14 +1217,25 @@
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bstr"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
+dependencies = [
+ "lazy_static",
+ "memchr",
+ "regex-automata 0.1.10",
+]
+
+[[package]]
+name = "bstr"
 version = "1.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c2f7349907b712260e64b0afe2f84692af14a454be26187d9df565c7f69266a"
 dependencies = [
  "memchr",
  "regex-automata 0.3.9",
  "serde",
@@ -842,18 +1255,38 @@
 [[package]]
 name = "bumpalo"
 version = "3.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
 
 [[package]]
+name = "bytecount"
+version = "0.6.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ce89b21cab1437276d2650d57e971f9d548a2d9037cc231abdc0562b97498ce"
+
+[[package]]
 name = "bytemuck"
 version = "1.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "374d28ec25809ee0e23827c2ab573d729e293f281dfe393500e7ad618baa61c6"
+dependencies = [
+ "bytemuck_derive",
+]
+
+[[package]]
+name = "bytemuck_derive"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
@@ -875,14 +1308,85 @@
 [[package]]
 name = "cache-padded"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "981520c98f422fcc584dc1a95c334e6953900b9106bc47a9839b81790009eb21"
 
 [[package]]
+name = "calloop"
+version = "0.12.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fba7adb4dd5aa98e5553510223000e7148f621165ec5f9acd7113f6ca4995298"
+dependencies = [
+ "bitflags 2.4.0",
+ "log",
+ "polling 3.5.0",
+ "rustix 0.38.32",
+ "slab",
+ "thiserror",
+]
+
+[[package]]
+name = "calloop-wayland-source"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0f0ea9b9476c7fad82841a8dbb380e2eae480c21910feba80725b46931ed8f02"
+dependencies = [
+ "calloop",
+ "rustix 0.38.32",
+ "wayland-backend",
+ "wayland-client",
+]
+
+[[package]]
+name = "camino"
+version = "1.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c59e92b5a388f549b863a7bea62612c09f24c8393560709a54558a9abdfb3b9c"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "cargo-platform"
+version = "0.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24b1f0365a6c6bb4020cd05806fd0d33c44d38046b8bd7f0e40814b9763cabfc"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "cargo_metadata"
+version = "0.14.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4acbb09d9ee8e23699b9634375c72795d095bf268439da88562cf9b501f181fa"
+dependencies = [
+ "camino",
+ "cargo-platform",
+ "semver",
+ "serde",
+ "serde_json",
+]
+
+[[package]]
+name = "cargo_metadata"
+version = "0.18.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2d886547e41f740c616ae73108f6eb70afe6d940c7bc697cb30f13daec073037"
+dependencies = [
+ "camino",
+ "cargo-platform",
+ "semver",
+ "serde",
+ "serde_json",
+ "thiserror",
+]
+
+[[package]]
 name = "cc"
 version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
 dependencies = [
  "jobserver",
  "libc",
@@ -911,51 +1415,83 @@
 [[package]]
 name = "cesu8"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d43a04d8753f35258c91f8ec639f792891f748a1edbd759cf1dcea3382ad83c"
 
 [[package]]
+name = "cfb"
+version = "0.7.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d38f2da7a0a2c4ccf0065be06397cc26a81f4e528be095826eee9d4adbb8c60f"
+dependencies = [
+ "byteorder",
+ "fnv",
+ "uuid",
+]
+
+[[package]]
 name = "cfg-if"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4785bdd1c96b2a846b2bd7cc02e86b6b3dbf14e7e53446c4f54c92a361040822"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cfg_aliases"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
+
+[[package]]
+name = "cfg_aliases"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77e53693616d3075149f4ead59bdeecd204ac6b8192d8969757601b74bddf00f"
+
+[[package]]
 name = "chrono"
-version = "0.4.31"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
  "wasm-bindgen",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.0",
 ]
 
 [[package]]
 name = "cipher"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
 dependencies = [
  "crypto-common",
  "inout",
 ]
 
 [[package]]
+name = "clang-format"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "696283b40e1a39d208ee614b92e5f6521d16962edeb47c48372585ec92419943"
+dependencies = [
+ "thiserror",
+]
+
+[[package]]
 name = "clap"
 version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "atty",
  "bitflags 1.3.2",
@@ -1028,62 +1564,155 @@
 [[package]]
 name = "clap_lex"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd7cc57abe963c6d3b9d8be5b06ba7c8957a930305ca90304f24ef040aa6f961"
 
 [[package]]
+name = "clean-path"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aaa6b4b263a5d737e9bf6b7c09b72c41a5480aec4d7219af827f6564e950b6a5"
+
+[[package]]
+name = "clipboard-win"
+version = "5.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "79f4473f5144e20d9aceaf2972478f06ddf687831eafeeb434fbaf0acc4144ad"
+dependencies = [
+ "error-code",
+]
+
+[[package]]
 name = "clircle"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8e87cbed5354f17bd8ca8821a097fb62599787fe8f611743fad7ee156a0a600"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
  "serde",
  "winapi 0.3.9",
 ]
 
 [[package]]
+name = "cocoa"
+version = "0.25.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f6140449f97a6e97f9511815c5632d84c8aacf8ac271ad77c559218161a1373c"
+dependencies = [
+ "bitflags 1.3.2",
+ "block",
+ "cocoa-foundation",
+ "core-foundation",
+ "core-graphics",
+ "foreign-types",
+ "libc",
+ "objc",
+]
+
+[[package]]
+name = "cocoa-foundation"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8c6234cbb2e4c785b456c0644748b1ac416dd045799740356f8363dfe00c93f7"
+dependencies = [
+ "bitflags 1.3.2",
+ "block",
+ "core-foundation",
+ "core-graphics-types",
+ "libc",
+ "objc",
+]
+
+[[package]]
 name = "codespan-reporting"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
+name = "color_quant"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
+
+[[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
+name = "com"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e17887fd17353b65b1b2ef1c526c83e26cd72e74f598a8dc1bee13a48f3d9f6"
+dependencies = [
+ "com_macros",
+]
+
+[[package]]
+name = "com_macros"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d375883580a668c7481ea6631fc1a8863e33cc335bf56bfad8d7e6d4b04b13a5"
+dependencies = [
+ "com_macros_support",
+ "proc-macro2",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "com_macros_support"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad899a1087a9296d5644792d7cb72b8e34c1bec8e7d4fbc002230169a6e8710c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "combine"
 version = "4.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
+name = "comfy-table"
+version = "7.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b34115915337defe99b2aff5c2ce6771e5fbc4079f4b506301f5cf394c8452f7"
+dependencies = [
+ "strum 0.26.2",
+ "strum_macros 0.26.2",
+ "unicode-width",
+]
+
+[[package]]
 name = "communication-layer-pub-sub"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "flume 0.10.14",
  "zenoh",
 ]
 
 [[package]]
 name = "communication-layer-request-reply"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 
 [[package]]
 name = "concurrent-queue"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f057a694a54f12365049b0958a1685bb52d567f5593b355fbf685838e873d400"
 dependencies = [
@@ -1135,28 +1764,61 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7bda66e858c683005a53a9a60c69a4aca7eeaa45d124526e389f7aec8e62f38"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "convert_case"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
+dependencies = [
+ "unicode-segmentation",
+]
+
+[[package]]
 name = "core-foundation"
-version = "0.9.3"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.4"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
+
+[[package]]
+name = "core-graphics"
+version = "0.23.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+checksum = "c07782be35f9e1140080c6b96f0d44b739e2278479f64e02fdab4e32dfd8b081"
+dependencies = [
+ "bitflags 1.3.2",
+ "core-foundation",
+ "core-graphics-types",
+ "foreign-types",
+ "libc",
+]
+
+[[package]]
+name = "core-graphics-types"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "45390e6114f68f718cc7a830514a96f903cccd70d02a8f6d9f643ac4ba45afaf"
+dependencies = [
+ "bitflags 1.3.2",
+ "core-foundation",
+ "libc",
+]
 
 [[package]]
 name = "cpufeatures"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
@@ -1169,57 +1831,70 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if 1.0.0",
 ]
 
 [[package]]
+name = "crossbeam"
+version = "0.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1137cd7e7fc0fb5d3c5a8678be38ec56e819125d8d7907411fe24ccb943faca8"
+dependencies = [
+ "crossbeam-channel",
+ "crossbeam-deque",
+ "crossbeam-epoch",
+ "crossbeam-queue",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "crossbeam-channel"
-version = "0.5.8"
+version = "0.5.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
 dependencies = [
- "cfg-if 1.0.0",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.3"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
- "cfg-if 1.0.0",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.15"
+version = "0.9.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
- "autocfg",
- "cfg-if 1.0.0",
  "crossbeam-utils",
- "memoffset 0.9.0",
- "scopeguard",
 ]
 
 [[package]]
-name = "crossbeam-utils"
-version = "0.8.16"
+name = "crossbeam-queue"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
+checksum = "df0346b5d5e76ac2fe4e327c5fd1118d6be7c51dfb18f9b7922923f287471e35"
 dependencies = [
- "cfg-if 1.0.0",
+ "crossbeam-utils",
 ]
 
 [[package]]
+name = "crossbeam-utils"
+version = "0.8.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
 name = "crossterm"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e64e6c0fbe2c17357405f7c758c1ef960fce08bdfb2c03d88d2a18d7e09c4b67"
 dependencies = [
  "bitflags 1.3.2",
  "crossterm_winapi",
@@ -1294,14 +1969,20 @@
 checksum = "82e95fbd621905b854affdc67943b043a0fbb6ed7385fd5a25650d19a8a6cfdf"
 dependencies = [
  "nix 0.27.1",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "cursor-icon"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96a6ac251f4a2aca6b3f91340350eab87ae57c3f127ffeb585e92bd336717991"
+
+[[package]]
 name = "cxx"
 version = "1.0.118"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2673ca5ae28334544ec2a6b18ebe666c42a2650abfb48abbd532ed409a44be2b"
 dependencies = [
  "cc",
  "cxxbridge-flags",
@@ -1343,16 +2024,26 @@
 
 [[package]]
 name = "darling"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d706e75d87e35569db781a9b5e2416cff1236a47ed380831f959382ccd5f858"
 dependencies = [
- "darling_core",
- "darling_macro",
+ "darling_core 0.10.2",
+ "darling_macro 0.10.2",
+]
+
+[[package]]
+name = "darling"
+version = "0.20.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
+dependencies = [
+ "darling_core 0.20.8",
+ "darling_macro 0.20.8",
 ]
 
 [[package]]
 name = "darling_core"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0c960ae2da4de88a91b2d920c2a7233b400bc33cb28453a2987822d8392519b"
@@ -1362,38 +2053,68 @@
  "proc-macro2",
  "quote",
  "strsim 0.9.3",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "darling_core"
+version = "0.20.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
+dependencies = [
+ "fnv",
+ "ident_case",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
 name = "darling_macro"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b5a2f4ac4969822c62224815d069952656cadc7084fdca9751e6d959189b72"
 dependencies = [
- "darling_core",
+ "darling_core 0.10.2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "darling_macro"
+version = "0.20.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
+dependencies = [
+ "darling_core 0.20.8",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
 name = "dashmap"
 version = "5.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978747c1d849a7d2ee5e8adc0159961c48fb7e5db2f06af6723b80123bb53856"
 dependencies = [
  "cfg-if 1.0.0",
  "hashbrown 0.14.3",
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
+name = "data-encoding"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
+
+[[package]]
 name = "der"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1a467a65c5e759bce6e65eaf91cc29f466cdc57cb65777bd646872a8a1fd4de"
 dependencies = [
  "const-oid",
  "pem-rfc7468",
@@ -1401,28 +2122,52 @@
 ]
 
 [[package]]
 name = "deranged"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2696e8a945f658fd14dc3b87242e6b80cd0f36ff04ea560fa39082368847946"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "derivative"
+version = "2.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fcc3dd5e9e9c0b295d6e1e4d811fb6f157d5ffd784b8d202fc62eac8035a770b"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "const-oid",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
+name = "directories-next"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "339ee130d97a610ea5a5872d2bbb130fdf68884ff09d3028b81bec8a1ac23bbc"
+dependencies = [
+ "cfg-if 1.0.0",
+ "dirs-sys-next",
+]
+
+[[package]]
 name = "dirs"
 version = "4.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
 dependencies = [
  "dirs-sys 0.3.7",
 ]
@@ -1456,54 +2201,90 @@
  "libc",
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "dirs-sys-next"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4ebda144c4fe02d1f7ea1a7d9641b6fc6b580adcfa024ae48797ecdeb6825b4d"
+dependencies = [
+ "libc",
+ "redox_users",
+ "winapi 0.3.9",
+]
+
+[[package]]
+name = "dispatch"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd0c93bb4b0c6d9b77f4435b0ae98c24d17f1c45b2ff844c6151a07256ca923b"
+
+[[package]]
+name = "dlib"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "330c60081dcc4c72131f8eb70510f1ac07223e5d4163db481a04a0befcffa412"
+dependencies = [
+ "libloading 0.8.3",
+]
+
+[[package]]
+name = "document-features"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef5282ad69563b5fc40319526ba27e0e7363d552a896f0297d54f767717f9b95"
+dependencies = [
+ "litrs",
+]
+
+[[package]]
 name = "dora-arrow-convert"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow",
  "eyre",
 ]
 
 [[package]]
 name = "dora-cli"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "bat",
  "clap 4.4.6",
  "communication-layer-request-reply",
  "ctrlc",
  "dora-coordinator",
  "dora-core",
  "dora-daemon",
  "dora-node-api-c",
  "dora-operator-api-c",
  "dora-runtime",
  "dora-tracing",
+ "duration-str",
  "eyre",
  "futures",
  "inquire",
- "notify",
+ "notify 5.2.0",
  "serde",
  "serde_json",
  "serde_yaml 0.9.30",
  "termcolor",
  "tokio",
  "tokio-stream",
  "tracing",
  "uuid",
  "webbrowser",
 ]
 
 [[package]]
 name = "dora-coordinator"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "ctrlc",
  "dora-core",
  "dora-tracing",
  "eyre",
  "futures",
  "futures-concurrency",
@@ -1513,15 +2294,15 @@
  "tokio-stream",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-core"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "dora-message",
  "eyre",
  "once_cell",
  "serde",
  "serde-with-expand-env",
@@ -1530,15 +2311,15 @@
  "tracing",
  "uuid",
  "which",
 ]
 
 [[package]]
 name = "dora-daemon"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "async-trait",
  "bincode",
  "ctrlc",
  "dora-arrow-convert",
  "dora-core",
@@ -1548,24 +2329,26 @@
  "eyre",
  "flume 0.10.14",
  "futures",
  "futures-concurrency",
  "serde_json",
  "serde_yaml 0.8.26",
  "shared-memory-server",
+ "sysinfo 0.30.11",
  "tokio",
  "tokio-stream",
  "tracing",
  "tracing-opentelemetry",
  "uuid",
+ "which",
 ]
 
 [[package]]
 name = "dora-download"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "eyre",
  "reqwest",
  "tokio",
  "tracing",
 ]
 
@@ -1585,37 +2368,37 @@
  "tokio-stream",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-message"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow-data",
  "arrow-schema",
  "eyre",
  "serde",
  "uhlc",
 ]
 
 [[package]]
 name = "dora-metrics"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "eyre",
  "opentelemetry 0.22.0",
  "opentelemetry-otlp",
  "opentelemetry-system-metrics",
  "opentelemetry_sdk 0.22.1",
 ]
 
 [[package]]
 name = "dora-node-api"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "arrow",
  "bincode",
  "dora-arrow-convert",
  "dora-core",
  "dora-tracing",
@@ -1629,42 +2412,42 @@
  "shared_memory_extended",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-c"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow-array",
  "dora-node-api",
  "eyre",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-cxx"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-node-api",
  "dora-ros2-bridge",
  "dora-ros2-bridge-msg-gen",
  "eyre",
  "futures-lite 2.2.0",
- "prettyplease",
+ "prettyplease 0.1.25",
  "rust-format",
  "serde",
  "serde-big-array",
 ]
 
 [[package]]
 name = "dora-node-api-python"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-ros2-bridge-python",
  "dora-runtime",
  "eyre",
@@ -1673,82 +2456,93 @@
  "pyo3",
  "pythonize",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-arrow-convert",
  "dora-operator-api-macros",
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-c"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-cxx"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-operator-api",
 ]
 
 [[package]]
 name = "dora-operator-api-macros"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dora-operator-api-python"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "arrow",
  "arrow-schema",
  "dora-node-api",
  "eyre",
  "flume 0.10.14",
  "pyo3",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api-types"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow",
  "dora-arrow-convert",
  "safer-ffi",
 ]
 
 [[package]]
 name = "dora-record"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "chrono",
  "dora-node-api",
  "dora-tracing",
  "eyre",
  "parquet",
  "tokio",
 ]
 
 [[package]]
+name = "dora-rerun"
+version = "0.3.4-rc2"
+dependencies = [
+ "dora-node-api",
+ "eyre",
+ "ndarray",
+ "rerun",
+ "tokio",
+]
+
+[[package]]
 name = "dora-ros2-bridge"
 version = "0.1.0"
 dependencies = [
  "array-init",
  "dora-daemon",
  "dora-ros2-bridge-msg-gen",
  "eyre",
@@ -1768,21 +2562,23 @@
 ]
 
 [[package]]
 name = "dora-ros2-bridge-msg-gen"
 version = "0.1.0"
 dependencies = [
  "anyhow",
+ "glob",
  "heck 0.3.3",
  "nom",
  "proc-macro2",
  "quote",
  "regex",
  "syn 1.0.109",
  "thiserror",
+ "tracing",
 ]
 
 [[package]]
 name = "dora-ros2-bridge-python"
 version = "0.1.0"
 dependencies = [
  "arrow",
@@ -1793,70 +2589,284 @@
  "pyo3",
  "serde",
  "serde_assert",
 ]
 
 [[package]]
 name = "dora-runtime"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "arrow",
  "dora-core",
  "dora-download",
  "dora-metrics",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-operator-api-types",
  "dora-tracing",
  "eyre",
  "flume 0.10.14",
  "futures",
  "futures-concurrency",
- "libloading",
+ "libloading 0.7.4",
  "pyo3",
  "pythonize",
  "serde_yaml 0.8.26",
  "tokio",
  "tokio-stream",
  "tracing",
  "tracing-opentelemetry",
 ]
 
 [[package]]
 name = "dora-tracing"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "eyre",
  "opentelemetry 0.18.0",
  "opentelemetry-jaeger",
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
 ]
 
 [[package]]
+name = "downcast-rs"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75b325c5dbd37f80359721ad39aca5a29fb04c89279657cffdda8736d0c0b9d2"
+
+[[package]]
 name = "dunce"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
 
 [[package]]
+name = "duration-str"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9f037c488d179e21c87ef5fa9c331e8e62f5dddfa84618b41bb197da03edff1"
+dependencies = [
+ "chrono",
+ "nom",
+ "rust_decimal",
+ "serde",
+ "thiserror",
+ "time",
+]
+
+[[package]]
 name = "dyn-clone"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23d2f3407d9a573d666de4b5bdf10569d73ca9478087346697dcbae6244bfbcd"
 
 [[package]]
+name = "ecolor"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "20930a432bbd57a6d55e07976089708d4893f3d556cf42a0d79e9e321fa73b10"
+dependencies = [
+ "bytemuck",
+ "serde",
+]
+
+[[package]]
+name = "eframe"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "020e2ccef6bbcec71dbc542f7eed64a5846fc3076727f5746da8fd307c91bab2"
+dependencies = [
+ "bytemuck",
+ "cocoa",
+ "directories-next",
+ "document-features",
+ "egui",
+ "egui-wgpu",
+ "egui-winit",
+ "egui_glow",
+ "image",
+ "js-sys",
+ "log",
+ "objc",
+ "parking_lot",
+ "percent-encoding",
+ "pollster",
+ "puffin",
+ "raw-window-handle 0.6.0",
+ "ron",
+ "serde",
+ "static_assertions",
+ "thiserror",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "web-time",
+ "wgpu",
+ "winapi 0.3.9",
+ "winit",
+]
+
+[[package]]
+name = "egui"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "584c5d1bf9a67b25778a3323af222dbe1a1feb532190e103901187f92c7fe29a"
+dependencies = [
+ "accesskit",
+ "ahash",
+ "backtrace",
+ "epaint",
+ "log",
+ "nohash-hasher",
+ "puffin",
+ "ron",
+ "serde",
+]
+
+[[package]]
+name = "egui-wgpu"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "469ff65843f88a702b731a1532b7d03b0e8e96d283e70f3a22b0e06c46cb9b37"
+dependencies = [
+ "bytemuck",
+ "document-features",
+ "egui",
+ "epaint",
+ "log",
+ "puffin",
+ "thiserror",
+ "type-map",
+ "web-time",
+ "wgpu",
+ "winit",
+]
+
+[[package]]
+name = "egui-winit"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2e3da0cbe020f341450c599b35b92de4af7b00abde85624fd16f09c885573609"
+dependencies = [
+ "accesskit_winit",
+ "arboard",
+ "egui",
+ "log",
+ "puffin",
+ "raw-window-handle 0.6.0",
+ "serde",
+ "smithay-clipboard",
+ "web-time",
+ "webbrowser",
+ "winit",
+]
+
+[[package]]
+name = "egui_commonmark"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e30fc4d40a8ef399a8debfbdae0462ca45912d81b9e81b24373337669e961201"
+dependencies = [
+ "egui",
+ "egui_extras",
+ "pulldown-cmark 0.10.2",
+]
+
+[[package]]
+name = "egui_extras"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b78779f35ded1a853786c9ce0b43fe1053e10a21ea3b23ebea411805ce41593"
+dependencies = [
+ "egui",
+ "ehttp",
+ "enum-map",
+ "image",
+ "log",
+ "mime_guess2",
+ "puffin",
+ "serde",
+]
+
+[[package]]
+name = "egui_glow"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e0e5d975f3c86edc3d35b1db88bb27c15dde7c55d3b5af164968ab5ede3f44ca"
+dependencies = [
+ "bytemuck",
+ "egui",
+ "egui-winit",
+ "glow",
+ "log",
+ "memoffset 0.9.0",
+ "puffin",
+ "wasm-bindgen",
+ "web-sys",
+ "winit",
+]
+
+[[package]]
+name = "egui_plot"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a7854b86dc1c2d352c5270db3d600011daa913d6b554141a03939761323288a1"
+dependencies = [
+ "egui",
+]
+
+[[package]]
+name = "egui_tiles"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0e2c0ff99daddcbdc54b141dbb7be3b014463da48a03ebc801bf63e500b23d75"
+dependencies = [
+ "ahash",
+ "egui",
+ "itertools 0.12.1",
+ "log",
+ "serde",
+]
+
+[[package]]
+name = "ehttp"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "59a81c221a1e4dad06cb9c9deb19aea1193a5eea084e8cd42d869068132bf876"
+dependencies = [
+ "document-features",
+ "futures-util",
+ "js-sys",
+ "ureq",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "wasm-streams",
+ "web-sys",
+]
+
+[[package]]
 name = "either"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
+name = "emath"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e4c3a552cfca14630702449d35f41c84a0d15963273771c6059175a803620f3f"
+dependencies = [
+ "bytemuck",
+ "serde",
+]
+
+[[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
 [[package]]
 name = "encoding_rs"
@@ -1864,14 +2874,35 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
 dependencies = [
  "cfg-if 1.0.0",
 ]
 
 [[package]]
+name = "enum-map"
+version = "2.7.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6866f3bfdf8207509a033af1a75a7b08abda06bbaaeae6669323fd5a097df2e9"
+dependencies = [
+ "enum-map-derive",
+ "serde",
+]
+
+[[package]]
+name = "enum-map-derive"
+version = "0.17.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f282cfdfe92516eb26c2af8589c274c7c17681f5ecc03c18255fe741c6aa64eb"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
 name = "enumflags2"
 version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5998b4f30320c9d93aed72f63af821bfdac50465b75428fce77b48ec482c3939"
 dependencies = [
  "enumflags2_derive",
  "serde",
@@ -1885,27 +2916,78 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
+name = "enumn"
+version = "0.1.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fd000fd6988e73bbe993ea3db9b1aa64906ab88766d654973924340c8cddb42"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
+name = "enumset"
+version = "1.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "226c0da7462c13fb57e5cc9e0dc8f0635e7d27f276a3a7fd30054647f669007d"
+dependencies = [
+ "enumset_derive",
+]
+
+[[package]]
+name = "enumset_derive"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e08b6c6ab82d70f08844964ba10c7babb716de2ecaeab9be5717918a5177d3af"
+dependencies = [
+ "darling 0.20.8",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
 name = "env_logger"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85cdab6a89accf66733ad5a1693a4dcced6aeff64602b634530dd73c1f3ee9f0"
 dependencies = [
  "humantime",
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
+name = "epaint"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b381f8b149657a4acf837095351839f32cd5c4aec1817fc4df84e18d76334176"
+dependencies = [
+ "ab_glyph",
+ "ahash",
+ "bytemuck",
+ "ecolor",
+ "emath",
+ "log",
+ "nohash-hasher",
+ "parking_lot",
+ "puffin",
+ "rayon",
+ "serde",
+]
+
+[[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
@@ -1914,25 +2996,46 @@
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "error-chain"
+version = "0.12.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2d2f06b9cac1506ece98fe3231e3cc9c4410ec3d5b1f24ae1c8946f0742cdefc"
+dependencies = [
+ "version_check",
+]
+
+[[package]]
+name = "error-code"
+version = "3.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0474425d51df81997e2f90a21591180b38eccf27292d755f3e30750225c175b"
+
+[[package]]
 name = "etcetera"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "136d1b5283a1ab77bd9257427ffd09d8667ced0570b6f938942bc7568ed5b943"
 dependencies = [
  "cfg-if 1.0.0",
  "home",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "ethnum"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b90ca2580b73ab6a1f724b76ca11ab632df820fd6040c336200d2c1df7b3c82c"
+
+[[package]]
 name = "event-listener"
 version = "2.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
 name = "event-listener"
@@ -1952,14 +3055,29 @@
 checksum = "958e4d70b6d5e81971bebec42271ec641e7ff4e170a6fa605f2b8a8b65cb97d3"
 dependencies = [
  "event-listener 4.0.0",
  "pin-project-lite",
 ]
 
 [[package]]
+name = "ewebsock"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6177769715c6ec5a324acee995183b22721ea23c58e49af14a828eadec85d120"
+dependencies = [
+ "document-features",
+ "js-sys",
+ "log",
+ "tungstenite 0.21.0",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+]
+
+[[package]]
 name = "ext-trait"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d772df1c1a777963712fb68e014235e80863d6a91a85c4e06ba2d16243a310e5"
 dependencies = [
  "ext-trait-proc_macros",
 ]
@@ -2006,26 +3124,48 @@
 [[package]]
 name = "fastrand"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
 
 [[package]]
+name = "fdeflate"
+version = "0.3.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4f9bfee30e4dedf0ab8b422f03af778d9612b63f502710fc500a334ebe2de645"
+dependencies = [
+ "simd-adler32",
+]
+
+[[package]]
 name = "filetime"
 version = "0.2.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4029edd3e734da6fe05b6cd7bd2960760a616bd2ddd0d59a0124746d6272af0"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
  "redox_syscall 0.3.5",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "fixed"
+version = "1.27.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fc715d38bea7b5bf487fcd79bcf8c209f0b58014f3018a7a19c2b855f472048"
+dependencies = [
+ "az",
+ "bytemuck",
+ "half",
+ "serde",
+ "typenum",
+]
+
+[[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flatbuffers"
@@ -2075,14 +3215,47 @@
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
+name = "foreign-types"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d737d9aa519fb7b749cbc3b962edcf310a8dd1f4b67c91c4f83975dbdd17d965"
+dependencies = [
+ "foreign-types-macros",
+ "foreign-types-shared",
+]
+
+[[package]]
+name = "foreign-types-macros"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a5c6c585bc94aaf2c7b51dd4c2ba22680844aba4c687be581871a6f518c5742"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
+name = "foreign-types-shared"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa9a19cbb55df58761df49b23516a86d432839add4af60fc256da840f66ed35b"
+
+[[package]]
+name = "foreign_vec"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
+
+[[package]]
 name = "form_urlencoded"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
@@ -2262,14 +3435,24 @@
 checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
+name = "gethostname"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0176e0459c2e4a1fe232f984bca6890e681076abb9934f6cea7c326f3fc47818"
+dependencies = [
+ "libc",
+ "windows-targets 0.48.5",
+]
+
+[[package]]
 name = "getrandom"
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if 1.0.0",
  "js-sys",
@@ -2327,27 +3510,48 @@
  "libc",
  "libgit2-sys",
  "log",
  "url",
 ]
 
 [[package]]
+name = "gl_generator"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a95dfc23a2b4a9a2f5ab41d194f8bfda3cabec42af4e39f08c339eb2a0c124d"
+dependencies = [
+ "khronos_api",
+ "log",
+ "xml-rs",
+]
+
+[[package]]
+name = "glam"
+version = "0.22.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "12f597d56c1bd55a811a1be189459e8fad2bbc272616375602443bdfb37fa774"
+dependencies = [
+ "bytemuck",
+ "serde",
+]
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "globset"
 version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "57da3b9b5b85bd66f31093f8c408b90a74431672542466497dcbdfdc02034be1"
 dependencies = [
  "aho-corasick",
- "bstr",
+ "bstr 1.6.2",
  "log",
  "regex-automata 0.4.3",
  "regex-syntax 0.8.2",
 ]
 
 [[package]]
 name = "gloo-timers"
@@ -2358,20 +3562,132 @@
  "futures-channel",
  "futures-core",
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "glow"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd348e04c43b32574f2de31c8bb397d96c9fcfa1371bd4ca6d8bdc464ab121b1"
+dependencies = [
+ "js-sys",
+ "slotmap",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
+name = "gltf"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b78f069cf941075835822953c345b9e1edd67ae347b81ace3aea9de38c2ef33"
+dependencies = [
+ "base64 0.13.1",
+ "byteorder",
+ "gltf-json",
+ "image",
+ "lazy_static",
+ "serde_json",
+ "urlencoding",
+]
+
+[[package]]
+name = "gltf-derive"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "438ffe1a5540d75403feaf23636b164e816e93f6f03131674722b3886ce32a57"
+dependencies = [
+ "inflections",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
+name = "gltf-json"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "655951ba557f2bc69ea4b0799446bae281fa78efae6319968bdd2c3e9a06d8e1"
+dependencies = [
+ "gltf-derive",
+ "serde",
+ "serde_derive",
+ "serde_json",
+]
+
+[[package]]
+name = "glutin_wgl_sys"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c8098adac955faa2d31079b65dc48841251f69efd3ac25477903fc424362ead"
+dependencies = [
+ "gl_generator",
+]
+
+[[package]]
+name = "gpu-alloc"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fbcd2dba93594b227a1f57ee09b8b9da8892c34d55aa332e034a228d0fe6a171"
+dependencies = [
+ "bitflags 2.4.0",
+ "gpu-alloc-types",
+]
+
+[[package]]
+name = "gpu-alloc-types"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "98ff03b468aa837d70984d55f5d3f846f6ec31fe34bbb97c4f85219caeee1ca4"
+dependencies = [
+ "bitflags 2.4.0",
+]
+
+[[package]]
+name = "gpu-allocator"
+version = "0.25.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f56f6318968d03c18e1bcf4857ff88c61157e9da8e47c5f29055d60e1228884"
+dependencies = [
+ "log",
+ "presser",
+ "thiserror",
+ "winapi 0.3.9",
+ "windows 0.52.0",
+]
+
+[[package]]
+name = "gpu-descriptor"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cc11df1ace8e7e564511f53af41f3e42ddc95b56fd07b3f4445d2a6048bc682c"
+dependencies = [
+ "bitflags 2.4.0",
+ "gpu-descriptor-types",
+ "hashbrown 0.14.3",
+]
+
+[[package]]
+name = "gpu-descriptor-types"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6bf0b36e6f090b7e1d8a4b49c0cb81c1f8376f72198c65dd3ad9ff3556b8b78c"
+dependencies = [
+ "bitflags 2.4.0",
+]
+
+[[package]]
 name = "grep-cli"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8fe4bdbf4300c8b039f5d7eec7fbc6760d2c85bb15ac7499c4d235667f6d747a"
 dependencies = [
- "bstr",
+ "bstr 1.6.2",
  "globset",
  "lazy_static",
  "log",
  "regex",
  "same-file",
  "termcolor",
  "winapi-util",
@@ -2384,44 +3700,70 @@
 checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
- "http",
- "indexmap 2.0.2",
+ "http 0.2.9",
+ "indexmap 2.2.6",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "half"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
 dependencies = [
+ "bytemuck",
  "cfg-if 1.0.0",
  "crunchy",
  "num-traits",
 ]
 
 [[package]]
+name = "hash_hasher"
+version = "2.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
+
+[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+dependencies = [
+ "ahash",
+ "allocator-api2",
+]
+
+[[package]]
+name = "hassle-rs"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af2a7e73e1f34c48da31fb668a907f250794837e08faa144fd24f0b8b741e890"
+dependencies = [
+ "bitflags 2.4.0",
+ "com",
+ "libc",
+ "libloading 0.8.3",
+ "thiserror",
+ "widestring",
+ "winapi 0.3.9",
+]
 
 [[package]]
 name = "heck"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
 dependencies = [
@@ -2452,14 +3794,20 @@
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
+name = "hexf-parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dfa686283ad6dd069f105e5ab091b04c62850d3e4cf5d67debad1933f55023df"
+
+[[package]]
 name = "hmac"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
@@ -2481,21 +3829,32 @@
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
+name = "http"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
 name = "http-body"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
 dependencies = [
  "bytes",
- "http",
+ "http 0.2.9",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2520,15 +3879,15 @@
 checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
- "http",
+ "http 0.2.9",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
  "socket2 0.4.9",
  "tokio",
@@ -2540,15 +3899,15 @@
 [[package]]
 name = "hyper-rustls"
 version = "0.24.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
 dependencies = [
  "futures-util",
- "http",
+ "http 0.2.9",
  "hyper",
  "rustls 0.21.10",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
@@ -2583,14 +3942,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
+name = "icrate"
+version = "0.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "99d3aaff8a54577104bafdf686ff18565c3b6903ca5782a2026ef06e2c7aa319"
+dependencies = [
+ "block2 0.3.0",
+ "dispatch",
+ "objc2 0.4.1",
+]
+
+[[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
 name = "idna"
@@ -2600,23 +3970,44 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "if-addrs"
-version = "0.10.2"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cabb0019d51a643781ff15c9c8a3e5dedc365c47211270f4e8f82812fedd8f0a"
+checksum = "624c5448ba529e74f594c65b7024f31b2de7b64a9b228b8df26796bbb6e32c36"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "image"
+version = "0.24.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5690139d2f55868e080017335e4b94cb7414274c74f1669c84fb5feba2c9f69d"
+dependencies = [
+ "bytemuck",
+ "byteorder",
+ "color_quant",
+ "jpeg-decoder",
+ "num-traits",
+ "png",
+ "tiff",
+]
+
+[[package]]
+name = "indent"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9f1a0777d972970f204fdf8ef319f1f4f8459131636d7e3c96c5d59570d0fa6"
+
+[[package]]
 name = "indenter"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce23b50ad8242c51a442f3ff322d56b02f08852c77e4c0b4d3fd684abc89c683"
 
 [[package]]
 name = "indexmap"
@@ -2626,29 +4017,45 @@
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.0.2"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8adf3ddd720272c6ea8bf59463c04e0f93d0bbf7c5439b691bca2987e0270897"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown 0.14.3",
+ "serde",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
 
 [[package]]
+name = "infer"
+version = "0.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cb33622da908807a06f9513c19b3c1ad50fab3e4137d82a78107d502075aa199"
+dependencies = [
+ "cfb",
+]
+
+[[package]]
+name = "inflections"
+version = "1.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a257582fdcde896fd96463bf2d40eefea0580021c0712a0e2b028b60b47a837a"
+
+[[package]]
 name = "inotify"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8069d3ec154eb856955c1c0fbffefbf5f3c40a104ec912d4797314c1801abff"
 dependencies = [
  "bitflags 1.3.2",
  "inotify-sys",
@@ -2786,15 +4193,15 @@
 [[package]]
 name = "is-terminal"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
  "hermit-abi 0.3.3",
- "rustix 0.38.28",
+ "rustix 0.38.32",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2809,14 +4216,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "jni"
@@ -2846,18 +4262,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "jpeg-decoder"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f5d4a7da358eff58addd2877a45865158f0d78c911d43a5784ceb7bbf52833b0"
+
+[[package]]
 name = "js-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "json5"
 version = "0.4.1"
@@ -2885,14 +4307,31 @@
 checksum = "7507624b29483431c0ba2d82aece8ca6cdba9382bff4ddd0f7490560c056098d"
 dependencies = [
  "winapi 0.2.8",
  "winapi-build",
 ]
 
 [[package]]
+name = "khronos-egl"
+version = "6.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6aae1df220ece3c0ada96b8153459b67eebe9ae9212258bb0134ae60416fdf76"
+dependencies = [
+ "libc",
+ "libloading 0.8.3",
+ "pkg-config",
+]
+
+[[package]]
+name = "khronos_api"
+version = "3.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2db585e1d738fc771bf08a151420d3ed193d9d895a36df7f6f8a9456b911ddc"
+
+[[package]]
 name = "kqueue"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7447f1ca1b7b563588a205fe93dea8df60fd981423a768bc1c0ded35ed147d0c"
 dependencies = [
  "kqueue-sys",
  "libc",
@@ -2994,17 +4433,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libgit2-sys"
 version = "0.16.2+1.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee4126d8b4ee5c9d9ea891dd875cfdc1e9d0950437179104b183d7d8a74d24e8"
 dependencies = [
@@ -3021,20 +4460,41 @@
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
  "cfg-if 1.0.0",
  "winapi 0.3.9",
 ]
 
 [[package]]
+name = "libloading"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
+dependencies = [
+ "cfg-if 1.0.0",
+ "windows-targets 0.52.0",
+]
+
+[[package]]
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
+name = "libredox"
+version = "0.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3af92c55d7d839293953fcd0fda5ecfe93297cfde6ffbdec13b41d99c0ba6607"
+dependencies = [
+ "bitflags 2.4.0",
+ "libc",
+ "redox_syscall 0.4.1",
+]
+
+[[package]]
 name = "libz-sys"
 version = "1.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d97137b25e321a73eef1418d1d5d2eda4d77e12813f8e6dead84bc52c5870a7b"
 dependencies = [
  "cc",
  "libc",
@@ -3075,18 +4535,24 @@
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4cd1a83af159aa67994778be9070f0ae1bd732942279cabb14f86f986a21456"
 
 [[package]]
+name = "litrs"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4ce301924b7887e9d637144fdade93f9dfff9b60981d4ac161db09720d39aa5"
+
+[[package]]
 name = "local-ip-address"
-version = "0.5.6"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "66357e687a569abca487dc399a9c9ac19beb3f13991ed49f00c144e02cbd42ab"
+checksum = "136ef34e18462b17bf39a7826f8f3bbc223341f8e83822beb8b77db9a3d49696"
 dependencies = [
  "libc",
  "neli",
  "thiserror",
  "windows-sys 0.48.0",
 ]
 
@@ -3094,35 +4560,56 @@
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
+ "serde",
 ]
 
 [[package]]
 name = "log"
 version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 dependencies = [
  "value-bag",
 ]
 
 [[package]]
+name = "log-once"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d8a05e3879b317b1b6dbf353e5bba7062bedcc59815267bb23eaa0c576cebf0"
+dependencies = [
+ "log",
+]
+
+[[package]]
 name = "lz4_flex"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "912b45c753ff5f7f5208307e8ace7d2a2e30d024e26d3509f3dce546c044ce15"
 dependencies = [
  "twox-hash",
 ]
 
 [[package]]
+name = "macaw"
+version = "0.18.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8fdbfdf07a7e53090afb7fd427eb0a4b46fc51cb484b2deba27b47919762dfb"
+dependencies = [
+ "glam",
+ "num-traits",
+ "serde",
+]
+
+[[package]]
 name = "macro_rules_attribute"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf0c9b980bf4f3a37fd7b1c066941dd1b1d0152ce6ee6e8fe8c49b9f6810d862"
 dependencies = [
  "macro_rules_attribute-proc_macro",
  "paste",
@@ -3155,26 +4642,45 @@
 [[package]]
 name = "matchit"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e7465ac9959cc2b1404e8e2367b43684a6d13790fe23056cc8c6c5a6b7bcb94"
 
 [[package]]
+name = "matrixmultiply"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7574c1cf36da4798ab73da5b215bbf444f50718207754cb522201d78d1cd0ff2"
+dependencies = [
+ "autocfg",
+ "rawpointer",
+]
+
+[[package]]
 name = "md5"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "490cc448043f947bae3cbee9c203358d62dbee0db12107a74be5c30ccfd09771"
 
 [[package]]
 name = "memchr"
 version = "2.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
 
 [[package]]
+name = "memmap2"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe751422e4a8caa417e13c3ea66452215d7d63e19e604f4980461212f3ae1322"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "memoffset"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
@@ -3203,32 +4709,68 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memory-stats"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34f79cf9964c5c9545493acda1263f1912f8d2c56c8a2ffee2606cb960acaacc"
+dependencies = [
+ "libc",
+ "winapi 0.3.9",
+]
+
+[[package]]
+name = "metal"
+version = "0.27.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c43f73953f8cbe511f021b58f18c3ce1c3d1ae13fe953293e13345bf83217f25"
+dependencies = [
+ "bitflags 2.4.0",
+ "block",
+ "core-graphics-types",
+ "foreign-types",
+ "log",
+ "objc",
+ "paste",
+]
+
+[[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
+name = "mime_guess2"
+version = "2.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "25a3333bb1609500601edc766a39b4c1772874a4ce26022f4d866854dc020c41"
+dependencies = [
+ "mime",
+ "unicase",
+]
+
+[[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
+ "simd-adler32",
 ]
 
 [[package]]
 name = "mio"
 version = "0.6.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4afd66f5b91bf2a3bc13fad0e21caedac168ca4c707504e75585648ae80e4cc4"
@@ -3280,39 +4822,59 @@
  "net2",
  "winapi 0.2.8",
  "ws2_32-sys",
 ]
 
 [[package]]
 name = "multiple-daemons-example-node"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "multiple-daemons-example-operator"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "multiple-daemons-example-sink"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
+name = "naga"
+version = "0.19.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50e3524642f53d9af419ab5e8dd29d3ba155708267667c2f3f06c88c9e130843"
+dependencies = [
+ "bit-set",
+ "bitflags 2.4.0",
+ "codespan-reporting",
+ "hexf-parse",
+ "indexmap 2.2.6",
+ "log",
+ "num-traits",
+ "rustc-hash",
+ "spirv",
+ "termcolor",
+ "thiserror",
+ "unicode-xid",
+]
+
+[[package]]
 name = "names"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bddcd3bf5144b6392de80e04c347cd7fab2508f6df16a85fc496ecd5cec39bc"
 dependencies = [
  "clap 3.2.25",
  "rand",
@@ -3324,20 +4886,63 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
+name = "natord"
+version = "1.0.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "308d96db8debc727c3fd9744aac51751243420e46edf401010908da7f8d5e57c"
+
+[[package]]
+name = "ndarray"
+version = "0.15.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
+dependencies = [
+ "matrixmultiply",
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "rawpointer",
+]
+
+[[package]]
+name = "ndk"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2076a31b7010b17a38c01907c45b945e8f11495ee4dd588309718901b1f7a5b7"
+dependencies = [
+ "bitflags 2.4.0",
+ "jni-sys",
+ "log",
+ "ndk-sys",
+ "num_enum",
+ "raw-window-handle 0.6.0",
+ "thiserror",
+]
+
+[[package]]
 name = "ndk-context"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "27b02d87554356db9e9a873add8782d4ea6e3e58ea071a9adb9a2e8ddb884a8b"
 
 [[package]]
+name = "ndk-sys"
+version = "0.5.0+25.2.9519653"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8c196769dd60fd4f363e11d948139556a344e79d451aeb2fa2fd040738ef7691"
+dependencies = [
+ "jni-sys",
+]
+
+[[package]]
 name = "neli"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1100229e06604150b3becd61a4965d5c70f3be1759544ea7274166f4be41ef43"
 dependencies = [
  "byteorder",
  "libc",
@@ -3366,14 +4971,20 @@
 dependencies = [
  "cfg-if 0.1.10",
  "libc",
  "winapi 0.3.9",
 ]
 
 [[package]]
+name = "never"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c96aba5aa877601bb3f6dd6a63a969e1f82e60646e81e71b14496995e9853c91"
+
+[[package]]
 name = "newline-converter"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f71d09d5c87634207f894c6b31b6a2b2c64ea3bdcf71bd5599fdbbe1600c00f"
 dependencies = [
  "unicode-segmentation",
 ]
@@ -3418,14 +5029,20 @@
 [[package]]
 name = "no-std-net"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43794a0ace135be66a25d3ae77d41b91615fb68ae937f904090203e81f755b65"
 
 [[package]]
+name = "nohash-hasher"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2bf50223579dc7cdcfb3bfcacf7069ff68243f8c363f62ffa99cf000a6b9c451"
+
+[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
@@ -3446,14 +5063,33 @@
  "libc",
  "mio 0.8.11",
  "walkdir",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "notify"
+version = "6.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6205bd8bb1e454ad2e27422015fb5e4f2bcc7e08fa8f27058670d208324a4d2d"
+dependencies = [
+ "bitflags 2.4.0",
+ "crossbeam-channel",
+ "filetime",
+ "fsevent-sys",
+ "inotify",
+ "kqueue",
+ "libc",
+ "log",
+ "mio 0.8.11",
+ "walkdir",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "ntapi"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e8a3895c6391c39d7fe7ebc444a87eb2991b2a0bc718fdabd071eec617fc68e4"
 dependencies = [
  "winapi 0.3.9",
 ]
@@ -3589,59 +5225,167 @@
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi 0.3.3",
  "libc",
 ]
 
 [[package]]
+name = "num_enum"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02339744ee7253741199f897151b38e72257d13802d4ee837285cc2990a90845"
+dependencies = [
+ "num_enum_derive",
+]
+
+[[package]]
+name = "num_enum_derive"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
+dependencies = [
+ "proc-macro-crate 3.1.0",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
+name = "num_threads"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c7398b9c8b70908f6371f47ed36737907c87c52af34c268fed0bf0ceb92ead9"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "nvml-wrapper"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7cd21b9f5a1cce3c3515c9ffa85f5c7443e07162dae0ccf4339bb7ca38ad3454"
 dependencies = [
  "bitflags 1.3.2",
- "libloading",
+ "libloading 0.7.4",
  "nvml-wrapper-sys",
  "static_assertions",
  "thiserror",
  "wrapcenum-derive",
 ]
 
 [[package]]
 name = "nvml-wrapper-sys"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c961a2ea9e91c59a69b78e69090f6f5b867bb46c0c56de9482da232437c4987e"
 dependencies = [
- "libloading",
+ "libloading 0.7.4",
 ]
 
 [[package]]
 name = "objc"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "915b1b472bc21c53464d6c8461c9d3af805ba1ef837e1cac254428f4a77177b1"
 dependencies = [
  "malloc_buf",
+ "objc_exception",
+]
+
+[[package]]
+name = "objc-foundation"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1add1b659e36c9607c7aab864a76c7a4c2760cd0cd2e120f3fb8b952c7e22bf9"
+dependencies = [
+ "block",
+ "objc",
+ "objc_id",
+]
+
+[[package]]
+name = "objc-sys"
+version = "0.2.0-beta.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df3b9834c1e95694a05a828b59f55fa2afec6288359cda67146126b3f90a55d7"
+
+[[package]]
+name = "objc-sys"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da284c198fb9b7b0603f8635185e85fbd5b64ee154b1ed406d489077de2d6d60"
+
+[[package]]
+name = "objc2"
+version = "0.3.0-beta.3.patch-leaks.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e01640f9f2cb1220bbe80325e179e532cb3379ebcd1bf2279d703c19fe3a468"
+dependencies = [
+ "block2 0.2.0-alpha.6",
+ "objc-sys 0.2.0-beta.2",
+ "objc2-encode 2.0.0-pre.2",
+]
+
+[[package]]
+name = "objc2"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "559c5a40fdd30eb5e344fbceacf7595a81e242529fb4e21cf5f43fb4f11ff98d"
+dependencies = [
+ "objc-sys 0.3.3",
+ "objc2-encode 3.0.0",
+]
+
+[[package]]
+name = "objc2-encode"
+version = "2.0.0-pre.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "abfcac41015b00a120608fdaa6938c44cb983fee294351cc4bac7638b4e50512"
+dependencies = [
+ "objc-sys 0.2.0-beta.2",
+]
+
+[[package]]
+name = "objc2-encode"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d079845b37af429bfe5dfa76e6d087d788031045b25cfc6fd898486fd9847666"
+
+[[package]]
+name = "objc_exception"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad970fb455818ad6cba4c122ad012fae53ae8b4795f86378bce65e4f6bab2ca4"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "objc_id"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c92d4ddb4bd7b50d730c215ff871754d0da6b2178849f8a2a2ab69712d0c073b"
+dependencies = [
+ "objc",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "onig"
 version = "6.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c4b31c8722ad9171c6d77d3557db078cab2bd50afcc9d09c8b315c59df8ca4f"
 dependencies = [
@@ -3713,15 +5457,15 @@
 name = "opentelemetry-otlp"
 version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a016b8d9495c639af2145ac22387dcb88e44118e45320d9238fbf4e7889abcb"
 dependencies = [
  "async-trait",
  "futures-core",
- "http",
+ "http 0.2.9",
  "opentelemetry 0.22.0",
  "opentelemetry-proto",
  "opentelemetry-semantic-conventions 0.14.0",
  "opentelemetry_sdk 0.22.1",
  "prost",
  "thiserror",
  "tokio",
@@ -3761,15 +5505,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dca748d4fe59e208f6c71bde86573d326f98ed29696d31dbf7d2454b8f1af2d"
 dependencies = [
  "eyre",
  "indexmap 1.9.3",
  "nvml-wrapper",
  "opentelemetry 0.22.0",
- "sysinfo",
+ "sysinfo 0.29.10",
  "tracing",
 ]
 
 [[package]]
 name = "opentelemetry_api"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3817,29 +5561,38 @@
  "crossbeam-channel",
  "futures-channel",
  "futures-executor",
  "futures-util",
  "glob",
  "once_cell",
  "opentelemetry 0.22.0",
- "ordered-float 4.1.1",
+ "ordered-float 4.2.0",
  "percent-encoding",
  "rand",
  "thiserror",
  "tokio",
  "tokio-stream",
 ]
 
 [[package]]
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
+name = "orbclient"
+version = "0.3.47"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "52f0d54bde9774d3a51dcf281a5def240c71996bc6ca05d2c847ec8b2b216166"
+dependencies = [
+ "libredox",
+]
+
+[[package]]
 name = "ordered-float"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3305af35278dd29f46fcdd139e0b1fbfae2153f0e5928b39b035542dd31e37b7"
 dependencies = [
  "num-traits",
 ]
@@ -3860,34 +5613,53 @@
 checksum = "2a54938017eacd63036332b4ae5c8a49fc8c0c1d6d629893057e4f13609edd06"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "ordered-float"
-version = "4.1.1"
+version = "4.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "536900a8093134cf9ccf00a27deb3532421099e958d9dd431135d0c7543ca1e8"
+checksum = "a76df7075c7d4d01fdcb46c912dd17fba5b60c78ea480b475f2b6ab6f666584e"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "ordered-stream"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9aa2b01e1d916879f73a53d01d1d6cee68adbb31d6d9177a8cfce093cced1d50"
+dependencies = [
+ "futures-core",
+ "pin-project-lite",
+]
+
+[[package]]
 name = "os_str_bytes"
 version = "6.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4d5d9eb14b174ee9aa2ef96dc2b94637a2d4b6e7cb873c7e171f0c20c6cf3eac"
 
 [[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
+name = "owned_ttf_parser"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d4586edfe4c648c71797a74c84bacb32b52b212eff5dfe2bb9f2c599844023e7"
+dependencies = [
+ "ttf-parser",
+]
+
+[[package]]
 name = "parking"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb813b8af86854136c6922af0598d719255ecb2179515e6e7730d468f05c9cae"
 
 [[package]]
 name = "parking_lot"
@@ -3957,14 +5729,47 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05ef02f6342ac01d8a93b65f96db53fe68a92a15f41144f97fb00a9e669633c3"
 dependencies = [
  "std_prelude",
 ]
 
 [[package]]
+name = "pathdiff"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
+
+[[package]]
+name = "peg"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9f76678828272f177ac33b7e2ac2e3e73cc6c1cd1e3e387928aa69562fa51367"
+dependencies = [
+ "peg-macros",
+ "peg-runtime",
+]
+
+[[package]]
+name = "peg-macros"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "636d60acf97633e48d266d7415a9355d4389cea327a193f87df395d88cd2b14d"
+dependencies = [
+ "peg-runtime",
+ "proc-macro2",
+ "quote",
+]
+
+[[package]]
+name = "peg-runtime"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9555b1514d2d99d78150d3c799d4c357a3e2c2a8062cd108e93a06d9057629c5"
+
+[[package]]
 name = "pem-rfc7468"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24d159833a9105500e0398934e205e0773f0b27529557134ecfc51c27646adac"
 dependencies = [
  "base64ct",
 ]
@@ -4023,15 +5828,15 @@
 [[package]]
 name = "petgraph"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
 dependencies = [
  "fixedbitset",
- "indexmap 2.0.2",
+ "indexmap 2.2.6",
 ]
 
 [[package]]
 name = "pin-project"
 version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fda4ed1c6c173e3fc7a83629421152e01d7b1f9b7f65fb301e490e8cfc656422"
@@ -4098,28 +5903,49 @@
 [[package]]
 name = "pkg-config"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
+name = "planus"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
+dependencies = [
+ "array-init-cursor",
+]
+
+[[package]]
 name = "plist"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdc0001cfea3db57a2e24bc0d818e9e20e554b5f97fabb9bc231dc240269ae06"
 dependencies = [
  "base64 0.21.4",
  "indexmap 1.9.3",
  "line-wrap",
- "quick-xml",
+ "quick-xml 0.29.0",
  "serde",
  "time",
 ]
 
 [[package]]
+name = "ply-rs"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dbadf9cb4a79d516de4c64806fe64ffbd8161d1ac685d000be789fb628b88963"
+dependencies = [
+ "byteorder",
+ "linked-hash-map",
+ "peg",
+ "skeptic",
+]
+
+[[package]]
 name = "pnet"
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0caaf5b11fd907ff15cf14a4477bfabca4b37ab9e447a4f8dead969a59cdafad"
 dependencies = [
  "pnet_base",
  "pnet_datalink",
@@ -4201,14 +6027,39 @@
  "libc",
  "pnet_base",
  "pnet_packet",
  "pnet_sys",
 ]
 
 [[package]]
+name = "png"
+version = "0.17.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "06e4b0d3d1312775e782c86c91a111aa1f910cbb65e1337f9975b5f9a554b5e1"
+dependencies = [
+ "bitflags 1.3.2",
+ "crc32fast",
+ "fdeflate",
+ "flate2",
+ "miniz_oxide",
+]
+
+[[package]]
+name = "poll-promise"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5f6a58fecbf9da8965bcdb20ce4fd29788d1acee68ddbb64f0ba1b81bccdb7df"
+dependencies = [
+ "document-features",
+ "static_assertions",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+]
+
+[[package]]
 name = "polling"
 version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b2d323e8ca7996b3e23126511a523f7e62924d93ecd5ae73b333815b0eb3dce"
 dependencies = [
  "autocfg",
  "bitflags 1.3.2",
@@ -4217,30 +6068,85 @@
  "libc",
  "log",
  "pin-project-lite",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "polling"
+version = "3.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24f040dee2588b4963afb4e420540439d126f73fdacf4a9c486a96d840bac3c9"
+dependencies = [
+ "cfg-if 1.0.0",
+ "concurrent-queue",
+ "pin-project-lite",
+ "rustix 0.38.32",
+ "tracing",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
+name = "pollster"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "22686f4785f02a4fcc856d3b3bb19bf6c8160d103f7a99cc258bddd0251dc7f2"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "presser"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e8cf8e6a8aa66ce33f63993ffc4ea4271eb5b0530a9002db8455ea6050c77bfa"
+
+[[package]]
 name = "prettyplease"
 version = "0.1.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8646e95016a7a6c4adea95bafa8a16baab64b583356217f2c85db4a39d9a86"
 dependencies = [
  "proc-macro2",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "prettyplease"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8d3928fb5db768cb86f891ff014f0144589297e3c6a1aba6ed7cecfdace270c7"
+dependencies = [
+ "proc-macro2",
+ "syn 2.0.48",
+]
+
+[[package]]
+name = "proc-macro-crate"
+version = "1.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
+dependencies = [
+ "once_cell",
+ "toml_edit 0.19.15",
+]
+
+[[package]]
+name = "proc-macro-crate"
+version = "3.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
+dependencies = [
+ "toml_edit 0.21.1",
+]
+
+[[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
@@ -4272,14 +6178,34 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "profiling"
+version = "1.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43d84d1d7a6ac92673717f9f6d1518374ef257669c24ebc5ac25d5033828be58"
+dependencies = [
+ "profiling-procmacros",
+ "puffin",
+]
+
+[[package]]
+name = "profiling-procmacros"
+version = "1.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8021cf59c8ec9c432cfc2526ac6b8aa508ecaf29cd415f271b8406c1b851c3fd"
+dependencies = [
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
 name = "prost"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d0f5d036824e4761737860779c906171497f6d55681139d8312388f8fe398922"
 dependencies = [
  "bytes",
  "prost-derive",
@@ -4288,21 +6214,72 @@
 [[package]]
 name = "prost-derive"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19de2de2a00075bf566bee3bd4db014b11587e84184d3f7a791bc17f1a8e9e48"
 dependencies = [
  "anyhow",
- "itertools 0.11.0",
+ "itertools 0.12.1",
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
+name = "puffin"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9f76ad4bb049fded4e572df72cbb6381ff5d1f41f85c3a04b56e4eca287a02f"
+dependencies = [
+ "anyhow",
+ "bincode",
+ "byteorder",
+ "cfg-if 1.0.0",
+ "lz4_flex",
+ "once_cell",
+ "parking_lot",
+ "serde",
+]
+
+[[package]]
+name = "puffin_http"
+version = "0.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4936c085e48efc86f6d96609dc5086d1d236afe3ec4676f09b157a4f4be83ff6"
+dependencies = [
+ "anyhow",
+ "crossbeam-channel",
+ "log",
+ "parking_lot",
+ "puffin",
+]
+
+[[package]]
+name = "pulldown-cmark"
+version = "0.9.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57206b407293d2bcd3af849ce869d52068623f19e1b5ff8e8778e3309439682b"
+dependencies = [
+ "bitflags 2.4.0",
+ "memchr",
+ "unicase",
+]
+
+[[package]]
+name = "pulldown-cmark"
+version = "0.10.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5f0530d13d87d1f549b66a3e8d0c688952abe5994e204ed62615baaf25dc029c"
+dependencies = [
+ "bitflags 2.4.0",
+ "memchr",
+ "unicase",
+]
+
+[[package]]
 name = "pyo3"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04e8453b658fe480c3e70c8ed4e3d3ec33eb74988bd186561b0cc66b85c3bc4b"
 dependencies = [
  "cfg-if 1.0.0",
  "eyre",
@@ -4377,14 +6354,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81b9228215d82c7b61490fec1de287136b5de6f5700f6e58ea9ad61a7964ca51"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "quick-xml"
+version = "0.31.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "quinn"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2e8b432585672228923edbbf64b8b12c14e1112f62e88737655b4a083dbcd78e"
 dependencies = [
  "bytes",
  "pin-project-lite",
@@ -4478,27 +6464,39 @@
 [[package]]
 name = "raw-window-handle"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2ff9a1f06a88b01621b7ae906ef0211290d1c8a168a15542486a8f61c0833b9"
 
 [[package]]
+name = "raw-window-handle"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42a9830a0e1b9fb145ebb365b8bc4ccd75f290f98c0247deafbbe2c75cefb544"
+
+[[package]]
 name = "raw_sync_2"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f067b45fa17e31d15636789c2638bd562da5496d498876cf0495df78f7e4fdcb"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
  "nix 0.23.2",
  "rand",
  "winapi 0.3.9",
 ]
 
 [[package]]
+name = "rawpointer"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
+
+[[package]]
 name = "rayon"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c27db03db7734835b3f53954b534c91069375ce6ccaa2e065441e07d9b6cdb1"
 dependencies = [
  "either",
  "rayon-core",
@@ -4511,14 +6509,1035 @@
 checksum = "5ce3fb6ad83f861aac485e76e1985cd109d9a3713802152be56c3b1f0e0658ed"
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "re_analytics"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "28ed083fc621e7e7d9b9a17dbb4986a5329a05ac1ff52692e77826820eac4de9"
+dependencies = [
+ "crossbeam",
+ "directories-next",
+ "ehttp",
+ "re_build_info",
+ "re_build_tools",
+ "re_log",
+ "serde",
+ "serde_json",
+ "sha2",
+ "thiserror",
+ "time",
+ "uuid",
+ "web-sys",
+]
+
+[[package]]
+name = "re_arrow2"
+version = "0.17.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c1285f33f03e2faf9f77b06c19f32f8c54792a4cbb19df762b9ea70b79e0773d"
+dependencies = [
+ "ahash",
+ "arrow-format",
+ "bytemuck",
+ "chrono",
+ "comfy-table",
+ "dyn-clone",
+ "either",
+ "ethnum",
+ "foreign_vec",
+ "getrandom",
+ "hash_hasher",
+ "hashbrown 0.14.3",
+ "num-traits",
+ "rustc_version",
+ "simdutf8",
+]
+
+[[package]]
+name = "re_build_info"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "147f2e79d9d8ef833666413adbc795403e250cfd8f29f41ede198a5a4dde8612"
+
+[[package]]
+name = "re_build_tools"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88dd6c26a72f68dd437dcbb462dc4fd5b6ab439f41f2dce2a12b95300266f725"
+dependencies = [
+ "anyhow",
+ "cargo_metadata 0.18.1",
+ "glob",
+ "sha2",
+ "time",
+ "unindent",
+ "walkdir",
+]
+
+[[package]]
+name = "re_crash_handler"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3feb098f6d9840f771f00b9c753f45eaa39687c5eac23549dbfe878a62c7d53d"
+dependencies = [
+ "backtrace",
+ "itertools 0.12.1",
+ "libc",
+ "parking_lot",
+ "re_analytics",
+ "re_build_info",
+]
+
+[[package]]
+name = "re_data_source"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa09ab2bd8dfb4d3a0c9541adf1ddf1eb880812a8d2e24875533bfce644db469"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "image",
+ "itertools 0.12.1",
+ "once_cell",
+ "parking_lot",
+ "rayon",
+ "re_build_tools",
+ "re_log",
+ "re_log_encoding",
+ "re_log_types",
+ "re_smart_channel",
+ "re_tracing",
+ "re_types",
+ "re_ws_comms",
+ "thiserror",
+ "walkdir",
+]
+
+[[package]]
+name = "re_data_store"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8faaee8c6f3c9aedf3b1b6c22050661861e41a8840f664d7685f6875667c9ba0"
+dependencies = [
+ "ahash",
+ "document-features",
+ "indent",
+ "itertools 0.12.1",
+ "nohash-hasher",
+ "once_cell",
+ "parking_lot",
+ "re_arrow2",
+ "re_error",
+ "re_format",
+ "re_log",
+ "re_log_types",
+ "re_tracing",
+ "re_types_core",
+ "smallvec",
+ "thiserror",
+ "web-time",
+]
+
+[[package]]
+name = "re_data_ui"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fde87a2c87ca648bdcce352cf086f7536679c53a7583f2d27c299363fbaf231"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "bytemuck",
+ "egui",
+ "egui_extras",
+ "egui_plot",
+ "image",
+ "itertools 0.12.1",
+ "re_data_store",
+ "re_entity_db",
+ "re_error",
+ "re_format",
+ "re_log",
+ "re_log_types",
+ "re_query",
+ "re_renderer",
+ "re_smart_channel",
+ "re_tracing",
+ "re_types",
+ "re_types_core",
+ "re_ui",
+ "re_viewer_context",
+ "rfd",
+]
+
+[[package]]
+name = "re_entity_db"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14f8d79b407fc1068f92994bcbf8681f1f6087547bf72ef6491f824a6965a0b2"
+dependencies = [
+ "ahash",
+ "document-features",
+ "emath",
+ "getrandom",
+ "itertools 0.12.1",
+ "nohash-hasher",
+ "parking_lot",
+ "re_data_store",
+ "re_format",
+ "re_int_histogram",
+ "re_log",
+ "re_log_encoding",
+ "re_log_types",
+ "re_query",
+ "re_query_cache",
+ "re_smart_channel",
+ "re_tracing",
+ "re_types_core",
+ "rmp-serde",
+ "serde",
+ "thiserror",
+ "web-time",
+]
+
+[[package]]
+name = "re_error"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a561ff5a4cdf5bc37c03f62fd78f618326c4cb0b10d2d7a062b33490bf9d630"
+
+[[package]]
+name = "re_format"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4405cf9203a791ff5e23bcbd54718635f9ec2323d48ea7d2c312adb6af756ca4"
+dependencies = [
+ "comfy-table",
+ "num-traits",
+ "re_arrow2",
+ "re_tuid",
+ "re_types_core",
+]
+
+[[package]]
+name = "re_int_histogram"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d422a395b4c0e0aed3acaca56a2b5681fc0a89d2a0d58323c2b940ae5944ac2f"
+dependencies = [
+ "smallvec",
+ "static_assertions",
+]
+
+[[package]]
+name = "re_log"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "35056426bb497a2bd30ec54f1aac35f32c6b0f2cd64fd833509ebb1e4be19f11"
+dependencies = [
+ "env_logger",
+ "js-sys",
+ "log",
+ "log-once",
+ "parking_lot",
+ "tracing",
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "re_log_encoding"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "10ff455e7e5e091cf8e43ce397c03ebad81357e3f45eab9a076674e7f2002618"
+dependencies = [
+ "ehttp",
+ "js-sys",
+ "lz4_flex",
+ "parking_lot",
+ "re_build_info",
+ "re_log",
+ "re_log_types",
+ "re_smart_channel",
+ "re_tracing",
+ "rmp-serde",
+ "thiserror",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "web-time",
+]
+
+[[package]]
+name = "re_log_types"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "239e3176efb51de961a8ea4d27af8b8076c37e40f8788b5a87e060fb806d7a29"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "backtrace",
+ "bytemuck",
+ "clean-path",
+ "crossbeam",
+ "document-features",
+ "fixed",
+ "half",
+ "itertools 0.12.1",
+ "natord",
+ "nohash-hasher",
+ "num-derive",
+ "num-traits",
+ "re_arrow2",
+ "re_format",
+ "re_log",
+ "re_string_interner",
+ "re_tracing",
+ "re_tuid",
+ "re_types_core",
+ "serde",
+ "serde_bytes",
+ "similar-asserts",
+ "smallvec",
+ "thiserror",
+ "time",
+ "typenum",
+ "uuid",
+ "web-time",
+]
+
+[[package]]
+name = "re_memory"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6812a6e08580fd7c6864eb018a8535093c23ab28cc4a607fe20b65b991dc1a36"
+dependencies = [
+ "ahash",
+ "backtrace",
+ "emath",
+ "itertools 0.12.1",
+ "memory-stats",
+ "nohash-hasher",
+ "once_cell",
+ "parking_lot",
+ "re_format",
+ "re_log",
+ "re_tracing",
+ "smallvec",
+ "sysinfo 0.30.11",
+ "wasm-bindgen",
+ "web-time",
+]
+
+[[package]]
+name = "re_query"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "64be284a20b1756e11702fbb6b9021ea9f291f6541dcf0def23dda8da803055c"
+dependencies = [
+ "backtrace",
+ "document-features",
+ "itertools 0.12.1",
+ "re_arrow2",
+ "re_data_store",
+ "re_format",
+ "re_log",
+ "re_log_types",
+ "re_tracing",
+ "re_types_core",
+ "serde",
+ "smallvec",
+ "thiserror",
+]
+
+[[package]]
+name = "re_query_cache"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cc2e00e32ea25bd8cc8393a184b5c0b135fac7cf86aad131d818f5973dd0ccbf"
+dependencies = [
+ "ahash",
+ "indent",
+ "itertools 0.12.1",
+ "parking_lot",
+ "paste",
+ "re_data_store",
+ "re_format",
+ "re_log",
+ "re_log_types",
+ "re_query",
+ "re_tracing",
+ "re_types_core",
+ "seq-macro",
+ "web-time",
+]
+
+[[package]]
+name = "re_renderer"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2902018a22e9cb535737582bc2c26e8e4939d0b24a5cd404c61919739e1f6d61"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "bitflags 2.4.0",
+ "bytemuck",
+ "cfg-if 1.0.0",
+ "cfg_aliases 0.2.0",
+ "clean-path",
+ "crossbeam",
+ "document-features",
+ "ecolor",
+ "enumset",
+ "getrandom",
+ "glam",
+ "gltf",
+ "half",
+ "itertools 0.12.1",
+ "macaw",
+ "never",
+ "notify 6.1.1",
+ "ordered-float 4.2.0",
+ "parking_lot",
+ "pathdiff",
+ "profiling",
+ "re_arrow2",
+ "re_build_tools",
+ "re_error",
+ "re_log",
+ "re_tracing",
+ "serde",
+ "slotmap",
+ "smallvec",
+ "static_assertions",
+ "thiserror",
+ "tinystl",
+ "tobj",
+ "type-map",
+ "walkdir",
+ "wasm-bindgen-futures",
+ "wgpu",
+ "wgpu-core",
+]
+
+[[package]]
+name = "re_sdk"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "45192dc7062d954626534e46709c3998a9c0773ffc48fad16d0ab2cd0278a895"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "crossbeam",
+ "document-features",
+ "itertools 0.12.1",
+ "once_cell",
+ "parking_lot",
+ "re_build_info",
+ "re_build_tools",
+ "re_data_source",
+ "re_log",
+ "re_log_encoding",
+ "re_log_types",
+ "re_memory",
+ "re_sdk_comms",
+ "re_smart_channel",
+ "re_types_core",
+ "re_web_viewer_server",
+ "re_ws_comms",
+ "thiserror",
+ "webbrowser",
+]
+
+[[package]]
+name = "re_sdk_comms"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3fe674910694817af5ff3efc4b36f19c7ce9e01f797e9d53b450e094eef3067a"
+dependencies = [
+ "ahash",
+ "crossbeam",
+ "document-features",
+ "rand",
+ "re_log",
+ "re_log_encoding",
+ "re_log_types",
+ "re_smart_channel",
+ "thiserror",
+ "tokio",
+]
+
+[[package]]
+name = "re_smart_channel"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "473934eb487c8f439cbde1e565c7a57e5a37909092c93d6a100efa1a8d52f5d6"
+dependencies = [
+ "crossbeam",
+ "parking_lot",
+ "re_tracing",
+ "serde",
+ "web-time",
+]
+
+[[package]]
+name = "re_space_view"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88a75158bba7b189228da2ca2c6801a74c42290a0120af78b93ec30035edafb3"
+dependencies = [
+ "ahash",
+ "egui",
+ "itertools 0.12.1",
+ "nohash-hasher",
+ "re_data_store",
+ "re_entity_db",
+ "re_log",
+ "re_log_types",
+ "re_query",
+ "re_tracing",
+ "re_types",
+ "re_types_core",
+ "re_viewer_context",
+ "slotmap",
+ "smallvec",
+]
+
+[[package]]
+name = "re_space_view_bar_chart"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ff7920522519199c365b5e049fe46c6dde0c4c1b356318239c0409c00e04495"
+dependencies = [
+ "egui",
+ "egui_plot",
+ "re_data_store",
+ "re_entity_db",
+ "re_log",
+ "re_log_types",
+ "re_renderer",
+ "re_space_view",
+ "re_tracing",
+ "re_types",
+ "re_ui",
+ "re_viewer_context",
+]
+
+[[package]]
+name = "re_space_view_dataframe"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4c09039219aae6bc2c6a1cb9e98c36f59858006ee639501b5c190f9e9d7fe7b"
+dependencies = [
+ "egui",
+ "egui_extras",
+ "re_data_store",
+ "re_data_ui",
+ "re_entity_db",
+ "re_log_types",
+ "re_query",
+ "re_renderer",
+ "re_tracing",
+ "re_types",
+ "re_ui",
+ "re_viewer_context",
+]
+
+[[package]]
+name = "re_space_view_spatial"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee0c742b6de79ca773bed2aa9255c2f0cad0a4b43181fed025d43e52a5885b73"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "bitflags 2.4.0",
+ "bytemuck",
+ "egui",
+ "glam",
+ "itertools 0.12.1",
+ "macaw",
+ "nohash-hasher",
+ "once_cell",
+ "parking_lot",
+ "rayon",
+ "re_data_store",
+ "re_data_ui",
+ "re_entity_db",
+ "re_error",
+ "re_format",
+ "re_log",
+ "re_log_types",
+ "re_query",
+ "re_query_cache",
+ "re_renderer",
+ "re_space_view",
+ "re_tracing",
+ "re_types",
+ "re_ui",
+ "re_viewer_context",
+ "serde",
+ "smallvec",
+ "web-time",
+]
+
+[[package]]
+name = "re_space_view_tensor"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "48ad9ea32a7ba75fa07ce1346450ce78dbe8b855086dd248d13d44f5cdfa24fc"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "bytemuck",
+ "egui",
+ "half",
+ "ndarray",
+ "re_data_store",
+ "re_data_ui",
+ "re_entity_db",
+ "re_log",
+ "re_log_types",
+ "re_renderer",
+ "re_space_view",
+ "re_tracing",
+ "re_types",
+ "re_ui",
+ "re_viewer_context",
+ "serde",
+ "thiserror",
+ "wgpu",
+]
+
+[[package]]
+name = "re_space_view_text_document"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ea29a1471fccfb28c79bf5b745655c0c3b0b14285a20dd61f29812ee54914cb0"
+dependencies = [
+ "egui",
+ "egui_commonmark",
+ "itertools 0.12.1",
+ "re_data_store",
+ "re_log",
+ "re_query",
+ "re_renderer",
+ "re_space_view",
+ "re_tracing",
+ "re_types",
+ "re_ui",
+ "re_viewer_context",
+]
+
+[[package]]
+name = "re_space_view_text_log"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60b72e7a3ec29386a91336cf60859d9668dad072ef4b14317dbf3c0bf86aec53"
+dependencies = [
+ "egui",
+ "egui_extras",
+ "itertools 0.12.1",
+ "re_data_store",
+ "re_data_ui",
+ "re_entity_db",
+ "re_log",
+ "re_log_types",
+ "re_query_cache",
+ "re_renderer",
+ "re_tracing",
+ "re_types",
+ "re_ui",
+ "re_viewer_context",
+]
+
+[[package]]
+name = "re_space_view_time_series"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c8d5194c716fed198893a3712afd4b71c05e914e9b26b9e2a54ed031b4467502"
+dependencies = [
+ "egui",
+ "egui_plot",
+ "itertools 0.12.1",
+ "parking_lot",
+ "rayon",
+ "re_data_store",
+ "re_format",
+ "re_log",
+ "re_log_types",
+ "re_query",
+ "re_query_cache",
+ "re_renderer",
+ "re_space_view",
+ "re_tracing",
+ "re_types",
+ "re_ui",
+ "re_viewer_context",
+]
+
+[[package]]
+name = "re_string_interner"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fbaf2000f39f12a01789ab13f5515028784e62be80006f9a3bdc92283ba9eff4"
+dependencies = [
+ "ahash",
+ "nohash-hasher",
+ "once_cell",
+ "parking_lot",
+ "serde",
+ "static_assertions",
+]
+
+[[package]]
+name = "re_time_panel"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a9a4e9831bc379ba8e9cc07987fe63a25100eea2f918f0f4da65d485631809c"
+dependencies = [
+ "egui",
+ "itertools 0.12.1",
+ "re_data_store",
+ "re_data_ui",
+ "re_entity_db",
+ "re_format",
+ "re_log_types",
+ "re_tracing",
+ "re_ui",
+ "re_viewer_context",
+ "re_viewport",
+ "serde",
+ "vec1",
+]
+
+[[package]]
+name = "re_tracing"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "61ca94b1087b377bde7e109c969b381c38d9a5a93a8265635a18aa3b341a5250"
+dependencies = [
+ "puffin",
+ "puffin_http",
+ "re_log",
+ "rfd",
+]
+
+[[package]]
+name = "re_tuid"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f82367ff940f00195fc6cc868d5e9cbec26ae1a3b7de6fa4b1c37457a42e93b5"
+dependencies = [
+ "document-features",
+ "getrandom",
+ "once_cell",
+ "serde",
+ "web-time",
+]
+
+[[package]]
+name = "re_types"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6acfd68909dd9720a2f9542ef0f660a33b3e7afd11c46c35f7e10101679d378e"
+dependencies = [
+ "anyhow",
+ "array-init",
+ "bytemuck",
+ "document-features",
+ "ecolor",
+ "egui_plot",
+ "glam",
+ "half",
+ "image",
+ "infer",
+ "itertools 0.12.1",
+ "linked-hash-map",
+ "mime_guess2",
+ "ndarray",
+ "nohash-hasher",
+ "once_cell",
+ "ply-rs",
+ "rayon",
+ "re_arrow2",
+ "re_build_tools",
+ "re_log",
+ "re_tracing",
+ "re_types_builder",
+ "re_types_core",
+ "smallvec",
+ "thiserror",
+ "uuid",
+ "zune-core",
+ "zune-jpeg",
+]
+
+[[package]]
+name = "re_types_builder"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe6bf1bb44be7f5ebed2d3f8bb46c67669d7ecbe52731ab0edd16cc2db3f02f2"
+dependencies = [
+ "anyhow",
+ "camino",
+ "clang-format",
+ "convert_case",
+ "flatbuffers",
+ "indent",
+ "itertools 0.12.1",
+ "prettyplease 0.2.17",
+ "proc-macro2",
+ "quote",
+ "rayon",
+ "re_arrow2",
+ "re_build_tools",
+ "re_log",
+ "re_tracing",
+ "rust-format",
+ "syn 2.0.48",
+ "tempfile",
+ "unindent",
+ "xshell",
+]
+
+[[package]]
+name = "re_types_core"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49a3d0143e33bd1d91ff8754511dbd1f038e4fa7bdc3fca0ac0f8619c0f778d3"
+dependencies = [
+ "anyhow",
+ "backtrace",
+ "bytemuck",
+ "document-features",
+ "once_cell",
+ "re_arrow2",
+ "re_error",
+ "re_string_interner",
+ "re_tracing",
+ "re_tuid",
+ "serde",
+ "smallvec",
+ "thiserror",
+]
+
+[[package]]
+name = "re_ui"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50017df0dca14a4995a71397db0a4f2e9a4a1118aee4e79c14beabdb92413cc6"
+dependencies = [
+ "egui",
+ "egui_commonmark",
+ "egui_extras",
+ "parking_lot",
+ "re_entity_db",
+ "re_format",
+ "re_log_types",
+ "serde",
+ "serde_json",
+ "strum 0.25.0",
+ "strum_macros 0.25.3",
+ "sublime_fuzzy",
+]
+
+[[package]]
+name = "re_viewer"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6770f90562ef536eecb5cf9490c2fe125c813b7e58c816afaf3c9b026fcb80e8"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "bytemuck",
+ "cfg-if 1.0.0",
+ "eframe",
+ "egui",
+ "egui-wgpu",
+ "egui_extras",
+ "egui_plot",
+ "egui_tiles",
+ "ehttp",
+ "image",
+ "itertools 0.12.1",
+ "js-sys",
+ "once_cell",
+ "poll-promise",
+ "re_analytics",
+ "re_build_info",
+ "re_build_tools",
+ "re_data_source",
+ "re_data_store",
+ "re_data_ui",
+ "re_entity_db",
+ "re_error",
+ "re_format",
+ "re_log",
+ "re_log_encoding",
+ "re_log_types",
+ "re_memory",
+ "re_query_cache",
+ "re_renderer",
+ "re_smart_channel",
+ "re_space_view",
+ "re_space_view_bar_chart",
+ "re_space_view_dataframe",
+ "re_space_view_spatial",
+ "re_space_view_tensor",
+ "re_space_view_text_document",
+ "re_space_view_text_log",
+ "re_space_view_time_series",
+ "re_time_panel",
+ "re_tracing",
+ "re_types",
+ "re_types_core",
+ "re_ui",
+ "re_viewer_context",
+ "re_viewport",
+ "re_ws_comms",
+ "rfd",
+ "ron",
+ "serde",
+ "serde_json",
+ "thiserror",
+ "time",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "web-time",
+ "wgpu",
+]
+
+[[package]]
+name = "re_viewer_context"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2de3a41feea776f865e3315f7422298a7299d5ac59068fbc5018fc9dd2865b8"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "arboard",
+ "bit-vec",
+ "bytemuck",
+ "egui",
+ "egui-wgpu",
+ "egui_tiles",
+ "glam",
+ "half",
+ "indexmap 2.2.6",
+ "itertools 0.12.1",
+ "macaw",
+ "ndarray",
+ "nohash-hasher",
+ "once_cell",
+ "parking_lot",
+ "re_data_source",
+ "re_data_store",
+ "re_entity_db",
+ "re_log",
+ "re_log_types",
+ "re_query",
+ "re_query_cache",
+ "re_renderer",
+ "re_smart_channel",
+ "re_string_interner",
+ "re_tracing",
+ "re_types",
+ "re_ui",
+ "serde",
+ "slotmap",
+ "smallvec",
+ "thiserror",
+ "uuid",
+ "wgpu",
+]
+
+[[package]]
+name = "re_viewport"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cc8b3fd1a6eefa041a7dec6a2556f6f9a60c47107e4a3297b9ebb7fa9ae1943"
+dependencies = [
+ "ahash",
+ "array-init",
+ "bytemuck",
+ "egui",
+ "egui_tiles",
+ "glam",
+ "image",
+ "itertools 0.12.1",
+ "nohash-hasher",
+ "once_cell",
+ "rayon",
+ "re_arrow2",
+ "re_data_store",
+ "re_data_ui",
+ "re_entity_db",
+ "re_log",
+ "re_log_types",
+ "re_query",
+ "re_renderer",
+ "re_smart_channel",
+ "re_space_view",
+ "re_space_view_time_series",
+ "re_tracing",
+ "re_types",
+ "re_types_core",
+ "re_ui",
+ "re_viewer_context",
+ "rmp-serde",
+ "smallvec",
+]
+
+[[package]]
+name = "re_web_viewer_server"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a9d11fe92ba3e159b2c4fe3640973d00cf8143ffb8d010078068a16b58a0c48b"
+dependencies = [
+ "clap 4.4.6",
+ "document-features",
+ "futures-util",
+ "hyper",
+ "re_analytics",
+ "re_log",
+ "thiserror",
+ "tokio",
+ "webbrowser",
+]
+
+[[package]]
+name = "re_ws_comms"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2fcd476b838119c1c57973c7df3b379cc6e74e9b97a72cf9bb4488170b95d20"
+dependencies = [
+ "anyhow",
+ "bincode",
+ "document-features",
+ "ewebsock",
+ "futures-channel",
+ "futures-util",
+ "parking_lot",
+ "re_format",
+ "re_log",
+ "re_log_types",
+ "re_memory",
+ "re_smart_channel",
+ "re_tracing",
+ "thiserror",
+ "tokio",
+ "tokio-tungstenite",
+ "tungstenite 0.20.1",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags 1.3.2",
 ]
@@ -4529,14 +7548,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+dependencies = [
+ "bitflags 1.3.2",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
  "getrandom",
  "redox_syscall 0.2.16",
@@ -4601,26 +7629,32 @@
 [[package]]
 name = "regex-syntax"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
+name = "renderdoc-sys"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b30a45b0cd0bcca8037f3d0dc3421eaf95327a17cad11964fb8179b4fc4832"
+
+[[package]]
 name = "reqwest"
 version = "0.11.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "046cd98826c46c2ac8ddecae268eb5c2e58628688a5fc7a2643704a73faba95b"
 dependencies = [
  "base64 0.21.4",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
- "http",
+ "http 0.2.9",
  "http-body",
  "hyper",
  "hyper-rustls",
  "ipnet",
  "js-sys",
  "log",
  "mime",
@@ -4641,14 +7675,70 @@
  "wasm-bindgen-futures",
  "web-sys",
  "webpki-roots 0.25.3",
  "winreg",
 ]
 
 [[package]]
+name = "rerun"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6978682653fc699d484b92d0ee75e25b73fdf9b0e50d62b67707d6bcd7f4cc96"
+dependencies = [
+ "anyhow",
+ "document-features",
+ "env_logger",
+ "itertools 0.12.1",
+ "log",
+ "puffin",
+ "rayon",
+ "re_analytics",
+ "re_build_info",
+ "re_build_tools",
+ "re_crash_handler",
+ "re_entity_db",
+ "re_format",
+ "re_log",
+ "re_log_types",
+ "re_memory",
+ "re_sdk",
+ "re_sdk_comms",
+ "re_smart_channel",
+ "re_tracing",
+ "re_types",
+ "re_viewer",
+ "re_web_viewer_server",
+]
+
+[[package]]
+name = "rfd"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c9e7b57df6e8472152674607f6cc68aa14a748a3157a857a94f516e11aeacc2"
+dependencies = [
+ "ashpd",
+ "async-io 1.13.0",
+ "block",
+ "dispatch",
+ "futures-util",
+ "js-sys",
+ "log",
+ "objc",
+ "objc-foundation",
+ "objc_id",
+ "pollster",
+ "raw-window-handle 0.5.2",
+ "urlencoding",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "rgb"
 version = "0.8.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "20ec2d3e3fc7a92ced357df9cebd5a10b6fb2aa1ee797bf7e9ce2f17dffc8f59"
 dependencies = [
  "bytemuck",
 ]
@@ -4689,27 +7779,63 @@
 checksum = "2fd1938faa63a2362ee1747afb2d10567d0fb1413b9cbd6198a8541485c4f773"
 dependencies = [
  "array-init",
  "cache-padded",
 ]
 
 [[package]]
+name = "rmp"
+version = "0.8.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "228ed7c16fa39782c3b3468e974aec2795e9089153cd08ee2e9aefb3613334c4"
+dependencies = [
+ "byteorder",
+ "num-traits",
+ "paste",
+]
+
+[[package]]
+name = "rmp-serde"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "938a142ab806f18b88a97b0dea523d39e0fd730a064b035726adcfc58a8a5188"
+dependencies = [
+ "byteorder",
+ "rmp",
+ "serde",
+]
+
+[[package]]
+name = "ron"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b91f7eff05f748767f183df4320a63d6936e9c6107d97c9e6bdd9784f4289c94"
+dependencies = [
+ "base64 0.21.4",
+ "bitflags 2.4.0",
+ "serde",
+ "serde_derive",
+]
+
+[[package]]
 name = "ros2-client"
-version = "0.6.1"
-source = "git+https://github.com/dora-rs/ros2-client.git?branch=deserialize-seed-2#23cbcc8557011cf3e89f95bab4fe02a40c5dac74"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f9bee0c156d235d3d52d217d29b628e56dd8a0be5308acb1925a7d76835ee5bb"
 dependencies = [
  "async-channel 2.1.1",
- "bstr",
+ "bstr 1.6.2",
  "bytes",
  "cdr-encoding-size",
  "chrono",
  "clap 4.4.6",
  "futures",
  "itertools 0.11.0",
  "lazy_static",
+ "libc",
  "log",
  "mio 0.6.23",
  "mio-extras",
  "nom",
  "pin-utils",
  "rustdds",
  "serde",
@@ -4737,64 +7863,75 @@
  "smallvec",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rust-dataflow-example-node"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
-name = "rust-dataflow-example-operator"
-version = "0.3.3-rc1"
+name = "rust-dataflow-example-sink"
+version = "0.3.4-rc2"
 dependencies = [
- "dora-operator-api",
+ "dora-node-api",
+ "eyre",
 ]
 
 [[package]]
-name = "rust-dataflow-example-sink"
-version = "0.3.3-rc1"
+name = "rust-dataflow-example-status-node"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "rust-format"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60e7c00b6c3bf5e38a880eec01d7e829d12ca682079f8238a464def3c4b31627"
 dependencies = [
- "prettyplease",
+ "prettyplease 0.1.25",
  "proc-macro2",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "rust-ros2-dataflow-example-node"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "dora-ros2-bridge",
  "eyre",
  "futures",
  "futures-timer",
  "rand",
  "serde_json",
  "tokio",
 ]
 
 [[package]]
+name = "rust_decimal"
+version = "1.35.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1790d1c4c0ca81211399e0e0af16333276f375209e71a37b67698a373db5b47a"
+dependencies = [
+ "arrayvec",
+ "num-traits",
+]
+
+[[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustc-hash"
@@ -4809,16 +7946,17 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustdds"
-version = "0.9.0"
-source = "git+https://github.com/dora-rs/RustDDS.git?branch=deserialize-seed-2#fae9fcfb582c4842b849268b3466875daf62fb7f"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f2fc6a62fccbe521b5de1bb40c06f4a9b8844337eb218c94577b40c5bae5f584"
 dependencies = [
  "bit-vec",
  "byteorder",
  "bytes",
  "cdr-encoding-size",
  "chrono",
  "enumflags2",
@@ -4856,17 +7994,17 @@
  "libc",
  "linux-raw-sys 0.3.8",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.28"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72e572a5e8ca657d7366229cdde4bd14c4eb5499a9573d4d366fe1b599daa316"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
  "bitflags 2.4.0",
  "errno",
  "libc",
  "linux-raw-sys 0.4.12",
  "windows-sys 0.52.0",
 ]
@@ -4887,19 +8025,33 @@
 name = "rustls"
 version = "0.21.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
 dependencies = [
  "log",
  "ring 0.17.7",
- "rustls-webpki",
+ "rustls-webpki 0.101.7",
  "sct",
 ]
 
 [[package]]
+name = "rustls"
+version = "0.22.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
+dependencies = [
+ "log",
+ "ring 0.17.7",
+ "rustls-pki-types",
+ "rustls-webpki 0.102.2",
+ "subtle",
+ "zeroize",
+]
+
+[[package]]
 name = "rustls-native-certs"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9aace74cb666635c918e9c12bc0d348266037aa8eb599b5cba565709a8dff00"
 dependencies = [
  "openssl-probe",
  "rustls-pemfile",
@@ -4913,24 +8065,41 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d3987094b1d07b653b7dfdc3f70ce9a1da9c51ac18c1b06b662e4f9a0e9f4b2"
 dependencies = [
  "base64 0.21.4",
 ]
 
 [[package]]
+name = "rustls-pki-types"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+
+[[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
  "ring 0.17.7",
  "untrusted 0.9.0",
 ]
 
 [[package]]
+name = "rustls-webpki"
+version = "0.102.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+dependencies = [
+ "ring 0.17.7",
+ "rustls-pki-types",
+ "untrusted 0.9.0",
+]
+
+[[package]]
 name = "rustversion"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
@@ -4965,15 +8134,15 @@
 [[package]]
 name = "safer_ffi-proc_macros"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf04ebd3786110e64269a74eea58c5564dd92a1e790c0f6f9871d6fe1b8e34db"
 dependencies = [
  "macro_rules_attribute",
- "prettyplease",
+ "prettyplease 0.1.25",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "same-file"
@@ -4990,14 +8159,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "scoped-tls"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1cf6437eb19a8f4a6cc0f7dca544973b0b78843adbfeb3683d1a94a0024a294"
+
+[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "scratch"
@@ -5039,14 +8214,17 @@
 ]
 
 [[package]]
 name = "semver"
 version = "1.0.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad977052201c6de01a8ef2aa3378c4bd23217a056337d1d6da40468d267a4fb0"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
@@ -5084,14 +8262,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92b7be0ad5a7b2eefaa5418eb141838270f1ad2d2c6e88acec3795d2425ffa97"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "serde_bytes"
+version = "0.11.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b8497c313fd43ab992087548117643f6fcd935cbf36f176ffda0aacf9591734"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "serde_derive"
 version = "1.0.195"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46fe8f8603d81ba86327b23a2e9cdf49e1255fb94a4c5f297f6ee0547178ea2c"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -5146,22 +8333,33 @@
 
 [[package]]
 name = "serde_yaml"
 version = "0.9.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1bf28c79a99f70ee1f1d83d10c875d2e70618417fda01ad1785e027579d9d38"
 dependencies = [
- "indexmap 2.0.2",
+ "indexmap 2.2.6",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
+name = "sha1"
+version = "0.10.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
+dependencies = [
+ "cfg-if 1.0.0",
+ "cpufeatures",
+ "digest",
+]
+
+[[package]]
 name = "sha2"
 version = "0.10.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "793db75ad2bcafc3ffa7c68b215fee268f537982cd901d132f89c6343f3a3dc8"
 dependencies = [
  "cfg-if 1.0.0",
  "cpufeatures",
@@ -5185,15 +8383,15 @@
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "shared-memory-server"
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 dependencies = [
  "bincode",
  "eyre",
  "raw_sync_2",
  "serde",
  "shared_memory_extended",
  "tracing",
@@ -5279,27 +8477,132 @@
 checksum = "74233d3b3b2f6d4b006dc19dee745e73e2a6bfb6f93607cd3b02bd5b00797d7c"
 dependencies = [
  "digest",
  "rand_core",
 ]
 
 [[package]]
+name = "simd-adler32"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d66dc143e6b11c1eddc06d5c423cfc97062865baf299914ab64caa38182078fe"
+
+[[package]]
+name = "simdutf8"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
+
+[[package]]
+name = "similar"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fa42c91313f1d05da9b26f267f931cf178d4aba455b4c4622dd7355eb80c6640"
+dependencies = [
+ "bstr 0.2.17",
+ "unicode-segmentation",
+]
+
+[[package]]
+name = "similar-asserts"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e041bb827d1bfca18f213411d51b665309f1afb37a04a5d1464530e13779fc0f"
+dependencies = [
+ "console",
+ "similar",
+]
+
+[[package]]
+name = "skeptic"
+version = "0.13.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "16d23b015676c90a0f01c197bfdc786c20342c73a0afdda9025adb0bc42940a8"
+dependencies = [
+ "bytecount",
+ "cargo_metadata 0.14.2",
+ "error-chain",
+ "glob",
+ "pulldown-cmark 0.9.6",
+ "tempfile",
+ "walkdir",
+]
+
+[[package]]
 name = "slab"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "slotmap"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dbff4acf519f630b3a3ddcfaea6c06b42174d9a44bc70c620e9ed1649d58b82a"
+dependencies = [
+ "serde",
+ "version_check",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "942b4a808e05215192e39f4ab80813e599068285906cc91aa64f923db842bd5a"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "smithay-client-toolkit"
+version = "0.18.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "922fd3eeab3bd820d76537ce8f582b1cf951eceb5475c28500c7457d9d17f53a"
+dependencies = [
+ "bitflags 2.4.0",
+ "calloop",
+ "calloop-wayland-source",
+ "cursor-icon",
+ "libc",
+ "log",
+ "memmap2",
+ "rustix 0.38.32",
+ "thiserror",
+ "wayland-backend",
+ "wayland-client",
+ "wayland-csd-frame",
+ "wayland-cursor",
+ "wayland-protocols",
+ "wayland-protocols-wlr",
+ "wayland-scanner",
+ "xkeysym",
+]
+
+[[package]]
+name = "smithay-clipboard"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c091e7354ea8059d6ad99eace06dd13ddeedbb0ac72d40a9a6e7ff790525882d"
+dependencies = [
+ "libc",
+ "smithay-client-toolkit",
+ "wayland-backend",
+]
+
+[[package]]
+name = "smol_str"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6845563ada680337a52d43bb0b29f396f2d911616f6573012645b9e3d048a49"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "snap"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b6b67fb9a61334225b5b790716f609cd58395f895b3fe8b328786812a40bc3b"
 
@@ -5327,15 +8630,15 @@
 name = "socketpair"
 version = "0.19.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a004c141c54615778c01a6722f6453fae7013e501b2b1f2dfe5684037174721"
 dependencies = [
  "io-extras",
  "io-lifetimes 2.0.2",
- "rustix 0.38.28",
+ "rustix 0.38.32",
  "uuid",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "speedy"
 version = "0.8.6"
@@ -5369,14 +8672,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
+name = "spirv"
+version = "0.3.0+sdk-1.3.268.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eda41003dc44290527a59b13432d4a0379379fa074b70174882adfbdfd917844"
+dependencies = [
+ "bitflags 2.4.0",
+]
+
+[[package]]
 name = "spki"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67cf02bbac7a337dc36e4f5a693db6c21e7863f45070f7064577eb4367a3212b"
 dependencies = [
  "base64ct",
  "der",
@@ -5415,14 +8727,61 @@
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
+name = "strum"
+version = "0.25.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
+dependencies = [
+ "strum_macros 0.25.3",
+]
+
+[[package]]
+name = "strum"
+version = "0.26.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5d8cec3501a5194c432b2b7976db6b7d10ec95c253208b45f83f7136aa985e29"
+
+[[package]]
+name = "strum_macros"
+version = "0.25.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
+dependencies = [
+ "heck 0.4.1",
+ "proc-macro2",
+ "quote",
+ "rustversion",
+ "syn 2.0.48",
+]
+
+[[package]]
+name = "strum_macros"
+version = "0.26.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
+dependencies = [
+ "heck 0.4.1",
+ "proc-macro2",
+ "quote",
+ "rustversion",
+ "syn 2.0.48",
+]
+
+[[package]]
+name = "sublime_fuzzy"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fa7986063f7c0ab374407e586d7048a3d5aac94f103f751088bf398e07cd5400"
+
+[[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
@@ -5495,14 +8854,29 @@
  "ntapi",
  "once_cell",
  "rayon",
  "winapi 0.3.9",
 ]
 
 [[package]]
+name = "sysinfo"
+version = "0.30.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87341a165d73787554941cd5ef55ad728011566fe714e987d1b976c15dbc3a83"
+dependencies = [
+ "cfg-if 1.0.0",
+ "core-foundation-sys",
+ "libc",
+ "ntapi",
+ "once_cell",
+ "rayon",
+ "windows 0.52.0",
+]
+
+[[package]]
 name = "system-configuration"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
@@ -5528,52 +8902,64 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
+name = "tempfile"
+version = "3.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
+dependencies = [
+ "cfg-if 1.0.0",
+ "fastrand 2.0.1",
+ "rustix 0.38.32",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "termcolor"
-version = "1.3.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6093bad37da69aab9d123a8091e4be0aa4a03e4d601ec641c327398315f62b64"
+checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "terminal_size"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21bebf2b7c9e0a515f6e0f8c51dc0f8e4696391e6f1ff30379559f8365fb0df7"
 dependencies = [
- "rustix 0.38.28",
+ "rustix 0.38.32",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
-version = "1.0.49"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1177e8c6d7ede7afde3585fd2513e611227efd6481bd78d2e82ba1ce16557ed4"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.49"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10712f02019e9288794769fba95cd6847df9874d49d871d062172f9dd41bc4cc"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
@@ -5616,21 +9002,35 @@
 dependencies = [
  "byteorder",
  "integer-encoding",
  "ordered-float 2.10.1",
 ]
 
 [[package]]
+name = "tiff"
+version = "0.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba1310fcea54c6a9a4fd1aad794ecc02c31682f6bfbecdf460bf19533eed1e3e"
+dependencies = [
+ "flate2",
+ "jpeg-decoder",
+ "weezl",
+]
+
+[[package]]
 name = "time"
 version = "0.3.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "426f806f4089c493dcac0d24c29c01e2c38baf8e30f1b716ee37e83d200b18fe"
 dependencies = [
  "deranged",
  "itoa",
+ "js-sys",
+ "libc",
+ "num_threads",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
@@ -5653,14 +9053,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
+name = "tinystl"
+version = "0.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fdbcdda2f86a57b89b5d9ac17cd4c9f3917ec8edcde403badf3d992d2947af2a"
+dependencies = [
+ "bytemuck",
+]
+
+[[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
@@ -5668,14 +9077,23 @@
 [[package]]
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
+name = "tobj"
+version = "4.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3bd4ba05f29e4c65b6c0c11a58b6465ffa820bac890d76ad407b4e81d8372e8"
+dependencies = [
+ "ahash",
+]
+
+[[package]]
 name = "tokio"
 version = "1.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
 dependencies = [
  "backtrace",
  "bytes",
@@ -5729,40 +9147,80 @@
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
+name = "tokio-tungstenite"
+version = "0.20.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "212d5dcb2a1ce06d81107c3d0ffa3121fe974b73f068c8282cb1c32328113b6c"
+dependencies = [
+ "futures-util",
+ "log",
+ "tokio",
+ "tungstenite 0.20.1",
+]
+
+[[package]]
 name = "tokio-util"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d68074620f57a0b21594d9735eb2e98ab38b17f80d3fcb189fca266771ca60d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
+name = "toml_datetime"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
+
+[[package]]
+name = "toml_edit"
+version = "0.19.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b5bb770da30e5cbfde35a2d7b9b8a2c4b8ef89548a7a6aeab5c9a576e3e7421"
+dependencies = [
+ "indexmap 2.2.6",
+ "toml_datetime",
+ "winnow",
+]
+
+[[package]]
+name = "toml_edit"
+version = "0.21.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
+dependencies = [
+ "indexmap 2.2.6",
+ "toml_datetime",
+ "winnow",
+]
+
+[[package]]
 name = "tonic"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76c4eb7a4e9ef9d4763600161f12f5070b92a578e1b634db88a6887844c91a13"
 dependencies = [
  "async-stream",
  "async-trait",
  "axum",
  "base64 0.21.4",
  "bytes",
  "h2",
- "http",
+ "http 0.2.9",
  "http-body",
  "hyper",
  "hyper-timeout",
  "percent-encoding",
  "pin-project",
  "prost",
  "tokio",
@@ -5807,14 +9265,15 @@
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
+ "log",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
@@ -5883,36 +9342,100 @@
 [[package]]
 name = "try-lock"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
 
 [[package]]
+name = "ttf-parser"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "17f77d76d837a7830fe1d4f12b7b4ba4192c1888001c7164257e4bc6d21d96b4"
+
+[[package]]
+name = "tungstenite"
+version = "0.20.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e3dac10fd62eaf6617d3a904ae222845979aec67c615d1c842b4002c7666fb9"
+dependencies = [
+ "byteorder",
+ "bytes",
+ "data-encoding",
+ "http 0.2.9",
+ "httparse",
+ "log",
+ "rand",
+ "sha1",
+ "thiserror",
+ "url",
+ "utf-8",
+]
+
+[[package]]
+name = "tungstenite"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ef1a641ea34f399a848dea702823bbecfb4c486f911735368f1f137cb8257e1"
+dependencies = [
+ "byteorder",
+ "bytes",
+ "data-encoding",
+ "http 1.1.0",
+ "httparse",
+ "log",
+ "rand",
+ "sha1",
+ "thiserror",
+ "url",
+ "utf-8",
+]
+
+[[package]]
 name = "twox-hash"
 version = "1.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
 dependencies = [
  "cfg-if 1.0.0",
  "static_assertions",
 ]
 
 [[package]]
+name = "type-map"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "deb68604048ff8fa93347f02441e4487594adc20bb8a084f9e564d2b827a0a9f"
+dependencies = [
+ "rustc-hash",
+]
+
+[[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "ucd-trie"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed646292ffc8188ef8ea4d1e0e0150fb15a5c2e12ad9b8fc191ae7a8a7f3c4b9"
 
 [[package]]
+name = "uds_windows"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "89daebc3e6fd160ac4aa9fc8b3bf71e1f74fbf92367ae71fb83a037e8bf164b9"
+dependencies = [
+ "memoffset 0.9.0",
+ "tempfile",
+ "winapi 0.3.9",
+]
+
+[[package]]
 name = "uhlc"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d291a7454d390b753ef68df8145da18367e32883ec2fa863959f0aefb915cdb"
 dependencies = [
  "hex",
  "humantime",
@@ -5920,14 +9443,23 @@
  "log",
  "serde",
  "spin 0.9.8",
  "uuid",
 ]
 
 [[package]]
+name = "unicase"
+version = "2.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7d2d4dafb69621809a81864c9c1b864479e1235c0dd4e199924b9742439ed89"
+dependencies = [
+ "version_check",
+]
+
+[[package]]
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
@@ -5953,14 +9485,20 @@
 [[package]]
 name = "unicode-width"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
 
 [[package]]
+name = "unicode-xid"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
+
+[[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "uninit"
@@ -6003,31 +9541,55 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "ureq"
+version = "2.9.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "11f214ce18d8b2cbe84ed3aa6486ed3f5b285cf8d8fbdbce9f3f767a724adc35"
+dependencies = [
+ "base64 0.21.4",
+ "flate2",
+ "log",
+ "once_cell",
+ "rustls 0.22.4",
+ "rustls-pki-types",
+ "rustls-webpki 0.102.2",
+ "url",
+ "webpki-roots 0.26.1",
+]
+
+[[package]]
 name = "url"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
+ "serde",
 ]
 
 [[package]]
 name = "urlencoding"
 version = "2.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "daf8dba3b7eb870caf1ddeed7bc9d2a049f3cfdfae7cb521b087cc33ae4c49da"
 
 [[package]]
+name = "utf-8"
+version = "0.7.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09cc8ee72d2a9becf2f2febe0205bbed8fc6615b7cb429ad062dc7b7ddd036a9"
+
+[[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
@@ -6036,14 +9598,15 @@
 checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
 dependencies = [
  "atomic",
  "getrandom",
  "rand",
  "serde",
  "uuid-macro-internal",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "uuid-macro-internal"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7abb14ae1a50dad63eaa768a458ef43d298cd1bd44951677bd10b732a9ba2a2d"
@@ -6092,14 +9655,20 @@
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
+name = "vec1"
+version = "1.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ffb60dcfffc189bfd4e2a81333c268619fee9db53da71bce2bcbd8e129c56936"
+
+[[package]]
 name = "vec_map"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
 
 [[package]]
 name = "version_check"
@@ -6136,83 +9705,215 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if 1.0.0",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn 2.0.48",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.37"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if 1.0.0",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
+
+[[package]]
+name = "wasm-streams"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "b65dc4c90b63b118468cf747d8bf3566c1913ef60be765b5730ead9e0a3ba129"
+dependencies = [
+ "futures-util",
+ "js-sys",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+]
+
+[[package]]
+name = "wayland-backend"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d50fa61ce90d76474c87f5fc002828d81b32677340112b4ef08079a9d459a40"
+dependencies = [
+ "cc",
+ "downcast-rs",
+ "rustix 0.38.32",
+ "scoped-tls",
+ "smallvec",
+ "wayland-sys",
+]
+
+[[package]]
+name = "wayland-client"
+version = "0.31.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "82fb96ee935c2cea6668ccb470fb7771f6215d1691746c2d896b447a00ad3f1f"
+dependencies = [
+ "bitflags 2.4.0",
+ "rustix 0.38.32",
+ "wayland-backend",
+ "wayland-scanner",
+]
+
+[[package]]
+name = "wayland-csd-frame"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "625c5029dbd43d25e6aa9615e88b829a5cad13b2819c4ae129fdbb7c31ab4c7e"
+dependencies = [
+ "bitflags 2.4.0",
+ "cursor-icon",
+ "wayland-backend",
+]
+
+[[package]]
+name = "wayland-cursor"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "71ce5fa868dd13d11a0d04c5e2e65726d0897be8de247c0c5a65886e283231ba"
+dependencies = [
+ "rustix 0.38.32",
+ "wayland-client",
+ "xcursor",
+]
+
+[[package]]
+name = "wayland-protocols"
+version = "0.31.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f81f365b8b4a97f422ac0e8737c438024b5951734506b0e1d775c73030561f4"
+dependencies = [
+ "bitflags 2.4.0",
+ "wayland-backend",
+ "wayland-client",
+ "wayland-scanner",
+]
+
+[[package]]
+name = "wayland-protocols-plasma"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23803551115ff9ea9bce586860c5c5a971e360825a0309264102a9495a5ff479"
+dependencies = [
+ "bitflags 2.4.0",
+ "wayland-backend",
+ "wayland-client",
+ "wayland-protocols",
+ "wayland-scanner",
+]
+
+[[package]]
+name = "wayland-protocols-wlr"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad1f61b76b6c2d8742e10f9ba5c3737f6530b4c243132c2a2ccc8aa96fe25cd6"
+dependencies = [
+ "bitflags 2.4.0",
+ "wayland-backend",
+ "wayland-client",
+ "wayland-protocols",
+ "wayland-scanner",
+]
+
+[[package]]
+name = "wayland-scanner"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "63b3a62929287001986fb58c789dce9b67604a397c15c611ad9f747300b6c283"
+dependencies = [
+ "proc-macro2",
+ "quick-xml 0.31.0",
+ "quote",
+]
+
+[[package]]
+name = "wayland-sys"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "15a0c8eaff5216d07f226cb7a549159267f3467b289d9a2e52fd3ef5aae2b7af"
+dependencies = [
+ "dlib",
+ "log",
+ "once_cell",
+ "pkg-config",
+]
 
 [[package]]
 name = "web-sys"
-version = "0.3.64"
+version = "0.3.69"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "web-time"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
+checksum = "aa30049b1c872b72c89866d458eae9f20380ab280ffd1b1e18df2d3e2d98cfe0"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webbrowser"
@@ -6222,15 +9923,15 @@
 dependencies = [
  "core-foundation",
  "home",
  "jni",
  "log",
  "ndk-context",
  "objc",
- "raw-window-handle",
+ "raw-window-handle 0.5.2",
  "url",
  "web-sys",
 ]
 
 [[package]]
 name = "webpki"
 version = "0.22.2"
@@ -6253,23 +9954,142 @@
 [[package]]
 name = "webpki-roots"
 version = "0.25.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1778a42e8b3b90bff8d0f5032bf22250792889a5cdc752aa0020c84abe3aaf10"
 
 [[package]]
+name = "webpki-roots"
+version = "0.26.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
+dependencies = [
+ "rustls-pki-types",
+]
+
+[[package]]
+name = "weezl"
+version = "0.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53a85b86a771b1c87058196170769dd264f66c0782acf1ae6cc51bfd64b39082"
+
+[[package]]
+name = "wgpu"
+version = "0.19.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cbd7311dbd2abcfebaabf1841a2824ed7c8be443a0f29166e5d3c6a53a762c01"
+dependencies = [
+ "arrayvec",
+ "cfg-if 1.0.0",
+ "cfg_aliases 0.1.1",
+ "js-sys",
+ "log",
+ "naga",
+ "parking_lot",
+ "profiling",
+ "raw-window-handle 0.6.0",
+ "smallvec",
+ "static_assertions",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "wgpu-core",
+ "wgpu-hal",
+ "wgpu-types",
+]
+
+[[package]]
+name = "wgpu-core"
+version = "0.19.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "28b94525fc99ba9e5c9a9e24764f2bc29bad0911a7446c12f446a8277369bf3a"
+dependencies = [
+ "arrayvec",
+ "bit-vec",
+ "bitflags 2.4.0",
+ "cfg_aliases 0.1.1",
+ "codespan-reporting",
+ "indexmap 2.2.6",
+ "log",
+ "naga",
+ "once_cell",
+ "parking_lot",
+ "profiling",
+ "raw-window-handle 0.6.0",
+ "rustc-hash",
+ "smallvec",
+ "thiserror",
+ "web-sys",
+ "wgpu-hal",
+ "wgpu-types",
+]
+
+[[package]]
+name = "wgpu-hal"
+version = "0.19.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fc1a4924366df7ab41a5d8546d6534f1f33231aa5b3f72b9930e300f254e39c3"
+dependencies = [
+ "android_system_properties",
+ "arrayvec",
+ "ash",
+ "bitflags 2.4.0",
+ "block",
+ "cfg_aliases 0.1.1",
+ "core-graphics-types",
+ "glow",
+ "glutin_wgl_sys",
+ "gpu-alloc",
+ "gpu-allocator",
+ "gpu-descriptor",
+ "hassle-rs",
+ "js-sys",
+ "khronos-egl",
+ "libc",
+ "libloading 0.8.3",
+ "log",
+ "metal",
+ "naga",
+ "ndk-sys",
+ "objc",
+ "once_cell",
+ "parking_lot",
+ "profiling",
+ "raw-window-handle 0.6.0",
+ "renderdoc-sys",
+ "rustc-hash",
+ "smallvec",
+ "thiserror",
+ "wasm-bindgen",
+ "web-sys",
+ "wgpu-types",
+ "winapi 0.3.9",
+]
+
+[[package]]
+name = "wgpu-types"
+version = "0.19.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b671ff9fb03f78b46ff176494ee1ebe7d603393f42664be55b64dc8d53969805"
+dependencies = [
+ "bitflags 2.4.0",
+ "js-sys",
+ "web-sys",
+]
+
+[[package]]
 name = "which"
 version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9bf3ea8596f3a0dd5980b46430f2058dfe2c36a27ccfbb1845d6fbfcd9ba6e14"
 dependencies = [
  "either",
  "home",
  "once_cell",
- "rustix 0.38.28",
+ "rustix 0.38.32",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "widestring"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -6351,18 +10171,61 @@
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
+ "windows-implement",
+ "windows-interface",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "windows"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
+dependencies = [
+ "windows-core",
+ "windows-targets 0.52.0",
+]
+
+[[package]]
+name = "windows-core"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
+dependencies = [
+ "windows-targets 0.52.0",
+]
+
+[[package]]
+name = "windows-implement"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5e2ee588991b9e7e6c8338edf3333fbe4da35dc72092643958ebb43f0ab2c49c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "windows-interface"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6fb8df20c9bcaa8ad6ab513f7b40104840c8867d5751126e4df3b08388d0cc7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
  "windows_aarch64_gnullvm 0.42.2",
  "windows_aarch64_msvc 0.42.2",
@@ -6598,14 +10461,70 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
 
 [[package]]
+name = "winit"
+version = "0.29.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0d59ad965a635657faf09c8f062badd885748428933dad8e8bdd64064d92e5ca"
+dependencies = [
+ "ahash",
+ "android-activity",
+ "atomic-waker",
+ "bitflags 2.4.0",
+ "bytemuck",
+ "calloop",
+ "cfg_aliases 0.1.1",
+ "core-foundation",
+ "core-graphics",
+ "cursor-icon",
+ "icrate",
+ "js-sys",
+ "libc",
+ "log",
+ "memmap2",
+ "ndk",
+ "ndk-sys",
+ "objc2 0.4.1",
+ "once_cell",
+ "orbclient",
+ "percent-encoding",
+ "raw-window-handle 0.6.0",
+ "redox_syscall 0.3.5",
+ "rustix 0.38.32",
+ "smithay-client-toolkit",
+ "smol_str",
+ "unicode-segmentation",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "wayland-backend",
+ "wayland-client",
+ "wayland-protocols",
+ "wayland-protocols-plasma",
+ "web-sys",
+ "web-time",
+ "windows-sys 0.48.0",
+ "x11-dl",
+ "x11rb",
+ "xkbcommon-dl",
+]
+
+[[package]]
+name = "winnow"
+version = "0.5.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
  "cfg-if 1.0.0",
  "windows-sys 0.48.0",
@@ -6633,15 +10552,15 @@
 
 [[package]]
 name = "wrapcenum-derive"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bcc065c85ad2c3bd12aa4118bf164835712e25080c392557801a13292c60aec"
 dependencies = [
- "darling",
+ "darling 0.10.2",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "ws2_32-sys"
@@ -6659,23 +10578,177 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
+name = "x11-dl"
+version = "2.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38735924fedd5314a6e548792904ed8c6de6636285cb9fec04d5b1db85c1516f"
+dependencies = [
+ "libc",
+ "once_cell",
+ "pkg-config",
+]
+
+[[package]]
+name = "x11rb"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8f25ead8c7e4cba123243a6367da5d3990e0d3affa708ea19dce96356bd9f1a"
+dependencies = [
+ "as-raw-xcb-connection",
+ "gethostname",
+ "libc",
+ "libloading 0.8.3",
+ "once_cell",
+ "rustix 0.38.32",
+ "x11rb-protocol",
+]
+
+[[package]]
+name = "x11rb-protocol"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e63e71c4b8bd9ffec2c963173a4dc4cbde9ee96961d4fcb4429db9929b606c34"
+
+[[package]]
+name = "xcursor"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6a0ccd7b4a5345edfcd0c3535718a4e9ff7798ffc536bb5b5a0e26ff84732911"
+
+[[package]]
+name = "xdg-home"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "21e5a325c3cb8398ad6cf859c1135b25dd29e186679cf2da7581d9679f63b38e"
+dependencies = [
+ "libc",
+ "winapi 0.3.9",
+]
+
+[[package]]
+name = "xkbcommon-dl"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d039de8032a9a8856a6be89cea3e5d12fdd82306ab7c94d74e6deab2460651c5"
+dependencies = [
+ "bitflags 2.4.0",
+ "dlib",
+ "log",
+ "once_cell",
+ "xkeysym",
+]
+
+[[package]]
+name = "xkeysym"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "054a8e68b76250b253f671d1268cb7f1ae089ec35e195b2efb2a4e9a836d0621"
+
+[[package]]
+name = "xml-rs"
+version = "0.8.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "791978798f0597cfc70478424c2b4fdc2b7a8024aaff78497ef00f24ef674193"
+
+[[package]]
+name = "xshell"
+version = "0.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6db0ab86eae739efd1b054a8d3d16041914030ac4e01cd1dca0cf252fd8b6437"
+dependencies = [
+ "xshell-macros",
+]
+
+[[package]]
+name = "xshell-macros"
+version = "0.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d422e8e38ec76e2f06ee439ccc765e9c6a9638b9e7c9f2e8255e4d41e8bd852"
+
+[[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
 
 [[package]]
+name = "zbus"
+version = "3.15.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "675d170b632a6ad49804c8cf2105d7c31eddd3312555cffd4b740e08e97c25e6"
+dependencies = [
+ "async-broadcast",
+ "async-executor",
+ "async-fs 1.6.0",
+ "async-io 1.13.0",
+ "async-lock 2.8.0",
+ "async-process",
+ "async-recursion",
+ "async-task",
+ "async-trait",
+ "blocking",
+ "byteorder",
+ "derivative",
+ "enumflags2",
+ "event-listener 2.5.3",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "hex",
+ "nix 0.26.4",
+ "once_cell",
+ "ordered-stream",
+ "rand",
+ "serde",
+ "serde_repr",
+ "sha1",
+ "static_assertions",
+ "tracing",
+ "uds_windows",
+ "winapi 0.3.9",
+ "xdg-home",
+ "zbus_macros",
+ "zbus_names",
+ "zvariant",
+]
+
+[[package]]
+name = "zbus_macros"
+version = "3.15.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7131497b0f887e8061b430c530240063d33bf9455fa34438f388a245da69e0a5"
+dependencies = [
+ "proc-macro-crate 1.3.1",
+ "proc-macro2",
+ "quote",
+ "regex",
+ "syn 1.0.109",
+ "zvariant_utils",
+]
+
+[[package]]
+name = "zbus_names"
+version = "2.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "437d738d3750bed6ca9b8d423ccc7a8eb284f6b1d6d4e225a0e4e6258d864c8d"
+dependencies = [
+ "serde",
+ "static_assertions",
+ "zvariant",
+]
+
+[[package]]
 name = "zenoh"
 version = "0.7.0-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44140d6ebcf2e52ee48acad0e9d960c2b1e868eec021da2538e58373d615fc18"
 dependencies = [
  "async-global-executor",
  "async-std",
@@ -6949,15 +11022,15 @@
 
 [[package]]
 name = "zenoh-plugin-trait"
 version = "0.7.0-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3b8bfb8e2625e1150dab46b7a4433f866aa06af763237d564b1aa8f6aaf0b29"
 dependencies = [
- "libloading",
+ "libloading 0.7.4",
  "log",
  "serde_json",
  "zenoh-core",
  "zenoh-macros",
  "zenoh-util",
 ]
 
@@ -7043,15 +11116,15 @@
  "clap 3.2.25",
  "futures",
  "hex",
  "home",
  "humantime",
  "lazy_static",
  "libc",
- "libloading",
+ "libloading 0.7.4",
  "log",
  "pnet",
  "pnet_datalink",
  "shellexpand 3.1.0",
  "winapi 0.3.9",
  "zenoh-cfg-properties",
  "zenoh-collections",
@@ -7109,7 +11182,61 @@
 version = "2.0.9+zstd.1.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
 dependencies = [
  "cc",
  "pkg-config",
 ]
+
+[[package]]
+name = "zune-core"
+version = "0.4.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f423a2c17029964870cfaabb1f13dfab7d092a62a29a89264f4d36990ca414a"
+
+[[package]]
+name = "zune-jpeg"
+version = "0.4.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec866b44a2a1fd6133d363f073ca1b179f438f99e7e5bfb1e33f7181facfe448"
+dependencies = [
+ "zune-core",
+]
+
+[[package]]
+name = "zvariant"
+version = "3.15.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4eef2be88ba09b358d3b58aca6e41cd853631d44787f319a1383ca83424fb2db"
+dependencies = [
+ "byteorder",
+ "enumflags2",
+ "libc",
+ "serde",
+ "static_assertions",
+ "url",
+ "zvariant_derive",
+]
+
+[[package]]
+name = "zvariant_derive"
+version = "3.15.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "37c24dc0bed72f5f90d1f8bb5b07228cbf63b3c6e9f82d82559d4bae666e7ed9"
+dependencies = [
+ "proc-macro-crate 1.3.1",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "zvariant_utils",
+]
+
+[[package]]
+name = "zvariant_utils"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7234f0d811589db492d16893e3f21e8e2fd282e6d01b0cddee310322062cc200"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
```

### Comparing `dora_rs-0.3.3rc1/Cargo.toml` & `dora_rs-0.3.4rc2/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [workspace]
 members = ["apis/python/node", "apis/rust/*", "libraries/extensions/telemetry/*"]
 
 [workspace.package]
 # Make sure to also bump `apis/node/python/__init__.py` version.
-version = "0.3.3-rc1"
+version = "0.3.4-rc2"
 description = "`dora` goal is to be a low latency, composable, and distributed data flow."
 documentation = "https://dora.carsmos.ai"
 license = "Apache-2.0"
 
 [workspace.dependencies]
-dora-node-api = { version = "0.3.3-rc1", path = "apis/rust/node", default-features = false }
-dora-node-api-python = { version = "0.3.3-rc1", path = "apis/python/node", default-features = false }
-dora-operator-api = { version = "0.3.3-rc1", path = "apis/rust/operator", default-features = false }
-dora-operator-api-macros = { version = "0.3.3-rc1", path = "apis/rust/operator/macros" }
-dora-operator-api-types = { version = "0.3.3-rc1", path = "apis/rust/operator/types" }
-dora-operator-api-python = { version = "0.3.3-rc1", path = "apis/python/operator" }
-dora-operator-api-c = { version = "0.3.3-rc1", path = "apis/c/operator" }
-dora-node-api-c = { version = "0.3.3-rc1", path = "apis/c/node" }
-dora-core = { version = "0.3.3-rc1", path = "libraries/core" }
-dora-arrow-convert = { version = "0.3.3-rc1", path = "libraries/arrow-convert" }
-dora-tracing = { version = "0.3.3-rc1", path = "libraries/extensions/telemetry/tracing" }
-dora-metrics = { version = "0.3.3-rc1", path = "libraries/extensions/telemetry/metrics" }
-dora-download = { version = "0.3.3-rc1", path = "libraries/extensions/download" }
-shared-memory-server = { version = "0.3.3-rc1", path = "libraries/shared-memory-server" }
-communication-layer-request-reply = { version = "0.3.3-rc1", path = "libraries/communication-layer/request-reply" }
-dora-message = { version = "0.3.3-rc1", path = "libraries/message" }
-dora-runtime = { version = "0.3.3-rc1", path = "binaries/runtime" }
-dora-daemon = { version = "0.3.3-rc1", path = "binaries/daemon" }
-dora-coordinator = { version = "0.3.3-rc1", path = "binaries/coordinator" }
+dora-node-api = { version = "0.3.4-rc2", path = "apis/rust/node", default-features = false }
+dora-node-api-python = { version = "0.3.4-rc2", path = "apis/python/node", default-features = false }
+dora-operator-api = { version = "0.3.4-rc2", path = "apis/rust/operator", default-features = false }
+dora-operator-api-macros = { version = "0.3.4-rc2", path = "apis/rust/operator/macros" }
+dora-operator-api-types = { version = "0.3.4-rc2", path = "apis/rust/operator/types" }
+dora-operator-api-python = { version = "0.3.4-rc2", path = "apis/python/operator" }
+dora-operator-api-c = { version = "0.3.4-rc2", path = "apis/c/operator" }
+dora-node-api-c = { version = "0.3.4-rc2", path = "apis/c/node" }
+dora-core = { version = "0.3.4-rc2", path = "libraries/core" }
+dora-arrow-convert = { version = "0.3.4-rc2", path = "libraries/arrow-convert" }
+dora-tracing = { version = "0.3.4-rc2", path = "libraries/extensions/telemetry/tracing" }
+dora-metrics = { version = "0.3.4-rc2", path = "libraries/extensions/telemetry/metrics" }
+dora-download = { version = "0.3.4-rc2", path = "libraries/extensions/download" }
+shared-memory-server = { version = "0.3.4-rc2", path = "libraries/shared-memory-server" }
+communication-layer-request-reply = { version = "0.3.4-rc2", path = "libraries/communication-layer/request-reply" }
+dora-message = { version = "0.3.4-rc2", path = "libraries/message" }
+dora-runtime = { version = "0.3.4-rc2", path = "binaries/runtime" }
+dora-daemon = { version = "0.3.4-rc2", path = "binaries/daemon" }
+dora-coordinator = { version = "0.3.4-rc2", path = "binaries/coordinator" }
 dora-ros2-bridge = { path = "libraries/extensions/ros2-bridge" }
 dora-ros2-bridge-msg-gen = { path = "libraries/extensions/ros2-bridge/msg-gen" }
 dora-ros2-bridge-python = { path = "libraries/extensions/ros2-bridge/python" }
 arrow = "48.0.0"
 arrow-schema = "48.0.0"
 arrow-data = "48.0.0"
 arrow-array = "48.0.0"
@@ -56,15 +56,15 @@
 dora-core = { workspace = true }
 dora-tracing = { workspace = true }
 dora-download = { workspace = true }
 dunce = "1.0.2"
 serde_yaml = "0.8.23"
 uuid = { version = "1.7", features = ["v7", "serde"] }
 tracing = "0.1.36"
-futures = "0.3.3-rc15"
+futures = "0.3.25"
 tokio-stream = "0.1.11"
 
 [[example]]
 name = "c-dataflow"
 path = "examples/c-dataflow/run.rs"
 
 [[example]]
```

