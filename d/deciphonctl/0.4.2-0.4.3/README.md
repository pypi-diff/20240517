# Comparing `tmp/deciphonctl-0.4.2.tar.gz` & `tmp/deciphonctl-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphonctl-0.4.2.tar", max compression
+gzip compressed data, was "deciphonctl-0.4.3.tar", max compression
```

## Comparing `deciphonctl-0.4.2.tar` & `deciphonctl-0.4.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1063 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/LICENSE
--rw-r--r--   0        0        0       15 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/README.md
--rw-r--r--   0        0        0        0 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/__init__.py
--rw-r--r--   0        0        0       28 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/__main__.py
--rw-r--r--   0        0        0     6028 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/cli.py
--rw-r--r--   0        0        0      755 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/consumer.py
--rw-r--r--   0        0        0      677 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/download.py
--rw-r--r--   0        0        0      157 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/file_path.py
--rw-r--r--   0        0        0     1088 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/files.py
--rw-r--r--   0        0        0     2382 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/models.py
--rw-r--r--   0        0        0      107 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/permissions.py
--rw-r--r--   0        0        0     3514 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/presser.py
--rw-r--r--   0        0        0     1242 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/progress.py
--rw-r--r--   0        0        0      423 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/progress_informer.py
--rw-r--r--   0        0        0      871 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/progress_logger.py
--rw-r--r--   0        0        0     3246 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/scanner.py
--rw-r--r--   0        0        0     5922 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/sched.py
--rw-r--r--   0        0        0      474 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/settings.py
--rw-r--r--   0        0        0      387 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/signals.py
--rw-r--r--   0        0        0      240 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/url.py
--rw-r--r--   0        0        0     1055 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/worker.py
--rw-r--r--   0        0        0      792 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 deciphonctl-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/__main__.py
+-rw-r--r--   0        0        0      502 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/catch_validation.py
+-rw-r--r--   0        0        0     6574 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/cli.py
+-rw-r--r--   0        0        0      755 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/consumer.py
+-rw-r--r--   0        0        0      677 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/download.py
+-rw-r--r--   0        0        0      157 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/file_path.py
+-rw-r--r--   0        0        0     1088 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/files.py
+-rw-r--r--   0        0        0     2382 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/models.py
+-rw-r--r--   0        0        0      107 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/permissions.py
+-rw-r--r--   0        0        0     3514 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/presser.py
+-rw-r--r--   0        0        0     1242 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/progress.py
+-rw-r--r--   0        0        0      423 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/progress_informer.py
+-rw-r--r--   0        0        0      871 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/progress_logger.py
+-rw-r--r--   0        0        0     3246 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/scanner.py
+-rw-r--r--   0        0        0     5922 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/sched.py
+-rw-r--r--   0        0        0      491 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/settings.py
+-rw-r--r--   0        0        0      387 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/signals.py
+-rw-r--r--   0        0        0      240 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/url.py
+-rw-r--r--   0        0        0     1055 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/deciphonctl/worker.py
+-rw-r--r--   0        0        0      792 2024-05-17 10:50:57.851623 deciphonctl-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 deciphonctl-0.4.3/PKG-INFO
```

### Comparing `deciphonctl-0.4.2/LICENSE` & `deciphonctl-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/cli.py` & `deciphonctl-0.4.3/deciphonctl/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import rich
 import typer
 from deciphon_core.schema import Gencode
 from loguru import logger
 from typer import Argument, FileText, Option
 from typing_extensions import Annotated
 
-from deciphonctl.settings import Settings
+from deciphonctl.catch_validation import catch_validation
 from deciphonctl.models import DBFile, HMMFile, LogLevel, Scan, Seq
 from deciphonctl.presser import presser_entry
 from deciphonctl.scanner import scanner_entry
 from deciphonctl.sched import Sched
+from deciphonctl.settings import Settings
 from deciphonctl.signals import raise_sigint_on_sigterm
 
 HMMFILE = Annotated[
     Path,
     Argument(
         exists=True,
         file_okay=True,
@@ -53,24 +54,37 @@
     ),
 ]
 OUTFILE = Annotated[
     Path,
     Option(file_okay=True, dir_okay=False, writable=True, help="Output file"),
 ]
 
+config = typer.Typer()
 hmm = typer.Typer()
 db = typer.Typer()
 job = typer.Typer()
 scan = typer.Typer()
 seq = typer.Typer()
 snap = typer.Typer()
 presser = typer.Typer()
 scanner = typer.Typer()
 
 
+@config.command("dump")
+def config_dump():
+    with catch_validation():
+        settings = Settings()
+        for field in settings.__fields__:
+            value = getattr(settings, field)
+            if value is None:
+                typer.echo(f"{field}=")
+            else:
+                typer.echo(f"{field}={value}")
+
+
 @hmm.command("add")
 def hmm_add(hmmfile: HMMFILE, gencode: GENCODE, epsilon: EPSILON = 0.01):
     settings = Settings()
     sched = Sched(settings.sched_url, settings.s3_url)
     sched.upload(hmmfile, sched.presigned.upload_hmm_post(hmmfile.name))
     sched.hmm_post(HMMFile(name=hmmfile.name), gencode, epsilon)
 
@@ -203,15 +217,20 @@
     raise_sigint_on_sigterm()
     logger.remove()
     logger.add(sys.stderr, level=log_level.value.upper())
     sched = Sched(settings.sched_url, settings.s3_url)
     scanner_entry(settings, sched, num_workers, num_threads)
 
 
-app = typer.Typer()
+app = typer.Typer(
+    add_completion=False,
+    pretty_exceptions_short=True,
+    pretty_exceptions_show_locals=False,
+)
+app.add_typer(config, name="config")
 app.add_typer(hmm, name="hmm")
 app.add_typer(db, name="db")
 app.add_typer(job, name="job")
 app.add_typer(scan, name="scan")
 app.add_typer(seq, name="seq")
 app.add_typer(presser, name="presser")
 app.add_typer(scanner, name="scanner")
```

### Comparing `deciphonctl-0.4.2/deciphonctl/consumer.py` & `deciphonctl-0.4.3/deciphonctl/consumer.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/download.py` & `deciphonctl-0.4.3/deciphonctl/download.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/files.py` & `deciphonctl-0.4.3/deciphonctl/files.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/models.py` & `deciphonctl-0.4.3/deciphonctl/models.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/presser.py` & `deciphonctl-0.4.3/deciphonctl/presser.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/progress.py` & `deciphonctl-0.4.3/deciphonctl/progress.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/progress_logger.py` & `deciphonctl-0.4.3/deciphonctl/progress_logger.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/scanner.py` & `deciphonctl-0.4.3/deciphonctl/scanner.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/sched.py` & `deciphonctl-0.4.3/deciphonctl/sched.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/deciphonctl/worker.py` & `deciphonctl-0.4.3/deciphonctl/worker.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.2/pyproject.toml` & `deciphonctl-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphonctl"
-version = "0.4.2"
+version = "0.4.3"
 description = "Control Deciphon server."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphonctl" }]
 
 [tool.poetry.dependencies]
```

### Comparing `deciphonctl-0.4.2/PKG-INFO` & `deciphonctl-0.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphonctl
-Version: 0.4.2
+Version: 0.4.3
 Summary: Control Deciphon server.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

