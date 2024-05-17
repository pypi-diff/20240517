# Comparing `tmp/PyTransportNSWv2-0.2.3.tar.gz` & `tmp/PyTransportNSWv2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyTransportNSWv2-0.2.3.tar", last modified: Sun Jun 28 08:20:05 2020, max compression
+gzip compressed data, was "dist/PyTransportNSWv2-0.2.4.tar", last modified: Sun Jun 28 10:00:55 2020, max compression
```

## Comparing `PyTransportNSWv2-0.2.3.tar` & `PyTransportNSWv2-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2020-06-28 08:20:05.903436 PyTransportNSWv2-0.2.3/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4221 2020-06-28 08:20:05.903436 PyTransportNSWv2-0.2.3/PKG-INFO
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2020-06-28 08:20:05.903436 PyTransportNSWv2-0.2.3/PyTransportNSWv2.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4221 2020-06-28 08:20:05.000000 PyTransportNSWv2-0.2.3/PyTransportNSWv2.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      292 2020-06-28 08:20:05.000000 PyTransportNSWv2-0.2.3/PyTransportNSWv2.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2020-06-28 08:20:05.000000 PyTransportNSWv2-0.2.3/PyTransportNSWv2.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       23 2020-06-28 08:20:05.000000 PyTransportNSWv2-0.2.3/PyTransportNSWv2.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       13 2020-06-28 08:20:05.000000 PyTransportNSWv2-0.2.3/PyTransportNSWv2.egg-info/top_level.txt
--rwxrwxr-x   0 andrew    (1000) andrew    (1000)     3201 2020-06-17 09:23:02.000000 PyTransportNSWv2-0.2.3/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2020-06-28 08:20:05.903436 PyTransportNSWv2-0.2.3/TransportNSW/
--rwxrwxr-x   0 andrew    (1000) andrew    (1000)    11754 2020-06-28 08:13:06.000000 PyTransportNSWv2-0.2.3/TransportNSW/TransportNSW.py
--rwxrwxr-x   0 andrew    (1000) andrew    (1000)       86 2020-06-16 09:35:09.000000 PyTransportNSWv2-0.2.3/TransportNSW/__init__.py
--rwxrwxr-x   0 andrew    (1000) andrew    (1000)      961 2020-06-28 07:50:07.000000 PyTransportNSWv2-0.2.3/TransportNSW/test.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2020-06-28 08:20:05.903436 PyTransportNSWv2-0.2.3/setup.cfg
--rwxrwxr-x   0 andrew    (1000) andrew    (1000)      804 2020-06-28 08:17:49.000000 PyTransportNSWv2-0.2.3/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2020-06-28 10:00:55.671437 PyTransportNSWv2-0.2.4/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4221 2020-06-28 10:00:55.671437 PyTransportNSWv2-0.2.4/PKG-INFO
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2020-06-28 10:00:55.671437 PyTransportNSWv2-0.2.4/PyTransportNSWv2.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4221 2020-06-28 10:00:55.000000 PyTransportNSWv2-0.2.4/PyTransportNSWv2.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      292 2020-06-28 10:00:55.000000 PyTransportNSWv2-0.2.4/PyTransportNSWv2.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2020-06-28 10:00:55.000000 PyTransportNSWv2-0.2.4/PyTransportNSWv2.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       23 2020-06-28 10:00:55.000000 PyTransportNSWv2-0.2.4/PyTransportNSWv2.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       13 2020-06-28 10:00:55.000000 PyTransportNSWv2-0.2.4/PyTransportNSWv2.egg-info/top_level.txt
+-rwxrwxr-x   0 andrew    (1000) andrew    (1000)     3201 2020-06-17 09:23:02.000000 PyTransportNSWv2-0.2.4/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2020-06-28 10:00:55.671437 PyTransportNSWv2-0.2.4/TransportNSW/
+-rwxrwxr-x   0 andrew    (1000) andrew    (1000)    11834 2020-06-28 09:33:49.000000 PyTransportNSWv2-0.2.4/TransportNSW/TransportNSW.py
+-rwxrwxr-x   0 andrew    (1000) andrew    (1000)       86 2020-06-16 09:35:09.000000 PyTransportNSWv2-0.2.4/TransportNSW/__init__.py
+-rwxrwxr-x   0 andrew    (1000) andrew    (1000)      805 2020-06-28 09:35:17.000000 PyTransportNSWv2-0.2.4/TransportNSW/test.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2020-06-28 10:00:55.671437 PyTransportNSWv2-0.2.4/setup.cfg
+-rwxrwxr-x   0 andrew    (1000) andrew    (1000)      804 2020-06-28 09:37:23.000000 PyTransportNSWv2-0.2.4/setup.py
```

### Comparing `PyTransportNSWv2-0.2.3/PKG-INFO` & `PyTransportNSWv2-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTransportNSWv2
-Version: 0.2.3
+Version: 0.2.4
 Summary: Get detailed per-trip transport information from TransportNSW
 Home-page: https://github.com/andystewart999/TransportNSW
 Author: andystewart999
 License: UNKNOWN
 Description: # TransportNSW
         Python lib to access Transport NSW information.
