# Comparing `tmp/ovp_docker_utils-1.0.8.tar.gz` & `tmp/ovp_docker_utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovp_docker_utils-1.0.8.tar", last modified: Sat Apr 27 21:07:12 2024, max compression
+gzip compressed data, was "ovp_docker_utils-1.0.9.tar", last modified: Fri May 17 20:17:03 2024, max compression
```

## Comparing `ovp_docker_utils-1.0.8.tar` & `ovp_docker_utils-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 21:07:12.765952 ovp_docker_utils-1.0.8/
--rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      380 2024-04-27 21:07:12.764359 ovp_docker_utils-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 21:07:12.725133 ovp_docker_utils-1.0.8/ovp_docker_utils/
--rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-27 21:05:02.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/__version__.py
--rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/defaults.py
--rw-rw-rw-   0        0        0     2427 2024-04-27 06:28:50.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/docker_compose_instance.py
--rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/oem_logging.py
--rw-rw-rw-   0        0        0    33916 2024-04-27 06:44:01.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/ovp_docker_utils.py
--rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/ssh_file_utils.py
--rw-rw-rw-   0        0        0     3948 2024-04-03 15:53:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/ssh_key_gen.py
-drwxrwxrwx   0        0        0        0 2024-04-27 21:07:12.763278 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/
--rw-rw-rw-   0        0        0      380 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 21:07:12.766480 ovp_docker_utils-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:17:03.498654 ovp_docker_utils-1.0.9/
+-rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      380 2024-05-17 20:17:03.497602 ovp_docker_utils-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 20:17:03.464077 ovp_docker_utils-1.0.9/ovp_docker_utils/
+-rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.9/ovp_docker_utils/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-05-17 20:16:39.000000 ovp_docker_utils-1.0.9/ovp_docker_utils/__version__.py
+-rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.9/ovp_docker_utils/defaults.py
+-rw-rw-rw-   0        0        0     2494 2024-05-17 20:14:31.000000 ovp_docker_utils-1.0.9/ovp_docker_utils/docker_compose_instance.py
+-rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.9/ovp_docker_utils/oem_logging.py
+-rw-rw-rw-   0        0        0    34129 2024-05-09 15:37:35.000000 ovp_docker_utils-1.0.9/ovp_docker_utils/ovp_docker_utils.py
+-rw-rw-rw-   0        0        0     6556 2024-05-07 13:25:08.000000 ovp_docker_utils-1.0.9/ovp_docker_utils/ssh_file_utils.py
+-rw-rw-rw-   0        0        0     3948 2024-05-06 22:03:20.000000 ovp_docker_utils-1.0.9/ovp_docker_utils/ssh_key_gen.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:17:03.496025 ovp_docker_utils-1.0.9/ovp_docker_utils.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-05-17 20:17:03.000000 ovp_docker_utils-1.0.9/ovp_docker_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-17 20:17:03.000000 ovp_docker_utils-1.0.9/ovp_docker_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 20:17:03.000000 ovp_docker_utils-1.0.9/ovp_docker_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-05-17 20:17:03.000000 ovp_docker_utils-1.0.9/ovp_docker_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2024-05-17 20:17:03.000000 ovp_docker_utils-1.0.9/ovp_docker_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 20:17:03.000000 ovp_docker_utils-1.0.9/ovp_docker_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 20:17:03.499184 ovp_docker_utils-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.9/setup.py
```

### Comparing `ovp_docker_utils-1.0.8/LICENSE` & `ovp_docker_utils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.8/README.md` & `ovp_docker_utils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.8/ovp_docker_utils/docker_compose_instance.py` & `ovp_docker_utils-1.0.9/ovp_docker_utils/docker_compose_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,26 +24,29 @@
     # otherwise, load from a tar file on the host machine
     docker_image_src_on_pc: str = None
     docker_image_dst_on_vpu: str = None
 
     docker_compose: dict = {}
 
     @model_validator(mode='after')
-    def validate_constraints(self) -> 'DockerComposeServiceInstance':
+    def _validate(self) -> 'DockerComposeServiceInstance':
         if not (self.docker_compose_src_on_pc.endswith(".yml") or self.docker_compose_src_on_pc.endswith(".yaml")):
             raise ValueError(
                 "docker_compose_src_on_pc must be a path to a yaml file")
         if not self.docker_compose:
             with open(self.docker_compose_src_on_pc, "r") as f:
                 self.docker_compose = yaml.load(f, yaml.BaseLoader)
-        else:
-            with open(self.docker_compose_src_on_pc, "w") as f:
-                yaml.dump(self.docker_compose, f)
         return self
 
+    def write_docker_compose(self, path: str = None):
+        if not path:
+            path = self.docker_compose_src_on_pc
+        with open(path, "w") as f:
+            yaml.dump(self.docker_compose, f)
+
     @property
     def service_name(self):
         return list(self.docker_compose["services"].keys())[0]
 
     @property
     def docker_repository_name(self):
         return self.docker_compose["services"][self.service_name]["image"]
```

### Comparing `ovp_docker_utils-1.0.8/ovp_docker_utils/oem_logging.py` & `ovp_docker_utils-1.0.9/ovp_docker_utils/oem_logging.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.8/ovp_docker_utils/ovp_docker_utils.py` & `ovp_docker_utils-1.0.9/ovp_docker_utils/ovp_docker_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,21 +332,25 @@
             logger.info("ifm3dpy unavailable")
         if USING_IFM3DPY:
             if len(self.config.possible_initial_ip_addresses_to_try) ==0:
                 VPU_config = ifm3dpy.O3R(self.config.IP).get()
                 logger.info(f"Connected to {self.config.IP}")
                 self._connected = True
             else:
-                possible_initial_ip_addresses = list(
-                    set([self.config.IP] + self.config.possible_initial_ip_addresses_to_try))
+                possible_initial_ip_addresses = self.config.possible_initial_ip_addresses_to_try
+                if self.config.IP not in possible_initial_ip_addresses:
+                    possible_initial_ip_addresses.insert(0, self.config.IP)
                 logger.info(
                     f"Trying to connect to VPU at any of the following addresses: {possible_initial_ip_addresses}")
 
                 for temp_IP in possible_initial_ip_addresses:
-                    VPU_config = ifm3dpy.O3R(temp_IP).get()
+                    try:
+                        VPU_config = ifm3dpy.O3R(temp_IP).get()
+                    except ifm3dpy.device.Error as e:
+                        continue
                     logger.info(f"Connected to {temp_IP}")
                     self._connected = True
                     break
                 if not self._connected:
                     logger.info(
                         f"VPU could not be found at any of the following addresses: {possible_initial_ip_addresses}")
                 elif temp_IP != self.config.IP:
```

### Comparing `ovp_docker_utils-1.0.8/ovp_docker_utils/ssh_file_utils.py` & `ovp_docker_utils-1.0.9/ovp_docker_utils/ssh_file_utils.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.8/ovp_docker_utils/ssh_key_gen.py` & `ovp_docker_utils-1.0.9/ovp_docker_utils/ssh_key_gen.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/SOURCES.txt` & `ovp_docker_utils-1.0.9/ovp_docker_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.8/setup.py` & `ovp_docker_utils-1.0.9/setup.py`

 * *Files identical despite different names*

