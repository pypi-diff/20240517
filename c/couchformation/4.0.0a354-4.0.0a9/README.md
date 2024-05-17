# Comparing `tmp/couchformation-4.0.0a354.tar.gz` & `tmp/couchformation-4.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchformation-4.0.0a354.tar", max compression
+gzip compressed data, was "couchformation-4.0.0a9.tar", last modified: Thu Sep 21 21:03:08 2023, max compression
```

## Comparing `couchformation-4.0.0a354.tar` & `couchformation-4.0.0a9.tar`

### file list

```diff
@@ -1,107 +1,23 @@
--rw-r--r--   0        0        0    10141 2024-01-11 14:36:20.239894 couchformation-4.0.0a354/LICENSE.txt
--rw-r--r--   0        0        0    10008 2024-05-17 01:02:25.417003 couchformation-4.0.0a354/README.md
--rw-r--r--   0        0        0      226 2024-05-17 01:02:25.416559 couchformation-4.0.0a354/couchformation/__init__.py
--rw-r--r--   0        0        0        0 2023-08-28 18:45:45.990788 couchformation-4.0.0a354/couchformation/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-08-28 19:47:21.352643 couchformation-4.0.0a354/couchformation/aws/driver/__init__.py
--rw-r--r--   0        0        0    10771 2024-04-09 13:19:10.353208 couchformation-4.0.0a354/couchformation/aws/driver/base.py
--rw-r--r--   0        0        0     7861 2024-01-23 15:33:47.972247 couchformation-4.0.0a354/couchformation/aws/driver/constants.py
--rw-r--r--   0        0        0     1273 2024-03-29 20:44:13.413971 couchformation-4.0.0a354/couchformation/aws/driver/cost.py
--rw-r--r--   0        0        0     6340 2024-05-16 00:42:29.039981 couchformation-4.0.0a354/couchformation/aws/driver/dns.py
--rw-r--r--   0        0        0     4036 2024-04-23 17:59:53.514684 couchformation-4.0.0a354/couchformation/aws/driver/gateway.py
--rw-r--r--   0        0        0     7172 2024-01-23 01:13:01.398158 couchformation-4.0.0a354/couchformation/aws/driver/image.py
--rw-r--r--   0        0        0     9964 2024-04-15 22:54:32.758677 couchformation-4.0.0a354/couchformation/aws/driver/instance.py
--rw-r--r--   0        0        0     4956 2024-04-19 21:46:33.766375 couchformation-4.0.0a354/couchformation/aws/driver/machine.py
--rw-r--r--   0        0        0     8807 2024-05-15 22:20:50.213638 couchformation-4.0.0a354/couchformation/aws/driver/network.py
--rw-r--r--   0        0        0     6385 2024-04-23 20:48:34.493622 couchformation-4.0.0a354/couchformation/aws/driver/nsg.py
--rw-r--r--   0        0        0     4972 2024-05-15 22:14:59.713184 couchformation-4.0.0a354/couchformation/aws/driver/route.py
--rw-r--r--   0        0        0     5138 2024-04-08 20:24:46.855130 couchformation-4.0.0a354/couchformation/aws/driver/sshkey.py
--rw-r--r--   0        0        0    23888 2024-05-16 13:41:00.221459 couchformation-4.0.0a354/couchformation/aws/network.py
--rw-r--r--   0        0        0    12788 2024-04-19 20:58:41.728467 couchformation-4.0.0a354/couchformation/aws/node.py
--rw-r--r--   0        0        0        0 2023-09-12 19:20:27.915328 couchformation-4.0.0a354/couchformation/azure/__init__.py
--rw-r--r--   0        0        0        0 2023-09-12 21:22:11.556480 couchformation-4.0.0a354/couchformation/azure/driver/__init__.py
--rw-r--r--   0        0        0    10275 2024-04-11 22:26:09.510807 couchformation-4.0.0a354/couchformation/azure/driver/base.py
--rw-r--r--   0        0        0     4850 2024-04-11 19:59:18.437128 couchformation-4.0.0a354/couchformation/azure/driver/constants.py
--rw-r--r--   0        0        0     2601 2024-04-11 22:03:36.736927 couchformation-4.0.0a354/couchformation/azure/driver/disk.py
--rw-r--r--   0        0        0     6199 2024-03-25 17:58:42.792359 couchformation-4.0.0a354/couchformation/azure/driver/dns.py
--rw-r--r--   0        0        0     6146 2024-04-29 15:37:35.940368 couchformation-4.0.0a354/couchformation/azure/driver/image.py
--rw-r--r--   0        0        0     6717 2024-04-11 21:28:45.775519 couchformation-4.0.0a354/couchformation/azure/driver/instance.py
--rw-r--r--   0        0        0     4479 2024-01-23 18:00:01.962839 couchformation-4.0.0a354/couchformation/azure/driver/machine.py
--rw-r--r--   0        0        0    14305 2024-04-25 21:53:08.049654 couchformation-4.0.0a354/couchformation/azure/driver/network.py
--rw-r--r--   0        0        0     7464 2024-03-25 19:42:32.057443 couchformation-4.0.0a354/couchformation/azure/driver/private_dns.py
--rw-r--r--   0        0        0    20853 2024-05-16 13:41:00.212823 couchformation-4.0.0a354/couchformation/azure/network.py
--rw-r--r--   0        0        0    15718 2024-04-23 15:09:01.190322 couchformation-4.0.0a354/couchformation/azure/node.py
--rw-r--r--   0        0        0        0 2024-05-15 16:19:22.415306 couchformation-4.0.0a354/couchformation/capella/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 16:21:37.951776 couchformation-4.0.0a354/couchformation/capella/driver/__init__.py
--rw-r--r--   0        0        0     1183 2024-03-27 22:44:27.829419 couchformation-4.0.0a354/couchformation/capella/driver/base.py
--rw-r--r--   0        0        0     3377 2024-03-27 21:54:02.391559 couchformation-4.0.0a354/couchformation/capella/driver/cb_bucket.py
--rw-r--r--   0        0        0    27385 2024-05-08 03:34:14.503742 couchformation-4.0.0a354/couchformation/capella/driver/cb_capella.py
--rw-r--r--   0        0        0     4456 2024-03-27 21:55:34.982411 couchformation-4.0.0a354/couchformation/capella/driver/cb_capella_config.py
--rw-r--r--   0        0        0    11842 2024-05-08 03:27:06.872261 couchformation-4.0.0a354/couchformation/capella/node.py
--rw-r--r--   0        0        0        0 2023-11-02 01:40:10.262340 couchformation-4.0.0a354/couchformation/cli/__init__.py
--rw-r--r--   0        0        0     5978 2024-04-15 18:53:03.819589 couchformation-4.0.0a354/couchformation/cli/cli.py
--rw-r--r--   0        0        0     6107 2024-05-16 19:19:02.317200 couchformation-4.0.0a354/couchformation/cli/cloudmgr.py
--rw-r--r--   0        0        0     1520 2024-04-16 17:56:40.697749 couchformation-4.0.0a354/couchformation/cli/dbdump.py
--rw-r--r--   0        0        0    13795 2023-09-11 22:16:04.182349 couchformation-4.0.0a354/couchformation/common/config/resources.py
--rw-r--r--   0        0        0    13632 2024-04-23 21:17:06.373416 couchformation-4.0.0a354/couchformation/config.py
--rw-r--r--   0        0        0     6946 2024-04-15 21:07:12.265938 couchformation-4.0.0a354/couchformation/constants.py
--rw-r--r--   0        0        0      579 2024-03-27 15:39:49.410925 couchformation-4.0.0a354/couchformation/data/build_profiles.yaml
--rw-r--r--   0        0        0      146 2024-02-09 18:58:57.050546 couchformation-4.0.0a354/couchformation/data/cloud_profiles.yaml
--rw-r--r--   0        0        0      377 2023-11-17 19:22:36.170232 couchformation-4.0.0a354/couchformation/data/container_profiles.yaml
--rw-r--r--   0        0        0      188 2024-04-15 20:50:27.114946 couchformation-4.0.0a354/couchformation/data/node_ports.yaml
--rw-r--r--   0        0        0     1919 2024-04-30 01:28:29.567620 couchformation-4.0.0a354/couchformation/data/node_profiles.yaml
--rw-r--r--   0        0        0     2431 2024-04-15 17:54:33.065085 couchformation-4.0.0a354/couchformation/data/option_help.yaml
--rw-r--r--   0        0        0     1343 2024-04-29 21:59:10.161063 couchformation-4.0.0a354/couchformation/data/provisioner_profiles.yaml
--rw-r--r--   0        0        0      205 2024-04-23 23:41:38.053629 couchformation-4.0.0a354/couchformation/data/strategy_profiles.yaml
--rw-r--r--   0        0        0     3861 2024-05-16 13:41:00.217440 couchformation-4.0.0a354/couchformation/data/target_profiles.yaml
--rw-r--r--   0        0        0    21348 2024-04-30 13:41:59.062708 couchformation-4.0.0a354/couchformation/deployment.py
--rw-r--r--   0        0        0        0 2023-11-17 14:45:37.838681 couchformation-4.0.0a354/couchformation/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-11-17 14:45:24.975643 couchformation-4.0.0a354/couchformation/docker/driver/__init__.py
--rw-r--r--   0        0        0     1341 2023-11-17 18:12:08.761914 couchformation-4.0.0a354/couchformation/docker/driver/base.py
--rw-r--r--   0        0        0      231 2023-11-20 17:51:38.312560 couchformation-4.0.0a354/couchformation/docker/driver/constants.py
--rw-r--r--   0        0        0     8613 2024-03-28 14:14:47.928646 couchformation-4.0.0a354/couchformation/docker/driver/container.py
--rw-r--r--   0        0        0     2658 2023-11-20 17:57:39.056124 couchformation-4.0.0a354/couchformation/docker/driver/network.py
--rw-r--r--   0        0        0     3717 2024-05-16 13:41:00.224362 couchformation-4.0.0a354/couchformation/docker/network.py
--rw-r--r--   0        0        0     3356 2024-04-17 13:30:08.168493 couchformation-4.0.0a354/couchformation/docker/node.py
--rw-r--r--   0        0        0     2111 2023-11-17 15:24:25.803736 couchformation-4.0.0a354/couchformation/docker/util.py
--rw-r--r--   0        0        0     2790 2024-03-26 18:46:14.516577 couchformation-4.0.0a354/couchformation/exception.py
--rw-r--r--   0        0        0        0 2023-08-29 15:42:02.837511 couchformation-4.0.0a354/couchformation/exec/__init__.py
--rw-r--r--   0        0        0      876 2024-01-10 21:47:39.481007 couchformation-4.0.0a354/couchformation/exec/process.py
--rw-r--r--   0        0        0        0 2023-11-02 01:40:35.138163 couchformation-4.0.0a354/couchformation/executor/__init__.py
--rw-r--r--   0        0        0     1103 2024-01-12 20:49:32.121168 couchformation-4.0.0a354/couchformation/executor/dispatch.py
--rw-r--r--   0        0        0    11667 2024-05-16 00:35:14.398285 couchformation-4.0.0a354/couchformation/executor/targets.py
--rw-r--r--   0        0        0      521 2023-10-17 14:42:59.612745 couchformation-4.0.0a354/couchformation/executor/taskqueue.py
--rw-r--r--   0        0        0      598 2024-01-02 17:20:41.808004 couchformation-4.0.0a354/couchformation/executor/worker.py
--rw-r--r--   0        0        0        0 2023-09-08 13:45:36.635733 couchformation-4.0.0a354/couchformation/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-09-08 17:48:51.884786 couchformation-4.0.0a354/couchformation/gcp/driver/__init__.py
--rw-r--r--   0        0        0     7628 2024-04-30 20:56:52.410370 couchformation-4.0.0a354/couchformation/gcp/driver/base.py
--rw-r--r--   0        0        0     3333 2024-01-23 22:39:02.477700 couchformation-4.0.0a354/couchformation/gcp/driver/constants.py
--rw-r--r--   0        0        0     3413 2024-01-25 19:10:07.609469 couchformation-4.0.0a354/couchformation/gcp/driver/disk.py
--rw-r--r--   0        0        0     5601 2024-03-25 22:34:34.688739 couchformation-4.0.0a354/couchformation/gcp/driver/dns.py
--rw-r--r--   0        0        0     4094 2024-04-25 19:02:14.722881 couchformation-4.0.0a354/couchformation/gcp/driver/firewall.py
--rw-r--r--   0        0        0     5103 2023-09-18 22:46:09.274171 couchformation-4.0.0a354/couchformation/gcp/driver/image.py
--rw-r--r--   0        0        0     7815 2024-04-22 18:18:28.423641 couchformation-4.0.0a354/couchformation/gcp/driver/instance.py
--rw-r--r--   0        0        0     3332 2023-09-12 13:04:14.169889 couchformation-4.0.0a354/couchformation/gcp/driver/machine.py
--rw-r--r--   0        0        0     8628 2024-03-25 22:26:58.105406 couchformation-4.0.0a354/couchformation/gcp/driver/network.py
--rw-r--r--   0        0        0    19619 2024-05-16 13:41:00.206875 couchformation-4.0.0a354/couchformation/gcp/network.py
--rw-r--r--   0        0        0    12030 2024-04-22 23:23:57.825354 couchformation-4.0.0a354/couchformation/gcp/node.py
--rw-r--r--   0        0        0     9203 2024-04-16 18:10:13.286398 couchformation-4.0.0a354/couchformation/kvdb.py
--rw-r--r--   0        0        0     1988 2023-11-20 20:32:05.946877 couchformation-4.0.0a354/couchformation/network.py
--rw-r--r--   0        0        0      331 2023-11-03 17:19:30.606393 couchformation-4.0.0a354/couchformation/null.py
--rw-r--r--   0        0        0    19560 2024-05-16 00:36:49.914474 couchformation-4.0.0a354/couchformation/project.py
--rw-r--r--   0        0        0        0 2023-08-30 23:18:42.303988 couchformation-4.0.0a354/couchformation/provisioner/__init__.py
--rw-r--r--   0        0        0     4105 2024-03-08 23:32:28.304554 couchformation-4.0.0a354/couchformation/provisioner/docker.py
--rw-r--r--   0        0        0      318 2023-10-12 04:30:47.897422 couchformation-4.0.0a354/couchformation/provisioner/provisioners.py
--rw-r--r--   0        0        0     8436 2024-04-29 17:00:59.413905 couchformation-4.0.0a354/couchformation/provisioner/remote.py
--rw-r--r--   0        0        0     3348 2024-03-08 22:22:58.860942 couchformation-4.0.0a354/couchformation/provisioner/sftp.py
--rw-r--r--   0        0        0     1837 2024-03-27 22:14:27.909240 couchformation-4.0.0a354/couchformation/provisioner/shell.py
--rw-r--r--   0        0        0     5671 2023-10-31 20:40:58.189889 couchformation-4.0.0a354/couchformation/provisioner/ssh.py
--rw-r--r--   0        0        0     5997 2024-04-29 17:00:59.420960 couchformation-4.0.0a354/couchformation/provisioner/winrm.py
--rw-r--r--   0        0        0    11611 2024-03-27 22:06:19.315729 couchformation-4.0.0a354/couchformation/restmgr.py
--rw-r--r--   0        0        0     2833 2023-11-01 22:24:12.512437 couchformation-4.0.0a354/couchformation/retry.py
--rw-r--r--   0        0        0     7976 2024-01-13 00:02:33.690890 couchformation-4.0.0a354/couchformation/ssh.py
--rw-r--r--   0        0        0    11449 2023-09-21 20:33:18.131180 couchformation-4.0.0a354/couchformation/state.py
--rw-r--r--   0        0        0        0 2024-04-09 14:24:33.869691 couchformation-4.0.0a354/couchformation/support/__init__.py
--rw-r--r--   0        0        0     7096 2024-05-01 14:26:20.534150 couchformation-4.0.0a354/couchformation/support/debug.py
--rw-r--r--   0        0        0     5588 2024-04-19 14:49:02.152490 couchformation-4.0.0a354/couchformation/util.py
--rw-r--r--   0        0        0     3039 2024-05-17 01:02:25.417695 couchformation-4.0.0a354/pyproject.toml
--rw-r--r--   0        0        0    12786 1970-01-01 00:00:00.000000 couchformation-4.0.0a354/PKG-INFO
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-09-21 21:03:08.071573 couchformation-4.0.0a9/
+-rw-r--r--   0 michael    (501) staff       (20)     1833 2023-09-21 21:03:08.071310 couchformation-4.0.0a9/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1042 2023-09-21 21:02:26.000000 couchformation-4.0.0a9/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-09-21 21:03:07.967487 couchformation-4.0.0a9/couchformation/
+-rw-r--r--   0 michael    (501) staff       (20)      163 2023-09-21 21:02:26.000000 couchformation-4.0.0a9/couchformation/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10098 2023-09-21 19:18:19.000000 couchformation-4.0.0a9/couchformation/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4922 2023-09-21 20:36:45.000000 couchformation-4.0.0a9/couchformation/constants.py
+-rw-r--r--   0 michael    (501) staff       (20)     4156 2023-09-21 18:42:19.000000 couchformation-4.0.0a9/couchformation/deployment.py
+-rw-r--r--   0 michael    (501) staff       (20)     1126 2023-09-15 15:04:28.000000 couchformation-4.0.0a9/couchformation/exception.py
+-rw-r--r--   0 michael    (501) staff       (20)     1596 2023-09-15 17:26:25.000000 couchformation-4.0.0a9/couchformation/network.py
+-rw-r--r--   0 michael    (501) staff       (20)     3027 2023-09-21 19:28:39.000000 couchformation-4.0.0a9/couchformation/project.py
+-rw-r--r--   0 michael    (501) staff       (20)     6591 2023-09-12 13:04:14.000000 couchformation-4.0.0a9/couchformation/ssh.py
+-rw-r--r--   0 michael    (501) staff       (20)    11449 2023-09-21 20:33:18.000000 couchformation-4.0.0a9/couchformation/state.py
+-rw-r--r--   0 michael    (501) staff       (20)     1720 2023-09-12 13:04:14.000000 couchformation-4.0.0a9/couchformation/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-09-21 21:03:08.069792 couchformation-4.0.0a9/couchformation.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1833 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      506 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       62 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/entry_points.txt
+-rw-r--r--   0 michael    (501) staff       (20)      824 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       15 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-09-21 21:03:08.071668 couchformation-4.0.0a9/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     2539 2023-09-12 13:14:30.000000 couchformation-4.0.0a9/setup.py
```

### Comparing `couchformation-4.0.0a354/couchformation/capella/node.py` & `couchformation-4.0.0a9/couchformation/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,259 +1,333 @@
 ##
 ##
 
