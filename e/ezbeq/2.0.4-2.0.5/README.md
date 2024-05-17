# Comparing `tmp/ezbeq-2.0.4.tar.gz` & `tmp/ezbeq-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezbeq-2.0.4.tar", max compression
+gzip compressed data, was "ezbeq-2.0.5.tar", max compression
```

## Comparing `ezbeq-2.0.4.tar` & `ezbeq-2.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1066 2023-12-14 10:02:27.406545 ezbeq-2.0.4/LICENSE
--rw-r--r--   0        0        0    12862 2023-12-14 10:02:27.406545 ezbeq-2.0.4/README.md
--rw-r--r--   0        0        0        6 2023-12-14 10:03:35.942132 ezbeq-2.0.4/ezbeq/VERSION
--rw-r--r--   0        0        0      264 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/__init__.py
--rw-r--r--   0        0        0       57 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/__init__.py
--rw-r--r--   0        0        0      481 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/audiotypes.py
--rw-r--r--   0        0        0      471 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/authors.py
--rw-r--r--   0        0        0     1545 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/catalogue.py
--rw-r--r--   0        0        0      487 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/contenttypes.py
--rw-r--r--   0        0        0    26273 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/devices.py
--rw-r--r--   0        0        0     2722 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/diagnostics.py
--rw-r--r--   0        0        0      479 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/languages.py
--rw-r--r--   0        0        0      450 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/load.py
--rw-r--r--   0        0        0      725 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/meta.py
--rw-r--r--   0        0        0     2540 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/search.py
--rw-r--r--   0        0        0      354 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/version.py
--rw-r--r--   0        0        0     8182 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/ws.py
--rw-r--r--   0        0        0      482 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/apis/years.py
--rw-r--r--   0        0        0    28594 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/camilladsp.py
--rw-r--r--   0        0        0    37382 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/catalogue.py
--rw-r--r--   0        0        0     9715 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/config.py
--rw-r--r--   0        0        0     9023 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/device.py
--rw-r--r--   0        0        0    13553 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/htp1.py
--rw-r--r--   0        0        0     4483 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/iir.py
--rw-r--r--   0        0        0    22990 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/jriver.py
--rw-r--r--   0        0        0     6955 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/main.py
--rw-r--r--   0        0        0    41213 2023-12-14 10:02:27.434545 ezbeq-2.0.4/ezbeq/minidsp.py
--rw-r--r--   0        0        0     9693 2023-12-14 10:02:27.438545 ezbeq-2.0.4/ezbeq/qsys.py
--rw-r--r--   0        0        0     4303 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0        0        0    14091 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0        0        0     3262 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/apple-touch-icon.png
--rw-r--r--   0        0        0   852949 2023-12-14 10:03:35.674134 ezbeq-2.0.4/ezbeq/ui/assets/index-d43a2bed.js
--rw-r--r--   0        0        0     5721 2023-12-14 10:03:35.674134 ezbeq-2.0.4/ezbeq/ui/assets/index-fce6f16f.css
--rw-r--r--   0        0        0    65456 2023-12-14 10:03:35.674134 ezbeq-2.0.4/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
--rw-r--r--   0        0        0     9628 2023-12-14 10:03:35.674134 ezbeq-2.0.4/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
--rw-r--r--   0        0        0    15344 2023-12-14 10:03:35.670134 ezbeq-2.0.4/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
--rw-r--r--   0        0        0     7112 2023-12-14 10:03:35.674134 ezbeq-2.0.4/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
--rw-r--r--   0        0        0    15744 2023-12-14 10:03:35.674134 ezbeq-2.0.4/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
--rw-r--r--   0        0        0    11872 2023-12-14 10:03:35.674134 ezbeq-2.0.4/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
--rw-r--r--   0        0        0     5560 2023-12-14 10:03:35.674134 ezbeq-2.0.4/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
--rw-r--r--   0        0        0      246 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/browserconfig.xml
--rw-r--r--   0        0        0      702 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0        0        0     1310 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0        0        0     7406 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/favicon.ico
--rw-r--r--   0        0        0     1012 2023-12-14 10:03:35.674134 ezbeq-2.0.4/ezbeq/ui/index.html
--rw-r--r--   0        0        0     2533 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0        0        0       67 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/robots.txt
--rw-r--r--   0        0        0     3278 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0        0        0      436 2023-12-14 10:03:35.138137 ezbeq-2.0.4/ezbeq/ui/site.webmanifest
--rw-r--r--   0        0        0     1285 2023-12-14 10:02:27.438545 ezbeq-2.0.4/pyproject.toml
--rw-r--r--   0        0        0    14068 1970-01-01 00:00:00.000000 ezbeq-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-14 12:07:03.003065 ezbeq-2.0.5/LICENSE
+-rw-r--r--   0        0        0    12862 2023-12-14 12:07:03.003065 ezbeq-2.0.5/README.md
+-rw-r--r--   0        0        0        6 2023-12-14 12:08:13.719157 ezbeq-2.0.5/ezbeq/VERSION
+-rw-r--r--   0        0        0      264 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/__init__.py
+-rw-r--r--   0        0        0       57 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/__init__.py
+-rw-r--r--   0        0        0      481 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/audiotypes.py
+-rw-r--r--   0        0        0      471 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/authors.py
+-rw-r--r--   0        0        0     1545 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/catalogue.py
+-rw-r--r--   0        0        0      487 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/contenttypes.py
+-rw-r--r--   0        0        0    26273 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/devices.py
+-rw-r--r--   0        0        0     2722 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/diagnostics.py
+-rw-r--r--   0        0        0      479 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/languages.py
+-rw-r--r--   0        0        0      450 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/load.py
+-rw-r--r--   0        0        0      725 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/meta.py
+-rw-r--r--   0        0        0     2540 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/search.py
+-rw-r--r--   0        0        0      354 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/version.py
+-rw-r--r--   0        0        0     8182 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/ws.py
+-rw-r--r--   0        0        0      482 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/apis/years.py
+-rw-r--r--   0        0        0    28594 2023-12-14 12:07:03.031065 ezbeq-2.0.5/ezbeq/camilladsp.py
+-rw-r--r--   0        0        0    37382 2023-12-14 12:07:03.035065 ezbeq-2.0.5/ezbeq/catalogue.py
+-rw-r--r--   0        0        0     9715 2023-12-14 12:07:03.035065 ezbeq-2.0.5/ezbeq/config.py
+-rw-r--r--   0        0        0     9023 2023-12-14 12:07:03.035065 ezbeq-2.0.5/ezbeq/device.py
+-rw-r--r--   0        0        0    13553 2023-12-14 12:07:03.035065 ezbeq-2.0.5/ezbeq/htp1.py
+-rw-r--r--   0        0        0     4483 2023-12-14 12:07:03.035065 ezbeq-2.0.5/ezbeq/iir.py
+-rw-r--r--   0        0        0    22997 2023-12-14 12:07:03.035065 ezbeq-2.0.5/ezbeq/jriver.py
+-rw-r--r--   0        0        0     6955 2023-12-14 12:07:03.035065 ezbeq-2.0.5/ezbeq/main.py
+-rw-r--r--   0        0        0    41213 2023-12-14 12:07:03.035065 ezbeq-2.0.5/ezbeq/minidsp.py
+-rw-r--r--   0        0        0     9693 2023-12-14 12:07:03.035065 ezbeq-2.0.5/ezbeq/qsys.py
+-rw-r--r--   0        0        0     4303 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0        0        0    14091 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0        0        0     3262 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/apple-touch-icon.png
+-rw-r--r--   0        0        0   852949 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/assets/index-d43a2bed.js
+-rw-r--r--   0        0        0     5721 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/assets/index-fce6f16f.css
+-rw-r--r--   0        0        0    65456 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
+-rw-r--r--   0        0        0     9628 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
+-rw-r--r--   0        0        0    15344 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
+-rw-r--r--   0        0        0     7112 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
+-rw-r--r--   0        0        0    15744 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
+-rw-r--r--   0        0        0    11872 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
+-rw-r--r--   0        0        0     5560 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
+-rw-r--r--   0        0        0      246 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0        0        0      702 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0        0        0     1310 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0        0        0     7406 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/favicon.ico
+-rw-r--r--   0        0        0     1012 2023-12-14 12:08:13.451157 ezbeq-2.0.5/ezbeq/ui/index.html
+-rw-r--r--   0        0        0     2533 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0        0        0       67 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/robots.txt
+-rw-r--r--   0        0        0     3278 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      436 2023-12-14 12:08:12.919156 ezbeq-2.0.5/ezbeq/ui/site.webmanifest
+-rw-r--r--   0        0        0     1285 2023-12-14 12:07:03.035065 ezbeq-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0    14068 1970-01-01 00:00:00.000000 ezbeq-2.0.5/PKG-INFO
```

### Comparing `ezbeq-2.0.4/LICENSE` & `ezbeq-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/README.md` & `ezbeq-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/apis/catalogue.py` & `ezbeq-2.0.5/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/apis/devices.py` & `ezbeq-2.0.5/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/apis/diagnostics.py` & `ezbeq-2.0.5/ezbeq/apis/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/apis/meta.py` & `ezbeq-2.0.5/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/apis/search.py` & `ezbeq-2.0.5/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/apis/ws.py` & `ezbeq-2.0.5/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/camilladsp.py` & `ezbeq-2.0.5/ezbeq/camilladsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/catalogue.py` & `ezbeq-2.0.5/ezbeq/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/config.py` & `ezbeq-2.0.5/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/device.py` & `ezbeq-2.0.5/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/htp1.py` & `ezbeq-2.0.5/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/iir.py` & `ezbeq-2.0.5/ezbeq/iir.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/jriver.py` & `ezbeq-2.0.5/ezbeq/jriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             zone_id = self._current_state.get_zone_id(slot)
             current_config_txt = self.__mcws.get_dsp(zone_id)
             new_config_txt = self.__remove_all_beq(current_config_txt)
             new_config_txt = include_filters_in_dsp(self.__peq_block, new_config_txt, xml_filts, replace=False)
             logger.info(new_config_txt)
             try:
                 self.__mcws.set_dsp(zone_id, new_config_txt)