```

### Comparing `PyTransportNSWv2-0.2.3/PyTransportNSWv2.egg-info/PKG-INFO` & `PyTransportNSWv2-0.2.4/PyTransportNSWv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTransportNSWv2
-Version: 0.2.3
+Version: 0.2.4
 Summary: Get detailed per-trip transport information from TransportNSW
 Home-page: https://github.com/andystewart999/TransportNSW
 Author: andystewart999
 License: UNKNOWN
 Description: # TransportNSW
         Python lib to access Transport NSW information.
```

### Comparing `PyTransportNSWv2-0.2.3/README.md` & `PyTransportNSWv2-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `PyTransportNSWv2-0.2.3/TransportNSW/TransportNSW.py` & `PyTransportNSWv2-0.2.4/TransportNSW/TransportNSW.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,26 +102,30 @@
         # log error and return empty object
         if response.status_code != 200:
             logger.warning("Error with the request sent; check api key")
             return self.info
 
         # Parse the result as a JSON object
         result = response.json()
-        print (result)
+        #print (result)
 
         # The API will always return a valid trip, so it's just a case of grabbing what we need...
         # We're only reporting on the origin and destination, it's out of scope to discuss the specifics of the ENTIRE journey
         # This isn't a route planner, just a 'how long until the next journey I've specified' tool
         # The assumption is that the travelee will know HOW to make the defined journey, they're just asking WHEN it's happening next
 
         legs = result['journeys'][0]['legs']
         first_leg = self.find_first_leg(legs)
         last_leg = self.find_last_leg(legs)
         changes = self.find_changes(legs)
 
+        print (first_leg)
+        print (last_leg)
+        print (changes)
+
         origin = result['journeys'][0]['legs'][first_leg]['origin']
         # probably tidy this up when we start to get occupancy data back
         first_destination = result['journeys'][0]['legs'][first_leg]['destination']
         destination = result['journeys'][0]['legs'][last_leg]['destination']
         transportation = result['journeys'][0]['legs'][first_leg]['transportation']
 
 
@@ -240,15 +244,15 @@
         # Hmm, we didn't find one
         return None
 
 
     def find_last_leg(self, legs):
         # Find the last non-footpath leg
         leg_count = len(legs)
-        for leg in range (leg_count-1, 0, -1):
+        for leg in range (leg_count - 1, -1, -1):
             leg_class = legs[leg]['transportation']['product']['class']
             #print (leg_class)
             if leg_class < 100:
                 # 100 is the class for walking, anything less is a train, bus, etc
                 return leg
 
         # Hmm, we didn't find one
```

### Comparing `PyTransportNSWv2-0.2.3/TransportNSW/test.py` & `PyTransportNSWv2-0.2.4/TransportNSW/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from TransportNSW import TransportNSW
 tnsw = TransportNSW()
 
 sApiKey = 'oWwCalKSy0ZQB5JTw7sTXlcaOjv01fto1W3v'
 #sStopId = '207261'   #Gordon, platform 1
-sStopId = '10101121' #Gordon station
+#sStopId = '10101121' #Gordon station
 #sDestId = '10101122' #Pymble station
-#sStopId = '2000336'  #Central, platform 16
-#sDestId = '2015137' #Redfern, platform 7
+sStopId = '2000336'  #Central, platform 16
+sDestId = '2015137' #Redfern, platform 7
 #sStopId = '2015133'  #Redfern, platform 11
 #sStopId = '207248'   # Gordon bus stop
-#sDestId = '207537'   # St Ives stop
+sStopId = '207537'   # St Ives stop
 #sDestId = '2073161'  #Pymble station
 #sStopId = '2000225'   # Circular Quay Wharf 4
 #sDestId = '20883'     # Taronga Zoo Wharf
 #sStopId = '20461'     # Abbotsford
 #sDestId = '2137186'   # Cabarita
 sDestId = '10101100'  # Central
 #sDestId = '10101421'   # Redfern
 
-sStopId = 'streetID:1500000021:8:95330012:1:Coree Pl:St Ives:Coree Pl::Coree Pl:2075:ANY:DIVA_SINGLEHOUSE:4885970:3740665:GDAV:nsw'
-sDestId = '10101100'
-
 nMinDueTime = 0
 
 journey = tnsw.get_trip(sStopId, sDestId, sApiKey, nMinDueTime)
 print (' ')
 print(journey)
```

### Comparing `PyTransportNSWv2-0.2.3/setup.py` & `PyTransportNSWv2-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyTransportNSWv2",
-    version="0.2.3",
+    version="0.2.4",
     author="andystewart999",
     description="Get detailed per-trip transport information from TransportNSW",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andystewart999/TransportNSW",
     packages=setuptools.find_packages(),
     install_requires=[
```