-import logging
-from couchformation.exception import FatalError
-from couchformation.capella.driver.base import CloudBase
-from couchformation.config import get_state_file, get_state_dir
-from couchformation.kvdb import KeyValueStore
-from couchformation.util import FileManager, Synchronize
-from couchformation.capella.driver.cb_capella import Capella, CapellaCluster, AllowedCIDR, Credentials, AppService
-from couchformation.util import PasswordUtility
-
-logger = logging.getLogger('couchformation.capella.node')
-logger.addHandler(logging.NullHandler())
-
-
-class CapellaNodeError(FatalError):
-    pass
-
-
-class CapellaDeployment(object):
-
-    def __init__(self, parameters: dict):
-        self.parameters = parameters
-        self.name = parameters.get('name')
-        self.deploy_type = parameters.get('type') if parameters.get('type') else "database"
-        self.cluster_id = parameters.get('instance_id')
-        self.project = parameters.get('project')
-        self.region = parameters.get('region') if parameters.get('region') else "us-east-1"
-        self.cloud = parameters.get('cloud')
-        self.provider = parameters.get('provider') if parameters.get('provider') else "aws"
-        self.username = parameters.get('username') if parameters.get('username') else "Administrator"
-        self.password = parameters.get('password')
-        self.account_email = parameters.get('account_email')
-        self.profile = parameters.get('profile') if parameters.get('profile') else 'default'
-        self.sw_version = self.parameters.get('sw_version') if self.parameters.get('sw_version') else "latest"
-        self.cidr = parameters.get('cidr') if parameters.get('cidr') else "10.0.0.0/23"
-        self.allow = parameters.get('allow') if parameters.get('allow') else "0.0.0.0/0"
-        self.db_name = f"{self.name}-database"
-
-        self.state_file = get_state_file(self.project, self.name)
-        self.state_dir = get_state_dir(self.project, self.name)
-
-        with Synchronize():
-            try:
-                FileManager().make_dir(self.state_dir)
-            except Exception as err:
-                raise CapellaNodeError(f"can not create state dir: {err}")
-
-        document = self.db_name
-        self.state = KeyValueStore(self.state_file, document)
-
-        CloudBase(self.parameters).test_session()
-
-    def compose(self):
-        if self.deploy_type == "mobile":
-            self.compose_app_svc()
+import os
+from typing import Optional, Union, List
+from enum import Enum
+import attr
+import argparse
+import couchformation.constants as C
+
+
+def get_base_dir():
+    if 'COUCH_FORMATION_CONFIG_DIR' in os.environ:
+        return os.environ['COUCH_FORMATION_CONFIG_DIR']
+    else:
+        return C.STATE_DIRECTORY
+
+
+def get_log_dir():
+    if 'COUCH_FORMATION_LOG_DIR' in os.environ:
+        return os.environ['COUCH_FORMATION_LOG_DIR']
+    else:
+        return C.LOG_DIRECTORY
+
+
+def get_resource_dir(name: str, tag: str):
+    return os.path.join(get_base_dir(), name, tag)
+
+
+def get_project_dir(name: str):
+    return os.path.join(get_base_dir(), name)
+
+
+def str_to_int(value: Union[str, int]) -> int:
+    return int(value)
+
+
+class AuthMode(Enum):
+    default = 0
+    sso = 1
+
+
+class PathMode(Enum):
+    resource = 0
+    common = 1
+
+
+class ProvisionMode(Enum):
+    public = 0
+    private = 1
+
+
+@attr.s
+class Parameters:
+    project: Optional[str] = attr.ib(default=None)
+    cloud: Optional[str] = attr.ib(default=None)
+    name: Optional[str] = attr.ib(default=None)
+    model: Optional[str] = attr.ib(default=None)
+    region: Optional[str] = attr.ib(default=None)
+    ssh_key: Optional[str] = attr.ib(default=None)
+    os_id: Optional[str] = attr.ib(default=None)
+    os_version: Optional[str] = attr.ib(default=None)
+    auth_mode: Optional[str] = attr.ib(default=None)
+    profile: Optional[str] = attr.ib(default=None)
+    base_dir: Optional[str] = attr.ib(default=None)
+    private_ip: Optional[bool] = attr.ib(default=None)
+    path_mode: Optional[PathMode] = attr.ib(default=None)
+    machine_type: Optional[str] = attr.ib(default=None)
+    quantity: Optional[int] = attr.ib(default=None)
+    services: Optional[str] = attr.ib(default=None)
+    volume_iops: Optional[str] = attr.ib(default=None)
+    volume_size: Optional[str] = attr.ib(default=None)
+    volume_type: Optional[str] = attr.ib(default=None)
+    volume_tier: Optional[str] = attr.ib(default=None)
+    root_size: Optional[str] = attr.ib(default=None)
+    connect_svc: Optional[str] = attr.ib(default=None)
+    connect_ip: Optional[str] = attr.ib(default=None)
+
+    @classmethod
+    def create(cls, args):
+        c = cls()
+        c.initialize_args(args)
+        return c
+
+    def initialize_args(self, args):
+        parser = argparse.ArgumentParser(add_help=False)
+        for attribute in self.__annotations__:
+            parser.add_argument(f"--{attribute}", action='store')
+        parameters, remainder = parser.parse_known_args(args)
+        self.from_namespace(parameters)
+
+    def from_namespace(self, namespace: argparse.Namespace):
+        args = vars(namespace)
+        for attribute in self.__annotations__:
+            if args.get(attribute):
+                setattr(self, attribute, args.get(attribute))
+
+    def from_dict(self, options: dict):
+        for attribute in self.__annotations__:
+            if options.get(attribute):
+                setattr(self, attribute, options.get(attribute))
+
+    @property
+    def project_dir(self):
+        return get_project_dir(self.project)
+
+    @property
+    def as_dict(self):
+        return {k: self.__dict__[k] for k in self.__dict__ if self.__dict__[k] is not None}
+
+
+@attr.s
+class BaseConfig:
+    project: Optional[str] = attr.ib(default="resources")
+    ssh_key: Optional[str] = attr.ib(default=os.path.join(os.environ['HOME'], '.ssh', 'couch-formation-key.pem'))
+    base_dir: Optional[str] = attr.ib(default=get_base_dir())
+    private_ip: Optional[bool] = attr.ib(default=False)
+
+    @classmethod
+    def create(cls, data: Union[list, dict]):
+        if type(data) == list:
+            c = cls()
+            c.initialize_args(data)
         else:
