# Comparing `tmp/pyqqq_cli-0.3.0.tar.gz` & `tmp/pyqqq_cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq_cli-0.3.0.tar", max compression
+gzip compressed data, was "pyqqq_cli-0.3.1.tar", max compression
```

## Comparing `pyqqq_cli-0.3.0.tar` & `pyqqq_cli-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1064 2024-04-22 08:23:09.109923 pyqqq_cli-0.3.0/README.md
--rw-r--r--   0        0        0      655 2024-05-10 08:56:21.840734 pyqqq_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      358 2024-05-10 08:53:22.816157 pyqqq_cli-0.3.0/qupiato/cli/config.py
--rw-r--r--   0        0        0     8797 2024-05-10 08:24:10.048864 pyqqq_cli-0.3.0/qupiato/cli/main.py
--rw-r--r--   0        0        0     7239 2024-05-10 08:53:22.817467 pyqqq_cli-0.3.0/qupiato/cli/utils.py
--rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 pyqqq_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-22 07:02:26.408726 pyqqq_cli-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1064 2024-04-23 08:03:52.967483 pyqqq_cli-0.3.1/README.md
+-rw-r--r--   0        0        0      655 2024-05-17 04:51:02.735765 pyqqq_cli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-04-01 04:44:33.805339 pyqqq_cli-0.3.1/qupiato/cli/config.py
+-rw-r--r--   0        0        0     8797 2024-05-14 02:14:49.586902 pyqqq_cli-0.3.1/qupiato/cli/main.py
+-rw-r--r--   0        0        0     7225 2024-05-14 02:14:49.587175 pyqqq_cli-0.3.1/qupiato/cli/utils.py
+-rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 pyqqq_cli-0.3.1/PKG-INFO
```

### Comparing `pyqqq_cli-0.3.0/README.md` & `pyqqq_cli-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.3.0/pyproject.toml` & `pyqqq_cli-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pyqqq-cli"
-version = "0.3.0"
+version = "0.3.1"
 description = "CLI tool for controlling strategies deployed on the PyQQQ platform."
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qupiato"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
 websockets = "^12.0"
 python-dotenv = "^1.0.1"
 requests = "^2.31.0"
-pyqqq = "^0.8.7"
+pyqqq = "^0.9.8"
 pyyaml = "^6.0.1"
 
 [tool.poetry.scripts]
 qqq = 'qupiato.cli.main:main'
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pyqqq_cli-0.3.0/qupiato/cli/main.py` & `pyqqq_cli-0.3.1/qupiato/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.3.0/qupiato/cli/utils.py` & `pyqqq_cli-0.3.1/qupiato/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,19 +177,19 @@
     if response.status_code != 200 and response.status_code != 201:
         raise Exception(f"Publishing failed with status code {response.status_code}")
 
     return response.json()
 
 # 사용자 정보 조회
 def get_user(uid):
-    url = f"{c.API_SERVER_URL}/user"
+    url = f"{c.API_SERVER_URL}/users/{uid}"
     headers = {
         'Authorization': f'Bearer {get_token()}'
     }
-    response = requests.get(url, headers=headers, params={'uid': uid})
+    response = requests.get(url, headers=headers)
 
     if response.status_code != 200:
         raise Exception("Failed to search strategies")
 
     return response.json()
 
 # websocket 메시지에 추가될 agent 정보
```

### Comparing `pyqqq_cli-0.3.0/PKG-INFO` & `pyqqq_cli-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyqqq-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI tool for controlling strategies deployed on the PyQQQ platform.
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: pyqqq (>=0.8.7,<0.9.0)
+Requires-Dist: pyqqq (>=0.9.8,<0.10.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Documentation, https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io
 Description-Content-Type: text/markdown
```

