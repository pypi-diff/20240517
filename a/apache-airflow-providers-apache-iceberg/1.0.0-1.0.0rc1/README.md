# Comparing `tmp/apache_airflow_providers_apache_iceberg-1.0.0.tar.gz` & `tmp/apache_airflow_providers_apache_iceberg-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_iceberg-1.0.0.tar", last modified: Fri May 10 23:40:02 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apache_iceberg-1.0.0rc1.tar", last modified: Fri May 10 23:40:02 2024, max compression
```

## Comparing `apache_airflow_providers_apache_iceberg-1.0.0.tar` & `apache_airflow_providers_apache_iceberg-1.0.0rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3069 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0/README.rst
--rw-r--r--   0        0        0    13569 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/LICENSE
--rw-r--r--   0        0        0     1501 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/__init__.py
--rw-r--r--   0        0        0     2147 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/hooks/__init__.py
--rw-r--r--   0        0        0     3208 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/hooks/iceberg.py
--rw-r--r--   0        0        0     2990 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_iceberg-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3073 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/LICENSE
+-rw-r--r--   0        0        0     1501 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/__init__.py
+-rw-r--r--   0        0        0     2147 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/hooks/__init__.py
+-rw-r--r--   0        0        0     3208 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/hooks/iceberg.py
+-rw-r--r--   0        0        0     2997 2024-05-10 23:40:02.000000 apache_airflow_providers_apache_iceberg-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_iceberg-1.0.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_apache_iceberg-1.0.0/README.rst` & `apache_airflow_providers_apache_iceberg-1.0.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-iceberg``
 
-Release: ``1.0.0``
+Release: ``1.0.0.rc1``
 
 
 `Iceberg <https://iceberg.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/LICENSE` & `apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/__init__.py` & `apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/get_provider_info.py` & `apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/hooks/__init__.py` & `apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_iceberg-1.0.0/airflow/providers/apache/iceberg/hooks/iceberg.py` & `apache_airflow_providers_apache_iceberg-1.0.0rc1/airflow/providers/apache/iceberg/hooks/iceberg.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_iceberg-1.0.0/pyproject.toml` & `apache_airflow_providers_apache_iceberg-1.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apache-iceberg"
-version = "1.0.0"
+version = "1.0.0.rc1"
 description = "Provider package apache-airflow-providers-apache-iceberg for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,15 +52,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.7.0",
+    "apache-airflow>=2.7.0rc0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-iceberg/1.0.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-iceberg/1.0.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_apache_iceberg-1.0.0/PKG-INFO` & `apache_airflow_providers_apache_iceberg-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-iceberg
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Provider package apache-airflow-providers-apache-iceberg for Apache Airflow
 Keywords: airflow-provider,apache.iceberg,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.7.0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-iceberg/1.0.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-iceberg/1.0.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
@@ -70,15 +70,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-iceberg``
 
-Release: ``1.0.0``
+Release: ``1.0.0.rc1``
 
 
 `Iceberg <https://iceberg.apache.org/>`__
 
 
 Provider package
 ----------------
```

