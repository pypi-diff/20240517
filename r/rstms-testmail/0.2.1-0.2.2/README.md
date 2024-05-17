# Comparing `tmp/rstms_testmail-0.2.1.tar.gz` & `tmp/rstms_testmail-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_testmail-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_testmail-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_testmail-0.2.1.tar` & `rstms_testmail-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      381 2024-05-09 14:44:16.073248 rstms_testmail-0.2.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1375 2024-04-28 12:24:23.591184 rstms_testmail-0.2.1/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-28 01:24:57.918261 rstms_testmail-0.2.1/LICENSE
--rw-r--r--   0        0        0      539 2024-04-28 01:24:57.918261 rstms_testmail-0.2.1/Makefile
--rw-r--r--   0        0        0      679 2024-04-28 01:24:57.930261 rstms_testmail-0.2.1/README.md
--rw-r--r--   0        0        0        6 2024-05-09 14:44:16.073248 rstms_testmail-0.2.1/VERSION
--rw-r--r--   0        0        0      615 2024-04-28 01:24:58.006260 rstms_testmail-0.2.1/docs/Makefile
--rw-r--r--   0        0        0       93 2024-04-28 01:24:58.018260 rstms_testmail-0.2.1/docs/cli.rst
--rwxr-xr-x   0        0        0     4934 2024-04-28 01:24:58.014260 rstms_testmail-0.2.1/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-28 01:24:58.018260 rstms_testmail-0.2.1/docs/contributing.rst
--rw-r--r--   0        0        0      298 2024-04-28 01:24:58.002260 rstms_testmail-0.2.1/docs/index.rst
--rw-r--r--   0        0        0     1158 2024-04-28 01:24:58.010260 rstms_testmail-0.2.1/docs/installation.rst
--rw-r--r--   0        0        0      776 2024-04-28 01:24:58.002260 rstms_testmail-0.2.1/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-28 01:24:57.998260 rstms_testmail-0.2.1/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-28 01:24:57.946261 rstms_testmail-0.2.1/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-28 01:24:57.954260 rstms_testmail-0.2.1/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-28 01:24:57.950260 rstms_testmail-0.2.1/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-28 01:24:57.946261 rstms_testmail-0.2.1/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-28 01:24:57.942261 rstms_testmail-0.2.1/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-28 01:24:57.938261 rstms_testmail-0.2.1/make/docs.mk
--rw-r--r--   0        0        0      610 2024-04-28 01:24:57.934261 rstms_testmail-0.2.1/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-28 01:24:57.938261 rstms_testmail-0.2.1/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-28 01:24:57.942261 rstms_testmail-0.2.1/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-28 01:24:57.942261 rstms_testmail-0.2.1/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-28 01:24:57.938261 rstms_testmail-0.2.1/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-28 01:24:57.946261 rstms_testmail-0.2.1/make/version.mk
--rw-r--r--   0        0        0     1232 2024-05-09 14:44:16.073248 rstms_testmail-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-28 01:24:57.890261 rstms_testmail-0.2.1/pytest.ini
--rw-r--r--   0        0        0       97 2024-05-09 14:44:15.909249 rstms_testmail-0.2.1/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-05-09 14:44:15.965249 rstms_testmail-0.2.1/requirements-docs.txt
--rw-r--r--   0        0        0       89 2024-05-09 14:44:15.853250 rstms_testmail-0.2.1/requirements.txt
--rw-r--r--   0        0        0      215 2024-04-28 01:57:04.207457 rstms_testmail-0.2.1/rstms_testmail/__init__.py
--rw-r--r--   0        0        0     3816 2024-05-09 14:27:36.176660 rstms_testmail-0.2.1/rstms_testmail/cli.py
--rw-r--r--   0        0        0      957 2024-04-28 02:18:58.990987 rstms_testmail-0.2.1/rstms_testmail/counter.py
--rw-r--r--   0        0        0     1067 2024-04-28 01:24:57.990260 rstms_testmail-0.2.1/rstms_testmail/exception_handler.py
--rw-r--r--   0        0        0     3817 2024-05-09 14:34:03.428254 rstms_testmail-0.2.1/rstms_testmail/gmail.py
--rw-r--r--   0        0        0      353 2024-04-28 06:41:02.468012 rstms_testmail-0.2.1/rstms_testmail/netstat.py
--rw-r--r--   0        0        0      594 2024-05-03 20:34:02.011028 rstms_testmail-0.2.1/rstms_testmail/sendgrid_server.py
--rw-r--r--   0        0        0     1027 2024-05-03 20:33:37.171309 rstms_testmail-0.2.1/rstms_testmail/settings.py
--rw-r--r--   0        0        0     1092 2024-04-28 01:57:04.247457 rstms_testmail-0.2.1/rstms_testmail/shell.py
--rw-r--r--   0        0        0     1244 2024-04-30 05:00:13.658436 rstms_testmail-0.2.1/rstms_testmail/smtp_server.py
--rw-r--r--   0        0        0      698 2024-04-28 07:28:06.715644 rstms_testmail-0.2.1/rstms_testmail/timer.py
--rw-r--r--   0        0        0      127 2024-05-09 14:44:16.073248 rstms_testmail-0.2.1/rstms_testmail/version.py
--rw-r--r--   0        0        0     2669 2024-04-28 08:38:07.194667 rstms_testmail-0.2.1/rstms_testmail/watcher.py
--rw-r--r--   0        0        0       44 2024-04-28 01:24:57.970260 rstms_testmail-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     2259 2024-04-28 01:57:04.271457 rstms_testmail-0.2.1/tests/test_cli.py
--rw-r--r--   0        0        0      330 2024-04-28 06:40:10.408723 rstms_testmail-0.2.1/tests/test_counter.py
--rw-r--r--   0        0        0      353 2024-04-28 13:04:29.510760 rstms_testmail-0.2.1/tests/test_gmail.py
--rw-r--r--   0        0        0      201 2024-04-28 06:40:42.264287 rstms_testmail-0.2.1/tests/test_netstat.py
--rw-r--r--   0        0        0      553 2024-04-28 13:09:49.371217 rstms_testmail-0.2.1/tests/test_sendgrid.py
--rw-r--r--   0        0        0     1156 2024-04-28 08:39:55.537304 rstms_testmail-0.2.1/tests/test_watcher.py
--rw-r--r--   0        0        0      430 2024-04-28 01:24:57.894261 rstms_testmail-0.2.1/tox.ini
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 rstms_testmail-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      381 2024-05-17 19:57:31.368779 rstms_testmail-0.2.2/.bumpversion.cfg
+-rw-r--r--   0        0        0     1375 2024-04-28 12:24:23.591184 rstms_testmail-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-28 01:24:57.918261 rstms_testmail-0.2.2/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-28 01:24:57.918261 rstms_testmail-0.2.2/Makefile
+-rw-r--r--   0        0        0      679 2024-04-28 01:24:57.930261 rstms_testmail-0.2.2/README.md
+-rw-r--r--   0        0        0        6 2024-05-17 19:57:31.368779 rstms_testmail-0.2.2/VERSION
+-rw-r--r--   0        0        0      615 2024-04-28 01:24:58.006260 rstms_testmail-0.2.2/docs/Makefile
+-rw-r--r--   0        0        0       93 2024-04-28 01:24:58.018260 rstms_testmail-0.2.2/docs/cli.rst
+-rwxr-xr-x   0        0        0     4934 2024-04-28 01:24:58.014260 rstms_testmail-0.2.2/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-28 01:24:58.018260 rstms_testmail-0.2.2/docs/contributing.rst
+-rw-r--r--   0        0        0      298 2024-04-28 01:24:58.002260 rstms_testmail-0.2.2/docs/index.rst
+-rw-r--r--   0        0        0     1158 2024-04-28 01:24:58.010260 rstms_testmail-0.2.2/docs/installation.rst
+-rw-r--r--   0        0        0      776 2024-04-28 01:24:58.002260 rstms_testmail-0.2.2/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-28 01:24:57.998260 rstms_testmail-0.2.2/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-28 01:24:57.946261 rstms_testmail-0.2.2/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-28 01:24:57.954260 rstms_testmail-0.2.2/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-28 01:24:57.950260 rstms_testmail-0.2.2/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-28 01:24:57.946261 rstms_testmail-0.2.2/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-28 01:24:57.942261 rstms_testmail-0.2.2/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-28 01:24:57.938261 rstms_testmail-0.2.2/make/docs.mk
+-rw-r--r--   0        0        0      610 2024-04-28 01:24:57.934261 rstms_testmail-0.2.2/make/lint.mk
+-rw-r--r--   0        0        0     1214 2024-04-28 01:24:57.938261 rstms_testmail-0.2.2/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-28 01:24:57.942261 rstms_testmail-0.2.2/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-28 01:24:57.942261 rstms_testmail-0.2.2/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-28 01:24:57.938261 rstms_testmail-0.2.2/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-28 01:24:57.946261 rstms_testmail-0.2.2/make/version.mk
+-rw-r--r--   0        0        0     1232 2024-05-17 19:57:31.368779 rstms_testmail-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-28 01:24:57.890261 rstms_testmail-0.2.2/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-17 19:57:31.216781 rstms_testmail-0.2.2/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-17 19:57:31.272780 rstms_testmail-0.2.2/requirements-docs.txt
+-rw-r--r--   0        0        0       89 2024-05-17 19:57:31.160781 rstms_testmail-0.2.2/requirements.txt
+-rw-r--r--   0        0        0      215 2024-04-28 01:57:04.207457 rstms_testmail-0.2.2/rstms_testmail/__init__.py
+-rw-r--r--   0        0        0     4699 2024-05-17 19:52:43.571922 rstms_testmail-0.2.2/rstms_testmail/cli.py
+-rw-r--r--   0        0        0      957 2024-04-28 02:18:58.990987 rstms_testmail-0.2.2/rstms_testmail/counter.py
+-rw-r--r--   0        0        0     1067 2024-04-28 01:24:57.990260 rstms_testmail-0.2.2/rstms_testmail/exception_handler.py
+-rw-r--r--   0        0        0     3676 2024-05-17 19:53:13.035598 rstms_testmail-0.2.2/rstms_testmail/gmail.py
+-rw-r--r--   0        0        0      353 2024-04-28 06:41:02.468012 rstms_testmail-0.2.2/rstms_testmail/netstat.py
+-rw-r--r--   0        0        0      584 2024-05-17 19:53:22.655493 rstms_testmail-0.2.2/rstms_testmail/sendgrid_server.py
+-rw-r--r--   0        0        0     1575 2024-05-17 19:52:23.144146 rstms_testmail-0.2.2/rstms_testmail/settings.py
+-rw-r--r--   0        0        0     1092 2024-04-28 01:57:04.247457 rstms_testmail-0.2.2/rstms_testmail/shell.py
+-rw-r--r--   0        0        0     1257 2024-05-17 19:52:23.124146 rstms_testmail-0.2.2/rstms_testmail/smtp_server.py
+-rw-r--r--   0        0        0      698 2024-04-28 07:28:06.715644 rstms_testmail-0.2.2/rstms_testmail/timer.py
+-rw-r--r--   0        0        0      127 2024-05-17 19:57:31.368779 rstms_testmail-0.2.2/rstms_testmail/version.py
+-rw-r--r--   0        0        0     2669 2024-04-28 08:38:07.194667 rstms_testmail-0.2.2/rstms_testmail/watcher.py
+-rw-r--r--   0        0        0       44 2024-04-28 01:24:57.970260 rstms_testmail-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-17 19:56:14.241618 rstms_testmail-0.2.2/tests/test_cli.py
+-rw-r--r--   0        0        0      330 2024-04-28 06:40:10.408723 rstms_testmail-0.2.2/tests/test_counter.py
+-rw-r--r--   0        0        0      353 2024-04-28 13:04:29.510760 rstms_testmail-0.2.2/tests/test_gmail.py
+-rw-r--r--   0        0        0      201 2024-04-28 06:40:42.264287 rstms_testmail-0.2.2/tests/test_netstat.py
+-rw-r--r--   0        0        0      553 2024-04-28 13:09:49.371217 rstms_testmail-0.2.2/tests/test_sendgrid.py
+-rw-r--r--   0        0        0     1156 2024-04-28 08:39:55.537304 rstms_testmail-0.2.2/tests/test_watcher.py
+-rw-r--r--   0        0        0      430 2024-04-28 01:24:57.894261 rstms_testmail-0.2.2/tox.ini
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 rstms_testmail-0.2.2/PKG-INFO
```

### Comparing `rstms_testmail-0.2.1/.gitignore` & `rstms_testmail-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/LICENSE` & `rstms_testmail-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/Makefile` & `rstms_testmail-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/README.md` & `rstms_testmail-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/docs/Makefile` & `rstms_testmail-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/docs/conf.py` & `rstms_testmail-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/docs/installation.rst` & `rstms_testmail-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/docs/make.bat` & `rstms_testmail-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/make/clean.mk` & `rstms_testmail-0.2.2/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/make/common.mk` & `rstms_testmail-0.2.2/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/make/docs.mk` & `rstms_testmail-0.2.2/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/make/lint.mk` & `rstms_testmail-0.2.2/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/make/publish.mk` & `rstms_testmail-0.2.2/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/make/release.mk` & `rstms_testmail-0.2.2/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/make/test.mk` & `rstms_testmail-0.2.2/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/make/version.mk` & `rstms_testmail-0.2.2/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/pyproject.toml` & `rstms_testmail-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-testmail"
-version = "0.2.1"
+version = "0.2.2"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_testmail"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_testmail-0.2.1/rstms_testmail/counter.py` & `rstms_testmail-0.2.2/rstms_testmail/counter.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/rstms_testmail/exception_handler.py` & `rstms_testmail-0.2.2/rstms_testmail/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/rstms_testmail/gmail.py` & `rstms_testmail-0.2.2/rstms_testmail/gmail.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import base64
-import os
 import tempfile
