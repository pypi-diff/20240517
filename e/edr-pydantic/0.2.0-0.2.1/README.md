# Comparing `tmp/edr_pydantic-0.2.0.tar.gz` & `tmp/edr_pydantic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edr_pydantic-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "edr_pydantic-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `edr_pydantic-0.2.0.tar` & `edr_pydantic-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      267 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/.gitignore
--rw-r--r--   0        0        0     2598 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11383 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/LICENSE
--rw-r--r--   0        0        0     4854 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/README.md
--rw-r--r--   0        0        0     1597 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/example.py
--rw-r--r--   0        0        0     1198 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0      208 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/setup.py
--rw-r--r--   0        0        0        0 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/__init__.py
--rw-r--r--   0        0        0      333 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/base_model.py
--rw-r--r--   0        0        0      961 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/capabilities.py
--rw-r--r--   0        0        0     1141 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/collections.py
--rw-r--r--   0        0        0      590 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/data_queries.py
--rw-r--r--   0        0        0      873 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/extent.py
--rw-r--r--   0        0        0      904 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/link.py
--rw-r--r--   0        0        0      357 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/observed_property.py
--rw-r--r--   0        0        0     1678 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/parameter.py
--rw-r--r--   0        0        0        0 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/py.typed
--rw-r--r--   0        0        0      569 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/unit.py
--rw-r--r--   0        0        0      851 2023-10-17 06:57:51.844018 edr_pydantic-0.2.0/src/edr_pydantic/variables.py
--rw-r--r--   0        0        0    30852 2023-10-17 06:57:51.848018 edr_pydantic-0.2.0/tests/test_data/doc-example-collections.json
--rw-r--r--   0        0        0    22444 2023-10-17 06:57:51.848018 edr_pydantic-0.2.0/tests/test_data/knmi-example-collections.json
--rw-r--r--   0        0        0       20 2023-10-17 06:57:51.848018 edr_pydantic-0.2.0/tests/test_data/label-or-symbol-unit.json
--rw-r--r--   0        0        0     1332 2023-10-17 06:57:51.848018 edr_pydantic-0.2.0/tests/test_data/landing-page.json
--rw-r--r--   0        0        0      839 2023-10-17 06:57:51.848018 edr_pydantic-0.2.0/tests/test_data/simple-instance.json
--rw-r--r--   0        0        0     1554 2023-10-17 06:57:51.848018 edr_pydantic-0.2.0/tests/test_edr.py
--rw-r--r--   0        0        0     5825 1970-01-01 00:00:00.000000 edr_pydantic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      267 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/.gitignore
+-rw-r--r--   0        0        0     2598 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11383 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5017 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/README.md
+-rw-r--r--   0        0        0     1597 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/example.py
+-rw-r--r--   0        0        0     1198 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0      208 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/setup.py
+-rw-r--r--   0        0        0        0 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/__init__.py
+-rw-r--r--   0        0        0      333 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/base_model.py
+-rw-r--r--   0        0        0      961 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/capabilities.py
+-rw-r--r--   0        0        0     1141 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/collections.py
+-rw-r--r--   0        0        0      590 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/data_queries.py
+-rw-r--r--   0        0        0      873 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/extent.py
+-rw-r--r--   0        0        0      904 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/link.py
+-rw-r--r--   0        0        0      357 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/observed_property.py
+-rw-r--r--   0        0        0     1678 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/parameter.py
+-rw-r--r--   0        0        0        0 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/py.typed
+-rw-r--r--   0        0        0      569 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/unit.py
+-rw-r--r--   0        0        0      851 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/src/edr_pydantic/variables.py
+-rw-r--r--   0        0        0    30852 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/tests/test_data/doc-example-collections.json
+-rw-r--r--   0        0        0    22444 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/tests/test_data/knmi-example-collections.json
+-rw-r--r--   0        0        0       20 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/tests/test_data/label-or-symbol-unit.json
+-rw-r--r--   0        0        0     1332 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/tests/test_data/landing-page.json
+-rw-r--r--   0        0        0      839 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/tests/test_data/simple-instance.json
+-rw-r--r--   0        0        0     1554 2023-10-30 14:57:58.175818 edr_pydantic-0.2.1/tests/test_edr.py
+-rw-r--r--   0        0        0     5988 1970-01-01 00:00:00.000000 edr_pydantic-0.2.1/PKG-INFO
```

### Comparing `edr_pydantic-0.2.0/.pre-commit-config.yaml` & `edr_pydantic-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/LICENSE` & `edr_pydantic-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/README.md` & `edr_pydantic-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -162,14 +162,18 @@
 pytest tests/
 ```
 
 ## Real world usage
 
 This library is used to build an Environmental Data Retrieval (EDR) API, serving observation data from surface weather data station data from the KNMI. See the [KNMI Data Platform](https://developer.dataplatform.knmi.nl/edr-api).
 
+## Related projects
+* [CoverageJSON Pydantic](https://github.com/KNMI/covjson-pydantic)
+* [geojson-pydantic](https://github.com/developmentseed/geojson-pydantic)
+
 ## TODOs
 Help is wanted in the following areas to fully implement the EDR spec:
 * See TODOs in code listing various small inconsistencies in the spec
 * In various places there could be more validation on content
 
 ## License
```

