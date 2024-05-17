# Comparing `tmp/ilcdlib-4.4.0.tar.gz` & `tmp/ilcdlib-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-4.4.0.tar", max compression
+gzip compressed data, was "ilcdlib-4.5.0.tar", max compression
```

## Comparing `ilcdlib-4.4.0.tar` & `ilcdlib-4.5.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11357 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/LICENSE
--rw-r--r--   0        0        0     4949 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/README.md
--rw-r--r--   0        0        0     3525 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17587 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0      837 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/compat/__init__.py
--rw-r--r--   0        0        0     1158 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/compat/pydantic.py
--rw-r--r--   0        0        0     1835 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0     4934 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/data/category_mapping/epdnorge.csv
--rw-r--r--   0        0        0    51577 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/data/category_mapping/oekobaudat.csv
--rw-r--r--   0        0        0   172140 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     6454 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     7064 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     3361 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     4173 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     4224 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3788 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     6864 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     2170 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/epditaly.py
--rw-r--r--   0        0        0     2341 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/epdnorge.py
--rw-r--r--   0        0        0     1329 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2105 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/itb.py
--rw-r--r--   0        0        0     3876 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3644 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    35343 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2248 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7895 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0    10680 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/category.py
--rw-r--r--   0        0        0     3603 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     3524 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     6247 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1866 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0    11347 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     2755 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/soda4lca/api_client_4x.py
--rw-r--r--   0        0        0     1206 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     6465 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/LICENSE
+-rw-r--r--   0        0        0     4949 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/README.md
+-rw-r--r--   0        0        0     3525 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    19110 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0      837 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/compat/__init__.py
+-rw-r--r--   0        0        0     1158 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/compat/pydantic.py
+-rw-r--r--   0        0        0     1835 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0     4934 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/data/category_mapping/epdnorge.csv
+-rw-r--r--   0        0        0    51577 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/data/category_mapping/oekobaudat.csv
+-rw-r--r--   0        0        0   172140 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     6488 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     7064 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     3361 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     4173 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     8138 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     4224 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3788 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2024-05-02 21:52:51.036437 ilcdlib-4.5.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     6864 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     2170 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/epd/dialect/epditaly.py
+-rw-r--r--   0        0        0     2341 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/epd/dialect/epdnorge.py
+-rw-r--r--   0        0        0     1329 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2326 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/epd/dialect/itb.py
+-rw-r--r--   0        0        0     3876 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3644 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    35487 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2248 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7895 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0    10680 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/mapping/category.py
+-rw-r--r--   0        0        0     3603 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     3524 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     6247 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1866 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    11347 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     2755 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/soda4lca/api_client_4x.py
+-rw-r--r--   0        0        0     1206 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     6465 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2024-05-02 21:52:51.040437 ilcdlib-4.5.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.5.0/PKG-INFO
```

### Comparing `ilcdlib-4.4.0/LICENSE` & `ilcdlib-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/README.md` & `ilcdlib-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/pyproject.toml` & `ilcdlib-4.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "4.4.0"
+version = "4.5.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
```

### Comparing `ilcdlib-4.4.0/src/ilcdlib/__init__.py` & `ilcdlib-4.5.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/__main__.py` & `ilcdlib-4.5.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/__version__.py` & `ilcdlib-4.5.0/src/ilcdlib/__version__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/cli.py` & `ilcdlib-4.5.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/common.py` & `ilcdlib-4.5.0/src/ilcdlib/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import abc
 import datetime
 import logging
+import re
 from typing import IO, Literal, Self, Sequence, TextIO, overload
 
 from openepd.model.epd import Epd
 from openepd.model.lcia import Impacts
 from openepd.model.pcr import Pcr
 
 from ilcdlib.const import IlcdDatasetType
@@ -172,14 +173,16 @@
         return []
 
 
 class IlcdXmlReader:
     """Base class for ILCD xml readers. It provides a set of helper methods to read ILCD data from ILCD xml."""
 
     _LANG_ATTRIB_NAME = "{http://www.w3.org/XML/1998/namespace}lang"
+    _UUID_REGEX = re.compile(r"uuid=([0-9a-fA-F\-]{36})")
+    ALLOW_URI_BASED_LOOKUP: bool = False
 
     def __init__(self, data_provider: BaseIlcdMediumSpecificReader):
         self.data_provider = data_provider
         self.reference_data_providers: dict[str, BaseIlcdMediumSpecificReader] = {
             "epd_ref_data": get_ilcd_epd_reference_data_provider()
         }
         self.xml_parser = XmlParser(
@@ -196,42 +199,69 @@
                 epd2013="http://www.iai.kit.edu/EPD/2013",
                 epd2019="http://www.iai.kit.edu/EPD/2019",
                 epd2019_indata="http://www.indata.network/EPD/2019",
             )
         )
         self.__logger = logging.Logger(__name__)
 
