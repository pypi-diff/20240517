# Comparing `tmp/keymateapi-0.3.3.tar.gz` & `tmp/keymateapi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keymateapi-0.3.3.tar", last modified: Fri Mar 22 17:19:24 2024, max compression
+gzip compressed data, was "keymateapi-0.4.0.tar", last modified: Fri May 17 15:45:53 2024, max compression
```

## Comparing `keymateapi-0.3.3.tar` & `keymateapi-0.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.270111 keymateapi-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-03-22 17:19:24.270111 keymateapi-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-03-22 17:19:15.000000 keymateapi-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 17:19:24.270111 keymateapi-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-22 17:19:15.000000 keymateapi-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.266111 keymateapi-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.266111 keymateapi-0.3.3/src/keymateapi/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.266111 keymateapi-0.3.3/src/keymateapi/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/_hooks/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.266111 keymateapi-0.3.3/src/keymateapi/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.270111 keymateapi-0.3.3/src/keymateapi/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/components/browseresultitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/components/browsewithproxyresultitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/components/searchresultitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.270111 keymateapi-0.3.3/src/keymateapi/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/errors/browse.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/errors/browseurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/errors/gptsbrowse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/errors/internetsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/errors/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/errors/ultrafastsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.270111 keymateapi-0.3.3/src/keymateapi/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/operations/browse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/operations/browseurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/operations/gptsbrowse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/operations/internetsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/operations/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/operations/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/operations/ultrafastsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/models/operations/upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    36136 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.270111 keymateapi-0.3.3/src/keymateapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    29904 2024-03-22 17:19:15.000000 keymateapi-0.3.3/src/keymateapi/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:19:24.266111 keymateapi-0.3.3/src/keymateapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-03-22 17:19:24.000000 keymateapi-0.3.3/src/keymateapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-22 17:19:24.000000 keymateapi-0.3.3/src/keymateapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:19:24.000000 keymateapi-0.3.3/src/keymateapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-22 17:19:24.000000 keymateapi-0.3.3/src/keymateapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 17:19:24.000000 keymateapi-0.3.3/src/keymateapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.249991 keymateapi-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-05-17 15:45:53.249991 keymateapi-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-17 15:45:45.000000 keymateapi-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:45:53.249991 keymateapi-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-17 15:45:45.000000 keymateapi-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.241991 keymateapi-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.245991 keymateapi-0.4.0/src/keymateapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.245991 keymateapi-0.4.0/src/keymateapi/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/_hooks/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.245991 keymateapi-0.4.0/src/keymateapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.245991 keymateapi-0.4.0/src/keymateapi/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/components/browseresultitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/components/browsewithproxyresultitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/components/searchresultitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.245991 keymateapi-0.4.0/src/keymateapi/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/errors/browse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/errors/browseurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/errors/gptsbrowse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/errors/internetsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/errors/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/errors/ultrafastsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.249991 keymateapi-0.4.0/src/keymateapi/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/operations/browse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/operations/browseurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/operations/gptsbrowse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/operations/internetsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/operations/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/operations/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/operations/ultrafastsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/models/operations/upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38757 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.249991 keymateapi-0.4.0/src/keymateapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-17 15:45:45.000000 keymateapi-0.4.0/src/keymateapi/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:45:53.245991 keymateapi-0.4.0/src/keymateapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-05-17 15:45:53.000000 keymateapi-0.4.0/src/keymateapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-17 15:45:53.000000 keymateapi-0.4.0/src/keymateapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:45:53.000000 keymateapi-0.4.0/src/keymateapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 15:45:53.000000 keymateapi-0.4.0/src/keymateapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 15:45:53.000000 keymateapi-0.4.0/src/keymateapi.egg-info/top_level.txt
```

### Comparing `keymateapi-0.3.3/PKG-INFO` & `keymateapi-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,590 +1,555 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6b65 796d  : 2.1.Name: keym
 00000020: 6174 6561 7069 0a56 6572 7369 6f6e 3a20  ateapi.Version: 
-00000030: 302e 332e 330a 5375 6d6d 6172 793a 2050  0.3.3.Summary: P
+00000030: 302e 342e 300a 5375 6d6d 6172 793a 2050  0.4.0.Summary: P
 00000040: 7974 686f 6e20 436c 6965 6e74 2053 444b  ython Client SDK
 00000050: 2047 656e 6572 6174 6564 2062 7920 5370   Generated by Sp
 00000060: 6561 6b65 6173 790a 486f 6d65 2d70 6167  eakeasy.Home-pag
