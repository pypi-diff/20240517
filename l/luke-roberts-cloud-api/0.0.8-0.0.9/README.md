# Comparing `tmp/luke_roberts_cloud_api-0.0.8.tar.gz` & `tmp/luke_roberts_cloud_api-0.0.9.tar.gz`

## Comparing `luke_roberts_cloud_api-0.0.8.tar` & `luke_roberts_cloud_api-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/const.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/lamp.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/luke_roberts_cloud.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/tests/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/LICENSE
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/src/luke_roberts_cloud_api/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/src/luke_roberts_cloud_api/const.py
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/src/luke_roberts_cloud_api/lamp.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/src/luke_roberts_cloud_api/luke_roberts_cloud.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/tests/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/LICENSE
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.9/PKG-INFO
```

### Comparing `luke_roberts_cloud_api-0.0.8/.github/workflows/python-app.yml` & `luke_roberts_cloud_api-0.0.9/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.8/.github/workflows/python-publish.yml` & `luke_roberts_cloud_api-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/lamp.py` & `luke_roberts_cloud_api-0.0.9/src/luke_roberts_cloud_api/lamp.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,25 +23,24 @@
         self._headers = headers
 
     async def _send_command(self, body):
         url = f"{BASE_URL}/lamps/{self._id}/command"
         # res = req.put(url=url, headers=self._headers, json=body, timeout=10)
         async with aiohttp.ClientSession() as session:
             async with session.put(url, headers=self._headers, json=body, timeout=10) as response:
-                res = await response.json()
-                if not res.ok:
-                    raise Exception(res.text)
+                if not response.ok:
+                    raise Exception(response.text)
 
     async def _get_state(self):
         url = f"{BASE_URL}/lamps/{self._id}/state"
         async with aiohttp.ClientSession() as session:
             async with session.get(url, headers=self._headers, timeout=10) as response:
                 if not response.ok:
                     raise Exception(response.text)
-                res = await response.json()
+                return await response.json()
 
     def getName(self):
         return self._name
 
     def getSerialNumber(self):
         return self._serial_number
 
@@ -87,15 +86,15 @@
         if scene > 31:
             scene = 31
         body = {"scene": scene}
         await self._send_command(body)
         await self.refresh()
 
     async def refresh(self):
-        state = self._get_state()
+        state = await self._get_state()
         self.brightness = state["brightness"]
         self.colortemp_kelvin = state["color"]["temperatureK"]
         self.power = state["on"]
         return self
 
     def __str__(self):
         return (f"{self._name}, "
```

### Comparing `luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/luke_roberts_cloud.py` & `luke_roberts_cloud_api-0.0.9/src/luke_roberts_cloud_api/luke_roberts_cloud.py`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.8/LICENSE` & `luke_roberts_cloud_api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.8/README.md` & `luke_roberts_cloud_api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.8/pyproject.toml` & `luke_roberts_cloud_api-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"#
 
 [project]
 name = "luke_roberts_cloud_api"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Julian Lenzenweger", email="j.lenzenweger@gmail.com" },
 ]
 description = "Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `luke_roberts_cloud_api-0.0.8/PKG-INFO` & `luke_roberts_cloud_api-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: luke_roberts_cloud_api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer.
 Project-URL: Homepage, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/tree/main
 Project-URL: Issues, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/issues
 Author-email: Julian Lenzenweger <j.lenzenweger@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