+    def allow_uri_based_lookup(self) -> bool:
+        """Return whether URI based lookup is allowed."""
+        return self.ALLOW_URI_BASED_LOOKUP
+
     def remap_xml_ns(self, doc_ns_map: dict[str, str]) -> None:
         """Remap XML namespaces."""
         for n, url in doc_ns_map.items():
             if url and url.endswith("EPD/2019"):  # Some providers use outdated, non-standard namespace
                 self.xml_parser.xml_ns["epd2019"] = url
 
+    def get_xml_for_entity(
+        self, provider: BaseIlcdMediumSpecificReader, entity_type: str, entity_id: str, entity_version: str | None
+    ) -> T_ET.Element | None:
+        """Attempt to fetch XML for given entity details and return it if successful."""
+        if provider.entity_exists(entity_type, entity_id, entity_version):
+            with provider.get_entity_stream(entity_type, entity_id, entity_version) as stream:
+                return self.xml_parser.get_xml_tree(stream)
+        return None
+
     def get_xml_tree(
-        self, entity_type: str, entity_id: str, entity_version: str | None, *, allow_static_datasets: bool = True
+        self,
+        entity_type: str,
+        entity_id: str,
+        entity_version: str | None,
+        *,
+        entity_uri: str | None = None,
+        allow_static_datasets: bool = True,
     ) -> T_ET.Element:
         """
         Get the xml tree for the given entity.
 
         :param entity_type: The type of the entity. e.g. "process", "contact", "flow", etc.
         :param entity_id: The id of the entity, typically a GUID.
         :param entity_version: The version of the entity e.g. 12.34.56
+        :param entity_uri: The url of the entity e.g. https://epdnorway.lca-data.com/datasetdetail/flowproperty.xhtml?uuid=01846770-4cfe-4a25-8ad9-919d8d378345
         :param allow_static_datasets: whether to allow to check entity in static datasets if it doesn't
                                       exist in the given one.
         :raise: ValueError if the entity does not exist.
         """
         try:
             with self.data_provider.get_entity_stream(entity_type, entity_id, entity_version) as stream:
                 return self.xml_parser.get_xml_tree(stream)
         except ValueError:
             if allow_static_datasets:
+                uuid_from_uri = self._UUID_REGEX.search(entity_uri) if entity_uri else None
+                uuid = uuid_from_uri.group(1) if uuid_from_uri else None
                 for dataset_name, dataset_provider in self.reference_data_providers.items():
-                    if dataset_provider.entity_exists(entity_type, entity_id, entity_version):
-                        with dataset_provider.get_entity_stream(entity_type, entity_id, entity_version) as stream:
-                            return self.xml_parser.get_xml_tree(stream)
+                    xml_tree = self.get_xml_for_entity(dataset_provider, entity_type, entity_id, entity_version)
+                    if xml_tree:
+                        return xml_tree
+                    if self.allow_uri_based_lookup() and uuid:
+                        xml_tree = self.get_xml_for_entity(dataset_provider, entity_type, uuid, entity_version)
+                        if xml_tree:
+                            return xml_tree
+
         raise ValueError(f"Entity {entity_id} version {entity_version} (type: {entity_type}) does not exist.")
 
     def _preprocess_path(self, path: XmlPath) -> str:
         """Convert XPath defined in a form of tuple or string into a string representation."""
         if not isinstance(path, str):
             str_path = "/".join(path)
         else:
@@ -339,21 +369,22 @@
         """
         xpath = f"{self._preprocess_path(path)}"
         el = self.xml_parser.get_el(root, xpath)
         if el is None or el.attrib is None:
             return default_value
         ref_id = el.attrib.get("refObjectId", None)
         ref_type = el.attrib.get("type", None)
+        ref_uri = el.attrib.get("uri", None)
         if ref_id is None or ref_type is None:
             return default_value
         try:
             ref_type = IlcdDatasetType(ref_type)
         except ValueError:
             pass
-        return IlcdReference(ref_type, ref_id, entity_version=None)
+        return IlcdReference(ref_type, ref_id, entity_version=None, entity_uri=ref_uri)
 
     def _get_external_tree(self, root: T_ET.Element, path: XmlPath) -> T_ET.Element | None:
         """
         Read XML document referenced by given path and return root XML element as result.
 
         Path param must point to the reference element (xml element with refObjectId, type, [version]) attributes.
         This method will locate the reference, and then read XML stream and parse it into XML tree.
@@ -364,15 +395,21 @@
         :param path: The path to the reference element (xpath in a form of tuple or string).
         :return: XML Element or None if not found.
         """
         ref = self._get_reference(root, path)
         if ref is None:
             return None
         try:
-            return self.get_xml_tree(ref.entity_type, ref.entity_id, ref.entity_version, allow_static_datasets=True)
+            return self.get_xml_tree(
+                ref.entity_type,
+                ref.entity_id,
+                ref.entity_version,
+                entity_uri=ref.entity_uri,
+                allow_static_datasets=True,
+            )
         except ValueError as e:
             self.__logger.warning(e)
             return None
 
     def _get_external_binary(self, root: T_ET.Element, path: XmlPath) -> IO[bytes] | None:
         """
         Read binary object from element reference.
