# Comparing `tmp/resend-1.0.2.tar.gz` & `tmp/resend-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resend-1.0.2.tar", last modified: Tue May 14 01:37:48 2024, max compression
+gzip compressed data, was "resend-1.1.0.tar", last modified: Fri May 17 21:47:27 2024, max compression
```

## Comparing `resend-1.0.2.tar` & `resend-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.903787 resend-1.0.2/
--rw-r--r--   0 derich     (501) staff       (20)     1070 2023-08-19 17:45:00.000000 resend-1.0.2/LICENSE.md
--rw-r--r--   0 derich     (501) staff       (20)     2430 2024-05-14 01:37:48.903715 resend-1.0.2/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)     1627 2024-05-14 01:16:37.000000 resend-1.0.2/README.md
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.899984 resend-1.0.2/resend/
--rw-r--r--   0 derich     (501) staff       (20)     1003 2024-05-14 01:16:37.000000 resend-1.0.2/resend/__init__.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.901211 resend-1.0.2/resend/api_keys/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/api_keys/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)      998 2024-05-09 01:36:14.000000 resend-1.0.2/resend/api_keys/_api_key.py
--rw-r--r--   0 derich     (501) staff       (20)     2310 2024-05-09 01:36:14.000000 resend-1.0.2/resend/api_keys/_api_keys.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.901668 resend-1.0.2/resend/audiences/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/audiences/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1192 2024-05-09 01:36:14.000000 resend-1.0.2/resend/audiences/_audience.py
--rw-r--r--   0 derich     (501) staff       (20)     2305 2024-05-09 01:36:14.000000 resend-1.0.2/resend/audiences/_audiences.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.902043 resend-1.0.2/resend/contacts/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/contacts/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1795 2024-05-09 01:36:14.000000 resend-1.0.2/resend/contacts/_contact.py
--rw-r--r--   0 derich     (501) staff       (20)     4400 2024-05-09 01:36:14.000000 resend-1.0.2/resend/contacts/_contacts.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.902667 resend-1.0.2/resend/domains/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/domains/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1987 2024-05-09 01:36:14.000000 resend-1.0.2/resend/domains/_domain.py
--rw-r--r--   0 derich     (501) staff       (20)     3887 2024-05-09 01:36:14.000000 resend-1.0.2/resend/domains/_domains.py
--rw-r--r--   0 derich     (501) staff       (20)     1416 2024-05-09 01:36:14.000000 resend-1.0.2/resend/domains/_record.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.903440 resend-1.0.2/resend/emails/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)      489 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_attachment.py
--rw-r--r--   0 derich     (501) staff       (20)      755 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_batch.py
--rw-r--r--   0 derich     (501) staff       (20)     2601 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_email.py
--rw-r--r--   0 derich     (501) staff       (20)     2717 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_emails.py
--rw-r--r--   0 derich     (501) staff       (20)      524 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_tag.py
--rw-r--r--   0 derich     (501) staff       (20)     6102 2024-05-14 01:16:37.000000 resend-1.0.2/resend/exceptions.py
--rw-r--r--   0 derich     (501) staff       (20)        0 2023-08-19 17:45:00.000000 resend-1.0.2/resend/py.typed
--rw-r--r--   0 derich     (501) staff       (20)     2363 2024-05-14 01:16:37.000000 resend-1.0.2/resend/request.py
--rw-r--r--   0 derich     (501) staff       (20)      133 2024-05-14 01:37:45.000000 resend-1.0.2/resend/version.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.900732 resend-1.0.2/resend.egg-info/
--rw-r--r--   0 derich     (501) staff       (20)     2430 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)      825 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/SOURCES.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/dependency_links.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/not-zip-safe
--rw-r--r--   0 derich     (501) staff       (20)       35 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/requires.txt
--rw-r--r--   0 derich     (501) staff       (20)        7 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/top_level.txt
--rw-r--r--   0 derich     (501) staff       (20)       67 2024-05-14 01:37:48.904498 resend-1.0.2/setup.cfg
--rw-r--r--   0 derich     (501) staff       (20)     1172 2024-05-14 01:16:37.000000 resend-1.0.2/setup.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.891757 resend-1.1.0/
+-rw-r--r--   0 derich     (501) staff       (20)     1070 2023-08-19 17:45:00.000000 resend-1.1.0/LICENSE.md
+-rw-r--r--   0 derich     (501) staff       (20)     2429 2024-05-17 21:47:27.891694 resend-1.1.0/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)     1626 2024-05-17 20:02:25.000000 resend-1.1.0/README.md
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.887871 resend-1.1.0/resend/
+-rw-r--r--   0 derich     (501) staff       (20)     1003 2024-05-14 01:16:37.000000 resend-1.1.0/resend/__init__.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.889125 resend-1.1.0/resend/api_keys/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/api_keys/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)      998 2024-05-09 01:36:14.000000 resend-1.1.0/resend/api_keys/_api_key.py
+-rw-r--r--   0 derich     (501) staff       (20)     2310 2024-05-09 01:36:14.000000 resend-1.1.0/resend/api_keys/_api_keys.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.889551 resend-1.1.0/resend/audiences/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/audiences/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1192 2024-05-09 01:36:14.000000 resend-1.1.0/resend/audiences/_audience.py
+-rw-r--r--   0 derich     (501) staff       (20)     2305 2024-05-09 01:36:14.000000 resend-1.1.0/resend/audiences/_audiences.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.889973 resend-1.1.0/resend/contacts/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/contacts/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1795 2024-05-09 01:36:14.000000 resend-1.1.0/resend/contacts/_contact.py
+-rw-r--r--   0 derich     (501) staff       (20)     4400 2024-05-09 01:36:14.000000 resend-1.1.0/resend/contacts/_contacts.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.890562 resend-1.1.0/resend/domains/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/domains/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1987 2024-05-09 01:36:14.000000 resend-1.1.0/resend/domains/_domain.py
+-rw-r--r--   0 derich     (501) staff       (20)     3887 2024-05-09 01:36:14.000000 resend-1.1.0/resend/domains/_domains.py
+-rw-r--r--   0 derich     (501) staff       (20)     1416 2024-05-09 01:36:14.000000 resend-1.1.0/resend/domains/_record.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.891411 resend-1.1.0/resend/emails/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/emails/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)      489 2024-05-09 01:36:14.000000 resend-1.1.0/resend/emails/_attachment.py
+-rw-r--r--   0 derich     (501) staff       (20)      962 2024-05-17 20:02:25.000000 resend-1.1.0/resend/emails/_batch.py
+-rw-r--r--   0 derich     (501) staff       (20)     2862 2024-05-17 20:02:25.000000 resend-1.1.0/resend/emails/_email.py
+-rw-r--r--   0 derich     (501) staff       (20)     2832 2024-05-17 20:02:25.000000 resend-1.1.0/resend/emails/_emails.py
+-rw-r--r--   0 derich     (501) staff       (20)      524 2024-05-09 01:36:14.000000 resend-1.1.0/resend/emails/_tag.py
+-rw-r--r--   0 derich     (501) staff       (20)     6108 2024-05-17 20:02:25.000000 resend-1.1.0/resend/exceptions.py
+-rw-r--r--   0 derich     (501) staff       (20)        0 2023-08-19 17:45:00.000000 resend-1.1.0/resend/py.typed
+-rw-r--r--   0 derich     (501) staff       (20)     2353 2024-05-17 20:02:25.000000 resend-1.1.0/resend/request.py
+-rw-r--r--   0 derich     (501) staff       (20)      448 2024-05-17 20:02:25.000000 resend-1.1.0/resend/utils.py
+-rw-r--r--   0 derich     (501) staff       (20)      133 2024-05-17 21:47:23.000000 resend-1.1.0/resend/version.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.888685 resend-1.1.0/resend.egg-info/
+-rw-r--r--   0 derich     (501) staff       (20)     2429 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)      841 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-14 01:37:48.000000 resend-1.1.0/resend.egg-info/not-zip-safe
+-rw-r--r--   0 derich     (501) staff       (20)       35 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/requires.txt
+-rw-r--r--   0 derich     (501) staff       (20)        7 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/top_level.txt
+-rw-r--r--   0 derich     (501) staff       (20)       67 2024-05-17 21:47:27.892583 resend-1.1.0/setup.cfg
+-rw-r--r--   0 derich     (501) staff       (20)     1172 2024-05-14 01:16:37.000000 resend-1.1.0/setup.py
```

### Comparing `resend-1.0.2/LICENSE.md` & `resend-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/PKG-INFO` & `resend-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.0.2
+Version: 1.1.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 Keywords: email,email platform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,15 @@
 ```py
 import os
 import resend
 
 resend.api_key = "re_yourkey"
 
 params: resend.Emails.SendParams = {
-    "sender": "onboarding@resend.dev",
+    "from_": "onboarding@resend.dev",
     "to": ["delivered@resend.dev"],
     "subject": "hi",
     "html": "<strong>hello, world!</strong>",
     "reply_to": "to@gmail.com",
     "bcc": "bcc@resend.dev",
     "cc": ["cc@resend.dev"],
     "tags": [
```

