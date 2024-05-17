# Comparing `tmp/ezbeq-2.1.0a0.tar.gz` & `tmp/ezbeq-2.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezbeq-2.1.0a0.tar", max compression
+gzip compressed data, was "ezbeq-2.1.0a2.tar", max compression
```

## Comparing `ezbeq-2.1.0a0.tar` & `ezbeq-2.1.0a2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1066 2024-05-17 12:32:43.748959 ezbeq-2.1.0a0/LICENSE
--rw-r--r--   0        0        0    15596 2024-05-17 12:32:43.748959 ezbeq-2.1.0a0/README.md
--rw-r--r--   0        0        0        8 2024-05-17 12:33:52.297304 ezbeq-2.1.0a0/ezbeq/VERSION
--rw-r--r--   0        0        0      264 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/__init__.py
--rw-r--r--   0        0        0       57 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/__init__.py
--rw-r--r--   0        0        0      481 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/audiotypes.py
--rw-r--r--   0        0        0      471 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/authors.py
--rw-r--r--   0        0        0     1545 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/catalogue.py
--rw-r--r--   0        0        0      487 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/contenttypes.py
--rw-r--r--   0        0        0    26273 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/devices.py
--rw-r--r--   0        0        0     2722 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/diagnostics.py
--rw-r--r--   0        0        0      479 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/languages.py
--rw-r--r--   0        0        0      450 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/load.py
--rw-r--r--   0        0        0      725 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/meta.py
--rw-r--r--   0        0        0     2540 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/search.py
--rw-r--r--   0        0        0      354 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/version.py
--rw-r--r--   0        0        0     8182 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/ws.py
--rw-r--r--   0        0        0      482 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/apis/years.py
--rw-r--r--   0        0        0    28594 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/camilladsp.py
--rw-r--r--   0        0        0    37382 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/catalogue.py
--rw-r--r--   0        0        0     8912 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/config.py
--rw-r--r--   0        0        0     9023 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/device.py
--rw-r--r--   0        0        0    13553 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/htp1.py
--rw-r--r--   0        0        0     4483 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/iir.py
--rw-r--r--   0        0        0    22997 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/jriver.py
--rw-r--r--   0        0        0     6834 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/main.py
--rw-r--r--   0        0        0    41427 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/minidsp.py
--rw-r--r--   0        0        0     9693 2024-05-17 12:32:43.776959 ezbeq-2.1.0a0/ezbeq/qsys.py
--rw-r--r--   0        0        0     4303 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0        0        0    14091 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0        0        0     3262 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/apple-touch-icon.png
--rw-r--r--   0        0        0   921462 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/index-B7t5VNAq.js
--rw-r--r--   0        0        0     7542 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/index-Bw8DTJKm.css
--rw-r--r--   0        0        0     8392 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-cyrillic-400-normal-DCQqOlfN.woff
--rw-r--r--   0        0        0     9628 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-cyrillic-400-normal-DVDTZtmW.woff2
--rw-r--r--   0        0        0    13468 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal--KougVX-.woff
--rw-r--r--   0        0        0    15344 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-DORK9bGA.woff2
--rw-r--r--   0        0        0     7112 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-greek-400-normal-BRWHCUYo.woff2
--rw-r--r--   0        0        0     6348 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-greek-400-normal-BnGNaKeW.woff
--rw-r--r--   0        0        0    14384 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-latin-400-normal-BU1SoK4h.woff
--rw-r--r--   0        0        0    15744 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-latin-400-normal-mTIRXP6Y.woff2
--rw-r--r--   0        0        0    11872 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-latin-ext-400-normal-4bLplyDh.woff2
--rw-r--r--   0        0        0    10208 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-latin-ext-400-normal-DloBNwoc.woff
--rw-r--r--   0        0        0     4752 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-vietnamese-400-normal-BkEBOAV9.woff
--rw-r--r--   0        0        0     5560 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-vietnamese-400-normal-kCRe3VZk.woff2
--rw-r--r--   0        0        0      246 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/browserconfig.xml
--rw-r--r--   0        0        0      702 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0        0        0     1310 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0        0        0     7406 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/favicon.ico
--rw-r--r--   0        0        0     1023 2024-05-17 12:33:51.993302 ezbeq-2.1.0a0/ezbeq/ui/index.html
--rw-r--r--   0        0        0     2533 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0        0        0       67 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/robots.txt
--rw-r--r--   0        0        0     3278 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0        0        0      436 2024-05-17 12:33:51.477300 ezbeq-2.1.0a0/ezbeq/ui/site.webmanifest
--rw-r--r--   0        0        0     1274 2024-05-17 12:32:43.780959 ezbeq-2.1.0a0/pyproject.toml
--rw-r--r--   0        0        0    16673 1970-01-01 00:00:00.000000 ezbeq-2.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 12:59:53.387090 ezbeq-2.1.0a2/LICENSE
+-rw-r--r--   0        0        0    15596 2024-05-17 12:59:53.387090 ezbeq-2.1.0a2/README.md
+-rw-r--r--   0        0        0        8 2024-05-17 13:01:04.670149 ezbeq-2.1.0a2/ezbeq/VERSION
+-rw-r--r--   0        0        0      264 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/audiotypes.py
+-rw-r--r--   0        0        0      471 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/authors.py
+-rw-r--r--   0        0        0     1545 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/catalogue.py
+-rw-r--r--   0        0        0      487 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/contenttypes.py
+-rw-r--r--   0        0        0    26273 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/devices.py
+-rw-r--r--   0        0        0     2722 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/diagnostics.py
+-rw-r--r--   0        0        0      479 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/languages.py
+-rw-r--r--   0        0        0      450 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/load.py
+-rw-r--r--   0        0        0      725 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/meta.py
+-rw-r--r--   0        0        0     2540 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/search.py
+-rw-r--r--   0        0        0      354 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/version.py
+-rw-r--r--   0        0        0     8182 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/ws.py
+-rw-r--r--   0        0        0      482 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/apis/years.py
+-rw-r--r--   0        0        0    28594 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/camilladsp.py
+-rw-r--r--   0        0        0    37382 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/catalogue.py
+-rw-r--r--   0        0        0     8912 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/config.py
+-rw-r--r--   0        0        0     9023 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/device.py
+-rw-r--r--   0        0        0    13553 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/htp1.py
+-rw-r--r--   0        0        0     4483 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/iir.py
+-rw-r--r--   0        0        0    22997 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/jriver.py
+-rw-r--r--   0        0        0     6834 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/main.py
+-rw-r--r--   0        0        0    41427 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/minidsp.py
+-rw-r--r--   0        0        0     9693 2024-05-17 12:59:53.415090 ezbeq-2.1.0a2/ezbeq/qsys.py
+-rw-r--r--   0        0        0     4303 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0        0        0    14091 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0        0        0     3262 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/apple-touch-icon.png
+-rw-r--r--   0        0        0   921462 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/index-B7t5VNAq.js
+-rw-r--r--   0        0        0     7542 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/index-Bw8DTJKm.css
+-rw-r--r--   0        0        0     8392 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-cyrillic-400-normal-DCQqOlfN.woff
+-rw-r--r--   0        0        0     9628 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-cyrillic-400-normal-DVDTZtmW.woff2
+-rw-r--r--   0        0        0    13468 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal--KougVX-.woff
+-rw-r--r--   0        0        0    15344 2024-05-17 13:01:04.486152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-DORK9bGA.woff2
+-rw-r--r--   0        0        0     7112 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-greek-400-normal-BRWHCUYo.woff2
+-rw-r--r--   0        0        0     6348 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-greek-400-normal-BnGNaKeW.woff
+-rw-r--r--   0        0        0    14384 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-latin-400-normal-BU1SoK4h.woff
+-rw-r--r--   0        0        0    15744 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-latin-400-normal-mTIRXP6Y.woff2
+-rw-r--r--   0        0        0    11872 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-latin-ext-400-normal-4bLplyDh.woff2
+-rw-r--r--   0        0        0    10208 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-latin-ext-400-normal-DloBNwoc.woff
+-rw-r--r--   0        0        0     4752 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-vietnamese-400-normal-BkEBOAV9.woff
+-rw-r--r--   0        0        0     5560 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-vietnamese-400-normal-kCRe3VZk.woff2
+-rw-r--r--   0        0        0      246 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0        0        0      702 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0        0        0     1310 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0        0        0     7406 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/favicon.ico
+-rw-r--r--   0        0        0     1023 2024-05-17 13:01:04.490152 ezbeq-2.1.0a2/ezbeq/ui/index.html
+-rw-r--r--   0        0        0     2533 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0        0        0       67 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/robots.txt
+-rw-r--r--   0        0        0     3278 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      436 2024-05-17 13:01:03.970159 ezbeq-2.1.0a2/ezbeq/ui/site.webmanifest
+-rw-r--r--   0        0        0     1274 2024-05-17 12:59:53.419090 ezbeq-2.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0    16673 1970-01-01 00:00:00.000000 ezbeq-2.1.0a2/PKG-INFO
```

### Comparing `ezbeq-2.1.0a0/LICENSE` & `ezbeq-2.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/README.md` & `ezbeq-2.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/apis/catalogue.py` & `ezbeq-2.1.0a2/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/apis/devices.py` & `ezbeq-2.1.0a2/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/apis/diagnostics.py` & `ezbeq-2.1.0a2/ezbeq/apis/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/apis/meta.py` & `ezbeq-2.1.0a2/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/apis/search.py` & `ezbeq-2.1.0a2/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/apis/ws.py` & `ezbeq-2.1.0a2/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/camilladsp.py` & `ezbeq-2.1.0a2/ezbeq/camilladsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/catalogue.py` & `ezbeq-2.1.0a2/ezbeq/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/config.py` & `ezbeq-2.1.0a2/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/device.py` & `ezbeq-2.1.0a2/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/htp1.py` & `ezbeq-2.1.0a2/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/iir.py` & `ezbeq-2.1.0a2/ezbeq/iir.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/jriver.py` & `ezbeq-2.1.0a2/ezbeq/jriver.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/main.py` & `ezbeq-2.1.0a2/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/minidsp.py` & `ezbeq-2.1.0a2/ezbeq/minidsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/qsys.py` & `ezbeq-2.1.0a2/ezbeq/qsys.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-2.1.0a2/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-2.1.0a2/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/apple-touch-icon.png` & `ezbeq-2.1.0a2/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/index-B7t5VNAq.js` & `ezbeq-2.1.0a2/ezbeq/ui/assets/index-B7t5VNAq.js`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/index-Bw8DTJKm.css` & `ezbeq-2.1.0a2/ezbeq/ui/assets/index-Bw8DTJKm.css`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-cyrillic-400-normal-DCQqOlfN.woff` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-cyrillic-400-normal-DCQqOlfN.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-cyrillic-400-normal-DVDTZtmW.woff2` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-cyrillic-400-normal-DVDTZtmW.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal--KougVX-.woff` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal--KougVX-.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-DORK9bGA.woff2` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-DORK9bGA.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-greek-400-normal-BRWHCUYo.woff2` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-greek-400-normal-BRWHCUYo.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-greek-400-normal-BnGNaKeW.woff` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-greek-400-normal-BnGNaKeW.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-latin-400-normal-BU1SoK4h.woff` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-latin-400-normal-BU1SoK4h.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-latin-400-normal-mTIRXP6Y.woff2` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-latin-400-normal-mTIRXP6Y.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-latin-ext-400-normal-4bLplyDh.woff2` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-latin-ext-400-normal-4bLplyDh.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-latin-ext-400-normal-DloBNwoc.woff` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-latin-ext-400-normal-DloBNwoc.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-vietnamese-400-normal-BkEBOAV9.woff` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-vietnamese-400-normal-BkEBOAV9.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/assets/roboto-vietnamese-400-normal-kCRe3VZk.woff2` & `ezbeq-2.1.0a2/ezbeq/ui/assets/roboto-vietnamese-400-normal-kCRe3VZk.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/favicon-16x16.png` & `ezbeq-2.1.0a2/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/favicon-32x32.png` & `ezbeq-2.1.0a2/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/favicon.ico` & `ezbeq-2.1.0a2/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/index.html` & `ezbeq-2.1.0a2/ezbeq/ui/index.html`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/mstile-150x150.png` & `ezbeq-2.1.0a2/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-2.1.0a2/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-2.1.0a0/pyproject.toml` & `ezbeq-2.1.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ezbeq"
-version = "2.1.0a0"
+version = "2.1.0a2"
 description = "A webapp which can send beqcatalogue filters to a DSP device"
 authors = ["3ll3d00d <mattkhan+ezbeq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ezbeq.readthedocs.io/"
 repository = "https://github.com/3ll3d00d/ezbeq"
 include = [
```

### Comparing `ezbeq-2.1.0a0/PKG-INFO` & `ezbeq-2.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 2.1.0a0
+Version: 2.1.0a2
 Summary: A webapp which can send beqcatalogue filters to a DSP device
 Home-page: https://ezbeq.readthedocs.io/
 License: MIT
 Author: 3ll3d00d
 Author-email: mattkhan+ezbeq@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

