# Comparing `tmp/pytroll_watchers-0.2.1.tar.gz` & `tmp/pytroll_watchers-0.2.2.tar.gz`

## Comparing `pytroll_watchers-0.2.1.tar` & `pytroll_watchers-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,43 @@
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/.github/workflows/deploy-sdist.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/docs/make.bat
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/docs/source/backends.rst
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/docs/source/cli.rst
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/docs/source/conf.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/docs/source/index.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/docs/source/other_api.rst
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/docs/source/published.rst
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/common.py
--rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/dataspace_watcher.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/datastore_watcher.py
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/dhus_watcher.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/local_watcher.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/main_interface.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/minio_notification_watcher.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/publisher.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/testing.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/version.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/backends/__init__.py
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/src/pytroll_watchers/backends/local.py
--rw-r--r--   0        0        0    20443 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/tests/dataspace_responses.yaml
--rw-r--r--   0        0        0   168450 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/tests/datastore_responses.yaml
--rw-r--r--   0        0        0    56167 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/tests/dhus_responses.yaml
--rw-r--r--   0        0        0    39852 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/tests/test_bucket_notification_watcher.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/tests/test_copernicus_dataspace_watcher.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/tests/test_datastore.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/tests/test_dhus.py
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/tests/test_local_watcher.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/tests/test_main_interface.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/README.md
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    42086 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/.github/workflows/deploy-sdist.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/docs/make.bat
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/docs/source/backends.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/docs/source/cli.rst
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/docs/source/conf.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/docs/source/index.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/docs/source/other_api.rst
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/docs/source/published.rst
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/docs/source/selector.rst
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/common.py
+-rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/dataspace_watcher.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/datastore_watcher.py
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/dhus_watcher.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/local_watcher.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/main_interface.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/minio_notification_watcher.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/publisher.py
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/selector.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/testing.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/version.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/backends/__init__.py
+-rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/src/pytroll_watchers/backends/local.py
+-rw-r--r--   0        0        0    20443 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/dataspace_responses.yaml
+-rw-r--r--   0        0        0   168450 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/datastore_responses.yaml
+-rw-r--r--   0        0        0    56167 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/dhus_responses.yaml
+-rw-r--r--   0        0        0    39852 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/test_bucket_notification_watcher.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/test_copernicus_dataspace_watcher.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/test_datastore.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/test_dhus.py
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/test_local_watcher.py
+-rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/test_main_interface.py
+-rw-r--r--   0        0        0     8739 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/tests/test_selector.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/README.md
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    42153 2020-02-02 00:00:00.000000 pytroll_watchers-0.2.2/PKG-INFO
```

### Comparing `pytroll_watchers-0.2.1/.readthedocs.yaml` & `pytroll_watchers-0.2.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/CHANGELOG.md` & `pytroll_watchers-0.2.2/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## Version 0.2.2 (2024/05/17)
+
+
+### Pull Requests Merged
+
+#### Features added
+
+* [PR 13](https://github.com/pytroll/pytroll-watchers/pull/13) - Add selector feature
+
+In this release 1 pull request was closed.
+
+
 ## Version 0.2.1 (2024/05/08)
 
 
 ### Pull Requests Merged
 
 #### Bugs fixed
```

### Comparing `pytroll_watchers-0.2.1/.github/workflows/ci.yml` & `pytroll_watchers-0.2.2/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -24,18 +24,19 @@
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
+        sudo apt install -y redis-server
         python -m pip install --upgrade pip
         python -m pip install ruff pytest pytest-cov freezegun responses
         python -m pip install git+https://github.com/gorakhargosh/watchdog
-        python -m pip install -e .[local,minio,publishing,ssh,dataspace,datastore,dhus]
+        python -m pip install -e .[local,minio,publishing,ssh,dataspace,datastore,dhus,selector]
     - name: Lint with ruff
       run: |
         ruff check .
     - name: Test with pytest
       run: |
         pytest --cov=pytroll_watchers tests --cov-report=xml
     - name: Upload coverage reports to Codecov
```

### Comparing `pytroll_watchers-0.2.1/.github/workflows/deploy-sdist.yaml` & `pytroll_watchers-0.2.2/.github/workflows/deploy-sdist.yaml`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/docs/Makefile` & `pytroll_watchers-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/docs/make.bat` & `pytroll_watchers-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/docs/source/backends.rst` & `pytroll_watchers-0.2.2/docs/source/backends.rst`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/docs/source/conf.py` & `pytroll_watchers-0.2.2/docs/source/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,27 @@
 copyright = "2024, Martin Raspaud"
 author = "Martin Raspaud"
 release = version
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
-extensions = ["sphinx.ext.napoleon", "sphinx.ext.autodoc"]
+extensions = ["sphinx.ext.napoleon", "sphinx.ext.autodoc", "sphinx.ext.intersphinx"]
 autodoc_mock_imports = ["watchdog", "minio", "posttroll", "pytest", "trollsift", "universal_path",
-                        "freezegun", "responses", "oauthlib", "requests_oauthlib", "defusedxml"]
+                        "freezegun", "responses", "oauthlib", "requests_oauthlib", "defusedxml", "redis"]
 
 templates_path = ["_templates"]
 exclude_patterns = []
 
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "alabaster"
 html_static_path = ["_static"]
