# Comparing `tmp/domaintools_api_v2-2.0.1.tar.gz` & `tmp/domaintools_api_v2-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domaintools_api_v2-2.0.1.tar", last modified: Thu May  9 16:27:06 2024, max compression
+gzip compressed data, was "domaintools_api_v2-2.0.2.tar", last modified: Fri May 17 14:56:38 2024, max compression
```

## Comparing `domaintools_api_v2-2.0.1.tar` & `domaintools_api_v2-2.0.2.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.547258 domaintools_api_v2-2.0.1/
--rw-r--r--   0 bluza      (502) staff       (20)     1078 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/LICENSE
--rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-09 16:27:06.547105 domaintools_api_v2-2.0.1/PKG-INFO
--rw-r--r--   0 bluza      (502) staff       (20)     7230 2024-03-04 18:03:36.000000 domaintools_api_v2-2.0.1/README.md
--rw-r--r--   0 bluza      (502) staff       (20)        5 2024-05-09 16:24:56.000000 domaintools_api_v2-2.0.1/VERSION
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.536625 domaintools_api_v2-2.0.1/domaintools/
--rw-r--r--   0 bluza      (502) staff       (20)      135 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     1181 2024-05-09 16:26:19.000000 domaintools_api_v2-2.0.1/domaintools/_version.py
--rw-r--r--   0 bluza      (502) staff       (20)    43189 2024-05-07 11:17:06.000000 domaintools_api_v2-2.0.1/domaintools/api.py
--rw-r--r--   0 bluza      (502) staff       (20)     8893 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/domaintools/base_results.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.538453 domaintools_api_v2-2.0.1/domaintools/cli/
--rw-r--r--   0 bluza      (502) staff       (20)      141 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     7819 2024-05-02 12:32:44.000000 domaintools_api_v2-2.0.1/domaintools/cli/api.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.541683 domaintools_api_v2-2.0.1/domaintools/cli/commands/
--rw-r--r--   0 bluza      (502) staff       (20)      133 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     2823 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/accounts.py
--rw-r--r--   0 bluza      (502) staff       (20)    18505 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/detects.py
--rw-r--r--   0 bluza      (502) staff       (20)    23368 2024-04-29 16:18:47.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/domains.py
--rw-r--r--   0 bluza      (502) staff       (20)     6835 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/ips.py
--rw-r--r--   0 bluza      (502) staff       (20)     6452 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/iris.py
--rw-r--r--   0 bluza      (502) staff       (20)     3315 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/phisheye.py
--rw-r--r--   0 bluza      (502) staff       (20)     1266 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/constants.py
--rw-r--r--   0 bluza      (502) staff       (20)      519 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/main.py
--rw-r--r--   0 bluza      (502) staff       (20)     6050 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.1/domaintools/cli/utils.py
--rw-r--r--   0 bluza      (502) staff       (20)      687 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/domaintools/exceptions.py
--rw-r--r--   0 bluza      (502) staff       (20)     5216 2024-05-07 12:07:39.000000 domaintools_api_v2-2.0.1/domaintools/filters.py
--rw-r--r--   0 bluza      (502) staff       (20)     3674 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/domaintools/results.py
--rw-r--r--   0 bluza      (502) staff       (20)     5811 2024-05-03 13:55:31.000000 domaintools_api_v2-2.0.1/domaintools/utils.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.546645 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/
--rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/PKG-INFO
--rw-r--r--   0 bluza      (502) staff       (20)     1006 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/SOURCES.txt
--rw-r--r--   0 bluza      (502) staff       (20)        1 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/dependency_links.txt
--rw-r--r--   0 bluza      (502) staff       (20)       52 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/entry_points.txt
--rw-r--r--   0 bluza      (502) staff       (20)       37 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/requires.txt
--rw-r--r--   0 bluza      (502) staff       (20)       30 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/top_level.txt
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.542822 domaintools_api_v2-2.0.1/domaintools_async/
--rw-r--r--   0 bluza      (502) staff       (20)     3015 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/domaintools_async/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     1453 2024-05-02 12:32:47.000000 domaintools_api_v2-2.0.1/pyproject.toml
--rw-r--r--   0 bluza      (502) staff       (20)      172 2024-05-09 16:27:06.547521 domaintools_api_v2-2.0.1/setup.cfg
--rwxr-xr-x   0 bluza      (502) staff       (20)     1541 2024-04-11 04:41:30.000000 domaintools_api_v2-2.0.1/setup.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.545570 domaintools_api_v2-2.0.1/tests/
--rw-r--r--   0 bluza      (502) staff       (20)    15279 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/tests/test_api.py
--rw-r--r--   0 bluza      (502) staff       (20)     1760 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/tests/test_async.py
--rw-r--r--   0 bluza      (502) staff       (20)     1045 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/tests/test_cli.py
--rw-r--r--   0 bluza      (502) staff       (20)     3004 2024-05-07 12:07:01.000000 domaintools_api_v2-2.0.1/tests/test_filters.py
--rw-r--r--   0 bluza      (502) staff       (20)     4055 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/tests/test_utils.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.670730 domaintools_api_v2-2.0.2/
+-rw-r--r--   0 bluza      (502) staff       (20)     1078 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/LICENSE
+-rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-17 14:56:38.670505 domaintools_api_v2-2.0.2/PKG-INFO
+-rw-r--r--   0 bluza      (502) staff       (20)     7230 2024-03-04 18:03:36.000000 domaintools_api_v2-2.0.2/README.md
+-rw-r--r--   0 bluza      (502) staff       (20)        5 2024-05-17 14:55:43.000000 domaintools_api_v2-2.0.2/VERSION
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.661265 domaintools_api_v2-2.0.2/domaintools/
+-rw-r--r--   0 bluza      (502) staff       (20)      135 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1181 2024-05-17 14:55:47.000000 domaintools_api_v2-2.0.2/domaintools/_version.py
+-rw-r--r--   0 bluza      (502) staff       (20)    40580 2024-05-17 14:15:19.000000 domaintools_api_v2-2.0.2/domaintools/api.py
+-rw-r--r--   0 bluza      (502) staff       (20)     8893 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/domaintools/base_results.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.664267 domaintools_api_v2-2.0.2/domaintools/cli/
+-rw-r--r--   0 bluza      (502) staff       (20)      141 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     7717 2024-05-17 14:55:21.000000 domaintools_api_v2-2.0.2/domaintools/cli/api.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.666942 domaintools_api_v2-2.0.2/domaintools/cli/commands/
+-rw-r--r--   0 bluza      (502) staff       (20)      133 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     2822 2024-05-17 14:30:51.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/accounts.py
+-rw-r--r--   0 bluza      (502) staff       (20)    18505 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/detects.py
+-rw-r--r--   0 bluza      (502) staff       (20)    23368 2024-04-29 16:18:47.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/domains.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6835 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/ips.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6452 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/iris.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3315 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/phisheye.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1266 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/constants.py
+-rw-r--r--   0 bluza      (502) staff       (20)      513 2024-05-17 14:34:04.000000 domaintools_api_v2-2.0.2/domaintools/cli/main.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6050 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.2/domaintools/cli/utils.py
+-rw-r--r--   0 bluza      (502) staff       (20)      687 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/domaintools/exceptions.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3674 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/domaintools/results.py
+-rw-r--r--   0 bluza      (502) staff       (20)     5619 2024-05-17 14:15:19.000000 domaintools_api_v2-2.0.2/domaintools/utils.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.669870 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/
+-rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/PKG-INFO
+-rw-r--r--   0 bluza      (502) staff       (20)      961 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 bluza      (502) staff       (20)        1 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       52 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/entry_points.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       37 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/requires.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       30 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/top_level.txt
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.668049 domaintools_api_v2-2.0.2/domaintools_async/
+-rw-r--r--   0 bluza      (502) staff       (20)     3015 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/domaintools_async/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1453 2024-05-17 14:15:46.000000 domaintools_api_v2-2.0.2/pyproject.toml
+-rw-r--r--   0 bluza      (502) staff       (20)      172 2024-05-17 14:56:38.671049 domaintools_api_v2-2.0.2/setup.cfg
+-rwxr-xr-x   0 bluza      (502) staff       (20)     1541 2024-04-11 04:41:30.000000 domaintools_api_v2-2.0.2/setup.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.669078 domaintools_api_v2-2.0.2/tests/
+-rw-r--r--   0 bluza      (502) staff       (20)    15279 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/tests/test_api.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1760 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/tests/test_async.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1045 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/tests/test_cli.py
+-rw-r--r--   0 bluza      (502) staff       (20)     4055 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/tests/test_utils.py
```

### Comparing `domaintools_api_v2-2.0.1/LICENSE` & `domaintools_api_v2-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/PKG-INFO` & `domaintools_api_v2-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domaintools_api_v2
-Version: 2.0.1
+Version: 2.0.2
 Summary: DomainTools Official Python API
 Author-email: DomainTools <integrations@domaintools.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 DomainTools
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.1 Summary:
+Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.2 Summary:
 DomainTools Official Python API Author-email: DomainTools
 domaintools.com> License: The MIT License (MIT) Copyright (c) 2016 DomainTools
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `domaintools_api_v2-2.0.1/README.md` & `domaintools_api_v2-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/_version.py` & `domaintools_api_v2-2.0.2/domaintools/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
 
-current = "2.0.1"
+current = "2.0.2"
```