-                self._current_state.set_title(slot, entry.formatted_title, entry.author)
+                self._current_state.set_title(slot, entry.formatted_title, author=entry.author)
             except Exception as e:
                 self._current_state.slot.last = 'ERROR'
                 self._current_state.slot.last_author = None
                 raise e
         self._hydrate_cache_broadcast(__do_it)
 
     def __remove_all_beq(self, current_config_txt) -> str:
```

### Comparing `ezbeq-2.0.4/ezbeq/main.py` & `ezbeq-2.0.5/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/minidsp.py` & `ezbeq-2.0.5/ezbeq/minidsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/qsys.py` & `ezbeq-2.0.5/ezbeq/qsys.py`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-2.0.5/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-2.0.5/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/apple-touch-icon.png` & `ezbeq-2.0.5/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/assets/index-d43a2bed.js` & `ezbeq-2.0.5/ezbeq/ui/assets/index-d43a2bed.js`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/assets/index-fce6f16f.css` & `ezbeq-2.0.5/ezbeq/ui/assets/index-fce6f16f.css`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff` & `ezbeq-2.0.5/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2` & `ezbeq-2.0.5/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2` & `ezbeq-2.0.5/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2` & `ezbeq-2.0.5/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2` & `ezbeq-2.0.5/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2` & `ezbeq-2.0.5/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2` & `ezbeq-2.0.5/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/favicon-16x16.png` & `ezbeq-2.0.5/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/favicon-32x32.png` & `ezbeq-2.0.5/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/favicon.ico` & `ezbeq-2.0.5/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/index.html` & `ezbeq-2.0.5/ezbeq/ui/index.html`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/mstile-150x150.png` & `ezbeq-2.0.5/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-2.0.5/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-2.0.4/pyproject.toml` & `ezbeq-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ezbeq"
-version = "2.0.4"
+version = "2.0.5"
 description = "A webapp which can send beqcatalogue filters to a DSP device"
 authors = ["3ll3d00d <mattkhan+ezbeq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ezbeq.readthedocs.io/"
 repository = "https://github.com/3ll3d00d/ezbeq"
 include = [
```

### Comparing `ezbeq-2.0.4/PKG-INFO` & `ezbeq-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 2.0.4
+Version: 2.0.5
 Summary: A webapp which can send beqcatalogue filters to a DSP device
 Home-page: https://ezbeq.readthedocs.io/
 License: MIT
 Author: 3ll3d00d
 Author-email: mattkhan+ezbeq@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