-            self.compose_database()
-
-    def compose_app_svc(self):
-        number = self.parameters.get('number') if self.parameters.get('number') else 1
-        document = f"{self.name}-node-group-{number:02d}"
-        group = KeyValueStore(self.state_file, document)
-
-        group['machine_type'] = self.parameters.get('machine_type')
-        group['quantity'] = self.parameters.get('quantity') if self.parameters.get('quantity') else 2
-
-    def compose_database(self):
-        number = self.parameters.get('number') if self.parameters.get('number') else 1
-        document = f"{self.name}-node-group-{number:02d}"
-        group = KeyValueStore(self.state_file, document)
-
-        group['cloud'] = self.parameters.get('provider')
-        group['machine_type'] = self.parameters.get('machine_type')
-        group['volume_size'] = self.parameters.get('volume_size') if self.parameters.get('volume_size') else "256"
-        group['quantity'] = self.parameters.get('quantity') if self.parameters.get('quantity') else 3
-        group['services'] = self.parameters.get('services') if self.parameters.get('services') else "data,index,query"
-
-    def deploy(self):
-        if self.deploy_type == "mobile":
-            self.deploy_app_svc()
-        else:
-            self.deploy_database()
-
-    def deploy_app_svc(self):
-        state_db = KeyValueStore(self.state_file)
-        node_groups = state_db.doc_id_startswith(f"{self.name}-node-group")
-
-        if len(node_groups) == 0:
-            raise CapellaNodeError("no node groups present")
-
-        if self.state.get('project_id'):
-            project_id = self.state.get('project_id')
-        else:
-            project_data = Capella(profile=self.profile).get_project(self.project)
-            if not project_data:
-                raise CapellaNodeError(f"Project {self.project} does not exist, please create a database for app service {self.name}")
-            else:
-                project_id = project_data.get('id')
-
-        self.state['project'] = self.project
-        self.state['type'] = self.deploy_type
-
-        if not self.cluster_id:
-            raise CapellaNodeError(f"Please connect the app service {self.name} to a Capella database")
-
-        self.state['instance_id'] = self.cluster_id
-
-        for group in node_groups:
-            group_db = KeyValueStore(self.state_file, group)
-
-            if self.state.get('app_svc_id'):
-                logger.info(f"App service {self.name} already exists")
-                app_svc_id = self.state['app_svc_id']
-            else:
-                quantity = int(group_db.get('quantity'))
-                machine = group_db.get('machine_type')
-                logger.info(f"Creating app service {self.name} with {quantity} {machine} nodes")
-                app_svc = AppService.create(self.name, "CouchFormation managed app service", quantity, machine, self.sw_version)
-
-                app_svc_id = Capella(project_id=project_id, profile=self.profile).create_app_svc(self.cluster_id, app_svc)
-                self.state['name'] = self.name
-                self.state['app_svc_id'] = app_svc_id
-                logger.info("Waiting for app service creation to complete")
-                if not Capella(project_id=project_id, profile=self.profile).wait_for_app_svc(self.cluster_id):
-                    raise CapellaNodeError("Timeout waiting for app service to deploy")
-
-            logger.info(f"App service ID: {app_svc_id}")
-
-        logger.info("Capella app service successfully created")
-
-        return self.state.as_dict
-
-    def deploy_database(self):
-        state_db = KeyValueStore(self.state_file)
-        node_groups = state_db.doc_id_startswith(f"{self.name}-node-group")
-
-        if len(node_groups) == 0:
-            raise CapellaNodeError("no node groups present")
-
-        cluster = CapellaCluster().create(self.name, "CouchFormation managed cluster", self.provider, self.region, self.cidr, version=self.sw_version)
-
-        for group in node_groups:
-            group_db = KeyValueStore(self.state_file, group)
-            cluster.add_service_group(group_db.get('cloud'),
-                                      group_db.get('machine_type'),
-                                      int(group_db.get('volume_size')),
-                                      int(group_db.get('quantity')),
-                                      group_db.get('services').split(','))
-
-        if self.state.get('project_id'):
-            project_id = self.state.get('project_id')
+            c = cls()
+            c.initialize_dict(data)
+        return c
+
+    def initialize_args(self, args):
+        parser = argparse.ArgumentParser(add_help=False)
+        for attribute in self.__annotations__:
+            parser.add_argument(f"--{attribute}", action='store')
+        parameters, remainder = parser.parse_known_args(args)
+        self.from_namespace(parameters)
+
+    def initialize_dict(self, options):
+        self.from_dict(options)
+
+    @property
+    def project_dir(self):
+        return get_project_dir(self.project)
+
+    def from_namespace(self, namespace: argparse.Namespace):
+        args = vars(namespace)
+        for attribute in self.__annotations__:
+            if args.get(attribute):
+                setattr(self, attribute, args.get(attribute))
+
+    def from_dict(self, options: dict):
+        for attribute in self.__annotations__:
+            if options.get(attribute):
+                setattr(self, attribute, options.get(attribute))
+
+    @property
+    def as_dict(self):
+        return self.__dict__
+
+
+@attr.s
+class NodeConfig:
+    machine_type: Optional[str] = attr.ib(default=None)
+    quantity: Optional[int] = attr.ib(default=1, converter=str_to_int)
+    services: Optional[str] = attr.ib(default="default")
+    volume_iops: Optional[str] = attr.ib(default="3000")
+    volume_size: Optional[str] = attr.ib(default="256")
+    volume_type: Optional[str] = attr.ib(default=None)
+    root_size: Optional[str] = attr.ib(default="256")
+
+    @classmethod
+    def create(cls, data: Union[list, dict]):
+        if type(data) == list:
+            c = cls()
+            c.initialize_args(data)
         else:
