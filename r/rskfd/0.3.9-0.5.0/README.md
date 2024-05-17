# Comparing `tmp/rskfd-0.3.9.tar.gz` & `tmp/rskfd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rskfd-0.3.9.tar", last modified: Wed May  8 16:08:20 2024, max compression
+gzip compressed data, was "rskfd-0.5.0.tar", last modified: Fri May 17 10:46:22 2024, max compression
```

## Comparing `rskfd-0.3.9.tar` & `rskfd-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.600732 rskfd-0.3.9/
--rw-rw-rw-   0        0        0     2248 2024-05-08 16:08:20.600732 rskfd-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.540302 rskfd-0.3.9/examples/
--rw-rw-rw-   0        0        0     3705 2023-02-16 10:45:21.000000 rskfd-0.3.9/examples/Wv2BinStream.py
--rw-rw-rw-   0        0        0     1322 2024-05-08 14:30:04.000000 rskfd-0.3.9/examples/fileopening.py
--rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.3.9/examples/instrumentexamples.py
--rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.3.9/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.548354 rskfd-0.3.9/rskfd/
--rw-rw-rw-   0        0        0     1299 2023-03-15 14:55:14.000000 rskfd-0.3.9/rskfd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.568528 rskfd-0.3.9/rskfd/helper/
--rw-rw-rw-   0        0        0     4389 2024-04-15 19:01:01.000000 rskfd-0.3.9/rskfd/helper/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.570543 rskfd-0.3.9/rskfd/iq_data_handling/
--rw-rw-rw-   0        0        0    21282 2024-05-08 14:18:43.000000 rskfd-0.3.9/rskfd/iq_data_handling/iqdata.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.590685 rskfd-0.3.9/rskfd/remote_control/
--rw-rw-rw-   0        0        0    14935 2024-04-16 04:51:55.000000 rskfd-0.3.9/rskfd/remote_control/instrument.py
--rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.3.9/rskfd/remote_control/instrumentRS.py
--rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.3.9/rskfd/remote_control/instrumentRSExceptions.py
--rw-rw-rw-   0        0        0     8562 2024-04-15 13:54:25.000000 rskfd-0.3.9/rskfd/remote_control/instrumentRS_FSW.py
--rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.3.9/rskfd/remote_control/instrumentRS_VSE.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.590685 rskfd-0.3.9/rskfd/signal_generation/
--rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.3.9/rskfd/signal_generation/signal_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.590685 rskfd-0.3.9/rskfd/snp_handling/
--rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.3.9/rskfd/snp_handling/snpfiles.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.600732 rskfd-0.3.9/rskfd.egg-info/
--rw-rw-rw-   0        0        0     2248 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-08 16:08:20.608781 rskfd-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1439 2024-05-08 16:06:54.000000 rskfd-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.482769 rskfd-0.5.0/
+-rw-rw-rw-   0        0        0     2247 2024-05-17 10:46:22.482769 rskfd-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.444896 rskfd-0.5.0/examples/
+-rw-rw-rw-   0        0        0     3705 2023-02-16 10:45:21.000000 rskfd-0.5.0/examples/Wv2BinStream.py
+-rw-rw-rw-   0        0        0     3001 2024-05-17 10:05:47.000000 rskfd-0.5.0/examples/fileopening.py
+-rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.5.0/examples/instrumentexamples.py
+-rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.5.0/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.446890 rskfd-0.5.0/rskfd/
+-rw-rw-rw-   0        0        0     1299 2023-03-15 14:55:14.000000 rskfd-0.5.0/rskfd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.460843 rskfd-0.5.0/rskfd/helper/
+-rw-rw-rw-   0        0        0     4386 2024-05-17 07:08:58.000000 rskfd-0.5.0/rskfd/helper/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.463832 rskfd-0.5.0/rskfd/iq_data_handling/
+-rw-rw-rw-   0        0        0    24739 2024-05-17 10:39:51.000000 rskfd-0.5.0/rskfd/iq_data_handling/iqdata.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.474796 rskfd-0.5.0/rskfd/remote_control/
+-rw-rw-rw-   0        0        0    14935 2024-04-16 04:51:55.000000 rskfd-0.5.0/rskfd/remote_control/instrument.py
+-rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.5.0/rskfd/remote_control/instrumentRS.py
+-rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.5.0/rskfd/remote_control/instrumentRSExceptions.py
+-rw-rw-rw-   0        0        0     8562 2024-04-15 13:54:25.000000 rskfd-0.5.0/rskfd/remote_control/instrumentRS_FSW.py
+-rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.5.0/rskfd/remote_control/instrumentRS_VSE.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.476789 rskfd-0.5.0/rskfd/signal_generation/
+-rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.5.0/rskfd/signal_generation/signal_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.478783 rskfd-0.5.0/rskfd/snp_handling/
+-rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.5.0/rskfd/snp_handling/snpfiles.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.480777 rskfd-0.5.0/rskfd.egg-info/
+-rw-rw-rw-   0        0        0     2247 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-17 10:46:22.484767 rskfd-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1438 2024-05-17 10:45:19.000000 rskfd-0.5.0/setup.py
```

### Comparing `rskfd-0.3.9/PKG-INFO` & `rskfd-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.3.9
+Version: 0.5.0
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
```

### Comparing `rskfd-0.3.9/README.md` & `rskfd-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/examples/Wv2BinStream.py` & `rskfd-0.5.0/examples/Wv2BinStream.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/examples/instrumentexamples.py` & `rskfd-0.5.0/examples/instrumentexamples.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/license.txt` & `rskfd-0.5.0/license.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/rskfd/__init__.py` & `rskfd-0.5.0/rskfd/__init__.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/rskfd/helper/helper.py` & `rskfd-0.5.0/rskfd/helper/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     if bPlotRelative:
         mag = 20*numpy.log10(numpy.abs(numpy.fft.fftshift(numpy.fft.fft(data[:limiterlen]))))
         # normalize to mean
         meanmag = 10*numpy.log10( numpy.mean( numpy.power( 10, mag/10)))
         mag = mag - meanmag
     else:
         mag = 10*numpy.log10(numpy.power( numpy.abs( numpy.fft.fftshift( numpy.fft.fft( data[:limiterlen]))), 2)/50/limiterlen)+30
