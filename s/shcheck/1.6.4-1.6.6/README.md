# Comparing `tmp/shcheck-1.6.4.tar.gz` & `tmp/shcheck-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shcheck-1.6.4.tar", last modified: Tue May  7 05:21:39 2024, max compression
+gzip compressed data, was "shcheck-1.6.6.tar", last modified: Fri May 17 13:01:04 2024, max compression
```

## Comparing `shcheck-1.6.4.tar` & `shcheck-1.6.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:21:39.637315 shcheck-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-07 05:21:35.000000 shcheck-1.6.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-07 05:21:39.637315 shcheck-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-07 05:21:35.000000 shcheck-1.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 05:21:39.637315 shcheck-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-07 05:21:35.000000 shcheck-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:21:39.637315 shcheck-1.6.4/shcheck/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:21:35.000000 shcheck-1.6.4/shcheck/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16364 2024-05-07 05:21:35.000000 shcheck-1.6.4/shcheck/shcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:21:39.637315 shcheck-1.6.4/shcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-07 05:21:39.000000 shcheck-1.6.4/shcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-07 05:21:39.000000 shcheck-1.6.4/shcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 05:21:39.000000 shcheck-1.6.4/shcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 05:21:39.000000 shcheck-1.6.4/shcheck.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      818 2024-05-07 05:21:35.000000 shcheck-1.6.4/shcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:21:39.637315 shcheck-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-07 05:21:35.000000 shcheck-1.6.4/tests/test_shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:01:04.082535 shcheck-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-17 13:00:59.000000 shcheck-1.6.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-17 13:01:04.082535 shcheck-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-17 13:00:59.000000 shcheck-1.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:01:04.082535 shcheck-1.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-17 13:00:59.000000 shcheck-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:01:04.082535 shcheck-1.6.6/shcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:00:59.000000 shcheck-1.6.6/shcheck/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16342 2024-05-17 13:00:59.000000 shcheck-1.6.6/shcheck/shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:01:04.082535 shcheck-1.6.6/shcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-17 13:01:04.000000 shcheck-1.6.6/shcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-17 13:01:04.000000 shcheck-1.6.6/shcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:01:04.000000 shcheck-1.6.6/shcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 13:01:04.000000 shcheck-1.6.6/shcheck.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      818 2024-05-17 13:00:59.000000 shcheck-1.6.6/shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:01:04.082535 shcheck-1.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-17 13:00:59.000000 shcheck-1.6.6/tests/test_shcheck.py
```

### Comparing `shcheck-1.6.4/LICENSE.txt` & `shcheck-1.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shcheck-1.6.4/PKG-INFO` & `shcheck-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcheck
-Version: 1.6.4
+Version: 1.6.6
 Summary: A basic tool to check security headers of a website
 Home-page: https://github.com/santoru/shcheck
 Author: santoru
 Author-email: santoru@pm.me
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shcheck Version: 1.6.4 Summary: A basic tool to
+Metadata-Version: 2.1 Name: shcheck Version: 1.6.6 Summary: A basic tool to
 check security headers of a website Home-page: https://github.com/santoru/
 shcheck Author: santoru Author-email: santoru@pm.me Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE.txt # shcheck -
 Security Header Check
                    _[_P_y_P_I_]_[_P_y_p_i_]_[_U_p_d_a_t_e_d_][Output on Facebook]
 ## Check security headers on a target website I did this tool to help me to
 check which security headers are enabled on certain websites. The tool is very
```

### Comparing `shcheck-1.6.4/README.md` & `shcheck-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `shcheck-1.6.4/setup.py` & `shcheck-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import setup
 
 PACKAGE_NAME = "shcheck"
-VERSION = "1.6.4"
+VERSION = "1.6.6"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def parse_requirements(filename):
     """Load requirements from a pip requirements file."""
```

### Comparing `shcheck-1.6.4/shcheck/shcheck.py` & `shcheck-1.6.6/shcheck/shcheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         log("[*] Effective URL: {}".format(colorize(rUrl, 'info')))
         parse_headers(response.getheaders())
         json_headers[f"{rUrl}"] = json_results
         json_results["present"] = {}
         json_results["missing"] = []
 
         # Before parsing, remove X-Frame-Options if there's CSP with frame-ancestors directive
-        if "Content-Security-Policy".lower() in str(headers).lower() and "frame-ancestors" in headers.get('Content-Security-Policy'.lower()).lower():
+        if "content-security-policy" in headers.keys() and "frame-ancestors" in headers.get("content-security-policy").lower():
             sec_headers.pop("X-Frame-Options", None)
             headers.pop("X-Frame-Options".lower(), None)
 
         for safeh in sec_headers:
             lsafeh = safeh.lower()
             if lsafeh in headers:
                 safe += 1
```

### Comparing `shcheck-1.6.4/shcheck.egg-info/PKG-INFO` & `shcheck-1.6.6/shcheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcheck
-Version: 1.6.4
+Version: 1.6.6
 Summary: A basic tool to check security headers of a website
 Home-page: https://github.com/santoru/shcheck
 Author: santoru
 Author-email: santoru@pm.me
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shcheck Version: 1.6.4 Summary: A basic tool to
+Metadata-Version: 2.1 Name: shcheck Version: 1.6.6 Summary: A basic tool to
 check security headers of a website Home-page: https://github.com/santoru/
 shcheck Author: santoru Author-email: santoru@pm.me Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE.txt # shcheck -
 Security Header Check
                    _[_P_y_P_I_]_[_P_y_p_i_]_[_U_p_d_a_t_e_d_][Output on Facebook]
 ## Check security headers on a target website I did this tool to help me to
 check which security headers are enabled on certain websites. The tool is very
```

### Comparing `shcheck-1.6.4/shcheck.py` & `shcheck-1.6.6/shcheck.py`

 * *Files identical despite different names*