-            project_data = Capella(profile=self.profile).get_project(self.project)
-            if not project_data:
-                logger.info(f"Creating project {self.project}")
-                project_id = Capella(profile=self.profile).create_project(self.project, self.account_email)
-                self.state['project_id'] = project_id
-            else:
-                project_id = project_data.get('id')
-
-        self.state['project'] = self.project
-        self.state['type'] = self.deploy_type
-
-        if self.state.get('instance_id'):
-            logger.info(f"Database {self.db_name} already exists")
-            cluster_id = self.state['instance_id']
+            c = cls()
+            c.initialize_dict(data)
+        return c
+
+    def initialize_args(self, args):
+        parser = argparse.ArgumentParser(add_help=False)
+        for attribute in self.__annotations__:
+            parser.add_argument(f"--{attribute}", action='store')
+        parameters, undefined = parser.parse_known_args(args)
+        self.from_namespace(parameters)
+
+    def initialize_dict(self, options):
+        self.from_dict(options)
+
+    def from_namespace(self, namespace: argparse.Namespace):
+        args = vars(namespace)
+        for attribute in self.__annotations__:
+            if args.get(attribute):
+                setattr(self, attribute, args.get(attribute))
+
+    def from_dict(self, options: dict):
+        for attribute in self.__annotations__:
+            if options.get(attribute):
+                setattr(self, attribute, options.get(attribute))
+
+    @property
+    def as_dict(self):
+        return self.__dict__
+
+
+@attr.s
+class DeploymentConfig:
+    core: Optional[BaseConfig] = attr.ib(default=BaseConfig())
+    config: Optional[List[NodeConfig]] = attr.ib(default=[])
+
+    def add_config(self, index: Union[str, int], config: NodeConfig):
+        index = int(index)
+        config.group = str(index)
+        if index > len(self.config) + 1:
+            raise ValueError(f"config index {index} out of range")
+        elif index == len(self.config) + 1:
+            self.config.append(config)
         else:
-            logger.info(f"Creating cluster {self.name}")
-            cluster_id = Capella(project_id=project_id, profile=self.profile).create_cluster(cluster)
-            self.state['instance_id'] = cluster_id
-            self.state['provider'] = self.provider
-            self.state['region'] = self.region
-            self.state['cidr'] = self.cidr
-            self.state['name'] = self.name
-            self.state['cloud'] = self.cloud
-            logger.info("Waiting for cluster creation to complete")
-            if not Capella(project_id=project_id, profile=self.profile).wait_for_cluster(self.name):
-                raise CapellaNodeError("Timeout waiting for cluster to deploy")
-
-        logger.info(f"Cluster ID: {cluster_id}")
-
-        cluster_info = Capella(project_id=project_id, profile=self.profile).get_cluster_by_id(cluster_id)
-        connect_string = cluster_info.get('connectionString')
-        self.state['connect_string'] = connect_string
-        logger.info(f"Connect string: {connect_string}")
+            self.config[index - 1] = config
 
-        if self.state.get('allow'):
-            logger.info(f"Allow list already set to {self.state.get('allow')}")
+    @classmethod
+    def new(cls, core: BaseConfig):
+        return cls(
+            core,
+            []
+        )
+
+    def reset(self, args):
+        self.config.clear()
+        self.core = BaseConfig().create(args)
+
+    @property
+    def length(self):
+        return len(self.config)
+
+    @property
+    def as_dict(self):
+        return self.__dict__
+
+
+@attr.s
+class NodeEntry:
+    name: Optional[str] = attr.ib(default=None)
+    username: Optional[str] = attr.ib(default=None)
+    private_ip: Optional[str] = attr.ib(default=None)
+    public_ip: Optional[str] = attr.ib(default=None)
+    use_private_ip: Optional[bool] = attr.ib(default=False)
+    availability_zone: Optional[str] = attr.ib(default=None)
+    services: Optional[str] = attr.ib(default=None)
+    connect_svc: Optional[str] = attr.ib(default=None)
+    connect_ip: Optional[str] = attr.ib(default=None)
+
+    @classmethod
+    def create(cls,
+               name: str,
+               username: str,
+               private_ip: str,
+               public_ip: str = None,
+               use_private_ip: bool = False,
+               zone: str = None,
+               services: str = "default",
+               connect_svc: str = None,
+               connect_ip: str = None
+               ):
+        return cls(
+            name,
+            username,
+            private_ip,
+            public_ip,
+            use_private_ip,
+            zone,
+            services,
+            connect_svc,
+            connect_ip
+        )
+
+
+@attr.s
+class NodeList:
+    username: Optional[str] = attr.ib(default=None)
+    ssh_key: Optional[str] = attr.ib(default=None)
+    nodes: Optional[List[NodeEntry]] = attr.ib(default=[])
+    working_dir: Optional[str] = attr.ib(default=None)
+    provision_ip: Optional[ProvisionMode] = attr.ib(default=ProvisionMode.public)
+
+    @classmethod
+    def create(cls, username: str, ssh_key: str, working_dir: str = None, use_private_ip: bool = False):
+        return cls(
+            username,
+            ssh_key,
+            [],
+            working_dir,
+            ProvisionMode(use_private_ip)
+        )
+
+    def add(self, name: str, private_ip: str, public_ip: str = None, zone: str = None, services: str = "default", connect_svc: str = None, connect_ip: str = None):
+        self.nodes.append(
+            NodeEntry.create(
+                name,
+                self.username,
+                private_ip,
+                public_ip,
+                bool(self.provision_ip.value),
+                zone,
+                services,
+                connect_svc,
+                connect_ip
+            )
+        )
+
+    @property
+    def node_list(self) -> List[NodeEntry]:
+        return self.nodes
+
+    def list_public_ip(self):
+        address_list = []
+        for entry in self.nodes:
+            address_list.append(entry.public_ip)
+        return address_list
+
+    def list_private_ip(self):
+        address_list = []
+        for entry in self.nodes:
+            address_list.append(entry.private_ip)
+        return address_list
+
+    def provision_list(self):
+        if self.provision_ip == ProvisionMode.public:
+            return self.list_public_ip()
         else:
-            allow_cidr = AllowedCIDR().create(self.allow)
-            logger.info(f"Configuring allowed CIDR {self.allow}")
-            Capella(project_id=project_id, profile=self.profile).allow_cidr(cluster_id, allow_cidr)
-            self.state['allow'] = self.allow
-
-        if self.state.get('username'):
-            logger.info(f"Database user {self.state.get('username')} already exists")
-        else:
-            if self.password:
-                password = self.password
-            else:
-                password = PasswordUtility().generate(16)
-                self.state['password'] = password
-                logger.info(f"Password: {password}")
-            credentials = Credentials().create(self.username, password)
-            logger.info(f"Creating database user {self.username}")
-            Capella(project_id=project_id, profile=self.profile).add_db_user(cluster_id, credentials)
-            self.state['username'] = self.username
-
-        logger.info("Capella database successfully created")
-
-        return self.state.as_dict
-
-    def destroy(self):
-        project = self.state.get('project')
-        if not project:
-            return
-        project_data = Capella(profile=self.profile).get_project(project)
-        project_id = project_data.get('id')
-        logger.info(f"Project {project} ID {project_id}")
-
-        if self.state.get('type') == "mobile":
-            self.destroy_app_svc(project_id)
-        else:
-            self.destroy_database(project, project_id)
-
-    def destroy_app_svc(self, project_id):
-        app_svc_name = self.state['name']
-        cluster_id = self.state['instance_id']
-
-        logger.info(f"Destroying app service {app_svc_name}")
-        Capella(project_id=project_id, profile=self.profile).delete_app_svc(cluster_id)
-        logger.info("Waiting for app service deletion to complete")
-        if not Capella(project_id=project_id, profile=self.profile).wait_for_app_svc_delete(cluster_id):
-            raise CapellaNodeError("Timeout waiting for app service deletion to complete")
-
-        self.state.clear()
-
-    def destroy_database(self, project, project_id):
-        cluster_name = self.state['name'] = self.name
-        logger.info(f"Destroying cluster {cluster_name}")
-        Capella(project_id=project_id, profile=self.profile).delete_cluster(cluster_name)
-        logger.info("Waiting for cluster deletion to complete")
-        if not Capella(project_id=project_id, profile=self.profile).wait_for_cluster_delete(cluster_name):
-            raise CapellaNodeError("Timeout waiting for cluster deletion to complete")
-
-        if self.state.get('project_id'):
-            cluster_list = Capella(project_id=project_id, profile=self.profile).list_clusters()
-            if len(cluster_list) == 0:
-                logger.info(f"Removing project {project}")
-                Capella(profile=self.profile).delete_project(project)
-            else:
-                logger.warning(f"Project {project} has active clusters, it will not be removed")
-
-        self.state.clear()
+            return self.list_private_ip()
 