```

### Comparing `ilcdlib-4.4.0/src/ilcdlib/compat/__init__.py` & `ilcdlib-4.5.0/src/ilcdlib/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/compat/pydantic.py` & `ilcdlib-4.5.0/src/ilcdlib/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/const.py` & `ilcdlib-4.5.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/data/category_mapping/epdnorge.csv` & `ilcdlib-4.5.0/src/ilcdlib/data/category_mapping/epdnorge.csv`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/data/category_mapping/oekobaudat.csv` & `ilcdlib-4.5.0/src/ilcdlib/data/category_mapping/oekobaudat.csv`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-4.5.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/dto.py` & `ilcdlib-4.5.0/src/ilcdlib/dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 class IlcdReference(NamedTuple):
     """A reference to an ILCD entity."""
 
     entity_type: str
     entity_id: str
     entity_version: str | None
+    entity_uri: str | None = None
 
     def to_url(self, base_url: str | None) -> str:
         """Convert the reference to a URL."""
         prefix = base_url if base_url is not None else "https://unknown.tld"
         if prefix.endswith("/"):
             prefix = prefix[:-1]
         prefix = prefix.removesuffix("/resource")
```

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/category.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/contact.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/exchage.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/exchage.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/flow.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,7 +195,13 @@
             result.append(
                 IlcdFlowPropertyDto(
                     dataset_reader=self.flow_property_reader_cls(flow_prop_el, self.data_provider),
                     mean_value=self._get_float(e, ("flow:meanValue",)),
                 )
             )
         return result
+
+
+class UriBasedIlcdFlowReader(IlcdFlowReader):
+    """Read an ILCD Flow XML file with URI based lookup enabled."""
+
+    ALLOW_URI_BASED_LOOKUP: bool = True
```

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/material.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/source.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/unit.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/entity/validation.py` & `ilcdlib-4.5.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/cli.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/epditaly.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/dialect/epditaly.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/epdnorge.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/dialect/epdnorge.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/itb.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/dialect/itb.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,22 +13,28 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
+from typing import Any
+
 from ilcdlib.dto import IlcdContactInfo, OpenEpdIlcdOrg, ValidationDto
+from ilcdlib.entity.flow import UriBasedIlcdFlowReader
 from ilcdlib.epd.reader import IlcdEpdReader
 from ilcdlib.type import LangDef
 
 
 class ItbIlcdXmlEpdReader(IlcdEpdReader):
     """Reader for EPDs in the Itb specific ILCD XML format."""
 
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs, flow_reader_cls=UriBasedIlcdFlowReader)
+
     @classmethod
     def is_known_url(cls, url: str) -> bool:
         """Return whether the URL recognized as a known Itb URL."""
         return "itb" in url.lower()
 
     def get_third_party_verifier_email(self, validations: list[ValidationDto]) -> OpenEpdIlcdOrg | None:
         """
```

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/factory.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/epd/reader.py` & `ilcdlib-4.5.0/src/ilcdlib/epd/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,18 @@
         self.standard_names_to_lcia_mapper = standard_names_to_lcia_mapper
         self.validation_reader_cls = validation_reader_cls
         if epd_process_id is None:
             entities = data_provider.list_entities(IlcdDatasetType.Processes)
             self.__epd_entity_ref = entities[0]
         else:
             self.__epd_entity_ref = IlcdReference(IlcdDatasetType.Processes, epd_process_id, epd_version)
-        self.epd_el_tree = self.get_xml_tree(*self.__epd_entity_ref, allow_static_datasets=False)
+        entity_type, entity_id, entity_version, entity_uri = self.__epd_entity_ref
+        self.epd_el_tree = self.get_xml_tree(
+            entity_type, entity_id, entity_version, entity_uri=entity_uri, allow_static_datasets=False
+        )
         self.remap_xml_ns(self.epd_el_tree.nsmap)  # type: ignore
         self.post_init()
 
     def post_init(self):
         """
         Post-initialization actions, will be executed as a last step in constructor.
```

### Comparing `ilcdlib-4.4.0/src/ilcdlib/extension.py` & `ilcdlib-4.5.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/http_common.py` & `ilcdlib-4.5.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-4.5.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/mapping/category.py` & `ilcdlib-4.5.0/src/ilcdlib/mapping/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/mapping/common.py` & `ilcdlib-4.5.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-4.5.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-4.5.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-4.5.0/src/ilcdlib/mapping/impacts.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-4.5.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-4.5.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/mapping/units.py` & `ilcdlib-4.5.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-4.5.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/medium/archive.py` & `ilcdlib-4.5.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-4.5.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/reference_data.py` & `ilcdlib-4.5.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-4.5.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-4.5.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-4.5.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/sanitizing/text.py` & `ilcdlib-4.5.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-4.5.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-4.5.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/soda4lca/api_client_4x.py` & `ilcdlib-4.5.0/src/ilcdlib/soda4lca/api_client_4x.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/type.py` & `ilcdlib-4.5.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/utils.py` & `ilcdlib-4.5.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/src/ilcdlib/xml_parser.py` & `ilcdlib-4.5.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.4.0/PKG-INFO` & `ilcdlib-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 4.4.0
+Version: 4.5.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 4.4.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 4.5.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