#### html2text {}

```diff
@@ -35,11 +35,13 @@
 { "label": "degree true" }, "observedProperty": { "id": "https://codes.wmo.int/
 common/quantity-kind/_windDirection", "label": "Wind Direction" } } } } ``` ##
 Contributing Make an editable install from within the repository root ```shell
 pip install -e '.[test]' ``` ### Running tests ```shell pytest tests/ ``` ##
 Real world usage This library is used to build an Environmental Data Retrieval
 (EDR) API, serving observation data from surface weather data station data from
 the KNMI. See the [KNMI Data Platform](https://developer.dataplatform.knmi.nl/
-edr-api). ## TODOs Help is wanted in the following areas to fully implement the
-EDR spec: * See TODOs in code listing various small inconsistencies in the spec
-* In various places there could be more validation on content ## License Apache
-License, Version 2.0
+edr-api). ## Related projects * [CoverageJSON Pydantic](https://github.com/
+KNMI/covjson-pydantic) * [geojson-pydantic](https://github.com/developmentseed/
+geojson-pydantic) ## TODOs Help is wanted in the following areas to fully
+implement the EDR spec: * See TODOs in code listing various small
+inconsistencies in the spec * In various places there could be more validation
+on content ## License Apache License, Version 2.0
```

### Comparing `edr_pydantic-0.2.0/example.py` & `edr_pydantic-0.2.1/example.py`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/pyproject.toml` & `edr_pydantic-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
     "Typing :: Typed",
 ]
-version = "0.2.0"
+version = "0.2.1"
 dependencies = ["pydantic>=2.3,<3"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 dev = ["pre-commit"]
 
 [project.urls]
```

### Comparing `edr_pydantic-0.2.0/src/edr_pydantic/capabilities.py` & `edr_pydantic-0.2.1/src/edr_pydantic/capabilities.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     postalCode: Optional[str] = None  # noqa: N815
     city: Optional[str] = None
     stateorprovince: Optional[str] = None
     country: Optional[str] = None
 
 
 class LandingPageModel(EdrBaseModel):
-    links: List[Link]
     title: Optional[str] = None
     description: Optional[str] = None
+    links: List[Link]
     keywords: Optional[List[str]] = None
     provider: Optional[Provider] = None
     contact: Optional[Contact] = None
 
 
 class ConformanceModel(EdrBaseModel):
     conformsTo: List[str]  # noqa: N815
