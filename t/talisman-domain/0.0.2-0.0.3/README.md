# Comparing `tmp/talisman-domain-0.0.2.tar.gz` & `tmp/talisman-domain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talisman-domain-0.0.2.tar", last modified: Fri Mar 29 10:53:38 2024, max compression
+gzip compressed data, was "talisman-domain-0.0.3.tar", last modified: Fri May 17 11:49:04 2024, max compression
```

## Comparing `talisman-domain-0.0.2.tar` & `talisman-domain-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:53:38.209053 talisman-domain-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      623 2024-03-29 10:53:38.205053 talisman-domain-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 10:53:31.000000 talisman-domain-0.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-03-28 13:58:37.000000 talisman-domain-0.0.2/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-29 10:53:38.209053 talisman-domain-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1451 2024-03-28 12:55:31.000000 talisman-domain-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:53:38.205053 talisman-domain-0.0.2/talisman_domain.egg-info/
--rw-r--r--   0 root         (0) root         (0)      623 2024-03-29 10:53:38.000000 talisman-domain-0.0.2/talisman_domain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1166 2024-03-29 10:53:38.000000 talisman-domain-0.0.2/talisman_domain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 10:53:38.000000 talisman-domain-0.0.2/talisman_domain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-03-29 10:53:38.000000 talisman-domain-0.0.2/talisman_domain.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      232 2024-03-29 10:53:38.000000 talisman-domain-0.0.2/talisman_domain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-29 10:53:38.000000 talisman-domain-0.0.2/talisman_domain.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:53:38.205053 talisman-domain-0.0.2/tie_domain/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:53:38.205053 talisman-domain-0.0.2/tie_domain/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 10:53:31.000000 talisman-domain-0.0.2/tie_domain/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/_queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:53:38.205053 talisman-domain-0.0.2/tie_domain/domain/_synthetic/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/_synthetic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1663 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/_synthetic/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     7526 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/producer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:53:38.205053 talisman-domain-0.0.2/tie_domain/domain/updates_manager/
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/updates_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/updates_manager/_abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/updates_manager/_ask.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/updates_manager/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/updates_manager/_never.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/updates_manager/_queries.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/domain/updates_manager/_timeout.py
--rw-rw-rw-   0 root         (0) root         (0)    11102 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:53:38.205053 talisman-domain-0.0.2/tie_domain/talisman_api/
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/talisman_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/talisman_api/_queries.py
--rw-rw-rw-   0 root         (0) root         (0)     3275 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/talisman_api/api_adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     2036 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/talisman_api/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:53:38.205053 talisman-domain-0.0.2/tie_domain/talisman_api/gql_clients/
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/talisman_api/gql_clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1729 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/talisman_api/gql_clients/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/talisman_api/gql_clients/keycloak.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-03-26 14:16:12.000000 talisman-domain-0.0.2/tie_domain/talisman_api/gql_clients/noauth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 11:49:04.445987 talisman-domain-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      623 2024-05-17 11:49:04.445987 talisman-domain-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 11:48:39.000000 talisman-domain-0.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-05-17 11:41:26.000000 talisman-domain-0.0.3/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 11:49:04.445987 talisman-domain-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-05-17 11:41:26.000000 talisman-domain-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 11:49:04.437987 talisman-domain-0.0.3/talisman_domain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      623 2024-05-17 11:49:04.000000 talisman-domain-0.0.3/talisman_domain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1166 2024-05-17 11:49:04.000000 talisman-domain-0.0.3/talisman_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 11:49:04.000000 talisman-domain-0.0.3/talisman_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-17 11:49:04.000000 talisman-domain-0.0.3/talisman_domain.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-17 11:49:04.000000 talisman-domain-0.0.3/talisman_domain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-17 11:49:04.000000 talisman-domain-0.0.3/talisman_domain.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 11:49:04.437987 talisman-domain-0.0.3/tie_domain/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 11:49:04.441987 talisman-domain-0.0.3/tie_domain/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 11:48:39.000000 talisman-domain-0.0.3/tie_domain/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/_queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 11:49:04.441987 talisman-domain-0.0.3/tie_domain/domain/_synthetic/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/_synthetic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/_synthetic/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     7685 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/producer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 11:49:04.441987 talisman-domain-0.0.3/tie_domain/domain/updates_manager/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/updates_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/updates_manager/_abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/updates_manager/_ask.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/updates_manager/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/updates_manager/_never.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/updates_manager/_queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/domain/updates_manager/_timeout.py
+-rw-rw-rw-   0 root         (0) root         (0)    11102 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 11:49:04.445987 talisman-domain-0.0.3/tie_domain/talisman_api/
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/talisman_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/talisman_api/_queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     3803 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/talisman_api/api_adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/talisman_api/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 11:49:04.445987 talisman-domain-0.0.3/tie_domain/talisman_api/gql_clients/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/talisman_api/gql_clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/talisman_api/gql_clients/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     3619 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/talisman_api/gql_clients/keycloak.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-17 09:35:12.000000 talisman-domain-0.0.3/tie_domain/talisman_api/gql_clients/noauth.py
```

### Comparing `talisman-domain-0.0.2/PKG-INFO` & `talisman-domain-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-domain
-Version: 0.0.2
+Version: 0.0.3
 Summary: Talisman domain implementations
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-domain-0.0.2/setup.py` & `talisman-domain-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description_content_type="text/markdown",
     author='ISPRAS Talisman NLP team',
     author_email='modis@ispras.ru',
     maintainer='Vladimir Mayorov',
     maintainer_email='vmayorov@ispras.ru',
     packages=find_packages(include=['tie_domain', 'tie_domain.*']),
     install_requires=[
-        'talisman-interfaces~=0.5.3', 'talisman-dm~=1.0.0a34',
+        'talisman-interfaces~=0.5.6', 'talisman-dm~=1.0.0a34',
         'aiohttp~=3.8.4', 'aiohttp-retry~=2.8.3', 'aiorwlock~=1.3.0',
         'fastapi>=0.73.0', 'pydantic~=1.10.4', 'gql~=3.4.0', 'graphql-core~=3.2.3',
         'requests~=2.31.0', 'python-keycloak~=2.16.2', 'typing_extensions~=4.8.0'
 
     ],
     entry_points={
         'talisman.plugins': ['domain = tie_domain']
```

### Comparing `talisman-domain-0.0.2/talisman_domain.egg-info/PKG-INFO` & `talisman-domain-0.0.3/talisman_domain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-domain
-Version: 0.0.2
+Version: 0.0.3
 Summary: Talisman domain implementations
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-domain-0.0.2/talisman_domain.egg-info/SOURCES.txt` & `talisman-domain-0.0.3/talisman_domain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talisman-domain-0.0.2/tie_domain/domain/_queries.py` & `talisman-domain-0.0.3/tie_domain/domain/_queries.py`

 * *Files identical despite different names*

### Comparing `talisman-domain-0.0.2/tie_domain/domain/_synthetic/platform.py` & `talisman-domain-0.0.3/tie_domain/domain/_synthetic/platform.py`

 * *Files identical despite different names*

### Comparing `talisman-domain-0.0.2/tie_domain/domain/producer.py` & `talisman-domain-0.0.3/tie_domain/domain/producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+import logging
 import os
 from typing import Dict, Iterable, Type, TypeVar
 
 from tdm.abstract.datamodel import AbstractDomainType
 from tdm.datamodel.domain import Domain
 from tdm.datamodel.values import DateTimeValue, DoubleValue, GeoPointValue, IntValue, LinkValue, StringValue, TimestampValue
 
@@ -10,14 +11,17 @@
                                         property_types)
 from tie_domain.domain.updates_manager import AbstractDomainUpdatesManager, MANAGERS
 from tie_domain.talisman_api import GQLClientConfig, TalismanAPIAdapter
 from tp_interfaces.domain.hooks import DOMAIN_CHANGE_HOOKS
 from tp_interfaces.domain.interfaces import AbstractDomainChangeHook, DomainProducer
 from tp_interfaces.domain.model.types import AtomValueType, ComponentValueType, CompositeValueType, ConceptType, DocumentType, \
     IdentifyingPropertyType, PropertyType, RelationPropertyType, RelationType
