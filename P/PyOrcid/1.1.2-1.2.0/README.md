# Comparing `tmp/pyorcid-1.1.2.tar.gz` & `tmp/pyorcid-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorcid-1.1.2.tar", max compression
+gzip compressed data, was "pyorcid-1.2.0.tar", max compression
```

## Comparing `pyorcid-1.1.2.tar` & `pyorcid-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1095 2023-08-22 23:55:20.259478 pyorcid-1.1.2/LICENSE
--rw-r--r--   0        0        0      718 2023-09-13 20:26:53.823355 pyorcid-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     8266 2023-09-13 20:20:08.416755 pyorcid-1.1.2/README.md
--rw-r--r--   0        0        0      122 2023-09-11 17:31:25.316280 pyorcid-1.1.2/src/pyorcid/__init__.py
--rw-r--r--   0        0        0    24378 2023-09-13 16:49:38.917814 pyorcid-1.1.2/src/pyorcid/orcid.py
--rw-r--r--   0        0        0     5087 2023-09-13 20:32:54.422039 pyorcid-1.1.2/src/pyorcid/orcid_authentication.py
--rw-r--r--   0        0        0     4259 2023-09-12 02:21:05.666755 pyorcid-1.1.2/src/pyorcid/orcid_scrapper.py
--rw-r--r--   0        0        0     8971 1970-01-01 00:00:00.000000 pyorcid-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-08-22 23:55:20.259478 pyorcid-1.2.0/LICENSE
+-rw-r--r--   0        0        0      714 2024-05-17 21:23:20.842963 pyorcid-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8603 2024-05-17 21:13:32.757217 pyorcid-1.2.0/README.md
+-rw-r--r--   0        0        0      161 2024-05-17 21:13:32.758561 pyorcid-1.2.0/src/pyorcid/__init__.py
+-rw-r--r--   0        0        0    27028 2024-05-17 21:13:32.759568 pyorcid-1.2.0/src/pyorcid/orcid.py
+-rw-r--r--   0        0        0     5341 2024-05-17 21:13:32.760653 pyorcid-1.2.0/src/pyorcid/orcid_authentication.py
+-rw-r--r--   0        0        0     4259 2023-09-12 02:21:05.666755 pyorcid-1.2.0/src/pyorcid/orcid_scrapper.py
+-rw-r--r--   0        0        0     6506 2024-05-17 21:13:32.761661 pyorcid-1.2.0/src/pyorcid/orcid_search.py
+-rw-r--r--   0        0        0     9301 1970-01-01 00:00:00.000000 pyorcid-1.2.0/PKG-INFO
```

### Comparing `pyorcid-1.1.2/LICENSE` & `pyorcid-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorcid-1.1.2/pyproject.toml` & `pyorcid-1.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "PyOrcid"
-version = "1.1.2"
+version = "1.2.0"
 license = "MIT"
 description = "API client for ORCID API"
 readme = "README.md"
 authors = ["Sriram Seelamneni <srirams0606@gmail.com>"]
 repository = "https://github.com/sri0606/PyOrcid"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -22,9 +22,7 @@
 python-dotenv = "*"
 urllib3 = "^1.26.7"
 requests = "^2.26.0"
 xmltojson = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
-
-
```

### Comparing `pyorcid-1.1.2/README.md` & `pyorcid-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -122,26 +122,32 @@
     print(key, value)
 ```
 ```python
 
 # Generate a markdown file with the summary of various section's data
 orcid.generate_markdown_file(output_file = "md_generator_example.md")
 ```
-
+#### Searching ORCID records
+```python
+from pyorcid import OrcidSearch
+#search through ORCID records, for details on the query format see https://info.orcid.org/documentation/api-tutorials/api-tutorial-searching-the-orcid-registry/  
+orcidSearch = OrcidSearch(orcid_access_token=access_token)
+orcidSearch.search("John Smith")
+```
 ## Access through OrcidScrapper feature of PyOrcid
 This is an alternative to Orcid API. You can only read the orcid profiles on public database. All you need is the Orcid ID of the researchers you wish to retrieve.
 OrcidScrapper can access all methods of Orcid class as it is inherited from it.
 
 ```python
 from src import pyorcid