```

### Comparing `edr_pydantic-0.2.0/src/edr_pydantic/collections.py` & `edr_pydantic-0.2.1/src/edr_pydantic/collections.py`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/src/edr_pydantic/data_queries.py` & `edr_pydantic-0.2.1/src/edr_pydantic/data_queries.py`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/src/edr_pydantic/extent.py` & `edr_pydantic-0.2.1/src/edr_pydantic/extent.py`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/src/edr_pydantic/link.py` & `edr_pydantic-0.2.1/src/edr_pydantic/link.py`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/src/edr_pydantic/parameter.py` & `edr_pydantic-0.2.1/src/edr_pydantic/parameter.py`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/src/edr_pydantic/unit.py` & `edr_pydantic-0.2.1/src/edr_pydantic/unit.py`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/src/edr_pydantic/variables.py` & `edr_pydantic-0.2.1/src/edr_pydantic/variables.py`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/tests/test_data/doc-example-collections.json` & `edr_pydantic-0.2.1/tests/test_data/doc-example-collections.json`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/tests/test_data/knmi-example-collections.json` & `edr_pydantic-0.2.1/tests/test_data/knmi-example-collections.json`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/tests/test_data/landing-page.json` & `edr_pydantic-0.2.1/tests/test_data/landing-page.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,8 +1,10 @@
 {
+    "title": "Observations API EDR",
+    "description": "The observation api in EDR format from the KNMI",
     "links": [
         {
             "href": "https://api.dataplatform.knmi.nl/edr/",
             "rel": "self",
             "title": "Landing Page in JSON"
         },
         {
@@ -22,16 +24,14 @@
         },
         {
             "href": "https://api.dataplatform.knmi.nl/edr/collections",
             "rel": "data",
             "title": "Collections metadata in JSON"
         }
     ],
-    "title": "Observations API EDR",
-    "description": "The observation api in EDR format from the KNMI",
     "keywords": [
         "Weather",
         "Temperature",
         "Wind",
         "Humidity",
         "Pressure",
         "Clouds",
```

### Comparing `edr_pydantic-0.2.0/tests/test_data/simple-instance.json` & `edr_pydantic-0.2.1/tests/test_data/simple-instance.json`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/tests/test_edr.py` & `edr_pydantic-0.2.1/tests/test_edr.py`

 * *Files identical despite different names*

### Comparing `edr_pydantic-0.2.0/PKG-INFO` & `edr_pydantic-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edr-pydantic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pydantic models for OGC Environmental Data (EDR) API
 Keywords: EDR,Pydantic
 Author-email: KNMI Data Platform Team <opendata@knmi.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -187,14 +187,18 @@
 pytest tests/
 ```
 
 ## Real world usage
 
 This library is used to build an Environmental Data Retrieval (EDR) API, serving observation data from surface weather data station data from the KNMI. See the [KNMI Data Platform](https://developer.dataplatform.knmi.nl/edr-api).
 
+## Related projects
+* [CoverageJSON Pydantic](https://github.com/KNMI/covjson-pydantic)
+* [geojson-pydantic](https://github.com/developmentseed/geojson-pydantic)
+
 ## TODOs
 Help is wanted in the following areas to fully implement the EDR spec:
 * See TODOs in code listing various small inconsistencies in the spec
 * In various places there could be more validation on content
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: edr-pydantic Version: 0.2.0 Summary: Pydantic
+Metadata-Version: 2.1 Name: edr-pydantic Version: 0.2.1 Summary: Pydantic
 models for OGC Environmental Data (EDR) API Keywords: EDR,Pydantic Author-
 email: KNMI Data Platform Team
 knmi.nl> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -48,11 +48,13 @@
 { "label": "degree true" }, "observedProperty": { "id": "https://codes.wmo.int/
 common/quantity-kind/_windDirection", "label": "Wind Direction" } } } } ``` ##
 Contributing Make an editable install from within the repository root ```shell
 pip install -e '.[test]' ``` ### Running tests ```shell pytest tests/ ``` ##
 Real world usage This library is used to build an Environmental Data Retrieval
 (EDR) API, serving observation data from surface weather data station data from
 the KNMI. See the [KNMI Data Platform](https://developer.dataplatform.knmi.nl/
-edr-api). ## TODOs Help is wanted in the following areas to fully implement the
-EDR spec: * See TODOs in code listing various small inconsistencies in the spec
-* In various places there could be more validation on content ## License Apache
-License, Version 2.0
+edr-api). ## Related projects * [CoverageJSON Pydantic](https://github.com/
+KNMI/covjson-pydantic) * [geojson-pydantic](https://github.com/developmentseed/
+geojson-pydantic) ## TODOs Help is wanted in the following areas to fully
+implement the EDR spec: * See TODOs in code listing various small
+inconsistencies in the spec * In various places there could be more validation
+on content ## License Apache License, Version 2.0
```

