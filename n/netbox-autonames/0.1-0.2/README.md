# Comparing `tmp/netbox_autonames-0.1.tar.gz` & `tmp/netbox_autonames-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_autonames-0.1.tar", last modified: Wed Sep  6 15:34:04 2023, max compression
+gzip compressed data, was "netbox_autonames-0.2.tar", last modified: Mon Nov 27 10:22:47 2023, max compression
```

## Comparing `netbox_autonames-0.1.tar` & `netbox_autonames-0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 15:34:04.805487 netbox_autonames-0.1/
--rw-r--r--   0 root         (0) root         (0)      278 2023-09-06 15:34:04.804487 netbox_autonames-0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 15:34:04.803487 netbox_autonames-0.1/netbox_autonames/
--rw-r--r--   0 root         (0) root         (0)      439 2023-09-06 15:33:23.000000 netbox_autonames-0.1/netbox_autonames/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-09-06 15:33:23.000000 netbox_autonames-0.1/netbox_autonames/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 15:34:04.804487 netbox_autonames-0.1/netbox_autonames.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2023-09-06 15:34:04.000000 netbox_autonames-0.1/netbox_autonames.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      264 2023-09-06 15:34:04.000000 netbox_autonames-0.1/netbox_autonames.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-06 15:34:04.000000 netbox_autonames-0.1/netbox_autonames.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-06 15:33:23.000000 netbox_autonames-0.1/netbox_autonames.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2023-09-06 15:34:04.000000 netbox_autonames-0.1/netbox_autonames.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-06 15:34:04.805487 netbox_autonames-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      389 2023-09-06 15:33:23.000000 netbox_autonames-0.1/setup.py
+drwxr-xr-x   0 fej       (1000) fej       (1001)        0 2023-11-27 10:22:47.163654 netbox_autonames-0.2/
+-rw-r--r--   0 fej       (1000) fej       (1001)    34547 2023-11-27 10:21:37.000000 netbox_autonames-0.2/LICENSE
+-rw-r--r--   0 fej       (1000) fej       (1001)      239 2023-11-27 10:22:47.162654 netbox_autonames-0.2/PKG-INFO
+-rw-r--r--   0 fej       (1000) fej       (1001)     2006 2023-11-27 10:21:37.000000 netbox_autonames-0.2/README.md
+drwxr-xr-x   0 fej       (1000) fej       (1001)        0 2023-11-27 10:22:47.162654 netbox_autonames-0.2/netbox_autonames/
+-rw-r--r--   0 fej       (1000) fej       (1001)      439 2023-11-27 10:21:37.000000 netbox_autonames-0.2/netbox_autonames/__init__.py
+-rw-r--r--   0 fej       (1000) fej       (1001)     1140 2023-11-27 10:21:37.000000 netbox_autonames-0.2/netbox_autonames/signals.py
+drwxr-xr-x   0 fej       (1000) fej       (1001)        0 2023-11-27 10:22:47.162654 netbox_autonames-0.2/netbox_autonames.egg-info/
+-rw-r--r--   0 fej       (1000) fej       (1001)      239 2023-11-27 10:22:47.000000 netbox_autonames-0.2/netbox_autonames.egg-info/PKG-INFO
+-rw-r--r--   0 fej       (1000) fej       (1001)      282 2023-11-27 10:22:47.000000 netbox_autonames-0.2/netbox_autonames.egg-info/SOURCES.txt
+-rw-r--r--   0 fej       (1000) fej       (1001)        1 2023-11-27 10:22:47.000000 netbox_autonames-0.2/netbox_autonames.egg-info/dependency_links.txt
+-rw-r--r--   0 fej       (1000) fej       (1001)        1 2023-11-27 10:22:47.000000 netbox_autonames-0.2/netbox_autonames.egg-info/not-zip-safe
+-rw-r--r--   0 fej       (1000) fej       (1001)       17 2023-11-27 10:22:47.000000 netbox_autonames-0.2/netbox_autonames.egg-info/top_level.txt
+-rw-r--r--   0 fej       (1000) fej       (1001)       38 2023-11-27 10:22:47.163654 netbox_autonames-0.2/setup.cfg
+-rw-r--r--   0 fej       (1000) fej       (1001)      389 2023-11-27 10:22:03.000000 netbox_autonames-0.2/setup.py
```

### Comparing `netbox_autonames-0.1/netbox_autonames/signals.py` & `netbox_autonames-0.2/netbox_autonames/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 from django.conf import settings
 import re
 
 @receiver(pre_save, sender=Device)
 def auto_generate_device_name(sender, instance, **kwargs):
     try:
         if not instance.name:
-            role = instance.device_role.slug
+            role = instance.role.slug
             device_name_map = settings.PLUGINS_CONFIG['netbox_autonames'].get('DEVICE_NAME_MAP', {})
             prefix = device_name_map.get(role)
             if prefix:
                 pattern = re.compile(f'^{prefix}(\d+)$')
-                existing_devices = Device.objects.filter(device_role__slug=role)
+                existing_devices = Device.objects.filter(role__slug=role)
                 max_num = 0
                 for device in existing_devices:
                     if device.name is None:
                         continue
                     match = pattern.match(device.name)
                     if match:
                         num = int(match.group(1))
                         if num > max_num:
                             max_num = num
                 next_num = max_num + 1
                 instance.name = f"{prefix}{next_num:04d}"
     except Exception as e:
         pass
-
```