-orcid_id = '0000-0003-0666-9883'
+orcid_id = 'xxxx-xxxx-xxxx-xxxx'
 orcid = pyorcid.OrcidScrapper(orcid_id=orcid_id)
 orcid.__dir__()
 ```
 ```
 works_data = orcid.works()[0]
 for key, value in works_data.items():
     print(key, value)
 
 orcid.record_summary()
 
-```
+```
```

### Comparing `pyorcid-1.1.2/src/pyorcid/orcid.py` & `pyorcid-1.2.0/src/pyorcid/orcid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import requests
 from dotenv import load_dotenv
 import os
+from datetime import datetime
 
 class Orcid():
     '''
     This is a wrapper class for ORCID API
     '''
-    def __init__(self,orcid_id, orcid_access_token = " ", state="public") -> None:
+    def __init__(self,orcid_id, orcid_access_token = " ", state="public", sandbox=False) -> None:
         '''
         Initialize orcid instance
         orcid_id : Orcid ID of the user
         orcid_access_token : Orcid access token obtained from the user with this orcid_id
         state  : Whether to use public or member API of ORCID
+        sandbox : a boolean value to show if the ORCID sandbox API should be used (default: False)
         '''
         self._orcid_id = orcid_id
         self._orcid_access_token = orcid_access_token
         self._state = state
+        self._sandbox = sandbox
         #For testing purposes (pytesting on github workflow)
         if orcid_access_token!=" ":
             try:
                 self.__test_is_access_token_valid()
             except:
                 if not self.__is_access_token_valid():
                     raise ValueError(f"Invalid access token! Please make sure the user with ORCID_ID:{orcid_id} has given access.")
@@ -40,20 +43,22 @@
             'Content-Type': 'application/json'
         }
 
         api_url = ""
 
         if self._state == "public":
             # Specify the ORCID record endpoint for the desired ORCID iD
-            # api_url = f'https://pub.sandbox.orcid.org/v3.0/{self._orcid_id}'  #for testing
             api_url = f'https://pub.orcid.org/v3.0/{self._orcid_id}'
+            if(self._sandbox):
+                api_url = f'https://pub.sandbox.orcid.org/v3.0/{self._orcid_id}'  #for testing
 
         elif self._state == "member":
-            # api_url = f'https://api.sandbox.orcid.org/v3.0/{self._orcid_id}'  #for testing
             api_url = f'https://api.orcid.org/v3.0/{self._orcid_id}'
+            if(self._sandbox):
+                api_url = f'https://api.sandbox.orcid.org/v3.0/{self._orcid_id}'  #for testing
 
         response = requests.get(api_url, headers=headers)
 
         if response.status_code == 404:
             # The request was successful, and the token is likely valid
             return False
         else:
@@ -74,33 +79,74 @@
             'Authorization': f'Bearer {access_token}',
             'Content-Type': 'application/json'
         }
         api_url = ""
 
         if self._state == "public":
             # Specify the ORCID record endpoint for the desired ORCID iD
-            # api_url = f'https://pub.sandbox.orcid.org/v3.0/{self._orcid_id}'  #for testing
             api_url = f'https://pub.orcid.org/v3.0/{self._orcid_id}/{section}'
+            if(self._sandbox):
+                api_url = f'https://pub.sandbox.orcid.org/v3.0/{self._orcid_id}/{section}'  #for testing
 
         elif self._state == "member":
-            # api_url = f'https://api.sandbox.orcid.org/v3.0/{self._orcid_id}'  #for testing
             api_url = f'https://api.orcid.org/v3.0/{self._orcid_id}/{section}'
+            if(self._sandbox):
+                api_url = f'https://api.sandbox.orcid.org/v3.0/{self._orcid_id}/{section}'  #for testing
+
 
         # Make a GET request to retrieve the ORCID record
         response = requests.get(api_url, headers=headers)
 
         # The request was successful
         data = response.json()
         # Check the response status code
         if response.status_code == 200 or data is not None:
             return data
         else:
             # Handle the case where the request failed
             print("Failed to retrieve ORCID data. Status code:", response.status_code)
             return None