+from tp_interfaces.logging.time import log_time
+
+logger = logging.getLogger(__name__)
 
 _SYNTHETIC_TYPES = bool(os.getenv('SYNTHETIC_TYPES', True))
 
 
 class ValueTypes(enum.Enum):
     Date = DateTimeValue
     Double = DoubleValue
@@ -51,17 +55,19 @@
         await self._updates_manager.__aenter__()
         return self
 
     async def __aexit__(self, *exc):
         await self._updates_manager.__aexit__(*exc)
         await self._adapter.__aexit__(*exc)
 
+    @log_time(logger=logger)
     async def has_changed(self) -> bool:
         return await self._updates_manager.has_changed
 
+    @log_time(logger=logger)
     async def _get_domain(self) -> Domain:
         await self._updates_manager.update()  # first we notify manager, that we reload domain
 
         def make_dictionary(obj) -> dict:
             ret = obj
             ret["dictionary"] = ret.get("list_names_dictionary", []) + ret.get("list_white_dictionary", [])
             return ret
```

### Comparing `talisman-domain-0.0.2/tie_domain/domain/updates_manager/_ask.py` & `talisman-domain-0.0.3/tie_domain/domain/updates_manager/_ask.py`

 * *Files identical despite different names*

### Comparing `talisman-domain-0.0.2/tie_domain/domain/updates_manager/_configuration.py` & `talisman-domain-0.0.3/tie_domain/domain/updates_manager/_configuration.py`

 * *Files identical despite different names*

### Comparing `talisman-domain-0.0.2/tie_domain/domain/updates_manager/_timeout.py` & `talisman-domain-0.0.3/tie_domain/domain/updates_manager/_timeout.py`

 * *Files identical despite different names*

### Comparing `talisman-domain-0.0.2/tie_domain/helper.py` & `talisman-domain-0.0.3/tie_domain/helper.py`

 * *Files identical despite different names*

### Comparing `talisman-domain-0.0.2/tie_domain/talisman_api/api_adapter.py` & `talisman-domain-0.0.3/tie_domain/talisman_api/api_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 from contextlib import AbstractAsyncContextManager
 from enum import Enum
 from typing import Dict, NamedTuple, Optional
 
 from gql import gql