-from pathlib import Path
-
+from email.message import EmailMessage
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
+from pathlib import Path
 
-import google.auth
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
-from email.message import EmailMessage
-from googleapiclient.errors import HttpError
 
 from .watcher import PortWatcher
 
-
-## If modifying these SCOPES, delete the file token.json.
+# If modifying these SCOPES, delete the file token.json.
 SCOPES = ["https://www.googleapis.com/auth/gmail.send"]
 
+
 class Gmail:
 
     def __init__(self, credentials, reset_token=False):
         """credentials is a base64 encoded credentials.json file. (see https://console.cloud.google.com)"""
 
         self.credentials = credentials
-        self.token_file = Path.home() / '.testmail-gmail-token.json'
+        self.token_file = Path.home() / ".testmail-gmail-token.json"
         if reset_token:
             self.token_file.unlink()
 
         with PortWatcher("ssh -q -N -R {}:localhost:{} beaker"):
             self.creds = self.authenticate_gmail_api()
 
             # create gmail api client
@@ -95,18 +91,11 @@
         message["Subject"] = subject
 
         # encoded message
         encoded_message = base64.urlsafe_b64encode(message.as_bytes()).decode()
 
         create_message = {"message": {"raw": encoded_message}}
         # pylint: disable=E1101
-        send_message = (
-            self.service.users()
-            .messages()
-            .send(userId="me", body=create_message)
-            .execute()
-        )
+        send_message = self.service.users().messages().send(userId="me", body=create_message).execute()
 
         print(f'Message id: {send_message["id"]}')
         return send_message