+        
+    def __timestamp_to_iso_date(self, timestamp):
+        '''
+        Converts a timestamp to an ISO date string
+        return : ISO date string
+        '''
+        try:
+            # Check if timestamp is a valid number
+            timestamp = float(timestamp)
+        except ValueError:
+            raise ValueError("Error: Invalid timestamp")
+
+        try:
+            # Convert the timestamp to seconds (from milliseconds if necessary)
+            if timestamp > 1e10:  # timestamp is likely in milliseconds
+                timestamp /= 1000
+
+            # Create a datetime object from the timestamp
+            dt = datetime.fromtimestamp(timestamp)
+
+            # Convert the datetime object to an ISO 8601 string
+            iso8601 = dt.isoformat()
+            return iso8601
+        except Exception as e:
+            raise ValueError(f"Error: {e}")
+        
+    def __deunicode_string(self, s):
+        '''
+        Removes non-ASCII characters from a string
+        return : a string with only ASCII characters
+        '''
+        try:
+            # Check if string contains any non-ASCII characters
+            s.encode('ascii')
+        except UnicodeEncodeError:
+            # String contains non-ASCII characters, remove them
+            s = s.encode('ascii', 'ignore').decode('ascii')
+        return s
 
     def record(self):
         '''
         Reads the Orcid record
         return  : a dictionary of summary view of the full ORCID record 
         '''
         return self.__read_section("record")
@@ -157,15 +203,15 @@
         data =  self.__read_section("keywords")
         lis = [(value["content"]) for value in data["keyword"]] 
 
         return (lis, data)
      
     def other_names(self):
         '''
-        Other names by which the researcher is know
+        Other names by which the researcher is known
         return  :
         '''
         return self.__read_section("other-names") 
     
     def personal_details(self):
         '''
         Personal details: the researcher's name, credit (published) name, and biography
@@ -224,15 +270,15 @@
 
             for fund_summary in funding_summaries:
                 title       = self.__get_value_from_keys(fund_summary,["title","title","value"])
                 fund_type   = self.__get_value_from_keys(fund_summary,["type"])
                 start_date  = self.get_formatted_date(fund_summary.get('start-date', {}))
                 end_date    = self.get_formatted_date(fund_summary.get('end-date', {}))
                 organization= self.__get_value_from_keys(fund_summary,["organization","name"])
-                organization_address = ', '.join(filter(None, self.__get_value_from_keys(fund_summary, ["organization", "address"]).values())) if self.__get_value_from_keys(fund_summary, ["organization", "address"]) is not None else ''
+                organization_address = self.__org_string_from_obj(self.__get_value_from_keys(fund_summary, ["organization", "address"]))
                 url         = self.__get_value_from_keys(fund_summary,["url","value"])
 
                 funding_detail = {
                     'title': title,
                     'type': fund_type,
                     'start-date': start_date,
                     'end-date': end_date,
@@ -267,15 +313,15 @@
 
             for work_summary in work_summaries:
                 title           = self.__get_value_from_keys(work_summary,["title","title","value"])
                 work_type       = self.__get_value_from_keys(work_summary,["type"])
                 publication_date= self.get_formatted_date(work_summary.get('publication-date', {}))
                 journal_title   = self.__get_value_from_keys(work_summary,["journal-title","value"])
                 organization    = self.__get_value_from_keys(work_summary,["organization","name"])
-                organization_address = ', '.join(filter(None, self.__get_value_from_keys(work_summary, ["organization", "address"]).values())) if self.__get_value_from_keys(work_summary, ["organization", "address"]) is not None else ''
+                organization_address = self.__org_string_from_obj(self.__get_value_from_keys(work_summary, ["organization", "address"]))
                 url             = self.__get_value_from_keys(work_summary,["url","value"])
 
                 work_detail = {
                     'title': title,
                     'type': work_type,
                     'publication-date': publication_date,
                     'journal title': journal_title,
@@ -392,29 +438,31 @@
             if isinstance(current_obj, dict) and key in current_obj:
                 current_obj = current_obj[key]
             else:
                 return False
 
         return True
 
-    def __get_value_from_keys(self,json_obj, keys):
+    def __get_value_from_keys(self, json_obj, keys):
         """
         Get the value associated with the last key in the list if all keys are accessible cumulatively.
 
         Args:
         json_obj (dict): The JSON-like object (dictionary).
         keys (list): List of keys to check for accessibility and retrieve the final value.
 
         Returns:
         Any: The value associated with the last key if all keys are accessible cumulatively, or None if not accessible.
         """
         if self.__are_keys_accessible(json_obj, keys):
             current_obj = json_obj
             for key in keys:
                 current_obj = current_obj[key]
+            if isinstance(current_obj, str):
+                current_obj = self.__deunicode_string(current_obj)
             return current_obj
         else:
             return None
         
     def __extract_details(self, data, key):
         '''
         Helper function for record_summary()