-from graphql import DocumentNode
+from graphql import DocumentNode, print_ast
 from requests import Timeout
 
+from tp_interfaces.logging.time import AsyncTimeMeasurer, log_time
 from ._queries import get_pagination_query
 from .gql_clients import AsyncAbstractGQLClient, AsyncKeycloakAwareGQLClient, AsyncNoAuthGQLClient
 
 logger = logging.getLogger(__name__)
 
 
 class APISchema(str, Enum):
@@ -18,15 +19,15 @@
     KB_UTILS = "kbutils"
 
 
 class GQLClientConfig(NamedTuple):
     uri: str
     auth: bool = False
     timeout: int = 60
-    concurrency_limit: int = 10
+    concurrency_limit: int = 30
 
     def configure(self) -> AsyncAbstractGQLClient:
         if self.auth:
             return AsyncKeycloakAwareGQLClient(self.uri, self.timeout, self.concurrency_limit)
         return AsyncNoAuthGQLClient(self.uri, self.timeout, self.concurrency_limit)
 
 
@@ -42,31 +43,40 @@
         return self
 
     async def __aexit__(self, exc_type=None, exc_val=None, exc_tb=None):
         await self._gql_client.__aexit__(exc_type, exc_val, exc_tb)
 
         self._gql_client = None
 