### Comparing `resend-1.0.2/README.md` & `resend-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ```py
 import os
 import resend
 
 resend.api_key = "re_yourkey"
 
 params: resend.Emails.SendParams = {
-    "sender": "onboarding@resend.dev",
+    "from_": "onboarding@resend.dev",
     "to": ["delivered@resend.dev"],
     "subject": "hi",
     "html": "<strong>hello, world!</strong>",
     "reply_to": "to@gmail.com",
     "bcc": "bcc@resend.dev",
     "cc": ["cc@resend.dev"],
     "tags": [
```

### Comparing `resend-1.0.2/resend/__init__.py` & `resend-1.1.0/resend/__init__.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/api_keys/_api_key.py` & `resend-1.1.0/resend/api_keys/_api_key.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/api_keys/_api_keys.py` & `resend-1.1.0/resend/api_keys/_api_keys.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/audiences/_audience.py` & `resend-1.1.0/resend/audiences/_audience.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/audiences/_audiences.py` & `resend-1.1.0/resend/audiences/_audiences.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/contacts/_contact.py` & `resend-1.1.0/resend/contacts/_contact.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/contacts/_contacts.py` & `resend-1.1.0/resend/contacts/_contacts.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/domains/_domain.py` & `resend-1.1.0/resend/domains/_domain.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/domains/_domains.py` & `resend-1.1.0/resend/domains/_domains.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/domains/_record.py` & `resend-1.1.0/resend/domains/_record.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/emails/_batch.py` & `resend-1.1.0/resend/emails/_batch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, List, cast
 
 from resend import request
+from resend.utils import replace_params
 
 from ._email import Email
 from ._emails import Emails
 
 
 class Batch:
     @classmethod
@@ -16,11 +17,15 @@
         Args:
             params (List[Emails.SendParams]): The list of emails to send
 
         Returns:
             List[Email]: A list of email objects
         """
         path = "/emails/batch"
-        resp = request.Request(
-            path=path, params=cast(Dict[Any, Any], params), verb="post"
-        ).perform()
+
+        # loop through the list of params and replace "from_" or "sender" with "from"
+        replaced_params = [
+            replace_params(cast(Dict[Any, Any], param)) for param in params
+        ]
+
+        resp = request.Request(path=path, params=replaced_params, verb="post").perform()
         return [Email.new_from_request(val) for val in resp["data"]]
```

### Comparing `resend-1.0.2/resend/emails/_email.py` & `resend-1.1.0/resend/emails/_email.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,24 @@
     """
     The Email ID.
     """
     to: Union[List[str], str]
     """
     List of email addresses to send the email to.
     """
+    from_: str
+    """
+    The email address of the sender.
+    "from" is a reserved keyword in python.
+    So accept either "from_" or "sender"
+    """
     sender: str
     """
     The email address of the sender. "from" is a reserved keyword in python.
-    So we use "sender" here instead
+    So accept either "from_" or "sender"
     """
     created_at: str
     """
     When the email was created.
     """
     subject: str
     """
@@ -48,26 +54,28 @@
     The last event of the email.
     """
 
     def __init__(
         self,
         id: str,
         to: Union[List[str], str],
+        from_: str,
         sender: str,
         created_at: str,
         subject: str,
         html: str,
         text: str,
         bcc: Union[List[str], str],
         cc: Union[List[str], str],
         reply_to: Union[List[str], str],
         last_event: str,
     ):
         self.id = id
         self.to = to
+        self.from_ = from_
         self.sender = sender
         self.created_at = created_at
         self.subject = subject
         self.html = html
         self.text = text
         self.bcc = bcc
         self.cc = cc
@@ -86,14 +94,15 @@
             Email: The new Email object
         """
         email = Email(
             id=val["id"] if "id" in val else "",
             to=val["to"] if "to" in val else "",
             # we set sender as the value from "from" here
             # because "from" is a reserved keyword in python
+            from_=val["from"] if "from" in val else "",
             sender=val["from"] if "from" in val else "",
             created_at=val["created_at"] if "created_at" in val else "",
             subject=val["subject"] if "subject" in val else "",
             html=val["html"] if "html" in val else "",
             text=val["text"] if "text" in val else "",
             bcc=val["bcc"] if "bcc" in val else "",
             cc=val["cc"] if "cc" in val else "",
```

### Comparing `resend-1.0.2/resend/emails/_emails.py` & `resend-1.1.0/resend/emails/_emails.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,30 @@
 
 from typing_extensions import NotRequired, TypedDict
 
 from resend import request
 from resend.emails._attachment import Attachment
 from resend.emails._email import Email
 from resend.emails._tag import Tag
+from resend.utils import replace_params
 
 
 class Emails:
     class SendParams(TypedDict):
-        sender: str
+        from_: NotRequired[str]
         """
         The email address of the sender.
-        "from" is a reserved keyword in python, so we use "sender" here instead
+        "from" is a reserved keyword in python.
+        So we accept either "from_" or "sender"
+        """
+        sender: NotRequired[str]
+        """
+        The email address of the sender.
+        "from" is a reserved keyword in python.
+        So we accept either "from_" or "sender"
         """
         to: Union[str, List[str]]
         """
         List of email addresses to send the email to.
         """
         subject: str
         """
@@ -66,21 +74,19 @@
             params (SendParams): The email parameters
 
         Returns:
             Email: The email object that was sent
         """
         path = "/emails"
 
-        # we need this workaround here because from is a reserved keyword
-        # in python, so we need to use "sender" on the SendParams
-        params["from"] = params["sender"]  # type: ignore
+        # replace "from_" or "sender" with "from"
+        p = replace_params(cast(Dict[Any, Any], params))
+
         return Email.new_from_request(
-            request.Request(
-                path=path, params=cast(Dict[Any, Any], params), verb="post"
-            ).perform()
+            request.Request(path=path, params=p, verb="post").perform()
         )
 
     @classmethod
     def get(cls, email_id: str) -> Email:
         """
         Retrieve a single email.
         see more: https://resend.com/docs/api-reference/emails/retrieve-email
```

### Comparing `resend-1.0.2/resend/emails/_tag.py` & `resend-1.1.0/resend/emails/_tag.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.2/resend/exceptions.py` & `resend-1.1.0/resend/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,17 @@
     },
     "401": {"missing_api_key": MissingApiKeyError},
     "403": {"invalid_api_key": InvalidApiKeyError},
     "500": {"application_error": ApplicationError},
 }
 
 
-def raise_for_code_and_type(code: Union[str, int], error_type: str, message: str) -> None:
+def raise_for_code_and_type(
+    code: Union[str, int], error_type: str, message: str
+) -> None:
     """Raise the appropriate error based on the code and type.
 
     Args:
         code (str): The error code
         error_type (str): The error type
         message (str): The error message
```

### Comparing `resend-1.0.2/resend/request.py` & `resend-1.1.0/resend/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import resend
 from resend.exceptions import raise_for_code_and_type
 from resend.version import get_version
 
 
 # This class wraps the HTTP request creation logic
 class Request:
-    def __init__(self, path: str, params: Dict[Any, Any], verb: str):
+
+    def __init__(self, path: str, params: Any, verb: str):
         self.path = path
         self.params = params
         self.verb = verb
 
     def perform(self) -> Any:
         """Is the main function that makes the HTTP request
         to the Resend API. It uses the path, params, and verb attributes
```

### Comparing `resend-1.0.2/resend.egg-info/PKG-INFO` & `resend-1.1.0/resend.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.0.2
+Version: 1.1.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 Keywords: email,email platform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,15 @@
 ```py
 import os
 import resend
 
 resend.api_key = "re_yourkey"
 
 params: resend.Emails.SendParams = {
-    "sender": "onboarding@resend.dev",
+    "from_": "onboarding@resend.dev",
     "to": ["delivered@resend.dev"],
     "subject": "hi",
     "html": "<strong>hello, world!</strong>",
     "reply_to": "to@gmail.com",
     "bcc": "bcc@resend.dev",
     "cc": ["cc@resend.dev"],
     "tags": [
```

### Comparing `resend-1.0.2/resend.egg-info/SOURCES.txt` & `resend-1.1.0/resend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 resend/__init__.py
 resend/exceptions.py
 resend/py.typed
 resend/request.py
+resend/utils.py
 resend/version.py
 resend.egg-info/PKG-INFO
 resend.egg-info/SOURCES.txt
 resend.egg-info/dependency_links.txt
 resend.egg-info/not-zip-safe
 resend.egg-info/requires.txt
 resend.egg-info/top_level.txt
```

### Comparing `resend-1.0.2/setup.py` & `resend-1.1.0/setup.py`

 * *Files identical despite different names*

