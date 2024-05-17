# Comparing `tmp/chainmeta-0.0.4.tar.gz` & `tmp/chainmeta-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainmeta-0.0.4.tar", last modified: Mon Apr 29 03:33:14 2024, max compression
+gzip compressed data, was "chainmeta-0.0.5.tar", last modified: Fri May 17 02:34:48 2024, max compression
```

## Comparing `chainmeta-0.0.4.tar` & `chainmeta-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.578966 chainmeta-0.0.4/
--rw-r--r--   0 zhanwu     (501) staff       (20)    11357 2024-04-10 07:26:37.000000 chainmeta-0.0.4/LICENSE
--rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-04-29 03:33:14.578775 chainmeta-0.0.4/PKG-INFO
--rw-r--r--   0 zhanwu     (501) staff       (20)      988 2024-04-10 07:26:37.000000 chainmeta-0.0.4/README.md
--rw-r--r--   0 zhanwu     (501) staff       (20)      784 2024-04-29 03:32:06.000000 chainmeta-0.0.4/pyproject.toml
--rw-r--r--   0 zhanwu     (501) staff       (20)       38 2024-04-29 03:33:14.579009 chainmeta-0.0.4/setup.cfg
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.574494 chainmeta-0.0.4/src/
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.576075 chainmeta-0.0.4/src/chainmeta/
--rw-r--r--   0 zhanwu     (501) staff       (20)     4925 2024-04-29 02:33:52.000000 chainmeta-0.0.4/src/chainmeta/__init__.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     2746 2024-04-29 03:06:44.000000 chainmeta-0.0.4/src/chainmeta/artifact.py
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.577264 chainmeta-0.0.4/src/chainmeta/config/
--rw-r--r--   0 zhanwu     (501) staff       (20)     3510 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/__init__.py
--rw-r--r--   0 zhanwu     (501) staff       (20)    20519 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/categories.json
--rw-r--r--   0 zhanwu     (501) staff       (20)     2679 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/chains.json
--rw-r--r--   0 zhanwu     (501) staff       (20)    43396 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/entities.json
--rw-r--r--   0 zhanwu     (501) staff       (20)      404 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/sources.json
--rw-r--r--   0 zhanwu     (501) staff       (20)      979 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/constants.py
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.577724 chainmeta-0.0.4/src/chainmeta/contrib/
--rw-r--r--   0 zhanwu     (501) staff       (20)     4529 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/contrib/chaintool.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     1342 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/contrib/chaintool_schema.json
--rw-r--r--   0 zhanwu     (501) staff       (20)     1293 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/contrib/messari.py
--rw-r--r--   0 zhanwu     (501) staff       (20)      423 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/contrib/messari_schema.json
--rw-r--r--   0 zhanwu     (501) staff       (20)    15594 2024-04-29 03:32:06.000000 chainmeta-0.0.4/src/chainmeta/db.py
--rw-r--r--   0 zhanwu     (501) staff       (20)      664 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/logger.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     1979 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/metadata.py
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.578081 chainmeta-0.0.4/src/chainmeta/schema/
--rw-r--r--   0 zhanwu     (501) staff       (20)     2743 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/schema/__init__.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     3320 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/schema/artifact_schema.json
--rw-r--r--   0 zhanwu     (501) staff       (20)     4124 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/schema/meta_schema.json
--rw-r--r--   0 zhanwu     (501) staff       (20)     2332 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/validator.py
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.578587 chainmeta-0.0.4/src/chainmeta.egg-info/
--rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/PKG-INFO
--rw-r--r--   0 zhanwu     (501) staff       (20)      901 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/SOURCES.txt
--rw-r--r--   0 zhanwu     (501) staff       (20)        1 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/dependency_links.txt
--rw-r--r--   0 zhanwu     (501) staff       (20)       45 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/requires.txt
--rw-r--r--   0 zhanwu     (501) staff       (20)       10 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/top_level.txt
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.578430 chainmeta-0.0.4/tests/
--rw-r--r--   0 zhanwu     (501) staff       (20)      715 2024-04-10 07:26:37.000000 chainmeta-0.0.4/tests/test_config.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     1738 2024-04-10 07:26:37.000000 chainmeta-0.0.4/tests/test_translator.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     1600 2024-04-10 07:26:37.000000 chainmeta-0.0.4/tests/test_validator.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-05-17 02:34:48.900417 chainmeta-0.0.5/
+-rw-r--r--   0 zhanwu     (501) staff       (20)    11357 2024-04-10 07:26:37.000000 chainmeta-0.0.5/LICENSE
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-05-17 02:34:48.900226 chainmeta-0.0.5/PKG-INFO
+-rw-r--r--   0 zhanwu     (501) staff       (20)      988 2024-04-10 07:26:37.000000 chainmeta-0.0.5/README.md
+-rw-r--r--   0 zhanwu     (501) staff       (20)      784 2024-05-17 02:22:13.000000 chainmeta-0.0.5/pyproject.toml
+-rw-r--r--   0 zhanwu     (501) staff       (20)       38 2024-05-17 02:34:48.900478 chainmeta-0.0.5/setup.cfg
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-05-17 02:34:48.894773 chainmeta-0.0.5/src/
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-05-17 02:34:48.896571 chainmeta-0.0.5/src/chainmeta/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     4925 2024-04-29 02:33:52.000000 chainmeta-0.0.5/src/chainmeta/__init__.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2746 2024-04-29 03:06:44.000000 chainmeta-0.0.5/src/chainmeta/artifact.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-05-17 02:34:48.898246 chainmeta-0.0.5/src/chainmeta/config/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     3510 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/config/__init__.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)    20519 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/config/categories.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2679 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/config/chains.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)    43396 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/config/entities.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)      404 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/config/sources.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)      979 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/constants.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-05-17 02:34:48.898865 chainmeta-0.0.5/src/chainmeta/contrib/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     4529 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/contrib/chaintool.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1342 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/contrib/chaintool_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1293 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/contrib/messari.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)      423 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/contrib/messari_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)    15594 2024-04-29 03:32:06.000000 chainmeta-0.0.5/src/chainmeta/db.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)      664 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/logger.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2129 2024-05-17 02:33:37.000000 chainmeta-0.0.5/src/chainmeta/metadata.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-05-17 02:34:48.899340 chainmeta-0.0.5/src/chainmeta/schema/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2743 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/schema/__init__.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     3320 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/schema/artifact_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     4124 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/schema/meta_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2332 2024-04-10 07:26:37.000000 chainmeta-0.0.5/src/chainmeta/validator.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-05-17 02:34:48.899979 chainmeta-0.0.5/src/chainmeta.egg-info/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-05-17 02:34:48.000000 chainmeta-0.0.5/src/chainmeta.egg-info/PKG-INFO
+-rw-r--r--   0 zhanwu     (501) staff       (20)      901 2024-05-17 02:34:48.000000 chainmeta-0.0.5/src/chainmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanwu     (501) staff       (20)        1 2024-05-17 02:34:48.000000 chainmeta-0.0.5/src/chainmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanwu     (501) staff       (20)       45 2024-05-17 02:34:48.000000 chainmeta-0.0.5/src/chainmeta.egg-info/requires.txt
+-rw-r--r--   0 zhanwu     (501) staff       (20)       10 2024-05-17 02:34:48.000000 chainmeta-0.0.5/src/chainmeta.egg-info/top_level.txt
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-05-17 02:34:48.899797 chainmeta-0.0.5/tests/
+-rw-r--r--   0 zhanwu     (501) staff       (20)      715 2024-04-10 07:26:37.000000 chainmeta-0.0.5/tests/test_config.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1738 2024-04-10 07:26:37.000000 chainmeta-0.0.5/tests/test_translator.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1600 2024-04-10 07:26:37.000000 chainmeta-0.0.5/tests/test_validator.py
```

### Comparing `chainmeta-0.0.4/LICENSE` & `chainmeta-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/PKG-INFO` & `chainmeta-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainmeta
-Version: 0.0.4
+Version: 0.0.5
 Summary: Onchain metadata exchange protocol
 Project-URL: Homepage, https://github.com/microscopexyz/chainmeta-core
 Project-URL: Issues, https://github.com/microscopexyz/chainmeta-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `chainmeta-0.0.4/README.md` & `chainmeta-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/pyproject.toml` & `chainmeta-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chainmeta"