-
-
```

### Comparing `rstms_testmail-0.2.1/rstms_testmail/sendgrid_server.py` & `rstms_testmail-0.2.2/rstms_testmail/sendgrid_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 import sendgrid
 import sendgrid.helpers.mail
 
 
 class SendGrid:
 
     def __init__(self, api_key):
@@ -14,9 +12,9 @@
             from_email=from_addr,
             to_emails=to_addr,
             subject=subject,
             plain_text_content=message_text,
         )
         response = self.client.send(message)
         headers = response.headers
-        self.result = {k:headers[k] for k in headers.keys()}
+        self.result = {k: headers[k] for k in headers.keys()}
         return None
```

### Comparing `rstms_testmail-0.2.1/rstms_testmail/settings.py` & `rstms_testmail-0.2.2/rstms_testmail/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,61 @@
-from pathlib import Path
 import json
+from pathlib import Path
+
 
 class Settings:
     def __init__(self, **kwargs):
-        profile=kwargs.pop('profile', "")
-        update_profile=kwargs.pop('update_profile', "")
-        dir = kwargs.pop('dir', '~')
-        if dir in ['~', None]:
+        profile = kwargs.pop("profile", "")
+        write_profile = kwargs.pop("write_profile", "")
+
+        dir = kwargs.pop("dir", "~")
+        if dir in ["~", None]:
             dir = Path.home()
         else:
             dir = Path(dir)
