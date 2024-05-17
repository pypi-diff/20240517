# Comparing `tmp/ckanext-vocabularies-0.0.7.tar.gz` & `tmp/ckanext-vocabularies-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-vocabularies-0.0.7.tar", last modified: Wed Jun  7 10:01:16 2023, max compression
+gzip compressed data, was "ckanext-vocabularies-0.0.8.tar", last modified: Fri May 17 08:53:45 2024, max compression
```

## Comparing `ckanext-vocabularies-0.0.7.tar` & `ckanext-vocabularies-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/
--rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)    34500 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/LICENSE
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      209 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/MANIFEST.in
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4411 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/PKG-INFO
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3730 2023-06-07 09:54:08.000000 ckanext-vocabularies-0.0.7/README.md
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/
--rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)      219 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/__init__.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/
--rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/__init__.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/assets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      335 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/assets/webassets.yml
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      734 2022-05-04 12:37:14.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/blueprints.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2022-05-03 12:07:07.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3087 2022-05-05 15:35:58.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/idsapi.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4650 2022-12-15 08:00:30.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/resourceapi.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     7006 2023-06-07 09:54:08.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/subscribe.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1535 2022-04-22 07:36:30.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/subscriptionapi.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     6285 2023-06-07 09:55:42.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/helpers.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      795 2022-05-04 12:35:14.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/logic.py
--rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)     2496 2022-05-05 05:51:21.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/plugin.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      827 2022-03-22 13:04:43.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/base.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.842673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/scheming/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/scheming/form_snippets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1392 2022-03-22 13:20:59.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/scheming/form_snippets/autocomplete_dropdown.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/tests/
--rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/tests/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1262 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/tests/test_plugin.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4411 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/PKG-INFO
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      961 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/SOURCES.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        1 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/dependency_links.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      169 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/entry_points.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/namespace_packages.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/top_level.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)       77 2023-06-07 09:54:08.000000 ckanext-vocabularies-0.0.7/requirements.txt
--rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)      613 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/setup.cfg
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3882 2023-06-07 09:54:08.000000 ckanext-vocabularies-0.0.7/setup.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    34500 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/LICENSE
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      209 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/MANIFEST.in
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4391 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/PKG-INFO
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3730 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/README.md
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.602450 ckanext-vocabularies-0.0.8/ckanext/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      219 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/__init__.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/ckanext/vocabularies/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/__init__.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/ckanext/vocabularies/assets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      335 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/assets/webassets.yml
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      734 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/blueprints.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3087 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/idsapi.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4650 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/resourceapi.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     7201 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/subscribe.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1535 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/subscriptionapi.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     6306 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/helpers.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      845 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/logic.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2620 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/plugin.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/ckanext/vocabularies/templates/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      827 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/templates/base.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.602450 ckanext-vocabularies-0.0.8/ckanext/vocabularies/templates/scheming/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/ckanext/vocabularies/templates/scheming/form_snippets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1392 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/templates/scheming/form_snippets/autocomplete_dropdown.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/ckanext/vocabularies/tests/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/tests/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1262 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/ckanext/vocabularies/tests/test_plugin.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/ckanext_vocabularies.egg-info/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4391 2024-05-17 08:53:45.000000 ckanext-vocabularies-0.0.8/ckanext_vocabularies.egg-info/PKG-INFO
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      961 2024-05-17 08:53:45.000000 ckanext-vocabularies-0.0.8/ckanext_vocabularies.egg-info/SOURCES.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        1 2024-05-17 08:53:45.000000 ckanext-vocabularies-0.0.8/ckanext_vocabularies.egg-info/dependency_links.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      134 2024-05-17 08:53:45.000000 ckanext-vocabularies-0.0.8/ckanext_vocabularies.egg-info/entry_points.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2024-05-17 08:53:45.000000 ckanext-vocabularies-0.0.8/ckanext_vocabularies.egg-info/namespace_packages.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2024-05-17 08:53:45.000000 ckanext-vocabularies-0.0.8/ckanext_vocabularies.egg-info/top_level.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)       77 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/requirements.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      613 2024-05-17 08:53:45.606450 ckanext-vocabularies-0.0.8/setup.cfg
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3882 2023-11-09 07:27:15.000000 ckanext-vocabularies-0.0.8/setup.py
```

### Comparing `ckanext-vocabularies-0.0.7/LICENSE` & `ckanext-vocabularies-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/PKG-INFO` & `ckanext-vocabularies-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ckanext-vocabularies
-Version: 0.0.7
+Version: 0.0.8
 Summary: Getting choices options for the scheming choise type of field, based on SKOS vocabulary served on a remote SPARQL endpoint
 Home-page: https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies
 Author: Sotirios Karampatakis
 Author-email: sotiris.karampatakis@semantic-web.com
 License: AGPL
 Keywords: CKAN vocabularies SKOS scheming
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies/workflows/Tests/badge.svg?branch=main)](https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies/actions)
@@ -141,9 +140,7 @@
 ## Funding
 This code was created as part of project TRUSTS: Trusted secure data sharing space.
 
 This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement [No 871481](https://cordis.europa.eu/project/id/871481).
 
 
 
-
-
```

### Comparing `ckanext-vocabularies-0.0.7/README.md` & `ckanext-vocabularies-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/blueprints.py` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/blueprints.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/idsapi.py` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/idsapi.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/resourceapi.py` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/resourceapi.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/subscribe.py` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/subscribe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 
 import ckan.plugins.toolkit as toolkit
 
 import pathlib
-from ckanext.ids.model import IdsResource, IdsAgreement, IdsSubscription
 from urllib.parse import urlparse
 from ckanext.vocabularies.dsc.resourceapi import ResourceApi
 from ckanext.vocabularies.dsc.subscriptionapi import SubscriptionApi
 from ckanext.vocabularies.dsc.idsapi import IdsApi
 
 log = logging.getLogger("ckanext.vocabularies.dsc.subscribe")
 # TODO: too hacky, fix this
@@ -45,14 +44,18 @@
 
         consumer = IdsApi(consumerUrl, auth=(username, password))
         local_node = toolkit.config.get("ckanext.ids.trusts_local_dataspace_connector_url")
 
     # IDS
     # Call description
     def make_agreement(self):
+        try:
+            from ckanext.ids.model import IdsResource, IdsAgreement
+        except ModuleNotFoundError:
+            return
         log.info("Making agreement...")
         offer = consumer.descriptionRequest(self.provider_alias + "/api/ids/data", self.offer_url)
         log.debug(offer)
         artifact = offer["ids:representation"][0]["ids:instance"][0]['@id']
         self.remote_artifact = artifact
         log.debug(artifact)
         ## Check if an agreement already exists
@@ -92,14 +95,18 @@
         data = consumerResources.get_data(first_artifact).text
         log.info("Data acquired successfully!")
         #log.debug(data)
         return data
 # Consumer
 
     def subscribe(self):
+        try:
+            from ckanext.ids.model import IdsAgreement, IdsSubscription
+        except ImportError:
+            return
         self.create_data_source()
         self.create_endpoint()
         self.link_endpoint_data_source()
         self.create_route()
         self.link_endpoint_route()
         local_agreement = IdsAgreement.get(self.agreement_url)
         consumerResources = ResourceApi(consumerUrl)
```

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/subscriptionapi.py` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/dsc/subscriptionapi.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/helpers.py` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,17 @@
             select ?concept ?prefLabel (GROUP_CONCAT(?broaderPrefLabel;SEPARATOR="|") as ?path) (count(?broader) as ?counter) 
             where {
                 ?concept a skos:Concept ;
                          skos:prefLabel ?prefLabel .
                 %(in_scheme_triple)s         
                 OPTIONAL { ?concept skos:broader+ ?broader .
                            ?broader skos:prefLabel ?broaderPrefLabel .
+                           FILTER (langMatches( lang(?broaderPrefLabel), "%(lang)s"))
                         }
-                FILTER ( langMatches( lang(?prefLabel), "%(lang)s") && langMatches( lang(?broaderPrefLabel), "%(lang)s"))       
+                FILTER ( langMatches( lang(?prefLabel), "%(lang)s"))       
                 }
                 group by ?concept ?prefLabel
             """%dict(in_scheme_triple=in_scheme_triple, lang=lang)
 
 
 def query_poolparty(sparql_endpoint, query):
     response = requests.post(sparql_endpoint, data={"query": query, "format": "application/json"}, headers={ "Content-Type": "application/x-www-form-urlencoded"}).content.decode("utf-8")
@@ -94,15 +95,15 @@
 
         graph.parse(data=data, format="text/turtle")
         graphs[dsc_resource] = graph
     results = json.loads(graph.query(query).serialize(format='json'))
     return results
 
 def query_local_resource(local_resource, query):
-    graph_id = uuid.uuid4(local_resource)
+    graph_id = local_resource
     if graph_id in graphs:
         graph = graphs[graph_id]
         log.debug('Graph exists in triplestore...querying')
     else:
         log.warn('Graph does not exist on triplestore...adding triples')
         graph = Graph()
         graph.parse(local_resource, format="text/turtle")
```

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/logic.py` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/logic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import logging
-from ckanext.ids.model import IdsResource, IdsAgreement
 from ckanext.vocabularies.dsc.subscribe import Subscription
 from ckanext.vocabularies.helpers import graphs
 from rdflib import Graph
 
 log = logging.getLogger("ckanext.vocabularies.logic")
 
 
 def update_vocabulary_dsc(dsc_resource):
+    try:
+        from ckanext.ids.model import IdsResource
+    except ModuleNotFoundError:
+        return
     local_resource = IdsResource.get(dsc_resource)
     local_agreement = local_resource.get_agreements()[0]
     log.info("Found the agreement url:" + local_agreement.id)
     subscription = Subscription(dsc_resource, None)
     subscription.agreement_url = local_agreement.id
     data = subscription.consume_resource()
     graph = Graph()
```

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/plugin.py` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,19 @@
     def update_config(self, config_):
         toolkit.add_template_directory(config_, 'templates')
         toolkit.add_public_directory(config_, 'public')
         toolkit.add_resource('assets',
             'vocabularies')
         SQLALCHEMY_URL = toolkit.config.get('sqlalchemy.url').replace("postgresql", "postgresql+psycopg2")
         toolkit.config.store.update({'ckanext.vocabularies.triplestore': SQLALCHEMY_URL})
-        self.find_or_create_dsc_user()
+        try:
+            from ckanext.ids.model import IdsResource
+            self.find_or_create_dsc_user()
+        except ModuleNotFoundError:
+            pass
 
     # Declare that this plugin will implement ITemplateHelpers.
     plugins.implements(plugins.ITemplateHelpers)
 
     def get_helpers(self):
         '''Register the skos_vocabulary_helper() function as a template
         helper function.
```

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/base.html` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/templates/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/scheming/form_snippets/autocomplete_dropdown.html` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/templates/scheming/form_snippets/autocomplete_dropdown.html`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/ckanext/vocabularies/tests/test_plugin.py` & `ckanext-vocabularies-0.0.8/ckanext/vocabularies/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/PKG-INFO` & `ckanext-vocabularies-0.0.8/ckanext_vocabularies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ckanext-vocabularies
-Version: 0.0.7
+Version: 0.0.8
 Summary: Getting choices options for the scheming choise type of field, based on SKOS vocabulary served on a remote SPARQL endpoint
 Home-page: https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies
 Author: Sotirios Karampatakis
 Author-email: sotiris.karampatakis@semantic-web.com
 License: AGPL
 Keywords: CKAN vocabularies SKOS scheming
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies/workflows/Tests/badge.svg?branch=main)](https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies/actions)
@@ -141,9 +140,7 @@
 ## Funding
 This code was created as part of project TRUSTS: Trusted secure data sharing space.
 
 This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement [No 871481](https://cordis.europa.eu/project/id/871481).
 
 
 
-
-
```

### Comparing `ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/SOURCES.txt` & `ckanext-vocabularies-0.0.8/ckanext_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/setup.cfg` & `ckanext-vocabularies-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.7/setup.py` & `ckanext-vocabularies-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='''ckanext-vocabularies''',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='0.0.7',
+    version='0.0.8',
 
     description='''Getting choices options for the scheming choise type of field, based on SKOS vocabulary served on a remote SPARQL endpoint''',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies',
```