-    def info(self):
-        return self.state.as_dict
+    def ip_csv_list(self):
+        return ','.join(self.list_private_ip())
```

### Comparing `couchformation-4.0.0a354/couchformation/network.py` & `couchformation-4.0.0a9/couchformation/network.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 ##
 ##
 
-import socket
 import ipaddress
 from ipaddress import IPv4Network
 import logging
 from typing import Union
 
 
 class NetworkDriver(object):
@@ -44,22 +43,7 @@
 
         if len(candidates) == 0:
             return None
 
         self.active_network = candidates[0]
         self.ip_space.append(self.active_network)
         return self.active_network.exploded
-
-
-class NetworkUtil(object):
-
-    @staticmethod
-    def local_ip_address():
-        try:
-            socket.setdefaulttimeout(2)
-            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-            s.connect(("8.8.8.8", 80))
-            local_ip = s.getsockname()[0]
-            s.close()
-            return local_ip
-        except TimeoutError:
-            return None
```

### Comparing `couchformation-4.0.0a354/couchformation/ssh.py` & `couchformation-4.0.0a9/couchformation/ssh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 ##
 ##
 
 import logging
 import os
-import rsa
 from enum import Enum
 from typing import Union, List
 from Crypto.PublicKey import RSA
-from Crypto.Util.number import long_to_bytes
-from Crypto.Cipher import PKCS1_OAEP
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 import hashlib
 from cryptography.exceptions import UnsupportedAlgorithm
 from couchformation.exception import FatalError, NonFatalError
 
 logger = logging.getLogger('couchformation.ssh')
