# Comparing `tmp/apache_airflow_providers_tabular-1.5.1.tar.gz` & `tmp/apache_airflow_providers_tabular-1.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_tabular-1.5.1.tar", last modified: Sat May 11 18:09:29 2024, max compression
+gzip compressed data, was "apache_airflow_providers_tabular-1.5.1rc1.tar", last modified: Sat May 11 18:09:29 2024, max compression
```

## Comparing `apache_airflow_providers_tabular-1.5.1.tar` & `apache_airflow_providers_tabular-1.5.1rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4281 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1/README.rst
--rw-r--r--   0        0        0    13569 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/LICENSE
--rw-r--r--   0        0        0     1494 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/__init__.py
--rw-r--r--   0        0        0     1995 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/hooks/__init__.py
--rw-r--r--   0        0        0     1259 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/hooks/tabular.py
--rw-r--r--   0        0        0     3090 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     6109 1970-01-01 00:00:00.000000 apache_airflow_providers_tabular-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     4285 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/LICENSE
+-rw-r--r--   0        0        0     1494 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/__init__.py
+-rw-r--r--   0        0        0     1995 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/hooks/__init__.py
+-rw-r--r--   0        0        0     1259 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/hooks/tabular.py
+-rw-r--r--   0        0        0     3097 2024-05-11 18:09:29.000000 apache_airflow_providers_tabular-1.5.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     6119 1970-01-01 00:00:00.000000 apache_airflow_providers_tabular-1.5.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_tabular-1.5.1/README.rst` & `apache_airflow_providers_tabular-1.5.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-tabular``
 
-Release: ``1.5.1``
+Release: ``1.5.1.rc1``
 
 
 `Tabular <https://tabular.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/LICENSE` & `apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/__init__.py` & `apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/get_provider_info.py` & `apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/hooks/__init__.py` & `apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tabular-1.5.1/airflow/providers/tabular/hooks/tabular.py` & `apache_airflow_providers_tabular-1.5.1rc1/airflow/providers/tabular/hooks/tabular.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tabular-1.5.1/pyproject.toml` & `apache_airflow_providers_tabular-1.5.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-tabular"
-version = "1.5.1"
+version = "1.5.1.rc1"
 description = "Provider package apache-airflow-providers-tabular for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -53,15 +53,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
     "apache-airflow-providers-apache-iceberg",
-    "apache-airflow>=2.7.0",
+    "apache-airflow>=2.7.0rc0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.1"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_tabular-1.5.1/PKG-INFO` & `apache_airflow_providers_tabular-1.5.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-tabular
-Version: 1.5.1
+Version: 1.5.1rc1
 Summary: Provider package apache-airflow-providers-tabular for Apache Airflow
 Keywords: airflow-provider,tabular,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow-providers-apache-iceberg
-Requires-Dist: apache-airflow>=2.7.0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: apache-airflow-providers-apache-iceberg ; extra == "apache.iceberg"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.1/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -73,15 +73,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-tabular``
 
-Release: ``1.5.1``
+Release: ``1.5.1.rc1``
 
 
 `Tabular <https://tabular.io/>`__
 
 
 Provider package
 ----------------
```