-00000070: 653a 2055 4e4b 4e4f 574e 0a41 7574 686f  e: UNKNOWN.Autho
-00000080: 723a 2053 7065 616b 6561 7379 0a4c 6963  r: Speakeasy.Lic
-00000090: 656e 7365 3a20 554e 4b4e 4f57 4e0a 4465  ense: UNKNOWN.De
-000000a0: 7363 7269 7074 696f 6e3a 2023 206b 6579  scription: # key
-000000b0: 6d61 7465 6170 690a 2020 2020 2020 2020  mateapi.        
-000000c0: 0a20 2020 2020 2020 203c 6469 7620 616c  .        <div al
-000000d0: 6967 6e3d 226c 6566 7422 3e0a 2020 2020  ign="left">.    
-000000e0: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-000000f0: 2268 7474 7073 3a2f 2f73 7065 616b 6561  "https://speakea
-00000100: 7379 6170 692e 6465 762f 223e 3c69 6d67  syapi.dev/"><img
-00000110: 2073 7263 3d22 6874 7470 733a 2f2f 6375   src="https://cu
-00000120: 7374 6f6d 2d69 636f 6e2d 6261 6467 6573  stom-icon-badges
-00000130: 2e64 656d 6f6c 6162 2e63 6f6d 2f62 6164  .demolab.com/bad
-00000140: 6765 2f2d 4275 696c 7425 3230 4279 2532  ge/-Built%20By%2
-00000150: 3053 7065 616b 6561 7379 2d32 3132 3031  0Speakeasy-21201
-00000160: 353f 7374 796c 653d 666f 722d 7468 652d  5?style=for-the-
-00000170: 6261 6467 6526 6c6f 676f 436f 6c6f 723d  badge&logoColor=
-00000180: 4642 4533 3331 266c 6f67 6f3d 7370 6561  FBE331&logo=spea
-00000190: 6b65 6173 7926 6c61 6265 6c43 6f6c 6f72  keasy&labelColor
-000001a0: 3d35 3435 3435 3422 202f 3e3c 2f61 3e0a  =545454" /></a>.
-000001b0: 2020 2020 2020 2020 2020 2020 3c61 2068              <a h
-000001c0: 7265 663d 2268 7474 7073 3a2f 2f6f 7065  ref="https://ope
-000001d0: 6e73 6f75 7263 652e 6f72 672f 6c69 6365  nsource.org/lice
-000001e0: 6e73 6573 2f4d 4954 223e 0a20 2020 2020  nses/MIT">.     
-000001f0: 2020 2020 2020 2020 2020 203c 696d 6720             <img 
-00000200: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000210: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000220: 652f 4c69 6365 6e73 652d 4d49 542d 626c  e/License-MIT-bl
-00000230: 7565 2e73 7667 2220 7374 796c 653d 2277  ue.svg" style="w
-00000240: 6964 7468 3a20 3130 3070 783b 2068 6569  idth: 100px; hei
-00000250: 6768 743a 2032 3870 783b 2220 2f3e 0a20  ght: 28px;" />. 
-00000260: 2020 2020 2020 2020 2020 203c 2f61 3e0a             </a>.
-00000270: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000280: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000290: 0a20 2020 2020 2020 2023 2320 f09f 8f97  .        ## ....
-000002a0: 202a 2a57 656c 636f 6d65 2074 6f20 796f   **Welcome to yo
-000002b0: 7572 206e 6577 2053 444b 212a 2a20 f09f  ur new SDK!** ..
-000002c0: 8f97 0a20 2020 2020 2020 200a 2020 2020  ...        .    
-000002d0: 2020 2020 4974 2068 6173 2062 6565 6e20      It has been 
-000002e0: 6765 6e65 7261 7465 6420 7375 6363 6573  generated succes
-000002f0: 7366 756c 6c79 2062 6173 6564 206f 6e20  sfully based on 
-00000300: 796f 7572 204f 7065 6e41 5049 2073 7065  your OpenAPI spe
-00000310: 632e 2048 6f77 6576 6572 2c20 6974 2069  c. However, it i
-00000320: 7320 6e6f 7420 7965 7420 7265 6164 7920  s not yet ready 
-00000330: 666f 7220 7072 6f64 7563 7469 6f6e 2075  for production u
-00000340: 7365 2e20 4865 7265 2061 7265 2073 6f6d  se. Here are som
-00000350: 6520 6e65 7874 2073 7465 7073 3a0a 2020  e next steps:.  
-00000360: 2020 2020 2020 2d20 5b20 5d20 f09f 9ba0        - [ ] ....
-00000370: 204d 616b 6520 796f 7572 2053 444b 2066   Make your SDK f
-00000380: 6565 6c20 6861 6e64 6372 6166 7465 6420  eel handcrafted 
-00000390: 6279 205b 6375 7374 6f6d 697a 696e 6720  by [customizing 
-000003a0: 6974 5d28 6874 7470 733a 2f2f 7777 772e  it](https://www.
-000003b0: 7370 6561 6b65 6173 7961 7069 2e64 6576  speakeasyapi.dev
-000003c0: 2f64 6f63 732f 6375 7374 6f6d 697a 652d  /docs/customize-
-000003d0: 7364 6b73 290a 2020 2020 2020 2020 2d20  sdks).        - 
-000003e0: 5b20 5d20 e299 bbef b88f 2052 6566 696e  [ ] ...... Refin
-000003f0: 6520 796f 7572 2053 444b 2071 7569 636b  e your SDK quick
-00000400: 6c79 2062 7920 6974 6572 6174 696e 6720  ly by iterating 
-00000410: 6c6f 6361 6c6c 7920 7769 7468 2074 6865  locally with the
-00000420: 205b 5370 6561 6b65 6173 7920 434c 495d   [Speakeasy CLI]
-00000430: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000440: 636f 6d2f 7370 6561 6b65 6173 792d 6170  com/speakeasy-ap
-00000450: 692f 7370 6561 6b65 6173 7929 0a20 2020  i/speakeasy).   
-00000460: 2020 2020 202d 205b 205d 20f0 9f8e 8120       - [ ] .... 
-00000470: 5075 626c 6973 6820 796f 7572 2053 444b  Publish your SDK
-00000480: 2074 6f20 7061 636b 6167 6520 6d61 6e61   to package mana
-00000490: 6765 7273 2062 7920 5b63 6f6e 6669 6775  gers by [configu
-000004a0: 7269 6e67 2061 7574 6f6d 6174 6963 2070  ring automatic p
-000004b0: 7562 6c69 7368 696e 675d 2868 7474 7073  ublishing](https
-000004c0: 3a2f 2f77 7777 2e73 7065 616b 6561 7379  ://www.speakeasy
-000004d0: 6170 692e 6465 762f 646f 6373 2f70 726f  api.dev/docs/pro
-000004e0: 6475 6374 696f 6e69 7a65 2d73 646b 732f  ductionize-sdks/
-000004f0: 7075 626c 6973 682d 7364 6b73 290a 2020  publish-sdks).  
-00000500: 2020 2020 2020 2d20 5b20 5d20 e29c a820        - [ ] ... 
-00000510: 5768 656e 2072 6561 6479 2074 6f20 7072  When ready to pr
-00000520: 6f64 7563 7469 6f6e 697a 652c 2064 656c  oductionize, del
-00000530: 6574 6520 7468 6973 2073 6563 7469 6f6e  ete this section
-00000540: 2066 726f 6d20 7468 6520 5245 4144 4d45   from the README
-00000550: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000560: 2020 3c21 2d2d 2053 7461 7274 2053 444b    <!-- Start SDK
-00000570: 2049 6e73 7461 6c6c 6174 696f 6e20 5b69   Installation [i
-00000580: 6e73 7461 6c6c 6174 696f 6e5d 202d 2d3e  nstallation] -->
-00000590: 0a20 2020 2020 2020 2023 2320 5344 4b20  .        ## SDK 
-000005a0: 496e 7374 616c 6c61 7469 6f6e 0a20 2020  Installation.   
-000005b0: 2020 2020 200a 2020 2020 2020 2020 6060       .        ``
-000005c0: 6062 6173 680a 2020 2020 2020 2020 7069  `bash.        pi
-000005d0: 7020 696e 7374 616c 6c20 6b65 796d 6174  p install keymat
-000005e0: 6561 7069 0a20 2020 2020 2020 2060 6060  eapi.        ```
-000005f0: 0a20 2020 2020 2020 203c 212d 2d20 456e  .        <!-- En
-00000600: 6420 5344 4b20 496e 7374 616c 6c61 7469  d SDK Installati
-00000610: 6f6e 205b 696e 7374 616c 6c61 7469 6f6e  on [installation
-00000620: 5d20 2d2d 3e0a 2020 2020 2020 2020 0a20  ] -->.        . 
-00000630: 2020 2020 2020 203c 212d 2d20 5374 6172         <!-- Star
-00000640: 7420 5344 4b20 4578 616d 706c 6520 5573  t SDK Example Us
-00000650: 6167 6520 5b75 7361 6765 5d20 2d2d 3e0a  age [usage] -->.
-00000660: 2020 2020 2020 2020 2323 2053 444b 2045          ## SDK E
-00000670: 7861 6d70 6c65 2055 7361 6765 0a20 2020  xample Usage.   
-00000680: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000690: 2320 4578 616d 706c 650a 2020 2020 2020  # Example.      
-000006a0: 2020 0a20 2020 2020 2020 2060 6060 7079    .        ```py
-000006b0: 7468 6f6e 0a20 2020 2020 2020 2069 6d70  thon.        imp
-000006c0: 6f72 7420 6b65 796d 6174 6561 7069 0a20  ort keymateapi. 
-000006d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000006e0: 7320 3d20 6b65 796d 6174 6561 7069 2e4b  s = keymateapi.K
-000006f0: 6579 6d61 7465 6170 6928 0a20 2020 2020  eymateapi(.     
-00000700: 2020 2020 2020 2062 6561 7265 725f 6175         bearer_au
-00000710: 7468 3d22 3c59 4f55 525f 4245 4152 4552  th="<YOUR_BEARER
-00000720: 5f54 4f4b 454e 5f48 4552 453e 222c 0a20  _TOKEN_HERE>",. 
-00000730: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00000740: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
-00000750: 2020 2072 6573 203d 2073 2e75 7073 6572     res = s.upser
-00000760: 7428 713d 273c 7661 6c75 653e 2729 0a20  t(q='<value>'). 
-00000770: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000780: 6966 2072 6573 2e6f 626a 6563 7420 6973  if res.object is
-00000790: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000007a0: 2020 2020 2020 2023 2068 616e 646c 6520         # handle 
-000007b0: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
-000007c0: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-000007d0: 2020 0a20 2020 2020 2020 2060 6060 0a20    .        ```. 
-000007e0: 2020 2020 2020 203c 212d 2d20 456e 6420         <!-- End 
-000007f0: 5344 4b20 4578 616d 706c 6520 5573 6167  SDK Example Usag
-00000800: 6520 5b75 7361 6765 5d20 2d2d 3e0a 2020  e [usage] -->.  
-00000810: 2020 2020 2020 0a20 2020 2020 2020 203c        .        <
-00000820: 212d 2d20 5374 6172 7420 4176 6169 6c61  !-- Start Availa
-00000830: 626c 6520 5265 736f 7572 6365 7320 616e  ble Resources an
-00000840: 6420 4f70 6572 6174 696f 6e73 205b 6f70  d Operations [op
-00000850: 6572 6174 696f 6e73 5d20 2d2d 3e0a 2020  erations] -->.  
-00000860: 2020 2020 2020 2323 2041 7661 696c 6162        ## Availab
-00000870: 6c65 2052 6573 6f75 7263 6573 2061 6e64  le Resources and
-00000880: 204f 7065 7261 7469 6f6e 730a 2020 2020   Operations.    
-00000890: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
-000008a0: 205b 4b65 796d 6174 6561 7069 2053 444b   [Keymateapi SDK
-000008b0: 5d28 646f 6373 2f73 646b 732f 6b65 796d  ](docs/sdks/keym
-000008c0: 6174 6561 7069 2f52 4541 444d 452e 6d64  ateapi/README.md
-000008d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000008e0: 2020 202a 205b 7570 7365 7274 5d28 646f     * [upsert](do
-000008f0: 6373 2f73 646b 732f 6b65 796d 6174 6561  cs/sdks/keymatea
-00000900: 7069 2f52 4541 444d 452e 6d64 2375 7073  pi/README.md#ups
-00000910: 6572 7429 202d 2049 6e73 6572 7473 2072  ert) - Inserts r
-00000920: 6563 6f72 6420 746f 204b 6579 6d61 7465  ecord to Keymate
-00000930: 204d 656d 6f72 792e 0a20 2020 2020 2020   Memory..       
-00000940: 202a 205b 7175 6572 795d 2864 6f63 732f   * [query](docs/
-00000950: 7364 6b73 2f6b 6579 6d61 7465 6170 692f  sdks/keymateapi/
-00000960: 5245 4144 4d45 2e6d 6423 7175 6572 7929  README.md#query)
-00000970: 202d 2051 7565 7269 6573 2074 6865 2075   - Queries the u
-00000980: 7365 7227 7320 4b65 796d 6174 6520 4d65  ser's Keymate Me
-00000990: 6d6f 7279 2e0a 2020 2020 2020 2020 2a20  mory..        * 
-000009a0: 5b62 726f 7773 6575 726c 5d28 646f 6373  [browseurl](docs
-000009b0: 2f73 646b 732f 6b65 796d 6174 6561 7069  /sdks/keymateapi
-000009c0: 2f52 4541 444d 452e 6d64 2362 726f 7773  /README.md#brows
-000009d0: 6575 726c 2920 2d20 5468 6520 706c 7567  eurl) - The plug
-000009e0: 696e 2065 6e61 626c 6573 2075 7365 7220  in enables user 
-000009f0: 746f 2063 6f6e 6475 6374 2077 6562 2062  to conduct web b
-00000a00: 726f 7773 696e 6720 6279 2065 7874 7261  rowsing by extra
-00000a10: 6374 696e 6720 7468 6520 7465 7874 2063  cting the text c
-00000a20: 6f6e 7465 6e74 206f 6620 6120 7370 6563  ontent of a spec
-00000a30: 6966 6965 6420 5552 4c2e 2049 7420 7769  ified URL. It wi
-00000a40: 6c6c 2067 656e 6572 6174 6520 7469 746c  ll generate titl
-00000a50: 6520 616e 6420 636f 6e74 656e 742e 0a20  e and content.. 
-00000a60: 2020 2020 2020 202a 205b 6272 6f77 7365         * [browse
-00000a70: 5d28 646f 6373 2f73 646b 732f 6b65 796d  ](docs/sdks/keym
-00000a80: 6174 6561 7069 2f52 4541 444d 452e 6d64  ateapi/README.md
-00000a90: 2362 726f 7773 6529 202d 2046 6574 6368  #browse) - Fetch
-00000aa0: 2061 6e79 2055 524c 7320 7769 7468 6f75   any URLs withou
-00000ab0: 7420 7072 6f78 7920 6974 2077 6f75 6c64  t proxy it would
-00000ac0: 2070 726f 6261 626c 7920 6661 696c 206f   probably fail o
-00000ad0: 6e20 6d61 6a6f 7220 7765 6273 6974 6573  n major websites
-00000ae0: 2062 7574 2071 7569 636b 6572 2074 6861   but quicker tha
-00000af0: 6e20 6272 6f77 7365 7572 6c20 0a20 2020  n browseurl .   
-00000b00: 2020 2020 202a 205b 7365 6172 6368 5d28       * [search](
-00000b10: 646f 6373 2f73 646b 732f 6b65 796d 6174  docs/sdks/keymat
-00000b20: 6561 7069 2f52 4541 444d 452e 6d64 2373  eapi/README.md#s
-00000b30: 6561 7263 6829 202d 2057 6974 686f 7574  earch) - Without
-00000b40: 2070 726f 7869 6573 2073 6561 7263 6865   proxies searche
-00000b50: 7320 6b65 7977 6f72 6420 6f6e 2074 6865  s keyword on the
-00000b60: 2069 6e74 6572 6e65 7420 616e 6420 6665   internet and fe
-00000b70: 7463 6865 7320 7572 6c73 2061 6e64 206f  tches urls and o
-00000b80: 7074 696d 697a 6573 206f 7574 7075 740a  ptimizes output.
-00000b90: 2020 2020 2020 2020 2a20 5b75 6c74 7261          * [ultra
-00000ba0: 6661 7374 7365 6172 6368 5d28 646f 6373  fastsearch](docs
-00000bb0: 2f73 646b 732f 6b65 796d 6174 6561 7069  /sdks/keymateapi
-00000bc0: 2f52 4541 444d 452e 6d64 2375 6c74 7261  /README.md#ultra
-00000bd0: 6661 7374 7365 6172 6368 2920 2d20 5468  fastsearch) - Th
-00000be0: 6973 2070 6c75 6769 6e20 7072 6f76 6964  is plugin provid
-00000bf0: 6573 2031 3020 756c 7472 6120 6661 7374  es 10 ultra fast
-00000c00: 2073 6561 7263 6820 7265 7375 6c74 7320   search results 
-00000c10: 6672 6f6d 206d 756c 7469 706c 6520 736f  from multiple so
-00000c20: 7572 6365 7320 6769 7669 6e67 2061 206d  urces giving a m
-00000c30: 6f72 6520 636f 6d70 7265 6865 6e73 6976  ore comprehensiv
-00000c40: 6520 7669 6577 2e0a 2020 2020 2020 2020  e view..        
-00000c50: 2a20 5b67 7074 7362 726f 7773 655d 2864  * [gptsbrowse](d
-00000c60: 6f63 732f 7364 6b73 2f6b 6579 6d61 7465  ocs/sdks/keymate
-00000c70: 6170 692f 5245 4144 4d45 2e6d 6423 6770  api/README.md#gp
-00000c80: 7473 6272 6f77 7365 2920 2d20 4665 7463  tsbrowse) - Fetc
-00000c90: 6820 6d65 6d6f 7279 2e6b 6579 6d61 7465  h memory.keymate
-00000ca0: 2e61 6920 5552 4c73 0a20 2020 2020 2020  .ai URLs.       
-00000cb0: 202a 205b 696e 7465 726e 6574 7365 6172   * [internetsear
-00000cc0: 6368 5d28 646f 6373 2f73 646b 732f 6b65  ch](docs/sdks/ke
-00000cd0: 796d 6174 6561 7069 2f52 4541 444d 452e  ymateapi/README.
-00000ce0: 6d64 2369 6e74 6572 6e65 7473 6561 7263  md#internetsearc
-00000cf0: 6829 202d 2043 6f6e 6475 6374 2061 6e20  h) - Conduct an 
-00000d00: 696e 7465 726e 6574 2073 6561 7263 680a  internet search.
-00000d10: 2020 2020 2020 2020 3c21 2d2d 2045 6e64          <!-- End
-00000d20: 2041 7661 696c 6162 6c65 2052 6573 6f75   Available Resou
-00000d30: 7263 6573 2061 6e64 204f 7065 7261 7469  rces and Operati
-00000d40: 6f6e 7320 5b6f 7065 7261 7469 6f6e 735d  ons [operations]
-00000d50: 202d 2d3e 0a20 2020 2020 2020 200a 2020   -->.        .  
-00000d60: 2020 2020 2020 3c21 2d2d 2053 7461 7274        <!-- Start
-00000d70: 2045 7272 6f72 2048 616e 646c 696e 6720   Error Handling 
-00000d80: 5b65 7272 6f72 735d 202d 2d3e 0a20 2020  [errors] -->.   
-00000d90: 2020 2020 2023 2320 4572 726f 7220 4861       ## Error Ha
-00000da0: 6e64 6c69 6e67 0a20 2020 2020 2020 200a  ndling.        .
-00000db0: 2020 2020 2020 2020 4861 6e64 6c69 6e67          Handling
-00000dc0: 2065 7272 6f72 7320 696e 2074 6869 7320   errors in this 
-00000dd0: 5344 4b20 7368 6f75 6c64 206c 6172 6765  SDK should large
-00000de0: 6c79 206d 6174 6368 2079 6f75 7220 6578  ly match your ex
-00000df0: 7065 6374 6174 696f 6e73 2e20 2041 6c6c  pectations.  All
-00000e00: 206f 7065 7261 7469 6f6e 7320 7265 7475   operations retu
-00000e10: 726e 2061 2072 6573 706f 6e73 6520 6f62  rn a response ob
-00000e20: 6a65 6374 206f 7220 7261 6973 6520 616e  ject or raise an
-00000e30: 2065 7272 6f72 2e20 2049 6620 4572 726f   error.  If Erro
-00000e40: 7220 6f62 6a65 6374 7320 6172 6520 7370  r objects are sp
-00000e50: 6563 6966 6965 6420 696e 2079 6f75 7220  ecified in your 
-00000e60: 4f70 656e 4150 4920 5370 6563 2c20 7468  OpenAPI Spec, th
-00000e70: 6520 5344 4b20 7769 6c6c 2072 6169 7365  e SDK will raise
-00000e80: 2074 6865 2061 7070 726f 7072 6961 7465   the appropriate
-00000e90: 2045 7272 6f72 2074 7970 652e 0a20 2020   Error type..   
-00000ea0: 2020 2020 200a 2020 2020 2020 2020 7c20       .        | 
-00000eb0: 4572 726f 7220 4f62 6a65 6374 2020 2020  Error Object    
-00000ec0: 2020 2020 2020 2020 2020 2020 207c 2053               | S
-00000ed0: 7461 7475 7320 436f 6465 2020 2020 2020  tatus Code      
-00000ee0: 2020 2020 2020 2020 2020 2020 7c20 436f              | Co
-00000ef0: 6e74 656e 7420 5479 7065 2020 2020 2020  ntent Type      
-00000f00: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-00000f10: 2020 2020 207c 202d 2d2d 2d2d 2d2d 2d2d       | ---------
-00000f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f30: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
-00000f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f50: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d  -- | -----------
-00000f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f70: 2d20 7c0a 2020 2020 2020 2020 7c20 6572  - |.        | er
-00000f80: 726f 7273 2e42 726f 7773 6575 726c 5265  rors.BrowseurlRe
-00000f90: 7370 6f6e 7365 426f 6479 207c 2034 3030  sponseBody | 400
-00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fb0: 2020 2020 2020 2020 2020 7c20 6170 706c            | appl
-00000fc0: 6963 6174 696f 6e2f 6a73 6f6e 2020 2020  ication/json    
-00000fd0: 2020 2020 2020 2020 207c 0a20 2020 2020           |.     
-00000fe0: 2020 207c 2065 7272 6f72 732e 5344 4b45     | errors.SDKE
-00000ff0: 7272 6f72 2020 2020 2020 2020 2020 2020  rror            
-00001000: 2020 7c20 3478 2d35 7878 2020 2020 2020    | 4x-5xx      
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 207c 202a 2f2a 2020 2020 2020 2020 2020   | */*          
-00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001040: 7c0a 2020 2020 2020 2020 0a20 2020 2020  |.        .     
-00001050: 2020 2023 2323 2045 7861 6d70 6c65 0a20     ### Example. 
-00001060: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001070: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-00001080: 2020 696d 706f 7274 206b 6579 6d61 7465    import keymate
-00001090: 6170 690a 2020 2020 2020 2020 6672 6f6d  api.        from
-000010a0: 206b 6579 6d61 7465 6170 692e 6d6f 6465   keymateapi.mode
-000010b0: 6c73 2069 6d70 6f72 7420 6572 726f 7273  ls import errors
-000010c0: 2c20 6f70 6572 6174 696f 6e73 0a20 2020  , operations.   
-000010d0: 2020 2020 200a 2020 2020 2020 2020 7320       .        s 
-000010e0: 3d20 6b65 796d 6174 6561 7069 2e4b 6579  = keymateapi.Key
-000010f0: 6d61 7465 6170 6928 0a20 2020 2020 2020  mateapi(.       
-00001100: 2020 2020 2062 6561 7265 725f 6175 7468       bearer_auth
-00001110: 3d22 3c59 4f55 525f 4245 4152 4552 5f54  ="<YOUR_BEARER_T
-00001120: 4f4b 454e 5f48 4552 453e 222c 0a20 2020  OKEN_HERE>",.   
-00001130: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
-00001140: 2020 2020 2020 2020 7265 7120 3d20 6f70          req = op
-00001150: 6572 6174 696f 6e73 2e42 726f 7773 6575  erations.Browseu
-00001160: 726c 5265 7175 6573 7428 0a20 2020 2020  rlRequest(.     
-00001170: 2020 2020 2020 2069 6e70 7574 7769 6e64         inputwind
-00001180: 6f77 776f 7264 733d 273c 7661 6c75 653e  owwords='<value>
-00001190: 272c 0a20 2020 2020 2020 2020 2020 2071  ',.            q
-000011a0: 3d27 6874 7470 733a 2f2f 6167 7265 6561  ='https://agreea
-000011b0: 626c 652d 6a75 6d62 6f2e 6e65 7427 2c0a  ble-jumbo.net',.
-000011c0: 2020 2020 2020 2020 2020 2020 7065 7263              perc
-000011d0: 656e 7469 6c65 3d27 3c76 616c 7565 3e27  entile='<value>'
-000011e0: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
-000011f0: 6d6f 6670 6167 6573 3d27 3c76 616c 7565  mofpages='<value
-00001200: 3e27 2c0a 2020 2020 2020 2020 290a 2020  >',.        ).  
-00001210: 2020 2020 2020 0a20 2020 2020 2020 2072        .        r
-00001220: 6573 203d 204e 6f6e 650a 2020 2020 2020  es = None.      
-00001230: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00001240: 2020 2072 6573 203d 2073 2e62 726f 7773     res = s.brows
-00001250: 6575 726c 2872 6571 290a 2020 2020 2020  eurl(req).      
-00001260: 2020 6578 6365 7074 2065 7272 6f72 732e    except errors.
-00001270: 4272 6f77 7365 7572 6c52 6573 706f 6e73  BrowseurlRespons
-00001280: 6542 6f64 7920 6173 2065 3a0a 2020 2020  eBody as e:.    
-00001290: 2020 2020 2020 2020 2320 6861 6e64 6c65          # handle
-000012a0: 2065 7863 6570 7469 6f6e 0a20 2020 2020   exception.     
-000012b0: 2020 2020 2020 2072 6169 7365 2865 290a         raise(e).
-000012c0: 2020 2020 2020 2020 6578 6365 7074 2065          except e
-000012d0: 7272 6f72 732e 5344 4b45 7272 6f72 2061  rrors.SDKError a
-000012e0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-000012f0: 2023 2068 616e 646c 6520 6578 6365 7074   # handle except
-00001300: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00001310: 7261 6973 6528 6529 0a20 2020 2020 2020  raise(e).       
-00001320: 200a 2020 2020 2020 2020 6966 2072 6573   .        if res
-00001330: 2e74 776f 5f68 756e 6472 6564 5f61 7070  .two_hundred_app
-00001340: 6c69 6361 7469 6f6e 5f6a 736f 6e5f 6f62  lication_json_ob
-00001350: 6a65 6374 2069 7320 6e6f 7420 4e6f 6e65  ject is not None
-00001360: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00001370: 6861 6e64 6c65 2072 6573 706f 6e73 650a  handle response.
-00001380: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00001390: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000013a0: 2020 6060 600a 2020 2020 2020 2020 3c21    ```.        <!
-000013b0: 2d2d 2045 6e64 2045 7272 6f72 2048 616e  -- End Error Han
-000013c0: 646c 696e 6720 5b65 7272 6f72 735d 202d  dling [errors] -
-000013d0: 2d3e 0a20 2020 2020 2020 200a 2020 2020  ->.        .    
-000013e0: 2020 2020 3c21 2d2d 2053 7461 7274 2053      <!-- Start S
-000013f0: 6572 7665 7220 5365 6c65 6374 696f 6e20  erver Selection 
-00001400: 5b73 6572 7665 725d 202d 2d3e 0a20 2020  [server] -->.   
-00001410: 2020 2020 2023 2320 5365 7276 6572 2053       ## Server S
-00001420: 656c 6563 7469 6f6e 0a20 2020 2020 2020  election.       
-00001430: 200a 2020 2020 2020 2020 2323 2320 5365   .        ### Se
-00001440: 6c65 6374 2053 6572 7665 7220 6279 2049  lect Server by I
-00001450: 6e64 6578 0a20 2020 2020 2020 200a 2020  ndex.        .  
-00001460: 2020 2020 2020 596f 7520 6361 6e20 6f76        You can ov
-00001470: 6572 7269 6465 2074 6865 2064 6566 6175  erride the defau
-00001480: 6c74 2073 6572 7665 7220 676c 6f62 616c  lt server global
-00001490: 6c79 2062 7920 7061 7373 696e 6720 6120  ly by passing a 
-000014a0: 7365 7276 6572 2069 6e64 6578 2074 6f20  server index to 
-000014b0: 7468 6520 6073 6572 7665 725f 6964 783a  the `server_idx:
-000014c0: 2069 6e74 6020 6f70 7469 6f6e 616c 2070   int` optional p
-000014d0: 6172 616d 6574 6572 2077 6865 6e20 696e  arameter when in
-000014e0: 6974 6961 6c69 7a69 6e67 2074 6865 2053  itializing the S
-000014f0: 444b 2063 6c69 656e 7420 696e 7374 616e  DK client instan
-00001500: 6365 2e20 5468 6520 7365 6c65 6374 6564  ce. The selected
-00001510: 2073 6572 7665 7220 7769 6c6c 2074 6865   server will the
-00001520: 6e20 6265 2075 7365 6420 6173 2074 6865  n be used as the
-00001530: 2064 6566 6175 6c74 206f 6e20 7468 6520   default on the 
-00001540: 6f70 6572 6174 696f 6e73 2074 6861 7420  operations that 
-00001550: 7573 6520 6974 2e20 5468 6973 2074 6162  use it. This tab
-00001560: 6c65 206c 6973 7473 2074 6865 2069 6e64  le lists the ind
-00001570: 6578 6573 2061 7373 6f63 6961 7465 6420  exes associated 
-00001580: 7769 7468 2074 6865 2061 7661 696c 6162  with the availab
-00001590: 6c65 2073 6572 7665 7273 3a0a 2020 2020  le servers:.    
-000015a0: 2020 2020 0a20 2020 2020 2020 207c 2023      .        | #
-000015b0: 207c 2053 6572 7665 7220 7c20 5661 7269   | Server | Vari
-000015c0: 6162 6c65 7320 7c0a 2020 2020 2020 2020  ables |.        
-000015d0: 7c20 2d20 7c20 2d2d 2d2d 2d2d 207c 202d  | - | ------ | -
-000015e0: 2d2d 2d2d 2d2d 2d2d 207c 0a20 2020 2020  -------- |.     
-000015f0: 2020 207c 2030 207c 2060 6874 7470 733a     | 0 | `https:
-00001600: 2f2f 7365 7276 6572 2e73 6561 7263 6877  //server.searchw
-00001610: 6562 2e6b 6579 6d61 7465 2e61 6960 207c  eb.keymate.ai` |
-00001620: 204e 6f6e 6520 7c0a 2020 2020 2020 2020   None |.        
-00001630: 0a20 2020 2020 2020 2023 2323 2320 4578  .        #### Ex
-00001640: 616d 706c 650a 2020 2020 2020 2020 0a20  ample.        . 
-00001650: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-00001660: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00001670: 6b65 796d 6174 6561 7069 0a20 2020 2020  keymateapi.     
-00001680: 2020 200a 2020 2020 2020 2020 7320 3d20     .        s = 
-00001690: 6b65 796d 6174 6561 7069 2e4b 6579 6d61  keymateapi.Keyma
-000016a0: 7465 6170 6928 0a20 2020 2020 2020 2020  teapi(.         
-000016b0: 2020 2073 6572 7665 725f 6964 783d 302c     server_idx=0,
-000016c0: 0a20 2020 2020 2020 2020 2020 2062 6561  .            bea
-000016d0: 7265 725f 6175 7468 3d22 3c59 4f55 525f  rer_auth="<YOUR_
-000016e0: 4245 4152 4552 5f54 4f4b 454e 5f48 4552  BEARER_TOKEN_HER
-000016f0: 453e 222c 0a20 2020 2020 2020 2029 0a20  E>",.        ). 
-00001700: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001710: 0a20 2020 2020 2020 2072 6573 203d 2073  .        res = s
-00001720: 2e75 7073 6572 7428 713d 273c 7661 6c75  .upsert(q='<valu
-00001730: 653e 2729 0a20 2020 2020 2020 200a 2020  e>').        .  
-00001740: 2020 2020 2020 6966 2072 6573 2e6f 626a        if res.obj
-00001750: 6563 7420 6973 206e 6f74 204e 6f6e 653a  ect is not None:
-00001760: 0a20 2020 2020 2020 2020 2020 2023 2068  .            # h
-00001770: 616e 646c 6520 7265 7370 6f6e 7365 0a20  andle response. 
-00001780: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00001790: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000017a0: 2060 6060 0a20 2020 2020 2020 200a 2020   ```.        .  
-000017b0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000017c0: 2323 204f 7665 7272 6964 6520 5365 7276  ## Override Serv
-000017d0: 6572 2055 524c 2050 6572 2d43 6c69 656e  er URL Per-Clien
-000017e0: 740a 2020 2020 2020 2020 0a20 2020 2020  t.        .     
-000017f0: 2020 2054 6865 2064 6566 6175 6c74 2073     The default s
-00001800: 6572 7665 7220 6361 6e20 616c 736f 2062  erver can also b
-00001810: 6520 6f76 6572 7269 6464 656e 2067 6c6f  e overridden glo
-00001820: 6261 6c6c 7920 6279 2070 6173 7369 6e67  bally by passing
-00001830: 2061 2055 524c 2074 6f20 7468 6520 6073   a URL to the `s
-00001840: 6572 7665 725f 7572 6c3a 2073 7472 6020  erver_url: str` 
-00001850: 6f70 7469 6f6e 616c 2070 6172 616d 6574  optional paramet
-00001860: 6572 2077 6865 6e20 696e 6974 6961 6c69  er when initiali
-00001870: 7a69 6e67 2074 6865 2053 444b 2063 6c69  zing the SDK cli
-00001880: 656e 7420 696e 7374 616e 6365 2e20 466f  ent instance. Fo
-00001890: 7220 6578 616d 706c 653a 0a20 2020 2020  r example:.     
-000018a0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-000018b0: 2020 2020 2069 6d70 6f72 7420 6b65 796d       import keym
-000018c0: 6174 6561 7069 0a20 2020 2020 2020 200a  ateapi.        .
-000018d0: 2020 2020 2020 2020 7320 3d20 6b65 796d          s = keym
-000018e0: 6174 6561 7069 2e4b 6579 6d61 7465 6170  ateapi.Keymateap
-000018f0: 6928 0a20 2020 2020 2020 2020 2020 2073  i(.            s
-00001900: 6572 7665 725f 7572 6c3d 2268 7474 7073  erver_url="https
-00001910: 3a2f 2f73 6572 7665 722e 7365 6172 6368  ://server.search
-00001920: 7765 622e 6b65 796d 6174 652e 6169 222c  web.keymate.ai",
-00001930: 0a20 2020 2020 2020 2020 2020 2062 6561  .            bea
-00001940: 7265 725f 6175 7468 3d22 3c59 4f55 525f  rer_auth="<YOUR_
-00001950: 4245 4152 4552 5f54 4f4b 454e 5f48 4552  BEARER_TOKEN_HER
-00001960: 453e 222c 0a20 2020 2020 2020 2029 0a20  E>",.        ). 
-00001970: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001980: 0a20 2020 2020 2020 2072 6573 203d 2073  .        res = s
-00001990: 2e75 7073 6572 7428 713d 273c 7661 6c75  .upsert(q='<valu
-000019a0: 653e 2729 0a20 2020 2020 2020 200a 2020  e>').        .  
-000019b0: 2020 2020 2020 6966 2072 6573 2e6f 626a        if res.obj
-000019c0: 6563 7420 6973 206e 6f74 204e 6f6e 653a  ect is not None:
-000019d0: 0a20 2020 2020 2020 2020 2020 2023 2068  .            # h
-000019e0: 616e 646c 6520 7265 7370 6f6e 7365 0a20  andle response. 
-000019f0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00001a00: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001a10: 2060 6060 0a20 2020 2020 2020 203c 212d   ```.        <!-
-00001a20: 2d20 456e 6420 5365 7276 6572 2053 656c  - End Server Sel
-00001a30: 6563 7469 6f6e 205b 7365 7276 6572 5d20  ection [server] 
-00001a40: 2d2d 3e0a 2020 2020 2020 2020 0a20 2020  -->.        .   
-00001a50: 2020 2020 203c 212d 2d20 5374 6172 7420       <!-- Start 
-00001a60: 4375 7374 6f6d 2048 5454 5020 436c 6965  Custom HTTP Clie
-00001a70: 6e74 205b 6874 7470 2d63 6c69 656e 745d  nt [http-client]
-00001a80: 202d 2d3e 0a20 2020 2020 2020 2023 2320   -->.        ## 
-00001a90: 4375 7374 6f6d 2048 5454 5020 436c 6965  Custom HTTP Clie
-00001aa0: 6e74 0a20 2020 2020 2020 200a 2020 2020  nt.        .    
-00001ab0: 2020 2020 5468 6520 5079 7468 6f6e 2053      The Python S
-00001ac0: 444b 206d 616b 6573 2041 5049 2063 616c  DK makes API cal
-00001ad0: 6c73 2075 7369 6e67 2074 6865 205b 7265  ls using the [re
-00001ae0: 7175 6573 7473 5d28 6874 7470 733a 2f2f  quests](https://
-00001af0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00001b00: 2f72 6571 7565 7374 732f 2920 4854 5450  /requests/) HTTP
-00001b10: 206c 6962 7261 7279 2e20 2049 6e20 6f72   library.  In or
-00001b20: 6465 7220 746f 2070 726f 7669 6465 2061  der to provide a
-00001b30: 2063 6f6e 7665 6e69 656e 7420 7761 7920   convenient way 
-00001b40: 746f 2063 6f6e 6669 6775 7265 2074 696d  to configure tim
-00001b50: 656f 7574 732c 2063 6f6f 6b69 6573 2c20  eouts, cookies, 
-00001b60: 7072 6f78 6965 732c 2063 7573 746f 6d20  proxies, custom 
-00001b70: 6865 6164 6572 732c 2061 6e64 206f 7468  headers, and oth
-00001b80: 6572 206c 6f77 2d6c 6576 656c 2063 6f6e  er low-level con
-00001b90: 6669 6775 7261 7469 6f6e 2c20 796f 7520  figuration, you 
-00001ba0: 6361 6e20 696e 6974 6961 6c69 7a65 2074  can initialize t
-00001bb0: 6865 2053 444b 2063 6c69 656e 7420 7769  he SDK client wi
-00001bc0: 7468 2061 2063 7573 746f 6d20 6072 6571  th a custom `req
-00001bd0: 7565 7374 732e 5365 7373 696f 6e60 206f  uests.Session` o
-00001be0: 626a 6563 742e 0a20 2020 2020 2020 200a  bject..        .
-00001bf0: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
-00001c00: 706c 652c 2079 6f75 2063 6f75 6c64 2073  ple, you could s
-00001c10: 7065 6369 6679 2061 2068 6561 6465 7220  pecify a header 
-00001c20: 666f 7220 6576 6572 7920 7265 7175 6573  for every reques
-00001c30: 7420 7468 6174 2074 6869 7320 7364 6b20  t that this sdk 
-00001c40: 6d61 6b65 7320 6173 2066 6f6c 6c6f 7773  makes as follows
-00001c50: 3a0a 2020 2020 2020 2020 6060 6070 7974  :.        ```pyt
-00001c60: 686f 6e0a 2020 2020 2020 2020 696d 706f  hon.        impo
-00001c70: 7274 206b 6579 6d61 7465 6170 690a 2020  rt keymateapi.  
-00001c80: 2020 2020 2020 696d 706f 7274 2072 6571        import req
-00001c90: 7565 7374 730a 2020 2020 2020 2020 0a20  uests.        . 
-00001ca0: 2020 2020 2020 2068 7474 705f 636c 6965         http_clie
-00001cb0: 6e74 203d 2072 6571 7565 7374 732e 5365  nt = requests.Se
-00001cc0: 7373 696f 6e28 290a 2020 2020 2020 2020  ssion().        
-00001cd0: 6874 7470 5f63 6c69 656e 742e 6865 6164  http_client.head
-00001ce0: 6572 732e 7570 6461 7465 287b 2778 2d63  ers.update({'x-c
-00001cf0: 7573 746f 6d2d 6865 6164 6572 273a 2027  ustom-header': '
-00001d00: 736f 6d65 5661 6c75 6527 7d29 0a20 2020  someValue'}).   
-00001d10: 2020 2020 2073 203d 206b 6579 6d61 7465       s = keymate
-00001d20: 6170 692e 4b65 796d 6174 6561 7069 2863  api.Keymateapi(c
-00001d30: 6c69 656e 743a 2068 7474 705f 636c 6965  lient: http_clie
-00001d40: 6e74 290a 2020 2020 2020 2020 6060 600a  nt).        ```.
-00001d50: 2020 2020 2020 2020 3c21 2d2d 2045 6e64          <!-- End
-00001d60: 2043 7573 746f 6d20 4854 5450 2043 6c69   Custom HTTP Cli
-00001d70: 656e 7420 5b68 7474 702d 636c 6965 6e74  ent [http-client
-00001d80: 5d20 2d2d 3e0a 2020 2020 2020 2020 0a20  ] -->.        . 
-00001d90: 2020 2020 2020 203c 212d 2d20 5374 6172         <!-- Star
-00001da0: 7420 4175 7468 656e 7469 6361 7469 6f6e  t Authentication
-00001db0: 205b 7365 6375 7269 7479 5d20 2d2d 3e0a   [security] -->.
-00001dc0: 2020 2020 2020 2020 2323 2041 7574 6865          ## Authe
-00001dd0: 6e74 6963 6174 696f 6e0a 2020 2020 2020  ntication.      
-00001de0: 2020 0a20 2020 2020 2020 2023 2323 2050    .        ### P
-00001df0: 6572 2d43 6c69 656e 7420 5365 6375 7269  er-Client Securi
-00001e00: 7479 2053 6368 656d 6573 0a20 2020 2020  ty Schemes.     
-00001e10: 2020 200a 2020 2020 2020 2020 5468 6973     .        This
-00001e20: 2053 444b 2073 7570 706f 7274 7320 7468   SDK supports th
-00001e30: 6520 666f 6c6c 6f77 696e 6720 7365 6375  e following secu
-00001e40: 7269 7479 2073 6368 656d 6520 676c 6f62  rity scheme glob
-00001e50: 616c 6c79 3a0a 2020 2020 2020 2020 0a20  ally:.        . 
-00001e60: 2020 2020 2020 207c 204e 616d 6520 2020         | Name   
-00001e70: 2020 2020 2020 207c 2054 7970 6520 2020         | Type   
-00001e80: 2020 2020 2020 207c 2053 6368 656d 6520         | Scheme 
-00001e90: 2020 2020 2020 207c 0a20 2020 2020 2020         |.       
-00001ea0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
-00001eb0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
-00001ec0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
-00001ed0: 207c 0a20 2020 2020 2020 207c 2060 6265   |.        | `be
-00001ee0: 6172 6572 5f61 7574 6860 207c 2068 7474  arer_auth` | htt
-00001ef0: 7020 2020 2020 2020 2020 207c 2048 5454  p          | HTT
-00001f00: 5020 4265 6172 6572 2020 207c 0a20 2020  P Bearer   |.   
-00001f10: 2020 2020 200a 2020 2020 2020 2020 546f       .        To
-00001f20: 2061 7574 6865 6e74 6963 6174 6520 7769   authenticate wi
-00001f30: 7468 2074 6865 2041 5049 2074 6865 2060  th the API the `
-00001f40: 6265 6172 6572 5f61 7574 6860 2070 6172  bearer_auth` par
-00001f50: 616d 6574 6572 206d 7573 7420 6265 2073  ameter must be s
-00001f60: 6574 2077 6865 6e20 696e 6974 6961 6c69  et when initiali
-00001f70: 7a69 6e67 2074 6865 2053 444b 2063 6c69  zing the SDK cli
-00001f80: 656e 7420 696e 7374 616e 6365 2e20 466f  ent instance. Fo
-00001f90: 7220 6578 616d 706c 653a 0a20 2020 2020  r example:.     
-00001fa0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-00001fb0: 2020 2020 2069 6d70 6f72 7420 6b65 796d       import keym
-00001fc0: 6174 6561 7069 0a20 2020 2020 2020 200a  ateapi.        .
-00001fd0: 2020 2020 2020 2020 7320 3d20 6b65 796d          s = keym
-00001fe0: 6174 6561 7069 2e4b 6579 6d61 7465 6170  ateapi.Keymateap
-00001ff0: 6928 0a20 2020 2020 2020 2020 2020 2062  i(.            b
-00002000: 6561 7265 725f 6175 7468 3d22 3c59 4f55  earer_auth="<YOU
-00002010: 525f 4245 4152 4552 5f54 4f4b 454e 5f48  R_BEARER_TOKEN_H
-00002020: 4552 453e 222c 0a20 2020 2020 2020 2029  ERE>",.        )
-00002030: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002040: 2020 0a20 2020 2020 2020 2072 6573 203d    .        res =
-00002050: 2073 2e75 7073 6572 7428 713d 273c 7661   s.upsert(q='<va
-00002060: 6c75 653e 2729 0a20 2020 2020 2020 200a  lue>').        .
-00002070: 2020 2020 2020 2020 6966 2072 6573 2e6f          if res.o
-00002080: 626a 6563 7420 6973 206e 6f74 204e 6f6e  bject is not Non
-00002090: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-000020a0: 2068 616e 646c 6520 7265 7370 6f6e 7365   handle response
-000020b0: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-000020c0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
-000020d0: 2020 2060 6060 0a20 2020 2020 2020 203c     ```.        <
-000020e0: 212d 2d20 456e 6420 4175 7468 656e 7469  !-- End Authenti
-000020f0: 6361 7469 6f6e 205b 7365 6375 7269 7479  cation [security
-00002100: 5d20 2d2d 3e0a 2020 2020 2020 2020 0a20  ] -->.        . 
-00002110: 2020 2020 2020 203c 212d 2d20 506c 6163         <!-- Plac
-00002120: 6568 6f6c 6465 7220 666f 7220 4675 7475  eholder for Futu
-00002130: 7265 2053 7065 616b 6561 7379 2053 444b  re Speakeasy SDK
-00002140: 2053 6563 7469 6f6e 7320 2d2d 3e0a 2020   Sections -->.  
-00002150: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00002160: 2044 6576 656c 6f70 6d65 6e74 0a20 2020   Development.   
-00002170: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00002180: 204d 6174 7572 6974 790a 2020 2020 2020   Maturity.      
-00002190: 2020 0a20 2020 2020 2020 2054 6869 7320    .        This 
-000021a0: 5344 4b20 6973 2069 6e20 6265 7461 2c20  SDK is in beta, 
-000021b0: 616e 6420 7468 6572 6520 6d61 7920 6265  and there may be
-000021c0: 2062 7265 616b 696e 6720 6368 616e 6765   breaking change
-000021d0: 7320 6265 7477 6565 6e20 7665 7273 696f  s between versio
-000021e0: 6e73 2077 6974 686f 7574 2061 206d 616a  ns without a maj
-000021f0: 6f72 2076 6572 7369 6f6e 2075 7064 6174  or version updat
-00002200: 652e 2054 6865 7265 666f 7265 2c20 7765  e. Therefore, we
-00002210: 2072 6563 6f6d 6d65 6e64 2070 696e 6e69   recommend pinni
-00002220: 6e67 2075 7361 6765 0a20 2020 2020 2020  ng usage.       
-00002230: 2074 6f20 6120 7370 6563 6966 6963 2070   to a specific p
-00002240: 6163 6b61 6765 2076 6572 7369 6f6e 2e20  ackage version. 
-00002250: 5468 6973 2077 6179 2c20 796f 7520 6361  This way, you ca
-00002260: 6e20 696e 7374 616c 6c20 7468 6520 7361  n install the sa
-00002270: 6d65 2076 6572 7369 6f6e 2065 6163 6820  me version each 
-00002280: 7469 6d65 2077 6974 686f 7574 2062 7265  time without bre
-00002290: 616b 696e 6720 6368 616e 6765 7320 756e  aking changes un
-000022a0: 6c65 7373 2079 6f75 2061 7265 2069 6e74  less you are int
-000022b0: 656e 7469 6f6e 616c 6c79 0a20 2020 2020  entionally.     
-000022c0: 2020 206c 6f6f 6b69 6e67 2066 6f72 2074     looking for t
-000022d0: 6865 206c 6174 6573 7420 7665 7273 696f  he latest versio
-000022e0: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-000022f0: 2020 2020 2323 2043 6f6e 7472 6962 7574      ## Contribut
-00002300: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
-00002310: 2020 2020 2020 5768 696c 6520 7765 2076        While we v
-00002320: 616c 7565 206f 7065 6e2d 736f 7572 6365  alue open-source
-00002330: 2063 6f6e 7472 6962 7574 696f 6e73 2074   contributions t
-00002340: 6f20 7468 6973 2053 444b 2c20 7468 6973  o this SDK, this
-00002350: 206c 6962 7261 7279 2069 7320 6765 6e65   library is gene
-00002360: 7261 7465 6420 7072 6f67 7261 6d6d 6174  rated programmat
-00002370: 6963 616c 6c79 2e0a 2020 2020 2020 2020  ically..        
-00002380: 4665 656c 2066 7265 6520 746f 206f 7065  Feel free to ope
-00002390: 6e20 6120 5052 206f 7220 6120 4769 7468  n a PR or a Gith
-000023a0: 7562 2069 7373 7565 2061 7320 6120 7072  ub issue as a pr
-000023b0: 6f6f 6620 6f66 2063 6f6e 6365 7074 2061  oof of concept a
-000023c0: 6e64 2077 6527 6c6c 2064 6f20 6f75 7220  nd we'll do our 
-000023d0: 6265 7374 2074 6f20 696e 636c 7564 6520  best to include 
-000023e0: 6974 2069 6e20 6120 6675 7475 7265 2072  it in a future r
-000023f0: 656c 6561 7365 210a 2020 2020 2020 2020  elease!.        
-00002400: 0a20 2020 2020 2020 2023 2323 2053 444b  .        ### SDK
-00002410: 2043 7265 6174 6564 2062 7920 5b53 7065   Created by [Spe
-00002420: 616b 6561 7379 5d28 6874 7470 733a 2f2f  akeasy](https://
-00002430: 646f 6373 2e73 7065 616b 6561 7379 6170  docs.speakeasyap
-00002440: 692e 6465 762f 646f 6373 2f75 7369 6e67  i.dev/docs/using
-00002450: 2d73 7065 616b 6561 7379 2f63 6c69 656e  -speakeasy/clien
-00002460: 742d 7364 6b73 290a 2020 2020 2020 2020  t-sdks).        
-00002470: 0a50 6c61 7466 6f72 6d3a 2055 4e4b 4e4f  .Platform: UNKNO
-00002480: 574e 0a52 6571 7569 7265 732d 5079 7468  WN.Requires-Pyth
-00002490: 6f6e 3a20 3e3d 332e 380a 4465 7363 7269  on: >=3.8.Descri
-000024a0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-000024b0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-000024c0: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
-000024d0: 3a20 6465 760a                           : dev.
+00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
+00000080: 622e 636f 6d2f 6f7a 6775 726e 6577 2f6b  b.com/ozgurnew/k
+00000090: 6579 6d61 7465 2d70 7974 686f 6e2d 7364  eymate-python-sd
+000000a0: 6b2e 6769 740a 4175 7468 6f72 3a20 5370  k.git.Author: Sp
+000000b0: 6561 6b65 6173 790a 4c69 6365 6e73 653a  eakeasy.License:
+000000c0: 2055 4e4b 4e4f 574e 0a44 6573 6372 6970   UNKNOWN.Descrip
+000000d0: 7469 6f6e 3a20 2320 6b65 796d 6174 6561  tion: # keymatea
+000000e0: 7069 0a20 2020 2020 2020 200a 2020 2020  pi.        .    
+000000f0: 2020 2020 0a20 2020 2020 2020 203c 212d      .        <!-
+00000100: 2d20 5374 6172 7420 5344 4b20 496e 7374  - Start SDK Inst
+00000110: 616c 6c61 7469 6f6e 205b 696e 7374 616c  allation [instal
+00000120: 6c61 7469 6f6e 5d20 2d2d 3e0a 2020 2020  lation] -->.    
+00000130: 2020 2020 2323 2053 444b 2049 6e73 7461      ## SDK Insta
+00000140: 6c6c 6174 696f 6e0a 2020 2020 2020 2020  llation.        
+00000150: 0a20 2020 2020 2020 2060 6060 6261 7368  .        ```bash
+00000160: 0a20 2020 2020 2020 2070 6970 2069 6e73  .        pip ins
+00000170: 7461 6c6c 206b 6579 6d61 7465 6170 690a  tall keymateapi.
+00000180: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+00000190: 2020 2020 3c21 2d2d 2045 6e64 2053 444b      <!-- End SDK
+000001a0: 2049 6e73 7461 6c6c 6174 696f 6e20 5b69   Installation [i
+000001b0: 6e73 7461 6c6c 6174 696f 6e5d 202d 2d3e  nstallation] -->
+000001c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000001d0: 2020 3c21 2d2d 2053 7461 7274 2053 444b    <!-- Start SDK
+000001e0: 2045 7861 6d70 6c65 2055 7361 6765 205b   Example Usage [
+000001f0: 7573 6167 655d 202d 2d3e 0a20 2020 2020  usage] -->.     
+00000200: 2020 2023 2320 5344 4b20 4578 616d 706c     ## SDK Exampl
+00000210: 6520 5573 6167 650a 2020 2020 2020 2020  e Usage.        
+00000220: 0a20 2020 2020 2020 2023 2323 2045 7861  .        ### Exa
+00000230: 6d70 6c65 0a20 2020 2020 2020 200a 2020  mple.        .  
+00000240: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00000250: 2020 2020 2020 2020 696d 706f 7274 206b          import k
+00000260: 6579 6d61 7465 6170 690a 2020 2020 2020  eymateapi.      
+00000270: 2020 0a20 2020 2020 2020 2073 203d 206b    .        s = k
+00000280: 6579 6d61 7465 6170 692e 4b65 796d 6174  eymateapi.Keymat
+00000290: 6561 7069 280a 2020 2020 2020 2020 2020  eapi(.          
+000002a0: 2020 6265 6172 6572 5f61 7574 683d 223c    bearer_auth="<
+000002b0: 594f 5552 5f42 4541 5245 525f 544f 4b45  YOUR_BEARER_TOKE
+000002c0: 4e5f 4845 5245 3e22 2c0a 2020 2020 2020  N_HERE>",.      
+000002d0: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
+000002e0: 2020 2020 2072 6573 203d 2073 2e75 7073       res = s.ups
+000002f0: 6572 7428 713d 2749 2070 7265 6665 7220  ert(q='I prefer 
+00000300: 436f 7374 6120 6f76 6572 2053 7461 7262  Costa over Starb
+00000310: 7563 6b73 2e27 290a 2020 2020 2020 2020  ucks.').        
+00000320: 0a20 2020 2020 2020 2069 6620 7265 732e  .        if res.
+00000330: 6f62 6a65 6374 2069 7320 6e6f 7420 4e6f  object is not No
+00000340: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00000350: 2320 6861 6e64 6c65 2072 6573 706f 6e73  # handle respons
+00000360: 650a 2020 2020 2020 2020 2020 2020 7061  e.            pa
+00000370: 7373 0a20 2020 2020 2020 200a 2020 2020  ss.        .    
+00000380: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00000390: 3c21 2d2d 2045 6e64 2053 444b 2045 7861  <!-- End SDK Exa
+000003a0: 6d70 6c65 2055 7361 6765 205b 7573 6167  mple Usage [usag
+000003b0: 655d 202d 2d3e 0a20 2020 2020 2020 200a  e] -->.        .
+000003c0: 2020 2020 2020 2020 3c21 2d2d 2053 7461          <!-- Sta
+000003d0: 7274 2041 7661 696c 6162 6c65 2052 6573  rt Available Res
+000003e0: 6f75 7263 6573 2061 6e64 204f 7065 7261  ources and Opera
+000003f0: 7469 6f6e 7320 5b6f 7065 7261 7469 6f6e  tions [operation
+00000400: 735d 202d 2d3e 0a20 2020 2020 2020 2023  s] -->.        #
+00000410: 2320 4176 6169 6c61 626c 6520 5265 736f  # Available Reso
+00000420: 7572 6365 7320 616e 6420 4f70 6572 6174  urces and Operat
+00000430: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
+00000440: 2020 2020 2020 2323 2320 5b4b 6579 6d61        ### [Keyma
+00000450: 7465 6170 6920 5344 4b5d 2868 7474 7073  teapi SDK](https
+00000460: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f7a  ://github.com/oz
+00000470: 6775 726e 6577 2f6b 6579 6d61 7465 2d70  gurnew/keymate-p
+00000480: 7974 686f 6e2d 7364 6b2f 626c 6f62 2f6d  ython-sdk/blob/m
+00000490: 6173 7465 722f 646f 6373 2f73 646b 732f  aster/docs/sdks/
+000004a0: 6b65 796d 6174 6561 7069 2f52 4541 444d  keymateapi/READM
+000004b0: 452e 6d64 290a 2020 2020 2020 2020 0a20  E.md).        . 
+000004c0: 2020 2020 2020 202a 205b 7570 7365 7274         * [upsert
+000004d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000004e0: 2e63 6f6d 2f6f 7a67 7572 6e65 772f 6b65  .com/ozgurnew/ke
+000004f0: 796d 6174 652d 7079 7468 6f6e 2d73 646b  ymate-python-sdk
+00000500: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
+00000510: 732f 7364 6b73 2f6b 6579 6d61 7465 6170  s/sdks/keymateap
+00000520: 692f 5245 4144 4d45 2e6d 6423 7570 7365  i/README.md#upse
+00000530: 7274 2920 2d20 496e 7365 7274 7320 7265  rt) - Inserts re
+00000540: 636f 7264 2074 6f20 4b65 796d 6174 6520  cord to Keymate 
+00000550: 4d65 6d6f 7279 2e0a 2020 2020 2020 2020  Memory..        
+00000560: 2a20 5b71 7565 7279 5d28 6874 7470 733a  * [query](https:
+00000570: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7a67  //github.com/ozg
+00000580: 7572 6e65 772f 6b65 796d 6174 652d 7079  urnew/keymate-py
+00000590: 7468 6f6e 2d73 646b 2f62 6c6f 622f 6d61  thon-sdk/blob/ma
+000005a0: 7374 6572 2f64 6f63 732f 7364 6b73 2f6b  ster/docs/sdks/k
+000005b0: 6579 6d61 7465 6170 692f 5245 4144 4d45  eymateapi/README
+000005c0: 2e6d 6423 7175 6572 7929 202d 2051 7565  .md#query) - Que
+000005d0: 7269 6573 2074 6865 2075 7365 7227 7320  ries the user's 
+000005e0: 4b65 796d 6174 6520 4d65 6d6f 7279 2e0a  Keymate Memory..
+000005f0: 2020 2020 2020 2020 2a20 5b62 726f 7773          * [brows
+00000600: 6575 726c 5d28 6874 7470 733a 2f2f 6769  eurl](https://gi
+00000610: 7468 7562 2e63 6f6d 2f6f 7a67 7572 6e65  thub.com/ozgurne
+00000620: 772f 6b65 796d 6174 652d 7079 7468 6f6e  w/keymate-python
+00000630: 2d73 646b 2f62 6c6f 622f 6d61 7374 6572  -sdk/blob/master
+00000640: 2f64 6f63 732f 7364 6b73 2f6b 6579 6d61  /docs/sdks/keyma
+00000650: 7465 6170 692f 5245 4144 4d45 2e6d 6423  teapi/README.md#
+00000660: 6272 6f77 7365 7572 6c29 202d 2054 6865  browseurl) - The
+00000670: 2070 6c75 6769 6e20 656e 6162 6c65 7320   plugin enables 
+00000680: 7573 6572 2074 6f20 636f 6e64 7563 7420  user to conduct 
+00000690: 7765 6220 6272 6f77 7369 6e67 2062 7920  web browsing by 
+000006a0: 6578 7472 6163 7469 6e67 2074 6865 2074  extracting the t
+000006b0: 6578 7420 636f 6e74 656e 7420 6f66 2061  ext content of a
+000006c0: 2073 7065 6369 6669 6564 2055 524c 2e20   specified URL. 
+000006d0: 4974 2077 696c 6c20 6765 6e65 7261 7465  It will generate
+000006e0: 2074 6974 6c65 2061 6e64 2063 6f6e 7465   title and conte
+000006f0: 6e74 2e0a 2020 2020 2020 2020 2a20 5b62  nt..        * [b
+00000700: 726f 7773 655d 2868 7474 7073 3a2f 2f67  rowse](https://g
+00000710: 6974 6875 622e 636f 6d2f 6f7a 6775 726e  ithub.com/ozgurn
+00000720: 6577 2f6b 6579 6d61 7465 2d70 7974 686f  ew/keymate-pytho
+00000730: 6e2d 7364 6b2f 626c 6f62 2f6d 6173 7465  n-sdk/blob/maste
+00000740: 722f 646f 6373 2f73 646b 732f 6b65 796d  r/docs/sdks/keym
+00000750: 6174 6561 7069 2f52 4541 444d 452e 6d64  ateapi/README.md
+00000760: 2362 726f 7773 6529 202d 2046 6574 6368  #browse) - Fetch
+00000770: 2061 6e79 2055 524c 7320 7769 7468 6f75   any URLs withou
+00000780: 7420 7072 6f78 7920 6974 2077 6f75 6c64  t proxy it would
+00000790: 2070 726f 6261 626c 7920 6661 696c 206f   probably fail o
+000007a0: 6e20 6d61 6a6f 7220 7765 6273 6974 6573  n major websites
+000007b0: 2062 7574 2071 7569 636b 6572 2074 6861   but quicker tha
+000007c0: 6e20 6272 6f77 7365 7572 6c20 0a20 2020  n browseurl .   
+000007d0: 2020 2020 202a 205b 7365 6172 6368 5d28       * [search](
+000007e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000007f0: 6f6d 2f6f 7a67 7572 6e65 772f 6b65 796d  om/ozgurnew/keym
+00000800: 6174 652d 7079 7468 6f6e 2d73 646b 2f62  ate-python-sdk/b
+00000810: 6c6f 622f 6d61 7374 6572 2f64 6f63 732f  lob/master/docs/
+00000820: 7364 6b73 2f6b 6579 6d61 7465 6170 692f  sdks/keymateapi/
+00000830: 5245 4144 4d45 2e6d 6423 7365 6172 6368  README.md#search
+00000840: 2920 2d20 5769 7468 6f75 7420 7072 6f78  ) - Without prox
+00000850: 6965 7320 7365 6172 6368 6573 206b 6579  ies searches key
+00000860: 776f 7264 206f 6e20 7468 6520 696e 7465  word on the inte
+00000870: 726e 6574 2061 6e64 2066 6574 6368 6573  rnet and fetches
+00000880: 2075 726c 7320 616e 6420 6f70 7469 6d69   urls and optimi
+00000890: 7a65 7320 6f75 7470 7574 0a20 2020 2020  zes output.     
+000008a0: 2020 202a 205b 756c 7472 6166 6173 7473     * [ultrafasts
+000008b0: 6561 7263 685d 2868 7474 7073 3a2f 2f67  earch](https://g
+000008c0: 6974 6875 622e 636f 6d2f 6f7a 6775 726e  ithub.com/ozgurn
+000008d0: 6577 2f6b 6579 6d61 7465 2d70 7974 686f  ew/keymate-pytho
+000008e0: 6e2d 7364 6b2f 626c 6f62 2f6d 6173 7465  n-sdk/blob/maste
+000008f0: 722f 646f 6373 2f73 646b 732f 6b65 796d  r/docs/sdks/keym
+00000900: 6174 6561 7069 2f52 4541 444d 452e 6d64  ateapi/README.md
+00000910: 2375 6c74 7261 6661 7374 7365 6172 6368  #ultrafastsearch
+00000920: 2920 2d20 5468 6973 2070 6c75 6769 6e20  ) - This plugin 
+00000930: 7072 6f76 6964 6573 2031 3020 756c 7472  provides 10 ultr
+00000940: 6120 6661 7374 2073 6561 7263 6820 7265  a fast search re
+00000950: 7375 6c74 7320 6672 6f6d 206d 756c 7469  sults from multi
+00000960: 706c 6520 736f 7572 6365 7320 6769 7669  ple sources givi
+00000970: 6e67 2061 206d 6f72 6520 636f 6d70 7265  ng a more compre
+00000980: 6865 6e73 6976 6520 7669 6577 2e0a 2020  hensive view..  
+00000990: 2020 2020 2020 2a20 5b67 7074 7362 726f        * [gptsbro
+000009a0: 7773 655d 2868 7474 7073 3a2f 2f67 6974  wse](https://git
+000009b0: 6875 622e 636f 6d2f 6f7a 6775 726e 6577  hub.com/ozgurnew
+000009c0: 2f6b 6579 6d61 7465 2d70 7974 686f 6e2d  /keymate-python-
+000009d0: 7364 6b2f 626c 6f62 2f6d 6173 7465 722f  sdk/blob/master/
+000009e0: 646f 6373 2f73 646b 732f 6b65 796d 6174  docs/sdks/keymat
+000009f0: 6561 7069 2f52 4541 444d 452e 6d64 2367  eapi/README.md#g
+00000a00: 7074 7362 726f 7773 6529 202d 2046 6574  ptsbrowse) - Fet
+00000a10: 6368 206d 656d 6f72 792e 6b65 796d 6174  ch memory.keymat
+00000a20: 652e 6169 2055 524c 730a 2020 2020 2020  e.ai URLs.      
+00000a30: 2020 2a20 5b69 6e74 6572 6e65 7473 6561    * [internetsea
+00000a40: 7263 685d 2868 7474 7073 3a2f 2f67 6974  rch](https://git
+00000a50: 6875 622e 636f 6d2f 6f7a 6775 726e 6577  hub.com/ozgurnew
+00000a60: 2f6b 6579 6d61 7465 2d70 7974 686f 6e2d  /keymate-python-
+00000a70: 7364 6b2f 626c 6f62 2f6d 6173 7465 722f  sdk/blob/master/
+00000a80: 646f 6373 2f73 646b 732f 6b65 796d 6174  docs/sdks/keymat
+00000a90: 6561 7069 2f52 4541 444d 452e 6d64 2369  eapi/README.md#i
+00000aa0: 6e74 6572 6e65 7473 6561 7263 6829 202d  nternetsearch) -
+00000ab0: 2043 6f6e 6475 6374 2061 6e20 696e 7465   Conduct an inte
+00000ac0: 726e 6574 2073 6561 7263 680a 2020 2020  rnet search.    
+00000ad0: 2020 2020 3c21 2d2d 2045 6e64 2041 7661      <!-- End Ava
+00000ae0: 696c 6162 6c65 2052 6573 6f75 7263 6573  ilable Resources
+00000af0: 2061 6e64 204f 7065 7261 7469 6f6e 7320   and Operations 
+00000b00: 5b6f 7065 7261 7469 6f6e 735d 202d 2d3e  [operations] -->
+00000b10: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000b20: 2020 3c21 2d2d 2053 7461 7274 2045 7272    <!-- Start Err
+00000b30: 6f72 2048 616e 646c 696e 6720 5b65 7272  or Handling [err
+00000b40: 6f72 735d 202d 2d3e 0a20 2020 2020 2020  ors] -->.       
+00000b50: 2023 2320 4572 726f 7220 4861 6e64 6c69   ## Error Handli
+00000b60: 6e67 0a20 2020 2020 2020 200a 2020 2020  ng.        .    
+00000b70: 2020 2020 4861 6e64 6c69 6e67 2065 7272      Handling err
+00000b80: 6f72 7320 696e 2074 6869 7320 5344 4b20  ors in this SDK 
+00000b90: 7368 6f75 6c64 206c 6172 6765 6c79 206d  should largely m
+00000ba0: 6174 6368 2079 6f75 7220 6578 7065 6374  atch your expect
+00000bb0: 6174 696f 6e73 2e20 2041 6c6c 206f 7065  ations.  All ope
+00000bc0: 7261 7469 6f6e 7320 7265 7475 726e 2061  rations return a
+00000bd0: 2072 6573 706f 6e73 6520 6f62 6a65 6374   response object
+00000be0: 206f 7220 7261 6973 6520 616e 2065 7272   or raise an err
+00000bf0: 6f72 2e20 2049 6620 4572 726f 7220 6f62  or.  If Error ob
+00000c00: 6a65 6374 7320 6172 6520 7370 6563 6966  jects are specif
+00000c10: 6965 6420 696e 2079 6f75 7220 4f70 656e  ied in your Open
+00000c20: 4150 4920 5370 6563 2c20 7468 6520 5344  API Spec, the SD
+00000c30: 4b20 7769 6c6c 2072 6169 7365 2074 6865  K will raise the
+00000c40: 2061 7070 726f 7072 6961 7465 2045 7272   appropriate Err
+00000c50: 6f72 2074 7970 652e 0a20 2020 2020 2020  or type..       
+00000c60: 200a 2020 2020 2020 2020 7c20 4572 726f   .        | Erro
+00000c70: 7220 4f62 6a65 6374 2020 2020 2020 2020  r Object        
+00000c80: 2020 2020 2020 2020 207c 2053 7461 7475           | Statu
+00000c90: 7320 436f 6465 2020 2020 2020 2020 2020  s Code          
+00000ca0: 2020 2020 2020 2020 7c20 436f 6e74 656e          | Conten
+00000cb0: 7420 5479 7065 2020 2020 2020 2020 2020  t Type          
+00000cc0: 2020 2020 2020 207c 0a20 2020 2020 2020         |.       
+00000cd0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00000ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
+00000cf0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
+00000d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+00000d10: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00000d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0a  ------------- |.
+00000d30: 2020 2020 2020 2020 7c20 6572 726f 7273          | errors
+00000d40: 2e42 726f 7773 6575 726c 5265 7370 6f6e  .BrowseurlRespon
+00000d50: 7365 426f 6479 207c 2034 3030 2020 2020  seBody | 400    
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 2020 2020 2020 7c20 6170 706c 6963 6174        | applicat
+00000d80: 696f 6e2f 6a73 6f6e 2020 2020 2020 2020  ion/json        
+00000d90: 2020 2020 207c 0a20 2020 2020 2020 207c       |.        |
+00000da0: 2065 7272 6f72 732e 5344 4b45 7272 6f72   errors.SDKError
+00000db0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00000dc0: 3478 782d 3578 7820 2020 2020 2020 2020  4xx-5xx         
+00000dd0: 2020 2020 2020 2020 2020 2020 207c 202a               | *
+00000de0: 2f2a 2020 2020 2020 2020 2020 2020 2020  /*              
+00000df0: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
+00000e00: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00000e10: 2323 2045 7861 6d70 6c65 0a20 2020 2020  ## Example.     
+00000e20: 2020 200a 2020 2020 2020 2020 6060 6070     .        ```p
+00000e30: 7974 686f 6e0a 2020 2020 2020 2020 696d  ython.        im
+00000e40: 706f 7274 206b 6579 6d61 7465 6170 690a  port keymateapi.
+00000e50: 2020 2020 2020 2020 6672 6f6d 206b 6579          from key
+00000e60: 6d61 7465 6170 692e 6d6f 6465 6c73 2069  mateapi.models i
+00000e70: 6d70 6f72 7420 6572 726f 7273 2c20 6f70  mport errors, op
+00000e80: 6572 6174 696f 6e73 0a20 2020 2020 2020  erations.       
+00000e90: 200a 2020 2020 2020 2020 7320 3d20 6b65   .        s = ke
+00000ea0: 796d 6174 6561 7069 2e4b 6579 6d61 7465  ymateapi.Keymate
+00000eb0: 6170 6928 0a20 2020 2020 2020 2020 2020  api(.           
+00000ec0: 2062 6561 7265 725f 6175 7468 3d22 3c59   bearer_auth="<Y
+00000ed0: 4f55 525f 4245 4152 4552 5f54 4f4b 454e  OUR_BEARER_TOKEN
+00000ee0: 5f48 4552 453e 222c 0a20 2020 2020 2020  _HERE>",.       
+00000ef0: 2029 0a20 2020 2020 2020 200a 2020 2020   ).        .    
+00000f00: 2020 2020 7265 7320 3d20 4e6f 6e65 0a20      res = None. 
+00000f10: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00000f20: 2020 2020 2020 2020 7265 7320 3d20 732e          res = s.
+00000f30: 6272 6f77 7365 7572 6c28 7265 7175 6573  browseurl(reques
+00000f40: 743d 6f70 6572 6174 696f 6e73 2e42 726f  t=operations.Bro
+00000f50: 7773 6575 726c 5265 7175 6573 7428 0a20  wseurlRequest(. 
+00000f60: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00000f70: 7769 6e64 6f77 776f 7264 733d 2731 3030  windowwords='100
+00000f80: 3030 272c 0a20 2020 2020 2020 2020 2020  00',.           
+00000f90: 2071 3d27 6874 7470 733a 2f2f 6b65 796d   q='https://keym
+00000fa0: 6174 652e 6169 272c 0a20 2020 2020 2020  ate.ai',.       
+00000fb0: 2020 2020 2070 6572 6365 6e74 696c 653d       percentile=
+00000fc0: 2731 272c 0a20 2020 2020 2020 2020 2020  '1',.           
+00000fd0: 206e 756d 6f66 7061 6765 733d 2731 272c   numofpages='1',
+00000fe0: 0a20 2020 2020 2020 2020 2020 2070 6167  .            pag
+00000ff0: 696e 673d 2731 272c 0a20 2020 2020 2020  ing='1',.       
+00001000: 2029 290a 2020 2020 2020 2020 6578 6365   )).        exce
+00001010: 7074 2065 7272 6f72 732e 4272 6f77 7365  pt errors.Browse
+00001020: 7572 6c52 6573 706f 6e73 6542 6f64 7920  urlResponseBody 
+00001030: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00001040: 2020 2320 6861 6e64 6c65 2065 7863 6570    # handle excep
+00001050: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00001060: 2072 6169 7365 2865 290a 2020 2020 2020   raise(e).      
+00001070: 2020 6578 6365 7074 2065 7272 6f72 732e    except errors.
+00001080: 5344 4b45 7272 6f72 2061 7320 653a 0a20  SDKError as e:. 
+00001090: 2020 2020 2020 2020 2020 2023 2068 616e             # han
+000010a0: 646c 6520 6578 6365 7074 696f 6e0a 2020  dle exception.  
+000010b0: 2020 2020 2020 2020 2020 7261 6973 6528            raise(
+000010c0: 6529 0a20 2020 2020 2020 200a 2020 2020  e).        .    
+000010d0: 2020 2020 6966 2072 6573 2e74 776f 5f68      if res.two_h
+000010e0: 756e 6472 6564 5f61 7070 6c69 6361 7469  undred_applicati
+000010f0: 6f6e 5f6a 736f 6e5f 6f62 6a65 6374 2069  on_json_object i
+00001100: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00001110: 2020 2020 2020 2020 2320 6861 6e64 6c65          # handle
+00001120: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+00001130: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00001140: 2020 200a 2020 2020 2020 2020 6060 600a     .        ```.
+00001150: 2020 2020 2020 2020 3c21 2d2d 2045 6e64          <!-- End
+00001160: 2045 7272 6f72 2048 616e 646c 696e 6720   Error Handling 
+00001170: 5b65 7272 6f72 735d 202d 2d3e 0a20 2020  [errors] -->.   
+00001180: 2020 2020 200a 2020 2020 2020 2020 3c21       .        <!
+00001190: 2d2d 2053 7461 7274 2053 6572 7665 7220  -- Start Server 
+000011a0: 5365 6c65 6374 696f 6e20 5b73 6572 7665  Selection [serve
+000011b0: 725d 202d 2d3e 0a20 2020 2020 2020 2023  r] -->.        #
+000011c0: 2320 5365 7276 6572 2053 656c 6563 7469  # Server Selecti
+000011d0: 6f6e 0a20 2020 2020 2020 200a 2020 2020  on.        .    
+000011e0: 2020 2020 2323 2320 5365 6c65 6374 2053      ### Select S
+000011f0: 6572 7665 7220 6279 2049 6e64 6578 0a20  erver by Index. 
+00001200: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001210: 596f 7520 6361 6e20 6f76 6572 7269 6465  You can override
+00001220: 2074 6865 2064 6566 6175 6c74 2073 6572   the default ser
+00001230: 7665 7220 676c 6f62 616c 6c79 2062 7920  ver globally by 
+00001240: 7061 7373 696e 6720 6120 7365 7276 6572  passing a server
+00001250: 2069 6e64 6578 2074 6f20 7468 6520 6073   index to the `s
+00001260: 6572 7665 725f 6964 783a 2069 6e74 6020  erver_idx: int` 
+00001270: 6f70 7469 6f6e 616c 2070 6172 616d 6574  optional paramet
+00001280: 6572 2077 6865 6e20 696e 6974 6961 6c69  er when initiali
+00001290: 7a69 6e67 2074 6865 2053 444b 2063 6c69  zing the SDK cli
+000012a0: 656e 7420 696e 7374 616e 6365 2e20 5468  ent instance. Th
+000012b0: 6520 7365 6c65 6374 6564 2073 6572 7665  e selected serve
+000012c0: 7220 7769 6c6c 2074 6865 6e20 6265 2075  r will then be u
+000012d0: 7365 6420 6173 2074 6865 2064 6566 6175  sed as the defau
+000012e0: 6c74 206f 6e20 7468 6520 6f70 6572 6174  lt on the operat
+000012f0: 696f 6e73 2074 6861 7420 7573 6520 6974  ions that use it
+00001300: 2e20 5468 6973 2074 6162 6c65 206c 6973  . This table lis
+00001310: 7473 2074 6865 2069 6e64 6578 6573 2061  ts the indexes a
+00001320: 7373 6f63 6961 7465 6420 7769 7468 2074  ssociated with t
+00001330: 6865 2061 7661 696c 6162 6c65 2073 6572  he available ser
+00001340: 7665 7273 3a0a 2020 2020 2020 2020 0a20  vers:.        . 
+00001350: 2020 2020 2020 207c 2023 207c 2053 6572         | # | Ser
+00001360: 7665 7220 7c20 5661 7269 6162 6c65 7320  ver | Variables 
+00001370: 7c0a 2020 2020 2020 2020 7c20 2d20 7c20  |.        | - | 
+00001380: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00001390: 2d2d 207c 0a20 2020 2020 2020 207c 2030  -- |.        | 0
+000013a0: 207c 2060 6874 7470 733a 2f2f 7365 7276   | `https://serv
+000013b0: 6572 2e73 6561 7263 6877 6562 2e6b 6579  er.searchweb.key
+000013c0: 6d61 7465 2e61 6960 207c 204e 6f6e 6520  mate.ai` | None 
+000013d0: 7c0a 2020 2020 2020 2020 0a20 2020 2020  |.        .     
+000013e0: 2020 2023 2323 2320 4578 616d 706c 650a     #### Example.
+000013f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001400: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+00001410: 2020 2069 6d70 6f72 7420 6b65 796d 6174     import keymat
+00001420: 6561 7069 0a20 2020 2020 2020 200a 2020  eapi.        .  
+00001430: 2020 2020 2020 7320 3d20 6b65 796d 6174        s = keymat
+00001440: 6561 7069 2e4b 6579 6d61 7465 6170 6928  eapi.Keymateapi(
+00001450: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+00001460: 7665 725f 6964 783d 302c 0a20 2020 2020  ver_idx=0,.     
+00001470: 2020 2020 2020 2062 6561 7265 725f 6175         bearer_au
+00001480: 7468 3d22 3c59 4f55 525f 4245 4152 4552  th="<YOUR_BEARER
+00001490: 5f54 4f4b 454e 5f48 4552 453e 222c 0a20  _TOKEN_HERE>",. 
+000014a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000014b0: 200a 2020 2020 2020 2020 7265 7320 3d20   .        res = 
+000014c0: 732e 7570 7365 7274 2871 3d27 4920 7072  s.upsert(q='I pr
+000014d0: 6566 6572 2043 6f73 7461 206f 7665 7220  efer Costa over 
+000014e0: 5374 6172 6275 636b 732e 2729 0a20 2020  Starbucks.').   
+000014f0: 2020 2020 200a 2020 2020 2020 2020 6966       .        if
+00001500: 2072 6573 2e6f 626a 6563 7420 6973 206e   res.object is n
+00001510: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00001520: 2020 2020 2023 2068 616e 646c 6520 7265       # handle re
+00001530: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
+00001540: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+00001550: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+00001560: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+00001570: 2020 2020 2020 2023 2323 204f 7665 7272         ### Overr
+00001580: 6964 6520 5365 7276 6572 2055 524c 2050  ide Server URL P
+00001590: 6572 2d43 6c69 656e 740a 2020 2020 2020  er-Client.      
+000015a0: 2020 0a20 2020 2020 2020 2054 6865 2064    .        The d
+000015b0: 6566 6175 6c74 2073 6572 7665 7220 6361  efault server ca
+000015c0: 6e20 616c 736f 2062 6520 6f76 6572 7269  n also be overri
+000015d0: 6464 656e 2067 6c6f 6261 6c6c 7920 6279  dden globally by
+000015e0: 2070 6173 7369 6e67 2061 2055 524c 2074   passing a URL t
+000015f0: 6f20 7468 6520 6073 6572 7665 725f 7572  o the `server_ur
+00001600: 6c3a 2073 7472 6020 6f70 7469 6f6e 616c  l: str` optional
+00001610: 2070 6172 616d 6574 6572 2077 6865 6e20   parameter when 
+00001620: 696e 6974 6961 6c69 7a69 6e67 2074 6865  initializing the
+00001630: 2053 444b 2063 6c69 656e 7420 696e 7374   SDK client inst
+00001640: 616e 6365 2e20 466f 7220 6578 616d 706c  ance. For exampl
+00001650: 653a 0a20 2020 2020 2020 2060 6060 7079  e:.        ```py
+00001660: 7468 6f6e 0a20 2020 2020 2020 2069 6d70  thon.        imp
+00001670: 6f72 7420 6b65 796d 6174 6561 7069 0a20  ort keymateapi. 
+00001680: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001690: 7320 3d20 6b65 796d 6174 6561 7069 2e4b  s = keymateapi.K
+000016a0: 6579 6d61 7465 6170 6928 0a20 2020 2020  eymateapi(.     
+000016b0: 2020 2020 2020 2073 6572 7665 725f 7572         server_ur
+000016c0: 6c3d 2268 7474 7073 3a2f 2f73 6572 7665  l="https://serve
+000016d0: 722e 7365 6172 6368 7765 622e 6b65 796d  r.searchweb.keym
+000016e0: 6174 652e 6169 222c 0a20 2020 2020 2020  ate.ai",.       
+000016f0: 2020 2020 2062 6561 7265 725f 6175 7468       bearer_auth
+00001700: 3d22 3c59 4f55 525f 4245 4152 4552 5f54  ="<YOUR_BEARER_T
+00001710: 4f4b 454e 5f48 4552 453e 222c 0a20 2020  OKEN_HERE>",.   
+00001720: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
+00001730: 2020 2020 2020 2020 7265 7320 3d20 732e          res = s.
+00001740: 7570 7365 7274 2871 3d27 4920 7072 6566  upsert(q='I pref
+00001750: 6572 2043 6f73 7461 206f 7665 7220 5374  er Costa over St
+00001760: 6172 6275 636b 732e 2729 0a20 2020 2020  arbucks.').     
+00001770: 2020 200a 2020 2020 2020 2020 6966 2072     .        if r
+00001780: 6573 2e6f 626a 6563 7420 6973 206e 6f74  es.object is not
+00001790: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000017a0: 2020 2023 2068 616e 646c 6520 7265 7370     # handle resp
+000017b0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
+000017c0: 2070 6173 730a 2020 2020 2020 2020 0a20   pass.        . 
+000017d0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+000017e0: 2020 203c 212d 2d20 456e 6420 5365 7276     <!-- End Serv
+000017f0: 6572 2053 656c 6563 7469 6f6e 205b 7365  er Selection [se
+00001800: 7276 6572 5d20 2d2d 3e0a 2020 2020 2020  rver] -->.      
+00001810: 2020 0a20 2020 2020 2020 203c 212d 2d20    .        <!-- 
+00001820: 5374 6172 7420 4375 7374 6f6d 2048 5454  Start Custom HTT
+00001830: 5020 436c 6965 6e74 205b 6874 7470 2d63  P Client [http-c
+00001840: 6c69 656e 745d 202d 2d3e 0a20 2020 2020  lient] -->.     
+00001850: 2020 2023 2320 4375 7374 6f6d 2048 5454     ## Custom HTT
+00001860: 5020 436c 6965 6e74 0a20 2020 2020 2020  P Client.       
+00001870: 200a 2020 2020 2020 2020 5468 6520 5079   .        The Py
+00001880: 7468 6f6e 2053 444b 206d 616b 6573 2041  thon SDK makes A
+00001890: 5049 2063 616c 6c73 2075 7369 6e67 2074  PI calls using t
+000018a0: 6865 205b 7265 7175 6573 7473 5d28 6874  he [requests](ht
+000018b0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000018c0: 726f 6a65 6374 2f72 6571 7565 7374 732f  roject/requests/
+000018d0: 2920 4854 5450 206c 6962 7261 7279 2e20  ) HTTP library. 
+000018e0: 2049 6e20 6f72 6465 7220 746f 2070 726f   In order to pro
+000018f0: 7669 6465 2061 2063 6f6e 7665 6e69 656e  vide a convenien
+00001900: 7420 7761 7920 746f 2063 6f6e 6669 6775  t way to configu
+00001910: 7265 2074 696d 656f 7574 732c 2063 6f6f  re timeouts, coo
+00001920: 6b69 6573 2c20 7072 6f78 6965 732c 2063  kies, proxies, c
+00001930: 7573 746f 6d20 6865 6164 6572 732c 2061  ustom headers, a
+00001940: 6e64 206f 7468 6572 206c 6f77 2d6c 6576  nd other low-lev
+00001950: 656c 2063 6f6e 6669 6775 7261 7469 6f6e  el configuration
+00001960: 2c20 796f 7520 6361 6e20 696e 6974 6961  , you can initia
+00001970: 6c69 7a65 2074 6865 2053 444b 2063 6c69  lize the SDK cli
+00001980: 656e 7420 7769 7468 2061 2063 7573 746f  ent with a custo
+00001990: 6d20 6072 6571 7565 7374 732e 5365 7373  m `requests.Sess
+000019a0: 696f 6e60 206f 626a 6563 742e 0a20 2020  ion` object..   
+000019b0: 2020 2020 200a 2020 2020 2020 2020 466f       .        Fo
+000019c0: 7220 6578 616d 706c 652c 2079 6f75 2063  r example, you c
+000019d0: 6f75 6c64 2073 7065 6369 6679 2061 2068  ould specify a h
+000019e0: 6561 6465 7220 666f 7220 6576 6572 7920  eader for every 
+000019f0: 7265 7175 6573 7420 7468 6174 2074 6869  request that thi
+00001a00: 7320 7364 6b20 6d61 6b65 7320 6173 2066  s sdk makes as f
+00001a10: 6f6c 6c6f 7773 3a0a 2020 2020 2020 2020  ollows:.        
+00001a20: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+00001a30: 2020 696d 706f 7274 206b 6579 6d61 7465    import keymate
+00001a40: 6170 690a 2020 2020 2020 2020 696d 706f  api.        impo
+00001a50: 7274 2072 6571 7565 7374 730a 2020 2020  rt requests.    
+00001a60: 2020 2020 0a20 2020 2020 2020 2068 7474      .        htt
+00001a70: 705f 636c 6965 6e74 203d 2072 6571 7565  p_client = reque
+00001a80: 7374 732e 5365 7373 696f 6e28 290a 2020  sts.Session().  
+00001a90: 2020 2020 2020 6874 7470 5f63 6c69 656e        http_clien
+00001aa0: 742e 6865 6164 6572 732e 7570 6461 7465  t.headers.update
+00001ab0: 287b 2778 2d63 7573 746f 6d2d 6865 6164  ({'x-custom-head
+00001ac0: 6572 273a 2027 736f 6d65 5661 6c75 6527  er': 'someValue'
+00001ad0: 7d29 0a20 2020 2020 2020 2073 203d 206b  }).        s = k
+00001ae0: 6579 6d61 7465 6170 692e 4b65 796d 6174  eymateapi.Keymat
+00001af0: 6561 7069 2863 6c69 656e 743d 6874 7470  eapi(client=http
+00001b00: 5f63 6c69 656e 7429 0a20 2020 2020 2020  _client).       
+00001b10: 2060 6060 0a20 2020 2020 2020 203c 212d   ```.        <!-
+00001b20: 2d20 456e 6420 4375 7374 6f6d 2048 5454  - End Custom HTT
+00001b30: 5020 436c 6965 6e74 205b 6874 7470 2d63  P Client [http-c
+00001b40: 6c69 656e 745d 202d 2d3e 0a20 2020 2020  lient] -->.     
+00001b50: 2020 200a 2020 2020 2020 2020 3c21 2d2d     .        <!--
+00001b60: 2053 7461 7274 2041 7574 6865 6e74 6963   Start Authentic
+00001b70: 6174 696f 6e20 5b73 6563 7572 6974 795d  ation [security]
+00001b80: 202d 2d3e 0a20 2020 2020 2020 2023 2320   -->.        ## 
+00001b90: 4175 7468 656e 7469 6361 7469 6f6e 0a20  Authentication. 
+00001ba0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001bb0: 2323 2320 5065 722d 436c 6965 6e74 2053  ### Per-Client S
+00001bc0: 6563 7572 6974 7920 5363 6865 6d65 730a  ecurity Schemes.
+00001bd0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001be0: 2054 6869 7320 5344 4b20 7375 7070 6f72   This SDK suppor
+00001bf0: 7473 2074 6865 2066 6f6c 6c6f 7769 6e67  ts the following
+00001c00: 2073 6563 7572 6974 7920 7363 6865 6d65   security scheme
+00001c10: 2067 6c6f 6261 6c6c 793a 0a20 2020 2020   globally:.     
+00001c20: 2020 200a 2020 2020 2020 2020 7c20 4e61     .        | Na
+00001c30: 6d65 2020 2020 2020 2020 2020 7c20 5479  me          | Ty
+00001c40: 7065 2020 2020 2020 2020 2020 7c20 5363  pe          | Sc
+00001c50: 6865 6d65 2020 2020 2020 2020 7c0a 2020  heme        |.  
+00001c60: 2020 2020 2020 7c20 2d2d 2d2d 2d2d 2d2d        | --------
+00001c70: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+00001c80: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+00001c90: 2d2d 2d2d 2d20 7c0a 2020 2020 2020 2020  ----- |.        
+00001ca0: 7c20 6062 6561 7265 725f 6175 7468 6020  | `bearer_auth` 
+00001cb0: 7c20 6874 7470 2020 2020 2020 2020 2020  | http          
+00001cc0: 7c20 4854 5450 2042 6561 7265 7220 2020  | HTTP Bearer   
+00001cd0: 7c0a 2020 2020 2020 2020 0a20 2020 2020  |.        .     
+00001ce0: 2020 2054 6f20 6175 7468 656e 7469 6361     To authentica
+00001cf0: 7465 2077 6974 6820 7468 6520 4150 4920  te with the API 
+00001d00: 7468 6520 6062 6561 7265 725f 6175 7468  the `bearer_auth
+00001d10: 6020 7061 7261 6d65 7465 7220 6d75 7374  ` parameter must
+00001d20: 2062 6520 7365 7420 7768 656e 2069 6e69   be set when ini
+00001d30: 7469 616c 697a 696e 6720 7468 6520 5344  tializing the SD
+00001d40: 4b20 636c 6965 6e74 2069 6e73 7461 6e63  K client instanc
+00001d50: 652e 2046 6f72 2065 7861 6d70 6c65 3a0a  e. For example:.
+00001d60: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00001d70: 6e0a 2020 2020 2020 2020 696d 706f 7274  n.        import
+00001d80: 206b 6579 6d61 7465 6170 690a 2020 2020   keymateapi.    
+00001d90: 2020 2020 0a20 2020 2020 2020 2073 203d      .        s =
+00001da0: 206b 6579 6d61 7465 6170 692e 4b65 796d   keymateapi.Keym
+00001db0: 6174 6561 7069 280a 2020 2020 2020 2020  ateapi(.        
+00001dc0: 2020 2020 6265 6172 6572 5f61 7574 683d      bearer_auth=
+00001dd0: 223c 594f 5552 5f42 4541 5245 525f 544f  "<YOUR_BEARER_TO
+00001de0: 4b45 4e5f 4845 5245 3e22 2c0a 2020 2020  KEN_HERE>",.    
+00001df0: 2020 2020 290a 2020 2020 2020 2020 0a20      ).        . 
+00001e00: 2020 2020 2020 2072 6573 203d 2073 2e75         res = s.u
+00001e10: 7073 6572 7428 713d 2749 2070 7265 6665  psert(q='I prefe
+00001e20: 7220 436f 7374 6120 6f76 6572 2053 7461  r Costa over Sta
+00001e30: 7262 7563 6b73 2e27 290a 2020 2020 2020  rbucks.').      
+00001e40: 2020 0a20 2020 2020 2020 2069 6620 7265    .        if re
+00001e50: 732e 6f62 6a65 6374 2069 7320 6e6f 7420  s.object is not 
+00001e60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00001e70: 2020 2320 6861 6e64 6c65 2072 6573 706f    # handle respo
+00001e80: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
+00001e90: 7061 7373 0a20 2020 2020 2020 200a 2020  pass.        .  
+00001ea0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00001eb0: 2020 3c21 2d2d 2045 6e64 2041 7574 6865    <!-- End Authe
+00001ec0: 6e74 6963 6174 696f 6e20 5b73 6563 7572  ntication [secur
+00001ed0: 6974 795d 202d 2d3e 0a20 2020 2020 2020  ity] -->.       
+00001ee0: 200a 2020 2020 2020 2020 3c21 2d2d 2050   .        <!-- P
+00001ef0: 6c61 6365 686f 6c64 6572 2066 6f72 2046  laceholder for F
+00001f00: 7574 7572 6520 5370 6561 6b65 6173 7920  uture Speakeasy 
+00001f10: 5344 4b20 5365 6374 696f 6e73 202d 2d3e  SDK Sections -->
+00001f20: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001f30: 2020 2320 4465 7665 6c6f 706d 656e 740a    # Development.
+00001f40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001f50: 2023 2320 4d61 7475 7269 7479 0a20 2020   ## Maturity.   
+00001f60: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
+00001f70: 6973 2053 444b 2069 7320 696e 2062 6574  is SDK is in bet
+00001f80: 612c 2061 6e64 2074 6865 7265 206d 6179  a, and there may
+00001f90: 2062 6520 6272 6561 6b69 6e67 2063 6861   be breaking cha
+00001fa0: 6e67 6573 2062 6574 7765 656e 2076 6572  nges between ver
+00001fb0: 7369 6f6e 7320 7769 7468 6f75 7420 6120  sions without a 
+00001fc0: 6d61 6a6f 7220 7665 7273 696f 6e20 7570  major version up
+00001fd0: 6461 7465 2e20 5468 6572 6566 6f72 652c  date. Therefore,
+00001fe0: 2077 6520 7265 636f 6d6d 656e 6420 7069   we recommend pi
+00001ff0: 6e6e 696e 6720 7573 6167 650a 2020 2020  nning usage.    
+00002000: 2020 2020 746f 2061 2073 7065 6369 6669      to a specifi
+00002010: 6320 7061 636b 6167 6520 7665 7273 696f  c package versio
+00002020: 6e2e 2054 6869 7320 7761 792c 2079 6f75  n. This way, you
+00002030: 2063 616e 2069 6e73 7461 6c6c 2074 6865   can install the
+00002040: 2073 616d 6520 7665 7273 696f 6e20 6561   same version ea
+00002050: 6368 2074 696d 6520 7769 7468 6f75 7420  ch time without 
+00002060: 6272 6561 6b69 6e67 2063 6861 6e67 6573  breaking changes
+00002070: 2075 6e6c 6573 7320 796f 7520 6172 6520   unless you are 
+00002080: 696e 7465 6e74 696f 6e61 6c6c 790a 2020  intentionally.  
+00002090: 2020 2020 2020 6c6f 6f6b 696e 6720 666f        looking fo
+000020a0: 7220 7468 6520 6c61 7465 7374 2076 6572  r the latest ver
+000020b0: 7369 6f6e 2e0a 2020 2020 2020 2020 0a20  sion..        . 
+000020c0: 2020 2020 2020 2023 2320 436f 6e74 7269         ## Contri
+000020d0: 6275 7469 6f6e 730a 2020 2020 2020 2020  butions.        
+000020e0: 0a20 2020 2020 2020 2057 6869 6c65 2077  .        While w
+000020f0: 6520 7661 6c75 6520 6f70 656e 2d73 6f75  e value open-sou
+00002100: 7263 6520 636f 6e74 7269 6275 7469 6f6e  rce contribution
+00002110: 7320 746f 2074 6869 7320 5344 4b2c 2074  s to this SDK, t
+00002120: 6869 7320 6c69 6272 6172 7920 6973 2067  his library is g
+00002130: 656e 6572 6174 6564 2070 726f 6772 616d  enerated program
+00002140: 6d61 7469 6361 6c6c 792e 0a20 2020 2020  matically..     
+00002150: 2020 2046 6565 6c20 6672 6565 2074 6f20     Feel free to 
+00002160: 6f70 656e 2061 2050 5220 6f72 2061 2047  open a PR or a G
+00002170: 6974 6875 6220 6973 7375 6520 6173 2061  ithub issue as a
+00002180: 2070 726f 6f66 206f 6620 636f 6e63 6570   proof of concep
+00002190: 7420 616e 6420 7765 276c 6c20 646f 206f  t and we'll do o
+000021a0: 7572 2062 6573 7420 746f 2069 6e63 6c75  ur best to inclu
+000021b0: 6465 2069 7420 696e 2061 2066 7574 7572  de it in a futur
+000021c0: 6520 7265 6c65 6173 6521 0a20 2020 2020  e release!.     
+000021d0: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
+000021e0: 5344 4b20 4372 6561 7465 6420 6279 205b  SDK Created by [
+000021f0: 5370 6561 6b65 6173 795d 2868 7474 7073  Speakeasy](https
+00002200: 3a2f 2f64 6f63 732e 7370 6561 6b65 6173  ://docs.speakeas
+00002210: 7961 7069 2e64 6576 2f64 6f63 732f 7573  yapi.dev/docs/us
+00002220: 696e 672d 7370 6561 6b65 6173 792f 636c  ing-speakeasy/cl
+00002230: 6965 6e74 2d73 646b 7329 0a20 2020 2020  ient-sdks).     
+00002240: 2020 200a 506c 6174 666f 726d 3a20 554e     .Platform: UN
+00002250: 4b4e 4f57 4e0a 5265 7175 6972 6573 2d50  KNOWN.Requires-P
+00002260: 7974 686f 6e3a 203e 3d33 2e38 0a44 6573  ython: >=3.8.Des
+00002270: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00002280: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00002290: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+000022a0: 7472 613a 2064 6576 0a                   tra: dev.
```

### Comparing `keymateapi-0.3.3/README.md` & `keymateapi-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,9 @@
 # keymateapi
 
-<div align="left">
-    <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
-    <a href="https://opensource.org/licenses/MIT">
-        <img src="https://img.shields.io/badge/License-MIT-blue.svg" style="width: 100px; height: 28px;" />
-    </a>
-</div>
-
-
-## 🏗 **Welcome to your new SDK!** 🏗
-
-It has been generated successfully based on your OpenAPI spec. However, it is not yet ready for production use. Here are some next steps:
-- [ ] 🛠 Make your SDK feel handcrafted by [customizing it](https://www.speakeasyapi.dev/docs/customize-sdks)
-- [ ] ♻️ Refine your SDK quickly by iterating locally with the [Speakeasy CLI](https://github.com/speakeasy-api/speakeasy)
-- [ ] 🎁 Publish your SDK to package managers by [configuring automatic publishing](https://www.speakeasyapi.dev/docs/productionize-sdks/publish-sdks)
-- [ ] ✨ When ready to productionize, delete this section from the README
 
 <!-- Start SDK Installation [installation] -->
 ## SDK Installation
 
 ```bash
 pip install keymateapi
 ```
@@ -32,16 +17,15 @@
 ```python
 import keymateapi
 
 s = keymateapi.Keymateapi(
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-
-res = s.upsert(q='<value>')
+res = s.upsert(q='I prefer Costa over Starbucks.')
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End SDK Example Usage [usage] -->
@@ -65,36 +49,35 @@
 ## Error Handling
 
 Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 
 | Error Object                 | Status Code                  | Content Type                 |
 | ---------------------------- | ---------------------------- | ---------------------------- |
 | errors.BrowseurlResponseBody | 400                          | application/json             |
-| errors.SDKError              | 4x-5xx                       | */*                          |
+| errors.SDKError              | 4xx-5xx                      | */*                          |
 
 ### Example
 
 ```python
 import keymateapi
 from keymateapi.models import errors, operations
 
 s = keymateapi.Keymateapi(
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-req = operations.BrowseurlRequest(
-    inputwindowwords='<value>',
-    q='https://agreeable-jumbo.net',
-    percentile='<value>',
-    numofpages='<value>',
-)
-
 res = None
 try:
-    res = s.browseurl(req)
+    res = s.browseurl(request=operations.BrowseurlRequest(
+    inputwindowwords='10000',
+    q='https://keymate.ai',
+    percentile='1',
+    numofpages='1',
+    paging='1',
+))
 except errors.BrowseurlResponseBody as e:
     # handle exception
     raise(e)
 except errors.SDKError as e:
     # handle exception
     raise(e)
 
@@ -122,16 +105,15 @@
 import keymateapi
 
 s = keymateapi.Keymateapi(
     server_idx=0,
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-
-res = s.upsert(q='<value>')
+res = s.upsert(q='I prefer Costa over Starbucks.')
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 
@@ -143,16 +125,15 @@
 import keymateapi
 
 s = keymateapi.Keymateapi(
     server_url="https://server.searchweb.keymate.ai",
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-
-res = s.upsert(q='<value>')
+res = s.upsert(q='I prefer Costa over Starbucks.')
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End Server Selection [server] -->
@@ -165,15 +146,15 @@
 For example, you could specify a header for every request that this sdk makes as follows:
 ```python
 import keymateapi
 import requests
 
 http_client = requests.Session()
 http_client.headers.update({'x-custom-header': 'someValue'})
-s = keymateapi.Keymateapi(client: http_client)
+s = keymateapi.Keymateapi(client=http_client)
 ```
 <!-- End Custom HTTP Client [http-client] -->
 
 <!-- Start Authentication [security] -->
 ## Authentication
 
 ### Per-Client Security Schemes
@@ -188,16 +169,15 @@
 ```python
 import keymateapi
 
 s = keymateapi.Keymateapi(
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-
-res = s.upsert(q='<value>')
+res = s.upsert(q='I prefer Costa over Starbucks.')
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End Authentication [security] -->
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keymateapi-0.3.3/src/keymateapi/_hooks/sdkhooks.py` & `keymateapi-0.4.0/src/keymateapi/_hooks/sdkhooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple
 
 
 class SDKHooks(Hooks):
     def __init__(self):
         self.sdk_init_hooks: List[SDKInitHook] = []
         self.before_request_hooks: List[BeforeRequestHook] = []
         self.after_success_hooks: List[AfterSuccessHook] = []
@@ -25,27 +25,29 @@
         self.after_error_hooks.append(hook)
 
     def sdk_init(self, base_url: str, client: requests.Session) -> Tuple[str, requests.Session]:
         for hook in self.sdk_init_hooks:
             base_url, client = hook.sdk_init(base_url, client)
         return base_url, client
 
-    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> Union[requests.PreparedRequest, Exception]:
+    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> requests.PreparedRequest:
         for hook in self.before_request_hooks:
-            request = hook.before_request(hook_ctx, request)
-            if isinstance(request, Exception):
-                raise request
+            out = hook.before_request(hook_ctx, request)
+            if isinstance(out, Exception):
+                raise out
+            request = out
 
         return request
 
     def after_success(self, hook_ctx: AfterSuccessContext, response: requests.Response) -> requests.Response:
         for hook in self.after_success_hooks:
-            response = hook.after_success(hook_ctx, response)
-            if isinstance(response, Exception):
-                raise response
+            out = hook.after_success(hook_ctx, response)
+            if isinstance(out, Exception):
+                raise out
+            response = out
         return response
 
     def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests.Response], error: Optional[Exception]) -> Tuple[Optional[requests.Response], Optional[Exception]]:
         for hook in self.after_error_hooks:
             result = hook.after_error(hook_ctx, response, error)
             if isinstance(result, Exception):
                 raise result
```

### Comparing `keymateapi-0.3.3/src/keymateapi/_hooks/types.py` & `keymateapi-0.4.0/src/keymateapi/_hooks/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,23 +13,27 @@
     def __init__(self, operation_id: str, oauth2_scopes: Optional[List[str]], security_source: Optional[Union[Any, Callable[[], Any]]]):
         self.operation_id = operation_id
         self.oauth2_scopes = oauth2_scopes
         self.security_source = security_source
 
 
 class BeforeRequestContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class AfterSuccessContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    
 
 
 class AfterErrorContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class SDKInitHook(ABC):
     @abstractmethod
     def sdk_init(self, base_url: str, client: requests_http.Session) -> Tuple[str, requests_http.Session]:
         pass
 
@@ -38,21 +42,21 @@
     @abstractmethod
     def before_request(self, hook_ctx: BeforeRequestContext, request: requests_http.PreparedRequest) -> Union[requests_http.PreparedRequest, Exception]:
         pass
 
 
 class AfterSuccessHook(ABC):
     @abstractmethod
-    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.PreparedRequest, Exception]:
+    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.Response, Exception]:
         pass
 
 
 class AfterErrorHook(ABC):
     @abstractmethod
-    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.PreparedRequest], Optional[Exception]], Exception]:
+    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.Response], Optional[Exception]], Exception]:
         pass
 
 
 class Hooks(ABC):
     @abstractmethod
     def register_sdk_init_hook(self, hook: SDKInitHook):
         pass
```

### Comparing `keymateapi-0.3.3/src/keymateapi/models/components/browseresultitem.py` & `keymateapi-0.4.0/src/keymateapi/models/components/browseresultitem.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/components/browsewithproxyresultitem.py` & `keymateapi-0.4.0/src/keymateapi/models/components/browsewithproxyresultitem.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/components/httpmetadata.py` & `keymateapi-0.4.0/src/keymateapi/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/components/searchresultitem.py` & `keymateapi-0.4.0/src/keymateapi/models/components/searchresultitem.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/errors/__init__.py` & `keymateapi-0.4.0/src/keymateapi/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/errors/browse.py` & `keymateapi-0.4.0/src/keymateapi/models/errors/browse.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/errors/browseurl.py` & `keymateapi-0.4.0/src/keymateapi/models/errors/browseurl.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/errors/gptsbrowse.py` & `keymateapi-0.4.0/src/keymateapi/models/errors/gptsbrowse.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/errors/internetsearch.py` & `keymateapi-0.4.0/src/keymateapi/models/errors/internetsearch.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/errors/sdkerror.py` & `keymateapi-0.4.0/src/keymateapi/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/errors/search.py` & `keymateapi-0.4.0/src/keymateapi/models/errors/search.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/errors/ultrafastsearch.py` & `keymateapi-0.4.0/src/keymateapi/models/errors/ultrafastsearch.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/operations/__init__.py` & `keymateapi-0.4.0/src/keymateapi/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/operations/browse.py` & `keymateapi-0.4.0/src/keymateapi/models/operations/browse.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/operations/browseurl.py` & `keymateapi-0.4.0/src/keymateapi/models/operations/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,53 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import browsewithproxyresultitem as components_browsewithproxyresultitem
+from ...models.components import browseresultitem as components_browseresultitem
 from ...models.components import httpmetadata as components_httpmetadata
 from dataclasses_json import Undefined, dataclass_json
 from keymateapi import utils
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class BrowseurlRequest:
-    inputwindowwords: str = dataclasses.field(metadata={'query_param': { 'field_name': 'inputwindowwords', 'style': 'form', 'explode': True }})
-    r"""Always set this !! . Set it as '10000' first if responsetoolarge occurs reduce it to 2000."""
+class SearchRequest:
     q: str = dataclasses.field(metadata={'query_param': { 'field_name': 'q', 'style': 'form', 'explode': True }})
-    r"""URL of the website."""
-    percentile: str = dataclasses.field(metadata={'query_param': { 'field_name': 'percentile', 'style': 'form', 'explode': True }})
-    r"""Start it as '1', increase to '2' if ResponseTooLarge occurs you can multiply it with 2 for each retry."""
-    numofpages: str = dataclasses.field(metadata={'query_param': { 'field_name': 'numofpages', 'style': 'form', 'explode': True }})
-    r"""Set it as '1'"""
-    paging: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'paging', 'style': 'form', 'explode': True }})
-    r"""Set it as '1' first then according to results you can increase it by one to get the other part of the same page."""
+    r"""URL starting with https://memory.keymate.ai. Must be a valid URL."""
+    percentile: str = dataclasses.field(default='1', metadata={'query_param': { 'field_name': 'percentile', 'style': 'form', 'explode': True }})
+    r"""For adjusting response scope in case of 'ResponseTooLarge' error. Starts with 1."""
+    numofpages: str = dataclasses.field(default='1', metadata={'query_param': { 'field_name': 'numofpages', 'style': 'form', 'explode': True }})
+    r"""Specifies the number of pages to return. Starts with 1 by default."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class BrowseurlResponseResponseBody:
-    r"""Error fetching search results"""
+class SearchResponseResponseBody:
+    r"""Generic or unexpected error."""
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    r"""Error message"""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class BrowseurlResponseBody:
-    r"""Successful operation"""
+class SearchResponseBody:
+    r"""Successful operation. Returns fetched results along with applicable rules."""
     currentkeymateuser: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currentkeymateuser'), 'exclude': lambda f: f is None }})
     notice_for_human: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noticeForHuman'), 'exclude': lambda f: f is None }})
-    results: Optional[List[components_browsewithproxyresultitem.BrowsewithProxyResultItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+    results: Optional[List[components_browseresultitem.BrowseResultItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
     rules: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rules'), 'exclude': lambda f: f is None }})
-    r"""The rules which recommend gpt to follow."""
     
 
 
 
 @dataclasses.dataclass
-class BrowseurlResponse:
+class SearchResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    two_hundred_application_json_object: Optional[BrowseurlResponseBody] = dataclasses.field(default=None)
-    r"""Successful operation"""
-    default_application_json_object: Optional[BrowseurlResponseResponseBody] = dataclasses.field(default=None)
-    r"""Error fetching search results"""
+    two_hundred_application_json_object: Optional[SearchResponseBody] = dataclasses.field(default=None)
+    r"""Successful operation. Returns fetched results along with applicable rules."""
+    default_application_json_object: Optional[SearchResponseResponseBody] = dataclasses.field(default=None)
+    r"""Generic or unexpected error."""
```

### Comparing `keymateapi-0.3.3/src/keymateapi/models/operations/gptsbrowse.py` & `keymateapi-0.4.0/src/keymateapi/models/operations/gptsbrowse.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/operations/internetsearch.py` & `keymateapi-0.4.0/src/keymateapi/models/operations/internetsearch.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/operations/query.py` & `keymateapi-0.4.0/src/keymateapi/models/operations/query.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/operations/search.py` & `keymateapi-0.4.0/src/keymateapi/models/operations/browseurl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import browseresultitem as components_browseresultitem
+from ...models.components import browsewithproxyresultitem as components_browsewithproxyresultitem
 from ...models.components import httpmetadata as components_httpmetadata
 from dataclasses_json import Undefined, dataclass_json
 from keymateapi import utils
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class SearchRequest:
+class BrowseurlRequest:
+    inputwindowwords: str = dataclasses.field(metadata={'query_param': { 'field_name': 'inputwindowwords', 'style': 'form', 'explode': True }})
+    r"""Always set this !! . Set it as '10000' first if responsetoolarge occurs reduce it to 2000."""
     q: str = dataclasses.field(metadata={'query_param': { 'field_name': 'q', 'style': 'form', 'explode': True }})
-    r"""URL starting with https://memory.keymate.ai. Must be a valid URL."""
-    percentile: str = dataclasses.field(default='1', metadata={'query_param': { 'field_name': 'percentile', 'style': 'form', 'explode': True }})
-    r"""For adjusting response scope in case of 'ResponseTooLarge' error. Starts with 1."""
-    numofpages: str = dataclasses.field(default='1', metadata={'query_param': { 'field_name': 'numofpages', 'style': 'form', 'explode': True }})
-    r"""Specifies the number of pages to return. Starts with 1 by default."""
+    r"""URL of the website."""
+    percentile: str = dataclasses.field(metadata={'query_param': { 'field_name': 'percentile', 'style': 'form', 'explode': True }})
+    r"""Start it as '1', increase to '2' if ResponseTooLarge occurs you can multiply it with 2 for each retry."""
+    numofpages: str = dataclasses.field(metadata={'query_param': { 'field_name': 'numofpages', 'style': 'form', 'explode': True }})
+    r"""Set it as '1'"""
+    paging: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'paging', 'style': 'form', 'explode': True }})
+    r"""Set it as '1' first then according to results you can increase it by one to get the other part of the same page."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchResponseResponseBody:
-    r"""Generic or unexpected error."""
+class BrowseurlResponseResponseBody:
+    r"""Error fetching search results"""
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+    r"""Error message"""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchResponseBody:
-    r"""Successful operation. Returns fetched results along with applicable rules."""
+class BrowseurlResponseBody:
+    r"""Successful operation"""
     currentkeymateuser: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currentkeymateuser'), 'exclude': lambda f: f is None }})
     notice_for_human: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noticeForHuman'), 'exclude': lambda f: f is None }})
-    results: Optional[List[components_browseresultitem.BrowseResultItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+    results: Optional[List[components_browsewithproxyresultitem.BrowsewithProxyResultItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
     rules: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rules'), 'exclude': lambda f: f is None }})
+    r"""The rules which recommend gpt to follow."""
     
 
 
 
 @dataclasses.dataclass
-class SearchResponse:
+class BrowseurlResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    two_hundred_application_json_object: Optional[SearchResponseBody] = dataclasses.field(default=None)
-    r"""Successful operation. Returns fetched results along with applicable rules."""
-    default_application_json_object: Optional[SearchResponseResponseBody] = dataclasses.field(default=None)
-    r"""Generic or unexpected error."""
+    two_hundred_application_json_object: Optional[BrowseurlResponseBody] = dataclasses.field(default=None)
+    r"""Successful operation"""
+    two_hundred_text_plain_res: Optional[str] = dataclasses.field(default=None)
+    r"""Successful operation"""
+    default_application_json_object: Optional[BrowseurlResponseResponseBody] = dataclasses.field(default=None)
+    r"""Error fetching search results"""
+    default_text_plain_res: Optional[str] = dataclasses.field(default=None)
+    r"""Error fetching search results"""
```

### Comparing `keymateapi-0.3.3/src/keymateapi/models/operations/ultrafastsearch.py` & `keymateapi-0.4.0/src/keymateapi/models/operations/ultrafastsearch.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/models/operations/upsert.py` & `keymateapi-0.4.0/src/keymateapi/models/operations/upsert.py`

 * *Files identical despite different names*

### Comparing `keymateapi-0.3.3/src/keymateapi/sdk.py` & `keymateapi-0.4.0/src/keymateapi/sdk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
+from .utils.retries import RetryConfig
+from enum import Enum
 from keymateapi import utils
-from keymateapi._hooks import HookContext, SDKHooks
+from keymateapi._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext, SDKHooks
 from keymateapi.models import components, errors, operations
 from typing import Callable, Dict, Optional, Union
+class BrowseurlAcceptEnum(str, Enum):
+    APPLICATION_JSON = "application/json"
+    TEXT_PLAIN = "text/plain"
 
 class Keymateapi:
     r"""Keymate.AI Web Search API: Enhances knowledge grounded responses by fetching URLs optimized for specific needs and performing authenticated internet searches."""
 
     sdk_configuration: SDKConfiguration
 
     def __init__(self,
                  bearer_auth: Union[str, Callable[[], str]],
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
-                 retry_config: Optional[utils.RetryConfig] = None
+                 retry_config: Optional[RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param bearer_auth: The bearer_auth required for authentication
         :type bearer_auth: Union[str, Callable[[], str]]
         :param server_idx: The index of the server to use for all operations
         :type server_idx: int
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session
         :param retry_config: The utils.RetryConfig to use globally
-        :type retry_config: utils.RetryConfig
+        :type retry_config: RetryConfig
         """
         if client is None:
             client = requests_http.Session()
 
         if callable(bearer_auth):
             def security():
                 return components.Security(bearer_auth = bearer_auth())
         else:
             security = components.Security(bearer_auth = bearer_auth)
 
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
+    
 
         self.sdk_configuration = SDKConfiguration(
             client,
             security,
             server_url,
             server_idx,
             retry_config=retry_config
@@ -60,15 +66,15 @@
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
         if current_server_url != server_url:
             self.sdk_configuration.server_url = server_url
 
         # pylint: disable=protected-access
-        self.sdk_configuration._hooks = hooks
+        self.sdk_configuration.__dict__['_hooks'] = hooks
 
 
     def upsert(self, q: str) -> operations.UpsertResponse:
         r"""Inserts record to Keymate Memory.
         It records the passed string in q parameter to keymate memory
         """
         hook_ctx = HookContext(operation_id='upsert', oauth2_scopes=[], security_source=self.sdk_configuration.security)
@@ -81,44 +87,44 @@
         url = base_url + '/upsert'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.UpsertRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.UpsertResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UpsertResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -143,121 +149,132 @@
         url = base_url + '/query'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.QueryRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.QueryResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.QueryResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
 
 
-    def browseurl(self, request: operations.BrowseurlRequest) -> operations.BrowseurlResponse:
+    def browseurl(self, request: operations.BrowseurlRequest, accept_header_override: Optional[BrowseurlAcceptEnum] = None) -> operations.BrowseurlResponse:
         r"""The plugin enables user to conduct web browsing by extracting the text content of a specified URL. It will generate title and content.
         This is the most powerful browsing endpoints it uses residential proxies and bypasses firewalls. Try this with Reddit, LinkedIn etc.
         """
         hook_ctx = HookContext(operation_id='browseurl', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/browseurl'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.BrowseurlRequest, request), **query_params }
-        headers['Accept'] = 'application/json'
+        query_params = { **utils.get_query_params(request), **query_params }
+        if accept_header_override is not None:
+            headers['Accept'] = accept_header_override.value
+        else:
+            headers['Accept'] = 'application/json;q=1, text/plain;q=0'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.BrowseurlResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.BrowseurlResponseBody])
                 res.two_hundred_application_json_object = out
+            # pylint: disable=no-else-return
+            elif utils.match_content_type(http_res.headers.get('Content-Type') or '', 'text/plain'):                
+                res.two_hundred_text_plain_res = http_res.text
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BrowseurlResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.BrowseurlResponseResponseBody])
                 res.default_application_json_object = out
+            # pylint: disable=no-else-return
+            elif utils.match_content_type(http_res.headers.get('Content-Type') or '', 'text/plain'):                
+                res.default_text_plain_res = http_res.text
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
 
@@ -279,69 +296,72 @@
         url = base_url + '/browse'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.BrowseRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.BrowseResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.BrowseResponseBody])
                 res.two_hundred_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BrowseResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BrowseResponseResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.BrowseResponseResponseBody])
                 res.default_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
@@ -364,69 +384,72 @@
         url = base_url + '/search'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.SearchRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.SearchResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchResponseBody])
                 res.two_hundred_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.SearchResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.SearchResponseResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchResponseResponseBody])
                 res.default_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
@@ -449,61 +472,63 @@
         url = base_url + '/ultrafastsearch'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.UltrafastsearchRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.UltrafastsearchResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UltrafastsearchResponseBody])
                 res.two_hundred_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.UltrafastsearchResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UltrafastsearchResponseResponseBody])
                 res.default_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
@@ -527,69 +552,72 @@
         url = base_url + '/gptsbrowse'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GptsbrowseRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.GptsbrowseResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GptsbrowseResponseBody])
                 res.two_hundred_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GptsbrowseResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GptsbrowseResponseResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GptsbrowseResponseResponseBody])
                 res.default_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
@@ -613,69 +641,72 @@
         url = base_url + '/internetsearch'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.InternetsearchRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.InternetsearchResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.InternetsearchResponseBody])
                 res.two_hundred_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.InternetsearchResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.InternetsearchResponseResponseBody)
                 out.http_meta = components.HTTPMetadata(request=req, response=http_res)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.InternetsearchResponseResponseBody])
                 res.default_application_json_object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `keymateapi-0.3.3/src/keymateapi/sdkconfiguration.py` & `keymateapi-0.4.0/src/keymateapi/sdkconfiguration.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,40 @@
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from dataclasses import dataclass
 from keymateapi.models import components
-from typing import Callable, Dict, Tuple, Union
+from typing import Callable, Dict, Optional, Tuple, Union
 
 
 SERVERS = [
     'https://server.searchweb.keymate.ai',
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
-    server_url: str = ''
-    server_idx: int = 0
+    server_url: Optional[str] = ''
+    server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.2'
-    sdk_version: str = '0.3.3'
-    gen_version: str = '2.286.7'
-    user_agent: str = 'speakeasy-sdk/python 0.3.3 2.286.7 1.0.2 keymateapi'
-    retry_config: RetryConfig = None
-    _hooks: SDKHooks = None
+    sdk_version: str = '0.4.0'
+    gen_version: str = '2.333.3'
+    user_agent: str = 'speakeasy-sdk/python 0.4.0 2.333.3 1.0.2 keymateapi'
+    retry_config: Optional[RetryConfig] = None
+
+    def __post_init__(self):
+        self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url:
+        if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], {}
```

### Comparing `keymateapi-0.3.3/src/keymateapi/utils/retries.py` & `keymateapi-0.4.0/src/keymateapi/utils/retries.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
@@ -110,11 +110,10 @@
             if now - start > max_elapsed_time:
                 if isinstance(exception, TemporaryError):
                     return exception.response
 
                 raise
             sleep = ((initial_interval/1000) *
                      exponent**retries + random.uniform(0, 1))
-            if sleep > max_interval/1000:
-                sleep = max_interval/1000
+            sleep = min(sleep, max_interval / 1000)
             time.sleep(sleep)
             retries += 1
```

### Comparing `keymateapi-0.3.3/src/keymateapi/utils/utils.py` & `keymateapi-0.4.0/src/keymateapi/utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,25 @@
 import re
 import sys
 from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
-                    get_args, get_origin)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    get_origin,
+)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
 from dataclasses_json import DataClassJsonMixin
 
 
 def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
@@ -26,470 +35,600 @@
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get('security')
+        metadata = sec_field.metadata.get("security")
         if metadata is None:
             continue
-        if metadata.get('option'):
+        if metadata.get("option"):
             _parse_security_option(headers, query_params, value)
             return headers, query_params
-        if metadata.get('scheme'):
+        if metadata.get("scheme"):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
                 _parse_security_scheme(headers, query_params, metadata, security)
             else:
                 _parse_security_scheme(headers, query_params, metadata, value)
 
     return headers, query_params
 
 
-def _parse_security_option(headers: Dict[str, str], query_params: Dict[str, str], option: Any):
+def _parse_security_option(
+    headers: Dict[str, str], query_params: Dict[str, str], option: Any
+):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get('security')
-        if metadata is None or metadata.get('scheme') is None:
+        metadata = opt_field.metadata.get("security")
+        if metadata is None or metadata.get("scheme") is None:
             continue
         _parse_security_scheme(
-            headers, query_params, metadata, getattr(option, opt_field.name))
+            headers, query_params, metadata, getattr(option, opt_field.name)
+        )
 
 
-def _parse_security_scheme(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, scheme: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    scheme: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
     if is_dataclass(scheme):
-        if scheme_type == 'http' and sub_type == 'basic':
+        if scheme_type == "http" and sub_type == "basic":
             _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get('security')
-            if metadata is None or metadata.get('field_name') is None:
+            metadata = scheme_field.metadata.get("security")
+            if metadata is None or metadata.get("field_name") is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                headers, query_params, scheme_metadata, metadata, value)
+                headers, query_params, scheme_metadata, metadata, value
+            )
     else:
         _parse_security_scheme_value(
-            headers, query_params, scheme_metadata, scheme_metadata, scheme)
+            headers, query_params, scheme_metadata, scheme_metadata, scheme
+        )
 
 
-def _parse_security_scheme_value(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, security_metadata: Dict, value: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme_value(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    security_metadata: Dict,
+    value: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
-    header_name = str(security_metadata.get('field_name'))
+    header_name = str(security_metadata.get("field_name"))
 
     if scheme_type == "apiKey":
-        if sub_type == 'header':
+        if sub_type == "header":
             headers[header_name] = value
-        elif sub_type == 'query':
+        elif sub_type == "query":
             query_params[header_name] = value
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     elif scheme_type == "openIdConnect":
         headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'oauth2':
-        if sub_type != 'client_credentials':
+    elif scheme_type == "oauth2":
+        if sub_type != "client_credentials":
             headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'http':
-        if sub_type == 'bearer':
+    elif scheme_type == "http":
+        if sub_type == "bearer":
             headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     else:
-        raise Exception('not supported')
+        raise Exception("not supported")
 
 
 def _apply_bearer(token: str) -> str:
-    return token.lower().startswith('bearer ') and token or f'Bearer {token}'
+    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
 
 
 def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
+        metadata = scheme_field.metadata.get("security")
+        if metadata is None or metadata.get("field_name") is None:
             continue
 
-        field_name = metadata.get('field_name')
+        field_name = metadata.get("field_name")
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == 'username':
+        if field_name == "username":
             username = value
-        if field_name == 'password':
+        if field_name == "password":
             password = value
 
-    data = f'{username}:{password}'.encode()
-    headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
+    data = f"{username}:{password}".encode()
+    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: Any,
-                 gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(
+    server_url: str,
+    path: str,
+    path_params: Any,
+    gbls: Optional[Any] = None,
+) -> str:
+    path_param_values: Dict[str, str] = {}
+
+    globals_already_populated = _populate_path_params(
+        path_params, gbls, path_param_values, []
+    )
+    if gbls is not None:
+        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
+
+    for key, value in path_param_values.items():
+        path = path.replace("{" + key + "}", value, 1)
+
+    return remove_suffix(server_url, "/") + path
+
+
+def _populate_path_params(
+    path_params: Any,
+    gbls: Any,
+    path_param_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        param_metadata = field.metadata.get('path_param')
+        param_metadata = field.metadata.get("path_param")
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        param = getattr(path_params, field.name) if path_params is not None else None
+        param, global_found = _populate_from_globals(
+            field.name, param, "path_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
+        serialization = param_metadata.get("serialization", "")
+        if serialization != "":
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param)
+                param_metadata, field.type, f_name, param
+            )
             for key, value in serialized_params.items():
-                path = path.replace(
-                    '{' + key + '}', value, 1)
+                path_param_values[key] = value
         else:
-            if param_metadata.get('style', 'simple') == 'simple':
+            if param_metadata.get("style", "simple") == "simple":
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get("explode"):
+                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
+                        param_value_metadata = param_field.metadata.get("path_param")
                         if not param_value_metadata:
                             continue
 
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
+                        param_name = param_value_metadata.get("field_name", field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get('explode'):
+                        if param_metadata.get("explode"):
                             pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
+                                f"{param_name}={_val_to_string(param_field_val)}"
+                            )
                         else:
                             pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                                f"{param_name},{_val_to_string(param_field_val)}"
+                            )
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        _val_to_string(param)
+                    )
 
-    return remove_suffix(server_url, '/') + path
+    return globals_already_populated
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace(
-            '{' + key + '}', value)
+        url_with_params = url_with_params.replace("{" + key + "}", value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[
-        str, List[str]]:
+def get_query_params(
+    query_params: Any,
+    gbls: Optional[Any] = None,
+) -> Dict[str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
+    if gbls is not None:
+        _populate_query_params(gbls, None, params, globals_already_populated)
+
+    return params
+
+
+def _populate_query_params(
+    query_params: Any,
+    gbls: Any,
+    query_param_values: Dict[str, List[str]],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        metadata = field.metadata.get('query_param')
+        metadata = field.metadata.get("query_param")
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
+        value = getattr(query_params, param_name) if query_params is not None else None
 
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
+        value, global_found = _populate_from_globals(
+            param_name, value, "query_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(param_name)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get('serialization', '')
-        if serialization != '':
+        serialization = metadata.get("serialization", "")
+        if serialization != "":
             serialized_parms = _get_serialized_params(
-                metadata, field.type, f_name, value)
+                metadata, field.type, f_name, value
+            )
             for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
+                if key in query_param_values:
+                    query_param_values[key].extend(value)
                 else:
-                    params[key] = [value]
+                    query_param_values[key] = [value]
         else:
-            style = metadata.get('style', 'form')
-            if style == 'deepObject':
-                params = {**params, **_get_deep_object_query_params(
-                    metadata, f_name, value)}
-            elif style == 'form':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, ",")}
-            elif style == 'pipeDelimited':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, "|")}
+            style = metadata.get("style", "form")
+            if style == "deepObject":
+                _populate_deep_object_query_params(
+                    metadata, f_name, value, query_param_values
+                )
+            elif style == "form":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, ",", query_param_values
+                )
+            elif style == "pipeDelimited":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, "|", query_param_values
+                )
             else:
-                raise Exception('not yet implemented')
-    return params
+                raise Exception("not yet implemented")
 
+    return globals_already_populated
 
-def get_headers(headers_params: Any) -> Dict[str, str]:
-    if headers_params is None:
-        return {}
 
+def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    param_fields: Tuple[Field, ...] = fields(headers_params)
-    for field in param_fields:
-        metadata = field.metadata.get('header')
-        if not metadata:
-            continue
+    globals_already_populated = []
+    if headers_params is not None:
+        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
+    if gbls is not None:
+        _populate_headers(gbls, None, headers, globals_already_populated)
 
-        value = _serialize_header(metadata.get(
-            'explode', False), getattr(headers_params, field.name))
+    return headers
 
-        if value != '':
-            headers[metadata.get('field_name', field.name)] = value
 
-    return headers
+def _populate_headers(
+    headers_params: Any,
+    gbls: Any,
+    header_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
 
+    param_fields: Tuple[Field, ...] = fields(headers_params)
+    for field in param_fields:
+        if field.name in skip_fields:
+            continue
+
+        metadata = field.metadata.get("header")
+        if not metadata:
+            continue
 
-def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: Any) -> Dict[str, str]:
+        value, global_found = _populate_from_globals(
+            field.name, getattr(headers_params, field.name), "header", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
+        value = _serialize_header(metadata.get("explode", False), value)
+
+        if value != "":
+            header_values[metadata.get("field_name", field.name)] = value
+
+    return globals_already_populated
+
+
+def _get_serialized_params(
+    metadata: Dict, field_type: type, field_name: str, obj: Any
+) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get('serialization', '')
-    if serialization == 'json':
-        params[metadata.get("field_name", field_name)
-               ] = marshal_json(obj, field_type)
+    serialization = metadata.get("serialization", "")
+    if serialization == "json":
+        params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
 
     return params
 
 
-def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: Any) -> Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_deep_object_query_params(
+    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
+):
     if obj is None:
-        return params
+        return
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('query_param')
+            obj_param_metadata = obj_field.metadata.get("query_param")
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                    if (
+                        params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        )
+                        is None
+                    ):
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                        ]
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        ] = []
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                    ].append(_val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    _val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                ] = [_val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                        ]
-
-                    params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
+                    if (
+                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
+                        is None
+                    ):
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
+
+                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
+                        _val_to_string(val)
+                    )
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)]
-    return params
+                    _val_to_string(value)
+                ]
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('query_param')
+    obj_param_metadata = obj_field.metadata.get("query_param")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: Dict, field_name: str, obj: Any, delimiter: str) -> Dict[
-        str, List[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _populate_delimited_query_params(
+    metadata: Dict,
+    field_name: str,
+    obj: Any,
+    delimiter: str,
+    query_param_values: Dict[str, List[str]],
+):
+    _populate_form(
+        field_name,
+        metadata.get("explode", True),
+        obj,
+        _get_query_param_field_name,
+        delimiter,
+        query_param_values,
+    )
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    "json": "application/json",
+    "form": "application/x-www-form-urlencoded",
+    "multipart": "multipart/form-data",
+    "raw": "application/octet-stream",
+    "string": "text/plain",
 }
 
 
-def serialize_request_body(request: Any, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
-        Optional[str], Optional[Any], Optional[Any]]:
+def serialize_request_body(
+    request: Any,
+    request_type: type,
+    request_field_name: str,
+    nullable: bool,
+    optional: bool,
+    serialization_method: str,
+    encoder=None,
+) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request, encoder)
+        return serialize_content_type(
+            request_field_name,
+            request_type,
+            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+            request,
+            encoder,
+        )
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get('request')
+            request_metadata = field.metadata.get("request")
             break
 
     if request_metadata is None:
-        raise Exception('invalid request type')
+        raise Exception("invalid request type")
 
-    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(
+        request_field_name,
+        request_type,
+        request_metadata.get("media_type", "application/octet-stream"),
+        request_val,
+    )
 
 
-def serialize_content_type(field_name: str, request_type: Any, media_type: str, request: Any, encoder=None) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
+def serialize_content_type(
+    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
+) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r'multipart\/.*', media_type) is not None:
+    if re.match(r"multipart\/.*", media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
+    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}")
+        f"invalid request body type {type(request)} for mediaType {media_type}"
+    )
 
 
-def serialize_multipart_form(media_type: str, request: Any) -> Tuple[str, Any, List[List[Any]]]:
+def serialize_multipart_form(
+    media_type: str, request: Any
+) -> Tuple[str, Any, List[List[Any]]]:
     form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get('multipart_form')
+        field_metadata = field.metadata.get("multipart_form")
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get('multipart_form')
+                file_metadata = file_field.metadata.get("multipart_form")
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get(
-                        "field_name", file_field.name)
+                    field_name = file_metadata.get("field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception('invalid multipart/form-data file')
+                raise Exception("invalid multipart/form-data file")
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [field_metadata.get("field_name", field.name), [
-                None, marshal_json(val, field.type), "application/json"]]
+            to_append = [
+                field_metadata.get("field_name", field.name),
+                [None, marshal_json(val, field.type), "application/json"],
+            ]
             form.append(to_append)
         else:
-            field_name = field_metadata.get(
-                "field_name", field.name)
+            field_name = field_metadata.get("field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append(
-                        [field_name + "[]", [None, _val_to_string(value)]])
+                    form.append([field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
-        str, List[str]]:
+def serialize_dict(
+    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
+) -> Dict[str, List[str]]:
     if existing is None:
         existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,215 +649,218 @@
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get('form')
+            metadata = field.metadata.get("form")
             if metadata is None:
                 continue
 
-            field_name = metadata.get('field_name', field.name)
+            field_name = metadata.get("field_name", field.name)
 
-            if metadata.get('json'):
+            if metadata.get("json"):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get('style', 'form') == 'form':
-                    form = {**form, **_populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
+                if metadata.get("style", "form") == "form":
+                    _populate_form(
+                        field_name,
+                        metadata.get("explode", True),
+                        val,
+                        _get_form_field_name,
+                        ",",
+                        form,
+                    )
                 else:
-                    raise Exception(
-                        f'Invalid form style for field {field.name}')
+                    raise Exception(f"Invalid form style for field {field.name}")
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f'Invalid request body type for field {field_name}')
+        raise Exception(f"Invalid request body type for field {field_name}")
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('form')
+    obj_param_metadata = obj_field.metadata.get("form")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: Any, get_field_name_func: Callable, delimiter: str) -> \
-        Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_form(
+    field_name: str,
+    explode: boolean,
+    obj: Any,
+    get_field_name_func: Callable,
+    delimiter: str,
+    form: Dict[str, List[str]],
+):
     if obj is None:
-        return params
+        return form
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == '':
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [_val_to_string(val)]
+                form[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = [_val_to_string(value)]
+                form[key] = [_val_to_string(value)]
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f"{key}{delimiter}{_val_to_string(value)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in params:
-                    params[field_name] = []
-                params[field_name].append(_val_to_string(value))
+                if not field_name in form:
+                    form[field_name] = []
+                form[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(
-                [str(item) for item in items])]
+            form[field_name] = [delimiter.join([str(item) for item in items])]
     else:
-        params[field_name] = [_val_to_string(obj)]
+        form[field_name] = [_val_to_string(obj)]
 
-    return params
+    return form
 
 
 def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ''
+        return ""
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('header')
+            obj_param_metadata = obj_field.metadata.get("header")
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get(
-                'field_name', obj_field.name)
-            if obj_field_name == '':
+            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(
-                    f'{obj_field_name}={_val_to_string(val)}')
+                items.append(f"{obj_field_name}={_val_to_string(val)}")
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={_val_to_string(value)}')
+                items.append(f"{key}={_val_to_string(value)}")
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join([str(item) for item in items])
+            return ",".join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     else:
-        return f'{_val_to_string(obj)}'
+        return f"{_val_to_string(obj)}"
 
-    return ''
+    return ""
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
-                               bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f'unable to unmarshal {data} as {typ} - {attr_err}') from attr_err
+            f"unable to unmarshal {data} as {typ} - {attr_err}"
+        ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
-        raise ValueError(
-            f"Could not marshal None into non-optional type: {typ}")
+        raise ValueError(f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass('Marshal', [('res', typ)],
-                             bases=(DataClassJsonMixin,))
+    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(',', ':'), sort_keys=True)
+    return json.dumps(val, separators=(",", ":"), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg['content-type'] = content_type
+    msg["content-type"] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
+        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
             return True
 
     return False
 
 
 def match_status_codes(status_codes: List[str], status_code: int) -> bool:
     for code in status_codes:
@@ -762,14 +904,41 @@
 
 
 def bigintdecoder(val):
     if isinstance(val, float):
         raise ValueError(f"{val} is a float")
     return int(val)
 
+def integerstrencoder(optional: bool):
+    def integerstrencode(val: int):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return integerstrencode
+
+
+def integerstrdecoder(val):
+    if isinstance(val, float):
+        raise ValueError(f"{val} is a float")
+    return int(val)
+
+
+def numberstrencoder(optional: bool):
+    def numberstrencode(val: float):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return numberstrencode
+
+
+def numberstrdecoder(val):
+    return float(val)
+
 
 def decimalencoder(optional: bool, as_str: bool):
     def decimalencode(val: Decimal):
         if optional and val is None:
             return None
 
         if as_str:
@@ -835,64 +1004,84 @@
 
 
 def union_encoder(all_encoders: Dict[str, Callable]):
     def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
+
     return selective_encoder
 
 
 def union_decoder(all_decoders: List[Callable]):
     def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
+
     return selective_decoder
 
 
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
 def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return str(val.isoformat().replace('+00:00', 'Z'))
+        return str(val.isoformat().replace("+00:00", "Z"))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(param_name: str, value: Any, param_type: str, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
+def _populate_from_globals(
+    param_name: str, value: Any, param_type: str, gbls: Any
+) -> Tuple[Any, bool]:
+    if gbls is None:
+        return value, False
+
+    global_fields = fields(gbls)
+
+    found = False
+    for field in global_fields:
+        if field.name is not param_name:
+            continue
+
+        found = True
+
+        if value is not None:
+            return value, True
 
-    return value
+        global_value = getattr(gbls, field.name)
+
+        param_metadata = field.metadata.get(param_type)
+        if param_metadata is None:
+            return value, True
+
+        return global_value, True
+
+    return value, found
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules['sdk.models.components'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models.components"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

### Comparing `keymateapi-0.3.3/src/keymateapi.egg-info/PKG-INFO` & `keymateapi-0.4.0/src/keymateapi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,590 +1,555 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6b65 796d  : 2.1.Name: keym
 00000020: 6174 6561 7069 0a56 6572 7369 6f6e 3a20  ateapi.Version: 
-00000030: 302e 332e 330a 5375 6d6d 6172 793a 2050  0.3.3.Summary: P
+00000030: 302e 342e 300a 5375 6d6d 6172 793a 2050  0.4.0.Summary: P
 00000040: 7974 686f 6e20 436c 6965 6e74 2053 444b  ython Client SDK
 00000050: 2047 656e 6572 6174 6564 2062 7920 5370   Generated by Sp
 00000060: 6561 6b65 6173 790a 486f 6d65 2d70 6167  eakeasy.Home-pag
-00000070: 653a 2055 4e4b 4e4f 574e 0a41 7574 686f  e: UNKNOWN.Autho
-00000080: 723a 2053 7065 616b 6561 7379 0a4c 6963  r: Speakeasy.Lic
-00000090: 656e 7365 3a20 554e 4b4e 4f57 4e0a 4465  ense: UNKNOWN.De
-000000a0: 7363 7269 7074 696f 6e3a 2023 206b 6579  scription: # key
-000000b0: 6d61 7465 6170 690a 2020 2020 2020 2020  mateapi.        
-000000c0: 0a20 2020 2020 2020 203c 6469 7620 616c  .        <div al
-000000d0: 6967 6e3d 226c 6566 7422 3e0a 2020 2020  ign="left">.    
-000000e0: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-000000f0: 2268 7474 7073 3a2f 2f73 7065 616b 6561  "https://speakea
-00000100: 7379 6170 692e 6465 762f 223e 3c69 6d67  syapi.dev/"><img
-00000110: 2073 7263 3d22 6874 7470 733a 2f2f 6375   src="https://cu
-00000120: 7374 6f6d 2d69 636f 6e2d 6261 6467 6573  stom-icon-badges
-00000130: 2e64 656d 6f6c 6162 2e63 6f6d 2f62 6164  .demolab.com/bad
-00000140: 6765 2f2d 4275 696c 7425 3230 4279 2532  ge/-Built%20By%2
-00000150: 3053 7065 616b 6561 7379 2d32 3132 3031  0Speakeasy-21201
-00000160: 353f 7374 796c 653d 666f 722d 7468 652d  5?style=for-the-
-00000170: 6261 6467 6526 6c6f 676f 436f 6c6f 723d  badge&logoColor=
-00000180: 4642 4533 3331 266c 6f67 6f3d 7370 6561  FBE331&logo=spea
-00000190: 6b65 6173 7926 6c61 6265 6c43 6f6c 6f72  keasy&labelColor
-000001a0: 3d35 3435 3435 3422 202f 3e3c 2f61 3e0a  =545454" /></a>.
-000001b0: 2020 2020 2020 2020 2020 2020 3c61 2068              <a h
-000001c0: 7265 663d 2268 7474 7073 3a2f 2f6f 7065  ref="https://ope
-000001d0: 6e73 6f75 7263 652e 6f72 672f 6c69 6365  nsource.org/lice
-000001e0: 6e73 6573 2f4d 4954 223e 0a20 2020 2020  nses/MIT">.     
-000001f0: 2020 2020 2020 2020 2020 203c 696d 6720             <img 
-00000200: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000210: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000220: 652f 4c69 6365 6e73 652d 4d49 542d 626c  e/License-MIT-bl
-00000230: 7565 2e73 7667 2220 7374 796c 653d 2277  ue.svg" style="w
-00000240: 6964 7468 3a20 3130 3070 783b 2068 6569  idth: 100px; hei
-00000250: 6768 743a 2032 3870 783b 2220 2f3e 0a20  ght: 28px;" />. 
-00000260: 2020 2020 2020 2020 2020 203c 2f61 3e0a             </a>.
-00000270: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000280: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000290: 0a20 2020 2020 2020 2023 2320 f09f 8f97  .        ## ....
-000002a0: 202a 2a57 656c 636f 6d65 2074 6f20 796f   **Welcome to yo
-000002b0: 7572 206e 6577 2053 444b 212a 2a20 f09f  ur new SDK!** ..
-000002c0: 8f97 0a20 2020 2020 2020 200a 2020 2020  ...        .    
-000002d0: 2020 2020 4974 2068 6173 2062 6565 6e20      It has been 
-000002e0: 6765 6e65 7261 7465 6420 7375 6363 6573  generated succes
-000002f0: 7366 756c 6c79 2062 6173 6564 206f 6e20  sfully based on 
-00000300: 796f 7572 204f 7065 6e41 5049 2073 7065  your OpenAPI spe
-00000310: 632e 2048 6f77 6576 6572 2c20 6974 2069  c. However, it i
-00000320: 7320 6e6f 7420 7965 7420 7265 6164 7920  s not yet ready 
-00000330: 666f 7220 7072 6f64 7563 7469 6f6e 2075  for production u
-00000340: 7365 2e20 4865 7265 2061 7265 2073 6f6d  se. Here are som
-00000350: 6520 6e65 7874 2073 7465 7073 3a0a 2020  e next steps:.  
-00000360: 2020 2020 2020 2d20 5b20 5d20 f09f 9ba0        - [ ] ....
-00000370: 204d 616b 6520 796f 7572 2053 444b 2066   Make your SDK f
-00000380: 6565 6c20 6861 6e64 6372 6166 7465 6420  eel handcrafted 
-00000390: 6279 205b 6375 7374 6f6d 697a 696e 6720  by [customizing 
-000003a0: 6974 5d28 6874 7470 733a 2f2f 7777 772e  it](https://www.
-000003b0: 7370 6561 6b65 6173 7961 7069 2e64 6576  speakeasyapi.dev
-000003c0: 2f64 6f63 732f 6375 7374 6f6d 697a 652d  /docs/customize-
-000003d0: 7364 6b73 290a 2020 2020 2020 2020 2d20  sdks).        - 
-000003e0: 5b20 5d20 e299 bbef b88f 2052 6566 696e  [ ] ...... Refin
-000003f0: 6520 796f 7572 2053 444b 2071 7569 636b  e your SDK quick
-00000400: 6c79 2062 7920 6974 6572 6174 696e 6720  ly by iterating 
-00000410: 6c6f 6361 6c6c 7920 7769 7468 2074 6865  locally with the
-00000420: 205b 5370 6561 6b65 6173 7920 434c 495d   [Speakeasy CLI]
-00000430: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000440: 636f 6d2f 7370 6561 6b65 6173 792d 6170  com/speakeasy-ap
-00000450: 692f 7370 6561 6b65 6173 7929 0a20 2020  i/speakeasy).   
-00000460: 2020 2020 202d 205b 205d 20f0 9f8e 8120       - [ ] .... 
-00000470: 5075 626c 6973 6820 796f 7572 2053 444b  Publish your SDK
-00000480: 2074 6f20 7061 636b 6167 6520 6d61 6e61   to package mana
-00000490: 6765 7273 2062 7920 5b63 6f6e 6669 6775  gers by [configu
-000004a0: 7269 6e67 2061 7574 6f6d 6174 6963 2070  ring automatic p
-000004b0: 7562 6c69 7368 696e 675d 2868 7474 7073  ublishing](https
-000004c0: 3a2f 2f77 7777 2e73 7065 616b 6561 7379  ://www.speakeasy
-000004d0: 6170 692e 6465 762f 646f 6373 2f70 726f  api.dev/docs/pro
-000004e0: 6475 6374 696f 6e69 7a65 2d73 646b 732f  ductionize-sdks/
-000004f0: 7075 626c 6973 682d 7364 6b73 290a 2020  publish-sdks).  
-00000500: 2020 2020 2020 2d20 5b20 5d20 e29c a820        - [ ] ... 
-00000510: 5768 656e 2072 6561 6479 2074 6f20 7072  When ready to pr
-00000520: 6f64 7563 7469 6f6e 697a 652c 2064 656c  oductionize, del
-00000530: 6574 6520 7468 6973 2073 6563 7469 6f6e  ete this section
-00000540: 2066 726f 6d20 7468 6520 5245 4144 4d45   from the README
-00000550: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000560: 2020 3c21 2d2d 2053 7461 7274 2053 444b    <!-- Start SDK
-00000570: 2049 6e73 7461 6c6c 6174 696f 6e20 5b69   Installation [i
-00000580: 6e73 7461 6c6c 6174 696f 6e5d 202d 2d3e  nstallation] -->
-00000590: 0a20 2020 2020 2020 2023 2320 5344 4b20  .        ## SDK 
-000005a0: 496e 7374 616c 6c61 7469 6f6e 0a20 2020  Installation.   
-000005b0: 2020 2020 200a 2020 2020 2020 2020 6060       .        ``
-000005c0: 6062 6173 680a 2020 2020 2020 2020 7069  `bash.        pi
-000005d0: 7020 696e 7374 616c 6c20 6b65 796d 6174  p install keymat
-000005e0: 6561 7069 0a20 2020 2020 2020 2060 6060  eapi.        ```
-000005f0: 0a20 2020 2020 2020 203c 212d 2d20 456e  .        <!-- En
-00000600: 6420 5344 4b20 496e 7374 616c 6c61 7469  d SDK Installati
-00000610: 6f6e 205b 696e 7374 616c 6c61 7469 6f6e  on [installation
-00000620: 5d20 2d2d 3e0a 2020 2020 2020 2020 0a20  ] -->.        . 
-00000630: 2020 2020 2020 203c 212d 2d20 5374 6172         <!-- Star
-00000640: 7420 5344 4b20 4578 616d 706c 6520 5573  t SDK Example Us
-00000650: 6167 6520 5b75 7361 6765 5d20 2d2d 3e0a  age [usage] -->.
-00000660: 2020 2020 2020 2020 2323 2053 444b 2045          ## SDK E
-00000670: 7861 6d70 6c65 2055 7361 6765 0a20 2020  xample Usage.   
-00000680: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000690: 2320 4578 616d 706c 650a 2020 2020 2020  # Example.      
-000006a0: 2020 0a20 2020 2020 2020 2060 6060 7079    .        ```py
-000006b0: 7468 6f6e 0a20 2020 2020 2020 2069 6d70  thon.        imp
-000006c0: 6f72 7420 6b65 796d 6174 6561 7069 0a20  ort keymateapi. 
-000006d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000006e0: 7320 3d20 6b65 796d 6174 6561 7069 2e4b  s = keymateapi.K
-000006f0: 6579 6d61 7465 6170 6928 0a20 2020 2020  eymateapi(.     
-00000700: 2020 2020 2020 2062 6561 7265 725f 6175         bearer_au
-00000710: 7468 3d22 3c59 4f55 525f 4245 4152 4552  th="<YOUR_BEARER
-00000720: 5f54 4f4b 454e 5f48 4552 453e 222c 0a20  _TOKEN_HERE>",. 
-00000730: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00000740: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
-00000750: 2020 2072 6573 203d 2073 2e75 7073 6572     res = s.upser
-00000760: 7428 713d 273c 7661 6c75 653e 2729 0a20  t(q='<value>'). 
-00000770: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000780: 6966 2072 6573 2e6f 626a 6563 7420 6973  if res.object is
-00000790: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000007a0: 2020 2020 2020 2023 2068 616e 646c 6520         # handle 
-000007b0: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
-000007c0: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-000007d0: 2020 0a20 2020 2020 2020 2060 6060 0a20    .        ```. 
-000007e0: 2020 2020 2020 203c 212d 2d20 456e 6420         <!-- End 
-000007f0: 5344 4b20 4578 616d 706c 6520 5573 6167  SDK Example Usag
-00000800: 6520 5b75 7361 6765 5d20 2d2d 3e0a 2020  e [usage] -->.  
-00000810: 2020 2020 2020 0a20 2020 2020 2020 203c        .        <
-00000820: 212d 2d20 5374 6172 7420 4176 6169 6c61  !-- Start Availa
-00000830: 626c 6520 5265 736f 7572 6365 7320 616e  ble Resources an
-00000840: 6420 4f70 6572 6174 696f 6e73 205b 6f70  d Operations [op
-00000850: 6572 6174 696f 6e73 5d20 2d2d 3e0a 2020  erations] -->.  
-00000860: 2020 2020 2020 2323 2041 7661 696c 6162        ## Availab
-00000870: 6c65 2052 6573 6f75 7263 6573 2061 6e64  le Resources and
-00000880: 204f 7065 7261 7469 6f6e 730a 2020 2020   Operations.    
-00000890: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
-000008a0: 205b 4b65 796d 6174 6561 7069 2053 444b   [Keymateapi SDK
-000008b0: 5d28 646f 6373 2f73 646b 732f 6b65 796d  ](docs/sdks/keym
-000008c0: 6174 6561 7069 2f52 4541 444d 452e 6d64  ateapi/README.md
-000008d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000008e0: 2020 202a 205b 7570 7365 7274 5d28 646f     * [upsert](do
-000008f0: 6373 2f73 646b 732f 6b65 796d 6174 6561  cs/sdks/keymatea
-00000900: 7069 2f52 4541 444d 452e 6d64 2375 7073  pi/README.md#ups
-00000910: 6572 7429 202d 2049 6e73 6572 7473 2072  ert) - Inserts r
-00000920: 6563 6f72 6420 746f 204b 6579 6d61 7465  ecord to Keymate
-00000930: 204d 656d 6f72 792e 0a20 2020 2020 2020   Memory..       
-00000940: 202a 205b 7175 6572 795d 2864 6f63 732f   * [query](docs/
-00000950: 7364 6b73 2f6b 6579 6d61 7465 6170 692f  sdks/keymateapi/
-00000960: 5245 4144 4d45 2e6d 6423 7175 6572 7929  README.md#query)
-00000970: 202d 2051 7565 7269 6573 2074 6865 2075   - Queries the u
-00000980: 7365 7227 7320 4b65 796d 6174 6520 4d65  ser's Keymate Me
-00000990: 6d6f 7279 2e0a 2020 2020 2020 2020 2a20  mory..        * 
-000009a0: 5b62 726f 7773 6575 726c 5d28 646f 6373  [browseurl](docs
-000009b0: 2f73 646b 732f 6b65 796d 6174 6561 7069  /sdks/keymateapi
-000009c0: 2f52 4541 444d 452e 6d64 2362 726f 7773  /README.md#brows
-000009d0: 6575 726c 2920 2d20 5468 6520 706c 7567  eurl) - The plug
-000009e0: 696e 2065 6e61 626c 6573 2075 7365 7220  in enables user 
-000009f0: 746f 2063 6f6e 6475 6374 2077 6562 2062  to conduct web b
-00000a00: 726f 7773 696e 6720 6279 2065 7874 7261  rowsing by extra
-00000a10: 6374 696e 6720 7468 6520 7465 7874 2063  cting the text c
-00000a20: 6f6e 7465 6e74 206f 6620 6120 7370 6563  ontent of a spec
-00000a30: 6966 6965 6420 5552 4c2e 2049 7420 7769  ified URL. It wi
-00000a40: 6c6c 2067 656e 6572 6174 6520 7469 746c  ll generate titl
-00000a50: 6520 616e 6420 636f 6e74 656e 742e 0a20  e and content.. 
-00000a60: 2020 2020 2020 202a 205b 6272 6f77 7365         * [browse
-00000a70: 5d28 646f 6373 2f73 646b 732f 6b65 796d  ](docs/sdks/keym
-00000a80: 6174 6561 7069 2f52 4541 444d 452e 6d64  ateapi/README.md
-00000a90: 2362 726f 7773 6529 202d 2046 6574 6368  #browse) - Fetch
-00000aa0: 2061 6e79 2055 524c 7320 7769 7468 6f75   any URLs withou
-00000ab0: 7420 7072 6f78 7920 6974 2077 6f75 6c64  t proxy it would
-00000ac0: 2070 726f 6261 626c 7920 6661 696c 206f   probably fail o
-00000ad0: 6e20 6d61 6a6f 7220 7765 6273 6974 6573  n major websites
-00000ae0: 2062 7574 2071 7569 636b 6572 2074 6861   but quicker tha
-00000af0: 6e20 6272 6f77 7365 7572 6c20 0a20 2020  n browseurl .   
-00000b00: 2020 2020 202a 205b 7365 6172 6368 5d28       * [search](
-00000b10: 646f 6373 2f73 646b 732f 6b65 796d 6174  docs/sdks/keymat
-00000b20: 6561 7069 2f52 4541 444d 452e 6d64 2373  eapi/README.md#s
-00000b30: 6561 7263 6829 202d 2057 6974 686f 7574  earch) - Without
-00000b40: 2070 726f 7869 6573 2073 6561 7263 6865   proxies searche
-00000b50: 7320 6b65 7977 6f72 6420 6f6e 2074 6865  s keyword on the
-00000b60: 2069 6e74 6572 6e65 7420 616e 6420 6665   internet and fe
-00000b70: 7463 6865 7320 7572 6c73 2061 6e64 206f  tches urls and o
-00000b80: 7074 696d 697a 6573 206f 7574 7075 740a  ptimizes output.
-00000b90: 2020 2020 2020 2020 2a20 5b75 6c74 7261          * [ultra
-00000ba0: 6661 7374 7365 6172 6368 5d28 646f 6373  fastsearch](docs
-00000bb0: 2f73 646b 732f 6b65 796d 6174 6561 7069  /sdks/keymateapi
-00000bc0: 2f52 4541 444d 452e 6d64 2375 6c74 7261  /README.md#ultra
-00000bd0: 6661 7374 7365 6172 6368 2920 2d20 5468  fastsearch) - Th
-00000be0: 6973 2070 6c75 6769 6e20 7072 6f76 6964  is plugin provid
-00000bf0: 6573 2031 3020 756c 7472 6120 6661 7374  es 10 ultra fast
-00000c00: 2073 6561 7263 6820 7265 7375 6c74 7320   search results 
-00000c10: 6672 6f6d 206d 756c 7469 706c 6520 736f  from multiple so
-00000c20: 7572 6365 7320 6769 7669 6e67 2061 206d  urces giving a m
-00000c30: 6f72 6520 636f 6d70 7265 6865 6e73 6976  ore comprehensiv
-00000c40: 6520 7669 6577 2e0a 2020 2020 2020 2020  e view..        
-00000c50: 2a20 5b67 7074 7362 726f 7773 655d 2864  * [gptsbrowse](d
-00000c60: 6f63 732f 7364 6b73 2f6b 6579 6d61 7465  ocs/sdks/keymate
-00000c70: 6170 692f 5245 4144 4d45 2e6d 6423 6770  api/README.md#gp
-00000c80: 7473 6272 6f77 7365 2920 2d20 4665 7463  tsbrowse) - Fetc
-00000c90: 6820 6d65 6d6f 7279 2e6b 6579 6d61 7465  h memory.keymate
-00000ca0: 2e61 6920 5552 4c73 0a20 2020 2020 2020  .ai URLs.       
-00000cb0: 202a 205b 696e 7465 726e 6574 7365 6172   * [internetsear
-00000cc0: 6368 5d28 646f 6373 2f73 646b 732f 6b65  ch](docs/sdks/ke
-00000cd0: 796d 6174 6561 7069 2f52 4541 444d 452e  ymateapi/README.
-00000ce0: 6d64 2369 6e74 6572 6e65 7473 6561 7263  md#internetsearc
-00000cf0: 6829 202d 2043 6f6e 6475 6374 2061 6e20  h) - Conduct an 
-00000d00: 696e 7465 726e 6574 2073 6561 7263 680a  internet search.
-00000d10: 2020 2020 2020 2020 3c21 2d2d 2045 6e64          <!-- End
-00000d20: 2041 7661 696c 6162 6c65 2052 6573 6f75   Available Resou
-00000d30: 7263 6573 2061 6e64 204f 7065 7261 7469  rces and Operati
-00000d40: 6f6e 7320 5b6f 7065 7261 7469 6f6e 735d  ons [operations]
-00000d50: 202d 2d3e 0a20 2020 2020 2020 200a 2020   -->.        .  
-00000d60: 2020 2020 2020 3c21 2d2d 2053 7461 7274        <!-- Start
-00000d70: 2045 7272 6f72 2048 616e 646c 696e 6720   Error Handling 
-00000d80: 5b65 7272 6f72 735d 202d 2d3e 0a20 2020  [errors] -->.   
-00000d90: 2020 2020 2023 2320 4572 726f 7220 4861       ## Error Ha
-00000da0: 6e64 6c69 6e67 0a20 2020 2020 2020 200a  ndling.        .
-00000db0: 2020 2020 2020 2020 4861 6e64 6c69 6e67          Handling
-00000dc0: 2065 7272 6f72 7320 696e 2074 6869 7320   errors in this 
-00000dd0: 5344 4b20 7368 6f75 6c64 206c 6172 6765  SDK should large
-00000de0: 6c79 206d 6174 6368 2079 6f75 7220 6578  ly match your ex
-00000df0: 7065 6374 6174 696f 6e73 2e20 2041 6c6c  pectations.  All
-00000e00: 206f 7065 7261 7469 6f6e 7320 7265 7475   operations retu
-00000e10: 726e 2061 2072 6573 706f 6e73 6520 6f62  rn a response ob
-00000e20: 6a65 6374 206f 7220 7261 6973 6520 616e  ject or raise an
-00000e30: 2065 7272 6f72 2e20 2049 6620 4572 726f   error.  If Erro
-00000e40: 7220 6f62 6a65 6374 7320 6172 6520 7370  r objects are sp
-00000e50: 6563 6966 6965 6420 696e 2079 6f75 7220  ecified in your 
-00000e60: 4f70 656e 4150 4920 5370 6563 2c20 7468  OpenAPI Spec, th
-00000e70: 6520 5344 4b20 7769 6c6c 2072 6169 7365  e SDK will raise
-00000e80: 2074 6865 2061 7070 726f 7072 6961 7465   the appropriate
-00000e90: 2045 7272 6f72 2074 7970 652e 0a20 2020   Error type..   
-00000ea0: 2020 2020 200a 2020 2020 2020 2020 7c20       .        | 
-00000eb0: 4572 726f 7220 4f62 6a65 6374 2020 2020  Error Object    
-00000ec0: 2020 2020 2020 2020 2020 2020 207c 2053               | S
-00000ed0: 7461 7475 7320 436f 6465 2020 2020 2020  tatus Code      
-00000ee0: 2020 2020 2020 2020 2020 2020 7c20 436f              | Co
-00000ef0: 6e74 656e 7420 5479 7065 2020 2020 2020  ntent Type      
-00000f00: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-00000f10: 2020 2020 207c 202d 2d2d 2d2d 2d2d 2d2d       | ---------
-00000f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f30: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
-00000f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f50: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d  -- | -----------
-00000f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f70: 2d20 7c0a 2020 2020 2020 2020 7c20 6572  - |.        | er
-00000f80: 726f 7273 2e42 726f 7773 6575 726c 5265  rors.BrowseurlRe
-00000f90: 7370 6f6e 7365 426f 6479 207c 2034 3030  sponseBody | 400
-00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fb0: 2020 2020 2020 2020 2020 7c20 6170 706c            | appl
-00000fc0: 6963 6174 696f 6e2f 6a73 6f6e 2020 2020  ication/json    
-00000fd0: 2020 2020 2020 2020 207c 0a20 2020 2020           |.     
-00000fe0: 2020 207c 2065 7272 6f72 732e 5344 4b45     | errors.SDKE
-00000ff0: 7272 6f72 2020 2020 2020 2020 2020 2020  rror            
-00001000: 2020 7c20 3478 2d35 7878 2020 2020 2020    | 4x-5xx      
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 207c 202a 2f2a 2020 2020 2020 2020 2020   | */*          
-00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001040: 7c0a 2020 2020 2020 2020 0a20 2020 2020  |.        .     
-00001050: 2020 2023 2323 2045 7861 6d70 6c65 0a20     ### Example. 
-00001060: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001070: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-00001080: 2020 696d 706f 7274 206b 6579 6d61 7465    import keymate
-00001090: 6170 690a 2020 2020 2020 2020 6672 6f6d  api.        from
-000010a0: 206b 6579 6d61 7465 6170 692e 6d6f 6465   keymateapi.mode
-000010b0: 6c73 2069 6d70 6f72 7420 6572 726f 7273  ls import errors
-000010c0: 2c20 6f70 6572 6174 696f 6e73 0a20 2020  , operations.   
-000010d0: 2020 2020 200a 2020 2020 2020 2020 7320       .        s 
-000010e0: 3d20 6b65 796d 6174 6561 7069 2e4b 6579  = keymateapi.Key
-000010f0: 6d61 7465 6170 6928 0a20 2020 2020 2020  mateapi(.       
-00001100: 2020 2020 2062 6561 7265 725f 6175 7468       bearer_auth
-00001110: 3d22 3c59 4f55 525f 4245 4152 4552 5f54  ="<YOUR_BEARER_T
-00001120: 4f4b 454e 5f48 4552 453e 222c 0a20 2020  OKEN_HERE>",.   
-00001130: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
-00001140: 2020 2020 2020 2020 7265 7120 3d20 6f70          req = op
-00001150: 6572 6174 696f 6e73 2e42 726f 7773 6575  erations.Browseu
-00001160: 726c 5265 7175 6573 7428 0a20 2020 2020  rlRequest(.     
-00001170: 2020 2020 2020 2069 6e70 7574 7769 6e64         inputwind
-00001180: 6f77 776f 7264 733d 273c 7661 6c75 653e  owwords='<value>
-00001190: 272c 0a20 2020 2020 2020 2020 2020 2071  ',.            q
-000011a0: 3d27 6874 7470 733a 2f2f 6167 7265 6561  ='https://agreea
-000011b0: 626c 652d 6a75 6d62 6f2e 6e65 7427 2c0a  ble-jumbo.net',.
-000011c0: 2020 2020 2020 2020 2020 2020 7065 7263              perc
-000011d0: 656e 7469 6c65 3d27 3c76 616c 7565 3e27  entile='<value>'
-000011e0: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
-000011f0: 6d6f 6670 6167 6573 3d27 3c76 616c 7565  mofpages='<value
-00001200: 3e27 2c0a 2020 2020 2020 2020 290a 2020  >',.        ).  
-00001210: 2020 2020 2020 0a20 2020 2020 2020 2072        .        r
-00001220: 6573 203d 204e 6f6e 650a 2020 2020 2020  es = None.      
-00001230: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00001240: 2020 2072 6573 203d 2073 2e62 726f 7773     res = s.brows
-00001250: 6575 726c 2872 6571 290a 2020 2020 2020  eurl(req).      
-00001260: 2020 6578 6365 7074 2065 7272 6f72 732e    except errors.
-00001270: 4272 6f77 7365 7572 6c52 6573 706f 6e73  BrowseurlRespons
-00001280: 6542 6f64 7920 6173 2065 3a0a 2020 2020  eBody as e:.    
-00001290: 2020 2020 2020 2020 2320 6861 6e64 6c65          # handle
-000012a0: 2065 7863 6570 7469 6f6e 0a20 2020 2020   exception.     
-000012b0: 2020 2020 2020 2072 6169 7365 2865 290a         raise(e).
-000012c0: 2020 2020 2020 2020 6578 6365 7074 2065          except e
-000012d0: 7272 6f72 732e 5344 4b45 7272 6f72 2061  rrors.SDKError a
-000012e0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-000012f0: 2023 2068 616e 646c 6520 6578 6365 7074   # handle except
-00001300: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00001310: 7261 6973 6528 6529 0a20 2020 2020 2020  raise(e).       
-00001320: 200a 2020 2020 2020 2020 6966 2072 6573   .        if res
-00001330: 2e74 776f 5f68 756e 6472 6564 5f61 7070  .two_hundred_app
-00001340: 6c69 6361 7469 6f6e 5f6a 736f 6e5f 6f62  lication_json_ob
-00001350: 6a65 6374 2069 7320 6e6f 7420 4e6f 6e65  ject is not None
-00001360: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00001370: 6861 6e64 6c65 2072 6573 706f 6e73 650a  handle response.
-00001380: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00001390: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000013a0: 2020 6060 600a 2020 2020 2020 2020 3c21    ```.        <!
-000013b0: 2d2d 2045 6e64 2045 7272 6f72 2048 616e  -- End Error Han
-000013c0: 646c 696e 6720 5b65 7272 6f72 735d 202d  dling [errors] -
-000013d0: 2d3e 0a20 2020 2020 2020 200a 2020 2020  ->.        .    
-000013e0: 2020 2020 3c21 2d2d 2053 7461 7274 2053      <!-- Start S
-000013f0: 6572 7665 7220 5365 6c65 6374 696f 6e20  erver Selection 
-00001400: 5b73 6572 7665 725d 202d 2d3e 0a20 2020  [server] -->.   
-00001410: 2020 2020 2023 2320 5365 7276 6572 2053       ## Server S
-00001420: 656c 6563 7469 6f6e 0a20 2020 2020 2020  election.       
-00001430: 200a 2020 2020 2020 2020 2323 2320 5365   .        ### Se
-00001440: 6c65 6374 2053 6572 7665 7220 6279 2049  lect Server by I
-00001450: 6e64 6578 0a20 2020 2020 2020 200a 2020  ndex.        .  
-00001460: 2020 2020 2020 596f 7520 6361 6e20 6f76        You can ov
-00001470: 6572 7269 6465 2074 6865 2064 6566 6175  erride the defau
-00001480: 6c74 2073 6572 7665 7220 676c 6f62 616c  lt server global
-00001490: 6c79 2062 7920 7061 7373 696e 6720 6120  ly by passing a 
-000014a0: 7365 7276 6572 2069 6e64 6578 2074 6f20  server index to 
-000014b0: 7468 6520 6073 6572 7665 725f 6964 783a  the `server_idx:
-000014c0: 2069 6e74 6020 6f70 7469 6f6e 616c 2070   int` optional p
-000014d0: 6172 616d 6574 6572 2077 6865 6e20 696e  arameter when in
-000014e0: 6974 6961 6c69 7a69 6e67 2074 6865 2053  itializing the S
-000014f0: 444b 2063 6c69 656e 7420 696e 7374 616e  DK client instan
-00001500: 6365 2e20 5468 6520 7365 6c65 6374 6564  ce. The selected
-00001510: 2073 6572 7665 7220 7769 6c6c 2074 6865   server will the
-00001520: 6e20 6265 2075 7365 6420 6173 2074 6865  n be used as the
-00001530: 2064 6566 6175 6c74 206f 6e20 7468 6520   default on the 
-00001540: 6f70 6572 6174 696f 6e73 2074 6861 7420  operations that 
-00001550: 7573 6520 6974 2e20 5468 6973 2074 6162  use it. This tab
-00001560: 6c65 206c 6973 7473 2074 6865 2069 6e64  le lists the ind
-00001570: 6578 6573 2061 7373 6f63 6961 7465 6420  exes associated 
-00001580: 7769 7468 2074 6865 2061 7661 696c 6162  with the availab
-00001590: 6c65 2073 6572 7665 7273 3a0a 2020 2020  le servers:.    
-000015a0: 2020 2020 0a20 2020 2020 2020 207c 2023      .        | #
-000015b0: 207c 2053 6572 7665 7220 7c20 5661 7269   | Server | Vari
-000015c0: 6162 6c65 7320 7c0a 2020 2020 2020 2020  ables |.        
-000015d0: 7c20 2d20 7c20 2d2d 2d2d 2d2d 207c 202d  | - | ------ | -
-000015e0: 2d2d 2d2d 2d2d 2d2d 207c 0a20 2020 2020  -------- |.     
-000015f0: 2020 207c 2030 207c 2060 6874 7470 733a     | 0 | `https:
-00001600: 2f2f 7365 7276 6572 2e73 6561 7263 6877  //server.searchw
-00001610: 6562 2e6b 6579 6d61 7465 2e61 6960 207c  eb.keymate.ai` |
-00001620: 204e 6f6e 6520 7c0a 2020 2020 2020 2020   None |.        
-00001630: 0a20 2020 2020 2020 2023 2323 2320 4578  .        #### Ex
-00001640: 616d 706c 650a 2020 2020 2020 2020 0a20  ample.        . 
-00001650: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-00001660: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00001670: 6b65 796d 6174 6561 7069 0a20 2020 2020  keymateapi.     
-00001680: 2020 200a 2020 2020 2020 2020 7320 3d20     .        s = 
-00001690: 6b65 796d 6174 6561 7069 2e4b 6579 6d61  keymateapi.Keyma
-000016a0: 7465 6170 6928 0a20 2020 2020 2020 2020  teapi(.         
-000016b0: 2020 2073 6572 7665 725f 6964 783d 302c     server_idx=0,
-000016c0: 0a20 2020 2020 2020 2020 2020 2062 6561  .            bea
-000016d0: 7265 725f 6175 7468 3d22 3c59 4f55 525f  rer_auth="<YOUR_
-000016e0: 4245 4152 4552 5f54 4f4b 454e 5f48 4552  BEARER_TOKEN_HER
-000016f0: 453e 222c 0a20 2020 2020 2020 2029 0a20  E>",.        ). 
-00001700: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001710: 0a20 2020 2020 2020 2072 6573 203d 2073  .        res = s
-00001720: 2e75 7073 6572 7428 713d 273c 7661 6c75  .upsert(q='<valu
-00001730: 653e 2729 0a20 2020 2020 2020 200a 2020  e>').        .  
-00001740: 2020 2020 2020 6966 2072 6573 2e6f 626a        if res.obj
-00001750: 6563 7420 6973 206e 6f74 204e 6f6e 653a  ect is not None:
-00001760: 0a20 2020 2020 2020 2020 2020 2023 2068  .            # h
-00001770: 616e 646c 6520 7265 7370 6f6e 7365 0a20  andle response. 
-00001780: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00001790: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000017a0: 2060 6060 0a20 2020 2020 2020 200a 2020   ```.        .  
-000017b0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000017c0: 2323 204f 7665 7272 6964 6520 5365 7276  ## Override Serv
-000017d0: 6572 2055 524c 2050 6572 2d43 6c69 656e  er URL Per-Clien
-000017e0: 740a 2020 2020 2020 2020 0a20 2020 2020  t.        .     
-000017f0: 2020 2054 6865 2064 6566 6175 6c74 2073     The default s
-00001800: 6572 7665 7220 6361 6e20 616c 736f 2062  erver can also b
-00001810: 6520 6f76 6572 7269 6464 656e 2067 6c6f  e overridden glo
-00001820: 6261 6c6c 7920 6279 2070 6173 7369 6e67  bally by passing
-00001830: 2061 2055 524c 2074 6f20 7468 6520 6073   a URL to the `s
-00001840: 6572 7665 725f 7572 6c3a 2073 7472 6020  erver_url: str` 
-00001850: 6f70 7469 6f6e 616c 2070 6172 616d 6574  optional paramet
-00001860: 6572 2077 6865 6e20 696e 6974 6961 6c69  er when initiali
-00001870: 7a69 6e67 2074 6865 2053 444b 2063 6c69  zing the SDK cli
-00001880: 656e 7420 696e 7374 616e 6365 2e20 466f  ent instance. Fo
-00001890: 7220 6578 616d 706c 653a 0a20 2020 2020  r example:.     
-000018a0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-000018b0: 2020 2020 2069 6d70 6f72 7420 6b65 796d       import keym
-000018c0: 6174 6561 7069 0a20 2020 2020 2020 200a  ateapi.        .
-000018d0: 2020 2020 2020 2020 7320 3d20 6b65 796d          s = keym
-000018e0: 6174 6561 7069 2e4b 6579 6d61 7465 6170  ateapi.Keymateap
-000018f0: 6928 0a20 2020 2020 2020 2020 2020 2073  i(.            s
-00001900: 6572 7665 725f 7572 6c3d 2268 7474 7073  erver_url="https
-00001910: 3a2f 2f73 6572 7665 722e 7365 6172 6368  ://server.search
-00001920: 7765 622e 6b65 796d 6174 652e 6169 222c  web.keymate.ai",
-00001930: 0a20 2020 2020 2020 2020 2020 2062 6561  .            bea
-00001940: 7265 725f 6175 7468 3d22 3c59 4f55 525f  rer_auth="<YOUR_
-00001950: 4245 4152 4552 5f54 4f4b 454e 5f48 4552  BEARER_TOKEN_HER
-00001960: 453e 222c 0a20 2020 2020 2020 2029 0a20  E>",.        ). 
-00001970: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001980: 0a20 2020 2020 2020 2072 6573 203d 2073  .        res = s
-00001990: 2e75 7073 6572 7428 713d 273c 7661 6c75  .upsert(q='<valu
-000019a0: 653e 2729 0a20 2020 2020 2020 200a 2020  e>').        .  
-000019b0: 2020 2020 2020 6966 2072 6573 2e6f 626a        if res.obj
-000019c0: 6563 7420 6973 206e 6f74 204e 6f6e 653a  ect is not None:
-000019d0: 0a20 2020 2020 2020 2020 2020 2023 2068  .            # h
-000019e0: 616e 646c 6520 7265 7370 6f6e 7365 0a20  andle response. 
-000019f0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00001a00: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001a10: 2060 6060 0a20 2020 2020 2020 203c 212d   ```.        <!-
-00001a20: 2d20 456e 6420 5365 7276 6572 2053 656c  - End Server Sel
-00001a30: 6563 7469 6f6e 205b 7365 7276 6572 5d20  ection [server] 
-00001a40: 2d2d 3e0a 2020 2020 2020 2020 0a20 2020  -->.        .   
-00001a50: 2020 2020 203c 212d 2d20 5374 6172 7420       <!-- Start 
-00001a60: 4375 7374 6f6d 2048 5454 5020 436c 6965  Custom HTTP Clie
-00001a70: 6e74 205b 6874 7470 2d63 6c69 656e 745d  nt [http-client]
-00001a80: 202d 2d3e 0a20 2020 2020 2020 2023 2320   -->.        ## 
-00001a90: 4375 7374 6f6d 2048 5454 5020 436c 6965  Custom HTTP Clie
-00001aa0: 6e74 0a20 2020 2020 2020 200a 2020 2020  nt.        .    
-00001ab0: 2020 2020 5468 6520 5079 7468 6f6e 2053      The Python S
-00001ac0: 444b 206d 616b 6573 2041 5049 2063 616c  DK makes API cal
-00001ad0: 6c73 2075 7369 6e67 2074 6865 205b 7265  ls using the [re
-00001ae0: 7175 6573 7473 5d28 6874 7470 733a 2f2f  quests](https://
-00001af0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00001b00: 2f72 6571 7565 7374 732f 2920 4854 5450  /requests/) HTTP
-00001b10: 206c 6962 7261 7279 2e20 2049 6e20 6f72   library.  In or
-00001b20: 6465 7220 746f 2070 726f 7669 6465 2061  der to provide a
-00001b30: 2063 6f6e 7665 6e69 656e 7420 7761 7920   convenient way 
-00001b40: 746f 2063 6f6e 6669 6775 7265 2074 696d  to configure tim
-00001b50: 656f 7574 732c 2063 6f6f 6b69 6573 2c20  eouts, cookies, 
-00001b60: 7072 6f78 6965 732c 2063 7573 746f 6d20  proxies, custom 
-00001b70: 6865 6164 6572 732c 2061 6e64 206f 7468  headers, and oth
-00001b80: 6572 206c 6f77 2d6c 6576 656c 2063 6f6e  er low-level con
-00001b90: 6669 6775 7261 7469 6f6e 2c20 796f 7520  figuration, you 
-00001ba0: 6361 6e20 696e 6974 6961 6c69 7a65 2074  can initialize t
-00001bb0: 6865 2053 444b 2063 6c69 656e 7420 7769  he SDK client wi
-00001bc0: 7468 2061 2063 7573 746f 6d20 6072 6571  th a custom `req
-00001bd0: 7565 7374 732e 5365 7373 696f 6e60 206f  uests.Session` o
-00001be0: 626a 6563 742e 0a20 2020 2020 2020 200a  bject..        .
-00001bf0: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
-00001c00: 706c 652c 2079 6f75 2063 6f75 6c64 2073  ple, you could s
-00001c10: 7065 6369 6679 2061 2068 6561 6465 7220  pecify a header 
-00001c20: 666f 7220 6576 6572 7920 7265 7175 6573  for every reques
-00001c30: 7420 7468 6174 2074 6869 7320 7364 6b20  t that this sdk 
-00001c40: 6d61 6b65 7320 6173 2066 6f6c 6c6f 7773  makes as follows
-00001c50: 3a0a 2020 2020 2020 2020 6060 6070 7974  :.        ```pyt
-00001c60: 686f 6e0a 2020 2020 2020 2020 696d 706f  hon.        impo
-00001c70: 7274 206b 6579 6d61 7465 6170 690a 2020  rt keymateapi.  
-00001c80: 2020 2020 2020 696d 706f 7274 2072 6571        import req
-00001c90: 7565 7374 730a 2020 2020 2020 2020 0a20  uests.        . 
-00001ca0: 2020 2020 2020 2068 7474 705f 636c 6965         http_clie
-00001cb0: 6e74 203d 2072 6571 7565 7374 732e 5365  nt = requests.Se
-00001cc0: 7373 696f 6e28 290a 2020 2020 2020 2020  ssion().        
-00001cd0: 6874 7470 5f63 6c69 656e 742e 6865 6164  http_client.head
-00001ce0: 6572 732e 7570 6461 7465 287b 2778 2d63  ers.update({'x-c
-00001cf0: 7573 746f 6d2d 6865 6164 6572 273a 2027  ustom-header': '
-00001d00: 736f 6d65 5661 6c75 6527 7d29 0a20 2020  someValue'}).   
-00001d10: 2020 2020 2073 203d 206b 6579 6d61 7465       s = keymate
-00001d20: 6170 692e 4b65 796d 6174 6561 7069 2863  api.Keymateapi(c
-00001d30: 6c69 656e 743a 2068 7474 705f 636c 6965  lient: http_clie
-00001d40: 6e74 290a 2020 2020 2020 2020 6060 600a  nt).        ```.
-00001d50: 2020 2020 2020 2020 3c21 2d2d 2045 6e64          <!-- End
-00001d60: 2043 7573 746f 6d20 4854 5450 2043 6c69   Custom HTTP Cli
-00001d70: 656e 7420 5b68 7474 702d 636c 6965 6e74  ent [http-client
-00001d80: 5d20 2d2d 3e0a 2020 2020 2020 2020 0a20  ] -->.        . 
-00001d90: 2020 2020 2020 203c 212d 2d20 5374 6172         <!-- Star
-00001da0: 7420 4175 7468 656e 7469 6361 7469 6f6e  t Authentication
-00001db0: 205b 7365 6375 7269 7479 5d20 2d2d 3e0a   [security] -->.
-00001dc0: 2020 2020 2020 2020 2323 2041 7574 6865          ## Authe
-00001dd0: 6e74 6963 6174 696f 6e0a 2020 2020 2020  ntication.      
-00001de0: 2020 0a20 2020 2020 2020 2023 2323 2050    .        ### P
-00001df0: 6572 2d43 6c69 656e 7420 5365 6375 7269  er-Client Securi
-00001e00: 7479 2053 6368 656d 6573 0a20 2020 2020  ty Schemes.     
-00001e10: 2020 200a 2020 2020 2020 2020 5468 6973     .        This
-00001e20: 2053 444b 2073 7570 706f 7274 7320 7468   SDK supports th
-00001e30: 6520 666f 6c6c 6f77 696e 6720 7365 6375  e following secu
-00001e40: 7269 7479 2073 6368 656d 6520 676c 6f62  rity scheme glob
-00001e50: 616c 6c79 3a0a 2020 2020 2020 2020 0a20  ally:.        . 
-00001e60: 2020 2020 2020 207c 204e 616d 6520 2020         | Name   
-00001e70: 2020 2020 2020 207c 2054 7970 6520 2020         | Type   
-00001e80: 2020 2020 2020 207c 2053 6368 656d 6520         | Scheme 
-00001e90: 2020 2020 2020 207c 0a20 2020 2020 2020         |.       
-00001ea0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
-00001eb0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
-00001ec0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
-00001ed0: 207c 0a20 2020 2020 2020 207c 2060 6265   |.        | `be
-00001ee0: 6172 6572 5f61 7574 6860 207c 2068 7474  arer_auth` | htt
-00001ef0: 7020 2020 2020 2020 2020 207c 2048 5454  p          | HTT
-00001f00: 5020 4265 6172 6572 2020 207c 0a20 2020  P Bearer   |.   
-00001f10: 2020 2020 200a 2020 2020 2020 2020 546f       .        To
-00001f20: 2061 7574 6865 6e74 6963 6174 6520 7769   authenticate wi
-00001f30: 7468 2074 6865 2041 5049 2074 6865 2060  th the API the `
-00001f40: 6265 6172 6572 5f61 7574 6860 2070 6172  bearer_auth` par
-00001f50: 616d 6574 6572 206d 7573 7420 6265 2073  ameter must be s
-00001f60: 6574 2077 6865 6e20 696e 6974 6961 6c69  et when initiali
-00001f70: 7a69 6e67 2074 6865 2053 444b 2063 6c69  zing the SDK cli
-00001f80: 656e 7420 696e 7374 616e 6365 2e20 466f  ent instance. Fo
-00001f90: 7220 6578 616d 706c 653a 0a20 2020 2020  r example:.     
-00001fa0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-00001fb0: 2020 2020 2069 6d70 6f72 7420 6b65 796d       import keym
-00001fc0: 6174 6561 7069 0a20 2020 2020 2020 200a  ateapi.        .
-00001fd0: 2020 2020 2020 2020 7320 3d20 6b65 796d          s = keym
-00001fe0: 6174 6561 7069 2e4b 6579 6d61 7465 6170  ateapi.Keymateap
-00001ff0: 6928 0a20 2020 2020 2020 2020 2020 2062  i(.            b
-00002000: 6561 7265 725f 6175 7468 3d22 3c59 4f55  earer_auth="<YOU
-00002010: 525f 4245 4152 4552 5f54 4f4b 454e 5f48  R_BEARER_TOKEN_H
-00002020: 4552 453e 222c 0a20 2020 2020 2020 2029  ERE>",.        )
-00002030: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002040: 2020 0a20 2020 2020 2020 2072 6573 203d    .        res =
-00002050: 2073 2e75 7073 6572 7428 713d 273c 7661   s.upsert(q='<va
-00002060: 6c75 653e 2729 0a20 2020 2020 2020 200a  lue>').        .
-00002070: 2020 2020 2020 2020 6966 2072 6573 2e6f          if res.o
-00002080: 626a 6563 7420 6973 206e 6f74 204e 6f6e  bject is not Non
-00002090: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-000020a0: 2068 616e 646c 6520 7265 7370 6f6e 7365   handle response
-000020b0: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-000020c0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
-000020d0: 2020 2060 6060 0a20 2020 2020 2020 203c     ```.        <
-000020e0: 212d 2d20 456e 6420 4175 7468 656e 7469  !-- End Authenti
-000020f0: 6361 7469 6f6e 205b 7365 6375 7269 7479  cation [security
-00002100: 5d20 2d2d 3e0a 2020 2020 2020 2020 0a20  ] -->.        . 
-00002110: 2020 2020 2020 203c 212d 2d20 506c 6163         <!-- Plac
-00002120: 6568 6f6c 6465 7220 666f 7220 4675 7475  eholder for Futu
-00002130: 7265 2053 7065 616b 6561 7379 2053 444b  re Speakeasy SDK
-00002140: 2053 6563 7469 6f6e 7320 2d2d 3e0a 2020   Sections -->.  
-00002150: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00002160: 2044 6576 656c 6f70 6d65 6e74 0a20 2020   Development.   
-00002170: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00002180: 204d 6174 7572 6974 790a 2020 2020 2020   Maturity.      
-00002190: 2020 0a20 2020 2020 2020 2054 6869 7320    .        This 
-000021a0: 5344 4b20 6973 2069 6e20 6265 7461 2c20  SDK is in beta, 
-000021b0: 616e 6420 7468 6572 6520 6d61 7920 6265  and there may be
-000021c0: 2062 7265 616b 696e 6720 6368 616e 6765   breaking change
-000021d0: 7320 6265 7477 6565 6e20 7665 7273 696f  s between versio
-000021e0: 6e73 2077 6974 686f 7574 2061 206d 616a  ns without a maj
-000021f0: 6f72 2076 6572 7369 6f6e 2075 7064 6174  or version updat
-00002200: 652e 2054 6865 7265 666f 7265 2c20 7765  e. Therefore, we
-00002210: 2072 6563 6f6d 6d65 6e64 2070 696e 6e69   recommend pinni
-00002220: 6e67 2075 7361 6765 0a20 2020 2020 2020  ng usage.       
-00002230: 2074 6f20 6120 7370 6563 6966 6963 2070   to a specific p
-00002240: 6163 6b61 6765 2076 6572 7369 6f6e 2e20  ackage version. 
-00002250: 5468 6973 2077 6179 2c20 796f 7520 6361  This way, you ca
-00002260: 6e20 696e 7374 616c 6c20 7468 6520 7361  n install the sa
-00002270: 6d65 2076 6572 7369 6f6e 2065 6163 6820  me version each 
-00002280: 7469 6d65 2077 6974 686f 7574 2062 7265  time without bre
-00002290: 616b 696e 6720 6368 616e 6765 7320 756e  aking changes un
-000022a0: 6c65 7373 2079 6f75 2061 7265 2069 6e74  less you are int
-000022b0: 656e 7469 6f6e 616c 6c79 0a20 2020 2020  entionally.     
-000022c0: 2020 206c 6f6f 6b69 6e67 2066 6f72 2074     looking for t
-000022d0: 6865 206c 6174 6573 7420 7665 7273 696f  he latest versio
-000022e0: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-000022f0: 2020 2020 2323 2043 6f6e 7472 6962 7574      ## Contribut
-00002300: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
-00002310: 2020 2020 2020 5768 696c 6520 7765 2076        While we v
-00002320: 616c 7565 206f 7065 6e2d 736f 7572 6365  alue open-source
-00002330: 2063 6f6e 7472 6962 7574 696f 6e73 2074   contributions t
-00002340: 6f20 7468 6973 2053 444b 2c20 7468 6973  o this SDK, this
-00002350: 206c 6962 7261 7279 2069 7320 6765 6e65   library is gene
-00002360: 7261 7465 6420 7072 6f67 7261 6d6d 6174  rated programmat
-00002370: 6963 616c 6c79 2e0a 2020 2020 2020 2020  ically..        
-00002380: 4665 656c 2066 7265 6520 746f 206f 7065  Feel free to ope
-00002390: 6e20 6120 5052 206f 7220 6120 4769 7468  n a PR or a Gith
-000023a0: 7562 2069 7373 7565 2061 7320 6120 7072  ub issue as a pr
-000023b0: 6f6f 6620 6f66 2063 6f6e 6365 7074 2061  oof of concept a
-000023c0: 6e64 2077 6527 6c6c 2064 6f20 6f75 7220  nd we'll do our 
-000023d0: 6265 7374 2074 6f20 696e 636c 7564 6520  best to include 
-000023e0: 6974 2069 6e20 6120 6675 7475 7265 2072  it in a future r
-000023f0: 656c 6561 7365 210a 2020 2020 2020 2020  elease!.        
-00002400: 0a20 2020 2020 2020 2023 2323 2053 444b  .        ### SDK
-00002410: 2043 7265 6174 6564 2062 7920 5b53 7065   Created by [Spe
-00002420: 616b 6561 7379 5d28 6874 7470 733a 2f2f  akeasy](https://
-00002430: 646f 6373 2e73 7065 616b 6561 7379 6170  docs.speakeasyap
-00002440: 692e 6465 762f 646f 6373 2f75 7369 6e67  i.dev/docs/using
-00002450: 2d73 7065 616b 6561 7379 2f63 6c69 656e  -speakeasy/clien
-00002460: 742d 7364 6b73 290a 2020 2020 2020 2020  t-sdks).        
-00002470: 0a50 6c61 7466 6f72 6d3a 2055 4e4b 4e4f  .Platform: UNKNO
-00002480: 574e 0a52 6571 7569 7265 732d 5079 7468  WN.Requires-Pyth
-00002490: 6f6e 3a20 3e3d 332e 380a 4465 7363 7269  on: >=3.8.Descri
-000024a0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-000024b0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-000024c0: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
-000024d0: 3a20 6465 760a                           : dev.
+00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
+00000080: 622e 636f 6d2f 6f7a 6775 726e 6577 2f6b  b.com/ozgurnew/k
+00000090: 6579 6d61 7465 2d70 7974 686f 6e2d 7364  eymate-python-sd
+000000a0: 6b2e 6769 740a 4175 7468 6f72 3a20 5370  k.git.Author: Sp
+000000b0: 6561 6b65 6173 790a 4c69 6365 6e73 653a  eakeasy.License:
+000000c0: 2055 4e4b 4e4f 574e 0a44 6573 6372 6970   UNKNOWN.Descrip
+000000d0: 7469 6f6e 3a20 2320 6b65 796d 6174 6561  tion: # keymatea
+000000e0: 7069 0a20 2020 2020 2020 200a 2020 2020  pi.        .    
+000000f0: 2020 2020 0a20 2020 2020 2020 203c 212d      .        <!-
+00000100: 2d20 5374 6172 7420 5344 4b20 496e 7374  - Start SDK Inst
+00000110: 616c 6c61 7469 6f6e 205b 696e 7374 616c  allation [instal
+00000120: 6c61 7469 6f6e 5d20 2d2d 3e0a 2020 2020  lation] -->.    
+00000130: 2020 2020 2323 2053 444b 2049 6e73 7461      ## SDK Insta
+00000140: 6c6c 6174 696f 6e0a 2020 2020 2020 2020  llation.        
+00000150: 0a20 2020 2020 2020 2060 6060 6261 7368  .        ```bash
+00000160: 0a20 2020 2020 2020 2070 6970 2069 6e73  .        pip ins
+00000170: 7461 6c6c 206b 6579 6d61 7465 6170 690a  tall keymateapi.
+00000180: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+00000190: 2020 2020 3c21 2d2d 2045 6e64 2053 444b      <!-- End SDK
+000001a0: 2049 6e73 7461 6c6c 6174 696f 6e20 5b69   Installation [i
+000001b0: 6e73 7461 6c6c 6174 696f 6e5d 202d 2d3e  nstallation] -->
+000001c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000001d0: 2020 3c21 2d2d 2053 7461 7274 2053 444b    <!-- Start SDK
+000001e0: 2045 7861 6d70 6c65 2055 7361 6765 205b   Example Usage [
+000001f0: 7573 6167 655d 202d 2d3e 0a20 2020 2020  usage] -->.     
+00000200: 2020 2023 2320 5344 4b20 4578 616d 706c     ## SDK Exampl
+00000210: 6520 5573 6167 650a 2020 2020 2020 2020  e Usage.        
+00000220: 0a20 2020 2020 2020 2023 2323 2045 7861  .        ### Exa
+00000230: 6d70 6c65 0a20 2020 2020 2020 200a 2020  mple.        .  
+00000240: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00000250: 2020 2020 2020 2020 696d 706f 7274 206b          import k
+00000260: 6579 6d61 7465 6170 690a 2020 2020 2020  eymateapi.      
+00000270: 2020 0a20 2020 2020 2020 2073 203d 206b    .        s = k
+00000280: 6579 6d61 7465 6170 692e 4b65 796d 6174  eymateapi.Keymat
+00000290: 6561 7069 280a 2020 2020 2020 2020 2020  eapi(.          
+000002a0: 2020 6265 6172 6572 5f61 7574 683d 223c    bearer_auth="<
+000002b0: 594f 5552 5f42 4541 5245 525f 544f 4b45  YOUR_BEARER_TOKE
+000002c0: 4e5f 4845 5245 3e22 2c0a 2020 2020 2020  N_HERE>",.      
+000002d0: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
+000002e0: 2020 2020 2072 6573 203d 2073 2e75 7073       res = s.ups
+000002f0: 6572 7428 713d 2749 2070 7265 6665 7220  ert(q='I prefer 
+00000300: 436f 7374 6120 6f76 6572 2053 7461 7262  Costa over Starb
+00000310: 7563 6b73 2e27 290a 2020 2020 2020 2020  ucks.').        
+00000320: 0a20 2020 2020 2020 2069 6620 7265 732e  .        if res.
+00000330: 6f62 6a65 6374 2069 7320 6e6f 7420 4e6f  object is not No
+00000340: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00000350: 2320 6861 6e64 6c65 2072 6573 706f 6e73  # handle respons
+00000360: 650a 2020 2020 2020 2020 2020 2020 7061  e.            pa
+00000370: 7373 0a20 2020 2020 2020 200a 2020 2020  ss.        .    
+00000380: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00000390: 3c21 2d2d 2045 6e64 2053 444b 2045 7861  <!-- End SDK Exa
+000003a0: 6d70 6c65 2055 7361 6765 205b 7573 6167  mple Usage [usag
+000003b0: 655d 202d 2d3e 0a20 2020 2020 2020 200a  e] -->.        .
+000003c0: 2020 2020 2020 2020 3c21 2d2d 2053 7461          <!-- Sta
+000003d0: 7274 2041 7661 696c 6162 6c65 2052 6573  rt Available Res
+000003e0: 6f75 7263 6573 2061 6e64 204f 7065 7261  ources and Opera
+000003f0: 7469 6f6e 7320 5b6f 7065 7261 7469 6f6e  tions [operation
+00000400: 735d 202d 2d3e 0a20 2020 2020 2020 2023  s] -->.        #
+00000410: 2320 4176 6169 6c61 626c 6520 5265 736f  # Available Reso
+00000420: 7572 6365 7320 616e 6420 4f70 6572 6174  urces and Operat
+00000430: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
+00000440: 2020 2020 2020 2323 2320 5b4b 6579 6d61        ### [Keyma
+00000450: 7465 6170 6920 5344 4b5d 2868 7474 7073  teapi SDK](https
+00000460: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f7a  ://github.com/oz
+00000470: 6775 726e 6577 2f6b 6579 6d61 7465 2d70  gurnew/keymate-p
+00000480: 7974 686f 6e2d 7364 6b2f 626c 6f62 2f6d  ython-sdk/blob/m
+00000490: 6173 7465 722f 646f 6373 2f73 646b 732f  aster/docs/sdks/
+000004a0: 6b65 796d 6174 6561 7069 2f52 4541 444d  keymateapi/READM
+000004b0: 452e 6d64 290a 2020 2020 2020 2020 0a20  E.md).        . 
+000004c0: 2020 2020 2020 202a 205b 7570 7365 7274         * [upsert
+000004d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000004e0: 2e63 6f6d 2f6f 7a67 7572 6e65 772f 6b65  .com/ozgurnew/ke
+000004f0: 796d 6174 652d 7079 7468 6f6e 2d73 646b  ymate-python-sdk
+00000500: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
+00000510: 732f 7364 6b73 2f6b 6579 6d61 7465 6170  s/sdks/keymateap
+00000520: 692f 5245 4144 4d45 2e6d 6423 7570 7365  i/README.md#upse
+00000530: 7274 2920 2d20 496e 7365 7274 7320 7265  rt) - Inserts re
+00000540: 636f 7264 2074 6f20 4b65 796d 6174 6520  cord to Keymate 
+00000550: 4d65 6d6f 7279 2e0a 2020 2020 2020 2020  Memory..        
+00000560: 2a20 5b71 7565 7279 5d28 6874 7470 733a  * [query](https:
+00000570: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7a67  //github.com/ozg
+00000580: 7572 6e65 772f 6b65 796d 6174 652d 7079  urnew/keymate-py
+00000590: 7468 6f6e 2d73 646b 2f62 6c6f 622f 6d61  thon-sdk/blob/ma
+000005a0: 7374 6572 2f64 6f63 732f 7364 6b73 2f6b  ster/docs/sdks/k
+000005b0: 6579 6d61 7465 6170 692f 5245 4144 4d45  eymateapi/README
+000005c0: 2e6d 6423 7175 6572 7929 202d 2051 7565  .md#query) - Que
+000005d0: 7269 6573 2074 6865 2075 7365 7227 7320  ries the user's 
+000005e0: 4b65 796d 6174 6520 4d65 6d6f 7279 2e0a  Keymate Memory..
+000005f0: 2020 2020 2020 2020 2a20 5b62 726f 7773          * [brows
+00000600: 6575 726c 5d28 6874 7470 733a 2f2f 6769  eurl](https://gi
+00000610: 7468 7562 2e63 6f6d 2f6f 7a67 7572 6e65  thub.com/ozgurne
+00000620: 772f 6b65 796d 6174 652d 7079 7468 6f6e  w/keymate-python
+00000630: 2d73 646b 2f62 6c6f 622f 6d61 7374 6572  -sdk/blob/master
+00000640: 2f64 6f63 732f 7364 6b73 2f6b 6579 6d61  /docs/sdks/keyma
+00000650: 7465 6170 692f 5245 4144 4d45 2e6d 6423  teapi/README.md#
+00000660: 6272 6f77 7365 7572 6c29 202d 2054 6865  browseurl) - The
+00000670: 2070 6c75 6769 6e20 656e 6162 6c65 7320   plugin enables 
+00000680: 7573 6572 2074 6f20 636f 6e64 7563 7420  user to conduct 
+00000690: 7765 6220 6272 6f77 7369 6e67 2062 7920  web browsing by 
+000006a0: 6578 7472 6163 7469 6e67 2074 6865 2074  extracting the t
+000006b0: 6578 7420 636f 6e74 656e 7420 6f66 2061  ext content of a
+000006c0: 2073 7065 6369 6669 6564 2055 524c 2e20   specified URL. 
+000006d0: 4974 2077 696c 6c20 6765 6e65 7261 7465  It will generate
+000006e0: 2074 6974 6c65 2061 6e64 2063 6f6e 7465   title and conte
+000006f0: 6e74 2e0a 2020 2020 2020 2020 2a20 5b62  nt..        * [b
+00000700: 726f 7773 655d 2868 7474 7073 3a2f 2f67  rowse](https://g
+00000710: 6974 6875 622e 636f 6d2f 6f7a 6775 726e  ithub.com/ozgurn
+00000720: 6577 2f6b 6579 6d61 7465 2d70 7974 686f  ew/keymate-pytho
+00000730: 6e2d 7364 6b2f 626c 6f62 2f6d 6173 7465  n-sdk/blob/maste
+00000740: 722f 646f 6373 2f73 646b 732f 6b65 796d  r/docs/sdks/keym
+00000750: 6174 6561 7069 2f52 4541 444d 452e 6d64  ateapi/README.md
+00000760: 2362 726f 7773 6529 202d 2046 6574 6368  #browse) - Fetch
+00000770: 2061 6e79 2055 524c 7320 7769 7468 6f75   any URLs withou
+00000780: 7420 7072 6f78 7920 6974 2077 6f75 6c64  t proxy it would
+00000790: 2070 726f 6261 626c 7920 6661 696c 206f   probably fail o
+000007a0: 6e20 6d61 6a6f 7220 7765 6273 6974 6573  n major websites
+000007b0: 2062 7574 2071 7569 636b 6572 2074 6861   but quicker tha
+000007c0: 6e20 6272 6f77 7365 7572 6c20 0a20 2020  n browseurl .   
+000007d0: 2020 2020 202a 205b 7365 6172 6368 5d28       * [search](
+000007e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000007f0: 6f6d 2f6f 7a67 7572 6e65 772f 6b65 796d  om/ozgurnew/keym
+00000800: 6174 652d 7079 7468 6f6e 2d73 646b 2f62  ate-python-sdk/b
+00000810: 6c6f 622f 6d61 7374 6572 2f64 6f63 732f  lob/master/docs/
+00000820: 7364 6b73 2f6b 6579 6d61 7465 6170 692f  sdks/keymateapi/
+00000830: 5245 4144 4d45 2e6d 6423 7365 6172 6368  README.md#search
+00000840: 2920 2d20 5769 7468 6f75 7420 7072 6f78  ) - Without prox
+00000850: 6965 7320 7365 6172 6368 6573 206b 6579  ies searches key
+00000860: 776f 7264 206f 6e20 7468 6520 696e 7465  word on the inte
+00000870: 726e 6574 2061 6e64 2066 6574 6368 6573  rnet and fetches
+00000880: 2075 726c 7320 616e 6420 6f70 7469 6d69   urls and optimi
+00000890: 7a65 7320 6f75 7470 7574 0a20 2020 2020  zes output.     
+000008a0: 2020 202a 205b 756c 7472 6166 6173 7473     * [ultrafasts
+000008b0: 6561 7263 685d 2868 7474 7073 3a2f 2f67  earch](https://g
+000008c0: 6974 6875 622e 636f 6d2f 6f7a 6775 726e  ithub.com/ozgurn
+000008d0: 6577 2f6b 6579 6d61 7465 2d70 7974 686f  ew/keymate-pytho
+000008e0: 6e2d 7364 6b2f 626c 6f62 2f6d 6173 7465  n-sdk/blob/maste
+000008f0: 722f 646f 6373 2f73 646b 732f 6b65 796d  r/docs/sdks/keym
+00000900: 6174 6561 7069 2f52 4541 444d 452e 6d64  ateapi/README.md
+00000910: 2375 6c74 7261 6661 7374 7365 6172 6368  #ultrafastsearch
+00000920: 2920 2d20 5468 6973 2070 6c75 6769 6e20  ) - This plugin 
+00000930: 7072 6f76 6964 6573 2031 3020 756c 7472  provides 10 ultr
+00000940: 6120 6661 7374 2073 6561 7263 6820 7265  a fast search re
+00000950: 7375 6c74 7320 6672 6f6d 206d 756c 7469  sults from multi
+00000960: 706c 6520 736f 7572 6365 7320 6769 7669  ple sources givi
+00000970: 6e67 2061 206d 6f72 6520 636f 6d70 7265  ng a more compre
+00000980: 6865 6e73 6976 6520 7669 6577 2e0a 2020  hensive view..  
+00000990: 2020 2020 2020 2a20 5b67 7074 7362 726f        * [gptsbro
+000009a0: 7773 655d 2868 7474 7073 3a2f 2f67 6974  wse](https://git
+000009b0: 6875 622e 636f 6d2f 6f7a 6775 726e 6577  hub.com/ozgurnew
+000009c0: 2f6b 6579 6d61 7465 2d70 7974 686f 6e2d  /keymate-python-
+000009d0: 7364 6b2f 626c 6f62 2f6d 6173 7465 722f  sdk/blob/master/
+000009e0: 646f 6373 2f73 646b 732f 6b65 796d 6174  docs/sdks/keymat
+000009f0: 6561 7069 2f52 4541 444d 452e 6d64 2367  eapi/README.md#g
+00000a00: 7074 7362 726f 7773 6529 202d 2046 6574  ptsbrowse) - Fet
+00000a10: 6368 206d 656d 6f72 792e 6b65 796d 6174  ch memory.keymat
+00000a20: 652e 6169 2055 524c 730a 2020 2020 2020  e.ai URLs.      
+00000a30: 2020 2a20 5b69 6e74 6572 6e65 7473 6561    * [internetsea
+00000a40: 7263 685d 2868 7474 7073 3a2f 2f67 6974  rch](https://git
+00000a50: 6875 622e 636f 6d2f 6f7a 6775 726e 6577  hub.com/ozgurnew
+00000a60: 2f6b 6579 6d61 7465 2d70 7974 686f 6e2d  /keymate-python-
+00000a70: 7364 6b2f 626c 6f62 2f6d 6173 7465 722f  sdk/blob/master/
+00000a80: 646f 6373 2f73 646b 732f 6b65 796d 6174  docs/sdks/keymat
+00000a90: 6561 7069 2f52 4541 444d 452e 6d64 2369  eapi/README.md#i
+00000aa0: 6e74 6572 6e65 7473 6561 7263 6829 202d  nternetsearch) -
+00000ab0: 2043 6f6e 6475 6374 2061 6e20 696e 7465   Conduct an inte
+00000ac0: 726e 6574 2073 6561 7263 680a 2020 2020  rnet search.    
+00000ad0: 2020 2020 3c21 2d2d 2045 6e64 2041 7661      <!-- End Ava
+00000ae0: 696c 6162 6c65 2052 6573 6f75 7263 6573  ilable Resources
+00000af0: 2061 6e64 204f 7065 7261 7469 6f6e 7320   and Operations 
+00000b00: 5b6f 7065 7261 7469 6f6e 735d 202d 2d3e  [operations] -->
+00000b10: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000b20: 2020 3c21 2d2d 2053 7461 7274 2045 7272    <!-- Start Err
+00000b30: 6f72 2048 616e 646c 696e 6720 5b65 7272  or Handling [err
+00000b40: 6f72 735d 202d 2d3e 0a20 2020 2020 2020  ors] -->.       
+00000b50: 2023 2320 4572 726f 7220 4861 6e64 6c69   ## Error Handli
+00000b60: 6e67 0a20 2020 2020 2020 200a 2020 2020  ng.        .    
+00000b70: 2020 2020 4861 6e64 6c69 6e67 2065 7272      Handling err
+00000b80: 6f72 7320 696e 2074 6869 7320 5344 4b20  ors in this SDK 
+00000b90: 7368 6f75 6c64 206c 6172 6765 6c79 206d  should largely m
+00000ba0: 6174 6368 2079 6f75 7220 6578 7065 6374  atch your expect
+00000bb0: 6174 696f 6e73 2e20 2041 6c6c 206f 7065  ations.  All ope
+00000bc0: 7261 7469 6f6e 7320 7265 7475 726e 2061  rations return a
+00000bd0: 2072 6573 706f 6e73 6520 6f62 6a65 6374   response object
+00000be0: 206f 7220 7261 6973 6520 616e 2065 7272   or raise an err
+00000bf0: 6f72 2e20 2049 6620 4572 726f 7220 6f62  or.  If Error ob
+00000c00: 6a65 6374 7320 6172 6520 7370 6563 6966  jects are specif
+00000c10: 6965 6420 696e 2079 6f75 7220 4f70 656e  ied in your Open
+00000c20: 4150 4920 5370 6563 2c20 7468 6520 5344  API Spec, the SD
+00000c30: 4b20 7769 6c6c 2072 6169 7365 2074 6865  K will raise the
+00000c40: 2061 7070 726f 7072 6961 7465 2045 7272   appropriate Err
+00000c50: 6f72 2074 7970 652e 0a20 2020 2020 2020  or type..       
+00000c60: 200a 2020 2020 2020 2020 7c20 4572 726f   .        | Erro
+00000c70: 7220 4f62 6a65 6374 2020 2020 2020 2020  r Object        
+00000c80: 2020 2020 2020 2020 207c 2053 7461 7475           | Statu
+00000c90: 7320 436f 6465 2020 2020 2020 2020 2020  s Code          
+00000ca0: 2020 2020 2020 2020 7c20 436f 6e74 656e          | Conten
+00000cb0: 7420 5479 7065 2020 2020 2020 2020 2020  t Type          
+00000cc0: 2020 2020 2020 207c 0a20 2020 2020 2020         |.       
+00000cd0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00000ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
+00000cf0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
+00000d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+00000d10: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00000d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0a  ------------- |.
+00000d30: 2020 2020 2020 2020 7c20 6572 726f 7273          | errors
+00000d40: 2e42 726f 7773 6575 726c 5265 7370 6f6e  .BrowseurlRespon
+00000d50: 7365 426f 6479 207c 2034 3030 2020 2020  seBody | 400    
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 2020 2020 2020 7c20 6170 706c 6963 6174        | applicat
+00000d80: 696f 6e2f 6a73 6f6e 2020 2020 2020 2020  ion/json        
+00000d90: 2020 2020 207c 0a20 2020 2020 2020 207c       |.        |
+00000da0: 2065 7272 6f72 732e 5344 4b45 7272 6f72   errors.SDKError
+00000db0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00000dc0: 3478 782d 3578 7820 2020 2020 2020 2020  4xx-5xx         
+00000dd0: 2020 2020 2020 2020 2020 2020 207c 202a               | *
+00000de0: 2f2a 2020 2020 2020 2020 2020 2020 2020  /*              
+00000df0: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
+00000e00: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00000e10: 2323 2045 7861 6d70 6c65 0a20 2020 2020  ## Example.     
+00000e20: 2020 200a 2020 2020 2020 2020 6060 6070     .        ```p
+00000e30: 7974 686f 6e0a 2020 2020 2020 2020 696d  ython.        im
+00000e40: 706f 7274 206b 6579 6d61 7465 6170 690a  port keymateapi.
+00000e50: 2020 2020 2020 2020 6672 6f6d 206b 6579          from key
+00000e60: 6d61 7465 6170 692e 6d6f 6465 6c73 2069  mateapi.models i
+00000e70: 6d70 6f72 7420 6572 726f 7273 2c20 6f70  mport errors, op
+00000e80: 6572 6174 696f 6e73 0a20 2020 2020 2020  erations.       
+00000e90: 200a 2020 2020 2020 2020 7320 3d20 6b65   .        s = ke
+00000ea0: 796d 6174 6561 7069 2e4b 6579 6d61 7465  ymateapi.Keymate
+00000eb0: 6170 6928 0a20 2020 2020 2020 2020 2020  api(.           
+00000ec0: 2062 6561 7265 725f 6175 7468 3d22 3c59   bearer_auth="<Y
+00000ed0: 4f55 525f 4245 4152 4552 5f54 4f4b 454e  OUR_BEARER_TOKEN
+00000ee0: 5f48 4552 453e 222c 0a20 2020 2020 2020  _HERE>",.       
+00000ef0: 2029 0a20 2020 2020 2020 200a 2020 2020   ).        .    
+00000f00: 2020 2020 7265 7320 3d20 4e6f 6e65 0a20      res = None. 
+00000f10: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00000f20: 2020 2020 2020 2020 7265 7320 3d20 732e          res = s.
+00000f30: 6272 6f77 7365 7572 6c28 7265 7175 6573  browseurl(reques
+00000f40: 743d 6f70 6572 6174 696f 6e73 2e42 726f  t=operations.Bro
+00000f50: 7773 6575 726c 5265 7175 6573 7428 0a20  wseurlRequest(. 
+00000f60: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00000f70: 7769 6e64 6f77 776f 7264 733d 2731 3030  windowwords='100
+00000f80: 3030 272c 0a20 2020 2020 2020 2020 2020  00',.           
+00000f90: 2071 3d27 6874 7470 733a 2f2f 6b65 796d   q='https://keym
+00000fa0: 6174 652e 6169 272c 0a20 2020 2020 2020  ate.ai',.       
+00000fb0: 2020 2020 2070 6572 6365 6e74 696c 653d       percentile=
+00000fc0: 2731 272c 0a20 2020 2020 2020 2020 2020  '1',.           
+00000fd0: 206e 756d 6f66 7061 6765 733d 2731 272c   numofpages='1',
+00000fe0: 0a20 2020 2020 2020 2020 2020 2070 6167  .            pag
+00000ff0: 696e 673d 2731 272c 0a20 2020 2020 2020  ing='1',.       
+00001000: 2029 290a 2020 2020 2020 2020 6578 6365   )).        exce
+00001010: 7074 2065 7272 6f72 732e 4272 6f77 7365  pt errors.Browse
+00001020: 7572 6c52 6573 706f 6e73 6542 6f64 7920  urlResponseBody 
+00001030: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00001040: 2020 2320 6861 6e64 6c65 2065 7863 6570    # handle excep
+00001050: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00001060: 2072 6169 7365 2865 290a 2020 2020 2020   raise(e).      
+00001070: 2020 6578 6365 7074 2065 7272 6f72 732e    except errors.
+00001080: 5344 4b45 7272 6f72 2061 7320 653a 0a20  SDKError as e:. 
+00001090: 2020 2020 2020 2020 2020 2023 2068 616e             # han
+000010a0: 646c 6520 6578 6365 7074 696f 6e0a 2020  dle exception.  
+000010b0: 2020 2020 2020 2020 2020 7261 6973 6528            raise(
+000010c0: 6529 0a20 2020 2020 2020 200a 2020 2020  e).        .    
+000010d0: 2020 2020 6966 2072 6573 2e74 776f 5f68      if res.two_h
+000010e0: 756e 6472 6564 5f61 7070 6c69 6361 7469  undred_applicati
+000010f0: 6f6e 5f6a 736f 6e5f 6f62 6a65 6374 2069  on_json_object i
+00001100: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00001110: 2020 2020 2020 2020 2320 6861 6e64 6c65          # handle
+00001120: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+00001130: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00001140: 2020 200a 2020 2020 2020 2020 6060 600a     .        ```.
+00001150: 2020 2020 2020 2020 3c21 2d2d 2045 6e64          <!-- End
+00001160: 2045 7272 6f72 2048 616e 646c 696e 6720   Error Handling 
+00001170: 5b65 7272 6f72 735d 202d 2d3e 0a20 2020  [errors] -->.   
+00001180: 2020 2020 200a 2020 2020 2020 2020 3c21       .        <!
+00001190: 2d2d 2053 7461 7274 2053 6572 7665 7220  -- Start Server 
+000011a0: 5365 6c65 6374 696f 6e20 5b73 6572 7665  Selection [serve
+000011b0: 725d 202d 2d3e 0a20 2020 2020 2020 2023  r] -->.        #
+000011c0: 2320 5365 7276 6572 2053 656c 6563 7469  # Server Selecti
+000011d0: 6f6e 0a20 2020 2020 2020 200a 2020 2020  on.        .    
+000011e0: 2020 2020 2323 2320 5365 6c65 6374 2053      ### Select S
+000011f0: 6572 7665 7220 6279 2049 6e64 6578 0a20  erver by Index. 
+00001200: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001210: 596f 7520 6361 6e20 6f76 6572 7269 6465  You can override
+00001220: 2074 6865 2064 6566 6175 6c74 2073 6572   the default ser
+00001230: 7665 7220 676c 6f62 616c 6c79 2062 7920  ver globally by 
+00001240: 7061 7373 696e 6720 6120 7365 7276 6572  passing a server
+00001250: 2069 6e64 6578 2074 6f20 7468 6520 6073   index to the `s
+00001260: 6572 7665 725f 6964 783a 2069 6e74 6020  erver_idx: int` 
+00001270: 6f70 7469 6f6e 616c 2070 6172 616d 6574  optional paramet
+00001280: 6572 2077 6865 6e20 696e 6974 6961 6c69  er when initiali
+00001290: 7a69 6e67 2074 6865 2053 444b 2063 6c69  zing the SDK cli
+000012a0: 656e 7420 696e 7374 616e 6365 2e20 5468  ent instance. Th
+000012b0: 6520 7365 6c65 6374 6564 2073 6572 7665  e selected serve
+000012c0: 7220 7769 6c6c 2074 6865 6e20 6265 2075  r will then be u
+000012d0: 7365 6420 6173 2074 6865 2064 6566 6175  sed as the defau
+000012e0: 6c74 206f 6e20 7468 6520 6f70 6572 6174  lt on the operat
+000012f0: 696f 6e73 2074 6861 7420 7573 6520 6974  ions that use it
+00001300: 2e20 5468 6973 2074 6162 6c65 206c 6973  . This table lis
+00001310: 7473 2074 6865 2069 6e64 6578 6573 2061  ts the indexes a
+00001320: 7373 6f63 6961 7465 6420 7769 7468 2074  ssociated with t
+00001330: 6865 2061 7661 696c 6162 6c65 2073 6572  he available ser
+00001340: 7665 7273 3a0a 2020 2020 2020 2020 0a20  vers:.        . 
+00001350: 2020 2020 2020 207c 2023 207c 2053 6572         | # | Ser
+00001360: 7665 7220 7c20 5661 7269 6162 6c65 7320  ver | Variables 
+00001370: 7c0a 2020 2020 2020 2020 7c20 2d20 7c20  |.        | - | 
+00001380: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00001390: 2d2d 207c 0a20 2020 2020 2020 207c 2030  -- |.        | 0
+000013a0: 207c 2060 6874 7470 733a 2f2f 7365 7276   | `https://serv
+000013b0: 6572 2e73 6561 7263 6877 6562 2e6b 6579  er.searchweb.key
+000013c0: 6d61 7465 2e61 6960 207c 204e 6f6e 6520  mate.ai` | None 
+000013d0: 7c0a 2020 2020 2020 2020 0a20 2020 2020  |.        .     
+000013e0: 2020 2023 2323 2320 4578 616d 706c 650a     #### Example.
+000013f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001400: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+00001410: 2020 2069 6d70 6f72 7420 6b65 796d 6174     import keymat
+00001420: 6561 7069 0a20 2020 2020 2020 200a 2020  eapi.        .  
+00001430: 2020 2020 2020 7320 3d20 6b65 796d 6174        s = keymat
+00001440: 6561 7069 2e4b 6579 6d61 7465 6170 6928  eapi.Keymateapi(
+00001450: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+00001460: 7665 725f 6964 783d 302c 0a20 2020 2020  ver_idx=0,.     
+00001470: 2020 2020 2020 2062 6561 7265 725f 6175         bearer_au
+00001480: 7468 3d22 3c59 4f55 525f 4245 4152 4552  th="<YOUR_BEARER
+00001490: 5f54 4f4b 454e 5f48 4552 453e 222c 0a20  _TOKEN_HERE>",. 
+000014a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000014b0: 200a 2020 2020 2020 2020 7265 7320 3d20   .        res = 
+000014c0: 732e 7570 7365 7274 2871 3d27 4920 7072  s.upsert(q='I pr
+000014d0: 6566 6572 2043 6f73 7461 206f 7665 7220  efer Costa over 
+000014e0: 5374 6172 6275 636b 732e 2729 0a20 2020  Starbucks.').   
+000014f0: 2020 2020 200a 2020 2020 2020 2020 6966       .        if
+00001500: 2072 6573 2e6f 626a 6563 7420 6973 206e   res.object is n
+00001510: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00001520: 2020 2020 2023 2068 616e 646c 6520 7265       # handle re
+00001530: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
+00001540: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+00001550: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+00001560: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+00001570: 2020 2020 2020 2023 2323 204f 7665 7272         ### Overr
+00001580: 6964 6520 5365 7276 6572 2055 524c 2050  ide Server URL P
+00001590: 6572 2d43 6c69 656e 740a 2020 2020 2020  er-Client.      
+000015a0: 2020 0a20 2020 2020 2020 2054 6865 2064    .        The d
+000015b0: 6566 6175 6c74 2073 6572 7665 7220 6361  efault server ca
+000015c0: 6e20 616c 736f 2062 6520 6f76 6572 7269  n also be overri
+000015d0: 6464 656e 2067 6c6f 6261 6c6c 7920 6279  dden globally by
+000015e0: 2070 6173 7369 6e67 2061 2055 524c 2074   passing a URL t
+000015f0: 6f20 7468 6520 6073 6572 7665 725f 7572  o the `server_ur
+00001600: 6c3a 2073 7472 6020 6f70 7469 6f6e 616c  l: str` optional
+00001610: 2070 6172 616d 6574 6572 2077 6865 6e20   parameter when 
+00001620: 696e 6974 6961 6c69 7a69 6e67 2074 6865  initializing the
+00001630: 2053 444b 2063 6c69 656e 7420 696e 7374   SDK client inst
+00001640: 616e 6365 2e20 466f 7220 6578 616d 706c  ance. For exampl
+00001650: 653a 0a20 2020 2020 2020 2060 6060 7079  e:.        ```py
+00001660: 7468 6f6e 0a20 2020 2020 2020 2069 6d70  thon.        imp
+00001670: 6f72 7420 6b65 796d 6174 6561 7069 0a20  ort keymateapi. 
+00001680: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001690: 7320 3d20 6b65 796d 6174 6561 7069 2e4b  s = keymateapi.K
+000016a0: 6579 6d61 7465 6170 6928 0a20 2020 2020  eymateapi(.     
+000016b0: 2020 2020 2020 2073 6572 7665 725f 7572         server_ur
+000016c0: 6c3d 2268 7474 7073 3a2f 2f73 6572 7665  l="https://serve
+000016d0: 722e 7365 6172 6368 7765 622e 6b65 796d  r.searchweb.keym
+000016e0: 6174 652e 6169 222c 0a20 2020 2020 2020  ate.ai",.       
+000016f0: 2020 2020 2062 6561 7265 725f 6175 7468       bearer_auth
+00001700: 3d22 3c59 4f55 525f 4245 4152 4552 5f54  ="<YOUR_BEARER_T
+00001710: 4f4b 454e 5f48 4552 453e 222c 0a20 2020  OKEN_HERE>",.   
+00001720: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
+00001730: 2020 2020 2020 2020 7265 7320 3d20 732e          res = s.
+00001740: 7570 7365 7274 2871 3d27 4920 7072 6566  upsert(q='I pref
+00001750: 6572 2043 6f73 7461 206f 7665 7220 5374  er Costa over St
+00001760: 6172 6275 636b 732e 2729 0a20 2020 2020  arbucks.').     
+00001770: 2020 200a 2020 2020 2020 2020 6966 2072     .        if r
+00001780: 6573 2e6f 626a 6563 7420 6973 206e 6f74  es.object is not
+00001790: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000017a0: 2020 2023 2068 616e 646c 6520 7265 7370     # handle resp
+000017b0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
+000017c0: 2070 6173 730a 2020 2020 2020 2020 0a20   pass.        . 
+000017d0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+000017e0: 2020 203c 212d 2d20 456e 6420 5365 7276     <!-- End Serv
+000017f0: 6572 2053 656c 6563 7469 6f6e 205b 7365  er Selection [se
+00001800: 7276 6572 5d20 2d2d 3e0a 2020 2020 2020  rver] -->.      
+00001810: 2020 0a20 2020 2020 2020 203c 212d 2d20    .        <!-- 
+00001820: 5374 6172 7420 4375 7374 6f6d 2048 5454  Start Custom HTT
+00001830: 5020 436c 6965 6e74 205b 6874 7470 2d63  P Client [http-c
+00001840: 6c69 656e 745d 202d 2d3e 0a20 2020 2020  lient] -->.     
+00001850: 2020 2023 2320 4375 7374 6f6d 2048 5454     ## Custom HTT
+00001860: 5020 436c 6965 6e74 0a20 2020 2020 2020  P Client.       
+00001870: 200a 2020 2020 2020 2020 5468 6520 5079   .        The Py
+00001880: 7468 6f6e 2053 444b 206d 616b 6573 2041  thon SDK makes A
+00001890: 5049 2063 616c 6c73 2075 7369 6e67 2074  PI calls using t
+000018a0: 6865 205b 7265 7175 6573 7473 5d28 6874  he [requests](ht
+000018b0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000018c0: 726f 6a65 6374 2f72 6571 7565 7374 732f  roject/requests/
+000018d0: 2920 4854 5450 206c 6962 7261 7279 2e20  ) HTTP library. 
+000018e0: 2049 6e20 6f72 6465 7220 746f 2070 726f   In order to pro
+000018f0: 7669 6465 2061 2063 6f6e 7665 6e69 656e  vide a convenien
+00001900: 7420 7761 7920 746f 2063 6f6e 6669 6775  t way to configu
+00001910: 7265 2074 696d 656f 7574 732c 2063 6f6f  re timeouts, coo
+00001920: 6b69 6573 2c20 7072 6f78 6965 732c 2063  kies, proxies, c
+00001930: 7573 746f 6d20 6865 6164 6572 732c 2061  ustom headers, a
+00001940: 6e64 206f 7468 6572 206c 6f77 2d6c 6576  nd other low-lev
+00001950: 656c 2063 6f6e 6669 6775 7261 7469 6f6e  el configuration
+00001960: 2c20 796f 7520 6361 6e20 696e 6974 6961  , you can initia
+00001970: 6c69 7a65 2074 6865 2053 444b 2063 6c69  lize the SDK cli
+00001980: 656e 7420 7769 7468 2061 2063 7573 746f  ent with a custo
+00001990: 6d20 6072 6571 7565 7374 732e 5365 7373  m `requests.Sess
+000019a0: 696f 6e60 206f 626a 6563 742e 0a20 2020  ion` object..   
+000019b0: 2020 2020 200a 2020 2020 2020 2020 466f       .        Fo
+000019c0: 7220 6578 616d 706c 652c 2079 6f75 2063  r example, you c
+000019d0: 6f75 6c64 2073 7065 6369 6679 2061 2068  ould specify a h
+000019e0: 6561 6465 7220 666f 7220 6576 6572 7920  eader for every 
+000019f0: 7265 7175 6573 7420 7468 6174 2074 6869  request that thi
+00001a00: 7320 7364 6b20 6d61 6b65 7320 6173 2066  s sdk makes as f
+00001a10: 6f6c 6c6f 7773 3a0a 2020 2020 2020 2020  ollows:.        
+00001a20: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+00001a30: 2020 696d 706f 7274 206b 6579 6d61 7465    import keymate
+00001a40: 6170 690a 2020 2020 2020 2020 696d 706f  api.        impo
+00001a50: 7274 2072 6571 7565 7374 730a 2020 2020  rt requests.    
+00001a60: 2020 2020 0a20 2020 2020 2020 2068 7474      .        htt
+00001a70: 705f 636c 6965 6e74 203d 2072 6571 7565  p_client = reque
+00001a80: 7374 732e 5365 7373 696f 6e28 290a 2020  sts.Session().  
+00001a90: 2020 2020 2020 6874 7470 5f63 6c69 656e        http_clien
+00001aa0: 742e 6865 6164 6572 732e 7570 6461 7465  t.headers.update
+00001ab0: 287b 2778 2d63 7573 746f 6d2d 6865 6164  ({'x-custom-head
+00001ac0: 6572 273a 2027 736f 6d65 5661 6c75 6527  er': 'someValue'
+00001ad0: 7d29 0a20 2020 2020 2020 2073 203d 206b  }).        s = k
+00001ae0: 6579 6d61 7465 6170 692e 4b65 796d 6174  eymateapi.Keymat
+00001af0: 6561 7069 2863 6c69 656e 743d 6874 7470  eapi(client=http
+00001b00: 5f63 6c69 656e 7429 0a20 2020 2020 2020  _client).       
+00001b10: 2060 6060 0a20 2020 2020 2020 203c 212d   ```.        <!-
+00001b20: 2d20 456e 6420 4375 7374 6f6d 2048 5454  - End Custom HTT
+00001b30: 5020 436c 6965 6e74 205b 6874 7470 2d63  P Client [http-c
+00001b40: 6c69 656e 745d 202d 2d3e 0a20 2020 2020  lient] -->.     
+00001b50: 2020 200a 2020 2020 2020 2020 3c21 2d2d     .        <!--
+00001b60: 2053 7461 7274 2041 7574 6865 6e74 6963   Start Authentic
+00001b70: 6174 696f 6e20 5b73 6563 7572 6974 795d  ation [security]
+00001b80: 202d 2d3e 0a20 2020 2020 2020 2023 2320   -->.        ## 
+00001b90: 4175 7468 656e 7469 6361 7469 6f6e 0a20  Authentication. 
+00001ba0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001bb0: 2323 2320 5065 722d 436c 6965 6e74 2053  ### Per-Client S
+00001bc0: 6563 7572 6974 7920 5363 6865 6d65 730a  ecurity Schemes.
+00001bd0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001be0: 2054 6869 7320 5344 4b20 7375 7070 6f72   This SDK suppor
+00001bf0: 7473 2074 6865 2066 6f6c 6c6f 7769 6e67  ts the following
+00001c00: 2073 6563 7572 6974 7920 7363 6865 6d65   security scheme
+00001c10: 2067 6c6f 6261 6c6c 793a 0a20 2020 2020   globally:.     
+00001c20: 2020 200a 2020 2020 2020 2020 7c20 4e61     .        | Na
+00001c30: 6d65 2020 2020 2020 2020 2020 7c20 5479  me          | Ty
+00001c40: 7065 2020 2020 2020 2020 2020 7c20 5363  pe          | Sc
+00001c50: 6865 6d65 2020 2020 2020 2020 7c0a 2020  heme        |.  
+00001c60: 2020 2020 2020 7c20 2d2d 2d2d 2d2d 2d2d        | --------
+00001c70: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+00001c80: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+00001c90: 2d2d 2d2d 2d20 7c0a 2020 2020 2020 2020  ----- |.        
+00001ca0: 7c20 6062 6561 7265 725f 6175 7468 6020  | `bearer_auth` 
+00001cb0: 7c20 6874 7470 2020 2020 2020 2020 2020  | http          
+00001cc0: 7c20 4854 5450 2042 6561 7265 7220 2020  | HTTP Bearer   
+00001cd0: 7c0a 2020 2020 2020 2020 0a20 2020 2020  |.        .     
+00001ce0: 2020 2054 6f20 6175 7468 656e 7469 6361     To authentica
+00001cf0: 7465 2077 6974 6820 7468 6520 4150 4920  te with the API 
+00001d00: 7468 6520 6062 6561 7265 725f 6175 7468  the `bearer_auth
+00001d10: 6020 7061 7261 6d65 7465 7220 6d75 7374  ` parameter must
+00001d20: 2062 6520 7365 7420 7768 656e 2069 6e69   be set when ini
+00001d30: 7469 616c 697a 696e 6720 7468 6520 5344  tializing the SD
+00001d40: 4b20 636c 6965 6e74 2069 6e73 7461 6e63  K client instanc
+00001d50: 652e 2046 6f72 2065 7861 6d70 6c65 3a0a  e. For example:.
+00001d60: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00001d70: 6e0a 2020 2020 2020 2020 696d 706f 7274  n.        import
+00001d80: 206b 6579 6d61 7465 6170 690a 2020 2020   keymateapi.    
+00001d90: 2020 2020 0a20 2020 2020 2020 2073 203d      .        s =
+00001da0: 206b 6579 6d61 7465 6170 692e 4b65 796d   keymateapi.Keym
+00001db0: 6174 6561 7069 280a 2020 2020 2020 2020  ateapi(.        
+00001dc0: 2020 2020 6265 6172 6572 5f61 7574 683d      bearer_auth=
+00001dd0: 223c 594f 5552 5f42 4541 5245 525f 544f  "<YOUR_BEARER_TO
+00001de0: 4b45 4e5f 4845 5245 3e22 2c0a 2020 2020  KEN_HERE>",.    
+00001df0: 2020 2020 290a 2020 2020 2020 2020 0a20      ).        . 
+00001e00: 2020 2020 2020 2072 6573 203d 2073 2e75         res = s.u
+00001e10: 7073 6572 7428 713d 2749 2070 7265 6665  psert(q='I prefe
+00001e20: 7220 436f 7374 6120 6f76 6572 2053 7461  r Costa over Sta
+00001e30: 7262 7563 6b73 2e27 290a 2020 2020 2020  rbucks.').      
+00001e40: 2020 0a20 2020 2020 2020 2069 6620 7265    .        if re
+00001e50: 732e 6f62 6a65 6374 2069 7320 6e6f 7420  s.object is not 
+00001e60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00001e70: 2020 2320 6861 6e64 6c65 2072 6573 706f    # handle respo
+00001e80: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
+00001e90: 7061 7373 0a20 2020 2020 2020 200a 2020  pass.        .  
+00001ea0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00001eb0: 2020 3c21 2d2d 2045 6e64 2041 7574 6865    <!-- End Authe
+00001ec0: 6e74 6963 6174 696f 6e20 5b73 6563 7572  ntication [secur
+00001ed0: 6974 795d 202d 2d3e 0a20 2020 2020 2020  ity] -->.       
+00001ee0: 200a 2020 2020 2020 2020 3c21 2d2d 2050   .        <!-- P
+00001ef0: 6c61 6365 686f 6c64 6572 2066 6f72 2046  laceholder for F
+00001f00: 7574 7572 6520 5370 6561 6b65 6173 7920  uture Speakeasy 
+00001f10: 5344 4b20 5365 6374 696f 6e73 202d 2d3e  SDK Sections -->
+00001f20: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001f30: 2020 2320 4465 7665 6c6f 706d 656e 740a    # Development.
+00001f40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001f50: 2023 2320 4d61 7475 7269 7479 0a20 2020   ## Maturity.   
+00001f60: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
+00001f70: 6973 2053 444b 2069 7320 696e 2062 6574  is SDK is in bet
+00001f80: 612c 2061 6e64 2074 6865 7265 206d 6179  a, and there may
+00001f90: 2062 6520 6272 6561 6b69 6e67 2063 6861   be breaking cha
+00001fa0: 6e67 6573 2062 6574 7765 656e 2076 6572  nges between ver
+00001fb0: 7369 6f6e 7320 7769 7468 6f75 7420 6120  sions without a 
+00001fc0: 6d61 6a6f 7220 7665 7273 696f 6e20 7570  major version up
+00001fd0: 6461 7465 2e20 5468 6572 6566 6f72 652c  date. Therefore,
+00001fe0: 2077 6520 7265 636f 6d6d 656e 6420 7069   we recommend pi
+00001ff0: 6e6e 696e 6720 7573 6167 650a 2020 2020  nning usage.    
+00002000: 2020 2020 746f 2061 2073 7065 6369 6669      to a specifi
+00002010: 6320 7061 636b 6167 6520 7665 7273 696f  c package versio
+00002020: 6e2e 2054 6869 7320 7761 792c 2079 6f75  n. This way, you
+00002030: 2063 616e 2069 6e73 7461 6c6c 2074 6865   can install the
+00002040: 2073 616d 6520 7665 7273 696f 6e20 6561   same version ea
+00002050: 6368 2074 696d 6520 7769 7468 6f75 7420  ch time without 
+00002060: 6272 6561 6b69 6e67 2063 6861 6e67 6573  breaking changes
+00002070: 2075 6e6c 6573 7320 796f 7520 6172 6520   unless you are 
+00002080: 696e 7465 6e74 696f 6e61 6c6c 790a 2020  intentionally.  
+00002090: 2020 2020 2020 6c6f 6f6b 696e 6720 666f        looking fo
+000020a0: 7220 7468 6520 6c61 7465 7374 2076 6572  r the latest ver
+000020b0: 7369 6f6e 2e0a 2020 2020 2020 2020 0a20  sion..        . 
+000020c0: 2020 2020 2020 2023 2320 436f 6e74 7269         ## Contri
+000020d0: 6275 7469 6f6e 730a 2020 2020 2020 2020  butions.        
+000020e0: 0a20 2020 2020 2020 2057 6869 6c65 2077  .        While w
+000020f0: 6520 7661 6c75 6520 6f70 656e 2d73 6f75  e value open-sou
+00002100: 7263 6520 636f 6e74 7269 6275 7469 6f6e  rce contribution
+00002110: 7320 746f 2074 6869 7320 5344 4b2c 2074  s to this SDK, t
+00002120: 6869 7320 6c69 6272 6172 7920 6973 2067  his library is g
+00002130: 656e 6572 6174 6564 2070 726f 6772 616d  enerated program
+00002140: 6d61 7469 6361 6c6c 792e 0a20 2020 2020  matically..     
+00002150: 2020 2046 6565 6c20 6672 6565 2074 6f20     Feel free to 
+00002160: 6f70 656e 2061 2050 5220 6f72 2061 2047  open a PR or a G
+00002170: 6974 6875 6220 6973 7375 6520 6173 2061  ithub issue as a
+00002180: 2070 726f 6f66 206f 6620 636f 6e63 6570   proof of concep
+00002190: 7420 616e 6420 7765 276c 6c20 646f 206f  t and we'll do o
+000021a0: 7572 2062 6573 7420 746f 2069 6e63 6c75  ur best to inclu
+000021b0: 6465 2069 7420 696e 2061 2066 7574 7572  de it in a futur
+000021c0: 6520 7265 6c65 6173 6521 0a20 2020 2020  e release!.     
+000021d0: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
+000021e0: 5344 4b20 4372 6561 7465 6420 6279 205b  SDK Created by [
+000021f0: 5370 6561 6b65 6173 795d 2868 7474 7073  Speakeasy](https
+00002200: 3a2f 2f64 6f63 732e 7370 6561 6b65 6173  ://docs.speakeas
+00002210: 7961 7069 2e64 6576 2f64 6f63 732f 7573  yapi.dev/docs/us
+00002220: 696e 672d 7370 6561 6b65 6173 792f 636c  ing-speakeasy/cl
+00002230: 6965 6e74 2d73 646b 7329 0a20 2020 2020  ient-sdks).     
+00002240: 2020 200a 506c 6174 666f 726d 3a20 554e     .Platform: UN
+00002250: 4b4e 4f57 4e0a 5265 7175 6972 6573 2d50  KNOWN.Requires-P
+00002260: 7974 686f 6e3a 203e 3d33 2e38 0a44 6573  ython: >=3.8.Des
+00002270: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00002280: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00002290: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+000022a0: 7472 613a 2064 6576 0a                   tra: dev.
```

### Comparing `keymateapi-0.3.3/src/keymateapi.egg-info/SOURCES.txt` & `keymateapi-0.4.0/src/keymateapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