+    @log_time(logger=logger)
     async def pagination_query(self, pagination: str, list_query: str) -> Dict:
-        ret = await self.gql_call(gql(get_pagination_query(pagination, list_query, 0)))
+        query = gql(get_pagination_query(pagination, list_query, 0))
+        async with AsyncTimeMeasurer(
+                f"{pagination} total query {id(query)}", inline_time=True, logger=logger, warning_threshold=1, extra={"query_id": id(query)}
+        ):
+            ret = await self.gql_call(query)
         total = list(ret.values())[0]['total']
-        return await self.gql_call(gql(get_pagination_query(pagination, list_query, total)))
+        query = gql(get_pagination_query(pagination, list_query, total))
+        async with AsyncTimeMeasurer(
+                f"{pagination} {total} items query {id(query)}", inline_time=True, logger=logger, extra={"query_id": id(query)}
+        ):
+            return await self.gql_call(query)
 
     async def gql_call(self, gql_operation: DocumentNode, variables: Optional[dict] = None, raise_on_timeout: bool = True):
         try:
             return await self._gql_client.execute(gql_operation, variables=variables)
 
         except Timeout as e:
             logger.error('Timeout while query processing', exc_info=e,
-                         extra={'query': gql_operation.to_dict(), 'variables': str(variables)})
+                         extra={'query': print_ast(gql_operation), 'variables': str(variables)})
             if raise_on_timeout:
                 raise e
         except Exception as e:
             logger.error('Some exception was occured during query processing.', exc_info=e,
-                         extra={'query': gql_operation.to_dict(), 'variables': str(variables)})
+                         extra={'query': print_ast(gql_operation), 'variables': str(variables)})
             raise e
 
 
 class CompositeAdapter(AbstractAsyncContextManager):
     def __init__(self, gql_uris: Dict[str, GQLClientConfig]):
         self._gql_uris = {APISchema(key): TalismanAPIAdapter(value) for key, value in gql_uris.items()}
         self._gql_clients: Optional[Dict[APISchema, TalismanAPIAdapter]] = None
```

### Comparing `talisman-domain-0.0.2/tie_domain/talisman_api/document.py` & `talisman-domain-0.0.3/tie_domain/talisman_api/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,33 @@
 
 import requests
 from aiohttp_retry import ExponentialRetry, RetryClient
 from fastapi.encoders import jsonable_encoder
 from pydantic import BaseModel
 from tdm import TalismanDocument, TalismanDocumentModel
 
+from tp_interfaces.logging.time import log_time
+
 logger = logging.getLogger(__name__)
 
 
 class LoadDocumentResponse(BaseModel):
     id: str
 
 
 class TalismanDocumentsAPIAdapter(AbstractAsyncContextManager):
     def __init__(self, loader_uri: str):
         self._loader_uri = loader_uri
         env_timeout = os.getenv('LOADER_TIMEOUT', None)
         self._timeout = float(env_timeout) if env_timeout is not None else None
 
+    @log_time(logger=logger, title="Talisman documents adapter initialization")
     async def __aenter__(self):
         self._client = RetryClient(
+            logger=logger,
             retry_options=ExponentialRetry(
                 attempts=os.getenv('LOADER_RETRIES', 3),
                 factor=os.getenv('LOADER_BACKOFF', 2)
             )
         )
         return self
```

### Comparing `talisman-domain-0.0.2/tie_domain/talisman_api/gql_clients/abstract.py` & `talisman-domain-0.0.3/tie_domain/talisman_api/gql_clients/abstract.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,40 +6,48 @@
 
 from aiorwlock import RWLock
 from gql import Client
 from gql.client import AsyncClientSession
 from gql.transport.aiohttp import AIOHTTPTransport, log as aiohttp_logger
 from gql.transport.requests import log as requests_logger
 
+from tp_interfaces.logging.time import AsyncTimeMeasurer
+
 requests_logger.setLevel(logging.WARNING)
 aiohttp_logger.setLevel(logging.ERROR)
 
