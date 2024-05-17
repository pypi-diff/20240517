# Comparing `tmp/DatastreamPy-2.0.21-py3-none-any.whl.zip` & `tmp/DatastreamPy-2.0.24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 51198 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat    16190 b- defN 24-Jan-30 08:10 DatastreamPy/DSConnect.py
--rw-rw-rw-  2.0 fat    22949 b- defN 24-Jan-30 08:12 DatastreamPy/DSUserDataObjectBase.py
--rw-rw-rw-  2.0 fat     5633 b- defN 23-Aug-11 08:57 DatastreamPy/DS_Requests.py
--rw-rw-rw-  2.0 fat    27153 b- defN 24-Jan-30 08:10 DatastreamPy/DS_Response.py
--rw-rw-rw-  2.0 fat    60200 b- defN 24-Jan-12 09:49 DatastreamPy/DatastreamEconomicFilters.py
--rw-rw-rw-  2.0 fat    52895 b- defN 24-Feb-13 09:08 DatastreamPy/DatastreamUserCreated_TimeSeries.py
--rw-rw-rw-  2.0 fat     1041 b- defN 23-Aug-11 08:57 DatastreamPy/__init__.py
--rw-rw-rw-  2.0 fat    27395 b- defN 24-Feb-13 09:10 DatastreamPy-2.0.21.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-13 09:10 DatastreamPy-2.0.21.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Feb-13 09:10 DatastreamPy-2.0.21.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      955 b- defN 24-Feb-13 09:10 DatastreamPy-2.0.21.dist-info/RECORD
-11 files, 214516 bytes uncompressed, 49580 bytes compressed:  76.9%
+Zip file size: 51260 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat    16190 b- defN 24-May-02 11:26 DatastreamPy/DSConnect.py
+-rw-rw-rw-  2.0 fat    22949 b- defN 24-May-02 11:26 DatastreamPy/DSUserDataObjectBase.py
+-rw-rw-rw-  2.0 fat     5633 b- defN 24-May-02 11:26 DatastreamPy/DS_Requests.py
+-rw-rw-rw-  2.0 fat    27568 b- defN 24-May-02 11:26 DatastreamPy/DS_Response.py
+-rw-rw-rw-  2.0 fat    60200 b- defN 24-May-02 11:26 DatastreamPy/DatastreamEconomicFilters.py
+-rw-rw-rw-  2.0 fat    52895 b- defN 24-May-02 11:26 DatastreamPy/DatastreamUserCreated_TimeSeries.py
+-rw-rw-rw-  2.0 fat     1041 b- defN 24-May-02 11:26 DatastreamPy/__init__.py
+-rw-rw-rw-  2.0 fat    27395 b- defN 24-May-17 15:08 DatastreamPy-2.0.24.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-17 15:08 DatastreamPy-2.0.24.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-17 15:08 DatastreamPy-2.0.24.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      955 b- defN 24-May-17 15:08 DatastreamPy-2.0.24.dist-info/RECORD
+11 files, 214931 bytes uncompressed, 49642 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: DatastreamPy/DatastreamUserCreated_TimeSeries.py
 Comment: 
 
 Filename: DatastreamPy/__init__.py
 Comment: 
 
-Filename: DatastreamPy-2.0.21.dist-info/METADATA
+Filename: DatastreamPy-2.0.24.dist-info/METADATA
 Comment: 
 
-Filename: DatastreamPy-2.0.21.dist-info/WHEEL
+Filename: DatastreamPy-2.0.24.dist-info/WHEEL
 Comment: 
 
-Filename: DatastreamPy-2.0.21.dist-info/top_level.txt
+Filename: DatastreamPy-2.0.24.dist-info/top_level.txt
 Comment: 
 
-Filename: DatastreamPy-2.0.21.dist-info/RECORD
+Filename: DatastreamPy-2.0.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DatastreamPy/DSUserDataObjectBase.py

```diff
@@ -20,15 +20,15 @@
 from enum import IntEnum
 import pytz
 import json
 import re
 from datetime import datetime, timedelta, date
 
 class DSPackageInfo:
-    buildVer = '2.0.21'
+    buildVer = '2.0.24'
     appId = 'DatastreamPy-' + buildVer
     UserAgent = ' DatastreamPy/' + buildVer
 
 class DSUserObjectFault(Exception):
     """
     DSUserObjectFault exception is a representation of the DSFault error returned from the API server.
     DSFaults are returned for the following reasons:
```

