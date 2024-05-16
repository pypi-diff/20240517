# Comparing `tmp/docta_http_client-0.1.1-py3-none-any.whl.zip` & `tmp/docta_http_client-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4072 bytes, number of entries: 10
+Zip file size: 4093 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       76 b- defN 24-May-08 20:05 docta_http_client/__init__.py
 -rw-r--r--  2.0 unx     1032 b- defN 24-May-08 01:50 docta_http_client/base_client.py
--rw-r--r--  2.0 unx      505 b- defN 24-May-08 00:32 docta_http_client/docta_http_client.py
+-rw-r--r--  2.0 unx      541 b- defN 24-May-16 21:38 docta_http_client/docta_http_client.py
 -rw-r--r--  2.0 unx       86 b- defN 24-May-07 23:50 docta_http_client/models.py
 -rw-r--r--  2.0 unx      691 b- defN 24-May-07 22:31 docta_http_client/utils.py
--rw-r--r--  2.0 unx     1065 b- defN 24-May-08 20:08 docta_http_client-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      505 b- defN 24-May-08 20:08 docta_http_client-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-08 20:08 docta_http_client-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-May-08 20:08 docta_http_client-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      866 b- defN 24-May-08 20:08 docta_http_client-0.1.1.dist-info/RECORD
-10 files, 4936 bytes uncompressed, 2568 bytes compressed:  48.0%
+-rw-r--r--  2.0 unx     1065 b- defN 24-May-16 23:05 docta_http_client-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      505 b- defN 24-May-16 23:05 docta_http_client-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 23:05 docta_http_client-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-16 23:05 docta_http_client-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      866 b- defN 24-May-16 23:05 docta_http_client-0.1.2.dist-info/RECORD
+10 files, 4972 bytes uncompressed, 2589 bytes compressed:  47.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: docta_http_client/models.py
 Comment: 
 
 Filename: docta_http_client/utils.py
 Comment: 
 
-Filename: docta_http_client-0.1.1.dist-info/LICENSE
+Filename: docta_http_client-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: docta_http_client-0.1.1.dist-info/METADATA
+Filename: docta_http_client-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: docta_http_client-0.1.1.dist-info/WHEEL
+Filename: docta_http_client-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: docta_http_client-0.1.1.dist-info/top_level.txt
+Filename: docta_http_client-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: docta_http_client-0.1.1.dist-info/RECORD
+Filename: docta_http_client-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docta_http_client/docta_http_client.py

```diff
@@ -1,9 +1,10 @@
 from .base_client import APIClient
 from .models import ModelType
+import json
 
 class DoctaHTTPClient(APIClient):
     def __init__(self, api_key, user_id):
         super().__init__(api_key, user_id)
         self.model = None
     
     def set_model(self, model: ModelType):
@@ -11,8 +12,8 @@
     
     def get_model(self):
         return self.model
     
     def run_docta(self, data):
         if not self.model:
             raise ValueError("model is not set")
-        return self.post(self.model._value_, data)
+        return json.loads(self.post(self.model._value_, data)["response"])
```

## Comparing `docta_http_client-0.1.1.dist-info/LICENSE` & `docta_http_client-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `docta_http_client-0.1.1.dist-info/RECORD` & `docta_http_client-0.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 docta_http_client/__init__.py,sha256=rq5dxH3b_rOuq-mHbZFwRAkWbH63wlGY8-NWjfRpRps,76
 docta_http_client/base_client.py,sha256=SsCivffkIZv2b1anbn76uUQaghJwcRGIVq94X9c4GEs,1032
-docta_http_client/docta_http_client.py,sha256=l6IZ278M_52a9EsRvnjrp9zbITVhz_ZUSnUQ-cFkBhY,505
+docta_http_client/docta_http_client.py,sha256=YX0QkgrmHLBUBvPzIzPZp_VZKYf0LxiMP1IE327rWjg,541
 docta_http_client/models.py,sha256=oEh6yoJkYGQBS79riZcFOPn9hKGa3cT1Wo0WlDuH_88,86
 docta_http_client/utils.py,sha256=cHvgG6gEBquhu1XBTkPwTObLd1adBx2kIkbd9-6nWKw,691
-docta_http_client-0.1.1.dist-info/LICENSE,sha256=7gNWxKhu4VQ5OcG2fgenn1w_coXRfbgSV-6tHxUr1Rw,1065
-docta_http_client-0.1.1.dist-info/METADATA,sha256=r5NXWxBwU2MdFRQeXKTDt8c7iLM2ObKP5pvRO0f3c3E,505
-docta_http_client-0.1.1.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-docta_http_client-0.1.1.dist-info/top_level.txt,sha256=pkMUieP5XMAdQiI4PP2_SDaj61cBi_OEqMC-Dl5z5JE,18
-docta_http_client-0.1.1.dist-info/RECORD,,
+docta_http_client-0.1.2.dist-info/LICENSE,sha256=7gNWxKhu4VQ5OcG2fgenn1w_coXRfbgSV-6tHxUr1Rw,1065
+docta_http_client-0.1.2.dist-info/METADATA,sha256=ZwTvVwaxulamV9r4cYMPj0h9EcCOmJKNLrsMIY6WYAE,505
+docta_http_client-0.1.2.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+docta_http_client-0.1.2.dist-info/top_level.txt,sha256=pkMUieP5XMAdQiI4PP2_SDaj61cBi_OEqMC-Dl5z5JE,18
+docta_http_client-0.1.2.dist-info/RECORD,,
```