+        self.dir = dir
+
         self.file = dir / f".{profile}_settings"
 
         old_settings = self.read()
 
         self._settings = {}
 
-        for k,v in kwargs.items():
+        for k, v in kwargs.items():
             if v is None:
                 v = old_settings.get(k, None)
             self._settings[k] = v
             setattr(self, k, v)
 
-        if update_profile:
-            self.write(self._settings, dir / f".{update_profile}_settings" )
+        if write_profile:
+            self.write(self._settings, dir / f".{write_profile}_settings")
+
+    def delete(self):
+        self.file.unlink()
+        return
+
+    def profiles(self):
+        profiles = []
+        label, _, _ = self.file.name.partition("_")
+        for item in self.file.parent.iterdir():
+            if not item.is_file():
+                continue
+            prefix, _, tail = item.name.partition("_")
+            if prefix != label:
+                continue
+            name, _, _ = tail.partition("_")
+            if name:
+                profiles.append(name)
+        return profiles
 
     def read(self):
         if self.file.is_file():
             content = self.file.read_text()
         else:
             content = "{}"
         return json.loads(content)
 
     def write(self, settings, file):
-        file.write_text(json.dumps(settings))
+        file.write_text(json.dumps(settings, indent=2))
 
     def dict(self):
         return self._settings