-    
-    freq = numpy.multiply( range( -limiterlen//2,(limiterlen+1)//2), fs/limiterlen)
+
+    freq = numpy.multiply(range(-(limiterlen//2), (limiterlen+1)//2), fs/limiterlen)
     plt.plot(freq,mag)
     plt.grid( True)
     plt.xlabel( 'freq / Hz')
     if bPlotRelative:
         plt.ylabel( 'relative power / dB')
     else:
         plt.ylabel( 'power / dBm')
```

### Comparing `rskfd-0.3.9/rskfd/iq_data_handling/iqdata.py` & `rskfd-0.5.0/rskfd/iq_data_handling/iqdata.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,123 +4,221 @@
 
 @author: RAMIAN
 """
 
 #TODO: errorhandling
 
 
+def __DataTypeStr2Int(DataType):
+    """
+    Converts a string data type to int, defaults to float 32
+    float32 ==> 1, float64 ==> 2, int8 ==> 3, int16 ==> 4, int32 ==> 5
+    """
+    RetType = 1
+    if DataType.lower().strip() == "float32":
+        RetType = 1
+    elif DataType.lower().strip() == "float64":
+        RetType = 2
+    elif DataType.lower().strip() == "int8":
+        RetType = 3
+    elif DataType.lower().strip() == "int16":
+        RetType = 4
+    elif DataType.lower().strip() == "int32":
+        RetType = 5
+
+    return RetType
+
+
+def __DataTypeInt2Str(DataType):
+    """
+    Converts a string data type to int, defaults to float 32
+    float32 ==> 1, float64 ==> 2, int8 ==> 3, int16 ==> 4, int32 ==> 5
+    """
+    RetType = "float32"
+    if DataType == 1:
+        RetType = "float32"
+    elif DataType == 2:
+        RetType = "float64"
+    elif DataType == 3:
+        RetType = "int8"
+    elif DataType == 4:
+        RetType = "int16"
+    elif DataType == 5:
+        RetType = "int32"
+
+    return RetType
+
+
+def __NumberOfBytes(DataType):
+    """
+    Returns number of bytes per value
+    float32 ==> 4, float64 ==> 8, int8 ==> 1, int16 ==> 2, int32 ==> 4
+    """
+    RetVal = 4
+    if not isinstance(DataType, int):
+        DataType = __DataTypeStr2Int(DataType)
+    if DataType == 1:
+        RetVal = 4
+    elif DataType == 2:
+        RetVal = 8
+    elif DataType == 3:
+        RetVal = 1
+    elif DataType == 4:
+        RetVal = 2
+    elif DataType == 5:
+        RetVal = 4
+
+    return RetVal
+
+
 def Iqiq2Complex( iqData):
     """Returns a complex list of I/Q samples from a single list containing IQIQIQ values
     complexList = Iqiq2Complex(iqiqiqList)"""
 
     import logging
-    
+
     if len(iqData) % 2 > 0:
         logging.warn("Expecting IQIQIQ order, input vector has odd number of samples!")
 
     NumberOfSamples = len(iqData) // 2
-                    
-    complexList = [ complex( iqData[2*n], iqData[2*n+1]) for n in range(NumberOfSamples)]    
+
+    complexList = [complex(iqData[2*n], iqData[2*n+1]) for n in range(NumberOfSamples)]    
     return complexList
 
 
 
-def Iiqq2Complex( iqData):
+def Iiqq2Complex(iqData):
     """Returns a complex list of I/Q samples from a single list containing IIIQQQ values
     complexList = Iiqq2Complex(iiiqqqList)"""
-    
+
     import logging
-    
+
     if len(iqData) % 2 > 0:
         logging.warn("Expecting IIIQQQ order, input vector has odd number of samples!")
 
     NumberOfSamples = len(iqData) // 2
-                    
-    complexList = [ complex( iqData[n], iqData[n+NumberOfSamples]) for n in range(NumberOfSamples)]    
+
+    complexList = [complex(iqData[n], iqData[n+NumberOfSamples]) for n in range(NumberOfSamples)]    
     return complexList
 
 
 
-def Complex2Iqiq( complexList):
+def Complex2Iqiq(complexList):
     """Returns a list of I/Q samples from a complex list.
     iqiqiqList = Complex2Iqiq(complexList)"""
-    
-    f= lambda iq,i: iq.real if i==0 else iq.imag
-    iqiqiqList = [ f(iq,i) for iq in complexList for i in range(2)]
+
+    f = lambda iq, i: iq.real if i == 0 else iq.imag
+    iqiqiqList = [f(iq, i) for iq in complexList for i in range(2)]
 
     return iqiqiqList
 
 
 
 def Complex2Iiqq( complexList):
     """Returns a list of I/Q samples from a complex list.
     iiiqqqList = Complex2Iiqq(complexList)"""
-    
-    iqiqiqList = [ iq.real for iq in complexList]
-    iqiqiqList.append( [ iq.imag for iq in complexList])        
+
+    iqiqiqList = [iq.real for iq in complexList]
+    iqiqiqList.append([iq.imag for iq in complexList])
 
     return iqiqiqList
 
 
 
-def WriteIqw( iqData, FileName, AppendExisting = False):
+def WriteIqw( iqData, FileName, AppendExisting=False, DataType="float32"):
     """Writes an IQW file (file of binary floats).
     iqData can be a list of complex or list of floats. List of floats will
     be written directly into iqw - regardles of order iiqq or iqiq.
     Note: IIIQQQ is a deprecated format, don't use it for new files.
-    writtenSamples = WriteIqw( iqList, "MyFile.iqiq.iqw")."""
-    
+    writtenSamples = WriteIqw( iqList, "MyFile.iqiq.iqw").
+    DataType (supported): float32, float64
+    """
+
     import struct
     import logging
-    
-    #check if iqData is complex
+
+    # check if iqData is complex
     if isinstance(iqData[0], complex):
-        iqData = Complex2Iqiq( iqData)
-        
+        iqData = Complex2Iqiq(iqData)
+
     NumberOfSamples = len(iqData) // 2
-        
+    ScalingFactor = 1
+
     try:
         if AppendExisting:
-            file = open( FileName, "ab")
+            file = open(FileName, "ab")
         else:
-            file = open( FileName, "wb")
-        file.write( struct.pack("f"*len(iqData),*iqData))
+            file = open(FileName, "wb")
+        if __DataTypeStr2Int(DataType) == 1:
+            # float 32
+            file.write(struct.pack("f"*len(iqData), *iqData))
+        elif __DataTypeStr2Int(DataType) == 2:
+            # float64
+            file.write(struct.pack("d"*len(iqData), *iqData))
+        elif __DataTypeStr2Int(DataType) == 3:
+            # int16
+            ScalingFactor = max(map(abs, iqData))/(2**(__NumberOfBytes(DataType)*8-1)-1)
+            iqData = [round(item / ScalingFactor) for item in iqData]
+            file.write(struct.pack("b"*len(iqData), *iqData))
+        elif __DataTypeStr2Int(DataType) == 4:
+            # int16
+            ScalingFactor = max(map(abs, iqData))/(2**(__NumberOfBytes(DataType)*8-1)-1)
+            iqData = [round(item / ScalingFactor) for item in iqData]
+            file.write(struct.pack("h"*len(iqData), *iqData))
+        elif __DataTypeStr2Int(DataType) == 5:
+            # int16
+            ScalingFactor = max(map(abs, iqData))/(2**(__NumberOfBytes(DataType)*8-1)-1)
+            iqData = [round(item / ScalingFactor) for item in iqData]
+            file.write(struct.pack("i"*len(iqData), *iqData))
+
         file.close
     except:
-        logging.error("File (" + FileName +") write error!" )
-    
-    return NumberOfSamples
+        logging.error("File (" + FileName + ") write error!")
+
+    return NumberOfSamples, ScalingFactor
 
 
 
-def ReadIqw( FileName, iqiq=True, BytesPerValue=4):
+def ReadIqw( FileName, iqiq=True, DataType="float32"):
     """Reads an IQW (can be iiqq or iqiq) file. Returns complex samples.
     If iqiq is True, samples are read pairwise (IQIQIQ),
     otherwise in blocks, i first then q (IIIQQQ)
     Note: IIIQQQ is a deprecated format, don't use it for new files.
     iqList = ReadIqw("MyFile.iqw", iqiq = True)
-    BytesPerValue specifies the word length per I/Q sample in the file"""
+    DataType (supported): float32, float64
+    """
 
     import struct
     import logging
 
+    BytesPerValue = __NumberOfBytes(__DataTypeStr2Int(DataType))
+
     try:
-        file = open( FileName, "rb")
+        file = open(FileName, "rb")
         data = file.read()
         file.close
+        ReadSamples = len(data) // BytesPerValue
     except:
         logging.error("File open error (" + FileName+")!")
 
-    ReadSamples = len(data) // BytesPerValue
-    if BytesPerValue == 4:
+    if __DataTypeStr2Int(DataType) == 1:
+        # float 32
         data = list(struct.unpack("f"*ReadSamples, data))
-    elif BytesPerValue == 8:
+    elif __DataTypeStr2Int(DataType) == 2:
+        # float64
         data = list(struct.unpack("d"*ReadSamples, data))
-    else:
-        logging.error("Unsupported word length!")
+    elif __DataTypeStr2Int(DataType) == 3:
+        # int8
+        data = list(struct.unpack("b"*ReadSamples, data))
+    elif __DataTypeStr2Int(DataType) == 4:
+        # int16
+        data = list(struct.unpack("h"*ReadSamples, data))
+    elif __DataTypeStr2Int(DataType) == 5:
+        # int32
+        data = list(struct.unpack("i"*ReadSamples, data))
 
     if iqiq:
         data = Iqiq2Complex(data)
     else:
         data = Iiqq2Complex(data)
 
     return data
@@ -135,76 +233,76 @@
     """
 
     import struct
     from datetime import date
     import math
     import logging
 
-    #check if iqData is complex
-    if isinstance( iqData[0], complex):
+    # check if iqData is complex
+    if isinstance(iqData[0], complex):
         iqData = Complex2Iqiq( iqData)
 
     NumberOfSamples = len(iqData) // 2
 
-    #Find maximum magnitude and scale for max to be FullScale (1.0)
+    # Find maximum magnitude and scale for max to be FullScale (1.0)
     power = []
     for n in range(NumberOfSamples):
         power.append(abs(iqData[2*n]**2 + iqData[2*n+1]**2))
     scaling = math.sqrt( max(power))
 
     # normalize to magnitude 1
     iqData = [ iq / scaling for iq in iqData]
 
-    #calculate rms in dB (below full scale)
+    # calculate rms in dB (below full scale)
     rms = math.sqrt(sum(power)/NumberOfSamples)/scaling
     rms = abs(20*math.log10( rms))
     # Convert to int16, use floor function, otherwise distribution is not correct
-    iqData = [ math.floor(iq * 32767 +.5) for iq in iqData]
+    iqData = [ math.floor(iq * 32767 + .5) for iq in iqData]
 
     try:
         file = open( FileName, "wb")
 
         # binary block, big endian
         for nIdx in range(len(iqData)):
-            file.write( struct.pack(">h",iqData[nIdx]))
+            file.write( struct.pack(">h", iqData[nIdx]))
 
         file.close()
     except:
-        logging.error("File (" + FileName +") write error!" )
+        logging.error("File (" + FileName + ") write error!" )
 
     return NumberOfSamples
 
 
 
 def WriteWv( iqData, fSamplingRate, FileName):
     """Writes a WV file.
     iqData can be a list of complex or list of floats (iqiqiq format mandatory).
     writtenSamples = WriteWv("MyFile.wv",complexList, fs)"""
-    
+
     import struct
     from datetime import date
     import math
     import logging
-    
-    #check if iqData is complex
+
+    # check if iqData is complex
     if isinstance( iqData[0], complex):
         iqData = Complex2Iqiq( iqData)
-        
+
     NumberOfSamples = len(iqData) // 2
-         
-    #Find maximum magnitude and scale for max to be FullScale (1.0)
+
+    # Find maximum magnitude and scale for max to be FullScale (1.0)
     power = []
     for n in range(NumberOfSamples):
         power.append(abs(iqData[2*n]**2 + iqData[2*n+1]**2))
-    scaling = math.sqrt( max(power))
-    
+    scaling = math.sqrt(max(power))
+
     # normalize to magnitude 1
-    iqData = [ iq / scaling for iq in iqData]
-    
-    #calculate rms in dB (below full scale)
+    iqData = [iq / scaling for iq in iqData]
+
+    # calculate rms in dB (below full scale)
     rms = math.sqrt(sum(power)/NumberOfSamples)/scaling
     rms = abs(20*math.log10( rms))
     # Convert to int16, use floor function, otherwise distribution is not correct
     iqData = [ math.floor(iq * 32767 +.5) for iq in iqData]
         
     try:
         file = open( FileName, "wb")
@@ -305,94 +403,98 @@
 
     if ReadData:
         return data, SamplingRate
     else:
         return SamplingRate, NumberOfSamples, RmsLevelOffset, RfRmsLevel
 
 
-def __WriteXml(fs, NumberOfSamples, filenameiqw, filenamexml, fCenterFrequency=0):
+def __WriteXml(fs, NumberOfSamples, filenameiqw, filenamexml, fCenterFrequency=0, DataType="float32", ScalingFactor=1):
     """Function to write the xml part of the iq.tar
-    __WriteXml( samplingrate, numberofsamples, filenameiqw, filenamexml)"""
+    __WriteXml( samplingrate, numberofsamples, filenameiqw, filenamexml)
+    DataType (supported): float32, float64
+    ScalingFactor: scaling factor in Volts
+    """
 
     from datetime import datetime
 
     xmlfile = open(filenamexml, "w")
 
     xmlfile.write("<?xml version=\"1.0\" encoding=\"UTF-8\"?>\n")
     xmlfile.write("<?xml-stylesheet type=\"text/xsl\" href=\"open_IqTar_xml_file_in_web_browser.xslt\"?>\n")
     xmlfile.write("<RS_IQ_TAR_FileFormat fileFormatVersion=\"2\" xsi:noNamespaceSchemaLocation=\"http://www.rohde-schwarz.com/file/RsIqTar.xsd\" xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\">\n")
-    #Optional
+    # Optional
     xmlfile.write("<Name>Python iq.tar Writer (iqdata.py)</Name>\n")
-    #Optional
+    # Optional
     xmlfile.write("<Comment>RS WaveForm, TheAE-RA</Comment>\n")
-    xmlfile.write("<DateTime>"+ datetime.now(None).isoformat() +"</DateTime>\n")
+    xmlfile.write("<DateTime>"+ datetime.now(None).isoformat() + "</DateTime>\n")
     xmlfile.write("<Samples>" + str(NumberOfSamples) + "</Samples>\n")
     xmlfile.write("<Clock unit=\"Hz\">" + str(fs) + "</Clock>\n")
     xmlfile.write("<Format>complex</Format>\n")
-    xmlfile.write("<DataType>float32</DataType>\n")
-    #Optional
-    xmlfile.write("<ScalingFactor unit=\"V\">1</ScalingFactor>\n")
-    #Optional
-    #xmlfile.write("<NumberOfChannels>1</NumberOfChannels>\n")
-    xmlfile.write("<DataFilename>" + filenameiqw+ "</DataFilename>\n")
-    #Optional
+    xmlfile.write(f"<DataType>{__DataTypeInt2Str(__DataTypeStr2Int(DataType))}</DataType>\n")
+    # Optional
+    xmlfile.write(f"<ScalingFactor unit=\"V\">{ScalingFactor}</ScalingFactor>\n")
+    # Optional
+    # xmlfile.write("<NumberOfChannels>1</NumberOfChannels>\n")
+    xmlfile.write("<DataFilename>" + filenameiqw + "</DataFilename>\n")
+    # Optional
     if fCenterFrequency != 0:
         xmlfile.write( f'<UserData><RohdeSchwarz><SpectrumAnalyzer><CenterFrequency unit="Hz">{fCenterFrequency}</CenterFrequency></SpectrumAnalyzer></RohdeSchwarz></UserData>\n')
 
     xmlfile.write("</RS_IQ_TAR_FileFormat>\n")
     xmlfile.close()
 
     return
 
 
 
-def WriteIqTar( iqData, fs, FileName, fCenterFrequency = 0):
+def WriteIqTar(iqData, fs, FileName, fCenterFrequency=0, DataType="float32"):
     """Writes an iq.tar file. Complex iqData values are interpreted as Volts.
     iqData can be a list of complex or list of floats (iqiqiq format).
-    writtenSamples = WriteIqTar(iqList,fs,"MyFile.iq.tar")"""
+    writtenSamples = WriteIqTar(iqList,fs,"MyFile.iq.tar")
+    DataType (supported): float32, float64
+    """
 
     import tarfile
     import os
     import re
     import logging
 
-    path,filename = os.path.split(FileName)
-
-    #Create binary file
-    binaryfile = re.sub( "iq.tar", "complex.1ch.float32", filename, flags=re.IGNORECASE)
-    NumberOfSamples = WriteIqw( iqData, os.path.join(path, binaryfile))
+    ScalingFactor = 1
+    path, filename = os.path.split(FileName)
+    # Create binary file
+    binaryfile = re.sub("iq.tar", f"complex.1ch.{__DataTypeInt2Str(__DataTypeStr2Int(DataType))}", filename, flags=re.IGNORECASE)
+    NumberOfSamples, ScalingFactor = WriteIqw(iqData, os.path.join(path, binaryfile), DataType=DataType)
     if NumberOfSamples == 0:
         return 0
 
-    #xsltfilename = "open_IqTar_xml_file_in_web_browser.xslt"
-
-    xmlfilename = re.sub( "iq.tar", "xml", filename, flags=re.IGNORECASE)
-    __WriteXml( fs, NumberOfSamples, binaryfile, os.path.join(path, xmlfilename), fCenterFrequency=fCenterFrequency)
+    # xsltfilename = "open_IqTar_xml_file_in_web_browser.xslt"
+    xmlfilename = re.sub("iq.tar", "xml", filename, flags=re.IGNORECASE)
+    __WriteXml(fs, NumberOfSamples, binaryfile, os.path.join(path, xmlfilename), fCenterFrequency=fCenterFrequency, DataType=DataType, ScalingFactor=ScalingFactor)
 
     try:
-        tar = tarfile.open( FileName, "w")
-        tar.add( os.path.join(path, binaryfile), arcname=binaryfile)
-        #xslt is optional
-        #tar.add( os.path.join(path, xsltfilename), arcname=xsltfilename)
-        tar.add( os.path.join(path, xmlfilename), arcname=xmlfilename)
+        tar = tarfile.open(FileName, "w")
+        tar.add(os.path.join(path, binaryfile), arcname=binaryfile)
+        # xslt is optional
+        # tar.add( os.path.join(path, xsltfilename), arcname=xsltfilename)
+        tar.add(os.path.join(path, xmlfilename), arcname=xmlfilename)
         tar.close()
-        os.remove( os.path.join(path, binaryfile))
-        os.remove( os.path.join(path, xmlfilename))
+        os.remove(os.path.join(path, binaryfile))
+        os.remove(os.path.join(path, xmlfilename))
     except:
         logging.error("IqTar (" + FileName +") write error!" )
 
     return NumberOfSamples
 
 
 
-def ReadIqTar( FileName, ChannelToRead = 1, BytesPerValue = 4):
+def ReadIqTar(FileName, ChannelToRead=1):
     """Reads an iq.tar file. 
     data,fs = ReadIqTar("MyFile.iq.tar", ChannelToRead = 1)
     ChannelToRead specifies the channel to be read. "0" reads all channels and returns a matrix.
-    BytesPerValue specifies the word length per I/Q sample in the file"""
+    """
 
     import tarfile
     import os
     import xml.etree.ElementTree as ET
     import logging
 
     data = []
@@ -405,38 +507,41 @@
         xmlfile = xmlfile[0]
         tar.extract(xmlfile)
         tree = ET.parse(xmlfile)
         root = tree.getroot()
         binaryfilename = root.find("DataFilename").text
         fs = float(root.find("Clock").text)
 
+        helper = root.find("DataType")
+        DataType = __DataTypeInt2Str(__DataTypeStr2Int(helper.text))
+
         helper = root.find("Samples")
         NumberOfSamples = 1
         if helper.text:
             NumberOfSamples = int(root.find("Samples").text)
 
         helper = root.find("ScalingFactor")
         ScalingFactor = 1
         if helper.text:
-            if helper.get("unit")!="V":
+            if helper.get("unit") != "V":
                 logging.warn("Only (V)olts scaling factor supported - assuming 1V!")
             else:
                 ScalingFactor = float(root.find("ScalingFactor").text)
 
         helper = root.find("NumberOfChannels")
         NumberOfChannels = 1
         if helper is not None:
             if helper.text:
                 NumberOfChannels = int(root.find("NumberOfChannels").text)
 
         os.remove(xmlfile)
         del root
         tar.extract(binaryfilename)
         tar.close()
-        data = ReadIqw(binaryfilename, BytesPerValue=BytesPerValue)
+        data = ReadIqw(binaryfilename, DataType=DataType)
         os.remove(binaryfilename)
 
     except:
         logging.error("IqTar (" + FileName + ") read error!")
 
     # Apply scaling factor
     if ScalingFactor != 1:
@@ -462,145 +567,144 @@
                         data1[n][m] = data[n*NumberOfChannels+m]
         data = data1
 
     return data, fs
 
 
 
-def Iqw2Iqtar( FileName, fs, keepIqw = False, fCenterFrequency = 0):
+def Iqw2Iqtar(FileName, fs, keepIqw=False, fCenterFrequency=0, DataType="float32"):
     """Converts an iqw file into iq.tar. Suggested to use after directly reading
     binary data from instrument into file (iqw).
     Note: iqw must be in iqiqiq format
     iqtarFilename = WriteIqTar(iqList,fs,"MyFile.iq.tar")"""
 
     import os
     import tarfile
     import re
     import logging
-    
+
     NumberOfSamples = 0
-    
+
     if os.path.isfile( FileName):
         NumberOfSamples = os.stat( FileName).st_size // 8
     else:
-        logging.error("File "+ FileName+" does not exist!")
-    
-    path,filename = os.path.split(FileName)
-    iqtarfile = re.sub( "iqw", "iq.tar", filename, flags=re.IGNORECASE)
-    xmlfile = re.sub( "iqw", "xml", filename, flags=re.IGNORECASE)
-    binaryfile = re.sub( "iqw", "complex.1ch.float32", filename, flags=re.IGNORECASE)
-    os.rename( FileName, os.path.join(path, binaryfile))
-    
-    __WriteXml( fs, NumberOfSamples, binaryfile, os.path.join(path, xmlfile), fCenterFrequency = fCenterFrequency)
-                          
+        logging.error("File " + FileName+" does not exist!")
+
+    path, filename = os.path.split(FileName)
+    iqtarfile = re.sub("iqw", "iq.tar", filename, flags=re.IGNORECASE)
+    xmlfile = re.sub("iqw", "xml", filename, flags=re.IGNORECASE)
+    binaryfile = re.sub("iqw", f"complex.1ch.{__DataTypeInt2Str(__DataTypeStr2Int(DataType))}", filename, flags=re.IGNORECASE)
+    os.rename(FileName, os.path.join(path, binaryfile))
+
+    __WriteXml(fs, NumberOfSamples, binaryfile, os.path.join(path, xmlfile), fCenterFrequency=fCenterFrequency, Datatype=DataType)
+
     try:
         tar = tarfile.open( os.path.join(path, iqtarfile), "w")
-        tar.add( os.path.join(path, binaryfile), arcname=binaryfile)
-        #xslt is optional
-        #tar.add( os.path.join(path, xsltfilename), arcname=xsltfilename)
-        tar.add( os.path.join(path, xmlfile), arcname=xmlfile)
+        tar.add(os.path.join(path, binaryfile), arcname=binaryfile)
+        # xslt is optional
+        # tar.add( os.path.join(path, xsltfilename), arcname=xsltfilename)
+        tar.add(os.path.join(path, xmlfile), arcname=xmlfile)
         tar.close()
-        if keepIqw == False:
-            os.remove( os.path.join(path, binaryfile))
+        if not keepIqw:
+            os.remove(os.path.join(path, binaryfile))
         else:
-            os.rename( os.path.join(path, binaryfile), FileName)
-        os.remove( os.path.join(path, xmlfile))
+            os.rename(os.path.join(path, binaryfile), FileName)
+        os.remove(os.path.join(path, xmlfile))
     except:
-        logging.error("IqTar (" + FileName +") write error!" )
+        logging.error("IqTar (" + FileName + ") write error!")
 
     return os.path.join(path, iqtarfile)
 
 
 
-def Iqw2Wv( FileName, fs, keepIqw = False):
+def Iqw2Wv(FileName, fs, keepIqw=False):
     """Converts an iqw file into wv. Suggested to use after directly reading
     binary data from instrument into file (iqw).
     Note: iqw must be in iqiqiq format
     writtenSamples = WriteIqTar(iqList,fs,"MyFile.iq.tar")"""
 
     import os
-    import tarfile
     import re
     import logging
     import numpy
     import math
     import struct
     from datetime import date
 
     NumberOfSamples = 0
     BytesPerValue = 4
     BlockSize = 10000
 
-    if os.path.isfile( FileName):
-        NumberOfSamples = os.stat( FileName).st_size // (BytesPerValue * 2)
+    if os.path.isfile(FileName):
+        NumberOfSamples = os.stat(FileName).st_size // (BytesPerValue * 2)
     else:
-        logging.error("File "+ FileName+" does not exist!")
+        logging.error("File " + FileName+" does not exist!")
 
     #path,filename = os.path.split(FileName)
-    wvfile = re.sub( "iqw", "wv", FileName, flags=re.IGNORECASE)
+    wvfile = re.sub("iqw", "wv", FileName, flags=re.IGNORECASE)
 
     rmsvalue = 0
     maxvalue = 0
 
     # first run throug iqw to determine rms and peak level  
     try:
         file = open( FileName, "rb")
         ReadCounter = 0
-        while ReadCounter<NumberOfSamples:
+        while ReadCounter < NumberOfSamples:
             data = file.read(2*BytesPerValue*BlockSize)
             ReadSamples = len(data) // BytesPerValue
             ReadCounter += ReadSamples / 2
             data = list(struct.unpack("f"*ReadSamples, data))
-            data = Iqiq2Complex( data)
-            data = numpy.abs( data)
-            rmsvalue += numpy.sum( numpy.power( numpy.abs(data), 2))
-            maxofvector = numpy.amax( data)
-            maxvalue = max( maxofvector, maxvalue)
+            data = Iqiq2Complex(data)
+            data = numpy.abs(data)
+            rmsvalue += numpy.sum(numpy.power(numpy.abs(data), 2))
+            maxofvector = numpy.amax(data)
+            maxvalue = max(maxofvector, maxvalue)
         file.close
-        rmsvalue = numpy.sqrt( rmsvalue/NumberOfSamples)
+        rmsvalue = numpy.sqrt(rmsvalue/NumberOfSamples)
     except:
-        logging.error( "File open error ("+ FileName+")!")
+        logging.error( "File open error (" + FileName+")!")
 
     scaling = maxvalue
-    maxvalue = 20*numpy.log10( maxvalue/scaling)
-    rmsvalue = 20*numpy.log10( rmsvalue/scaling)
+    maxvalue = 20*numpy.log10(maxvalue/scaling)
+    rmsvalue = 20*numpy.log10(rmsvalue/scaling)
 
     # now we convert the data
     try:
-        fileout = open( wvfile, "wb")     
-        file = open( FileName, "rb")
+        fileout = open(wvfile, "wb")     
+        file = open(FileName, "rb")
 
-        #header
-        fileout.write( "{TYPE: SMU-WV,0}".encode("ASCII"))
-        fileout.write( "{COMMENT: R&S WaveForm, TheAE-RA}".encode("ASCII"))
-        fileout.write( ("{DATE: " + str(date.today())+ "}").encode("ASCII"))
-        fileout.write( ("{CLOCK:" +str(fs) + "}").encode("ASCII"))
-        fileout.write( ("{LEVEL OFFS:" +  "{:2.4f}".format(-1*rmsvalue) + "," + "{:2.4f}".format(maxvalue) + "}").encode("ASCII"))
-        fileout.write( ("{SAMPLES:" + str(NumberOfSamples) + "}").encode("ASCII"))
-        fileout.write( ("{WAVEFORM-" +  str(4*NumberOfSamples+1) + ": #").encode("ASCII"))
+        # header
+        fileout.write("{TYPE: SMU-WV,0}".encode("ASCII"))
+        fileout.write("{COMMENT: R&S WaveForm, TheAE-RA}".encode("ASCII"))
+        fileout.write(("{DATE: " + str(date.today())+ "}").encode("ASCII"))
+        fileout.write(("{CLOCK:" + str(fs) + "}").encode("ASCII"))
+        fileout.write(("{LEVEL OFFS:" + "{:2.4f}".format(-1*rmsvalue) + "," + "{:2.4f}".format(maxvalue) + "}").encode("ASCII"))
+        fileout.write(("{SAMPLES:" + str(NumberOfSamples) + "}").encode("ASCII"))
+        fileout.write(("{WAVEFORM-" + str(4*NumberOfSamples+1) + ": #").encode("ASCII"))
 
         # now copy data from iqw to wv
         ReadCounter = 0
-        while ReadCounter<NumberOfSamples:
+        while ReadCounter < NumberOfSamples:
             data = file.read(2*BytesPerValue*BlockSize)
             ReadSamples = len(data) // BytesPerValue
             ReadCounter += ReadSamples / 2
             data = list(struct.unpack("f"*ReadSamples, data))
             data = data / scaling
             # Convert to int16, use floor function, otherwise distribution is not correct
-            data = [ math.floor(iq * 32767 +.5) for iq in data]
-            fileout.write( struct.pack("h"*len(data),*data))
-  
-        fileout.write( "}".encode("ASCII"))
+            data = [math.floor(iq * 32767 + .5) for iq in data]
+            fileout.write(struct.pack("h"*len(data),*data))
+
+        fileout.write("}".encode("ASCII"))
         fileout.close()
         file.close()
 
         # remove iqw
-        os.remove( FileName)
+        os.remove(FileName)
     except:
-        logging.error("File (" + FileName +") write error!" )    
+        logging.error("File (" + FileName + ") write error!")    
 
 
 
 if __name__ == "__main__":
     # execute only if run as a script
     pass
```

### Comparing `rskfd-0.3.9/rskfd/remote_control/instrument.py` & `rskfd-0.5.0/rskfd/remote_control/instrument.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/rskfd/remote_control/instrumentRS.py` & `rskfd-0.5.0/rskfd/remote_control/instrumentRS.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/rskfd/remote_control/instrumentRSExceptions.py` & `rskfd-0.5.0/rskfd/remote_control/instrumentRSExceptions.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/rskfd/remote_control/instrumentRS_FSW.py` & `rskfd-0.5.0/rskfd/remote_control/instrumentRS_FSW.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/rskfd/remote_control/instrumentRS_VSE.py` & `rskfd-0.5.0/rskfd/remote_control/instrumentRS_VSE.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/rskfd/signal_generation/signal_generation.py` & `rskfd-0.5.0/rskfd/signal_generation/signal_generation.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/rskfd/snp_handling/snpfiles.py` & `rskfd-0.5.0/rskfd/snp_handling/snpfiles.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/rskfd.egg-info/PKG-INFO` & `rskfd-0.5.0/rskfd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.3.9
+Version: 0.5.0
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
```

### Comparing `rskfd-0.3.9/rskfd.egg-info/SOURCES.txt` & `rskfd-0.5.0/rskfd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.9/setup.py` & `rskfd-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   long_description = filein.read()
 
 setuptools.setup(
   name = 'rskfd',
   #packages = ['rskfd','rskfd.remote_control','rskfd.iq_data_handling','rskfd.signal_generation','rskfd.helper'],
   #packages = setuptools.find_packages(),
   packages = setuptools.find_namespace_packages(),
-  version = '0.3.9',
+  version = '0.5.0',
   license='MIT',
   description = 'Python Package for Instrument Control and Data Handling',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   author = 'Florian Ramian', 
   author_email = 'gitlab@ramian.eu',
   url = 'https://gitlab.com/ramian/rskfd',   # gitlab
@@ -21,15 +21,15 @@
   keywords = ['INSTRUMENT CONTROL', 'I/Q DATA','WV','IQ.TAR'],
   install_requires=[
           'numpy',
           'scipy'
       ],
   python_requires='>=3.0',
   classifiers=[
-    'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+    'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Scientific/Engineering',
     'Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
   ],
```