## DatastreamPy/DS_Response.py

```diff
@@ -1612,87 +1612,112 @@
 000064b0: 616d 6520 3d20 7365 6c66 2e5f 6765 745f  ame = self._get_
 000064c0: 4461 7461 7479 7065 5661 6c75 6573 2872  DatatypeValues(r
 000064d0: 6573 706f 6e73 655f 6a73 6f6e 290d 0a20  esponse_json).. 
 000064e0: 2020 2020 2020 2069 6620 286c 656e 2864         if (len(d
 000064f0: 6174 6573 5f63 6f6e 7665 7274 6564 2920  ates_converted) 
 00006500: 3d3d 206c 656e 2864 6174 6166 7261 6d65  == len(dataframe
 00006510: 2e69 6e64 6578 2929 3a0d 0a20 2020 2020  .index)):..     
-00006520: 2020 2020 2020 2069 6620 286c 656e 2864         if (len(d
-00006530: 6174 6573 5f63 6f6e 7665 7274 6564 2920  ates_converted) 
-00006540: 3e20 3129 3a0d 0a20 2020 2020 2020 2020  > 1):..         
-00006550: 2020 2020 2020 2023 6461 7461 6672 616d         #datafram
-00006560: 652e 696e 7365 7274 286c 6f63 203d 2030  e.insert(loc = 0
-00006570: 2c20 636f 6c75 6d6e 203d 2027 4461 7465  , column = 'Date
-00006580: 7327 2c20 7661 6c75 6520 3d20 6461 7465  s', value = date
-00006590: 735f 636f 6e76 6572 7465 6429 0d0a 2020  s_converted)..  
-000065a0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-000065b0: 7461 6672 616d 652e 696e 6465 7820 3d20  taframe.index = 
-000065c0: 6461 7465 735f 636f 6e76 6572 7465 640d  dates_converted.
-000065d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000065e0: 2064 6174 6166 7261 6d65 2e69 6e64 6578   dataframe.index
-000065f0: 2e6e 616d 6520 3d20 2744 6174 6573 270d  .name = 'Dates'.
-00006600: 0a20 2020 2020 2020 2065 6c69 6620 286c  .        elif (l
-00006610: 656e 2864 6174 6573 5f63 6f6e 7665 7274  en(dates_convert
-00006620: 6564 2920 3d3d 2031 293a 0d0a 2020 2020  ed) == 1):..    
-00006630: 2020 2020 2020 2020 6461 7461 6672 616d          datafram
-00006640: 655b 2744 6174 6573 275d 203d 2064 6174  e['Dates'] = dat
-00006650: 6573 5f63 6f6e 7665 7274 6564 5b30 5d0d  es_converted[0].
-00006660: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00006670: 2020 2072 6574 7572 6e20 6461 7461 6672     return datafr
-00006680: 616d 650d 0a0d 0a20 2020 2064 6566 205f  ame....    def _
-00006690: 666f 726d 6174 5f62 756e 646c 655f 7265  format_bundle_re
-000066a0: 7370 6f6e 7365 2873 656c 662c 7265 7370  sponse(self,resp
-000066b0: 6f6e 7365 5f6a 736f 6e29 3a0d 0a20 2020  onse_json):..   
-000066c0: 2020 2020 2066 6f72 6d61 7474 6564 5265       formattedRe
-000066d0: 7370 203d 205b 5d0d 0a20 2020 2020 2020  sp = []..       
-000066e0: 2066 6f72 2065 6163 6844 6174 6152 6573   for eachDataRes
-000066f0: 706f 6e73 6520 696e 2072 6573 706f 6e73  ponse in respons
-00006700: 655f 6a73 6f6e 5b27 4461 7461 5265 7370  e_json['DataResp
-00006710: 6f6e 7365 7327 5d3a 0d0a 2020 2020 2020  onses']:..      
-00006720: 2020 2020 2020 6466 203d 2073 656c 662e        df = self.
-00006730: 5f66 6f72 6d61 745f 5265 7370 6f6e 7365  _format_Response
-00006740: 2865 6163 6844 6174 6152 6573 706f 6e73  (eachDataRespons
-00006750: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00006760: 666f 726d 6174 7465 6452 6573 702e 6170  formattedResp.ap
-00006770: 7065 6e64 2864 6629 2020 2020 2020 0d0a  pend(df)      ..
-00006780: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006790: 2020 2020 2072 6574 7572 6e20 666f 726d       return form
-000067a0: 6174 7465 6452 6573 700d 0a20 2020 0d0a  attedResp..   ..
-000067b0: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-000067c0: 205f 6765 745f 6d65 7461 6461 7461 2873   _get_metadata(s
-000067d0: 656c 662c 206a 736f 6e52 6573 7029 3a0d  elf, jsonResp):.
-000067e0: 0a20 2020 2020 2020 206e 616d 6573 203d  .        names =
-000067f0: 207b 7d0d 0a20 2020 2020 2020 2069 6620   {}..        if 
-00006800: 6a73 6f6e 5265 7370 5b27 5379 6d62 6f6c  jsonResp['Symbol
-00006810: 4e61 6d65 7327 5d3a 0d0a 2020 2020 2020  Names']:..      
-00006820: 2020 2020 2020 666f 7220 6920 696e 206a        for i in j
-00006830: 736f 6e52 6573 705b 2753 796d 626f 6c4e  sonResp['SymbolN
-00006840: 616d 6573 275d 3a0d 0a20 2020 2020 2020  ames']:..       
-00006850: 2020 2020 2020 2020 206e 616d 6573 2e75           names.u
-00006860: 7064 6174 6528 7b69 5b27 4b65 7927 5d3a  pdate({i['Key']:
-00006870: 2069 5b27 5661 6c75 6527 5d7d 290d 0a20   i['Value']}).. 
-00006880: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00006890: 0a20 2020 2020 2020 2069 6620 6a73 6f6e  .        if json
-000068a0: 5265 7370 5b27 4461 7461 5479 7065 4e61  Resp['DataTypeNa
-000068b0: 6d65 7327 5d3a 0d0a 2020 2020 2020 2020  mes']:..        
-000068c0: 2020 2020 666f 7220 6920 696e 206a 736f      for i in jso
-000068d0: 6e52 6573 705b 2744 6174 6154 7970 654e  nResp['DataTypeN
-000068e0: 616d 6573 275d 3a0d 0a20 2020 2020 2020  ames']:..       
-000068f0: 2020 2020 2020 2020 206e 616d 6573 2e75           names.u
-00006900: 7064 6174 6528 7b69 5b27 4b65 7927 5d3a  pdate({i['Key']:
-00006910: 2069 5b27 5661 6c75 6527 5d7d 290d 0a20   i['Value']}).. 
-00006920: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
-00006930: 6566 205f 6765 745f 6d65 7461 6461 7461  ef _get_metadata
-00006940: 5f62 756e 646c 6528 7365 6c66 2c20 6a73  _bundle(self, js
-00006950: 6f6e 5265 7370 293a 0d0a 2020 2020 2020  onResp):..      
-00006960: 2020 666f 7220 6561 6368 4461 7461 5265    for eachDataRe
-00006970: 7370 6f6e 7365 2069 6e20 6a73 6f6e 5265  sponse in jsonRe
-00006980: 7370 3a0d 0a20 2020 2020 2020 2020 2020  sp:..           
-00006990: 2073 656c 662e 5f67 6574 5f6d 6574 6164   self._get_metad
-000069a0: 6174 6128 6561 6368 4461 7461 5265 7370  ata(eachDataResp
-000069b0: 6f6e 7365 290d 0a23 2d2d 2d2d 2d2d 2d2d  onse)..#--------
-000069c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000069d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000069e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000069f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d  -------------...
-00006a10: 0a                                       .
+00006520: 2020 2020 2020 2064 6174 6166 7261 6d65         dataframe
+00006530: 2e69 6e64 6578 2e6e 616d 6520 3d20 2744  .index.name = 'D
+00006540: 6174 6573 270d 0a20 2020 2020 2020 2020  ates'..         
+00006550: 2020 2064 6174 6166 7261 6d65 2e69 6e64     dataframe.ind
+00006560: 6578 203d 2064 6174 6573 5f63 6f6e 7665  ex = dates_conve
+00006570: 7274 6564 0d0a 2020 2020 2020 2020 656c  rted..        el
+00006580: 6966 2028 6c65 6e28 6461 7465 735f 636f  if (len(dates_co
+00006590: 6e76 6572 7465 6429 203d 3d20 3129 3a0d  nverted) == 1):.
+000065a0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000065b0: 6166 7261 6d65 5b27 4461 7465 7327 5d20  aframe['Dates'] 
+000065c0: 3d20 6461 7465 735f 636f 6e76 6572 7465  = dates_converte
+000065d0: 645b 305d 0d0a 2020 2020 2020 2020 2020  d[0]..          
+000065e0: 2020 6966 2028 6c65 6e28 6461 7461 6672    if (len(datafr
+000065f0: 616d 652e 696e 6465 7829 203e 206c 656e  ame.index) > len
+00006600: 2864 6174 6573 5f63 6f6e 7665 7274 6564  (dates_converted
+00006610: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00006620: 2020 2020 2064 6174 6166 7261 6d65 2e69       dataframe.i
+00006630: 6e64 6578 203d 2064 6174 6166 7261 6d65  ndex = dataframe
+00006640: 5b27 4461 7465 7327 5d0d 0a20 2020 2020  ['Dates']..     
+00006650: 2020 2020 2020 2020 2020 2064 6174 6166             dataf
+00006660: 7261 6d65 203d 2064 6174 6166 7261 6d65  rame = dataframe
+00006670: 2e64 726f 7028 636f 6c75 6d6e 733d 2744  .drop(columns='D
+00006680: 6174 6573 272c 2061 7869 7320 3d20 3129  ates', axis = 1)
+00006690: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000066a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000066b0: 2020 0d0a 2020 2020 2020 2020 2320 2020    ..        #   
+000066c0: 2069 6620 286c 656e 2864 6174 6573 5f63   if (len(dates_c
+000066d0: 6f6e 7665 7274 6564 2920 3e20 3129 3a0d  onverted) > 1):.
+000066e0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+000066f0: 2020 2364 6174 6166 7261 6d65 2e69 6e73    #dataframe.ins
+00006700: 6572 7428 6c6f 6320 3d20 302c 2063 6f6c  ert(loc = 0, col
+00006710: 756d 6e20 3d20 2744 6174 6573 272c 2076  umn = 'Dates', v
+00006720: 616c 7565 203d 2064 6174 6573 5f63 6f6e  alue = dates_con
+00006730: 7665 7274 6564 290d 0a20 2020 2020 2020  verted)..       
+00006740: 2023 2020 2020 2020 2020 6461 7461 6672   #        datafr
+00006750: 616d 652e 696e 6465 7820 3d20 6461 7465  ame.index = date
+00006760: 735f 636f 6e76 6572 7465 640d 0a20 2020  s_converted..   
+00006770: 2020 2020 2023 2020 2020 2020 2020 6461       #        da
+00006780: 7461 6672 616d 652e 696e 6465 782e 6e61  taframe.index.na
+00006790: 6d65 203d 2027 4461 7465 7327 0d0a 2020  me = 'Dates'..  
+000067a0: 2020 2020 2020 2365 6c69 6620 286c 656e        #elif (len
+000067b0: 2864 6174 6573 5f63 6f6e 7665 7274 6564  (dates_converted
+000067c0: 2920 3d3d 2031 293a 0d0a 2020 2020 2020  ) == 1):..      
+000067d0: 2020 2320 2020 2064 6174 6166 7261 6d65    #    dataframe
+000067e0: 5b27 4461 7465 7327 5d20 3d20 6461 7465  ['Dates'] = date
+000067f0: 735f 636f 6e76 6572 7465 645b 305d 0d0a  s_converted[0]..
+00006800: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00006810: 2020 7265 7475 726e 2064 6174 6166 7261    return datafra
+00006820: 6d65 0d0a 0d0a 2020 2020 6465 6620 5f66  me....    def _f
+00006830: 6f72 6d61 745f 6275 6e64 6c65 5f72 6573  ormat_bundle_res
+00006840: 706f 6e73 6528 7365 6c66 2c72 6573 706f  ponse(self,respo
+00006850: 6e73 655f 6a73 6f6e 293a 0d0a 2020 2020  nse_json):..    
+00006860: 2020 2020 666f 726d 6174 7465 6452 6573      formattedRes
+00006870: 7020 3d20 5b5d 0d0a 2020 2020 2020 2020  p = []..        
+00006880: 666f 7220 6561 6368 4461 7461 5265 7370  for eachDataResp
+00006890: 6f6e 7365 2069 6e20 7265 7370 6f6e 7365  onse in response
+000068a0: 5f6a 736f 6e5b 2744 6174 6152 6573 706f  _json['DataRespo
+000068b0: 6e73 6573 275d 3a0d 0a20 2020 2020 2020  nses']:..       
+000068c0: 2020 2020 2064 6620 3d20 7365 6c66 2e5f       df = self._
+000068d0: 666f 726d 6174 5f52 6573 706f 6e73 6528  format_Response(
+000068e0: 6561 6368 4461 7461 5265 7370 6f6e 7365  eachDataResponse
+000068f0: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00006900: 6f72 6d61 7474 6564 5265 7370 2e61 7070  ormattedResp.app
+00006910: 656e 6428 6466 2920 2020 2020 200d 0a20  end(df)      .. 
+00006920: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00006930: 2020 2020 7265 7475 726e 2066 6f72 6d61      return forma
+00006940: 7474 6564 5265 7370 0d0a 2020 200d 0a20  ttedResp..   .. 
+00006950: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
+00006960: 5f67 6574 5f6d 6574 6164 6174 6128 7365  _get_metadata(se
+00006970: 6c66 2c20 6a73 6f6e 5265 7370 293a 0d0a  lf, jsonResp):..
+00006980: 2020 2020 2020 2020 6e61 6d65 7320 3d20          names = 
+00006990: 7b7d 0d0a 2020 2020 2020 2020 6966 206a  {}..        if j
+000069a0: 736f 6e52 6573 705b 2753 796d 626f 6c4e  sonResp['SymbolN
+000069b0: 616d 6573 275d 3a0d 0a20 2020 2020 2020  ames']:..       
+000069c0: 2020 2020 2066 6f72 2069 2069 6e20 6a73       for i in js
+000069d0: 6f6e 5265 7370 5b27 5379 6d62 6f6c 4e61  onResp['SymbolNa
+000069e0: 6d65 7327 5d3a 0d0a 2020 2020 2020 2020  mes']:..        
+000069f0: 2020 2020 2020 2020 6e61 6d65 732e 7570          names.up
+00006a00: 6461 7465 287b 695b 274b 6579 275d 3a20  date({i['Key']: 
+00006a10: 695b 2756 616c 7565 275d 7d29 0d0a 2020  i['Value']})..  
+00006a20: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00006a30: 2020 2020 2020 2020 6966 206a 736f 6e52          if jsonR
+00006a40: 6573 705b 2744 6174 6154 7970 654e 616d  esp['DataTypeNam
+00006a50: 6573 275d 3a0d 0a20 2020 2020 2020 2020  es']:..         
+00006a60: 2020 2066 6f72 2069 2069 6e20 6a73 6f6e     for i in json
+00006a70: 5265 7370 5b27 4461 7461 5479 7065 4e61  Resp['DataTypeNa
+00006a80: 6d65 7327 5d3a 0d0a 2020 2020 2020 2020  mes']:..        
+00006a90: 2020 2020 2020 2020 6e61 6d65 732e 7570          names.up
+00006aa0: 6461 7465 287b 695b 274b 6579 275d 3a20  date({i['Key']: 
+00006ab0: 695b 2756 616c 7565 275d 7d29 0d0a 2020  i['Value']})..  
+00006ac0: 2020 2020 2020 0d0a 0d0a 2020 2020 6465        ....    de
+00006ad0: 6620 5f67 6574 5f6d 6574 6164 6174 615f  f _get_metadata_
+00006ae0: 6275 6e64 6c65 2873 656c 662c 206a 736f  bundle(self, jso
+00006af0: 6e52 6573 7029 3a0d 0a20 2020 2020 2020  nResp):..       
+00006b00: 2066 6f72 2065 6163 6844 6174 6152 6573   for eachDataRes
+00006b10: 706f 6e73 6520 696e 206a 736f 6e52 6573  ponse in jsonRes
+00006b20: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
+00006b30: 7365 6c66 2e5f 6765 745f 6d65 7461 6461  self._get_metada
+00006b40: 7461 2865 6163 6844 6174 6152 6573 706f  ta(eachDataRespo
+00006b50: 6e73 6529 0d0a 232d 2d2d 2d2d 2d2d 2d2d  nse)..#---------
+00006b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a  ------------....
```

## Comparing `DatastreamPy-2.0.21.dist-info/METADATA` & `DatastreamPy-2.0.24.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DatastreamPy
-Version: 2.0.21
+Version: 2.0.24
 Summary: Python package for Datastream Web Services API
 Author: LSEG
 Author-email: datastreamapi@lseg.com
 License: Apache Software License (http://www.apache.org/licenses/LICENSE-2.0)
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
```

