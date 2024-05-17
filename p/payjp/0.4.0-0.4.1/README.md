# Comparing `tmp/payjp-0.4.0.tar.gz` & `tmp/payjp-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payjp-0.4.0.tar", last modified: Wed Apr 10 02:25:12 2024, max compression
+gzip compressed data, was "payjp-0.4.1.tar", last modified: Fri May 17 02:23:58 2024, max compression
```

## Comparing `payjp-0.4.0.tar` & `payjp-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:25:12.427127 payjp-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 02:25:03.000000 payjp-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 02:25:12.427127 payjp-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 02:25:03.000000 payjp-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:25:12.427127 payjp-0.4.0/payjp/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:25:12.427127 payjp-0.4.0/payjp/test/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/test_requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33026 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:25:12.427127 payjp-0.4.0/payjp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:25:12.427127 payjp-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-10 02:25:03.000000 payjp-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:23:58.687333 payjp-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-17 02:23:47.000000 payjp-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-17 02:23:58.687333 payjp-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-17 02:23:47.000000 payjp-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:23:58.683333 payjp-0.4.1/payjp/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:23:58.687333 payjp-0.4.1/payjp/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/test/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/test/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/test/test_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33497 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/test/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 02:23:47.000000 payjp-0.4.1/payjp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 02:23:58.687333 payjp-0.4.1/payjp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-17 02:23:58.000000 payjp-0.4.1/payjp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-17 02:23:58.000000 payjp-0.4.1/payjp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 02:23:58.000000 payjp-0.4.1/payjp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 02:23:58.000000 payjp-0.4.1/payjp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 02:23:58.000000 payjp-0.4.1/payjp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 02:23:58.687333 payjp-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-17 02:23:47.000000 payjp-0.4.1/setup.py
```

### Comparing `payjp-0.4.0/LICENSE` & `payjp-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/README.md` & `payjp-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/payjp/__init__.py` & `payjp-0.4.1/payjp/__init__.py`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/payjp/api_requestor.py` & `payjp-0.4.1/payjp/api_requestor.py`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/payjp/error.py` & `payjp-0.4.1/payjp/error.py`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/payjp/http_client.py` & `payjp-0.4.1/payjp/http_client.py`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/payjp/resource.py` & `payjp-0.4.1/payjp/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,8 +432,20 @@
 
 
 class Term(ListableAPIResource):
     pass
 
 
 class Balance(ListableAPIResource):
-    pass
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        object.__setattr__(self, 'statement_urls', self.__statement_urls)
+
+    def __statement_urls(self, *args, **kwargs):
+        return self.__class__.statement_urls(self.get('id'), *args, **kwargs)
+
+    @classmethod
+    def statement_urls(cls, id, api_key=None, payjp_account=None, api_base=None, **params):
+        requestor = api_requestor.APIRequestor(api_key, account=payjp_account, api_base=api_base)
+        url = cls.class_url() + f'/{id}/statement_urls'
+        response, api_key = requestor.request('post', url, params)
+        return convert_to_payjp_object(response, api_key, payjp_account, api_base)
```

### Comparing `payjp-0.4.0/payjp/test/helper.py` & `payjp-0.4.1/payjp/test/helper.py`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/payjp/test/test_http_client.py` & `payjp-0.4.1/payjp/test/test_http_client.py`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/payjp/test/test_integration.py` & `payjp-0.4.1/payjp/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/payjp/test/test_requestor.py` & `payjp-0.4.1/payjp/test/test_requestor.py`

 * *Files identical despite different names*

### Comparing `payjp-0.4.0/payjp/test/test_resources.py` & `payjp-0.4.1/payjp/test/test_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1206,10 +1206,25 @@
         self.requestor_mock.request.assert_called_with(
             'post',
             '/v1/statements/st_xxx/statement_urls',
             {},
             None
         )
 
+    def test_statement_urls(self):
+        payjp.Balance.statement_urls('ba_xxx')
+        self.requestor_mock.request.assert_called_with(
+            'post',
+            '/v1/balances/ba_xxx/statement_urls',
+            {},
+        )
+
+        balance = payjp.Balance.retrieve('ba_xxx')
+        balance.statement_urls()
+        self.requestor_mock.request.assert_called_with(
+            'post',
+            '/v1/balances/ba_xxx/statement_urls',
+            {},
+        )
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `payjp-0.4.0/setup.py` & `payjp-0.4.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     raise DeprecationWarning('Python 2.6 and older are no longer supported by PAY.JP. ')
 
 install_requires.append('requests >= 2.7.0')
 install_requires.append('six >= 1.9.0')
 
 setup(
     name="payjp",
-    version="0.4.0",
+    version="0.4.1",
     description='PAY.JP python bindings',
     author="PAY.JP",
     author_email='support@pay.jp',
     packages=['payjp', 'payjp.test'],
     url='https://github.com/payjp/payjp-python',
     install_requires=install_requires,
     tests_require=[
```