@@ -430,39 +478,62 @@
             for summary in summaries:
                 key_summary = summary.get(f'{key}-summary', {})
                 department  = self.__get_value_from_keys(key_summary,["department-name"])
                 role        = self.__get_value_from_keys(key_summary,["role-title"])
                 start_date  = self.get_formatted_date(key_summary.get('start-date', {}))
                 end_date    = self.get_formatted_date(key_summary.get('end-date', {}))
                 organization = self.__get_value_from_keys(key_summary,["organization","name"])
-                organization_address = ', '.join(filter(None, self.__get_value_from_keys(key_summary, ["organization", "address"]).values())) if self.__get_value_from_keys(key_summary, ["organization", "address"]) is not None else ''
+                
+                # Extract the organization address components into a string
+                organization_address = self.__org_string_from_obj(self.__get_value_from_keys(key_summary, ["organization", "address"]))
+
                 url  = self.__get_value_from_keys(key_summary,["url","value"])
                 detail = {
                     'Department': department,
                     'Role': role,
                     'start-date': start_date,
                     'end-date': end_date,
                     'organization': organization,
                     'organization-address': organization_address,
                     'url': url,
                 }
                 
                 details.append(detail)
         
         return details
+    
+    def __org_string_from_obj(self, org_obj):
+        '''
+        Helper function for record_summary()
+        '''
+        org_string = ''
+        if not isinstance(org_obj, dict):
+            return org_string
+
+        # Build a string from the organization components without unicode characters
+        org_parts = filter(None, org_obj.values())
+        if org_parts is not None:
+            org_string = ', '.join([self.__deunicode_string(i) for i in org_parts])
+        
+        return org_string
 
 
     def record_summary(self):
         '''
         A cleaner version of Orcid record
         return  : a dictionary of summary view of the full ORCID record
         '''
         data = self.record()
         extracted_data = {
+            'ORCiD ID': self._orcid_id,
+            'Last Modified': self.__timestamp_to_iso_date(self.__get_value_from_keys(data,["history","last-modified-date","value"])),
             'Name': self.__get_value_from_keys(data,["person","name","given-names","value"]),
+            'Family Name': self.__get_value_from_keys(data,["person","name","family-name","value"]),
+            'Credit Name': self.__get_value_from_keys(data,["person","name","credit-name","value"]),
+            'Other Names': [name['content'] for name in self.__get_value_from_keys(data,["person","other-names","other-name"])],
             'Biography': self.__get_value_from_keys(data,["person","biography","content"]),
             'Emails': [email['email'] for email in self.__get_value_from_keys(data,["person","emails","email"])],
             'Research Tags (keywords)': [keyword['content'] for keyword in self.__get_value_from_keys(data,["person","keywords","keyword"])],
         }
 
         # Extract education details
         education_details = self.educations()[0]
```

### Comparing `pyorcid-1.1.2/src/pyorcid/orcid_authentication.py` & `pyorcid-1.2.0/src/pyorcid/orcid_authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,44 +3,47 @@
 
 class OrcidAuthentication:
     '''
     OrcidAuthentication is a class that handles the Orcid's OAuth 2.0 authorrization.
     The Orcid's OAuth 2.0 authorrization is used to access the ORCID record of the user that gave access.
     
     '''