@@ -51,25 +48,14 @@
         for location in SSH_PATHS:
             for file_found in os.listdir(location):
                 if file_found == name or next((f"{name}{e.value}" for e in SSHExtensions if f"{name}{e.value}" == file_found), None):
                     return location + '/' + file_found
         return None
 
     @staticmethod
-    def decrypt_with_key(encrypted_data: bytes, key_file: str) -> str:
-        try:
-            with open(key_file, 'r') as file_handle:
-                blob = file_handle.read()
-                private_key = rsa.PrivateKey.load_pkcs1(blob.encode('latin-1'))
-                decrypted = rsa.decrypt(encrypted_data, private_key)
-                return decrypted.decode('utf-8')
-        except OSError as err:
-            raise SSHError(f"can not read key file {key_file}: {err}.")
-
-    @staticmethod
     def list_private_key_files() -> Union[List[dict], None]:
         dir_list = []
         key_file_list = []
 
         for location in SSH_PATHS:
             for file_name in os.listdir(location):
                 full_path = location + '/' + file_name
@@ -143,37 +129,14 @@
         prime_q = rsa_key.q
         private_key = RSA.construct((modulus, pub_exp_e, pri_exp_d, prime_p, prime_q))
         public_key = private_key.public_key().exportKey('OpenSSH')
         ssh_public_key = public_key.decode('utf-8')
         return ssh_public_key
 
     @staticmethod
-    def get_mod_exp(key_file: str):
-        if not os.path.isabs(key_file):
-            key_file = SSHUtil.ssh_key_absolute_path(key_file)
-        fh = open(key_file, 'r')
-        key_pem = fh.read()
-        fh.close()
-        rsa_key = RSA.importKey(key_pem)
-        modulus = long_to_bytes(rsa_key.n)
-        exponent = long_to_bytes(rsa_key.e)
-        return modulus, exponent
-
-    @staticmethod
-    def decrypt_with_rsa(encrypted_data: bytes, key_file: str):
-        if not os.path.isabs(key_file):
-            key_file = SSHUtil.ssh_key_absolute_path(key_file)
-        fh = open(key_file, 'r')
-        key_pem = fh.read()
-        fh.close()
-        rsa_key = RSA.importKey(key_pem)
-        cipher = PKCS1_OAEP.new(rsa_key)
-        return cipher.decrypt(encrypted_data)
-
-    @staticmethod
     def write_file(file_name: str, data: str) -> bool:
         try:
             file_handle = open(file_name, 'w')
             file_handle.write(data)
             file_handle.write("\n")
             file_handle.close()
             return True
```

### Comparing `couchformation-4.0.0a354/couchformation/state.py` & `couchformation-4.0.0a9/couchformation/state.py`

 * *Files identical despite different names*

