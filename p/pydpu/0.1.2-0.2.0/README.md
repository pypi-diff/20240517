# Comparing `tmp/pydpu-0.1.2.tar.gz` & `tmp/pydpu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydpu-0.1.2.tar", max compression
+gzip compressed data, was "pydpu-0.2.0.tar", max compression
```

## Comparing `pydpu-0.1.2.tar` & `pydpu-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,94 @@
--rw-r--r--   0        0        0    11357 2023-02-11 01:27:43.624915 pydpu-0.1.2/LICENSE
--rw-r--r--   0        0        0     2910 2023-02-11 01:27:43.624915 pydpu-0.1.2/README.md
--rw-r--r--   0        0        0      112 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/__init__.py
--rw-r--r--   0        0        0       70 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/__main__.py
--rw-r--r--   0        0        0     1971 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/cli.py
--rw-r--r--   0        0        0      303 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/inventory.py
--rw-r--r--   0        0        0      944 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/ipsec.py
--rw-r--r--   0        0        0        0 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/__init__.py
--rw-r--r--   0        0        0      237 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/__init__.py
--rw-r--r--   0        0        0    12035 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_aio_pb2.py
--rw-r--r--   0        0        0    11206 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_aio_pb2_grpc.py
--rw-r--r--   0        0        0     1027 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_iscsi_pb2.py
--rw-r--r--   0        0        0      159 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_iscsi_pb2_grpc.py
--rw-r--r--   0        0        0    11330 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_null_pb2.py
--rw-r--r--   0        0        0    10858 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_null_pb2_grpc.py
--rw-r--r--   0        0        0     1041 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_nvme_pcie_pb2.py
--rw-r--r--   0        0        0      159 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_nvme_pcie_pb2_grpc.py
--rw-r--r--   0        0        0    16284 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_nvme_tcp_pb2.py
--rw-r--r--   0        0        0    13875 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/backend_nvme_tcp_pb2_grpc.py
--rw-r--r--   0        0        0    37698 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/frontend_nvme_pcie_pb2.py
--rw-r--r--   0        0        0    32137 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/frontend_nvme_pcie_pb2_grpc.py
--rw-r--r--   0        0        0    11529 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_blk_pb2.py
--rw-r--r--   0        0        0    11402 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_blk_pb2_grpc.py
--rw-r--r--   0        0        0     1033 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_fs_pb2.py
--rw-r--r--   0        0        0      159 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_fs_pb2_grpc.py
--rw-r--r--   0        0        0    33720 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_scsi_pb2.py
--rw-r--r--   0        0        0    33353 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_scsi_pb2_grpc.py
--rw-r--r--   0        0        0     7141 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/inventory_pb2.py
--rw-r--r--   0        0        0     2518 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/inventory_pb2_grpc.py
--rw-r--r--   0        0        0    36194 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/ipsec_pb2.py
--rw-r--r--   0        0        0    16206 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/ipsec_pb2_grpc.py
--rw-r--r--   0        0        0    12265 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/middleend_pb2.py
--rw-r--r--   0        0        0    11229 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/middleend_pb2_grpc.py
--rw-r--r--   0        0        0     1420 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/object_key_pb2.py
--rw-r--r--   0        0        0      159 2023-02-11 01:27:43.628915 pydpu-0.1.2/pydpu/proto/v1/object_key_pb2_grpc.py
--rw-r--r--   0        0        0     3319 2023-02-11 01:27:43.632915 pydpu-0.1.2/pydpu/proto/v1/opicommon_pb2.py
--rw-r--r--   0        0        0      159 2023-02-11 01:27:43.632915 pydpu-0.1.2/pydpu/proto/v1/opicommon_pb2_grpc.py
--rw-r--r--   0        0        0     1338 2023-02-11 01:27:43.632915 pydpu-0.1.2/pydpu/proto/v1/uuid_pb2.py
--rw-r--r--   0        0        0      159 2023-02-11 01:27:43.632915 pydpu-0.1.2/pydpu/proto/v1/uuid_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-02-11 01:27:43.632915 pydpu-0.1.2/pydpu/storage.py
--rw-r--r--   0        0        0      850 2023-02-11 01:27:43.632915 pydpu-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 pydpu-0.1.2/setup.py
--rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 pydpu-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-17 13:56:00.625090 pydpu-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4428 2024-05-17 13:56:00.625090 pydpu-0.2.0/README.md
+-rw-r--r--   0        0        0      113 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/__init__.py
+-rw-r--r--   0        0        0       70 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/__main__.py
+-rw-r--r--   0        0        0     6018 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/cli.py
+-rw-r--r--   0        0        0        0 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/__init__.py
+-rw-r--r--   0        0        0     1236 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/accounts.py
+-rw-r--r--   0        0        0     1261 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/certificates.py
+-rw-r--r--   0        0        0     4733 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/managers.py
+-rw-r--r--   0        0        0     3246 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/systems.py
+-rw-r--r--   0        0        0     1771 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/update.py
+-rw-r--r--   0        0        0     1615 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/evpn.py
+-rw-r--r--   0        0        0      475 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/inventory.py
+-rw-r--r--   0        0        0     1060 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/ipsec.py
+-rw-r--r--   0        0        0        0 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/__init__.py
+-rw-r--r--   0        0        0      237 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/__init__.py
+-rw-r--r--   0        0        0    10979 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_aio_pb2.py
+-rw-r--r--   0        0        0    10677 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_aio_pb2_grpc.py
+-rw-r--r--   0        0        0     1203 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_iscsi_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_iscsi_pb2_grpc.py
+-rw-r--r--   0        0        0    11443 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_malloc_pb2.py
+-rw-r--r--   0        0        0    11053 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_malloc_pb2_grpc.py
+-rw-r--r--   0        0        0    10920 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_null_pb2.py
+-rw-r--r--   0        0        0    10795 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_null_pb2_grpc.py
+-rw-r--r--   0        0        0    31330 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_nvme_pb2.py
+-rw-r--r--   0        0        0    26793 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_nvme_pb2_grpc.py
+-rw-r--r--   0        0        0    21683 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/bgp_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/bgp_pb2_grpc.py
+-rw-r--r--   0        0        0   115486 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/cloudrpc_pb2.py
+-rw-r--r--   0        0        0   160377 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/cloudrpc_pb2_grpc.py
+-rw-r--r--   0        0        0     2476 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/component_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/component_pb2_grpc.py
+-rw-r--r--   0        0        0     6088 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/device_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/device_pb2_grpc.py
+-rw-r--r--   0        0        0    39939 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/frontend_nvme_pb2.py
+-rw-r--r--   0        0        0    31407 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/frontend_nvme_pb2_grpc.py
+-rw-r--r--   0        0        0    11460 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_blk_pb2.py
+-rw-r--r--   0        0        0    11241 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_blk_pb2_grpc.py
+-rw-r--r--   0        0        0     1214 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_fs_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_fs_pb2_grpc.py
+-rw-r--r--   0        0        0    32429 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_scsi_pb2.py
+-rw-r--r--   0        0        0    33020 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_scsi_pb2_grpc.py
+-rw-r--r--   0        0        0     7161 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/interface_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/interface_pb2_grpc.py
+-rw-r--r--   0        0        0     5931 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/inventory_pb2.py
+-rw-r--r--   0        0        0     2513 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/inventory_pb2_grpc.py
+-rw-r--r--   0        0        0    25046 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/ipsec_pb2.py
+-rw-r--r--   0        0        0    16579 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/ipsec_pb2_grpc.py
+-rw-r--r--   0        0        0     1173 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/k8s_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/k8s_pb2_grpc.py
+-rw-r--r--   0        0        0    22564 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/l2_xpu_infra_mgr_pb2.py
+-rw-r--r--   0        0        0    18666 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/l2_xpu_infra_mgr_pb2_grpc.py
+-rw-r--r--   0        0        0    20461 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/l3_xpu_infra_mgr_pb2.py
+-rw-r--r--   0        0        0    17364 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/l3_xpu_infra_mgr_pb2_grpc.py
+-rw-r--r--   0        0        0     5526 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/mapping_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/mapping_pb2_grpc.py
+-rw-r--r--   0        0        0    12210 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/middleend_encryption_pb2.py
+-rw-r--r--   0        0        0    11693 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/middleend_encryption_pb2_grpc.py
+-rw-r--r--   0        0        0    11668 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/middleend_qos_volume_pb2.py
+-rw-r--r--   0        0        0    11224 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/middleend_qos_volume_pb2_grpc.py
+-rw-r--r--   0        0        0     9053 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkethernet_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkethernet_pb2_grpc.py
+-rw-r--r--   0        0        0    25191 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkinterfaces_pb2.py
+-rw-r--r--   0        0        0     6223 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkinterfaces_pb2_grpc.py
+-rw-r--r--   0        0        0    12778 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkpolicy_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkpolicy_pb2_grpc.py
+-rw-r--r--   0        0        0    10272 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networktypes_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networktypes_pb2_grpc.py
+-rw-r--r--   0        0        0     6922 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkvlan_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkvlan_pb2_grpc.py
+-rw-r--r--   0        0        0     6830 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/nexthop_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/nexthop_pb2_grpc.py
+-rw-r--r--   0        0        0     8855 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/opicommon_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/opicommon_pb2_grpc.py
+-rw-r--r--   0        0        0    11334 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/port_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/port_pb2_grpc.py
+-rw-r--r--   0        0        0     6551 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/route_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/route_pb2_grpc.py
+-rw-r--r--   0        0        0     3971 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/subnet_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/subnet_pb2_grpc.py
+-rw-r--r--   0        0        0     1191 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/telco_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/telco_pb2_grpc.py
+-rw-r--r--   0        0        0     3745 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/tunnel_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/tunnel_pb2_grpc.py
+-rw-r--r--   0        0        0     4397 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/underlayroute_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/underlayroute_pb2_grpc.py
+-rw-r--r--   0        0        0     4668 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/vnic_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/vnic_pb2_grpc.py
+-rw-r--r--   0        0        0     4440 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/vpc_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/vpc_pb2_grpc.py
+-rw-r--r--   0        0        0    21661 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/storage.py
+-rw-r--r--   0        0        0      868 2024-05-17 13:56:00.629090 pydpu-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 pydpu-0.2.0/setup.py
+-rw-r--r--   0        0        0     5159 1970-01-01 00:00:00.000000 pydpu-0.2.0/PKG-INFO
```

### Comparing `pydpu-0.1.2/LICENSE` & `pydpu-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydpu-0.1.2/pydpu/ipsec.py` & `pydpu-0.2.0/pydpu/ipsec.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 import grpc
 
 from .proto.v1 import ipsec_pb2, ipsec_pb2_grpc
 
 
 def get_stats(address):
-    channel = grpc.insecure_channel(address)
-    stub = ipsec_pb2_grpc.IPsecStub(channel)
-    a = stub.IPsecVersion(ipsec_pb2.IPsecVersionReq())
-    b = stub.IPsecStats(ipsec_pb2.IPsecStatsReq())
-    c = stub.IPsecListConns(ipsec_pb2.IPsecListConnsReq(ike="tun1_0_0"))
-    d = stub.IPsecListSas(ipsec_pb2.IPsecListSasReq(ike="tun1_0_0"))
-    e = stub.IPsecListCerts(ipsec_pb2.IPsecListCertsReq())
-    print(a, b, c, d, e)
+    with grpc.insecure_channel(address) as channel:
+        stub = ipsec_pb2_grpc.IPsecServiceStub(channel)
+        a = stub.IPsecVersion(ipsec_pb2.IPsecVersionRequest())
+        b = stub.IPsecStats(ipsec_pb2.IPsecStatsRequest())
+        c = stub.IPsecListConns(ipsec_pb2.IPsecListConnsRequest(ike="tun1_0_0"))
+        d = stub.IPsecListSas(ipsec_pb2.IPsecListSasRequest(ike="tun1_0_0"))
+        e = stub.IPsecListCerts(ipsec_pb2.IPsecListCertsRequest())
+        print(a, b, c, d, e)
 
 
 def create_new_tunnel(address):