```

### Comparing `rstms_testmail-0.2.1/rstms_testmail/shell.py` & `rstms_testmail-0.2.2/rstms_testmail/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/rstms_testmail/smtp_server.py` & `rstms_testmail-0.2.2/rstms_testmail/smtp_server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import smtplib
-from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+
 
 class SMTPServer:
 
     def __init__(self, system, port, username, password):
-        _, _, self.server = system.partition(':')
+        self.protocol, _, self.server = system.partition(":")
         self.port = int(port)
         self.username = username
         self.password = password
 
     def send(self, from_addr, to_addr, subject, message):
         """
         Send an email using an SMTP server that requires SSL and authentication.
@@ -18,18 +19,18 @@
         - from_addr: str - the sender's email address
         - to_addr: str - the recipient's email address
         - subject: str - the subject of the email
         - message: str - the body of the email
         """
         # Create the container email message.
         mime_message = MIMEMultipart()
-        mime_message['Subject'] = subject
-        mime_message['From'] = from_addr
-        mime_message['To'] = to_addr
-        mime_message.attach(MIMEText(message, 'plain'))
+        mime_message["Subject"] = subject
+        mime_message["From"] = from_addr
+        mime_message["To"] = to_addr
+        mime_message.attach(MIMEText(message, "plain"))
 
         # Connect to the SMTP server using SSL
         server = smtplib.SMTP_SSL(self.server, self.port)
         server.login(self.username, self.password)
         server.sendmail(from_addr, to_addr, mime_message.as_string())
         server.quit()
         return None
```

### Comparing `rstms_testmail-0.2.1/rstms_testmail/timer.py` & `rstms_testmail-0.2.2/rstms_testmail/timer.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/rstms_testmail/watcher.py` & `rstms_testmail-0.2.2/rstms_testmail/watcher.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/tests/test_cli.py` & `rstms_testmail-0.2.2/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return result
 
     return _run
 
 
 def test_cli_no_args(run):
     result = run([])
-    assert "Usage:" in result.output
+    assert result.output
 
 
 def test_cli_help(run):
     result = run(["--help"])
     assert "Show this message and exit." in result.output
```

### Comparing `rstms_testmail-0.2.1/tests/test_sendgrid.py` & `rstms_testmail-0.2.2/tests/test_sendgrid.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/tests/test_watcher.py` & `rstms_testmail-0.2.2/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.1/PKG-INFO` & `rstms_testmail-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-testmail
-Version: 0.2.1
+Version: 0.2.2
 Summary: Top-level package for rstms-testmail.
 Keywords: rstms_testmail
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

