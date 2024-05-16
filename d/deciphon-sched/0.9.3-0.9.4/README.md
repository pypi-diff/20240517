# Comparing `tmp/deciphon_sched-0.9.3.tar.gz` & `tmp/deciphon_sched-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_sched-0.9.3.tar", max compression
+gzip compressed data, was "deciphon_sched-0.9.4.tar", max compression
```

## Comparing `deciphon_sched-0.9.3.tar` & `deciphon_sched-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1063 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/LICENSE
--rw-r--r--   0        0        0      345 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/README.md
--rw-r--r--   0        0        0        0 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/__init__.py
--rw-r--r--   0        0        0     1077 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/cli.py
--rw-r--r--   0        0        0      793 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/database.py
--rw-r--r--   0        0        0     1523 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/errors.py
--rw-r--r--   0        0        0      760 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/journal.py
--rw-r--r--   0        0        0      299 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/logger.py
--rw-r--r--   0        0        0     1548 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/main.py
--rw-r--r--   0        0        0      533 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/sched/__init__.py
--rw-r--r--   0        0        0     3395 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/sched/dbs.py
--rw-r--r--   0        0        0     3597 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/sched/hmms.py
--rw-r--r--   0        0        0     1681 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/sched/jobs.py
--rw-r--r--   0        0        0     9146 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/sched/models.py
--rw-r--r--   0        0        0     6874 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/sched/scans.py
--rw-r--r--   0        0        0     3476 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/sched/schemas.py
--rw-r--r--   0        0        0      926 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/sched/seqs.py
--rw-r--r--   0        0        0      964 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/settings.py
--rw-r--r--   0        0        0     2599 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/storage.py
--rw-r--r--   0        0        0     1548 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/deciphon_sched/testing.py
--rw-r--r--   0        0        0     1285 2023-10-20 10:27:45.545047 deciphon_sched-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 deciphon_sched-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/LICENSE
+-rw-r--r--   0        0        0      345 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/README.md
+-rw-r--r--   0        0        0        0 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/__init__.py
+-rw-r--r--   0        0        0     1077 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/cli.py
+-rw-r--r--   0        0        0      793 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/database.py
+-rw-r--r--   0        0        0     1523 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/errors.py
+-rw-r--r--   0        0        0      760 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/journal.py
+-rw-r--r--   0        0        0      299 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/logger.py
+-rw-r--r--   0        0        0     1548 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/main.py
+-rw-r--r--   0        0        0      533 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/sched/__init__.py
+-rw-r--r--   0        0        0     3395 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/sched/dbs.py
+-rw-r--r--   0        0        0     3597 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/sched/hmms.py
+-rw-r--r--   0        0        0     1681 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/sched/jobs.py
+-rw-r--r--   0        0        0     9146 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/sched/models.py
+-rw-r--r--   0        0        0     6874 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/sched/scans.py
+-rw-r--r--   0        0        0     3476 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/sched/schemas.py
+-rw-r--r--   0        0        0      926 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/sched/seqs.py
+-rw-r--r--   0        0        0      964 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/settings.py
+-rw-r--r--   0        0        0     2599 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/storage.py
+-rw-r--r--   0        0        0     1548 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/deciphon_sched/testing.py
+-rw-r--r--   0        0        0     1285 2023-10-20 10:35:05.613038 deciphon_sched-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 deciphon_sched-0.9.4/PKG-INFO
```

### Comparing `deciphon_sched-0.9.3/LICENSE` & `deciphon_sched-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/cli.py` & `deciphon_sched-0.9.4/deciphon_sched/cli.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/database.py` & `deciphon_sched-0.9.4/deciphon_sched/database.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/errors.py` & `deciphon_sched-0.9.4/deciphon_sched/errors.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/journal.py` & `deciphon_sched-0.9.4/deciphon_sched/journal.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/main.py` & `deciphon_sched-0.9.4/deciphon_sched/main.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/sched/__init__.py` & `deciphon_sched-0.9.4/deciphon_sched/sched/__init__.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/sched/dbs.py` & `deciphon_sched-0.9.4/deciphon_sched/sched/dbs.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/sched/hmms.py` & `deciphon_sched-0.9.4/deciphon_sched/sched/hmms.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/sched/jobs.py` & `deciphon_sched-0.9.4/deciphon_sched/sched/jobs.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/sched/models.py` & `deciphon_sched-0.9.4/deciphon_sched/sched/models.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/sched/scans.py` & `deciphon_sched-0.9.4/deciphon_sched/sched/scans.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/sched/schemas.py` & `deciphon_sched-0.9.4/deciphon_sched/sched/schemas.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/sched/seqs.py` & `deciphon_sched-0.9.4/deciphon_sched/sched/seqs.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/settings.py` & `deciphon_sched-0.9.4/deciphon_sched/settings.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/storage.py` & `deciphon_sched-0.9.4/deciphon_sched/storage.py`

 * *Files identical despite different names*

### Comparing `deciphon_sched-0.9.3/deciphon_sched/testing.py` & `deciphon_sched-0.9.4/deciphon_sched/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,14 @@
         self.port = port
         self.with_exposed_ports(self.port)
 
     @wait_container_is_ready(ConnectionError)
     def _healthcheck(self):
         host = self.get_container_host_ip()
         port = int(self.get_exposed_port(self.port))
-        paho.mqtt.client.Client().connect(host, port, 5)
+        paho.mqtt.client.Client().connect(host, port, 1)
 
     def start(self):
         self.with_command("mosquitto -c /mosquitto-no-auth.conf")
         super().start()
         self._healthcheck()
         return self
```

### Comparing `deciphon_sched-0.9.3/pyproject.toml` & `deciphon_sched-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphon-sched"
-version = "0.9.3"
+version = "0.9.4"
 description = "Deciphon scheduler"
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `deciphon_sched-0.9.3/PKG-INFO` & `deciphon_sched-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphon-sched
-Version: 0.9.3
+Version: 0.9.4
 Summary: Deciphon scheduler
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