-    channel = grpc.insecure_channel(address)
-    stub = ipsec_pb2_grpc.IPsecStub(channel)
-    # connection_1 = stub.IPsecLoadConn(tun1_0_0)
-    # connection_2 = stub.IPsecLoadConn(tun1_0_1)
-    print(
-        "tbd",
-        stub,
-        grpc.StatusCode.UNIMPLEMENTED,
-        ipsec_pb2.IPsecStatsReq(),
-    )
+    with grpc.insecure_channel(address) as channel:
+        stub = ipsec_pb2_grpc.IPsecServiceStub(channel)
+        # connection_1 = stub.IPsecLoadConn(tun1_0_0)
+        # connection_2 = stub.IPsecLoadConn(tun1_0_1)
+        print(
+            "tbd",
+            stub,
+            grpc.StatusCode.UNIMPLEMENTED,
+            ipsec_pb2.IPsecStatsRequest(),
+        )
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/backend_aio_pb2_grpc.py` & `pydpu-0.2.0/pydpu/proto/v1/backend_aio_pb2_grpc.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,234 +2,240 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 import backend_aio_pb2 as backend__aio__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-class AioControllerServiceStub(object):
+class AioVolumeServiceStub(object):
     """Back End (network-facing) APIs. This service is for AIO generic kernel block device.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.CreateAioController = channel.unary_unary(
-                '/opi_api.storage.v1.AioControllerService/CreateAioController',
-                request_serializer=backend__aio__pb2.CreateAioControllerRequest.SerializeToString,
-                response_deserializer=backend__aio__pb2.AioController.FromString,
-                )
-        self.DeleteAioController = channel.unary_unary(
-                '/opi_api.storage.v1.AioControllerService/DeleteAioController',
-                request_serializer=backend__aio__pb2.DeleteAioControllerRequest.SerializeToString,
+        self.CreateAioVolume = channel.unary_unary(
+                '/opi_api.storage.v1.AioVolumeService/CreateAioVolume',
+                request_serializer=backend__aio__pb2.CreateAioVolumeRequest.SerializeToString,
+                response_deserializer=backend__aio__pb2.AioVolume.FromString,
+                )
+        self.DeleteAioVolume = channel.unary_unary(
+                '/opi_api.storage.v1.AioVolumeService/DeleteAioVolume',
+                request_serializer=backend__aio__pb2.DeleteAioVolumeRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
-        self.UpdateAioController = channel.unary_unary(
-                '/opi_api.storage.v1.AioControllerService/UpdateAioController',
-                request_serializer=backend__aio__pb2.UpdateAioControllerRequest.SerializeToString,
-                response_deserializer=backend__aio__pb2.AioController.FromString,
+        self.UpdateAioVolume = channel.unary_unary(
+                '/opi_api.storage.v1.AioVolumeService/UpdateAioVolume',
+                request_serializer=backend__aio__pb2.UpdateAioVolumeRequest.SerializeToString,
+                response_deserializer=backend__aio__pb2.AioVolume.FromString,
                 )
-        self.ListAioControllers = channel.unary_unary(
-                '/opi_api.storage.v1.AioControllerService/ListAioControllers',
-                request_serializer=backend__aio__pb2.ListAioControllersRequest.SerializeToString,
-                response_deserializer=backend__aio__pb2.ListAioControllersResponse.FromString,
+        self.ListAioVolumes = channel.unary_unary(
+                '/opi_api.storage.v1.AioVolumeService/ListAioVolumes',
+                request_serializer=backend__aio__pb2.ListAioVolumesRequest.SerializeToString,
+                response_deserializer=backend__aio__pb2.ListAioVolumesResponse.FromString,
                 )
-        self.GetAioController = channel.unary_unary(
-                '/opi_api.storage.v1.AioControllerService/GetAioController',
-                request_serializer=backend__aio__pb2.GetAioControllerRequest.SerializeToString,
-                response_deserializer=backend__aio__pb2.AioController.FromString,
+        self.GetAioVolume = channel.unary_unary(
+                '/opi_api.storage.v1.AioVolumeService/GetAioVolume',
+                request_serializer=backend__aio__pb2.GetAioVolumeRequest.SerializeToString,
+                response_deserializer=backend__aio__pb2.AioVolume.FromString,
                 )
-        self.AioControllerStats = channel.unary_unary(
-                '/opi_api.storage.v1.AioControllerService/AioControllerStats',
-                request_serializer=backend__aio__pb2.AioControllerStatsRequest.SerializeToString,
-                response_deserializer=backend__aio__pb2.AioControllerStatsResponse.FromString,
+        self.StatsAioVolume = channel.unary_unary(
+                '/opi_api.storage.v1.AioVolumeService/StatsAioVolume',
+                request_serializer=backend__aio__pb2.StatsAioVolumeRequest.SerializeToString,
+                response_deserializer=backend__aio__pb2.StatsAioVolumeResponse.FromString,
                 )
 
 
-class AioControllerServiceServicer(object):
+class AioVolumeServiceServicer(object):
     """Back End (network-facing) APIs. This service is for AIO generic kernel block device.
     """
 
-    def CreateAioController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def CreateAioVolume(self, request, context):
+        """Create an Aio Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteAioController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def DeleteAioVolume(self, request, context):
+        """Delete an Aio Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UpdateAioController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def UpdateAioVolume(self, request, context):
+        """Update an Aio Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListAioControllers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ListAioVolumes(self, request, context):
+        """List Aio Volumes
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetAioController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetAioVolume(self, request, context):
+        """Get an Aio Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def AioControllerStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsAioVolume(self, request, context):
+        """Get an Aio Volume statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_AioControllerServiceServicer_to_server(servicer, server):
+def add_AioVolumeServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'CreateAioController': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateAioController,
-                    request_deserializer=backend__aio__pb2.CreateAioControllerRequest.FromString,
-                    response_serializer=backend__aio__pb2.AioController.SerializeToString,
-            ),
-            'DeleteAioController': grpc.unary_unary_rpc_method_handler(
-                    servicer.DeleteAioController,
-                    request_deserializer=backend__aio__pb2.DeleteAioControllerRequest.FromString,
+            'CreateAioVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateAioVolume,
+                    request_deserializer=backend__aio__pb2.CreateAioVolumeRequest.FromString,
+                    response_serializer=backend__aio__pb2.AioVolume.SerializeToString,
+            ),
+            'DeleteAioVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteAioVolume,
+                    request_deserializer=backend__aio__pb2.DeleteAioVolumeRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
-            'UpdateAioController': grpc.unary_unary_rpc_method_handler(
-                    servicer.UpdateAioController,
-                    request_deserializer=backend__aio__pb2.UpdateAioControllerRequest.FromString,
-                    response_serializer=backend__aio__pb2.AioController.SerializeToString,
-            ),
-            'ListAioControllers': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListAioControllers,
-                    request_deserializer=backend__aio__pb2.ListAioControllersRequest.FromString,
-                    response_serializer=backend__aio__pb2.ListAioControllersResponse.SerializeToString,
-            ),
-            'GetAioController': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAioController,
-                    request_deserializer=backend__aio__pb2.GetAioControllerRequest.FromString,
-                    response_serializer=backend__aio__pb2.AioController.SerializeToString,
-            ),
-            'AioControllerStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.AioControllerStats,
-                    request_deserializer=backend__aio__pb2.AioControllerStatsRequest.FromString,
-                    response_serializer=backend__aio__pb2.AioControllerStatsResponse.SerializeToString,
+            'UpdateAioVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateAioVolume,
+                    request_deserializer=backend__aio__pb2.UpdateAioVolumeRequest.FromString,
+                    response_serializer=backend__aio__pb2.AioVolume.SerializeToString,
+            ),
+            'ListAioVolumes': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListAioVolumes,
+                    request_deserializer=backend__aio__pb2.ListAioVolumesRequest.FromString,
+                    response_serializer=backend__aio__pb2.ListAioVolumesResponse.SerializeToString,
+            ),
+            'GetAioVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAioVolume,
+                    request_deserializer=backend__aio__pb2.GetAioVolumeRequest.FromString,
+                    response_serializer=backend__aio__pb2.AioVolume.SerializeToString,
+            ),
+            'StatsAioVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsAioVolume,
+                    request_deserializer=backend__aio__pb2.StatsAioVolumeRequest.FromString,
+                    response_serializer=backend__aio__pb2.StatsAioVolumeResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'opi_api.storage.v1.AioControllerService', rpc_method_handlers)
+            'opi_api.storage.v1.AioVolumeService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class AioControllerService(object):
+class AioVolumeService(object):
     """Back End (network-facing) APIs. This service is for AIO generic kernel block device.
     """
 
     @staticmethod
-    def CreateAioController(request,
+    def CreateAioVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioControllerService/CreateAioController',
-            backend__aio__pb2.CreateAioControllerRequest.SerializeToString,
-            backend__aio__pb2.AioController.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioVolumeService/CreateAioVolume',
+            backend__aio__pb2.CreateAioVolumeRequest.SerializeToString,
+            backend__aio__pb2.AioVolume.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteAioController(request,
+    def DeleteAioVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioControllerService/DeleteAioController',
-            backend__aio__pb2.DeleteAioControllerRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioVolumeService/DeleteAioVolume',
+            backend__aio__pb2.DeleteAioVolumeRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UpdateAioController(request,
+    def UpdateAioVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioControllerService/UpdateAioController',
-            backend__aio__pb2.UpdateAioControllerRequest.SerializeToString,
-            backend__aio__pb2.AioController.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioVolumeService/UpdateAioVolume',
+            backend__aio__pb2.UpdateAioVolumeRequest.SerializeToString,
+            backend__aio__pb2.AioVolume.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListAioControllers(request,
+    def ListAioVolumes(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioControllerService/ListAioControllers',
-            backend__aio__pb2.ListAioControllersRequest.SerializeToString,
-            backend__aio__pb2.ListAioControllersResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioVolumeService/ListAioVolumes',
+            backend__aio__pb2.ListAioVolumesRequest.SerializeToString,
+            backend__aio__pb2.ListAioVolumesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetAioController(request,
+    def GetAioVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioControllerService/GetAioController',
-            backend__aio__pb2.GetAioControllerRequest.SerializeToString,
-            backend__aio__pb2.AioController.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioVolumeService/GetAioVolume',
+            backend__aio__pb2.GetAioVolumeRequest.SerializeToString,
+            backend__aio__pb2.AioVolume.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def AioControllerStats(request,
+    def StatsAioVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioControllerService/AioControllerStats',
-            backend__aio__pb2.AioControllerStatsRequest.SerializeToString,
-            backend__aio__pb2.AioControllerStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.AioVolumeService/StatsAioVolume',
+            backend__aio__pb2.StatsAioVolumeRequest.SerializeToString,
+            backend__aio__pb2.StatsAioVolumeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/backend_iscsi_pb2.py` & `pydpu-0.2.0/pydpu/proto/v1/k8s_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: backend_iscsi.proto
+# source: k8s.proto
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x62\x61\x63kend_iscsi.proto\x12\x12opi_api.storage.v1B`\n\x12opi_api.storage.v1B\x11\x42\x61\x63kendIscsiProtoP\x01Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/gob\x06proto3')
-
-
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tk8s.proto\x12\x1copi_api.network.k8s.v1alpha1Be\n\x1copi_api.network.k8s.v1alpha1B\x08K8sProtoP\x01Z9github.com/opiproject/opi-api/network/k8s/v1alpha1/gen/gob\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'k8s_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\022opi_api.storage.v1B\021BackendIscsiProtoP\001Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/go'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034opi_api.network.k8s.v1alpha1B\010K8sProtoP\001Z9github.com/opiproject/opi-api/network/k8s/v1alpha1/gen/go'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/backend_null_pb2_grpc.py` & `pydpu-0.2.0/pydpu/proto/v1/backend_null_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,234 +2,240 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 import backend_null_pb2 as backend__null__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-class NullDebugServiceStub(object):
+class NullVolumeServiceStub(object):
     """Back End (network-facing) APIs. This is debug interface for null block devices.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.CreateNullDebug = channel.unary_unary(
-                '/opi_api.storage.v1.NullDebugService/CreateNullDebug',
-                request_serializer=backend__null__pb2.CreateNullDebugRequest.SerializeToString,
-                response_deserializer=backend__null__pb2.NullDebug.FromString,
-                )
-        self.DeleteNullDebug = channel.unary_unary(
-                '/opi_api.storage.v1.NullDebugService/DeleteNullDebug',
-                request_serializer=backend__null__pb2.DeleteNullDebugRequest.SerializeToString,
+        self.CreateNullVolume = channel.unary_unary(
+                '/opi_api.storage.v1.NullVolumeService/CreateNullVolume',
+                request_serializer=backend__null__pb2.CreateNullVolumeRequest.SerializeToString,
+                response_deserializer=backend__null__pb2.NullVolume.FromString,
+                )
+        self.DeleteNullVolume = channel.unary_unary(
+                '/opi_api.storage.v1.NullVolumeService/DeleteNullVolume',
+                request_serializer=backend__null__pb2.DeleteNullVolumeRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
-        self.UpdateNullDebug = channel.unary_unary(
-                '/opi_api.storage.v1.NullDebugService/UpdateNullDebug',
-                request_serializer=backend__null__pb2.UpdateNullDebugRequest.SerializeToString,
-                response_deserializer=backend__null__pb2.NullDebug.FromString,
+        self.UpdateNullVolume = channel.unary_unary(
+                '/opi_api.storage.v1.NullVolumeService/UpdateNullVolume',
+                request_serializer=backend__null__pb2.UpdateNullVolumeRequest.SerializeToString,
+                response_deserializer=backend__null__pb2.NullVolume.FromString,
                 )
-        self.ListNullDebugs = channel.unary_unary(
-                '/opi_api.storage.v1.NullDebugService/ListNullDebugs',
-                request_serializer=backend__null__pb2.ListNullDebugsRequest.SerializeToString,
-                response_deserializer=backend__null__pb2.ListNullDebugsResponse.FromString,
+        self.ListNullVolumes = channel.unary_unary(
+                '/opi_api.storage.v1.NullVolumeService/ListNullVolumes',
+                request_serializer=backend__null__pb2.ListNullVolumesRequest.SerializeToString,
+                response_deserializer=backend__null__pb2.ListNullVolumesResponse.FromString,
                 )
-        self.GetNullDebug = channel.unary_unary(
-                '/opi_api.storage.v1.NullDebugService/GetNullDebug',
-                request_serializer=backend__null__pb2.GetNullDebugRequest.SerializeToString,
-                response_deserializer=backend__null__pb2.NullDebug.FromString,
+        self.GetNullVolume = channel.unary_unary(
+                '/opi_api.storage.v1.NullVolumeService/GetNullVolume',
+                request_serializer=backend__null__pb2.GetNullVolumeRequest.SerializeToString,
+                response_deserializer=backend__null__pb2.NullVolume.FromString,
                 )
-        self.NullDebugStats = channel.unary_unary(
-                '/opi_api.storage.v1.NullDebugService/NullDebugStats',
-                request_serializer=backend__null__pb2.NullDebugStatsRequest.SerializeToString,
-                response_deserializer=backend__null__pb2.NullDebugStatsResponse.FromString,
+        self.StatsNullVolume = channel.unary_unary(
+                '/opi_api.storage.v1.NullVolumeService/StatsNullVolume',
+                request_serializer=backend__null__pb2.StatsNullVolumeRequest.SerializeToString,
+                response_deserializer=backend__null__pb2.StatsNullVolumeResponse.FromString,
                 )
 
 
-class NullDebugServiceServicer(object):
+class NullVolumeServiceServicer(object):
     """Back End (network-facing) APIs. This is debug interface for null block devices.
     """
 
-    def CreateNullDebug(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def CreateNullVolume(self, request, context):
+        """Create an Null Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteNullDebug(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def DeleteNullVolume(self, request, context):
+        """Delete an Null Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UpdateNullDebug(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def UpdateNullVolume(self, request, context):
+        """Update an Null Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListNullDebugs(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ListNullVolumes(self, request, context):
+        """List Null Volumes
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetNullDebug(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetNullVolume(self, request, context):
+        """Get an Null Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def NullDebugStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsNullVolume(self, request, context):
+        """Get an Null Volume statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_NullDebugServiceServicer_to_server(servicer, server):
+def add_NullVolumeServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'CreateNullDebug': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateNullDebug,
-                    request_deserializer=backend__null__pb2.CreateNullDebugRequest.FromString,
-                    response_serializer=backend__null__pb2.NullDebug.SerializeToString,
-            ),
-            'DeleteNullDebug': grpc.unary_unary_rpc_method_handler(
-                    servicer.DeleteNullDebug,
-                    request_deserializer=backend__null__pb2.DeleteNullDebugRequest.FromString,
+            'CreateNullVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateNullVolume,
+                    request_deserializer=backend__null__pb2.CreateNullVolumeRequest.FromString,
+                    response_serializer=backend__null__pb2.NullVolume.SerializeToString,
+            ),
+            'DeleteNullVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteNullVolume,
+                    request_deserializer=backend__null__pb2.DeleteNullVolumeRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
-            'UpdateNullDebug': grpc.unary_unary_rpc_method_handler(
-                    servicer.UpdateNullDebug,
-                    request_deserializer=backend__null__pb2.UpdateNullDebugRequest.FromString,
-                    response_serializer=backend__null__pb2.NullDebug.SerializeToString,
-            ),
-            'ListNullDebugs': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListNullDebugs,
-                    request_deserializer=backend__null__pb2.ListNullDebugsRequest.FromString,
-                    response_serializer=backend__null__pb2.ListNullDebugsResponse.SerializeToString,
-            ),
-            'GetNullDebug': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNullDebug,
-                    request_deserializer=backend__null__pb2.GetNullDebugRequest.FromString,
-                    response_serializer=backend__null__pb2.NullDebug.SerializeToString,
-            ),
-            'NullDebugStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.NullDebugStats,
-                    request_deserializer=backend__null__pb2.NullDebugStatsRequest.FromString,
-                    response_serializer=backend__null__pb2.NullDebugStatsResponse.SerializeToString,
+            'UpdateNullVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateNullVolume,
+                    request_deserializer=backend__null__pb2.UpdateNullVolumeRequest.FromString,
+                    response_serializer=backend__null__pb2.NullVolume.SerializeToString,
+            ),
+            'ListNullVolumes': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListNullVolumes,
+                    request_deserializer=backend__null__pb2.ListNullVolumesRequest.FromString,
+                    response_serializer=backend__null__pb2.ListNullVolumesResponse.SerializeToString,
+            ),
+            'GetNullVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetNullVolume,
+                    request_deserializer=backend__null__pb2.GetNullVolumeRequest.FromString,
+                    response_serializer=backend__null__pb2.NullVolume.SerializeToString,
+            ),
+            'StatsNullVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsNullVolume,
+                    request_deserializer=backend__null__pb2.StatsNullVolumeRequest.FromString,
+                    response_serializer=backend__null__pb2.StatsNullVolumeResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'opi_api.storage.v1.NullDebugService', rpc_method_handlers)
+            'opi_api.storage.v1.NullVolumeService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class NullDebugService(object):
+class NullVolumeService(object):
     """Back End (network-facing) APIs. This is debug interface for null block devices.
     """
 
     @staticmethod
-    def CreateNullDebug(request,
+    def CreateNullVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullDebugService/CreateNullDebug',
-            backend__null__pb2.CreateNullDebugRequest.SerializeToString,
-            backend__null__pb2.NullDebug.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullVolumeService/CreateNullVolume',
+            backend__null__pb2.CreateNullVolumeRequest.SerializeToString,
+            backend__null__pb2.NullVolume.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteNullDebug(request,
+    def DeleteNullVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullDebugService/DeleteNullDebug',
-            backend__null__pb2.DeleteNullDebugRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullVolumeService/DeleteNullVolume',
+            backend__null__pb2.DeleteNullVolumeRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UpdateNullDebug(request,
+    def UpdateNullVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullDebugService/UpdateNullDebug',
-            backend__null__pb2.UpdateNullDebugRequest.SerializeToString,
-            backend__null__pb2.NullDebug.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullVolumeService/UpdateNullVolume',
+            backend__null__pb2.UpdateNullVolumeRequest.SerializeToString,
+            backend__null__pb2.NullVolume.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListNullDebugs(request,
+    def ListNullVolumes(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullDebugService/ListNullDebugs',
-            backend__null__pb2.ListNullDebugsRequest.SerializeToString,
-            backend__null__pb2.ListNullDebugsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullVolumeService/ListNullVolumes',
+            backend__null__pb2.ListNullVolumesRequest.SerializeToString,
+            backend__null__pb2.ListNullVolumesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetNullDebug(request,
+    def GetNullVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullDebugService/GetNullDebug',
-            backend__null__pb2.GetNullDebugRequest.SerializeToString,
-            backend__null__pb2.NullDebug.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullVolumeService/GetNullVolume',
+            backend__null__pb2.GetNullVolumeRequest.SerializeToString,
+            backend__null__pb2.NullVolume.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def NullDebugStats(request,
+    def StatsNullVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullDebugService/NullDebugStats',
-            backend__null__pb2.NullDebugStatsRequest.SerializeToString,
-            backend__null__pb2.NullDebugStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.NullVolumeService/StatsNullVolume',
+            backend__null__pb2.StatsNullVolumeRequest.SerializeToString,
+            backend__null__pb2.StatsNullVolumeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/backend_nvme_pcie_pb2.py` & `pydpu-0.2.0/pydpu/proto/v1/backend_iscsi_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: backend_nvme_pcie.proto
+# source: backend_iscsi.proto
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x62\x61\x63kend_nvme_pcie.proto\x12\x12opi_api.storage.v1Bc\n\x12opi_api.storage.v1B\x14\x42\x61\x63kendNvmePcieProtoP\x01Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/gob\x06proto3')
-
-
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x62\x61\x63kend_iscsi.proto\x12\x12opi_api.storage.v1B`\n\x12opi_api.storage.v1B\x11\x42\x61\x63kendIscsiProtoP\x01Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/gob\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'backend_iscsi_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\022opi_api.storage.v1B\024BackendNvmePcieProtoP\001Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/go'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\022opi_api.storage.v1B\021BackendIscsiProtoP\001Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/go'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/frontend_nvme_pcie_pb2_grpc.py` & `pydpu-0.2.0/pydpu/proto/v1/frontend_nvme_pb2_grpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,631 +1,657 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-import frontend_nvme_pcie_pb2 as frontend__nvme__pcie__pb2
+import frontend_nvme_pb2 as frontend__nvme__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 class FrontendNvmeServiceStub(object):
-    """Front End (host-facing) APIs. Mostly used for NVMe/PCIe emulation and host presentation.
+    """Front End APIs. Used for creation of xPU managed Nvme devices
+    e.g. emulated host-facing Nvme/Pcie controllers as well as
+    Nvme-oF controllers
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.CreateNVMeSubsystem = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/CreateNVMeSubsystem',
-                request_serializer=frontend__nvme__pcie__pb2.CreateNVMeSubsystemRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeSubsystem.FromString,
-                )
-        self.DeleteNVMeSubsystem = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/DeleteNVMeSubsystem',
-                request_serializer=frontend__nvme__pcie__pb2.DeleteNVMeSubsystemRequest.SerializeToString,
+        self.CreateNvmeSubsystem = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/CreateNvmeSubsystem',
+                request_serializer=frontend__nvme__pb2.CreateNvmeSubsystemRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.NvmeSubsystem.FromString,
+                )
+        self.DeleteNvmeSubsystem = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/DeleteNvmeSubsystem',
+                request_serializer=frontend__nvme__pb2.DeleteNvmeSubsystemRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
-        self.UpdateNVMeSubsystem = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/UpdateNVMeSubsystem',
-                request_serializer=frontend__nvme__pcie__pb2.UpdateNVMeSubsystemRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeSubsystem.FromString,
-                )
-        self.ListNVMeSubsystems = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/ListNVMeSubsystems',
-                request_serializer=frontend__nvme__pcie__pb2.ListNVMeSubsystemsRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.ListNVMeSubsystemsResponse.FromString,
-                )
-        self.GetNVMeSubsystem = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/GetNVMeSubsystem',
-                request_serializer=frontend__nvme__pcie__pb2.GetNVMeSubsystemRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeSubsystem.FromString,
-                )
-        self.NVMeSubsystemStats = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/NVMeSubsystemStats',
-                request_serializer=frontend__nvme__pcie__pb2.NVMeSubsystemStatsRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeSubsystemStatsResponse.FromString,
-                )
-        self.CreateNVMeController = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/CreateNVMeController',
-                request_serializer=frontend__nvme__pcie__pb2.CreateNVMeControllerRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeController.FromString,
-                )
-        self.DeleteNVMeController = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/DeleteNVMeController',
-                request_serializer=frontend__nvme__pcie__pb2.DeleteNVMeControllerRequest.SerializeToString,
+        self.UpdateNvmeSubsystem = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/UpdateNvmeSubsystem',
+                request_serializer=frontend__nvme__pb2.UpdateNvmeSubsystemRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.NvmeSubsystem.FromString,
+                )
+        self.ListNvmeSubsystems = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/ListNvmeSubsystems',
+                request_serializer=frontend__nvme__pb2.ListNvmeSubsystemsRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.ListNvmeSubsystemsResponse.FromString,
+                )
+        self.GetNvmeSubsystem = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/GetNvmeSubsystem',
+                request_serializer=frontend__nvme__pb2.GetNvmeSubsystemRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.NvmeSubsystem.FromString,
+                )
+        self.StatsNvmeSubsystem = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/StatsNvmeSubsystem',
+                request_serializer=frontend__nvme__pb2.StatsNvmeSubsystemRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.StatsNvmeSubsystemResponse.FromString,
+                )
+        self.CreateNvmeController = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/CreateNvmeController',
+                request_serializer=frontend__nvme__pb2.CreateNvmeControllerRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.NvmeController.FromString,
+                )
+        self.DeleteNvmeController = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/DeleteNvmeController',
+                request_serializer=frontend__nvme__pb2.DeleteNvmeControllerRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
-        self.UpdateNVMeController = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/UpdateNVMeController',
-                request_serializer=frontend__nvme__pcie__pb2.UpdateNVMeControllerRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeController.FromString,
-                )
-        self.ListNVMeControllers = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/ListNVMeControllers',
-                request_serializer=frontend__nvme__pcie__pb2.ListNVMeControllersRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.ListNVMeControllersResponse.FromString,
-                )
-        self.GetNVMeController = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/GetNVMeController',
-                request_serializer=frontend__nvme__pcie__pb2.GetNVMeControllerRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeController.FromString,
-                )
-        self.NVMeControllerStats = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/NVMeControllerStats',
-                request_serializer=frontend__nvme__pcie__pb2.NVMeControllerStatsRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeControllerStatsResponse.FromString,
-                )
-        self.CreateNVMeNamespace = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/CreateNVMeNamespace',
-                request_serializer=frontend__nvme__pcie__pb2.CreateNVMeNamespaceRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeNamespace.FromString,
-                )
-        self.DeleteNVMeNamespace = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/DeleteNVMeNamespace',
-                request_serializer=frontend__nvme__pcie__pb2.DeleteNVMeNamespaceRequest.SerializeToString,
+        self.UpdateNvmeController = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/UpdateNvmeController',
+                request_serializer=frontend__nvme__pb2.UpdateNvmeControllerRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.NvmeController.FromString,
+                )
+        self.ListNvmeControllers = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/ListNvmeControllers',
+                request_serializer=frontend__nvme__pb2.ListNvmeControllersRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.ListNvmeControllersResponse.FromString,
+                )
+        self.GetNvmeController = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/GetNvmeController',
+                request_serializer=frontend__nvme__pb2.GetNvmeControllerRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.NvmeController.FromString,
+                )
+        self.StatsNvmeController = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/StatsNvmeController',
+                request_serializer=frontend__nvme__pb2.StatsNvmeControllerRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.StatsNvmeControllerResponse.FromString,
+                )
+        self.CreateNvmeNamespace = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/CreateNvmeNamespace',
+                request_serializer=frontend__nvme__pb2.CreateNvmeNamespaceRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.NvmeNamespace.FromString,
+                )
+        self.DeleteNvmeNamespace = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/DeleteNvmeNamespace',
+                request_serializer=frontend__nvme__pb2.DeleteNvmeNamespaceRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
-        self.UpdateNVMeNamespace = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/UpdateNVMeNamespace',
-                request_serializer=frontend__nvme__pcie__pb2.UpdateNVMeNamespaceRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeNamespace.FromString,
-                )
-        self.ListNVMeNamespaces = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/ListNVMeNamespaces',
-                request_serializer=frontend__nvme__pcie__pb2.ListNVMeNamespacesRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.ListNVMeNamespacesResponse.FromString,
-                )
-        self.GetNVMeNamespace = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/GetNVMeNamespace',
-                request_serializer=frontend__nvme__pcie__pb2.GetNVMeNamespaceRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeNamespace.FromString,
-                )
-        self.NVMeNamespaceStats = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendNvmeService/NVMeNamespaceStats',
-                request_serializer=frontend__nvme__pcie__pb2.NVMeNamespaceStatsRequest.SerializeToString,
-                response_deserializer=frontend__nvme__pcie__pb2.NVMeNamespaceStatsResponse.FromString,
+        self.UpdateNvmeNamespace = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/UpdateNvmeNamespace',
+                request_serializer=frontend__nvme__pb2.UpdateNvmeNamespaceRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.NvmeNamespace.FromString,
+                )
+        self.ListNvmeNamespaces = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/ListNvmeNamespaces',
+                request_serializer=frontend__nvme__pb2.ListNvmeNamespacesRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.ListNvmeNamespacesResponse.FromString,
+                )
+        self.GetNvmeNamespace = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/GetNvmeNamespace',
+                request_serializer=frontend__nvme__pb2.GetNvmeNamespaceRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.NvmeNamespace.FromString,
+                )
+        self.StatsNvmeNamespace = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendNvmeService/StatsNvmeNamespace',
+                request_serializer=frontend__nvme__pb2.StatsNvmeNamespaceRequest.SerializeToString,
+                response_deserializer=frontend__nvme__pb2.StatsNvmeNamespaceResponse.FromString,
                 )
 
 
 class FrontendNvmeServiceServicer(object):
-    """Front End (host-facing) APIs. Mostly used for NVMe/PCIe emulation and host presentation.
+    """Front End APIs. Used for creation of xPU managed Nvme devices
+    e.g. emulated host-facing Nvme/Pcie controllers as well as
+    Nvme-oF controllers
     """
 
-    def CreateNVMeSubsystem(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def CreateNvmeSubsystem(self, request, context):
+        """Create an Nvme Subsystem
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteNVMeSubsystem(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def DeleteNvmeSubsystem(self, request, context):
+        """Delete an Nvme Subsystem
+        Fails if there are any associated objects
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UpdateNVMeSubsystem(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def UpdateNvmeSubsystem(self, request, context):
+        """Update an Nvme Subsystem
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListNVMeSubsystems(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ListNvmeSubsystems(self, request, context):
+        """List Nvme Subsystems
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetNVMeSubsystem(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetNvmeSubsystem(self, request, context):
+        """Get an Nvme Subsystem
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def NVMeSubsystemStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsNvmeSubsystem(self, request, context):
+        """Get an Nvme Subsystem statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateNVMeController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def CreateNvmeController(self, request, context):
+        """Create an Nvme Controller
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteNVMeController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def DeleteNvmeController(self, request, context):
+        """Delete an Nvme Controller
+        Fails if there are any associated objects
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UpdateNVMeController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def UpdateNvmeController(self, request, context):
+        """Update an Nvme Controller
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListNVMeControllers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ListNvmeControllers(self, request, context):
+        """List Nvme Controllers
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetNVMeController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetNvmeController(self, request, context):
+        """Get an Nvme Controller
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def NVMeControllerStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsNvmeController(self, request, context):
+        """Get an Nvme Controller statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateNVMeNamespace(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def CreateNvmeNamespace(self, request, context):
+        """Create an Nvme Namespace
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteNVMeNamespace(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def DeleteNvmeNamespace(self, request, context):
+        """Delete an Nvme Namespace
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UpdateNVMeNamespace(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def UpdateNvmeNamespace(self, request, context):
+        """Update an Nvme Namespace
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListNVMeNamespaces(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ListNvmeNamespaces(self, request, context):
+        """List Nvme Namespaces
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetNVMeNamespace(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetNvmeNamespace(self, request, context):
+        """Get an Nvme Namespace
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def NVMeNamespaceStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsNvmeNamespace(self, request, context):
+        """Get an Nvme Namespace statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_FrontendNvmeServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'CreateNVMeSubsystem': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateNVMeSubsystem,
-                    request_deserializer=frontend__nvme__pcie__pb2.CreateNVMeSubsystemRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeSubsystem.SerializeToString,
-            ),
-            'DeleteNVMeSubsystem': grpc.unary_unary_rpc_method_handler(
-                    servicer.DeleteNVMeSubsystem,
-                    request_deserializer=frontend__nvme__pcie__pb2.DeleteNVMeSubsystemRequest.FromString,
+            'CreateNvmeSubsystem': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateNvmeSubsystem,
+                    request_deserializer=frontend__nvme__pb2.CreateNvmeSubsystemRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.NvmeSubsystem.SerializeToString,
+            ),
+            'DeleteNvmeSubsystem': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteNvmeSubsystem,
+                    request_deserializer=frontend__nvme__pb2.DeleteNvmeSubsystemRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
-            'UpdateNVMeSubsystem': grpc.unary_unary_rpc_method_handler(
-                    servicer.UpdateNVMeSubsystem,
-                    request_deserializer=frontend__nvme__pcie__pb2.UpdateNVMeSubsystemRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeSubsystem.SerializeToString,
-            ),
-            'ListNVMeSubsystems': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListNVMeSubsystems,
-                    request_deserializer=frontend__nvme__pcie__pb2.ListNVMeSubsystemsRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.ListNVMeSubsystemsResponse.SerializeToString,
-            ),
-            'GetNVMeSubsystem': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNVMeSubsystem,
-                    request_deserializer=frontend__nvme__pcie__pb2.GetNVMeSubsystemRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeSubsystem.SerializeToString,
-            ),
-            'NVMeSubsystemStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.NVMeSubsystemStats,
-                    request_deserializer=frontend__nvme__pcie__pb2.NVMeSubsystemStatsRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeSubsystemStatsResponse.SerializeToString,
-            ),
-            'CreateNVMeController': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateNVMeController,
-                    request_deserializer=frontend__nvme__pcie__pb2.CreateNVMeControllerRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeController.SerializeToString,
-            ),
-            'DeleteNVMeController': grpc.unary_unary_rpc_method_handler(
-                    servicer.DeleteNVMeController,
-                    request_deserializer=frontend__nvme__pcie__pb2.DeleteNVMeControllerRequest.FromString,
+            'UpdateNvmeSubsystem': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateNvmeSubsystem,
+                    request_deserializer=frontend__nvme__pb2.UpdateNvmeSubsystemRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.NvmeSubsystem.SerializeToString,
+            ),
+            'ListNvmeSubsystems': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListNvmeSubsystems,
+                    request_deserializer=frontend__nvme__pb2.ListNvmeSubsystemsRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.ListNvmeSubsystemsResponse.SerializeToString,
+            ),
+            'GetNvmeSubsystem': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetNvmeSubsystem,
+                    request_deserializer=frontend__nvme__pb2.GetNvmeSubsystemRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.NvmeSubsystem.SerializeToString,
+            ),
+            'StatsNvmeSubsystem': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsNvmeSubsystem,
+                    request_deserializer=frontend__nvme__pb2.StatsNvmeSubsystemRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.StatsNvmeSubsystemResponse.SerializeToString,
+            ),
+            'CreateNvmeController': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateNvmeController,
+                    request_deserializer=frontend__nvme__pb2.CreateNvmeControllerRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.NvmeController.SerializeToString,
+            ),
+            'DeleteNvmeController': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteNvmeController,
+                    request_deserializer=frontend__nvme__pb2.DeleteNvmeControllerRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
-            'UpdateNVMeController': grpc.unary_unary_rpc_method_handler(
-                    servicer.UpdateNVMeController,
-                    request_deserializer=frontend__nvme__pcie__pb2.UpdateNVMeControllerRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeController.SerializeToString,
-            ),
-            'ListNVMeControllers': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListNVMeControllers,
-                    request_deserializer=frontend__nvme__pcie__pb2.ListNVMeControllersRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.ListNVMeControllersResponse.SerializeToString,
-            ),
-            'GetNVMeController': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNVMeController,
-                    request_deserializer=frontend__nvme__pcie__pb2.GetNVMeControllerRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeController.SerializeToString,
-            ),
-            'NVMeControllerStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.NVMeControllerStats,
-                    request_deserializer=frontend__nvme__pcie__pb2.NVMeControllerStatsRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeControllerStatsResponse.SerializeToString,
-            ),
-            'CreateNVMeNamespace': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateNVMeNamespace,
-                    request_deserializer=frontend__nvme__pcie__pb2.CreateNVMeNamespaceRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeNamespace.SerializeToString,
-            ),
-            'DeleteNVMeNamespace': grpc.unary_unary_rpc_method_handler(
-                    servicer.DeleteNVMeNamespace,
-                    request_deserializer=frontend__nvme__pcie__pb2.DeleteNVMeNamespaceRequest.FromString,
+            'UpdateNvmeController': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateNvmeController,
+                    request_deserializer=frontend__nvme__pb2.UpdateNvmeControllerRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.NvmeController.SerializeToString,
+            ),
+            'ListNvmeControllers': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListNvmeControllers,
+                    request_deserializer=frontend__nvme__pb2.ListNvmeControllersRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.ListNvmeControllersResponse.SerializeToString,
+            ),
+            'GetNvmeController': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetNvmeController,
+                    request_deserializer=frontend__nvme__pb2.GetNvmeControllerRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.NvmeController.SerializeToString,
+            ),
+            'StatsNvmeController': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsNvmeController,
+                    request_deserializer=frontend__nvme__pb2.StatsNvmeControllerRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.StatsNvmeControllerResponse.SerializeToString,
+            ),
+            'CreateNvmeNamespace': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateNvmeNamespace,
+                    request_deserializer=frontend__nvme__pb2.CreateNvmeNamespaceRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.NvmeNamespace.SerializeToString,
+            ),
+            'DeleteNvmeNamespace': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteNvmeNamespace,
+                    request_deserializer=frontend__nvme__pb2.DeleteNvmeNamespaceRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
-            'UpdateNVMeNamespace': grpc.unary_unary_rpc_method_handler(
-                    servicer.UpdateNVMeNamespace,
-                    request_deserializer=frontend__nvme__pcie__pb2.UpdateNVMeNamespaceRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeNamespace.SerializeToString,
-            ),
-            'ListNVMeNamespaces': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListNVMeNamespaces,
-                    request_deserializer=frontend__nvme__pcie__pb2.ListNVMeNamespacesRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.ListNVMeNamespacesResponse.SerializeToString,
-            ),
-            'GetNVMeNamespace': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNVMeNamespace,
-                    request_deserializer=frontend__nvme__pcie__pb2.GetNVMeNamespaceRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeNamespace.SerializeToString,
-            ),
-            'NVMeNamespaceStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.NVMeNamespaceStats,
-                    request_deserializer=frontend__nvme__pcie__pb2.NVMeNamespaceStatsRequest.FromString,
-                    response_serializer=frontend__nvme__pcie__pb2.NVMeNamespaceStatsResponse.SerializeToString,
+            'UpdateNvmeNamespace': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateNvmeNamespace,
+                    request_deserializer=frontend__nvme__pb2.UpdateNvmeNamespaceRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.NvmeNamespace.SerializeToString,
+            ),
+            'ListNvmeNamespaces': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListNvmeNamespaces,
+                    request_deserializer=frontend__nvme__pb2.ListNvmeNamespacesRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.ListNvmeNamespacesResponse.SerializeToString,
+            ),
+            'GetNvmeNamespace': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetNvmeNamespace,
+                    request_deserializer=frontend__nvme__pb2.GetNvmeNamespaceRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.NvmeNamespace.SerializeToString,
+            ),
+            'StatsNvmeNamespace': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsNvmeNamespace,
+                    request_deserializer=frontend__nvme__pb2.StatsNvmeNamespaceRequest.FromString,
+                    response_serializer=frontend__nvme__pb2.StatsNvmeNamespaceResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'opi_api.storage.v1.FrontendNvmeService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class FrontendNvmeService(object):
-    """Front End (host-facing) APIs. Mostly used for NVMe/PCIe emulation and host presentation.
+    """Front End APIs. Used for creation of xPU managed Nvme devices
+    e.g. emulated host-facing Nvme/Pcie controllers as well as
+    Nvme-oF controllers
     """
 
     @staticmethod
-    def CreateNVMeSubsystem(request,
+    def CreateNvmeSubsystem(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/CreateNVMeSubsystem',
-            frontend__nvme__pcie__pb2.CreateNVMeSubsystemRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeSubsystem.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/CreateNvmeSubsystem',
+            frontend__nvme__pb2.CreateNvmeSubsystemRequest.SerializeToString,
+            frontend__nvme__pb2.NvmeSubsystem.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteNVMeSubsystem(request,
+    def DeleteNvmeSubsystem(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/DeleteNVMeSubsystem',
-            frontend__nvme__pcie__pb2.DeleteNVMeSubsystemRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/DeleteNvmeSubsystem',
+            frontend__nvme__pb2.DeleteNvmeSubsystemRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UpdateNVMeSubsystem(request,
+    def UpdateNvmeSubsystem(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/UpdateNVMeSubsystem',
-            frontend__nvme__pcie__pb2.UpdateNVMeSubsystemRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeSubsystem.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/UpdateNvmeSubsystem',
+            frontend__nvme__pb2.UpdateNvmeSubsystemRequest.SerializeToString,
+            frontend__nvme__pb2.NvmeSubsystem.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListNVMeSubsystems(request,
+    def ListNvmeSubsystems(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/ListNVMeSubsystems',
-            frontend__nvme__pcie__pb2.ListNVMeSubsystemsRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.ListNVMeSubsystemsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/ListNvmeSubsystems',
+            frontend__nvme__pb2.ListNvmeSubsystemsRequest.SerializeToString,
+            frontend__nvme__pb2.ListNvmeSubsystemsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetNVMeSubsystem(request,
+    def GetNvmeSubsystem(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/GetNVMeSubsystem',
-            frontend__nvme__pcie__pb2.GetNVMeSubsystemRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeSubsystem.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/GetNvmeSubsystem',
+            frontend__nvme__pb2.GetNvmeSubsystemRequest.SerializeToString,
+            frontend__nvme__pb2.NvmeSubsystem.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def NVMeSubsystemStats(request,
+    def StatsNvmeSubsystem(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/NVMeSubsystemStats',
-            frontend__nvme__pcie__pb2.NVMeSubsystemStatsRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeSubsystemStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/StatsNvmeSubsystem',
+            frontend__nvme__pb2.StatsNvmeSubsystemRequest.SerializeToString,
+            frontend__nvme__pb2.StatsNvmeSubsystemResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateNVMeController(request,
+    def CreateNvmeController(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/CreateNVMeController',
-            frontend__nvme__pcie__pb2.CreateNVMeControllerRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeController.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/CreateNvmeController',
+            frontend__nvme__pb2.CreateNvmeControllerRequest.SerializeToString,
+            frontend__nvme__pb2.NvmeController.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteNVMeController(request,
+    def DeleteNvmeController(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/DeleteNVMeController',
-            frontend__nvme__pcie__pb2.DeleteNVMeControllerRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/DeleteNvmeController',
+            frontend__nvme__pb2.DeleteNvmeControllerRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UpdateNVMeController(request,
+    def UpdateNvmeController(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/UpdateNVMeController',
-            frontend__nvme__pcie__pb2.UpdateNVMeControllerRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeController.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/UpdateNvmeController',
+            frontend__nvme__pb2.UpdateNvmeControllerRequest.SerializeToString,
+            frontend__nvme__pb2.NvmeController.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListNVMeControllers(request,
+    def ListNvmeControllers(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/ListNVMeControllers',
-            frontend__nvme__pcie__pb2.ListNVMeControllersRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.ListNVMeControllersResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/ListNvmeControllers',
+            frontend__nvme__pb2.ListNvmeControllersRequest.SerializeToString,
+            frontend__nvme__pb2.ListNvmeControllersResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetNVMeController(request,
+    def GetNvmeController(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/GetNVMeController',
-            frontend__nvme__pcie__pb2.GetNVMeControllerRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeController.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/GetNvmeController',
+            frontend__nvme__pb2.GetNvmeControllerRequest.SerializeToString,
+            frontend__nvme__pb2.NvmeController.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def NVMeControllerStats(request,
+    def StatsNvmeController(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/NVMeControllerStats',
-            frontend__nvme__pcie__pb2.NVMeControllerStatsRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeControllerStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/StatsNvmeController',
+            frontend__nvme__pb2.StatsNvmeControllerRequest.SerializeToString,
+            frontend__nvme__pb2.StatsNvmeControllerResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateNVMeNamespace(request,
+    def CreateNvmeNamespace(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/CreateNVMeNamespace',
-            frontend__nvme__pcie__pb2.CreateNVMeNamespaceRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeNamespace.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/CreateNvmeNamespace',
+            frontend__nvme__pb2.CreateNvmeNamespaceRequest.SerializeToString,
+            frontend__nvme__pb2.NvmeNamespace.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteNVMeNamespace(request,
+    def DeleteNvmeNamespace(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/DeleteNVMeNamespace',
-            frontend__nvme__pcie__pb2.DeleteNVMeNamespaceRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/DeleteNvmeNamespace',
+            frontend__nvme__pb2.DeleteNvmeNamespaceRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UpdateNVMeNamespace(request,
+    def UpdateNvmeNamespace(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/UpdateNVMeNamespace',
-            frontend__nvme__pcie__pb2.UpdateNVMeNamespaceRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeNamespace.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/UpdateNvmeNamespace',
+            frontend__nvme__pb2.UpdateNvmeNamespaceRequest.SerializeToString,
+            frontend__nvme__pb2.NvmeNamespace.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListNVMeNamespaces(request,
+    def ListNvmeNamespaces(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/ListNVMeNamespaces',
-            frontend__nvme__pcie__pb2.ListNVMeNamespacesRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.ListNVMeNamespacesResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/ListNvmeNamespaces',
+            frontend__nvme__pb2.ListNvmeNamespacesRequest.SerializeToString,
+            frontend__nvme__pb2.ListNvmeNamespacesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetNVMeNamespace(request,
+    def GetNvmeNamespace(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/GetNVMeNamespace',
-            frontend__nvme__pcie__pb2.GetNVMeNamespaceRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeNamespace.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/GetNvmeNamespace',
+            frontend__nvme__pb2.GetNvmeNamespaceRequest.SerializeToString,
+            frontend__nvme__pb2.NvmeNamespace.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def NVMeNamespaceStats(request,
+    def StatsNvmeNamespace(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/NVMeNamespaceStats',
-            frontend__nvme__pcie__pb2.NVMeNamespaceStatsRequest.SerializeToString,
-            frontend__nvme__pcie__pb2.NVMeNamespaceStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendNvmeService/StatsNvmeNamespace',
+            frontend__nvme__pb2.StatsNvmeNamespaceRequest.SerializeToString,
+            frontend__nvme__pb2.StatsNvmeNamespaceResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_blk_pb2_grpc.py` & `pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_blk_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,57 +37,63 @@
                 response_deserializer=frontend__virtio__blk__pb2.ListVirtioBlksResponse.FromString,
                 )
         self.GetVirtioBlk = channel.unary_unary(
                 '/opi_api.storage.v1.FrontendVirtioBlkService/GetVirtioBlk',
                 request_serializer=frontend__virtio__blk__pb2.GetVirtioBlkRequest.SerializeToString,
                 response_deserializer=frontend__virtio__blk__pb2.VirtioBlk.FromString,
                 )
-        self.VirtioBlkStats = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendVirtioBlkService/VirtioBlkStats',
-                request_serializer=frontend__virtio__blk__pb2.VirtioBlkStatsRequest.SerializeToString,
-                response_deserializer=frontend__virtio__blk__pb2.VirtioBlkStatsResponse.FromString,
+        self.StatsVirtioBlk = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendVirtioBlkService/StatsVirtioBlk',
+                request_serializer=frontend__virtio__blk__pb2.StatsVirtioBlkRequest.SerializeToString,
+                response_deserializer=frontend__virtio__blk__pb2.StatsVirtioBlkResponse.FromString,
                 )
 
 
 class FrontendVirtioBlkServiceServicer(object):
     """Front End (host-facing) APIs. Mostly used for Virtio-blk emulation emulation and host presentation as alternative to Nvme.
     """
 
     def CreateVirtioBlk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Create an Virtio Blk
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteVirtioBlk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Delete an Virtio Blk
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateVirtioBlk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Update an Virtio Blk
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListVirtioBlks(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """List Virtio Blks
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetVirtioBlk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Get an Virtio Blk
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def VirtioBlkStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsVirtioBlk(self, request, context):
+        """Get an Virtio Blk statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_FrontendVirtioBlkServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -112,18 +118,18 @@
                     response_serializer=frontend__virtio__blk__pb2.ListVirtioBlksResponse.SerializeToString,
             ),
             'GetVirtioBlk': grpc.unary_unary_rpc_method_handler(
                     servicer.GetVirtioBlk,
                     request_deserializer=frontend__virtio__blk__pb2.GetVirtioBlkRequest.FromString,
                     response_serializer=frontend__virtio__blk__pb2.VirtioBlk.SerializeToString,
             ),
-            'VirtioBlkStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.VirtioBlkStats,
-                    request_deserializer=frontend__virtio__blk__pb2.VirtioBlkStatsRequest.FromString,
-                    response_serializer=frontend__virtio__blk__pb2.VirtioBlkStatsResponse.SerializeToString,
+            'StatsVirtioBlk': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsVirtioBlk,
+                    request_deserializer=frontend__virtio__blk__pb2.StatsVirtioBlkRequest.FromString,
+                    response_serializer=frontend__virtio__blk__pb2.StatsVirtioBlkResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'opi_api.storage.v1.FrontendVirtioBlkService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -214,22 +220,22 @@
         return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioBlkService/GetVirtioBlk',
             frontend__virtio__blk__pb2.GetVirtioBlkRequest.SerializeToString,
             frontend__virtio__blk__pb2.VirtioBlk.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def VirtioBlkStats(request,
+    def StatsVirtioBlk(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioBlkService/VirtioBlkStats',
-            frontend__virtio__blk__pb2.VirtioBlkStatsRequest.SerializeToString,
-            frontend__virtio__blk__pb2.VirtioBlkStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioBlkService/StatsVirtioBlk',
+            frontend__virtio__blk__pb2.StatsVirtioBlkRequest.SerializeToString,
+            frontend__virtio__blk__pb2.StatsVirtioBlkResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_fs_pb2.py` & `pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_fs_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: frontend_virtio_fs.proto
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x66rontend_virtio_fs.proto\x12\x12opi_api.storage.v1Bd\n\x12opi_api.storage.v1B\x15\x46rontendVirtioFsProtoP\x01Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/gob\x06proto3')
 
-
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'frontend_virtio_fs_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\022opi_api.storage.v1B\025FrontendVirtioFsProtoP\001Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/go'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\022opi_api.storage.v1B\025FrontendVirtioFsProtoP\001Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/go'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_scsi_pb2.py` & `pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_scsi_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,366 +1,222 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: frontend_virtio_scsi.proto
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 import opicommon_pb2 as opicommon__pb2
-import object_key_pb2 as object__key__pb2
 from google.api import client_pb2 as google_dot_api_dot_client__pb2
 from google.api import resource_pb2 as google_dot_api_dot_resource__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66rontend_virtio_scsi.proto\x12\x12opi_api.storage.v1\x1a\x0fopicommon.proto\x1a\x10object_key.proto\x1a\x17google/api/client.proto\x1a\x19google/api/resource.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a google/protobuf/field_mask.proto\"N\n\x10VirtioScsiTarget\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\x12\x10\n\x08max_luns\x18\x02 \x01(\x05\"r\n\x14VirtioScsiController\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\x12\x30\n\x07pcie_id\x18\x02 \x01(\x0b\x32\x1f.opi_api.storage.v1.PciEndpoint\"\x9b\x01\n\rVirtioScsiLun\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\x12/\n\ttarget_id\x18\x02 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\x12/\n\tvolume_id\x18\x03 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\"\xc2\x01\n\x1d\x43reateVirtioScsiTargetRequest\x12;\n\x06parent\x18\x01 \x01(\tB+\xe0\x41\x02\xfa\x41%\n#opi_api.storage.v1/VirtioScsiTarget\x12\x45\n\x12virtio_scsi_target\x18\x02 \x01(\x0b\x32$.opi_api.storage.v1.VirtioScsiTargetB\x03\xe0\x41\x02\x12\x1d\n\x15virtio_scsi_target_id\x18\x03 \x01(\t\"Z\n\x1d\x44\x65leteVirtioScsiTargetRequest\x12\x39\n\x04name\x18\x01 \x01(\tB+\xe0\x41\x02\xfa\x41%\n#opi_api.storage.v1/VirtioScsiTarget\"\x92\x01\n\x1dUpdateVirtioScsiTargetRequest\x12@\n\x12virtio_scsi_target\x18\x01 \x01(\x0b\x32$.opi_api.storage.v1.VirtioScsiTarget\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x82\x01\n\x1cListVirtioScsiTargetsRequest\x12;\n\x06parent\x18\x01 \x01(\tB+\xe0\x41\x02\xfa\x41%\n#opi_api.storage.v1/VirtioScsiTarget\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"{\n\x1dListVirtioScsiTargetsResponse\x12\x41\n\x13virtio_scsi_targets\x18\x01 \x03(\x0b\x32$.opi_api.storage.v1.VirtioScsiTarget\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"W\n\x1aGetVirtioScsiTargetRequest\x12\x39\n\x04name\x18\x01 \x01(\tB+\xe0\x41\x02\xfa\x41%\n#opi_api.storage.v1/VirtioScsiTarget\"O\n\x1cVirtioScsiTargetStatsRequest\x12/\n\ttarget_id\x18\x01 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\"y\n\x1dVirtioScsiTargetStatsResponse\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\x12.\n\x05stats\x18\x02 \x01(\x0b\x32\x1f.opi_api.storage.v1.VolumeStats\"\xd6\x01\n!CreateVirtioScsiControllerRequest\x12?\n\x06parent\x18\x01 \x01(\tB/\xe0\x41\x02\xfa\x41)\n\'opi_api.storage.v1/VirtioScsiController\x12M\n\x16virtio_scsi_controller\x18\x02 \x01(\x0b\x32(.opi_api.storage.v1.VirtioScsiControllerB\x03\xe0\x41\x02\x12!\n\x19virtio_scsi_controller_id\x18\x03 \x01(\t\"b\n!DeleteVirtioScsiControllerRequest\x12=\n\x04name\x18\x01 \x01(\tB/\xe0\x41\x02\xfa\x41)\n\'opi_api.storage.v1/VirtioScsiController\"\x9e\x01\n!UpdateVirtioScsiControllerRequest\x12H\n\x16virtio_scsi_controller\x18\x01 \x01(\x0b\x32(.opi_api.storage.v1.VirtioScsiController\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x8a\x01\n ListVirtioScsiControllersRequest\x12?\n\x06parent\x18\x01 \x01(\tB/\xe0\x41\x02\xfa\x41)\n\'opi_api.storage.v1/VirtioScsiController\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"\x87\x01\n!ListVirtioScsiControllersResponse\x12I\n\x17virtio_scsi_controllers\x18\x01 \x03(\x0b\x32(.opi_api.storage.v1.VirtioScsiController\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"_\n\x1eGetVirtioScsiControllerRequest\x12=\n\x04name\x18\x01 \x01(\tB/\xe0\x41\x02\xfa\x41)\n\'opi_api.storage.v1/VirtioScsiController\"W\n VirtioScsiControllerStatsRequest\x12\x33\n\rcontroller_id\x18\x01 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\"}\n!VirtioScsiControllerStatsResponse\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\x12.\n\x05stats\x18\x02 \x01(\x0b\x32\x1f.opi_api.storage.v1.VolumeStats\"\xb3\x01\n\x1a\x43reateVirtioScsiLunRequest\x12\x38\n\x06parent\x18\x01 \x01(\tB(\xe0\x41\x02\xfa\x41\"\n opi_api.storage.v1/VirtioScsiLun\x12?\n\x0fvirtio_scsi_lun\x18\x02 \x01(\x0b\x32!.opi_api.storage.v1.VirtioScsiLunB\x03\xe0\x41\x02\x12\x1a\n\x12virtio_scsi_lun_id\x18\x03 \x01(\t\"T\n\x1a\x44\x65leteVirtioScsiLunRequest\x12\x36\n\x04name\x18\x01 \x01(\tB(\xe0\x41\x02\xfa\x41\"\n opi_api.storage.v1/VirtioScsiLun\"\x89\x01\n\x1aUpdateVirtioScsiLunRequest\x12:\n\x0fvirtio_scsi_lun\x18\x01 \x01(\x0b\x32!.opi_api.storage.v1.VirtioScsiLun\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"|\n\x19ListVirtioScsiLunsRequest\x12\x38\n\x06parent\x18\x01 \x01(\tB(\xe0\x41\x02\xfa\x41\"\n opi_api.storage.v1/VirtioScsiLun\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"r\n\x1aListVirtioScsiLunsResponse\x12;\n\x10virtio_scsi_luns\x18\x01 \x03(\x0b\x32!.opi_api.storage.v1.VirtioScsiLun\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"Q\n\x17GetVirtioScsiLunRequest\x12\x36\n\x04name\x18\x01 \x01(\tB(\xe0\x41\x02\xfa\x41\"\n opi_api.storage.v1/VirtioScsiLun\"~\n\x19VirtioScsiLunStatsRequest\x12\x33\n\rcontroller_id\x18\x01 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\x12,\n\x06lun_id\x18\x02 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\"v\n\x1aVirtioScsiLunStatsResponse\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.opi_api.common.v1.ObjectKey\x12.\n\x05stats\x18\x02 \x01(\x0b\x32\x1f.opi_api.storage.v1.VolumeStats2\xa1\x19\n\x19\x46rontendVirtioScsiService\x12\xd8\x01\n\x16\x43reateVirtioScsiTarget\x12\x31.opi_api.storage.v1.CreateVirtioScsiTargetRequest\x1a$.opi_api.storage.v1.VirtioScsiTarget\"e\x82\xd3\xe4\x93\x02-\"\x17/v1/{parent=subsystems}:\x12virtio_scsi_target\xda\x41/parent,virtio_scsi_target,virtio_scsi_target_id\x12\x9c\x01\n\x16\x44\x65leteVirtioScsiTarget\x12\x31.opi_api.storage.v1.DeleteVirtioScsiTargetRequest\x1a\x16.google.protobuf.Empty\"7\x82\xd3\xe4\x93\x02**(/v1/{name=subsystems}/{virtioscsitarget}\xda\x41\x04name\x12\xd8\x01\n\x16UpdateVirtioScsiTarget\x12\x31.opi_api.storage.v1.UpdateVirtioScsiTargetRequest\x1a$.opi_api.storage.v1.VirtioScsiTarget\"e\x82\xd3\xe4\x93\x02>2(/v1/{virtio_scsi_target.name=subsystems}:\x12virtio_scsi_target\xda\x41\x1evirtio_scsi_target,update_mask\x12\xa6\x01\n\x15ListVirtioScsiTargets\x12\x30.opi_api.storage.v1.ListVirtioScsiTargetsRequest\x1a\x31.opi_api.storage.v1.ListVirtioScsiTargetsResponse\"(\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/{parent=subsystems}\xda\x41\x06parent\x12\xa4\x01\n\x13GetVirtioScsiTarget\x12..opi_api.storage.v1.GetVirtioScsiTargetRequest\x1a$.opi_api.storage.v1.VirtioScsiTarget\"7\x82\xd3\xe4\x93\x02*\x12(/v1/{name=subsystems}/{virtioscsitarget}\xda\x41\x04name\x12~\n\x15VirtioScsiTargetStats\x12\x30.opi_api.storage.v1.VirtioScsiTargetStatsRequest\x1a\x31.opi_api.storage.v1.VirtioScsiTargetStatsResponse\"\x00\x12\xf0\x01\n\x1a\x43reateVirtioScsiController\x12\x35.opi_api.storage.v1.CreateVirtioScsiControllerRequest\x1a(.opi_api.storage.v1.VirtioScsiController\"q\x82\xd3\xe4\x93\x02\x31\"\x17/v1/{parent=subsystems}:\x16virtio_scsi_controller\xda\x41\x37parent,virtio_scsi_controller,virtio_scsi_controller_id\x12\xa7\x01\n\x1a\x44\x65leteVirtioScsiController\x12\x35.opi_api.storage.v1.DeleteVirtioScsiControllerRequest\x1a\x16.google.protobuf.Empty\":\x82\xd3\xe4\x93\x02-*+/v1/{name=virtioscsictrls}/{virtioscsictrl}\xda\x41\x04name\x12\xf0\x01\n\x1aUpdateVirtioScsiController\x12\x35.opi_api.storage.v1.UpdateVirtioScsiControllerRequest\x1a(.opi_api.storage.v1.VirtioScsiController\"q\x82\xd3\xe4\x93\x02\x46\x32,/v1/{virtio_scsi_controller.name=subsystems}:\x16virtio_scsi_controller\xda\x41\"virtio_scsi_controller,update_mask\x12\xb2\x01\n\x19ListVirtioScsiControllers\x12\x34.opi_api.storage.v1.ListVirtioScsiControllersRequest\x1a\x35.opi_api.storage.v1.ListVirtioScsiControllersResponse\"(\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/{parent=subsystems}\xda\x41\x06parent\x12\xae\x01\n\x17GetVirtioScsiController\x12\x32.opi_api.storage.v1.GetVirtioScsiControllerRequest\x1a(.opi_api.storage.v1.VirtioScsiController\"5\x82\xd3\xe4\x93\x02(\x12&/v1/{name=subsystems}/{virtioscsictrl}\xda\x41\x04name\x12\x8a\x01\n\x19VirtioScsiControllerStats\x12\x34.opi_api.storage.v1.VirtioScsiControllerStatsRequest\x1a\x35.opi_api.storage.v1.VirtioScsiControllerStatsResponse\"\x00\x12\xc6\x01\n\x13\x43reateVirtioScsiLun\x12..opi_api.storage.v1.CreateVirtioScsiLunRequest\x1a!.opi_api.storage.v1.VirtioScsiLun\"\\\x82\xd3\xe4\x93\x02*\"\x17/v1/{parent=subsystems}:\x0fvirtio_scsi_lun\xda\x41)parent,virtio_scsi_lun,virtio_scsi_lun_id\x12\x97\x01\n\x13\x44\x65leteVirtioScsiLun\x12..opi_api.storage.v1.DeleteVirtioScsiLunRequest\x1a\x16.google.protobuf.Empty\"8\x82\xd3\xe4\x93\x02+*)/v1/{name=virtioscsiluns}/{virtioscsilun}\xda\x41\x04name\x12\xc6\x01\n\x13UpdateVirtioScsiLun\x12..opi_api.storage.v1.UpdateVirtioScsiLunRequest\x1a!.opi_api.storage.v1.VirtioScsiLun\"\\\x82\xd3\xe4\x93\x02\x38\x32%/v1/{virtio_scsi_lun.name=subsystems}:\x0fvirtio_scsi_lun\xda\x41\x1bvirtio_scsi_lun,update_mask\x12\x9d\x01\n\x12ListVirtioScsiLuns\x12-.opi_api.storage.v1.ListVirtioScsiLunsRequest\x1a..opi_api.storage.v1.ListVirtioScsiLunsResponse\"(\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/{parent=subsystems}\xda\x41\x06parent\x12\x98\x01\n\x10GetVirtioScsiLun\x12+.opi_api.storage.v1.GetVirtioScsiLunRequest\x1a!.opi_api.storage.v1.VirtioScsiLun\"4\x82\xd3\xe4\x93\x02\'\x12%/v1/{name=subsystems}/{virtioscsilun}\xda\x41\x04name\x12u\n\x12VirtioScsiLunStats\x12-.opi_api.storage.v1.VirtioScsiLunStatsRequest\x1a..opi_api.storage.v1.VirtioScsiLunStatsResponse\"\x00\x42\x66\n\x12opi_api.storage.v1B\x17\x46rontendVirtioScsiProtoP\x01Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/gob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66rontend_virtio_scsi.proto\x12\x12opi_api.storage.v1\x1a\x0fopicommon.proto\x1a\x17google/api/client.proto\x1a\x19google/api/resource.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a google/protobuf/field_mask.proto\"\xb8\x01\n\x10VirtioScsiTarget\x12\x18\n\x04name\x18\x01 \x01(\tB\x04\xe2\x41\x01\x08R\x04name\x12\x1f\n\x08max_luns\x18\x02 \x01(\x05\x42\x04\xe2\x41\x01\x01R\x07maxLuns:i\xea\x41\x66\n#opi_api.storage.v1/VirtioScsiTarget\x12\x1avirtioScsiTargets/{volume}*\x11virtioScsiTargets2\x10virtioScsiTarget\"\xed\x02\n\x14VirtioScsiController\x12\x18\n\x04name\x18\x01 \x01(\tB\x04\xe2\x41\x01\x08R\x04name\x12>\n\x07pcie_id\x18\x02 \x01(\x0b\x32\x1f.opi_api.storage.v1.PciEndpointB\x04\xe2\x41\x01\x02R\x06pcieId\x12?\n\tmin_limit\x18\x03 \x01(\x0b\x32\x1c.opi_api.storage.v1.QosLimitB\x04\xe2\x41\x01\x01R\x08minLimit\x12?\n\tmax_limit\x18\x04 \x01(\x0b\x32\x1c.opi_api.storage.v1.QosLimitB\x04\xe2\x41\x01\x01R\x08maxLimit:y\xea\x41v\n\'opi_api.storage.v1/VirtioScsiController\x12\x1evirtioScsiControllers/{volume}*\x15virtioScsiControllers2\x14virtioScsiController\"\xe4\x01\n\rVirtioScsiLun\x12\x18\n\x04name\x18\x01 \x01(\tB\x04\xe2\x41\x01\x08R\x04name\x12,\n\x0ftarget_name_ref\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\rtargetNameRef\x12,\n\x0fvolume_name_ref\x18\x03 \x01(\tB\x04\xe2\x41\x01\x02R\rvolumeNameRef:]\xea\x41Z\n opi_api.storage.v1/VirtioScsiLun\x12\x17virtioScsiLuns/{volume}*\x0evirtioScsiLuns2\rvirtioScsiLun\"\xb2\x01\n\x1d\x43reateVirtioScsiTargetRequest\x12X\n\x12virtio_scsi_target\x18\x01 \x01(\x0b\x32$.opi_api.storage.v1.VirtioScsiTargetB\x04\xe2\x41\x01\x02R\x10virtioScsiTarget\x12\x37\n\x15virtio_scsi_target_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x01R\x12virtioScsiTargetId\"\x8c\x01\n\x1d\x44\x65leteVirtioScsiTargetRequest\x12@\n\x04name\x18\x01 \x01(\tB,\xe2\x41\x01\x02\xfa\x41%\n#opi_api.storage.v1/VirtioScsiTargetR\x04name\x12)\n\rallow_missing\x18\x02 \x01(\x08\x42\x04\xe2\x41\x01\x01R\x0c\x61llowMissing\"\xe7\x01\n\x1dUpdateVirtioScsiTargetRequest\x12X\n\x12virtio_scsi_target\x18\x01 \x01(\x0b\x32$.opi_api.storage.v1.VirtioScsiTargetB\x04\xe2\x41\x01\x02R\x10virtioScsiTarget\x12\x41\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskB\x04\xe2\x41\x01\x01R\nupdateMask\x12)\n\rallow_missing\x18\x03 \x01(\x08\x42\x04\xe2\x41\x01\x01R\x0c\x61llowMissing\"\xac\x01\n\x1cListVirtioScsiTargetsRequest\x12\x44\n\x06parent\x18\x01 \x01(\tB,\xe2\x41\x01\x02\xfa\x41%\x12#opi_api.storage.v1/VirtioScsiTargetR\x06parent\x12!\n\tpage_size\x18\x02 \x01(\x05\x42\x04\xe2\x41\x01\x01R\x08pageSize\x12#\n\npage_token\x18\x03 \x01(\tB\x04\xe2\x41\x01\x01R\tpageToken\"\x9d\x01\n\x1dListVirtioScsiTargetsResponse\x12T\n\x13virtio_scsi_targets\x18\x01 \x03(\x0b\x32$.opi_api.storage.v1.VirtioScsiTargetR\x11virtioScsiTargets\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\"^\n\x1aGetVirtioScsiTargetRequest\x12@\n\x04name\x18\x01 \x01(\tB,\xe2\x41\x01\x02\xfa\x41%\n#opi_api.storage.v1/VirtioScsiTargetR\x04name\"`\n\x1cStatsVirtioScsiTargetRequest\x12@\n\x04name\x18\x01 \x01(\tB,\xe2\x41\x01\x02\xfa\x41%\n#opi_api.storage.v1/VirtioScsiTargetR\x04name\"V\n\x1dStatsVirtioScsiTargetResponse\x12\x35\n\x05stats\x18\x01 \x01(\x0b\x32\x1f.opi_api.storage.v1.VolumeStatsR\x05stats\"\xca\x01\n!CreateVirtioScsiControllerRequest\x12\x64\n\x16virtio_scsi_controller\x18\x01 \x01(\x0b\x32(.opi_api.storage.v1.VirtioScsiControllerB\x04\xe2\x41\x01\x02R\x14virtioScsiController\x12?\n\x19virtio_scsi_controller_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x01R\x16virtioScsiControllerId\"\x94\x01\n!DeleteVirtioScsiControllerRequest\x12\x44\n\x04name\x18\x01 \x01(\tB0\xe2\x41\x01\x02\xfa\x41)\n\'opi_api.storage.v1/VirtioScsiControllerR\x04name\x12)\n\rallow_missing\x18\x02 \x01(\x08\x42\x04\xe2\x41\x01\x01R\x0c\x61llowMissing\"\xf7\x01\n!UpdateVirtioScsiControllerRequest\x12\x64\n\x16virtio_scsi_controller\x18\x01 \x01(\x0b\x32(.opi_api.storage.v1.VirtioScsiControllerB\x04\xe2\x41\x01\x02R\x14virtioScsiController\x12\x41\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskB\x04\xe2\x41\x01\x01R\nupdateMask\x12)\n\rallow_missing\x18\x03 \x01(\x08\x42\x04\xe2\x41\x01\x01R\x0c\x61llowMissing\"\xb4\x01\n ListVirtioScsiControllersRequest\x12H\n\x06parent\x18\x01 \x01(\tB0\xe2\x41\x01\x02\xfa\x41)\x12\'opi_api.storage.v1/VirtioScsiControllerR\x06parent\x12!\n\tpage_size\x18\x02 \x01(\x05\x42\x04\xe2\x41\x01\x01R\x08pageSize\x12#\n\npage_token\x18\x03 \x01(\tB\x04\xe2\x41\x01\x01R\tpageToken\"\xad\x01\n!ListVirtioScsiControllersResponse\x12`\n\x17virtio_scsi_controllers\x18\x01 \x03(\x0b\x32(.opi_api.storage.v1.VirtioScsiControllerR\x15virtioScsiControllers\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\"f\n\x1eGetVirtioScsiControllerRequest\x12\x44\n\x04name\x18\x01 \x01(\tB0\xe2\x41\x01\x02\xfa\x41)\n\'opi_api.storage.v1/VirtioScsiControllerR\x04name\"h\n StatsVirtioScsiControllerRequest\x12\x44\n\x04name\x18\x01 \x01(\tB0\xe2\x41\x01\x02\xfa\x41)\n\'opi_api.storage.v1/VirtioScsiControllerR\x04name\"Z\n!StatsVirtioScsiControllerResponse\x12\x35\n\x05stats\x18\x01 \x01(\x0b\x32\x1f.opi_api.storage.v1.VolumeStatsR\x05stats\"\xa0\x01\n\x1a\x43reateVirtioScsiLunRequest\x12O\n\x0fvirtio_scsi_lun\x18\x01 \x01(\x0b\x32!.opi_api.storage.v1.VirtioScsiLunB\x04\xe2\x41\x01\x02R\rvirtioScsiLun\x12\x31\n\x12virtio_scsi_lun_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x01R\x0fvirtioScsiLunId\"\x86\x01\n\x1a\x44\x65leteVirtioScsiLunRequest\x12=\n\x04name\x18\x01 \x01(\tB)\xe2\x41\x01\x02\xfa\x41\"\n opi_api.storage.v1/VirtioScsiLunR\x04name\x12)\n\rallow_missing\x18\x02 \x01(\x08\x42\x04\xe2\x41\x01\x01R\x0c\x61llowMissing\"\xdb\x01\n\x1aUpdateVirtioScsiLunRequest\x12O\n\x0fvirtio_scsi_lun\x18\x01 \x01(\x0b\x32!.opi_api.storage.v1.VirtioScsiLunB\x04\xe2\x41\x01\x02R\rvirtioScsiLun\x12\x41\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskB\x04\xe2\x41\x01\x01R\nupdateMask\x12)\n\rallow_missing\x18\x03 \x01(\x08\x42\x04\xe2\x41\x01\x01R\x0c\x61llowMissing\"\xa6\x01\n\x19ListVirtioScsiLunsRequest\x12\x41\n\x06parent\x18\x01 \x01(\tB)\xe2\x41\x01\x02\xfa\x41\"\x12 opi_api.storage.v1/VirtioScsiLunR\x06parent\x12!\n\tpage_size\x18\x02 \x01(\x05\x42\x04\xe2\x41\x01\x01R\x08pageSize\x12#\n\npage_token\x18\x03 \x01(\tB\x04\xe2\x41\x01\x01R\tpageToken\"\x91\x01\n\x1aListVirtioScsiLunsResponse\x12K\n\x10virtio_scsi_luns\x18\x01 \x03(\x0b\x32!.opi_api.storage.v1.VirtioScsiLunR\x0evirtioScsiLuns\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\"X\n\x17GetVirtioScsiLunRequest\x12=\n\x04name\x18\x01 \x01(\tB)\xe2\x41\x01\x02\xfa\x41\"\n opi_api.storage.v1/VirtioScsiLunR\x04name\"\x90\x01\n\x19StatsVirtioScsiLunRequest\x12=\n\x04name\x18\x01 \x01(\tB)\xe2\x41\x01\x02\xfa\x41\"\n opi_api.storage.v1/VirtioScsiLunR\x04name\x12\x34\n\x13\x63ontroller_name_ref\x18\x02 \x01(\tB\x04\xe2\x41\x01\x01R\x11\x63ontrollerNameRef\"S\n\x1aStatsVirtioScsiLunResponse\x12\x35\n\x05stats\x18\x01 \x01(\x0b\x32\x1f.opi_api.storage.v1.VolumeStatsR\x05stats2\x9c\x1a\n\x19\x46rontendVirtioScsiService\x12\xcf\x01\n\x16\x43reateVirtioScsiTarget\x12\x31.opi_api.storage.v1.CreateVirtioScsiTargetRequest\x1a$.opi_api.storage.v1.VirtioScsiTarget\"\\\xda\x41(virtio_scsi_target,virtio_scsi_target_id\x82\xd3\xe4\x93\x02+\"\x15/v1/virtioScsiTargets:\x12virtio_scsi_target\x12\x92\x01\n\x16\x44\x65leteVirtioScsiTarget\x12\x31.opi_api.storage.v1.DeleteVirtioScsiTargetRequest\x1a\x16.google.protobuf.Empty\"-\xda\x41\x04name\x82\xd3\xe4\x93\x02 *\x1e/v1/{name=virtioScsiTargets/*}\x12\xe1\x01\n\x16UpdateVirtioScsiTarget\x12\x31.opi_api.storage.v1.UpdateVirtioScsiTargetRequest\x1a$.opi_api.storage.v1.VirtioScsiTarget\"n\xda\x41\x1evirtio_scsi_target,update_mask\x82\xd3\xe4\x93\x02G21/v1/{virtio_scsi_target.name=virtioScsiTargets/*}:\x12virtio_scsi_target\x12\xad\x01\n\x15ListVirtioScsiTargets\x12\x30.opi_api.storage.v1.ListVirtioScsiTargetsRequest\x1a\x31.opi_api.storage.v1.ListVirtioScsiTargetsResponse\"/\xda\x41\x06parent\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{parent=virtioScsiTargets}\x12\x9a\x01\n\x13GetVirtioScsiTarget\x12..opi_api.storage.v1.GetVirtioScsiTargetRequest\x1a$.opi_api.storage.v1.VirtioScsiTarget\"-\xda\x41\x04name\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=virtioScsiTargets/*}\x12\xb1\x01\n\x15StatsVirtioScsiTarget\x12\x30.opi_api.storage.v1.StatsVirtioScsiTargetRequest\x1a\x31.opi_api.storage.v1.StatsVirtioScsiTargetResponse\"3\xda\x41\x04name\x82\xd3\xe4\x93\x02&\x12$/v1/{name=virtioScsiTargets/*}:stats\x12\xeb\x01\n\x1a\x43reateVirtioScsiController\x12\x35.opi_api.storage.v1.CreateVirtioScsiControllerRequest\x1a(.opi_api.storage.v1.VirtioScsiController\"l\xda\x41\x30virtio_scsi_controller,virtio_scsi_controller_id\x82\xd3\xe4\x93\x02\x33\"\x19/v1/virtioScsiControllers:\x16virtio_scsi_controller\x12\x9e\x01\n\x1a\x44\x65leteVirtioScsiController\x12\x35.opi_api.storage.v1.DeleteVirtioScsiControllerRequest\x1a\x16.google.protobuf.Empty\"1\xda\x41\x04name\x82\xd3\xe4\x93\x02$*\"/v1/{name=virtioScsiControllers/*}\x12\xfd\x01\n\x1aUpdateVirtioScsiController\x12\x35.opi_api.storage.v1.UpdateVirtioScsiControllerRequest\x1a(.opi_api.storage.v1.VirtioScsiController\"~\xda\x41\"virtio_scsi_controller,update_mask\x82\xd3\xe4\x93\x02S29/v1/{virtio_scsi_controller.name=virtioScsiControllers/*}:\x16virtio_scsi_controller\x12\xbd\x01\n\x19ListVirtioScsiControllers\x12\x34.opi_api.storage.v1.ListVirtioScsiControllersRequest\x1a\x35.opi_api.storage.v1.ListVirtioScsiControllersResponse\"3\xda\x41\x06parent\x82\xd3\xe4\x93\x02$\x12\"/v1/{parent=virtioScsiControllers}\x12\xaa\x01\n\x17GetVirtioScsiController\x12\x32.opi_api.storage.v1.GetVirtioScsiControllerRequest\x1a(.opi_api.storage.v1.VirtioScsiController\"1\xda\x41\x04name\x82\xd3\xe4\x93\x02$\x12\"/v1/{name=virtioScsiControllers/*}\x12\xc1\x01\n\x19StatsVirtioScsiController\x12\x34.opi_api.storage.v1.StatsVirtioScsiControllerRequest\x1a\x35.opi_api.storage.v1.StatsVirtioScsiControllerResponse\"7\xda\x41\x04name\x82\xd3\xe4\x93\x02*\x12(/v1/{name=virtioScsiControllers/*}:stats\x12\xba\x01\n\x13\x43reateVirtioScsiLun\x12..opi_api.storage.v1.CreateVirtioScsiLunRequest\x1a!.opi_api.storage.v1.VirtioScsiLun\"P\xda\x41\"virtio_scsi_lun,virtio_scsi_lun_id\x82\xd3\xe4\x93\x02%\"\x12/v1/virtioScsiLuns:\x0fvirtio_scsi_lun\x12\x89\x01\n\x13\x44\x65leteVirtioScsiLun\x12..opi_api.storage.v1.DeleteVirtioScsiLunRequest\x1a\x16.google.protobuf.Empty\"*\xda\x41\x04name\x82\xd3\xe4\x93\x02\x1d*\x1b/v1/{name=virtioScsiLuns/*}\x12\xcc\x01\n\x13UpdateVirtioScsiLun\x12..opi_api.storage.v1.UpdateVirtioScsiLunRequest\x1a!.opi_api.storage.v1.VirtioScsiLun\"b\xda\x41\x1bvirtio_scsi_lun,update_mask\x82\xd3\xe4\x93\x02>2+/v1/{virtio_scsi_lun.name=virtioScsiLuns/*}:\x0fvirtio_scsi_lun\x12\xa1\x01\n\x12ListVirtioScsiLuns\x12-.opi_api.storage.v1.ListVirtioScsiLunsRequest\x1a..opi_api.storage.v1.ListVirtioScsiLunsResponse\",\xda\x41\x06parent\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/{parent=virtioScsiLuns}\x12\x8e\x01\n\x10GetVirtioScsiLun\x12+.opi_api.storage.v1.GetVirtioScsiLunRequest\x1a!.opi_api.storage.v1.VirtioScsiLun\"*\xda\x41\x04name\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/{name=virtioScsiLuns/*}\x12\xa5\x01\n\x12StatsVirtioScsiLun\x12-.opi_api.storage.v1.StatsVirtioScsiLunRequest\x1a..opi_api.storage.v1.StatsVirtioScsiLunResponse\"0\xda\x41\x04name\x82\xd3\xe4\x93\x02#\x12!/v1/{name=virtioScsiLuns/*}:statsBf\n\x12opi_api.storage.v1B\x17\x46rontendVirtioScsiProtoP\x01Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/gob\x06proto3')
 
-
-
-_VIRTIOSCSITARGET = DESCRIPTOR.message_types_by_name['VirtioScsiTarget']
-_VIRTIOSCSICONTROLLER = DESCRIPTOR.message_types_by_name['VirtioScsiController']
-_VIRTIOSCSILUN = DESCRIPTOR.message_types_by_name['VirtioScsiLun']
-_CREATEVIRTIOSCSITARGETREQUEST = DESCRIPTOR.message_types_by_name['CreateVirtioScsiTargetRequest']
-_DELETEVIRTIOSCSITARGETREQUEST = DESCRIPTOR.message_types_by_name['DeleteVirtioScsiTargetRequest']
-_UPDATEVIRTIOSCSITARGETREQUEST = DESCRIPTOR.message_types_by_name['UpdateVirtioScsiTargetRequest']
-_LISTVIRTIOSCSITARGETSREQUEST = DESCRIPTOR.message_types_by_name['ListVirtioScsiTargetsRequest']
-_LISTVIRTIOSCSITARGETSRESPONSE = DESCRIPTOR.message_types_by_name['ListVirtioScsiTargetsResponse']
-_GETVIRTIOSCSITARGETREQUEST = DESCRIPTOR.message_types_by_name['GetVirtioScsiTargetRequest']
-_VIRTIOSCSITARGETSTATSREQUEST = DESCRIPTOR.message_types_by_name['VirtioScsiTargetStatsRequest']
-_VIRTIOSCSITARGETSTATSRESPONSE = DESCRIPTOR.message_types_by_name['VirtioScsiTargetStatsResponse']
-_CREATEVIRTIOSCSICONTROLLERREQUEST = DESCRIPTOR.message_types_by_name['CreateVirtioScsiControllerRequest']
-_DELETEVIRTIOSCSICONTROLLERREQUEST = DESCRIPTOR.message_types_by_name['DeleteVirtioScsiControllerRequest']
-_UPDATEVIRTIOSCSICONTROLLERREQUEST = DESCRIPTOR.message_types_by_name['UpdateVirtioScsiControllerRequest']
-_LISTVIRTIOSCSICONTROLLERSREQUEST = DESCRIPTOR.message_types_by_name['ListVirtioScsiControllersRequest']
-_LISTVIRTIOSCSICONTROLLERSRESPONSE = DESCRIPTOR.message_types_by_name['ListVirtioScsiControllersResponse']
-_GETVIRTIOSCSICONTROLLERREQUEST = DESCRIPTOR.message_types_by_name['GetVirtioScsiControllerRequest']
-_VIRTIOSCSICONTROLLERSTATSREQUEST = DESCRIPTOR.message_types_by_name['VirtioScsiControllerStatsRequest']
-_VIRTIOSCSICONTROLLERSTATSRESPONSE = DESCRIPTOR.message_types_by_name['VirtioScsiControllerStatsResponse']
-_CREATEVIRTIOSCSILUNREQUEST = DESCRIPTOR.message_types_by_name['CreateVirtioScsiLunRequest']
-_DELETEVIRTIOSCSILUNREQUEST = DESCRIPTOR.message_types_by_name['DeleteVirtioScsiLunRequest']
-_UPDATEVIRTIOSCSILUNREQUEST = DESCRIPTOR.message_types_by_name['UpdateVirtioScsiLunRequest']
-_LISTVIRTIOSCSILUNSREQUEST = DESCRIPTOR.message_types_by_name['ListVirtioScsiLunsRequest']
-_LISTVIRTIOSCSILUNSRESPONSE = DESCRIPTOR.message_types_by_name['ListVirtioScsiLunsResponse']
-_GETVIRTIOSCSILUNREQUEST = DESCRIPTOR.message_types_by_name['GetVirtioScsiLunRequest']
-_VIRTIOSCSILUNSTATSREQUEST = DESCRIPTOR.message_types_by_name['VirtioScsiLunStatsRequest']
-_VIRTIOSCSILUNSTATSRESPONSE = DESCRIPTOR.message_types_by_name['VirtioScsiLunStatsResponse']
-VirtioScsiTarget = _reflection.GeneratedProtocolMessageType('VirtioScsiTarget', (_message.Message,), {
-  'DESCRIPTOR' : _VIRTIOSCSITARGET,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.VirtioScsiTarget)
-  })
-_sym_db.RegisterMessage(VirtioScsiTarget)
-
-VirtioScsiController = _reflection.GeneratedProtocolMessageType('VirtioScsiController', (_message.Message,), {
-  'DESCRIPTOR' : _VIRTIOSCSICONTROLLER,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.VirtioScsiController)
-  })
-_sym_db.RegisterMessage(VirtioScsiController)
-
-VirtioScsiLun = _reflection.GeneratedProtocolMessageType('VirtioScsiLun', (_message.Message,), {
-  'DESCRIPTOR' : _VIRTIOSCSILUN,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.VirtioScsiLun)
-  })
-_sym_db.RegisterMessage(VirtioScsiLun)
-
-CreateVirtioScsiTargetRequest = _reflection.GeneratedProtocolMessageType('CreateVirtioScsiTargetRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEVIRTIOSCSITARGETREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.CreateVirtioScsiTargetRequest)
-  })
-_sym_db.RegisterMessage(CreateVirtioScsiTargetRequest)
-
-DeleteVirtioScsiTargetRequest = _reflection.GeneratedProtocolMessageType('DeleteVirtioScsiTargetRequest', (_message.Message,), {
-  'DESCRIPTOR' : _DELETEVIRTIOSCSITARGETREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.DeleteVirtioScsiTargetRequest)
-  })
-_sym_db.RegisterMessage(DeleteVirtioScsiTargetRequest)
-
-UpdateVirtioScsiTargetRequest = _reflection.GeneratedProtocolMessageType('UpdateVirtioScsiTargetRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UPDATEVIRTIOSCSITARGETREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.UpdateVirtioScsiTargetRequest)
-  })
-_sym_db.RegisterMessage(UpdateVirtioScsiTargetRequest)
-
-ListVirtioScsiTargetsRequest = _reflection.GeneratedProtocolMessageType('ListVirtioScsiTargetsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _LISTVIRTIOSCSITARGETSREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.ListVirtioScsiTargetsRequest)
-  })
-_sym_db.RegisterMessage(ListVirtioScsiTargetsRequest)
-
-ListVirtioScsiTargetsResponse = _reflection.GeneratedProtocolMessageType('ListVirtioScsiTargetsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _LISTVIRTIOSCSITARGETSRESPONSE,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.ListVirtioScsiTargetsResponse)
-  })
-_sym_db.RegisterMessage(ListVirtioScsiTargetsResponse)
-
-GetVirtioScsiTargetRequest = _reflection.GeneratedProtocolMessageType('GetVirtioScsiTargetRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETVIRTIOSCSITARGETREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.GetVirtioScsiTargetRequest)
-  })
-_sym_db.RegisterMessage(GetVirtioScsiTargetRequest)
-
-VirtioScsiTargetStatsRequest = _reflection.GeneratedProtocolMessageType('VirtioScsiTargetStatsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _VIRTIOSCSITARGETSTATSREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.VirtioScsiTargetStatsRequest)
-  })
-_sym_db.RegisterMessage(VirtioScsiTargetStatsRequest)
-
-VirtioScsiTargetStatsResponse = _reflection.GeneratedProtocolMessageType('VirtioScsiTargetStatsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _VIRTIOSCSITARGETSTATSRESPONSE,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.VirtioScsiTargetStatsResponse)
-  })
-_sym_db.RegisterMessage(VirtioScsiTargetStatsResponse)
-
-CreateVirtioScsiControllerRequest = _reflection.GeneratedProtocolMessageType('CreateVirtioScsiControllerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEVIRTIOSCSICONTROLLERREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.CreateVirtioScsiControllerRequest)
-  })
-_sym_db.RegisterMessage(CreateVirtioScsiControllerRequest)
-
-DeleteVirtioScsiControllerRequest = _reflection.GeneratedProtocolMessageType('DeleteVirtioScsiControllerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _DELETEVIRTIOSCSICONTROLLERREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.DeleteVirtioScsiControllerRequest)
-  })
-_sym_db.RegisterMessage(DeleteVirtioScsiControllerRequest)
-
-UpdateVirtioScsiControllerRequest = _reflection.GeneratedProtocolMessageType('UpdateVirtioScsiControllerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UPDATEVIRTIOSCSICONTROLLERREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.UpdateVirtioScsiControllerRequest)
-  })
-_sym_db.RegisterMessage(UpdateVirtioScsiControllerRequest)
-
-ListVirtioScsiControllersRequest = _reflection.GeneratedProtocolMessageType('ListVirtioScsiControllersRequest', (_message.Message,), {
-  'DESCRIPTOR' : _LISTVIRTIOSCSICONTROLLERSREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.ListVirtioScsiControllersRequest)
-  })
-_sym_db.RegisterMessage(ListVirtioScsiControllersRequest)
-
-ListVirtioScsiControllersResponse = _reflection.GeneratedProtocolMessageType('ListVirtioScsiControllersResponse', (_message.Message,), {
-  'DESCRIPTOR' : _LISTVIRTIOSCSICONTROLLERSRESPONSE,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.ListVirtioScsiControllersResponse)
-  })
-_sym_db.RegisterMessage(ListVirtioScsiControllersResponse)
-
-GetVirtioScsiControllerRequest = _reflection.GeneratedProtocolMessageType('GetVirtioScsiControllerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETVIRTIOSCSICONTROLLERREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.GetVirtioScsiControllerRequest)
-  })
-_sym_db.RegisterMessage(GetVirtioScsiControllerRequest)
-
-VirtioScsiControllerStatsRequest = _reflection.GeneratedProtocolMessageType('VirtioScsiControllerStatsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _VIRTIOSCSICONTROLLERSTATSREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.VirtioScsiControllerStatsRequest)
-  })
-_sym_db.RegisterMessage(VirtioScsiControllerStatsRequest)
-
-VirtioScsiControllerStatsResponse = _reflection.GeneratedProtocolMessageType('VirtioScsiControllerStatsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _VIRTIOSCSICONTROLLERSTATSRESPONSE,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.VirtioScsiControllerStatsResponse)
-  })
-_sym_db.RegisterMessage(VirtioScsiControllerStatsResponse)
-
-CreateVirtioScsiLunRequest = _reflection.GeneratedProtocolMessageType('CreateVirtioScsiLunRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEVIRTIOSCSILUNREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.CreateVirtioScsiLunRequest)
-  })
-_sym_db.RegisterMessage(CreateVirtioScsiLunRequest)
-
-DeleteVirtioScsiLunRequest = _reflection.GeneratedProtocolMessageType('DeleteVirtioScsiLunRequest', (_message.Message,), {
-  'DESCRIPTOR' : _DELETEVIRTIOSCSILUNREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.DeleteVirtioScsiLunRequest)
-  })
-_sym_db.RegisterMessage(DeleteVirtioScsiLunRequest)
-
-UpdateVirtioScsiLunRequest = _reflection.GeneratedProtocolMessageType('UpdateVirtioScsiLunRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UPDATEVIRTIOSCSILUNREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.UpdateVirtioScsiLunRequest)
-  })
-_sym_db.RegisterMessage(UpdateVirtioScsiLunRequest)
-
-ListVirtioScsiLunsRequest = _reflection.GeneratedProtocolMessageType('ListVirtioScsiLunsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _LISTVIRTIOSCSILUNSREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.ListVirtioScsiLunsRequest)
-  })
-_sym_db.RegisterMessage(ListVirtioScsiLunsRequest)
-
-ListVirtioScsiLunsResponse = _reflection.GeneratedProtocolMessageType('ListVirtioScsiLunsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _LISTVIRTIOSCSILUNSRESPONSE,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.ListVirtioScsiLunsResponse)
-  })
-_sym_db.RegisterMessage(ListVirtioScsiLunsResponse)
-
-GetVirtioScsiLunRequest = _reflection.GeneratedProtocolMessageType('GetVirtioScsiLunRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETVIRTIOSCSILUNREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.GetVirtioScsiLunRequest)
-  })
-_sym_db.RegisterMessage(GetVirtioScsiLunRequest)
-
-VirtioScsiLunStatsRequest = _reflection.GeneratedProtocolMessageType('VirtioScsiLunStatsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _VIRTIOSCSILUNSTATSREQUEST,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.VirtioScsiLunStatsRequest)
-  })
-_sym_db.RegisterMessage(VirtioScsiLunStatsRequest)
-
-VirtioScsiLunStatsResponse = _reflection.GeneratedProtocolMessageType('VirtioScsiLunStatsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _VIRTIOSCSILUNSTATSRESPONSE,
-  '__module__' : 'frontend_virtio_scsi_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.storage.v1.VirtioScsiLunStatsResponse)
-  })
-_sym_db.RegisterMessage(VirtioScsiLunStatsResponse)
-
-_FRONTENDVIRTIOSCSISERVICE = DESCRIPTOR.services_by_name['FrontendVirtioScsiService']
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'frontend_virtio_scsi_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\022opi_api.storage.v1B\027FrontendVirtioScsiProtoP\001Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/go'
-  _CREATEVIRTIOSCSITARGETREQUEST.fields_by_name['parent']._options = None
-  _CREATEVIRTIOSCSITARGETREQUEST.fields_by_name['parent']._serialized_options = b'\340A\002\372A%\n#opi_api.storage.v1/VirtioScsiTarget'
-  _CREATEVIRTIOSCSITARGETREQUEST.fields_by_name['virtio_scsi_target']._options = None
-  _CREATEVIRTIOSCSITARGETREQUEST.fields_by_name['virtio_scsi_target']._serialized_options = b'\340A\002'
-  _DELETEVIRTIOSCSITARGETREQUEST.fields_by_name['name']._options = None
-  _DELETEVIRTIOSCSITARGETREQUEST.fields_by_name['name']._serialized_options = b'\340A\002\372A%\n#opi_api.storage.v1/VirtioScsiTarget'
-  _LISTVIRTIOSCSITARGETSREQUEST.fields_by_name['parent']._options = None
-  _LISTVIRTIOSCSITARGETSREQUEST.fields_by_name['parent']._serialized_options = b'\340A\002\372A%\n#opi_api.storage.v1/VirtioScsiTarget'
-  _GETVIRTIOSCSITARGETREQUEST.fields_by_name['name']._options = None
-  _GETVIRTIOSCSITARGETREQUEST.fields_by_name['name']._serialized_options = b'\340A\002\372A%\n#opi_api.storage.v1/VirtioScsiTarget'
-  _CREATEVIRTIOSCSICONTROLLERREQUEST.fields_by_name['parent']._options = None
-  _CREATEVIRTIOSCSICONTROLLERREQUEST.fields_by_name['parent']._serialized_options = b'\340A\002\372A)\n\'opi_api.storage.v1/VirtioScsiController'
-  _CREATEVIRTIOSCSICONTROLLERREQUEST.fields_by_name['virtio_scsi_controller']._options = None
-  _CREATEVIRTIOSCSICONTROLLERREQUEST.fields_by_name['virtio_scsi_controller']._serialized_options = b'\340A\002'
-  _DELETEVIRTIOSCSICONTROLLERREQUEST.fields_by_name['name']._options = None
-  _DELETEVIRTIOSCSICONTROLLERREQUEST.fields_by_name['name']._serialized_options = b'\340A\002\372A)\n\'opi_api.storage.v1/VirtioScsiController'
-  _LISTVIRTIOSCSICONTROLLERSREQUEST.fields_by_name['parent']._options = None
-  _LISTVIRTIOSCSICONTROLLERSREQUEST.fields_by_name['parent']._serialized_options = b'\340A\002\372A)\n\'opi_api.storage.v1/VirtioScsiController'
-  _GETVIRTIOSCSICONTROLLERREQUEST.fields_by_name['name']._options = None
-  _GETVIRTIOSCSICONTROLLERREQUEST.fields_by_name['name']._serialized_options = b'\340A\002\372A)\n\'opi_api.storage.v1/VirtioScsiController'
-  _CREATEVIRTIOSCSILUNREQUEST.fields_by_name['parent']._options = None
-  _CREATEVIRTIOSCSILUNREQUEST.fields_by_name['parent']._serialized_options = b'\340A\002\372A\"\n opi_api.storage.v1/VirtioScsiLun'
-  _CREATEVIRTIOSCSILUNREQUEST.fields_by_name['virtio_scsi_lun']._options = None
-  _CREATEVIRTIOSCSILUNREQUEST.fields_by_name['virtio_scsi_lun']._serialized_options = b'\340A\002'
-  _DELETEVIRTIOSCSILUNREQUEST.fields_by_name['name']._options = None
-  _DELETEVIRTIOSCSILUNREQUEST.fields_by_name['name']._serialized_options = b'\340A\002\372A\"\n opi_api.storage.v1/VirtioScsiLun'
-  _LISTVIRTIOSCSILUNSREQUEST.fields_by_name['parent']._options = None
-  _LISTVIRTIOSCSILUNSREQUEST.fields_by_name['parent']._serialized_options = b'\340A\002\372A\"\n opi_api.storage.v1/VirtioScsiLun'
-  _GETVIRTIOSCSILUNREQUEST.fields_by_name['name']._options = None
-  _GETVIRTIOSCSILUNREQUEST.fields_by_name['name']._serialized_options = b'\340A\002\372A\"\n opi_api.storage.v1/VirtioScsiLun'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['CreateVirtioScsiTarget']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['CreateVirtioScsiTarget']._serialized_options = b'\202\323\344\223\002-\"\027/v1/{parent=subsystems}:\022virtio_scsi_target\332A/parent,virtio_scsi_target,virtio_scsi_target_id'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['DeleteVirtioScsiTarget']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['DeleteVirtioScsiTarget']._serialized_options = b'\202\323\344\223\002**(/v1/{name=subsystems}/{virtioscsitarget}\332A\004name'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['UpdateVirtioScsiTarget']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['UpdateVirtioScsiTarget']._serialized_options = b'\202\323\344\223\002>2(/v1/{virtio_scsi_target.name=subsystems}:\022virtio_scsi_target\332A\036virtio_scsi_target,update_mask'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['ListVirtioScsiTargets']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['ListVirtioScsiTargets']._serialized_options = b'\202\323\344\223\002\031\022\027/v1/{parent=subsystems}\332A\006parent'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['GetVirtioScsiTarget']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['GetVirtioScsiTarget']._serialized_options = b'\202\323\344\223\002*\022(/v1/{name=subsystems}/{virtioscsitarget}\332A\004name'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['CreateVirtioScsiController']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['CreateVirtioScsiController']._serialized_options = b'\202\323\344\223\0021\"\027/v1/{parent=subsystems}:\026virtio_scsi_controller\332A7parent,virtio_scsi_controller,virtio_scsi_controller_id'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['DeleteVirtioScsiController']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['DeleteVirtioScsiController']._serialized_options = b'\202\323\344\223\002-*+/v1/{name=virtioscsictrls}/{virtioscsictrl}\332A\004name'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['UpdateVirtioScsiController']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['UpdateVirtioScsiController']._serialized_options = b'\202\323\344\223\002F2,/v1/{virtio_scsi_controller.name=subsystems}:\026virtio_scsi_controller\332A\"virtio_scsi_controller,update_mask'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['ListVirtioScsiControllers']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['ListVirtioScsiControllers']._serialized_options = b'\202\323\344\223\002\031\022\027/v1/{parent=subsystems}\332A\006parent'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['GetVirtioScsiController']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['GetVirtioScsiController']._serialized_options = b'\202\323\344\223\002(\022&/v1/{name=subsystems}/{virtioscsictrl}\332A\004name'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['CreateVirtioScsiLun']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['CreateVirtioScsiLun']._serialized_options = b'\202\323\344\223\002*\"\027/v1/{parent=subsystems}:\017virtio_scsi_lun\332A)parent,virtio_scsi_lun,virtio_scsi_lun_id'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['DeleteVirtioScsiLun']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['DeleteVirtioScsiLun']._serialized_options = b'\202\323\344\223\002+*)/v1/{name=virtioscsiluns}/{virtioscsilun}\332A\004name'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['UpdateVirtioScsiLun']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['UpdateVirtioScsiLun']._serialized_options = b'\202\323\344\223\00282%/v1/{virtio_scsi_lun.name=subsystems}:\017virtio_scsi_lun\332A\033virtio_scsi_lun,update_mask'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['ListVirtioScsiLuns']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['ListVirtioScsiLuns']._serialized_options = b'\202\323\344\223\002\031\022\027/v1/{parent=subsystems}\332A\006parent'
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['GetVirtioScsiLun']._options = None
-  _FRONTENDVIRTIOSCSISERVICE.methods_by_name['GetVirtioScsiLun']._serialized_options = b'\202\323\344\223\002\'\022%/v1/{name=subsystems}/{virtioscsilun}\332A\004name'
-  _VIRTIOSCSITARGET._serialized_start=263
-  _VIRTIOSCSITARGET._serialized_end=341
-  _VIRTIOSCSICONTROLLER._serialized_start=343
-  _VIRTIOSCSICONTROLLER._serialized_end=457
-  _VIRTIOSCSILUN._serialized_start=460
-  _VIRTIOSCSILUN._serialized_end=615
-  _CREATEVIRTIOSCSITARGETREQUEST._serialized_start=618
-  _CREATEVIRTIOSCSITARGETREQUEST._serialized_end=812
-  _DELETEVIRTIOSCSITARGETREQUEST._serialized_start=814
-  _DELETEVIRTIOSCSITARGETREQUEST._serialized_end=904
-  _UPDATEVIRTIOSCSITARGETREQUEST._serialized_start=907
-  _UPDATEVIRTIOSCSITARGETREQUEST._serialized_end=1053
-  _LISTVIRTIOSCSITARGETSREQUEST._serialized_start=1056
-  _LISTVIRTIOSCSITARGETSREQUEST._serialized_end=1186
-  _LISTVIRTIOSCSITARGETSRESPONSE._serialized_start=1188
-  _LISTVIRTIOSCSITARGETSRESPONSE._serialized_end=1311
-  _GETVIRTIOSCSITARGETREQUEST._serialized_start=1313
-  _GETVIRTIOSCSITARGETREQUEST._serialized_end=1400
-  _VIRTIOSCSITARGETSTATSREQUEST._serialized_start=1402
-  _VIRTIOSCSITARGETSTATSREQUEST._serialized_end=1481
-  _VIRTIOSCSITARGETSTATSRESPONSE._serialized_start=1483
-  _VIRTIOSCSITARGETSTATSRESPONSE._serialized_end=1604
-  _CREATEVIRTIOSCSICONTROLLERREQUEST._serialized_start=1607
-  _CREATEVIRTIOSCSICONTROLLERREQUEST._serialized_end=1821
-  _DELETEVIRTIOSCSICONTROLLERREQUEST._serialized_start=1823
-  _DELETEVIRTIOSCSICONTROLLERREQUEST._serialized_end=1921
-  _UPDATEVIRTIOSCSICONTROLLERREQUEST._serialized_start=1924
-  _UPDATEVIRTIOSCSICONTROLLERREQUEST._serialized_end=2082
-  _LISTVIRTIOSCSICONTROLLERSREQUEST._serialized_start=2085
-  _LISTVIRTIOSCSICONTROLLERSREQUEST._serialized_end=2223
-  _LISTVIRTIOSCSICONTROLLERSRESPONSE._serialized_start=2226
-  _LISTVIRTIOSCSICONTROLLERSRESPONSE._serialized_end=2361
-  _GETVIRTIOSCSICONTROLLERREQUEST._serialized_start=2363
-  _GETVIRTIOSCSICONTROLLERREQUEST._serialized_end=2458
-  _VIRTIOSCSICONTROLLERSTATSREQUEST._serialized_start=2460
-  _VIRTIOSCSICONTROLLERSTATSREQUEST._serialized_end=2547
-  _VIRTIOSCSICONTROLLERSTATSRESPONSE._serialized_start=2549
-  _VIRTIOSCSICONTROLLERSTATSRESPONSE._serialized_end=2674
-  _CREATEVIRTIOSCSILUNREQUEST._serialized_start=2677
-  _CREATEVIRTIOSCSILUNREQUEST._serialized_end=2856
-  _DELETEVIRTIOSCSILUNREQUEST._serialized_start=2858
-  _DELETEVIRTIOSCSILUNREQUEST._serialized_end=2942
-  _UPDATEVIRTIOSCSILUNREQUEST._serialized_start=2945
-  _UPDATEVIRTIOSCSILUNREQUEST._serialized_end=3082
-  _LISTVIRTIOSCSILUNSREQUEST._serialized_start=3084
-  _LISTVIRTIOSCSILUNSREQUEST._serialized_end=3208
-  _LISTVIRTIOSCSILUNSRESPONSE._serialized_start=3210
-  _LISTVIRTIOSCSILUNSRESPONSE._serialized_end=3324
-  _GETVIRTIOSCSILUNREQUEST._serialized_start=3326
-  _GETVIRTIOSCSILUNREQUEST._serialized_end=3407
-  _VIRTIOSCSILUNSTATSREQUEST._serialized_start=3409
-  _VIRTIOSCSILUNSTATSREQUEST._serialized_end=3535
-  _VIRTIOSCSILUNSTATSRESPONSE._serialized_start=3537
-  _VIRTIOSCSILUNSTATSRESPONSE._serialized_end=3655
-  _FRONTENDVIRTIOSCSISERVICE._serialized_start=3658
-  _FRONTENDVIRTIOSCSISERVICE._serialized_end=6891
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\022opi_api.storage.v1B\027FrontendVirtioScsiProtoP\001Z5github.com/opiproject/opi-api/storage/v1alpha1/gen/go'
+  _globals['_VIRTIOSCSITARGET'].fields_by_name['name']._options = None
+  _globals['_VIRTIOSCSITARGET'].fields_by_name['name']._serialized_options = b'\342A\001\010'
+  _globals['_VIRTIOSCSITARGET'].fields_by_name['max_luns']._options = None
+  _globals['_VIRTIOSCSITARGET'].fields_by_name['max_luns']._serialized_options = b'\342A\001\001'
+  _globals['_VIRTIOSCSITARGET']._options = None
+  _globals['_VIRTIOSCSITARGET']._serialized_options = b'\352Af\n#opi_api.storage.v1/VirtioScsiTarget\022\032virtioScsiTargets/{volume}*\021virtioScsiTargets2\020virtioScsiTarget'
+  _globals['_VIRTIOSCSICONTROLLER'].fields_by_name['name']._options = None
+  _globals['_VIRTIOSCSICONTROLLER'].fields_by_name['name']._serialized_options = b'\342A\001\010'
+  _globals['_VIRTIOSCSICONTROLLER'].fields_by_name['pcie_id']._options = None
+  _globals['_VIRTIOSCSICONTROLLER'].fields_by_name['pcie_id']._serialized_options = b'\342A\001\002'
+  _globals['_VIRTIOSCSICONTROLLER'].fields_by_name['min_limit']._options = None
+  _globals['_VIRTIOSCSICONTROLLER'].fields_by_name['min_limit']._serialized_options = b'\342A\001\001'
+  _globals['_VIRTIOSCSICONTROLLER'].fields_by_name['max_limit']._options = None
+  _globals['_VIRTIOSCSICONTROLLER'].fields_by_name['max_limit']._serialized_options = b'\342A\001\001'
+  _globals['_VIRTIOSCSICONTROLLER']._options = None
+  _globals['_VIRTIOSCSICONTROLLER']._serialized_options = b'\352Av\n\'opi_api.storage.v1/VirtioScsiController\022\036virtioScsiControllers/{volume}*\025virtioScsiControllers2\024virtioScsiController'
+  _globals['_VIRTIOSCSILUN'].fields_by_name['name']._options = None
+  _globals['_VIRTIOSCSILUN'].fields_by_name['name']._serialized_options = b'\342A\001\010'
+  _globals['_VIRTIOSCSILUN'].fields_by_name['target_name_ref']._options = None
+  _globals['_VIRTIOSCSILUN'].fields_by_name['target_name_ref']._serialized_options = b'\342A\001\002'
+  _globals['_VIRTIOSCSILUN'].fields_by_name['volume_name_ref']._options = None
+  _globals['_VIRTIOSCSILUN'].fields_by_name['volume_name_ref']._serialized_options = b'\342A\001\002'
+  _globals['_VIRTIOSCSILUN']._options = None
+  _globals['_VIRTIOSCSILUN']._serialized_options = b'\352AZ\n opi_api.storage.v1/VirtioScsiLun\022\027virtioScsiLuns/{volume}*\016virtioScsiLuns2\rvirtioScsiLun'
+  _globals['_CREATEVIRTIOSCSITARGETREQUEST'].fields_by_name['virtio_scsi_target']._options = None
+  _globals['_CREATEVIRTIOSCSITARGETREQUEST'].fields_by_name['virtio_scsi_target']._serialized_options = b'\342A\001\002'
+  _globals['_CREATEVIRTIOSCSITARGETREQUEST'].fields_by_name['virtio_scsi_target_id']._options = None
+  _globals['_CREATEVIRTIOSCSITARGETREQUEST'].fields_by_name['virtio_scsi_target_id']._serialized_options = b'\342A\001\001'
+  _globals['_DELETEVIRTIOSCSITARGETREQUEST'].fields_by_name['name']._options = None
+  _globals['_DELETEVIRTIOSCSITARGETREQUEST'].fields_by_name['name']._serialized_options = b'\342A\001\002\372A%\n#opi_api.storage.v1/VirtioScsiTarget'
+  _globals['_DELETEVIRTIOSCSITARGETREQUEST'].fields_by_name['allow_missing']._options = None
+  _globals['_DELETEVIRTIOSCSITARGETREQUEST'].fields_by_name['allow_missing']._serialized_options = b'\342A\001\001'
+  _globals['_UPDATEVIRTIOSCSITARGETREQUEST'].fields_by_name['virtio_scsi_target']._options = None
+  _globals['_UPDATEVIRTIOSCSITARGETREQUEST'].fields_by_name['virtio_scsi_target']._serialized_options = b'\342A\001\002'
+  _globals['_UPDATEVIRTIOSCSITARGETREQUEST'].fields_by_name['update_mask']._options = None
+  _globals['_UPDATEVIRTIOSCSITARGETREQUEST'].fields_by_name['update_mask']._serialized_options = b'\342A\001\001'
+  _globals['_UPDATEVIRTIOSCSITARGETREQUEST'].fields_by_name['allow_missing']._options = None
+  _globals['_UPDATEVIRTIOSCSITARGETREQUEST'].fields_by_name['allow_missing']._serialized_options = b'\342A\001\001'
+  _globals['_LISTVIRTIOSCSITARGETSREQUEST'].fields_by_name['parent']._options = None
+  _globals['_LISTVIRTIOSCSITARGETSREQUEST'].fields_by_name['parent']._serialized_options = b'\342A\001\002\372A%\022#opi_api.storage.v1/VirtioScsiTarget'
+  _globals['_LISTVIRTIOSCSITARGETSREQUEST'].fields_by_name['page_size']._options = None
+  _globals['_LISTVIRTIOSCSITARGETSREQUEST'].fields_by_name['page_size']._serialized_options = b'\342A\001\001'
+  _globals['_LISTVIRTIOSCSITARGETSREQUEST'].fields_by_name['page_token']._options = None
+  _globals['_LISTVIRTIOSCSITARGETSREQUEST'].fields_by_name['page_token']._serialized_options = b'\342A\001\001'
+  _globals['_GETVIRTIOSCSITARGETREQUEST'].fields_by_name['name']._options = None
+  _globals['_GETVIRTIOSCSITARGETREQUEST'].fields_by_name['name']._serialized_options = b'\342A\001\002\372A%\n#opi_api.storage.v1/VirtioScsiTarget'
+  _globals['_STATSVIRTIOSCSITARGETREQUEST'].fields_by_name['name']._options = None
+  _globals['_STATSVIRTIOSCSITARGETREQUEST'].fields_by_name['name']._serialized_options = b'\342A\001\002\372A%\n#opi_api.storage.v1/VirtioScsiTarget'
+  _globals['_CREATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['virtio_scsi_controller']._options = None
+  _globals['_CREATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['virtio_scsi_controller']._serialized_options = b'\342A\001\002'
+  _globals['_CREATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['virtio_scsi_controller_id']._options = None
+  _globals['_CREATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['virtio_scsi_controller_id']._serialized_options = b'\342A\001\001'
+  _globals['_DELETEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['name']._options = None
+  _globals['_DELETEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['name']._serialized_options = b'\342A\001\002\372A)\n\'opi_api.storage.v1/VirtioScsiController'
+  _globals['_DELETEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['allow_missing']._options = None
+  _globals['_DELETEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['allow_missing']._serialized_options = b'\342A\001\001'
+  _globals['_UPDATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['virtio_scsi_controller']._options = None
+  _globals['_UPDATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['virtio_scsi_controller']._serialized_options = b'\342A\001\002'
+  _globals['_UPDATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['update_mask']._options = None
+  _globals['_UPDATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['update_mask']._serialized_options = b'\342A\001\001'
+  _globals['_UPDATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['allow_missing']._options = None
+  _globals['_UPDATEVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['allow_missing']._serialized_options = b'\342A\001\001'
+  _globals['_LISTVIRTIOSCSICONTROLLERSREQUEST'].fields_by_name['parent']._options = None
+  _globals['_LISTVIRTIOSCSICONTROLLERSREQUEST'].fields_by_name['parent']._serialized_options = b'\342A\001\002\372A)\022\'opi_api.storage.v1/VirtioScsiController'
+  _globals['_LISTVIRTIOSCSICONTROLLERSREQUEST'].fields_by_name['page_size']._options = None
+  _globals['_LISTVIRTIOSCSICONTROLLERSREQUEST'].fields_by_name['page_size']._serialized_options = b'\342A\001\001'
+  _globals['_LISTVIRTIOSCSICONTROLLERSREQUEST'].fields_by_name['page_token']._options = None
+  _globals['_LISTVIRTIOSCSICONTROLLERSREQUEST'].fields_by_name['page_token']._serialized_options = b'\342A\001\001'
+  _globals['_GETVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['name']._options = None
+  _globals['_GETVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['name']._serialized_options = b'\342A\001\002\372A)\n\'opi_api.storage.v1/VirtioScsiController'
+  _globals['_STATSVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['name']._options = None
+  _globals['_STATSVIRTIOSCSICONTROLLERREQUEST'].fields_by_name['name']._serialized_options = b'\342A\001\002\372A)\n\'opi_api.storage.v1/VirtioScsiController'
+  _globals['_CREATEVIRTIOSCSILUNREQUEST'].fields_by_name['virtio_scsi_lun']._options = None
+  _globals['_CREATEVIRTIOSCSILUNREQUEST'].fields_by_name['virtio_scsi_lun']._serialized_options = b'\342A\001\002'
+  _globals['_CREATEVIRTIOSCSILUNREQUEST'].fields_by_name['virtio_scsi_lun_id']._options = None
+  _globals['_CREATEVIRTIOSCSILUNREQUEST'].fields_by_name['virtio_scsi_lun_id']._serialized_options = b'\342A\001\001'
+  _globals['_DELETEVIRTIOSCSILUNREQUEST'].fields_by_name['name']._options = None
+  _globals['_DELETEVIRTIOSCSILUNREQUEST'].fields_by_name['name']._serialized_options = b'\342A\001\002\372A\"\n opi_api.storage.v1/VirtioScsiLun'
+  _globals['_DELETEVIRTIOSCSILUNREQUEST'].fields_by_name['allow_missing']._options = None
+  _globals['_DELETEVIRTIOSCSILUNREQUEST'].fields_by_name['allow_missing']._serialized_options = b'\342A\001\001'
+  _globals['_UPDATEVIRTIOSCSILUNREQUEST'].fields_by_name['virtio_scsi_lun']._options = None
+  _globals['_UPDATEVIRTIOSCSILUNREQUEST'].fields_by_name['virtio_scsi_lun']._serialized_options = b'\342A\001\002'
+  _globals['_UPDATEVIRTIOSCSILUNREQUEST'].fields_by_name['update_mask']._options = None
+  _globals['_UPDATEVIRTIOSCSILUNREQUEST'].fields_by_name['update_mask']._serialized_options = b'\342A\001\001'
+  _globals['_UPDATEVIRTIOSCSILUNREQUEST'].fields_by_name['allow_missing']._options = None
+  _globals['_UPDATEVIRTIOSCSILUNREQUEST'].fields_by_name['allow_missing']._serialized_options = b'\342A\001\001'
+  _globals['_LISTVIRTIOSCSILUNSREQUEST'].fields_by_name['parent']._options = None
+  _globals['_LISTVIRTIOSCSILUNSREQUEST'].fields_by_name['parent']._serialized_options = b'\342A\001\002\372A\"\022 opi_api.storage.v1/VirtioScsiLun'
+  _globals['_LISTVIRTIOSCSILUNSREQUEST'].fields_by_name['page_size']._options = None
+  _globals['_LISTVIRTIOSCSILUNSREQUEST'].fields_by_name['page_size']._serialized_options = b'\342A\001\001'
+  _globals['_LISTVIRTIOSCSILUNSREQUEST'].fields_by_name['page_token']._options = None
+  _globals['_LISTVIRTIOSCSILUNSREQUEST'].fields_by_name['page_token']._serialized_options = b'\342A\001\001'
+  _globals['_GETVIRTIOSCSILUNREQUEST'].fields_by_name['name']._options = None
+  _globals['_GETVIRTIOSCSILUNREQUEST'].fields_by_name['name']._serialized_options = b'\342A\001\002\372A\"\n opi_api.storage.v1/VirtioScsiLun'
+  _globals['_STATSVIRTIOSCSILUNREQUEST'].fields_by_name['name']._options = None
+  _globals['_STATSVIRTIOSCSILUNREQUEST'].fields_by_name['name']._serialized_options = b'\342A\001\002\372A\"\n opi_api.storage.v1/VirtioScsiLun'
+  _globals['_STATSVIRTIOSCSILUNREQUEST'].fields_by_name['controller_name_ref']._options = None
+  _globals['_STATSVIRTIOSCSILUNREQUEST'].fields_by_name['controller_name_ref']._serialized_options = b'\342A\001\001'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['CreateVirtioScsiTarget']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['CreateVirtioScsiTarget']._serialized_options = b'\332A(virtio_scsi_target,virtio_scsi_target_id\202\323\344\223\002+\"\025/v1/virtioScsiTargets:\022virtio_scsi_target'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['DeleteVirtioScsiTarget']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['DeleteVirtioScsiTarget']._serialized_options = b'\332A\004name\202\323\344\223\002 *\036/v1/{name=virtioScsiTargets/*}'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['UpdateVirtioScsiTarget']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['UpdateVirtioScsiTarget']._serialized_options = b'\332A\036virtio_scsi_target,update_mask\202\323\344\223\002G21/v1/{virtio_scsi_target.name=virtioScsiTargets/*}:\022virtio_scsi_target'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['ListVirtioScsiTargets']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['ListVirtioScsiTargets']._serialized_options = b'\332A\006parent\202\323\344\223\002 \022\036/v1/{parent=virtioScsiTargets}'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['GetVirtioScsiTarget']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['GetVirtioScsiTarget']._serialized_options = b'\332A\004name\202\323\344\223\002 \022\036/v1/{name=virtioScsiTargets/*}'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['StatsVirtioScsiTarget']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['StatsVirtioScsiTarget']._serialized_options = b'\332A\004name\202\323\344\223\002&\022$/v1/{name=virtioScsiTargets/*}:stats'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['CreateVirtioScsiController']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['CreateVirtioScsiController']._serialized_options = b'\332A0virtio_scsi_controller,virtio_scsi_controller_id\202\323\344\223\0023\"\031/v1/virtioScsiControllers:\026virtio_scsi_controller'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['DeleteVirtioScsiController']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['DeleteVirtioScsiController']._serialized_options = b'\332A\004name\202\323\344\223\002$*\"/v1/{name=virtioScsiControllers/*}'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['UpdateVirtioScsiController']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['UpdateVirtioScsiController']._serialized_options = b'\332A\"virtio_scsi_controller,update_mask\202\323\344\223\002S29/v1/{virtio_scsi_controller.name=virtioScsiControllers/*}:\026virtio_scsi_controller'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['ListVirtioScsiControllers']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['ListVirtioScsiControllers']._serialized_options = b'\332A\006parent\202\323\344\223\002$\022\"/v1/{parent=virtioScsiControllers}'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['GetVirtioScsiController']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['GetVirtioScsiController']._serialized_options = b'\332A\004name\202\323\344\223\002$\022\"/v1/{name=virtioScsiControllers/*}'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['StatsVirtioScsiController']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['StatsVirtioScsiController']._serialized_options = b'\332A\004name\202\323\344\223\002*\022(/v1/{name=virtioScsiControllers/*}:stats'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['CreateVirtioScsiLun']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['CreateVirtioScsiLun']._serialized_options = b'\332A\"virtio_scsi_lun,virtio_scsi_lun_id\202\323\344\223\002%\"\022/v1/virtioScsiLuns:\017virtio_scsi_lun'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['DeleteVirtioScsiLun']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['DeleteVirtioScsiLun']._serialized_options = b'\332A\004name\202\323\344\223\002\035*\033/v1/{name=virtioScsiLuns/*}'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['UpdateVirtioScsiLun']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['UpdateVirtioScsiLun']._serialized_options = b'\332A\033virtio_scsi_lun,update_mask\202\323\344\223\002>2+/v1/{virtio_scsi_lun.name=virtioScsiLuns/*}:\017virtio_scsi_lun'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['ListVirtioScsiLuns']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['ListVirtioScsiLuns']._serialized_options = b'\332A\006parent\202\323\344\223\002\035\022\033/v1/{parent=virtioScsiLuns}'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['GetVirtioScsiLun']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['GetVirtioScsiLun']._serialized_options = b'\332A\004name\202\323\344\223\002\035\022\033/v1/{name=virtioScsiLuns/*}'
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['StatsVirtioScsiLun']._options = None
+  _globals['_FRONTENDVIRTIOSCSISERVICE'].methods_by_name['StatsVirtioScsiLun']._serialized_options = b'\332A\004name\202\323\344\223\002#\022!/v1/{name=virtioScsiLuns/*}:stats'
+  _globals['_VIRTIOSCSITARGET']._serialized_start=246
+  _globals['_VIRTIOSCSITARGET']._serialized_end=430
+  _globals['_VIRTIOSCSICONTROLLER']._serialized_start=433
+  _globals['_VIRTIOSCSICONTROLLER']._serialized_end=798
+  _globals['_VIRTIOSCSILUN']._serialized_start=801
+  _globals['_VIRTIOSCSILUN']._serialized_end=1029
+  _globals['_CREATEVIRTIOSCSITARGETREQUEST']._serialized_start=1032
+  _globals['_CREATEVIRTIOSCSITARGETREQUEST']._serialized_end=1210
+  _globals['_DELETEVIRTIOSCSITARGETREQUEST']._serialized_start=1213
+  _globals['_DELETEVIRTIOSCSITARGETREQUEST']._serialized_end=1353
+  _globals['_UPDATEVIRTIOSCSITARGETREQUEST']._serialized_start=1356
+  _globals['_UPDATEVIRTIOSCSITARGETREQUEST']._serialized_end=1587
+  _globals['_LISTVIRTIOSCSITARGETSREQUEST']._serialized_start=1590
+  _globals['_LISTVIRTIOSCSITARGETSREQUEST']._serialized_end=1762
+  _globals['_LISTVIRTIOSCSITARGETSRESPONSE']._serialized_start=1765
+  _globals['_LISTVIRTIOSCSITARGETSRESPONSE']._serialized_end=1922
+  _globals['_GETVIRTIOSCSITARGETREQUEST']._serialized_start=1924
+  _globals['_GETVIRTIOSCSITARGETREQUEST']._serialized_end=2018
+  _globals['_STATSVIRTIOSCSITARGETREQUEST']._serialized_start=2020
+  _globals['_STATSVIRTIOSCSITARGETREQUEST']._serialized_end=2116
+  _globals['_STATSVIRTIOSCSITARGETRESPONSE']._serialized_start=2118
+  _globals['_STATSVIRTIOSCSITARGETRESPONSE']._serialized_end=2204
+  _globals['_CREATEVIRTIOSCSICONTROLLERREQUEST']._serialized_start=2207
+  _globals['_CREATEVIRTIOSCSICONTROLLERREQUEST']._serialized_end=2409
+  _globals['_DELETEVIRTIOSCSICONTROLLERREQUEST']._serialized_start=2412
+  _globals['_DELETEVIRTIOSCSICONTROLLERREQUEST']._serialized_end=2560
+  _globals['_UPDATEVIRTIOSCSICONTROLLERREQUEST']._serialized_start=2563
+  _globals['_UPDATEVIRTIOSCSICONTROLLERREQUEST']._serialized_end=2810
+  _globals['_LISTVIRTIOSCSICONTROLLERSREQUEST']._serialized_start=2813
+  _globals['_LISTVIRTIOSCSICONTROLLERSREQUEST']._serialized_end=2993
+  _globals['_LISTVIRTIOSCSICONTROLLERSRESPONSE']._serialized_start=2996
+  _globals['_LISTVIRTIOSCSICONTROLLERSRESPONSE']._serialized_end=3169
+  _globals['_GETVIRTIOSCSICONTROLLERREQUEST']._serialized_start=3171
+  _globals['_GETVIRTIOSCSICONTROLLERREQUEST']._serialized_end=3273
+  _globals['_STATSVIRTIOSCSICONTROLLERREQUEST']._serialized_start=3275
+  _globals['_STATSVIRTIOSCSICONTROLLERREQUEST']._serialized_end=3379
+  _globals['_STATSVIRTIOSCSICONTROLLERRESPONSE']._serialized_start=3381
+  _globals['_STATSVIRTIOSCSICONTROLLERRESPONSE']._serialized_end=3471
+  _globals['_CREATEVIRTIOSCSILUNREQUEST']._serialized_start=3474
+  _globals['_CREATEVIRTIOSCSILUNREQUEST']._serialized_end=3634
+  _globals['_DELETEVIRTIOSCSILUNREQUEST']._serialized_start=3637
+  _globals['_DELETEVIRTIOSCSILUNREQUEST']._serialized_end=3771
+  _globals['_UPDATEVIRTIOSCSILUNREQUEST']._serialized_start=3774
+  _globals['_UPDATEVIRTIOSCSILUNREQUEST']._serialized_end=3993
+  _globals['_LISTVIRTIOSCSILUNSREQUEST']._serialized_start=3996
+  _globals['_LISTVIRTIOSCSILUNSREQUEST']._serialized_end=4162
+  _globals['_LISTVIRTIOSCSILUNSRESPONSE']._serialized_start=4165
+  _globals['_LISTVIRTIOSCSILUNSRESPONSE']._serialized_end=4310
+  _globals['_GETVIRTIOSCSILUNREQUEST']._serialized_start=4312
+  _globals['_GETVIRTIOSCSILUNREQUEST']._serialized_end=4400
+  _globals['_STATSVIRTIOSCSILUNREQUEST']._serialized_start=4403
+  _globals['_STATSVIRTIOSCSILUNREQUEST']._serialized_end=4547
+  _globals['_STATSVIRTIOSCSILUNRESPONSE']._serialized_start=4549
+  _globals['_STATSVIRTIOSCSILUNRESPONSE']._serialized_end=4632
+  _globals['_FRONTENDVIRTIOSCSISERVICE']._serialized_start=4635
+  _globals['_FRONTENDVIRTIOSCSISERVICE']._serialized_end=7991
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/frontend_virtio_scsi_pb2_grpc.py` & `pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_scsi_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,18 +37,18 @@
                 response_deserializer=frontend__virtio__scsi__pb2.ListVirtioScsiTargetsResponse.FromString,
                 )
         self.GetVirtioScsiTarget = channel.unary_unary(
                 '/opi_api.storage.v1.FrontendVirtioScsiService/GetVirtioScsiTarget',
                 request_serializer=frontend__virtio__scsi__pb2.GetVirtioScsiTargetRequest.SerializeToString,
                 response_deserializer=frontend__virtio__scsi__pb2.VirtioScsiTarget.FromString,
                 )
-        self.VirtioScsiTargetStats = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendVirtioScsiService/VirtioScsiTargetStats',
-                request_serializer=frontend__virtio__scsi__pb2.VirtioScsiTargetStatsRequest.SerializeToString,
-                response_deserializer=frontend__virtio__scsi__pb2.VirtioScsiTargetStatsResponse.FromString,
+        self.StatsVirtioScsiTarget = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendVirtioScsiService/StatsVirtioScsiTarget',
+                request_serializer=frontend__virtio__scsi__pb2.StatsVirtioScsiTargetRequest.SerializeToString,
+                response_deserializer=frontend__virtio__scsi__pb2.StatsVirtioScsiTargetResponse.FromString,
                 )
         self.CreateVirtioScsiController = channel.unary_unary(
                 '/opi_api.storage.v1.FrontendVirtioScsiService/CreateVirtioScsiController',
                 request_serializer=frontend__virtio__scsi__pb2.CreateVirtioScsiControllerRequest.SerializeToString,
                 response_deserializer=frontend__virtio__scsi__pb2.VirtioScsiController.FromString,
                 )
         self.DeleteVirtioScsiController = channel.unary_unary(
@@ -67,18 +67,18 @@
                 response_deserializer=frontend__virtio__scsi__pb2.ListVirtioScsiControllersResponse.FromString,
                 )
         self.GetVirtioScsiController = channel.unary_unary(
                 '/opi_api.storage.v1.FrontendVirtioScsiService/GetVirtioScsiController',
                 request_serializer=frontend__virtio__scsi__pb2.GetVirtioScsiControllerRequest.SerializeToString,
                 response_deserializer=frontend__virtio__scsi__pb2.VirtioScsiController.FromString,
                 )
-        self.VirtioScsiControllerStats = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendVirtioScsiService/VirtioScsiControllerStats',
-                request_serializer=frontend__virtio__scsi__pb2.VirtioScsiControllerStatsRequest.SerializeToString,
-                response_deserializer=frontend__virtio__scsi__pb2.VirtioScsiControllerStatsResponse.FromString,
+        self.StatsVirtioScsiController = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendVirtioScsiService/StatsVirtioScsiController',
+                request_serializer=frontend__virtio__scsi__pb2.StatsVirtioScsiControllerRequest.SerializeToString,
+                response_deserializer=frontend__virtio__scsi__pb2.StatsVirtioScsiControllerResponse.FromString,
                 )
         self.CreateVirtioScsiLun = channel.unary_unary(
                 '/opi_api.storage.v1.FrontendVirtioScsiService/CreateVirtioScsiLun',
                 request_serializer=frontend__virtio__scsi__pb2.CreateVirtioScsiLunRequest.SerializeToString,
                 response_deserializer=frontend__virtio__scsi__pb2.VirtioScsiLun.FromString,
                 )
         self.DeleteVirtioScsiLun = channel.unary_unary(
@@ -97,129 +97,147 @@
                 response_deserializer=frontend__virtio__scsi__pb2.ListVirtioScsiLunsResponse.FromString,
                 )
         self.GetVirtioScsiLun = channel.unary_unary(
                 '/opi_api.storage.v1.FrontendVirtioScsiService/GetVirtioScsiLun',
                 request_serializer=frontend__virtio__scsi__pb2.GetVirtioScsiLunRequest.SerializeToString,
                 response_deserializer=frontend__virtio__scsi__pb2.VirtioScsiLun.FromString,
                 )
-        self.VirtioScsiLunStats = channel.unary_unary(
-                '/opi_api.storage.v1.FrontendVirtioScsiService/VirtioScsiLunStats',
-                request_serializer=frontend__virtio__scsi__pb2.VirtioScsiLunStatsRequest.SerializeToString,
-                response_deserializer=frontend__virtio__scsi__pb2.VirtioScsiLunStatsResponse.FromString,
+        self.StatsVirtioScsiLun = channel.unary_unary(
+                '/opi_api.storage.v1.FrontendVirtioScsiService/StatsVirtioScsiLun',
+                request_serializer=frontend__virtio__scsi__pb2.StatsVirtioScsiLunRequest.SerializeToString,
+                response_deserializer=frontend__virtio__scsi__pb2.StatsVirtioScsiLunResponse.FromString,
                 )
 
 
 class FrontendVirtioScsiServiceServicer(object):
     """Front End (host-facing) APIs. Mostly used for Virtio-scsi emulation and host presentation as alternative to Virtio-blk.
     """
 
     def CreateVirtioScsiTarget(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Create an Virtio Scsi Target
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteVirtioScsiTarget(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Delete an Virtio Scsi Target
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateVirtioScsiTarget(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Update an Virtio Scsi Target
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListVirtioScsiTargets(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """List Virtio Scsi Targets
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetVirtioScsiTarget(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Get an Virtio Scsi Target
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def VirtioScsiTargetStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsVirtioScsiTarget(self, request, context):
+        """Get an Virtio Scsi Target statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateVirtioScsiController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Create an Virtio Scsi Controller
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteVirtioScsiController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Delete an Virtio Scsi Controller
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateVirtioScsiController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Update an Virtio Scsi Controller
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListVirtioScsiControllers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """List Virtio Scsi Controllers
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetVirtioScsiController(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Get an Virtio Scsi Controller
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def VirtioScsiControllerStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsVirtioScsiController(self, request, context):
+        """Get an Virtio Scsi Controller statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateVirtioScsiLun(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Create an Virtio Scsi Lun
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteVirtioScsiLun(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Delete an Virtio Scsi Lun
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateVirtioScsiLun(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Update an Virtio Scsi Lun
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListVirtioScsiLuns(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """List Virtio Scsi Luns
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetVirtioScsiLun(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Get an Virtio Scsi Lun
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def VirtioScsiLunStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsVirtioScsiLun(self, request, context):
+        """Get an Virtio Scsi Lun statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_FrontendVirtioScsiServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -244,18 +262,18 @@
                     response_serializer=frontend__virtio__scsi__pb2.ListVirtioScsiTargetsResponse.SerializeToString,
             ),
             'GetVirtioScsiTarget': grpc.unary_unary_rpc_method_handler(
                     servicer.GetVirtioScsiTarget,
                     request_deserializer=frontend__virtio__scsi__pb2.GetVirtioScsiTargetRequest.FromString,
                     response_serializer=frontend__virtio__scsi__pb2.VirtioScsiTarget.SerializeToString,
             ),
-            'VirtioScsiTargetStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.VirtioScsiTargetStats,
-                    request_deserializer=frontend__virtio__scsi__pb2.VirtioScsiTargetStatsRequest.FromString,
-                    response_serializer=frontend__virtio__scsi__pb2.VirtioScsiTargetStatsResponse.SerializeToString,
+            'StatsVirtioScsiTarget': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsVirtioScsiTarget,
+                    request_deserializer=frontend__virtio__scsi__pb2.StatsVirtioScsiTargetRequest.FromString,
+                    response_serializer=frontend__virtio__scsi__pb2.StatsVirtioScsiTargetResponse.SerializeToString,
             ),
             'CreateVirtioScsiController': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateVirtioScsiController,
                     request_deserializer=frontend__virtio__scsi__pb2.CreateVirtioScsiControllerRequest.FromString,
                     response_serializer=frontend__virtio__scsi__pb2.VirtioScsiController.SerializeToString,
             ),
             'DeleteVirtioScsiController': grpc.unary_unary_rpc_method_handler(
@@ -274,18 +292,18 @@
                     response_serializer=frontend__virtio__scsi__pb2.ListVirtioScsiControllersResponse.SerializeToString,
             ),
             'GetVirtioScsiController': grpc.unary_unary_rpc_method_handler(
                     servicer.GetVirtioScsiController,
                     request_deserializer=frontend__virtio__scsi__pb2.GetVirtioScsiControllerRequest.FromString,
                     response_serializer=frontend__virtio__scsi__pb2.VirtioScsiController.SerializeToString,
             ),
-            'VirtioScsiControllerStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.VirtioScsiControllerStats,
-                    request_deserializer=frontend__virtio__scsi__pb2.VirtioScsiControllerStatsRequest.FromString,
-                    response_serializer=frontend__virtio__scsi__pb2.VirtioScsiControllerStatsResponse.SerializeToString,
+            'StatsVirtioScsiController': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsVirtioScsiController,
+                    request_deserializer=frontend__virtio__scsi__pb2.StatsVirtioScsiControllerRequest.FromString,
+                    response_serializer=frontend__virtio__scsi__pb2.StatsVirtioScsiControllerResponse.SerializeToString,
             ),
             'CreateVirtioScsiLun': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateVirtioScsiLun,
                     request_deserializer=frontend__virtio__scsi__pb2.CreateVirtioScsiLunRequest.FromString,
                     response_serializer=frontend__virtio__scsi__pb2.VirtioScsiLun.SerializeToString,
             ),
             'DeleteVirtioScsiLun': grpc.unary_unary_rpc_method_handler(
@@ -304,18 +322,18 @@
                     response_serializer=frontend__virtio__scsi__pb2.ListVirtioScsiLunsResponse.SerializeToString,
             ),
             'GetVirtioScsiLun': grpc.unary_unary_rpc_method_handler(
                     servicer.GetVirtioScsiLun,
                     request_deserializer=frontend__virtio__scsi__pb2.GetVirtioScsiLunRequest.FromString,
                     response_serializer=frontend__virtio__scsi__pb2.VirtioScsiLun.SerializeToString,
             ),
-            'VirtioScsiLunStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.VirtioScsiLunStats,
-                    request_deserializer=frontend__virtio__scsi__pb2.VirtioScsiLunStatsRequest.FromString,
-                    response_serializer=frontend__virtio__scsi__pb2.VirtioScsiLunStatsResponse.SerializeToString,
+            'StatsVirtioScsiLun': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsVirtioScsiLun,
+                    request_deserializer=frontend__virtio__scsi__pb2.StatsVirtioScsiLunRequest.FromString,
+                    response_serializer=frontend__virtio__scsi__pb2.StatsVirtioScsiLunResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'opi_api.storage.v1.FrontendVirtioScsiService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -406,27 +424,27 @@
         return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioScsiService/GetVirtioScsiTarget',
             frontend__virtio__scsi__pb2.GetVirtioScsiTargetRequest.SerializeToString,
             frontend__virtio__scsi__pb2.VirtioScsiTarget.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def VirtioScsiTargetStats(request,
+    def StatsVirtioScsiTarget(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioScsiService/VirtioScsiTargetStats',
-            frontend__virtio__scsi__pb2.VirtioScsiTargetStatsRequest.SerializeToString,
-            frontend__virtio__scsi__pb2.VirtioScsiTargetStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioScsiService/StatsVirtioScsiTarget',
+            frontend__virtio__scsi__pb2.StatsVirtioScsiTargetRequest.SerializeToString,
+            frontend__virtio__scsi__pb2.StatsVirtioScsiTargetResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def CreateVirtioScsiController(request,
             target,
             options=(),
@@ -508,27 +526,27 @@
         return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioScsiService/GetVirtioScsiController',
             frontend__virtio__scsi__pb2.GetVirtioScsiControllerRequest.SerializeToString,
             frontend__virtio__scsi__pb2.VirtioScsiController.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def VirtioScsiControllerStats(request,
+    def StatsVirtioScsiController(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioScsiService/VirtioScsiControllerStats',
-            frontend__virtio__scsi__pb2.VirtioScsiControllerStatsRequest.SerializeToString,
-            frontend__virtio__scsi__pb2.VirtioScsiControllerStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioScsiService/StatsVirtioScsiController',
+            frontend__virtio__scsi__pb2.StatsVirtioScsiControllerRequest.SerializeToString,
+            frontend__virtio__scsi__pb2.StatsVirtioScsiControllerResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def CreateVirtioScsiLun(request,
             target,
             options=(),
@@ -610,22 +628,22 @@
         return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioScsiService/GetVirtioScsiLun',
             frontend__virtio__scsi__pb2.GetVirtioScsiLunRequest.SerializeToString,
             frontend__virtio__scsi__pb2.VirtioScsiLun.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def VirtioScsiLunStats(request,
+    def StatsVirtioScsiLun(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioScsiService/VirtioScsiLunStats',
-            frontend__virtio__scsi__pb2.VirtioScsiLunStatsRequest.SerializeToString,
-            frontend__virtio__scsi__pb2.VirtioScsiLunStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.FrontendVirtioScsiService/StatsVirtioScsiLun',
+            frontend__virtio__scsi__pb2.StatsVirtioScsiLunRequest.SerializeToString,
+            frontend__virtio__scsi__pb2.StatsVirtioScsiLunResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/inventory_pb2_grpc.py` & `pydpu-0.2.0/pydpu/proto/v1/inventory_pb2_grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 import inventory_pb2 as inventory__pb2
 
 
-class InventorySvcStub(object):
+class InventoryServiceStub(object):
     """Service functions for the device inventory data
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.InventoryGet = channel.unary_unary(
-                '/opi_api.inventory.v1.InventorySvc/InventoryGet',
-                request_serializer=inventory__pb2.InventoryGetRequest.SerializeToString,
-                response_deserializer=inventory__pb2.InventoryGetResponse.FromString,
+        self.GetInventory = channel.unary_unary(
+                '/opi_api.inventory.v1.InventoryService/GetInventory',
+                request_serializer=inventory__pb2.GetInventoryRequest.SerializeToString,
+                response_deserializer=inventory__pb2.Inventory.FromString,
                 )
 
 
-class InventorySvcServicer(object):
+class InventoryServiceServicer(object):
     """Service functions for the device inventory data
     """
 
-    def InventoryGet(self, request, context):
+    def GetInventory(self, request, context):
         """retrieves the inventory data for the device
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_InventorySvcServicer_to_server(servicer, server):
+def add_InventoryServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'InventoryGet': grpc.unary_unary_rpc_method_handler(
-                    servicer.InventoryGet,
-                    request_deserializer=inventory__pb2.InventoryGetRequest.FromString,
-                    response_serializer=inventory__pb2.InventoryGetResponse.SerializeToString,
+            'GetInventory': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetInventory,
+                    request_deserializer=inventory__pb2.GetInventoryRequest.FromString,
+                    response_serializer=inventory__pb2.Inventory.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'opi_api.inventory.v1.InventorySvc', rpc_method_handlers)
+            'opi_api.inventory.v1.InventoryService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class InventorySvc(object):
+class InventoryService(object):
     """Service functions for the device inventory data
     """
 
     @staticmethod
-    def InventoryGet(request,
+    def GetInventory(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.inventory.v1.InventorySvc/InventoryGet',
-            inventory__pb2.InventoryGetRequest.SerializeToString,
-            inventory__pb2.InventoryGetResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.inventory.v1.InventoryService/GetInventory',
+            inventory__pb2.GetInventoryRequest.SerializeToString,
+            inventory__pb2.Inventory.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/ipsec_pb2_grpc.py` & `pydpu-0.2.0/pydpu/proto/v1/ipsec_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 import ipsec_pb2 as ipsec__pb2
 
 
-class IPsecStub(object):
-    """Missing associated documentation comment in .proto file."""
+class IPsecServiceStub(object):
+    """Service functions for IPSec Protocol 
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.IPsecVersion = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecVersion',
-                request_serializer=ipsec__pb2.IPsecVersionReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecVersionResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecVersion',
+                request_serializer=ipsec__pb2.IPsecVersionRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecVersionResponse.FromString,
                 )
         self.IPsecStats = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecStats',
-                request_serializer=ipsec__pb2.IPsecStatsReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecStatsResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecStats',
+                request_serializer=ipsec__pb2.IPsecStatsRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecStatsResponse.FromString,
                 )
         self.IPsecInitiate = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecInitiate',
-                request_serializer=ipsec__pb2.IPsecInitiateReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecInitiateResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecInitiate',
+                request_serializer=ipsec__pb2.IPsecInitiateRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecInitiateResponse.FromString,
                 )
         self.IPsecTerminate = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecTerminate',
-                request_serializer=ipsec__pb2.IPsecTerminateReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecTerminateResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecTerminate',
+                request_serializer=ipsec__pb2.IPsecTerminateRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecTerminateResponse.FromString,
                 )
         self.IPsecRekey = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecRekey',
-                request_serializer=ipsec__pb2.IPsecRekeyReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecRekeyResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecRekey',
+                request_serializer=ipsec__pb2.IPsecRekeyRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecRekeyResponse.FromString,
                 )
         self.IPsecListSas = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecListSas',
-                request_serializer=ipsec__pb2.IPsecListSasReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecListSasResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecListSas',
+                request_serializer=ipsec__pb2.IPsecListSasRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecListSasResponse.FromString,
                 )
         self.IPsecListConns = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecListConns',
-                request_serializer=ipsec__pb2.IPsecListConnsReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecListConnsResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecListConns',
+                request_serializer=ipsec__pb2.IPsecListConnsRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecListConnsResponse.FromString,
                 )
         self.IPsecListCerts = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecListCerts',
-                request_serializer=ipsec__pb2.IPsecListCertsReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecListCertsResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecListCerts',
+                request_serializer=ipsec__pb2.IPsecListCertsRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecListCertsResponse.FromString,
                 )
         self.IPsecLoadConn = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecLoadConn',
-                request_serializer=ipsec__pb2.IPsecLoadConnReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecLoadConnResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecLoadConn',
+                request_serializer=ipsec__pb2.IPsecLoadConnRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecLoadConnResponse.FromString,
                 )
         self.IPsecUnloadConn = channel.unary_unary(
-                '/opi_api.security.v1.IPsec/IPsecUnloadConn',
-                request_serializer=ipsec__pb2.IPsecUnloadConnReq.SerializeToString,
-                response_deserializer=ipsec__pb2.IPsecUnloadConnResp.FromString,
+                '/opi_api.security.v1.IPsecService/IPsecUnloadConn',
+                request_serializer=ipsec__pb2.IPsecUnloadConnRequest.SerializeToString,
+                response_deserializer=ipsec__pb2.IPsecUnloadConnResponse.FromString,
                 )
 
 
-class IPsecServicer(object):
-    """Missing associated documentation comment in .proto file."""
+class IPsecServiceServicer(object):
+    """Service functions for IPSec Protocol 
+    """
 
     def IPsecVersion(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -126,238 +128,239 @@
     def IPsecUnloadConn(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_IPsecServicer_to_server(servicer, server):
+def add_IPsecServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'IPsecVersion': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecVersion,
-                    request_deserializer=ipsec__pb2.IPsecVersionReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecVersionResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecVersionRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecVersionResponse.SerializeToString,
             ),
             'IPsecStats': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecStats,
-                    request_deserializer=ipsec__pb2.IPsecStatsReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecStatsResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecStatsRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecStatsResponse.SerializeToString,
             ),
             'IPsecInitiate': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecInitiate,
-                    request_deserializer=ipsec__pb2.IPsecInitiateReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecInitiateResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecInitiateRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecInitiateResponse.SerializeToString,
             ),
             'IPsecTerminate': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecTerminate,
-                    request_deserializer=ipsec__pb2.IPsecTerminateReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecTerminateResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecTerminateRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecTerminateResponse.SerializeToString,
             ),
             'IPsecRekey': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecRekey,
-                    request_deserializer=ipsec__pb2.IPsecRekeyReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecRekeyResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecRekeyRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecRekeyResponse.SerializeToString,
             ),
             'IPsecListSas': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecListSas,
-                    request_deserializer=ipsec__pb2.IPsecListSasReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecListSasResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecListSasRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecListSasResponse.SerializeToString,
             ),
             'IPsecListConns': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecListConns,
-                    request_deserializer=ipsec__pb2.IPsecListConnsReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecListConnsResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecListConnsRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecListConnsResponse.SerializeToString,
             ),
             'IPsecListCerts': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecListCerts,
-                    request_deserializer=ipsec__pb2.IPsecListCertsReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecListCertsResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecListCertsRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecListCertsResponse.SerializeToString,
             ),
             'IPsecLoadConn': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecLoadConn,
-                    request_deserializer=ipsec__pb2.IPsecLoadConnReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecLoadConnResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecLoadConnRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecLoadConnResponse.SerializeToString,
             ),
             'IPsecUnloadConn': grpc.unary_unary_rpc_method_handler(
                     servicer.IPsecUnloadConn,
-                    request_deserializer=ipsec__pb2.IPsecUnloadConnReq.FromString,
-                    response_serializer=ipsec__pb2.IPsecUnloadConnResp.SerializeToString,
+                    request_deserializer=ipsec__pb2.IPsecUnloadConnRequest.FromString,
+                    response_serializer=ipsec__pb2.IPsecUnloadConnResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'opi_api.security.v1.IPsec', rpc_method_handlers)
+            'opi_api.security.v1.IPsecService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class IPsec(object):
-    """Missing associated documentation comment in .proto file."""
+class IPsecService(object):
+    """Service functions for IPSec Protocol 
+    """
 
     @staticmethod
     def IPsecVersion(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecVersion',
-            ipsec__pb2.IPsecVersionReq.SerializeToString,
-            ipsec__pb2.IPsecVersionResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecVersion',
+            ipsec__pb2.IPsecVersionRequest.SerializeToString,
+            ipsec__pb2.IPsecVersionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IPsecStats(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecStats',
-            ipsec__pb2.IPsecStatsReq.SerializeToString,
-            ipsec__pb2.IPsecStatsResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecStats',
+            ipsec__pb2.IPsecStatsRequest.SerializeToString,
+            ipsec__pb2.IPsecStatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IPsecInitiate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecInitiate',
-            ipsec__pb2.IPsecInitiateReq.SerializeToString,
-            ipsec__pb2.IPsecInitiateResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecInitiate',
+            ipsec__pb2.IPsecInitiateRequest.SerializeToString,
+            ipsec__pb2.IPsecInitiateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IPsecTerminate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecTerminate',
-            ipsec__pb2.IPsecTerminateReq.SerializeToString,
-            ipsec__pb2.IPsecTerminateResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecTerminate',
+            ipsec__pb2.IPsecTerminateRequest.SerializeToString,
+            ipsec__pb2.IPsecTerminateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IPsecRekey(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecRekey',
-            ipsec__pb2.IPsecRekeyReq.SerializeToString,
-            ipsec__pb2.IPsecRekeyResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecRekey',
+            ipsec__pb2.IPsecRekeyRequest.SerializeToString,
+            ipsec__pb2.IPsecRekeyResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IPsecListSas(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecListSas',
-            ipsec__pb2.IPsecListSasReq.SerializeToString,
-            ipsec__pb2.IPsecListSasResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecListSas',
+            ipsec__pb2.IPsecListSasRequest.SerializeToString,
+            ipsec__pb2.IPsecListSasResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IPsecListConns(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecListConns',
-            ipsec__pb2.IPsecListConnsReq.SerializeToString,
-            ipsec__pb2.IPsecListConnsResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecListConns',
+            ipsec__pb2.IPsecListConnsRequest.SerializeToString,
+            ipsec__pb2.IPsecListConnsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IPsecListCerts(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecListCerts',
-            ipsec__pb2.IPsecListCertsReq.SerializeToString,
-            ipsec__pb2.IPsecListCertsResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecListCerts',
+            ipsec__pb2.IPsecListCertsRequest.SerializeToString,
+            ipsec__pb2.IPsecListCertsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IPsecLoadConn(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecLoadConn',
-            ipsec__pb2.IPsecLoadConnReq.SerializeToString,
-            ipsec__pb2.IPsecLoadConnResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecLoadConn',
+            ipsec__pb2.IPsecLoadConnRequest.SerializeToString,
+            ipsec__pb2.IPsecLoadConnResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IPsecUnloadConn(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsec/IPsecUnloadConn',
-            ipsec__pb2.IPsecUnloadConnReq.SerializeToString,
-            ipsec__pb2.IPsecUnloadConnResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.security.v1.IPsecService/IPsecUnloadConn',
+            ipsec__pb2.IPsecUnloadConnRequest.SerializeToString,
+            ipsec__pb2.IPsecUnloadConnResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/middleend_pb2_grpc.py` & `pydpu-0.2.0/pydpu/proto/v1/middleend_encryption_pb2_grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,171 +1,177 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-import middleend_pb2 as middleend__pb2
+import middleend_encryption_pb2 as middleend__encryption__pb2
 
 
-class MiddleendServiceStub(object):
+class MiddleendEncryptionServiceStub(object):
     """Middle End (Storage Services) APIs. For example, encryption, compression, raid, QoS, multipath, ...
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.CreateEncryptedVolume = channel.unary_unary(
-                '/opi_api.storage.v1.MiddleendService/CreateEncryptedVolume',
-                request_serializer=middleend__pb2.CreateEncryptedVolumeRequest.SerializeToString,
-                response_deserializer=middleend__pb2.EncryptedVolume.FromString,
+                '/opi_api.storage.v1.MiddleendEncryptionService/CreateEncryptedVolume',
+                request_serializer=middleend__encryption__pb2.CreateEncryptedVolumeRequest.SerializeToString,
+                response_deserializer=middleend__encryption__pb2.EncryptedVolume.FromString,
                 )
         self.DeleteEncryptedVolume = channel.unary_unary(
-                '/opi_api.storage.v1.MiddleendService/DeleteEncryptedVolume',
-                request_serializer=middleend__pb2.DeleteEncryptedVolumeRequest.SerializeToString,
+                '/opi_api.storage.v1.MiddleendEncryptionService/DeleteEncryptedVolume',
+                request_serializer=middleend__encryption__pb2.DeleteEncryptedVolumeRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.UpdateEncryptedVolume = channel.unary_unary(
-                '/opi_api.storage.v1.MiddleendService/UpdateEncryptedVolume',
-                request_serializer=middleend__pb2.UpdateEncryptedVolumeRequest.SerializeToString,
-                response_deserializer=middleend__pb2.EncryptedVolume.FromString,
+                '/opi_api.storage.v1.MiddleendEncryptionService/UpdateEncryptedVolume',
+                request_serializer=middleend__encryption__pb2.UpdateEncryptedVolumeRequest.SerializeToString,
+                response_deserializer=middleend__encryption__pb2.EncryptedVolume.FromString,
                 )
         self.ListEncryptedVolumes = channel.unary_unary(
-                '/opi_api.storage.v1.MiddleendService/ListEncryptedVolumes',
-                request_serializer=middleend__pb2.ListEncryptedVolumesRequest.SerializeToString,
-                response_deserializer=middleend__pb2.ListEncryptedVolumesResponse.FromString,
+                '/opi_api.storage.v1.MiddleendEncryptionService/ListEncryptedVolumes',
+                request_serializer=middleend__encryption__pb2.ListEncryptedVolumesRequest.SerializeToString,
+                response_deserializer=middleend__encryption__pb2.ListEncryptedVolumesResponse.FromString,
                 )
         self.GetEncryptedVolume = channel.unary_unary(
-                '/opi_api.storage.v1.MiddleendService/GetEncryptedVolume',
-                request_serializer=middleend__pb2.GetEncryptedVolumeRequest.SerializeToString,
-                response_deserializer=middleend__pb2.EncryptedVolume.FromString,
+                '/opi_api.storage.v1.MiddleendEncryptionService/GetEncryptedVolume',
+                request_serializer=middleend__encryption__pb2.GetEncryptedVolumeRequest.SerializeToString,
+                response_deserializer=middleend__encryption__pb2.EncryptedVolume.FromString,
                 )
-        self.EncryptedVolumeStats = channel.unary_unary(
-                '/opi_api.storage.v1.MiddleendService/EncryptedVolumeStats',
-                request_serializer=middleend__pb2.EncryptedVolumeStatsRequest.SerializeToString,
-                response_deserializer=middleend__pb2.EncryptedVolumeStatsResponse.FromString,
+        self.StatsEncryptedVolume = channel.unary_unary(
+                '/opi_api.storage.v1.MiddleendEncryptionService/StatsEncryptedVolume',
+                request_serializer=middleend__encryption__pb2.StatsEncryptedVolumeRequest.SerializeToString,
+                response_deserializer=middleend__encryption__pb2.StatsEncryptedVolumeResponse.FromString,
                 )
 
 
-class MiddleendServiceServicer(object):
+class MiddleendEncryptionServiceServicer(object):
     """Middle End (Storage Services) APIs. For example, encryption, compression, raid, QoS, multipath, ...
     """
 
     def CreateEncryptedVolume(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Create an Encrypted Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteEncryptedVolume(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Delete an Encrypted Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateEncryptedVolume(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Update an Encrypted Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListEncryptedVolumes(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """List Encrypted Volumes
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetEncryptedVolume(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Get an Encrypted Volume
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def EncryptedVolumeStats(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def StatsEncryptedVolume(self, request, context):
+        """Get an Encrypted Volume statistics
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_MiddleendServiceServicer_to_server(servicer, server):
+def add_MiddleendEncryptionServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateEncryptedVolume': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateEncryptedVolume,
-                    request_deserializer=middleend__pb2.CreateEncryptedVolumeRequest.FromString,
-                    response_serializer=middleend__pb2.EncryptedVolume.SerializeToString,
+                    request_deserializer=middleend__encryption__pb2.CreateEncryptedVolumeRequest.FromString,
+                    response_serializer=middleend__encryption__pb2.EncryptedVolume.SerializeToString,
             ),
             'DeleteEncryptedVolume': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteEncryptedVolume,
-                    request_deserializer=middleend__pb2.DeleteEncryptedVolumeRequest.FromString,
+                    request_deserializer=middleend__encryption__pb2.DeleteEncryptedVolumeRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'UpdateEncryptedVolume': grpc.unary_unary_rpc_method_handler(
                     servicer.UpdateEncryptedVolume,
-                    request_deserializer=middleend__pb2.UpdateEncryptedVolumeRequest.FromString,
-                    response_serializer=middleend__pb2.EncryptedVolume.SerializeToString,
+                    request_deserializer=middleend__encryption__pb2.UpdateEncryptedVolumeRequest.FromString,
+                    response_serializer=middleend__encryption__pb2.EncryptedVolume.SerializeToString,
             ),
             'ListEncryptedVolumes': grpc.unary_unary_rpc_method_handler(
                     servicer.ListEncryptedVolumes,
-                    request_deserializer=middleend__pb2.ListEncryptedVolumesRequest.FromString,
-                    response_serializer=middleend__pb2.ListEncryptedVolumesResponse.SerializeToString,
+                    request_deserializer=middleend__encryption__pb2.ListEncryptedVolumesRequest.FromString,
+                    response_serializer=middleend__encryption__pb2.ListEncryptedVolumesResponse.SerializeToString,
             ),
             'GetEncryptedVolume': grpc.unary_unary_rpc_method_handler(
                     servicer.GetEncryptedVolume,
-                    request_deserializer=middleend__pb2.GetEncryptedVolumeRequest.FromString,
-                    response_serializer=middleend__pb2.EncryptedVolume.SerializeToString,
+                    request_deserializer=middleend__encryption__pb2.GetEncryptedVolumeRequest.FromString,
+                    response_serializer=middleend__encryption__pb2.EncryptedVolume.SerializeToString,
             ),
-            'EncryptedVolumeStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.EncryptedVolumeStats,
-                    request_deserializer=middleend__pb2.EncryptedVolumeStatsRequest.FromString,
-                    response_serializer=middleend__pb2.EncryptedVolumeStatsResponse.SerializeToString,
+            'StatsEncryptedVolume': grpc.unary_unary_rpc_method_handler(
+                    servicer.StatsEncryptedVolume,
+                    request_deserializer=middleend__encryption__pb2.StatsEncryptedVolumeRequest.FromString,
+                    response_serializer=middleend__encryption__pb2.StatsEncryptedVolumeResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'opi_api.storage.v1.MiddleendService', rpc_method_handlers)
+            'opi_api.storage.v1.MiddleendEncryptionService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class MiddleendService(object):
+class MiddleendEncryptionService(object):
     """Middle End (Storage Services) APIs. For example, encryption, compression, raid, QoS, multipath, ...
     """
 
     @staticmethod
     def CreateEncryptedVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendService/CreateEncryptedVolume',
-            middleend__pb2.CreateEncryptedVolumeRequest.SerializeToString,
-            middleend__pb2.EncryptedVolume.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendEncryptionService/CreateEncryptedVolume',
+            middleend__encryption__pb2.CreateEncryptedVolumeRequest.SerializeToString,
+            middleend__encryption__pb2.EncryptedVolume.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def DeleteEncryptedVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendService/DeleteEncryptedVolume',
-            middleend__pb2.DeleteEncryptedVolumeRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendEncryptionService/DeleteEncryptedVolume',
+            middleend__encryption__pb2.DeleteEncryptedVolumeRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def UpdateEncryptedVolume(request,
             target,
@@ -173,63 +179,63 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendService/UpdateEncryptedVolume',
-            middleend__pb2.UpdateEncryptedVolumeRequest.SerializeToString,
-            middleend__pb2.EncryptedVolume.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendEncryptionService/UpdateEncryptedVolume',
+            middleend__encryption__pb2.UpdateEncryptedVolumeRequest.SerializeToString,
+            middleend__encryption__pb2.EncryptedVolume.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ListEncryptedVolumes(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendService/ListEncryptedVolumes',
-            middleend__pb2.ListEncryptedVolumesRequest.SerializeToString,
-            middleend__pb2.ListEncryptedVolumesResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendEncryptionService/ListEncryptedVolumes',
+            middleend__encryption__pb2.ListEncryptedVolumesRequest.SerializeToString,
+            middleend__encryption__pb2.ListEncryptedVolumesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetEncryptedVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendService/GetEncryptedVolume',
-            middleend__pb2.GetEncryptedVolumeRequest.SerializeToString,
-            middleend__pb2.EncryptedVolume.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendEncryptionService/GetEncryptedVolume',
+            middleend__encryption__pb2.GetEncryptedVolumeRequest.SerializeToString,
+            middleend__encryption__pb2.EncryptedVolume.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def EncryptedVolumeStats(request,
+    def StatsEncryptedVolume(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendService/EncryptedVolumeStats',
-            middleend__pb2.EncryptedVolumeStatsRequest.SerializeToString,
-            middleend__pb2.EncryptedVolumeStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/opi_api.storage.v1.MiddleendEncryptionService/StatsEncryptedVolume',
+            middleend__encryption__pb2.StatsEncryptedVolumeRequest.SerializeToString,
+            middleend__encryption__pb2.StatsEncryptedVolumeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pydpu-0.1.2/pydpu/proto/v1/uuid_pb2.py` & `pydpu-0.2.0/pydpu/proto/v1/telco_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: uuid.proto
+# source: telco.proto
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nuuid.proto\x12\x11opi_api.common.v1\"\x15\n\x04Uuid\x12\r\n\x05value\x18\x01 \x01(\tBP\n\x11opi_api.common.v1B\tUuidProtoP\x01Z.github.com/opiproject/opi-api/common/v1/gen/gob\x06proto3')
-
-
-
-_UUID = DESCRIPTOR.message_types_by_name['Uuid']
-Uuid = _reflection.GeneratedProtocolMessageType('Uuid', (_message.Message,), {
-  'DESCRIPTOR' : _UUID,
-  '__module__' : 'uuid_pb2'
-  # @@protoc_insertion_point(class_scope:opi_api.common.v1.Uuid)
-  })
-_sym_db.RegisterMessage(Uuid)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btelco.proto\x12\x1eopi_api.network.telco.v1alpha1Bk\n\x1eopi_api.network.telco.v1alpha1B\nTelcoProtoP\x01Z;github.com/opiproject/opi-api/network/telco/v1alpha1/gen/gob\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'telco_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\021opi_api.common.v1B\tUuidProtoP\001Z.github.com/opiproject/opi-api/common/v1/gen/go'
-  _UUID._serialized_start=33
-  _UUID._serialized_end=54
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\036opi_api.network.telco.v1alpha1B\nTelcoProtoP\001Z;github.com/opiproject/opi-api/network/telco/v1alpha1/gen/go'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pydpu-0.1.2/pyproject.toml` & `pydpu-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "pydpu"
-version = "0.1.2"
+version = "0.2.0"
 description = "Python library and cli to communicate with DPUs and IPUs"
 authors = ["OPI Dev <opi-dev@lists.opiproject.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 dpu = "pydpu.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 Click = "^8.1"
 grpcio = "^1.51.1"
 google = "^3.0.0"
 google-api-core = "^2.11.0"
-
+redfish = "^3.2.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
-flake8 = "^6.0.0"
+flake8 = "^7.0.0"
 bandit = "^1.7.4"
 isort = "^5.12.0"
 bump2version = "^1.0.1"
 grpcio-tools = "^1.51.1"
 mypy-protobuf = "^3.4.0"
```

### Comparing `pydpu-0.1.2/setup.py` & `pydpu-0.2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['pydpu', 'pydpu.proto', 'pydpu.proto.v1']
+['pydpu', 'pydpu.dpuredfish', 'pydpu.proto', 'pydpu.proto.v1']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Click>=8.1,<9.0',
  'google-api-core>=2.11.0,<3.0.0',
  'google>=3.0.0,<4.0.0',
- 'grpcio>=1.51.1,<2.0.0']
+ 'grpcio>=1.51.1,<2.0.0',
+ 'redfish>=3.2.1,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['dpu = pydpu.cli:main']}
 
 setup_kwargs = {
     'name': 'pydpu',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'Python library and cli to communicate with DPUs and IPUs',
-    'long_description': '# pydpu\n\n[![License](https://img.shields.io/github/license/opiproject/pydpu?style=flat&color=blue&label=License)](https://github.com/opiproject/pydpu/blob/main/LICENSE)\n[![Pulls](https://img.shields.io/docker/pulls/opiproject/pydpu.svg?logo=docker&style=flat&label=Pulls)](https://hub.docker.com/r/opiproject/pydpu)\n[![PyPI](https://img.shields.io/pypi/v/pydpu)](https://pypi.org/project/pydpu/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)\n[![codecov](https://codecov.io/gh/opiproject/pydpu/branch/main/graph/badge.svg)](https://codecov.io/gh/opiproject/pydpu)\n[![Linters](https://github.com/opiproject/pydpu/actions/workflows/linters.yml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/linters.yml)\n[![Docker](https://github.com/opiproject/pydpu/actions/workflows/docker.yaml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/docker.yaml)\n[![Tests](https://github.com/opiproject/pydpu/actions/workflows/test.yaml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/test.yaml)\n\nPython library and cli to communicate with DPUs and IPUs\n\n## I Want To Contribute\n\nThis project welcomes contributions and suggestions.  We are happy to have the Community involved via submission of **Issues and Pull Requests** (with substantive content or even just fixes). We are hoping for the documents, test framework, etc. to become a community process with active engagement.  PRs can be reviewed by by any number of people, and a maintainer may accept.\n\nSee [CONTRIBUTING](https://github.com/opiproject/opi/blob/main/CONTRIBUTING.md) and [GitHub Basic Process](https://github.com/opiproject/opi/blob/main/doc-github-rules.md) for more details.\n\n## Installation\n\nThere are several ways of running this CLI.\n\n### Docker\n\n```sh\ndocker pull opiproject/pydpu:<version>\n```\n\nYou can specify a version like `0.1.1` or use `latest` to get the most up-to-date version.\n\nRun latest version of the CLI in a container:\n\n```sh\ndocker run --rm opiproject/pydpu:latest --help\n```\n\nReplace `--help` with any `pydpu` command, without `pydpu` itself.\n\n### PyPI\n\n```sh\npip install pydpu\n```\n\n## Usage\n\n### Inventory\n\nTo get inventory, run:\n\n```sh\npydpu --address=localhost:50151 inventory get\n```\n\n### Ipsec\n\nTo create a tunnel, run:\n\n```sh\npydpu --address=localhost:50151 ipsec create-tunnel\n```\n\nTo get statistics, run:\n\n```sh\npydpu --address=localhost:50151 ipsec stats\n```\n\n## Packaging\n\nThis project uses [poetry](https://python-poetry.org/) to manage dependencies, build, etc.\n\n## Releasing new versions\n\n```sh\n# Make sure you have dev dependencies installed\n$ poetry install --group dev\n# Use bump2version to update version strings and create a new tag\n$ bump2version <patch|minor|major>\n# Push new tag\n$ git push --tags\n# Create GitHub release\n$ gh release create v$(poetry version -s) --generate-notes\n```\n',
+    'long_description': '# pydpu\n\n[![License](https://img.shields.io/github/license/opiproject/pydpu?style=flat&color=blue&label=License)](https://github.com/opiproject/pydpu/blob/main/LICENSE)\n[![Pulls](https://img.shields.io/docker/pulls/opiproject/pydpu.svg?logo=docker&style=flat&label=Pulls)](https://hub.docker.com/r/opiproject/pydpu)\n[![PyPI](https://img.shields.io/pypi/v/pydpu)](https://pypi.org/project/pydpu/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)\n[![codecov](https://codecov.io/gh/opiproject/pydpu/branch/main/graph/badge.svg)](https://codecov.io/gh/opiproject/pydpu)\n[![Linters](https://github.com/opiproject/pydpu/actions/workflows/linters.yml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/linters.yml)\n[![CodeQL](https://github.com/opiproject/pydpu/actions/workflows/codeql.yml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/codeql.yml)\n[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/opiproject/pydpu/badge)](https://securityscorecards.dev/viewer/?platform=github.com&org=opiproject&repo=pydpu)\n[![Docker](https://github.com/opiproject/pydpu/actions/workflows/docker.yaml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/docker.yaml)\n[![Tests](https://github.com/opiproject/pydpu/actions/workflows/python.yaml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/python.yaml)\n[![GitHub stars](https://img.shields.io/github/stars/opiproject/pydpu.svg?style=flat-square&label=github%20stars)](https://github.com/opiproject/pydpu)\n[![GitHub Contributors](https://img.shields.io/github/contributors/opiproject/pydpu.svg?style=flat-square)](https://github.com/opiproject/pydpu/graphs/contributors)\n\nPython library and cli to communicate with DPUs and IPUs\n\n## I Want To Contribute\n\nThis project welcomes contributions and suggestions.  We are happy to have the Community involved via submission of **Issues and Pull Requests** (with substantive content or even just fixes). We are hoping for the documents, test framework, etc. to become a community process with active engagement.  PRs can be reviewed by by any number of people, and a maintainer may accept.\n\nSee [CONTRIBUTING](https://github.com/opiproject/opi/blob/main/CONTRIBUTING.md) and [GitHub Basic Process](https://github.com/opiproject/opi/blob/main/doc-github-rules.md) for more details.\n\n## Installation\n\nThere are several ways of running this CLI.\n\n### Docker\n\n```sh\ndocker pull opiproject/pydpu:<version>\n```\n\nYou can specify a version like `0.1.1` or use `latest` to get the most up-to-date version.\n\nRun latest version of the CLI in a container:\n\n```sh\ndocker run -it --rm --network=host opiproject/pydpu:latest --help\n```\n\nReplace `--help` with any `pydpu` command, without `pydpu` itself.\n\n### PyPI\n\n```sh\npip install pydpu\n```\n\n## Usage\n\n### Version\n\nTo get version, run:\n\n```sh\n$ pydpu --version\ndpu, version 0.1.1\n```\n\n### Redfish\n\nTo communicate over redfish, run:\n\n```sh\npydpu --address=10.10.10.10 redfish --username root --password 0penBmc test\n```\n\n### Inventory\n\nTo get inventory, run:\n\n```sh\npydpu --address=localhost:50151 inventory get\n```\n\n### Ipsec\n\nTo create a tunnel, run:\n\n```sh\npydpu --address=localhost:50151 ipsec create-tunnel\n```\n\nTo get statistics, run:\n\n```sh\npydpu --address=localhost:50151 ipsec stats\n```\n\n### Storage\n\nTo create a subsystem, run:\n\n```sh\npydpu --address=localhost:50151 storage subsystem\n```\n\nTo create a controller, run:\n\n```sh\npydpu --address=localhost:50151 storage controller\n```\n\nTo create a namespace, run:\n\n```sh\npydpu --address=localhost:50151 storage namespace\n```\n\n### Evpn\n\nTo create a logical bridge, run:\n\n```sh\npydpu --address=localhost:50151 evpn bridge\n```\n\nTo create a bridge port, run:\n\n```sh\npydpu --address=localhost:50151 evpn port\n```\n\nTo create a vrf, run:\n\n```sh\npydpu --address=localhost:50151 evpn vrf\n```\n\nTo create a svi, run:\n\n```sh\npydpu --address=localhost:50151 evpn svi\n```\n\n## Packaging\n\nThis project uses [poetry](https://python-poetry.org/) to manage dependencies, build, etc.\n\n## Releasing new versions\n\n```sh\n# Make sure you have dev dependencies installed\n$ poetry install --group dev\n# Use bump2version to update version strings and create a new tag\n$ bump2version <patch|minor|major>\n# Push new tag\n$ git push --tags\n# Create GitHub release\n$ gh release create v$(poetry version -s) --generate-notes\n```\n',
     'author': 'OPI Dev',
     'author_email': 'opi-dev@lists.opiproject.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pydpu-0.1.2/PKG-INFO` & `pydpu-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 Metadata-Version: 2.1
 Name: pydpu
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python library and cli to communicate with DPUs and IPUs
 License: Apache-2.0
 Author: OPI Dev
 Author-email: opi-dev@lists.opiproject.org
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Click (>=8.1,<9.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-core (>=2.11.0,<3.0.0)
 Requires-Dist: grpcio (>=1.51.1,<2.0.0)
+Requires-Dist: redfish (>=3.2.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # pydpu
 
 [![License](https://img.shields.io/github/license/opiproject/pydpu?style=flat&color=blue&label=License)](https://github.com/opiproject/pydpu/blob/main/LICENSE)
 [![Pulls](https://img.shields.io/docker/pulls/opiproject/pydpu.svg?logo=docker&style=flat&label=Pulls)](https://hub.docker.com/r/opiproject/pydpu)
 [![PyPI](https://img.shields.io/pypi/v/pydpu)](https://pypi.org/project/pydpu/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/opiproject/pydpu/branch/main/graph/badge.svg)](https://codecov.io/gh/opiproject/pydpu)
 [![Linters](https://github.com/opiproject/pydpu/actions/workflows/linters.yml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/linters.yml)
+[![CodeQL](https://github.com/opiproject/pydpu/actions/workflows/codeql.yml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/codeql.yml)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/opiproject/pydpu/badge)](https://securityscorecards.dev/viewer/?platform=github.com&org=opiproject&repo=pydpu)
 [![Docker](https://github.com/opiproject/pydpu/actions/workflows/docker.yaml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/docker.yaml)
-[![Tests](https://github.com/opiproject/pydpu/actions/workflows/test.yaml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/test.yaml)
+[![Tests](https://github.com/opiproject/pydpu/actions/workflows/python.yaml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/python.yaml)
+[![GitHub stars](https://img.shields.io/github/stars/opiproject/pydpu.svg?style=flat-square&label=github%20stars)](https://github.com/opiproject/pydpu)
+[![GitHub Contributors](https://img.shields.io/github/contributors/opiproject/pydpu.svg?style=flat-square)](https://github.com/opiproject/pydpu/graphs/contributors)
 
 Python library and cli to communicate with DPUs and IPUs
 
 ## I Want To Contribute
 
 This project welcomes contributions and suggestions.  We are happy to have the Community involved via submission of **Issues and Pull Requests** (with substantive content or even just fixes). We are hoping for the documents, test framework, etc. to become a community process with active engagement.  PRs can be reviewed by by any number of people, and a maintainer may accept.
 
@@ -47,27 +52,44 @@
 ```
 
 You can specify a version like `0.1.1` or use `latest` to get the most up-to-date version.
 
 Run latest version of the CLI in a container:
 
 ```sh
-docker run --rm opiproject/pydpu:latest --help
+docker run -it --rm --network=host opiproject/pydpu:latest --help
 ```
 
 Replace `--help` with any `pydpu` command, without `pydpu` itself.
 
 ### PyPI
 
 ```sh
 pip install pydpu
 ```
 
 ## Usage
 
+### Version
+
+To get version, run:
+
+```sh
+$ pydpu --version
+dpu, version 0.1.1
+```
+
+### Redfish
+
+To communicate over redfish, run:
+
+```sh
+pydpu --address=10.10.10.10 redfish --username root --password 0penBmc test
+```
+
 ### Inventory
 
 To get inventory, run:
 
 ```sh
 pydpu --address=localhost:50151 inventory get
 ```
@@ -82,14 +104,60 @@
 
 To get statistics, run:
 
 ```sh
 pydpu --address=localhost:50151 ipsec stats
 ```
 
+### Storage
+
+To create a subsystem, run:
+
+```sh
+pydpu --address=localhost:50151 storage subsystem
+```
+
+To create a controller, run:
+
+```sh
+pydpu --address=localhost:50151 storage controller
+```
+
+To create a namespace, run:
+
+```sh
+pydpu --address=localhost:50151 storage namespace
+```
+
+### Evpn
+
+To create a logical bridge, run:
+
+```sh
+pydpu --address=localhost:50151 evpn bridge
+```
+
+To create a bridge port, run:
+
+```sh
+pydpu --address=localhost:50151 evpn port
+```
+
+To create a vrf, run:
+
+```sh
+pydpu --address=localhost:50151 evpn vrf
+```
+
+To create a svi, run:
+
+```sh
+pydpu --address=localhost:50151 evpn svi
+```
+
 ## Packaging
 
 This project uses [poetry](https://python-poetry.org/) to manage dependencies, build, etc.
 
 ## Releasing new versions
 
 ```sh
```