+logger = logging.getLogger(__name__)
+
 
 class AsyncAbstractGQLClient(AbstractAsyncContextManager, metaclass=ABCMeta):
 
     def __init__(self, gql_uri: str, timeout: int = 60, concurrency_limit: int = 10):
         self._gql_uri = gql_uri
         self._timeout = timeout
         self._client: Optional[Client] = None
         self._session: Optional[AsyncClientSession] = None
 
         self._sema = Semaphore(concurrency_limit)
         self._rw_lock = RWLock()
 
     async def execute(self, query, variables=None, operation_name=None, extra_headers=None, timeout=None):
         async with self._sema, self._rw_lock.reader_lock:
-            return await self._session.execute(query, variables, operation_name)
+            async with AsyncTimeMeasurer(
+                    f"query {id(query)}", inline_time=True, logger=logger, extra={"query_id": id(query)}, warning_threshold=5000
+            ):
+                return await self._session.execute(query, variables, operation_name)
 
     async def _configure_session(self, headers: dict = None):
         async with self._rw_lock.writer_lock:
             await self._close_session()
 
             transport = AIOHTTPTransport(url=self._gql_uri, headers=headers)
             self._client = Client(transport=transport, fetch_schema_from_transport=True, execute_timeout=self._timeout)
 
-            self._session = await self._client.connect_async(reconnecting=True)
+            # here we could change default behaviour of query retrying: just change retry_execute to backoff decorator
+            self._session = await self._client.connect_async(reconnecting=True, retry_execute=True)
 
     async def _close_session(self):
         if self._session is not None:
             await self._client.close_async()
         self._session = None
         self._client = None
```

### Comparing `talisman-domain-0.0.2/tie_domain/talisman_api/gql_clients/keycloak.py` & `talisman-domain-0.0.3/tie_domain/talisman_api/gql_clients/keycloak.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 import logging
 import os
 import time
 from asyncio import Lock
 from typing import Optional
 
 from keycloak import KeycloakOpenID
+from urllib3.util.retry import log
 
+from tp_interfaces.logging.time import TimeMeasurer
 from .abstract import AsyncAbstractGQLClient
 
 logger = logging.getLogger(__name__)
+log.setLevel(logging.INFO)
 
 
 class AuthEnvs(enum.Enum):
     AUTH_URL = "KEYCLOAK_AUTH_URL"
     REALM = "KEYCLOAK_REALM"
     CLIENT_ID = "KEYCLOAK_CLIENT_ID"
     CLIENT_KEY = "KEYCLOAK_CLIENT_KEY"
@@ -48,19 +51,19 @@
     async def _ensure_session_liveness(self):
         offsetted_time = time.time() + self._TIME_OFFSET
         if offsetted_time < self._access_expiration_timestamp:
             return
 
         time_before_req = time.time()
         if offsetted_time < self._refresh_expiration_timestamp and self._refresh_token is not None:
-            logger.info("refreshing access token with refresh token")
-            token_info = self._keycloak_openid.refresh_token(self._refresh_token)
+            with TimeMeasurer("refreshing access token with refresh token", logger=logger):
+                token_info = self._keycloak_openid.refresh_token(self._refresh_token)
         else:
-            logger.info("refreshing access token with credentials")
-            token_info = self._keycloak_openid.token(self._auth[AuthEnvs.USER], self._auth[AuthEnvs.PWD])
+            with TimeMeasurer("refreshing access token with credentials", logger=logger):
+                token_info = self._keycloak_openid.token(self._auth[AuthEnvs.USER], self._auth[AuthEnvs.PWD])
 
         self._access_token = token_info['access_token']
         self._access_expiration_timestamp = time_before_req + token_info['expires_in']
         self._refresh_token = token_info['refresh_token']
         self._refresh_expiration_timestamp = time_before_req + token_info['refresh_expires_in']
 
         headers = {"X-Auth-Token": self._access_token, "Authorization": f"Bearer {self._access_token}"}
```

