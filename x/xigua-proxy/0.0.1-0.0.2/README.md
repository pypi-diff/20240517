# Comparing `tmp/xigua_proxy-0.0.1.tar.gz` & `tmp/xigua_proxy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xigua_proxy-0.0.1.tar", last modified: Fri May 17 07:47:00 2024, max compression
+gzip compressed data, was "xigua_proxy-0.0.2.tar", last modified: Fri May 17 08:51:47 2024, max compression
```

## Comparing `xigua_proxy-0.0.1.tar` & `xigua_proxy-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 07:47:00.815155 xigua_proxy-0.0.1/
--rw-rw-rw-   0        0        0      128 2024-05-17 07:47:00.814157 xigua_proxy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        5 2024-05-09 08:09:24.000000 xigua_proxy-0.0.1/README.txt
--rw-rw-rw-   0        0        0       52 2024-04-06 07:14:29.000000 xigua_proxy-0.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 07:47:00.815155 xigua_proxy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      251 2024-05-17 07:46:40.000000 xigua_proxy-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:47:00.799006 xigua_proxy-0.0.1/xigua_proxy/
--rw-rw-rw-   0        0        0       32 2024-05-17 05:08:06.000000 xigua_proxy-0.0.1/xigua_proxy/__init__.py
--rw-rw-rw-   0        0        0     4013 2024-05-17 07:32:32.000000 xigua_proxy-0.0.1/xigua_proxy/xigua_porxy.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:47:00.814157 xigua_proxy-0.0.1/xigua_proxy.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-17 07:47:00.000000 xigua_proxy-0.0.1/xigua_proxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-05-17 07:47:00.000000 xigua_proxy-0.0.1/xigua_proxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:47:00.000000 xigua_proxy-0.0.1/xigua_proxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 07:47:00.000000 xigua_proxy-0.0.1/xigua_proxy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 08:51:47.858850 xigua_proxy-0.0.2/
+-rw-rw-rw-   0        0        0      128 2024-05-17 08:51:47.857852 xigua_proxy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2024-05-09 08:09:24.000000 xigua_proxy-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       52 2024-04-06 07:14:29.000000 xigua_proxy-0.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 08:51:47.858850 xigua_proxy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      251 2024-05-17 08:51:05.000000 xigua_proxy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:51:47.845885 xigua_proxy-0.0.2/xigua_proxy/
+-rw-rw-rw-   0        0        0       32 2024-05-17 05:08:06.000000 xigua_proxy-0.0.2/xigua_proxy/__init__.py
+-rw-rw-rw-   0        0        0     4139 2024-05-17 08:50:33.000000 xigua_proxy-0.0.2/xigua_proxy/xigua_porxy.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:51:47.857852 xigua_proxy-0.0.2/xigua_proxy.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-17 08:51:47.000000 xigua_proxy-0.0.2/xigua_proxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-05-17 08:51:47.000000 xigua_proxy-0.0.2/xigua_proxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 08:51:47.000000 xigua_proxy-0.0.2/xigua_proxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 08:51:47.000000 xigua_proxy-0.0.2/xigua_proxy.egg-info/top_level.txt
```

### Comparing `xigua_proxy-0.0.1/xigua_proxy/xigua_porxy.py` & `xigua_proxy-0.0.2/xigua_proxy/xigua_porxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import os
 import requests
 import datetime
 import re
 import time
 import socket
 warnings.filterwarnings('ignore')
+"""
+需要传入 订单的 secret_id 和 secret_key
+"""
 
 
 class MyProxy(object):
 
     def __init__(self, secret_id, secret_key):
         self.secret_id = secret_id
         self.secret_key = secret_key
@@ -32,16 +35,19 @@
         headers = {
             "User-Agent": 'Mozilla/5.0'
         }
         auth = kdl.Auth(secret_id=secret_id, secret_key=secret_key)
         client = kdl.Client(auth)
 
         def ip_address():
-            _response = requests.get("https://api.ipify.org/?format=json")
-            _ip = _response.json()["ip"]
+            try:
+                _response = requests.get("https://api.ipify.org/?format=json")
+                _ip = _response.json()["ip"]
+            except:
+                _ip = ''
             return str(_ip)
 
         my_ip = ip_address()
         try:
             ip_whitelist = client.get_ip_whitelist()  # 检查ip白名单, 如果这句报错，就直接设置白名单
             if my_ip not in ip_whitelist:
                 ip_whitelist.append(my_ip)
```