### Comparing `domaintools_api_v2-2.0.1/domaintools/api.py` & `domaintools_api_v2-2.0.2/domaintools/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,14 @@
 from hashlib import sha1, sha256, md5
 from hmac import new as hmac
 from types import MethodType
 import re
 
 from domaintools._version import current as version
 from domaintools.results import GroupedIterable, ParsedWhois, Reputation, Results
-from domaintools.filters import (
-    filter_by_riskscore,
-    filter_by_expire_date,
-    filter_by_date_updated_after,
-    filter_by_field,
-    DTResultFilter,
-)
 
 AVAILABLE_KEY_SIGN_HASHES = ["sha1", "sha256", "md5"]
 
 
 def delimited(items, character="|"):
     """Returns a character delimited version of the provided list as a Python string"""
     return character.join(items) if type(items) in (list, tuple, set) else items
@@ -552,55 +545,23 @@
             raise ValueError("One or more domains to enrich must be provided")
 
         domains = ",".join(domains)
         data_updated_after = kwargs.get("data_updated_after", None)
         if hasattr(data_updated_after, "strftime"):
             data_updated_after = data_updated_after.strftime("%Y-%m-%d")
 
-        results = self._results(
+        return self._results(
             "iris-enrich",
             "/v1/iris-enrich/",
             domain=domains,
             data_updated_after=data_updated_after,
             items_path=("results",),
             **kwargs,
         )
 
-        risk_score = kwargs.pop("risk_score", {}) or None
-        younger_than_date = kwargs.pop("younger_than_date", {}) or None
-        older_than_date = kwargs.pop("older_than_date", {}) or None
-        updated_after = kwargs.pop("updated_after", {}) or None
-        include_domains_with_missing_field = (
-            kwargs.pop("include_domains_with_missing_field", {}) or None
-        )
-        exclude_domains_with_missing_field = (
-            kwargs.pop("exclude_domains_with_missing_field", {}) or None
-        )
-
-        filtered_results = DTResultFilter(result_set=results).by(
-            [
-                filter_by_riskscore(threshold=risk_score),
-                filter_by_expire_date(date=younger_than_date, lookup_type="before"),
-                filter_by_expire_date(date=older_than_date, lookup_type="after"),
-                filter_by_date_updated_after(date=updated_after),
-                filter_by_field(
-                    field=include_domains_with_missing_field, filter_type="include"
-                ),
-                filter_by_field(
-                    field=exclude_domains_with_missing_field, filter_type="exclude"
-                ),
-            ]
-        )
-
-        results["results"] = filtered_results
-        results["results_count"] = len(filtered_results)
-        results["total_count"] = len(filtered_results)
-
-        return results
-
     def iris_enrich_cli(self, domains=None, **kwargs):
         """Returns back enriched data related to the specified domains using our Iris Enrich service.
          This is a CLI version of the iris_enrich method to help maintain backwards compatibility.
 
         api.iris_enrich(['domaintools.com', 'google.com'])
 
         api.iris_enrich(DOMAIN_LIST)['results_count'] Returns the number of results
@@ -636,20 +597,14 @@
         self,
         domains=None,
         data_updated_after=None,
         expiration_date=None,
         create_date=None,
         active=None,
         search_hash=None,
-        risk_score=None,
-        younger_than_date=None,
-        older_than_date=None,
-        updated_after=None,
-        include_domains_with_missing_field=None,
-        exclude_domains_with_missing_field=None,
         **kwargs,
     ):
         """Returns back a list of domains based on the provided filters.
         The following filters are available beyond what is parameterized as kwargs:
 
             - ip: Search for domains having this IP.
             - email: Search for domains with this email in their data.
@@ -703,46 +658,25 @@
         if hasattr(expiration_date, "strftime"):
             expiration_date = expiration_date.strftime("%Y-%m-%d")
         if hasattr(create_date, "strftime"):
             create_date = create_date.strftime("%Y-%m-%d")
         if isinstance(active, bool):
             kwargs["active"] = str(active).lower()
 
-        results = self._results(
+        return self._results(
             "iris-investigate",
             "/v1/iris-investigate/",
             domain=domains,
             data_updated_after=data_updated_after,
             expiration_date=expiration_date,
             create_date=create_date,
             items_path=("results",),
             **kwargs,
         )
 
-        filtered_results = DTResultFilter(result_set=results).by(
-            [
-                filter_by_riskscore(threshold=risk_score),
-                filter_by_expire_date(date=younger_than_date, lookup_type="before"),
-                filter_by_expire_date(date=older_than_date, lookup_type="after"),
-                filter_by_date_updated_after(date=updated_after),
-                filter_by_field(
-                    field=include_domains_with_missing_field, filter_type="include"
-                ),
-                filter_by_field(
-                    field=exclude_domains_with_missing_field, filter_type="exclude"
-                ),
-            ]
-        )
-
-        results["results"] = filtered_results
-        results["results_count"] = len(filtered_results)
-        results["total_count"] = len(filtered_results)
-
-        return results
-
     def iris_detect_monitors(
         self,
         include_counts=False,
         datetime_counts_since=None,
         sort=None,
         order="desc",
         offset=0,
```

### Comparing `domaintools_api_v2-2.0.1/domaintools/base_results.py` & `domaintools_api_v2-2.0.2/domaintools/base_results.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/cli/api.py` & `domaintools_api_v2-2.0.2/domaintools/cli/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional, Dict, Tuple
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich import print
 
 from domaintools.api import API
 from domaintools.exceptions import ServiceException
 from domaintools.cli.utils import get_file_extension
+from domaintools.cli import constants
 
 
 class DTCLICommand:
     API_SUCCESS_STATUS = 200
     APP_PARTNER_NAME = "python_wrapper_cli_2.0.0"
 
     @staticmethod
@@ -89,21 +90,17 @@
             else response.as_list()
         )
 
     @classmethod
     def _get_credentials(cls, params: Optional[Dict] = {}) -> Tuple[str]:
         user = params.pop("user")
         key = params.pop("key")
+        creds_file = params.pop("creds_file", {}) or ""
 
         if not user or not key:
-            creds_file = params.pop("creds_file") or ""
-            typer.echo(
-                f"No user or key parameter given. Using credentials in {creds_file} instead."
-            )
-
             try:
                 if "~" in creds_file:
                     # expand user path if path uses "~".
                     creds_file = os.path.expanduser(creds_file)
 
                 with open(creds_file, "r") as cf:
                     user, key = cf.readline().strip(), cf.readline().strip()
@@ -159,39 +156,40 @@
                 domains = cls._get_domains_from_source(source=source)
                 if params["domains"]:
                     # append to existing domain parameter if found
                     params["domains"] = params["domains"] + "," + domains
                 else:
                     params["domains"] = domains
 
-            typer.echo(f"Using api credentials with a username of: {user}")
-
             with Progress(
                 SpinnerColumn(),
                 TextColumn("[progress.description]{task.description}"),
                 transient=True,
             ) as progress:
 
                 progress.add_task(
-                    description=f"Executing [green]{name}[/green] api call..."
+                    description=f"Using api credentials with a username of: [cyan]{user}[/cyan]\nExecuting [green]{name}[/green] api call...",
+                    total=None,
                 )
 
                 dt_api = API(
                     user,
                     key,
                     app_name=cls.APP_PARTNER_NAME,
                     verify_ssl=verify_ssl,
                     rate_limit=rate_limit,
                 )
+                dt_api_func = getattr(dt_api, name)
 
                 params = params | kwargs
-                response = getattr(dt_api, name)(**params)
+
+                response = dt_api_func(**params)
                 progress.add_task(
                     description=f"Preparing results with format of {response_format}...",
-                    total=0,
+                    total=None,
                 )
 
                 output = cls._get_formatted_output(
                     cmd_name=name, response=response, out_format=response_format
                 )
 
                 if isinstance(out_file, _io.TextIOWrapper):
@@ -199,15 +197,14 @@
                     print(output)
                 else:
                     # if it's a file then write
                     out_file.write(output if output.endswith("\n") else output + "\n")
                 time.sleep(0.5)
 
             name = typer.style(name, fg=typer.colors.CYAN, bold=True)
-            typer.echo(f"Done fetching results from `{name}` command.")
         except Exception as e:
             if isinstance(e, ServiceException):
                 code = typer.style(getattr(e, "code", 400), fg=typer.colors.BRIGHT_RED)
                 _reason = getattr(e, "reason", {})
                 # check data type first as some of the reasons is just plain text
                 if isinstance(_reason, dict):
                     _reason = (
```

### Comparing `domaintools_api_v2-2.0.1/domaintools/cli/commands/accounts.py` & `domaintools_api_v2-2.0.2/domaintools/cli/commands/accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,12 +79,11 @@
     ),
     no_verify_ssl: bool = typer.Option(
         False,
         "--no-verify-ssl",
         help="Skip verification of SSL certificate when making HTTPs API calls",
     ),
 ):
-
     DTCLICommand.run(name=c.AVAILABLE_API_CALLS, params=ctx.params)
 
 
 __all__ = ["account_information", "available_api_calls"]
```

### Comparing `domaintools_api_v2-2.0.1/domaintools/cli/commands/detects.py` & `domaintools_api_v2-2.0.2/domaintools/cli/commands/detects.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/cli/commands/domains.py` & `domaintools_api_v2-2.0.2/domaintools/cli/commands/domains.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/cli/commands/ips.py` & `domaintools_api_v2-2.0.2/domaintools/cli/commands/ips.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/cli/commands/iris.py` & `domaintools_api_v2-2.0.2/domaintools/cli/commands/iris.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/cli/commands/phisheye.py` & `domaintools_api_v2-2.0.2/domaintools/cli/commands/phisheye.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/cli/constants.py` & `domaintools_api_v2-2.0.2/domaintools/cli/constants.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/cli/utils.py` & `domaintools_api_v2-2.0.2/domaintools/cli/utils.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/exceptions.py` & `domaintools_api_v2-2.0.2/domaintools/exceptions.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/results.py` & `domaintools_api_v2-2.0.2/domaintools/results.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/domaintools/utils.py` & `domaintools_api_v2-2.0.2/domaintools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 from datetime import datetime
-
-from typing import Optional
-
 import re
 
 
 def get_domain_age(create_date):
     """
     Finds how many days old a domain is given a start date.
     Args:
@@ -169,13 +166,7 @@
                 elif isinstance(temp_data, tuple):
                     return_data.append([name[1:].upper().replace("_", " "), temp_data])
     count -= 1
     if count:
         return
     else:
         return return_data
-
-
-def convert_str_to_dateobj(
-    string_date: str, date_format: Optional[str] = "%Y-%m-%d"
-) -> datetime:
-    return datetime.strptime(string_date, date_format)
```

### Comparing `domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/PKG-INFO` & `domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domaintools_api_v2
-Version: 2.0.1
+Version: 2.0.2
 Summary: DomainTools Official Python API
 Author-email: DomainTools <integrations@domaintools.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 DomainTools
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.1 Summary:
+Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.2 Summary:
 DomainTools Official Python API Author-email: DomainTools
 domaintools.com> License: The MIT License (MIT) Copyright (c) 2016 DomainTools
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/SOURCES.txt` & `domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 setup.cfg
 setup.py
 domaintools/__init__.py
 domaintools/_version.py
 domaintools/api.py
 domaintools/base_results.py
 domaintools/exceptions.py
-domaintools/filters.py
 domaintools/results.py
 domaintools/utils.py
 domaintools/cli/__init__.py
 domaintools/cli/api.py
 domaintools/cli/constants.py
 domaintools/cli/main.py
 domaintools/cli/utils.py
@@ -30,9 +29,8 @@
 domaintools_api_v2.egg-info/entry_points.txt
 domaintools_api_v2.egg-info/requires.txt
 domaintools_api_v2.egg-info/top_level.txt
 domaintools_async/__init__.py
 tests/test_api.py
 tests/test_async.py
 tests/test_cli.py
-tests/test_filters.py
 tests/test_utils.py
```

### Comparing `domaintools_api_v2-2.0.1/domaintools_async/__init__.py` & `domaintools_api_v2-2.0.2/domaintools_async/__init__.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/pyproject.toml` & `domaintools_api_v2-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/setup.py` & `domaintools_api_v2-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/tests/test_api.py` & `domaintools_api_v2-2.0.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/tests/test_async.py` & `domaintools_api_v2-2.0.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/tests/test_cli.py` & `domaintools_api_v2-2.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.1/tests/test_utils.py` & `domaintools_api_v2-2.0.2/tests/test_utils.py`

 * *Files identical despite different names*