-    def __init__(self, client_id, client_secret, redirect_uri=""):
+    def __init__(self, client_id, client_secret, redirect_uri="", sandbox=False):
         '''
         initializes the ORCidAuthentication and gets the access token
         Parameters
         ----------
         client_id : str : client id obtained from the registered application
         client_secret : str : client secret obtained from the registered application
         redirect_uri : str : redirect uri obtained from the registered application
+        sandbox : bool : a boolean value to show if the ORCID sandbox API should be used (default: False)
 
         '''
         self.__client_id = client_id
         self.__client_secret = client_secret
         self.__redirect_uri = redirect_uri
+        self.__sandbox = sandbox
         return None
     
     
     def get_private_access_token(self):
         '''
         Send a request for Orcid's OAuth 2.0 authorrization
         This method is used for Member API (read/update) and Public API's /read-limited scope
         Requires user authorization
         '''
 
-       # Set the necessary parameters
-        # auth_url_endpoint = "https://sandbox.orcid.org/oauth/authorize"   #for testing
-        # token_url = "https://sandbox.orcid.org/oauth/token"               #for testing
-
+        # Set the necessary parameters
         auth_url_endpoint = "https://orcid.org/oauth/authorize"
         token_url = "https://orcid.org/oauth/token"
 
+        if(self.__sandbox):
+            auth_url_endpoint = "https://sandbox.orcid.org/oauth/authorize"
+            token_url = "https://sandbox.orcid.org/oauth/token"
+
         # Step 1: Redirect the user to the authorization URL
         params = {
             'client_id': self.__client_id,
             'response_type': 'code',
             'redirect_uri': self.__redirect_uri,
             'scope': '/authenticate'
         }
@@ -69,14 +72,18 @@
         """
         This method gets token for reading public data (/read-public scope) from Orcid.
         Doesnt' require user authentication 
         return: access token
         """
         scope='/read-public'
         token_url = "https://orcid.org/oauth/token"
+        
+        if(self.__sandbox):
+            token_url = "https://sandbox.orcid.org/oauth/token"
+
         params = {
             'client_id': self.__client_id,
             'client_secret': self.__client_secret,
             'scope': scope,
             'grant_type': 'client_credentials'
         }
         headers = {'Accept': 'application/json'}
```

### Comparing `pyorcid-1.1.2/src/pyorcid/orcid_scrapper.py` & `pyorcid-1.2.0/src/pyorcid/orcid_scrapper.py`

 * *Files identical despite different names*

### Comparing `pyorcid-1.1.2/PKG-INFO` & `pyorcid-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOrcid
-Version: 1.1.2
+Version: 1.2.0
 Summary: API client for ORCID API
 Home-page: https://github.com/sri0606/PyOrcid
 License: MIT
 Keywords: orcid,orcid-api,pyorcid
 Author: Sriram Seelamneni
 Author-email: srirams0606@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -146,26 +146,33 @@
     print(key, value)
 ```
 ```python
 
 # Generate a markdown file with the summary of various section's data
 orcid.generate_markdown_file(output_file = "md_generator_example.md")
 ```
-
+#### Searching ORCID records
+```python
+from pyorcid import OrcidSearch
+#search through ORCID records, for details on the query format see https://info.orcid.org/documentation/api-tutorials/api-tutorial-searching-the-orcid-registry/  
+orcidSearch = OrcidSearch(orcid_access_token=access_token)
+orcidSearch.search("John Smith")
+```
 ## Access through OrcidScrapper feature of PyOrcid
 This is an alternative to Orcid API. You can only read the orcid profiles on public database. All you need is the Orcid ID of the researchers you wish to retrieve.
 OrcidScrapper can access all methods of Orcid class as it is inherited from it.
 
 ```python
 from src import pyorcid
-orcid_id = '0000-0003-0666-9883'
+orcid_id = 'xxxx-xxxx-xxxx-xxxx'
 orcid = pyorcid.OrcidScrapper(orcid_id=orcid_id)
 orcid.__dir__()
 ```
 ```
 works_data = orcid.works()[0]
 for key, value in works_data.items():
     print(key, value)
 
 orcid.record_summary()
 
 ```
+
```