-version = "0.0.4"
+version = "0.0.5"
 authors = []
 description = "Onchain metadata exchange protocol"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chainmeta-0.0.4/src/chainmeta/__init__.py` & `chainmeta-0.0.5/src/chainmeta/__init__.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/artifact.py` & `chainmeta-0.0.5/src/chainmeta/artifact.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/config/__init__.py` & `chainmeta-0.0.5/src/chainmeta/config/__init__.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/config/categories.json` & `chainmeta-0.0.5/src/chainmeta/config/categories.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/config/chains.json` & `chainmeta-0.0.5/src/chainmeta/config/chains.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/config/entities.json` & `chainmeta-0.0.5/src/chainmeta/config/entities.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/constants.py` & `chainmeta-0.0.5/src/chainmeta/constants.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/contrib/chaintool.py` & `chainmeta-0.0.5/src/chainmeta/contrib/chaintool.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/contrib/chaintool_schema.json` & `chainmeta-0.0.5/src/chainmeta/contrib/chaintool_schema.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/contrib/messari.py` & `chainmeta-0.0.5/src/chainmeta/contrib/messari.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/db.py` & `chainmeta-0.0.5/src/chainmeta/db.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/logger.py` & `chainmeta-0.0.5/src/chainmeta/logger.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/metadata.py` & `chainmeta-0.0.5/src/chainmeta/metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import ast
 from abc import ABC
 from dataclasses import dataclass
 from typing import List, Optional
 
 
 @dataclass
 class ChainmetaItem:
@@ -45,14 +46,18 @@
 
     # Last updated time
     submitted_on: str
 
     # Additional metadata
     additional_metadata: dict
 
+    def __post_init__(self):
+        if isinstance(self.categories, str):
+            self.categories = ast.literal_eval(self.categories)
+
 
 class ITranslator(ABC):
     def to_common_schema(self, raw_metadata) -> Optional[ChainmetaItem]:
         pass
 
     def from_common_schema(
         self, common_schema_metadata: ChainmetaItem
```

### Comparing `chainmeta-0.0.4/src/chainmeta/schema/__init__.py` & `chainmeta-0.0.5/src/chainmeta/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/schema/artifact_schema.json` & `chainmeta-0.0.5/src/chainmeta/schema/artifact_schema.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/schema/meta_schema.json` & `chainmeta-0.0.5/src/chainmeta/schema/meta_schema.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta/validator.py` & `chainmeta-0.0.5/src/chainmeta/validator.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/src/chainmeta.egg-info/PKG-INFO` & `chainmeta-0.0.5/src/chainmeta.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainmeta
-Version: 0.0.4
+Version: 0.0.5
 Summary: Onchain metadata exchange protocol
 Project-URL: Homepage, https://github.com/microscopexyz/chainmeta-core
 Project-URL: Issues, https://github.com/microscopexyz/chainmeta-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `chainmeta-0.0.4/src/chainmeta.egg-info/SOURCES.txt` & `chainmeta-0.0.5/src/chainmeta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/tests/test_config.py` & `chainmeta-0.0.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/tests/test_translator.py` & `chainmeta-0.0.5/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.4/tests/test_validator.py` & `chainmeta-0.0.5/tests/test_validator.py`

 * *Files identical despite different names*