+
+# intersphinx
+intersphinx_mapping = {
+    "posttroll": ("https://posttroll.readthedocs.io/en/latest/", None),
+    "redis": ("https://redis.readthedocs.io/en/latest/", None),
+}
```

### Comparing `pytroll_watchers-0.2.1/docs/source/index.rst` & `pytroll_watchers-0.2.2/docs/source/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,15 @@
    :maxdepth: 2
    :caption: Contents:
 
    cli
    published
    backends
    other_api
+   selector
 
 Pytroll-watcher is a library and command-line tool to detect changes on a local or remote file system.
 
 
 Indices and tables
 ==================
```

### Comparing `pytroll_watchers-0.2.1/docs/source/published.rst` & `pytroll_watchers-0.2.2/docs/source/published.rst`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/common.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/common.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/dataspace_watcher.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/dataspace_watcher.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/datastore_watcher.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/datastore_watcher.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/dhus_watcher.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/dhus_watcher.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/local_watcher.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/local_watcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 """
 import logging
 import os
 from pathlib import Path
 from urllib.parse import urlunparse
 
 from upath import UPath
+from upath._flavour import WrappedFileSystemFlavour
 
 from pytroll_watchers.backends.local import listen_to_local_events
 from pytroll_watchers.publisher import SecurityError, file_publisher_from_generator, parse_metadata
 
+# This is a workaround for a but in universal_pathlib, see
+WrappedFileSystemFlavour.protocol_config["netloc_is_anchor"].add("ssh")
 logger = logging.getLogger(__name__)
 
 
 def file_publisher(fs_config, publisher_config, message_config):
     """Publish files coming from local filesystem events.
 
     Args:
@@ -68,11 +71,11 @@
     with listen_to_local_events(directory, file_pattern, observer_type) as events:
         for path in events:
             try:
                 file_metadata = parse_metadata(pattern, path)
             except ValueError:
                 continue
             if protocol is not None:
-                uri = urlunparse((protocol, None, path, None, None, None))
+                uri = urlunparse((protocol, None, str(path), None, None, None))
                 yield UPath(uri, **storage_options), file_metadata
             else:
                 yield Path(path), file_metadata
```

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/main_interface.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/main_interface.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/minio_notification_watcher.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/minio_notification_watcher.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/publisher.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/publisher.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/testing.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/testing.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/src/pytroll_watchers/backends/local.py` & `pytroll_watchers-0.2.2/src/pytroll_watchers/backends/local.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/tests/dataspace_responses.yaml` & `pytroll_watchers-0.2.2/tests/dataspace_responses.yaml`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/tests/datastore_responses.yaml` & `pytroll_watchers-0.2.2/tests/datastore_responses.yaml`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/tests/dhus_responses.yaml` & `pytroll_watchers-0.2.2/tests/dhus_responses.yaml`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/tests/test_bucket_notification_watcher.py` & `pytroll_watchers-0.2.2/tests/test_bucket_notification_watcher.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/tests/test_copernicus_dataspace_watcher.py` & `pytroll_watchers-0.2.2/tests/test_copernicus_dataspace_watcher.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/tests/test_datastore.py` & `pytroll_watchers-0.2.2/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/tests/test_dhus.py` & `pytroll_watchers-0.2.2/tests/test_dhus.py`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/tests/test_local_watcher.py` & `pytroll_watchers-0.2.2/tests/test_local_watcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,16 +84,16 @@
     publisher_settings = dict(nameservers=False, port=1979)
     message_settings = dict(subject="/segment/viirs/l1b/", atype="file", data=dict(sensor="viirs"))
 
     caplog.set_level("INFO")
     with patched_local_events([filename]):
         with patched_publisher() as messages:
             local_watcher.file_publisher(fs_config=local_settings,
-                                        publisher_config=publisher_settings,
-                                        message_config=message_settings)
+                                         publisher_config=publisher_settings,
+                                         message_config=message_settings)
 
     assert "uri" not in message_settings["data"]
     assert len(messages) == 1
     message = Message(rawstr=messages[0])
     assert message.data["uri"] == f"file://{str(tmp_path)}/foo.txt"
     assert message.data["sensor"] == "viirs"
     assert "fs" not in message.data
@@ -111,9 +111,9 @@
     message_settings = dict(subject="/segment/viirs/l1b/", atype="file", data=dict(sensor="viirs"))
 
     caplog.set_level("INFO")
     with patched_local_events([filename]):
         with patched_publisher():
             with pytest.raises(SecurityError):
                 local_watcher.file_publisher(fs_config=local_settings,
-                                            publisher_config=publisher_settings,
-                                            message_config=message_settings)
+                                             publisher_config=publisher_settings,
+                                             message_config=message_settings)
```

### Comparing `pytroll_watchers-0.2.1/tests/test_main_interface.py` & `pytroll_watchers-0.2.2/tests/test_main_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Tests for the gathered publisher functions."""
 
+import json
 import logging
+from unittest import mock
 
 import pytest
 import yaml
+from posttroll.message import Message
 from posttroll.testing import patched_publisher
 from pytroll_watchers.local_watcher import file_generator as local_generator
 from pytroll_watchers.local_watcher import file_publisher as local_publisher
 from pytroll_watchers.main_interface import (
     cli,
     get_generator_for_backend,
     get_publisher_for_backend,
     publish_from_config,
 )
 from pytroll_watchers.minio_notification_watcher import file_generator as minio_generator
 from pytroll_watchers.minio_notification_watcher import file_publisher as minio_publisher
 from pytroll_watchers.testing import patched_bucket_listener, patched_local_events  # noqa
+from upath import UPath
 
 
 def test_getting_right_publisher():
     """Test getting the right publisher for a given backend."""
     file_publisher = get_publisher_for_backend("minio")
     assert file_publisher == minio_publisher
     file_publisher = get_publisher_for_backend("local")
@@ -50,14 +54,41 @@
         filename = tmp_path / "bla"
         with patched_local_events([filename]):
             publish_from_config(config)
             assert len(msgs) == 1
             assert str(filename) in msgs[0]
 
 
+def test_pass_config_to_file_publisher_for_local_backend_with_protocol(tmp_path, patched_local_events, monkeypatch):  # noqa
+    """Test passing a config to create a file publisher from a local fs with protocol."""
+    new_fs = mock.Mock()
+    host = "myhost.pytroll.org"
+    fs = dict(cls="fsspec.implementations.sftp.SFTPFileSystem",
+              protocol="sftp",
+              args=[],
+              host=host)
+    new_fs.to_json.return_value = json.dumps(fs)
+    monkeypatch.setattr(UPath, "fs", new_fs)
+    local_settings = dict(directory=tmp_path, protocol="ssh", storage_options=dict(host=host))
+    publisher_settings = dict(nameservers=False, port=1979)
+    message_settings = dict(subject="/segment/viirs/l1b/", atype="file", data=dict(sensor="viirs"))
+    config = dict(backend="local",
+                  fs_config=local_settings,
+                  publisher_config=publisher_settings,
+                  message_config=message_settings)
+    with patched_publisher() as msgs:
+        filename = tmp_path / "bla"
+        with patched_local_events([filename]):
+            publish_from_config(config)
+            assert len(msgs) == 1
+            msg = Message.decode(msgs[0])
+            assert msg.data["path"] == str(filename)
+
+
+
 def test_pass_config_to_object_publisher_for_minio_backend(patched_bucket_listener):  # noqa
     """Test passing a config to create an objec publisher from minio bucket."""
     s3_settings = dict(endpoint_url="someendpoint",
                        bucket_name="viirs-data",
                        storage_options=dict())
     publisher_settings = dict(nameservers=False, port=1979)
     message_settings = dict(subject="/segment/viirs/l1b/", atype="file", data=dict(sensor="viirs"))
```

### Comparing `pytroll_watchers-0.2.1/LICENSE.txt` & `pytroll_watchers-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytroll_watchers-0.2.1/pyproject.toml` & `pytroll_watchers-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Communications"
 ]
 
 [project.scripts]
 pytroll-watcher = "pytroll_watchers.main_interface:cli"
+pytroll-selector = "pytroll_watchers.selector:cli"
 
 [project.entry-points."pytroll_watchers.backends"]
 local = "pytroll_watchers.local_watcher"
 minio = "pytroll_watchers.minio_notification_watcher"
 dataspace = "pytroll_watchers.dataspace_watcher"
 datastore = "pytroll_watchers.datastore_watcher"
 dhus = "pytroll_watchers.dhus_watcher"
@@ -35,14 +36,15 @@
 minio = ["minio", "s3fs"]
 local = ["watchdog"]
 publishing = ["posttroll"]
 ssh = ["paramiko"]
 dataspace = ["oauthlib", "requests_oauthlib", "s3fs"]
 datastore = ["oauthlib", "requests_oauthlib"]
 dhus = ["defusedxml"]
+selector = ["redis"]
 
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
```

### Comparing `pytroll_watchers-0.2.1/PKG-INFO` & `pytroll_watchers-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytroll-watchers
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility functions and scripts to watch for new files on local or remote filesystems.
 Project-URL: Documentation, https://pytroll-watchers.readthedocs.io/en/latest/
 Author-email: Martin Raspaud <martin.raspaud@smhi.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -702,14 +702,16 @@
 Provides-Extra: local
 Requires-Dist: watchdog; extra == 'local'
 Provides-Extra: minio
 Requires-Dist: minio; extra == 'minio'
 Requires-Dist: s3fs; extra == 'minio'
 Provides-Extra: publishing
 Requires-Dist: posttroll; extra == 'publishing'
+Provides-Extra: selector
+Requires-Dist: redis; extra == 'selector'
 Provides-Extra: ssh
 Requires-Dist: paramiko; extra == 'ssh'
 Description-Content-Type: text/markdown
 
 # pytroll-watchers
 
 Utility functions and scripts to watch for new files on local or remote filesystems.
```

