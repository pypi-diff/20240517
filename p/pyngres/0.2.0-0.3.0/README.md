# Comparing `tmp/pyngres-0.2.0.tar.gz` & `tmp/pyngres-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyngres-0.2.0.tar", last modified: Wed Mar  6 14:40:28 2024, max compression
+gzip compressed data, was "pyngres-0.3.0.tar", last modified: Fri May 17 14:41:20 2024, max compression
```

## Comparing `pyngres-0.2.0.tar` & `pyngres-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-06 14:40:16.000000 pyngres-0.2.0/
--rw-rw-rw-   0        0        0     1086 2023-05-02 12:46:41.000000 pyngres-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      320 2024-03-06 14:40:16.000000 pyngres-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4433 2024-03-06 10:02:09.000000 pyngres-0.2.0/README.md
--rw-rw-rw-   0        0        0      433 2024-03-06 14:40:16.000000 pyngres-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-05-02 12:46:41.000000 pyngres-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-06 14:40:16.000000 pyngres-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-06 14:40:16.000000 pyngres-0.2.0/src/pyngres/
--rw-rw-rw-   0        0        0    20635 2023-07-13 07:49:21.000000 pyngres-0.2.0/src/pyngres/IIAPI_CONSTANTS.py
--rw-rw-rw-   0        0        0    21166 2024-03-06 14:05:32.000000 pyngres-0.2.0/src/pyngres/IIAPI_PARM.py
--rw-rw-rw-   0        0        0     9408 2024-03-06 14:14:58.000000 pyngres-0.2.0/src/pyngres/__init__.py
--rw-rw-rw-   0        0        0     4323 2024-03-04 11:21:19.000000 pyngres-0.2.0/src/pyngres/asyncio.py
--rw-rw-rw-   0        0        0     3863 2024-03-04 11:31:31.000000 pyngres-0.2.0/src/pyngres/blocking.py
-drwxrwxrwx   0        0        0        0 2024-03-06 14:40:16.000000 pyngres-0.2.0/src/pyngres.egg-info/
--rw-rw-rw-   0        0        0      320 2024-03-06 14:40:15.000000 pyngres-0.2.0/src/pyngres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-03-06 14:40:16.000000 pyngres-0.2.0/src/pyngres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-06 14:40:15.000000 pyngres-0.2.0/src/pyngres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-06 14:40:15.000000 pyngres-0.2.0/src/pyngres.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-06 14:40:15.000000 pyngres-0.2.0/src/pyngres.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 14:41:02.000000 pyngres-0.3.0/
+-rw-rw-rw-   0        0        0     1086 2023-05-02 12:46:41.000000 pyngres-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      333 2024-05-17 14:41:02.000000 pyngres-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5146 2024-05-17 09:02:39.000000 pyngres-0.3.0/README.md
+-rw-rw-rw-   0        0        0      448 2024-05-17 14:41:02.000000 pyngres-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-05-02 12:46:41.000000 pyngres-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:41:02.000000 pyngres-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 14:41:02.000000 pyngres-0.3.0/src/pyngres/
+-rw-rw-rw-   0        0        0    23963 2024-05-08 13:15:05.000000 pyngres-0.3.0/src/pyngres/IIAPI_CONSTANTS.py
+-rw-rw-rw-   0        0        0    20916 2024-05-16 09:10:26.000000 pyngres-0.3.0/src/pyngres/IIAPI_PARM.py
+-rw-rw-rw-   0        0        0    14406 2024-05-16 10:32:48.000000 pyngres-0.3.0/src/pyngres/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-03-08 15:42:02.000000 pyngres-0.3.0/src/pyngres/asyncio.py
+-rw-rw-rw-   0        0        0     4011 2024-03-08 15:43:02.000000 pyngres-0.3.0/src/pyngres/blocking.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:41:02.000000 pyngres-0.3.0/src/pyngres.egg-info/
+-rw-rw-rw-   0        0        0      333 2024-05-17 14:41:01.000000 pyngres-0.3.0/src/pyngres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-05-17 14:41:02.000000 pyngres-0.3.0/src/pyngres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 14:41:01.000000 pyngres-0.3.0/src/pyngres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 14:41:01.000000 pyngres-0.3.0/src/pyngres.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 14:41:01.000000 pyngres-0.3.0/src/pyngres.egg-info/top_level.txt
```

### Comparing `pyngres-0.2.0/LICENSE` & `pyngres-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyngres-0.2.0/README.md` & `pyngres-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,103 @@
 # Pyngres
 
-Pyngres is a Python wrapper for the Actian Ingres OpenAPI.
+Pyngres is a Python wrapper for the Actian Ingres/Vector/X OpenAPI. It is
+currently available for Windows, Linux, and Darwin.
 
 ## Installation
 
+Pyngres requires Python 3.8 or higher. 
+
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pyngres.
 
 ```bash
 pip install pyngres
 ```
 
 (Note for **Conda** and **Miniconda** users: there is an as-yet undiagnosed problem that prevents **pip** from properly resolving the dependency on **loguru**. As a workaround install loguru before installing pyngres.)
 
 ## Usage
 
-The pyngres package contains three modules. The pyngres module is a set of
-Python bindings for the Actian OpenAPI. Anyone familiar with the OpenAPI and
+The pyngres package contains three modules. The base **pyngres** module is a set of
+Python bindings for the Actian OpenAPI. It is used exactly like the iilibapi 
+library is used in a C program. The programmer is expected to use `IIapi_wait()` to 
+complete asynchronous OpenAPI calls. Anyone familiar with the OpenAPI and
 with Python programming will find their expertise using the OpenAPI in C is 
-directly transferable.
+directly transferable. 
+
+The second module is **pyngres.asyncio** which makes pyngres
+usable with the Python asyncio package. It provides very clean support for
+the asynchronous OpenAPI functions. The third package is **pyngres.blocking**, which
+simply conceals the busy-wait loops that are required when using the OpenAPI 
+in a synchronous application.
 
 ```python
 import pyngres as ii
 ```
+or
+```python
+import pyngres.asyncio as ii
+```
+or
+```python
+import pyngres.blocking as ii
+```
+
+**Linux** and **Darwin:** initialize your Ingres environment by executing **~/.ing**XX**sh**, where XX
+is your installation identifier (usually **II** or **AC**). Example:
+
+```
+. ~/.ingIIsh
+```
+
+**Windows:** your Ingres installation will usually be initialized already.
+
+Set the `IIAPI_DEV_MODE` environment variable to 'ON' or call `loguru.enable('pyngres')`
+in your application code to start pyngres API tracing using 
+[Loguru](https://loguru.readthedocs.io/en/stable/).
+
 
 ### pyngres.asyncio
 
-The OpenAPI is intrinsically asynchronous. The API sends a request to a 
+The pyngres.asyncio package can be used in place of the bare-bones pyngres
+package. The OpenAPI is intrinsically asynchronous. The OpenAPI sends a request to a 
 server and then returns to the caller without waiting for the request to 
-be completed. It is up to the programmer to insert calls to IIapiWait() 
-to pass control back to the API so that it can set the gp_completed flag 
-and invoke any callback routine that was requested.
+be completed. Ordinarily, using the bare-bones OpenAPI, that would mean
+it is up to the programmer to insert calls to `IIapi_wait()` 
+to pass control back to the OpenAPI so that it can set the gp_completed flag 
+and invoke any callback routine that was requested. Using pyngres.asyncio 
+instead with the Python asyncio features is much tidier.
 
-The Python asyncio package provides design patterns and a well-known
-infrastructure that make asynchronous programming more convenient and support
+Python asyncio provides infrastructure and well-known design patterns that
+make asynchronous programming more convenient and supports
 concurrent execution. The asyncio package facilitates the development of 
-highly responsive event driven applications, such as GUI applications.
+highly responsive event-driven applications, such as GUI applications.
 
-The pyngres.asyncio package can be used in place of the bare-bones pyngres
-package. It supports all the same entry points, but all the asynchronous 
+**pyngres.asyncio** supports all the same entry points, but all the asynchronous 
 OpenAPI functions are awaitable. They are executed in the asyncio event loop
-concurrently with any other awaitables. (The one exception is the IIapi_await()
+concurrently with any other awaitables. (The one exception is the `IIapi_wait()`
 function which does not exist in pyngres.asyncio; it would serve no purpose.)
 
 ```python
 import pyngres.asyncio as ii
 ```
 
 ### pyngres.blocking
 
 OpenAPI applications that have no need to cooperate with other asyncio 
 packages can use the pyngres.blocking package. It is functionally identical
 to the base pyngres package except that all the of the OpenAPI functions 
 block until completion in a platform independent way. This slightly reduces
-the visual clutter of hard-coded loops calling IIapi_wait(), and eliminates
+the visual clutter of hard-coded loops calling `IIapi_wait()`, and eliminates
 the risk of omitting a necessary wait loop. 
 
-The pyngres.blocking package includes a null
-implementation of IIapi_wait() so that pyngres.blocking can simply be
-substituted for pyngres in an existing application without requiring 
-any changes. 
-
 ```python
 import pyngres.blocking as ii
 ```
 
-**Linux:** initialize your Ingres environment by executing **~/.ing**XX**sh**, where XX
-is your installation identifier (usually **II**). Example:
-
-```
-. ~/.ingIIsh
-```
-
-**Windows:** your Ingres installation will usually be initialized already.
-
-Set the `IIAPI_DEV_MODE` environment variable or call `loguru.enable('pyngres')` in your application code to start pyngres API tracing using [Loguru](https://loguru.readthedocs.io/en/stable/).
-
 ## API
 
 See [OpenAPI User Guide](https://docs.actian.com/ingres/11.2/#page/OpenAPIUser/OpenAPIUser_Title.htm) for details on the use the Ingres OpenAPI. The following API functions are supported by pyngres:
 
 - `IIapi_abort()`
 - `IIapi_autocommit()`
 - `IIapi_batch()`
@@ -127,7 +146,8 @@
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
+
```

### Comparing `pyngres-0.2.0/src/pyngres/IIAPI_CONSTANTS.py` & `pyngres-0.3.0/src/pyngres/IIAPI_CONSTANTS.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,123 +19,133 @@
 IIAPI_LEVEL_2 = 2
 IIAPI_LEVEL_3 = 3
 IIAPI_LEVEL_4 = 4
 IIAPI_LEVEL_5 = 5
 IIAPI_LEVEL_6 = 6
 IIAPI_LEVEL_7 = 7
 
-IIAPI_DTE_TYPE = 3
+IIAPI_HNDL_TYPE = -1       ## API Handle 
+IIAPI_CHR_TYPE = 32        ## Text Fixed 
+IIAPI_CHA_TYPE = 20        ## Character Fixed 
+IIAPI_VCH_TYPE = 21        ## Character Variable 
+IIAPI_LVCH_TYPE = 22       ## Character Long 
+IIAPI_LCLOC_TYPE = 36      ## Character Long Locator 
+IIAPI_BYTE_TYPE = 23       ## Binary Fixed 
+IIAPI_VBYTE_TYPE = 24      ## Binary Variable 
+IIAPI_LBYTE_TYPE = 25      ## Binary Long 
+IIAPI_LBLOC_TYPE = 35      ## Binary Long Locator 
+IIAPI_NCHA_TYPE = 26       ## Unicode Fixed 
+IIAPI_NVCH_TYPE = 27       ## Unicode Variable 
+IIAPI_LNVCH_TYPE = 28      ## Unicode Long 
+IIAPI_LNLOC_TYPE = 29      ## Unicode Long Locator 
+IIAPI_TXT_TYPE = 37        ## Text Variable 
+IIAPI_LTXT_TYPE = 41       ## Text Var (typeless NULL) 
+IIAPI_INT_TYPE = 30        ## Integer 
+IIAPI_FLT_TYPE = 31        ## Floating Point 
+IIAPI_MNY_TYPE =  5        ## Money 
+IIAPI_DEC_TYPE = 10        ## Decimal 
+IIAPI_BOOL_TYPE = 38       ## Boolean 
+IIAPI_UUID_TYPE = 55       ## UUID 
+IIAPI_IPV4_TYPE = 66       ## IPv4 
+IIAPI_IPV6_TYPE = 67       ## IPv6 
+IIAPI_DTE_TYPE =  3        ## Ingres Date 
 IIAPI_IDATE_TYPE = IIAPI_DTE_TYPE
-IIAPI_DATE_TYPE = 4
+IIAPI_DATE_TYPE =  4       ## ANSI Date 
 IIAPI_ADATE_TYPE = IIAPI_DATE_TYPE
-IIAPI_MNY_TYPE = 5
-IIAPI_TMWO_TYPE = 6
-IIAPI_TMTZ_TYPE = 7
-IIAPI_TIME_TYPE = 8
-IIAPI_TSWO_TYPE = 9
-IIAPI_DEC_TYPE = 10
-IIAPI_LOGKEY_TYPE = 11
-IIAPI_TABKEY_TYPE = 12
-IIAPI_TSTZ_TYPE = 18
-IIAPI_TS_TYPE = 19
-IIAPI_CHA_TYPE = 20
-IIAPI_VCH_TYPE = 21
-IIAPI_LVCH_TYPE = 22
-IIAPI_BYTE_TYPE = 23
-IIAPI_VBYTE_TYPE = 24
-IIAPI_LBYTE_TYPE = 25
-IIAPI_NCHA_TYPE = 26
-IIAPI_NVCH_TYPE = 27
-IIAPI_LNVCH_TYPE = 28
-IIAPI_INT_TYPE = 30
-IIAPI_FLT_TYPE = 31
-IIAPI_CHR_TYPE = 32
-IIAPI_INTYM_TYPE = 33
-IIAPI_INTDS_TYPE = 34
-IIAPI_TXT_TYPE = 37
-IIAPI_BOOL_TYPE = 38
-IIAPI_LTXT_TYPE = 41
-IIAPI_UUID_TYPE = 55
-IIAPI_GEOM_TYPE = 56
-IIAPI_POINT_TYPE = 57
-IIAPI_MPOINT_TYPE = 58
-IIAPI_LINE_TYPE = 59
-IIAPI_MLINE_TYPE = 61
-IIAPI_POLY_TYPE = 62
-IIAPI_MPOLY_TYPE = 63
-IIAPI_NBR_TYPE = 64
-IIAPI_GEOMC_TYPE = 65
-IIAPI_IPV4_TYPE = 66
-IIAPI_IPV6_TYPE = 67
-IIAPI_CURVE_TYPE = 68
-IIAPI_SURF_TYPE = 69
-IIAPI_PSURF_TYPE = 70
-IIAPI_GEOMZ_TYPE = 71
-IIAPI_POINTZ_TYPE = 72
-IIAPI_LINEZ_TYPE = 73
-IIAPI_POLYZ_TYPE = 74
-IIAPI_MPOINTZ_TYPE = 75
-IIAPI_MLINEZ_TYPE = 76
-IIAPI_MPOLYZ_TYPE = 77
-IIAPI_GEOMCZ_TYPE = 78
-IIAPI_CURVEZ_TYPE = 79
-IIAPI_SURFZ_TYPE = 80
-IIAPI_PSURFZ_TYPE = 81
-IIAPI_GEOMM_TYPE = 82
-IIAPI_POINTM_TYPE = 83
-IIAPI_LINEM_TYPE = 84
-IIAPI_POLYM_TYPE = 85
-IIAPI_MPOINTM_TYPE = 86
-IIAPI_MLINEM_TYPE = 87
-IIAPI_MPOLYM_TYPE = 88
-IIAPI_GEOMCM_TYPE = 89
-IIAPI_CURVEM_TYPE = 90
-IIAPI_SURFM_TYPE = 91
-IIAPI_PSURFM_TYPE = 92
-IIAPI_GEOMZM_TYPE = 93
-IIAPI_POINTZM_TYPE = 94
-IIAPI_LINEZM_TYPE = 95
-IIAPI_POLYZM_TYPE = 100
-IIAPI_MPOINTZM_TYPE = 101
-IIAPI_MLINEZM_TYPE = 102
-IIAPI_MPOLYZM_TYPE = 103
-IIAPI_GEOMCZM_TYPE = 104
-IIAPI_CURVEZM_TYPE = 105
-IIAPI_SURFZM_TYPE = 106
-IIAPI_PSURFZM_TYPE = 107
-IIAPI_MCURVE_TYPE = 108
-IIAPI_MSURF_TYPE = 109
-IIAPI_MCURVEZ_TYPE = 110
-IIAPI_MSURFZ_TYPE = 111
-IIAPI_MCURVEM_TYPE = 112
-IIAPI_MSURFM_TYPE = 113
-IIAPI_MCURVEZM_TYPE = 114
-IIAPI_MSURFZM_TYPE = 115
-IIAPI_CSTR_TYPE = 116
-IIAPI_CSTRZ_TYPE = 117
-IIAPI_CSTRM_TYPE = 118
-IIAPI_CSTRZM_TYPE = 119
-IIAPI_CCURVE_TYPE = 120
-IIAPI_CCURVEZ_TYPE = 121
-IIAPI_CCURVEM_TYPE = 122
-IIAPI_CCURVEZM_TYPE = 123
-IIAPI_CPOLY_TYPE = 124
-IIAPI_CPOLYZ_TYPE = 125
-IIAPI_CPOLYM_TYPE = 126
-IIAPI_CPOLYZM_TYPE = 127
-IIAPI_TIN_TYPE = 128
-IIAPI_TINZ_TYPE = 129
-IIAPI_TINM_TYPE = 130
-IIAPI_TINZM_TYPE = 131
-IIAPI_TRI_TYPE = 132
-IIAPI_TRIZ_TYPE = 133
-IIAPI_TRIM_TYPE = 134
-IIAPI_TRIZM_TYPE = 135
-IIAPI_BOX_TYPE = 136
-IIAPI_BOXZ_TYPE = 137
+IIAPI_TIME_TYPE =  8       ## Time 
+IIAPI_TMWO_TYPE =  6       ## Time without Timezone 
+IIAPI_TMTZ_TYPE =  7       ## Time with Timezone 
+IIAPI_TS_TYPE = 19         ## Timestamp 
+IIAPI_TSWO_TYPE =  9       ## Timestamp without Timezone 
+IIAPI_TSTZ_TYPE = 18       ## Timestamp with Timezone 
+IIAPI_INTYM_TYPE = 33      ## Interval Year to Month 
+IIAPI_INTDS_TYPE = 34      ## Interval Day to Second 
+IIAPI_LOGKEY_TYPE = 11     ## Logical Key 
+IIAPI_TABKEY_TYPE = 12     ## Table Key 
+IIAPI_GEOM_TYPE = 56       ## Spatial Long Byte 
+IIAPI_POINT_TYPE = 57      ## Point Long Byte 
+IIAPI_MPOINT_TYPE = 58     ## MPoint Long Byte 
+IIAPI_LINE_TYPE = 59       ## Line Long Byte 
+IIAPI_MLINE_TYPE = 61      ## MLine Long Byte 
+IIAPI_POLY_TYPE = 62       ## Poly Long Byte 
+IIAPI_MPOLY_TYPE = 63      ## Mpoly Long Byte 
+IIAPI_NBR_TYPE = 64        ## NBR Byte 
+IIAPI_GEOMC_TYPE = 65      ## Geomc Long Byte 
+IIAPI_CURVE_TYPE = 68      ## CURVE Spatial Type 
+IIAPI_SURF_TYPE = 69       ## SURF Spatial Type 
+IIAPI_PSURF_TYPE = 70      ## PSURF Spatial Type 
+IIAPI_GEOMZ_TYPE = 71      ## GEOMZ Spatial Type 
+IIAPI_POINTZ_TYPE = 72     ## POINTZ Spatial Type 
+IIAPI_LINEZ_TYPE = 73      ## LINEZ Spatial Type 
+IIAPI_POLYZ_TYPE = 74      ## POLYZ Spatial Type 
+IIAPI_MPOINTZ_TYPE = 75    ## MPOINTZ Spatial Type 
+IIAPI_MLINEZ_TYPE = 76     ## MLINEZ Spatial Type 
+IIAPI_MPOLYZ_TYPE = 77     ## MPOLYZ Spatial Type 
+IIAPI_GEOMCZ_TYPE = 78     ## GEOMCZ Spatial Type 
+IIAPI_CURVEZ_TYPE = 79     ## CURVEZ Spatial Type 
+IIAPI_SURFZ_TYPE = 80      ## SURFZ Spatial Type 
+IIAPI_PSURFZ_TYPE = 81     ## PSURFZ Spatial Type 
+IIAPI_GEOMM_TYPE = 82      ## GEOMM Spatial Type 
+IIAPI_POINTM_TYPE = 83     ## POINTM Spatial Type 
+IIAPI_LINEM_TYPE = 84      ## LINEM Spatial Type 
+IIAPI_POLYM_TYPE = 85      ## POLYM Spatial Type 
+IIAPI_MPOINTM_TYPE = 86    ## MPOINTM Spatial Type 
+IIAPI_MLINEM_TYPE = 87     ## MLINEM Spatial Type 
+IIAPI_MPOLYM_TYPE = 88     ## MPOLYM Spatial Type 
+IIAPI_GEOMCM_TYPE = 89     ## GEOMCM Spatial Type 
+IIAPI_CURVEM_TYPE = 90     ## CURVEM Spatial Type 
+IIAPI_SURFM_TYPE = 91      ## SURFM Spatial Type 
+IIAPI_PSURFM_TYPE = 92     ## PSURFM Spatial Type 
+IIAPI_GEOMZM_TYPE = 93     ## GEOMZM Spatial Type 
+IIAPI_POINTZM_TYPE = 94    ## POINTZM Spatial Type 
+IIAPI_LINEZM_TYPE = 95     ## LINEZM Spatial Type 
+IIAPI_POLYZM_TYPE = 100    ## POLYZM Spatial Type 
+IIAPI_MPOINTZM_TYPE = 101  ## MPOINTZM Spatial Type 
+IIAPI_MLINEZM_TYPE = 102   ## MLINEZM Spatial Type 
+IIAPI_MPOLYZM_TYPE = 103   ## MPOLYZM Spatial Type 
+IIAPI_GEOMCZM_TYPE = 104   ## GEOMCZM Spatial Type 
+IIAPI_CURVEZM_TYPE = 105   ## CURVEZM Spatial Type 
+IIAPI_SURFZM_TYPE = 106    ## SURFZM Spatial Type 
+IIAPI_PSURFZM_TYPE = 107   ## PSURFZM Spatial Type 
+IIAPI_MCURVE_TYPE = 108    ## MCURVE Spatial Type 
+IIAPI_MSURF_TYPE = 109     ## MSURF Spatial Type 
+IIAPI_MCURVEZ_TYPE = 110   ## MCURVEZ Spatial Type 
+IIAPI_MSURFZ_TYPE = 111    ## MSURFZ Spatial Type 
+IIAPI_MCURVEM_TYPE = 112   ## MCURVEM Spatial Type 
+IIAPI_MSURFM_TYPE = 113    ## MSURFM Spatial Type 
+IIAPI_MCURVEZM_TYPE = 114  ## MCURVEZM Spatial Type 
+IIAPI_MSURFZM_TYPE = 115   ## MSURFZM Spatial Type 
+IIAPI_CSTR_TYPE = 116      ## CSTR Spatial Type 
+IIAPI_CSTRZ_TYPE = 117     ## CSTRZ Spatial Type 
+IIAPI_CSTRM_TYPE = 118     ## CSTRM Spatial Type 
+IIAPI_CSTRZM_TYPE = 119    ## CSTRZM Spatial Type 
+IIAPI_CCURVE_TYPE = 120    ## CCURVE Spatial Type 
+IIAPI_CCURVEZ_TYPE = 121   ## CCURVEZ Spatial Type 
+IIAPI_CCURVEM_TYPE = 122   ## CCURVEM Spatial Type 
+IIAPI_CCURVEZM_TYPE = 123  ## CCURVEZM Spatial Type 
+IIAPI_CPOLY_TYPE = 124     ## CPOLY Spatial Type 
+IIAPI_CPOLYZ_TYPE = 125    ## CPOLYZ Spatial Type 
+IIAPI_CPOLYM_TYPE = 126    ## CPOLYM Spatial Type 
+IIAPI_CPOLYZM_TYPE = 127   ## CPOLYZM Spatial Type 
+IIAPI_TIN_TYPE = 128       ## TIN Spatial Type 
+IIAPI_TINZ_TYPE = 129      ## TINZ Spatial Type 
+IIAPI_TINM_TYPE = 130      ## TINM Spatial Type 
+IIAPI_TINZM_TYPE = 131     ## TINZM Spatial Type 
+IIAPI_TRI_TYPE = 132       ## TRI Spatial Type 
+IIAPI_TRIZ_TYPE = 133      ## TRIZ Spatial Type 
+IIAPI_TRIM_TYPE = 134      ## TRIM Spatial Type 
+IIAPI_TRIZM_TYPE = 135     ## TRIZM Spatial Type 
+IIAPI_BOX_TYPE = 136       ## BOX Spatial Type 
+IIAPI_BOXZ_TYPE = 137      ## BOXZ Spatial Type 
+
+IIAPI_VAR_TYPES = {IIAPI_VBYTE_TYPE, IIAPI_VCH_TYPE, IIAPI_NVCH_TYPE}
+IIAPI_LONG_TYPES = {IIAPI_LVCH_TYPE, IIAPI_LBYTE_TYPE, IIAPI_LNVCH_TYPE, 
+    IIAPI_GEOM_TYPE, IIAPI_POINT_TYPE, IIAPI_MPOINT_TYPE,
+    IIAPI_LINE_TYPE, IIAPI_MLINE_TYPE, IIAPI_POLY_TYPE,
+    IIAPI_MPOLY_TYPE, IIAPI_NBR_TYPE, IIAPI_GEOMC_TYPE}
 
 
 IIAPI_BOOL_LEN = 1
 IIAPI_DATE_LEN = 4
 IIAPI_ADATE_LEN = IIAPI_DATE_LEN
 IIAPI_DTE_LEN = 12
 IIAPI_EP_MAX_SEGMENT_LEN = 24
```

### Comparing `pyngres-0.2.0/src/pyngres/IIAPI_PARM.py` & `pyngres-0.3.0/src/pyngres/IIAPI_PARM.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import ctypes
+import ctypes as C
 import os
 import struct
 from loguru import logger
 
 from .IIAPI_CONSTANTS import *
 
 
 ##  the following are known from iiapidep.h
-II_BOOL = ctypes.c_int  ##  II_BOOL is not what you might guess...
-II_CHAR = ctypes.c_char
-II_FLOAT4 = ctypes.c_float
-II_FLOAT8 = ctypes.c_double
-II_INT = ctypes.c_int
-II_INT1 = ctypes.c_char
-II_INT2 = ctypes.c_short
-II_INT4 = ctypes.c_int
-II_INT8 = ctypes.c_longlong
-II_LONG = ctypes.c_int
-II_PTR = ctypes.c_void_p
-II_STR = ctypes.c_char_p  ##  use for e.g. II_CHAR II_FAR *string
-II_UCHAR = ctypes.c_ubyte
-II_UINT1 = ctypes.c_ubyte
-II_UINT2 = ctypes.c_ushort
-II_UINT4 = ctypes.c_uint
-II_UINT8 = ctypes.c_ulonglong
-II_ULONG = ctypes.c_uint
+II_BOOL = C.c_int  ##  II_BOOL is not what you might guess...
+II_CHAR = C.c_char
+II_FLOAT4 = C.c_float
+II_FLOAT8 = C.c_double
+II_INT = C.c_int
+II_INT1 = C.c_char
+II_INT2 = C.c_short
+II_INT4 = C.c_int
+II_INT8 = C.c_longlong
+II_LONG = C.c_int
+II_PTR = C.c_void_p
+II_STR = C.c_char_p  ##  use for e.g. II_CHAR II_FAR *string
+II_UCHAR = C.c_ubyte
+II_UINT1 = C.c_ubyte
+II_UINT2 = C.c_ushort
+II_UINT4 = C.c_uint
+II_UINT8 = C.c_ulonglong
+II_ULONG = C.c_uint
 
 IIAPI_DT_ID = II_INT2
 IIAPI_QUERYTYPE = II_ULONG
 IIAPI_STATUS = II_ULONG
 
 
 ##  defining the IIAPI_DEV_MODE envar puts the API in development mode
 if 'IIAPI_DEV_MODE' in os.environ:
     IIAPI_DEV_MODE = True
 else:
     IIAPI_DEV_MODE = False
 
 
-class IIAPI(ctypes.Structure):
+class IIAPI(C.Structure):
     '''structures for the Ingres OpenAPI'''
 
     if IIAPI_DEV_MODE:
         ##  this checking is only useful during development
         def __setattr__(self, name, value):
             '''prevent undeclared attributes from being set'''
             names = [name for name, type in self._fields_]
@@ -71,16 +71,18 @@
 
 
     def field_by_suffix(self,suffix):
         '''get a structure field using only its name-suffix'''
 
         prefix = self._field_name_prefix()
         full_name = prefix + '_' + suffix
-        ##  don't use try/except here; let it be fatal
-        field = getattr(self,full_name)
+        try:
+            field = getattr(self,full_name)
+        except AttributeError:
+            field = None
         return field
 
 
     def genParm(self):
         '''return the genParm field (if any)'''
 
         return self.field_by_suffix('genParm')
@@ -169,27 +171,27 @@
 class IIAPI_FDATADESCR(IIAPI_MEMBER):
     '''
     This data type describes the data in a copy file. It also describes
     how the file should be formatted.
     '''
 
     _fields_ = [
-        ('fd_name', ctypes.c_char_p),
-        ('fd_type', ctypes.c_short),
-        ('fd_length', ctypes.c_short),
-        ('fd_prec', ctypes.c_short),
-        ('fd_column', ctypes.c_int),
-        ('fd_funcID', ctypes.c_int),
-        ('fd_cvLen', ctypes.c_int),
-        ('fd_cvPrec', ctypes.c_int),
-        ('fd_delimiter', ctypes.c_bool),
-        ('fd_delimLength', ctypes.c_short),
-        ('fd_delimValue', ctypes.c_char_p),
-        ('fd_nullable', ctypes.c_bool),
-        ('fd_nullInfo', ctypes.c_bool),
+        ('fd_name', C.c_char_p),
+        ('fd_type', C.c_short),
+        ('fd_length', C.c_short),
+        ('fd_prec', C.c_short),
+        ('fd_column', C.c_int),
+        ('fd_funcID', C.c_int),
+        ('fd_cvLen', C.c_int),
+        ('fd_cvPrec', C.c_int),
+        ('fd_delimiter', C.c_bool),
+        ('fd_delimLength', C.c_short),
+        ('fd_delimValue', C.c_char_p),
+        ('fd_nullable', C.c_bool),
+        ('fd_nullInfo', C.c_bool),
         ('fd_nullDescr', IIAPI_DESCRIPTOR),
         ('fd_nullValue', IIAPI_DATAVALUE),
     ]
 
 
 class IIAPI_COPYMAP(IIAPI_MEMBER):
     '''
@@ -202,17 +204,17 @@
     _fields_ = [
         ('cp_copyFrom', II_BOOL),
         ('cp_flags', II_ULONG),
         ('cp_errorCount', II_LONG),
         ('cp_fileName', II_STR),
         ('cp_logName', II_STR),
         ('cp_dbmsCount', II_INT2),
-        ('cp_dbmsDescr', ctypes.POINTER(IIAPI_DESCRIPTOR)),
+        ('cp_dbmsDescr', C.POINTER(IIAPI_DESCRIPTOR)),
         ('cp_fileCount', II_INT2),
-        ('cp_fileDescr', ctypes.POINTER(IIAPI_FDATADESCR)),
+        ('cp_fileDescr', C.POINTER(IIAPI_FDATADESCR)),
     ]
 
 
 class IIAPI_SVR_ERRINFO(IIAPI_MEMBER):
     '''additional server information associated with error messages'''
 
     # svr_severity (from iiapi.h):
@@ -224,16 +226,16 @@
     _fields_ = [
         ('svr_id_error', II_LONG),
         ('svr_local_error', II_LONG),
         ('svr_id_server', II_LONG),
         ('svr_server_type', II_LONG),
         ('svr_severity', II_LONG),
         ('svr_parmCount', II_INT2),
-        ('svr_parmDescr', ctypes.POINTER(IIAPI_DESCRIPTOR)),
-        ('svr_parmValue', ctypes.POINTER(IIAPI_DATAVALUE)),
+        ('svr_parmDescr', C.POINTER(IIAPI_DESCRIPTOR)),
+        ('svr_parmValue', C.POINTER(IIAPI_DATAVALUE)),
     ]
 
 
 class IIAPI_II_TRAN_ID(IIAPI_MEMBER):
     '''Ingres transaction ID'''
 
     _fields_ = [
@@ -269,15 +271,15 @@
         ('xa_tranID', IIAPI_XA_TRAN_ID),
         ('xa_branchSeqnum', II_INT4),
         ('xa_branchFlag', II_INT4),
     ]
 
 
 ##  NB this is a union not a struct
-class IIAPI_2PC_TRAN_ID(ctypes.Union):
+class IIAPI_2PC_TRAN_ID(C.Union):
     '''2PC transaction identifier'''
 
     _fields_ = [
         ('iiXID', IIAPI_II_DIS_TRAN_ID), 
         ('xaXID', IIAPI_XA_DIS_TRAN_ID)
     ]
 
@@ -313,25 +315,25 @@
 
 
 class IIAPI_ABORTPARM(IIAPI_PARM):
     '''parameter block for IIapi_abort'''
 
     _fields_ = [
         ('ab_genParm', IIAPI_GENPARM), 
-        ('ab_connHandle', ctypes.c_void_p)
+        ('ab_connHandle', C.c_void_p)
     ]
 
 
 class IIAPI_AUTOPARM(IIAPI_PARM):
     '''parameter block for IIapi_autocommit'''
 
     _fields_ = [
         ('ac_genParm', IIAPI_GENPARM),
-        ('ac_connHandle', ctypes.c_void_p),
-        ('ac_tranHandle', ctypes.c_void_p),
+        ('ac_connHandle', C.c_void_p),
+        ('ac_tranHandle', C.c_void_p),
     ]
 
 
 class IIAPI_BATCHPARM(IIAPI_PARM):
     '''parameter block for IIapi_batch'''
 
     _fields_ = [
@@ -416,15 +418,15 @@
     _fields_ = [('dc_genParm', IIAPI_GENPARM), ('dc_connHandle', II_PTR)]
 
 
 class IIAPI_EVENTPARM(IIAPI_PARM):
     '''parameter block for setting up an event handler'''
 
     _fields_ = [
-        ('ev_endHandle', II_PTR),
+        ('ev_envHandle', II_PTR),
         ('ev_connHandle', II_PTR),
         ('ev_eventName', II_STR),
         ('ev_eventOwner', II_STR),
         ('ev_eventDB', II_STR),
         ('ev_eventTime', IIAPI_DATAVALUE),
     ]
 
@@ -446,15 +448,15 @@
     '''parameter block for IIapi_getColumns'''
 
     _fields_ = [
         ('gc_genParm', IIAPI_GENPARM),
         ('gc_stmtHandle', II_PTR),
         ('gc_rowCount', II_INT2),  # incorrectly documented II_INT
         ('gc_columnCount', II_INT2),  # incorrectly documented II_INT
-        ('gc_columnData', ctypes.POINTER(IIAPI_DATAVALUE)),
+        ('gc_columnData', C.POINTER(IIAPI_DATAVALUE)),
         ('gc_rowsReturned', II_INT2),  # incorrectly documented II_INT
         ('gc_moreSegments', II_BOOL),
     ]
 
 
 class IIAPI_GETCOLINFOPARM(IIAPI_PARM):
     '''parameter block for IIapi_getColumnInfo'''
@@ -481,40 +483,40 @@
 class IIAPI_GETDESCRPARM(IIAPI_PARM):
     '''query result descriptor block'''
 
     _fields_ = [
         ('gd_genParm', IIAPI_GENPARM),
         ('gd_stmtHandle', II_PTR),
         ('gd_descriptorCount', II_INT2),
-        ('gd_descriptor', ctypes.POINTER(IIAPI_DESCRIPTOR)),
+        ('gd_descriptor', C.POINTER(IIAPI_DESCRIPTOR)),
     ]
 
 
 class IIAPI_GETEINFOPARM(IIAPI_PARM):
     '''OpenAPI parameter block for returning error and user-defined info'''
 
     _fields_ = [
         ('ge_errorHandle', II_PTR),
         ('ge_type', II_LONG),
         ('ge_SQLSTATE', II_CHAR * (II_SQLSTATE_LEN + 1)),
         ('ge_errorCode', II_LONG),
         ('ge_message', II_STR),
         ('ge_serverInfoAvail', II_BOOL),
-        ('ge_serverInfo', ctypes.POINTER(IIAPI_SVR_ERRINFO)),
+        ('ge_serverInfo', C.POINTER(IIAPI_SVR_ERRINFO)),
         ('ge_status', IIAPI_STATUS),
     ]
 
 
 class IIAPI_GETEVENTPARM(IIAPI_PARM):
     '''parameter block for IIapi_getEvent'''
 
     _fields_ = [
         ('gv_genParm', IIAPI_GENPARM),
-        ('gv_connHandle', ctypes.c_void_p),
-        ('gv_timeout', ctypes.c_int),
+        ('gv_connHandle', C.c_void_p),
+        ('gv_timeout', C.c_int),
     ]
 
 
 class IIAPI_GETQINFOPARM(IIAPI_PARM):
     '''parameter block for IIapi_getQueryInfo()'''
 
     _fields_ = [
@@ -577,27 +579,27 @@
 class IIAPI_PUTCOLPARM(IIAPI_PARM):
     '''parameter block for IIapi_putColumns()'''
 
     _fields_ = [
         ('pc_genParm', IIAPI_GENPARM),
         ('pc_stmtHandle', II_PTR),
         ('pc_columnCount', II_INT2),
-        ('pc_columnData', ctypes.POINTER(IIAPI_DATAVALUE)),
+        ('pc_columnData', C.POINTER(IIAPI_DATAVALUE)),
         ('pc_moreSegments', II_BOOL),
     ]
 
 
 class IIAPI_PUTPARMPARM(IIAPI_PARM):
     '''parameter block for IIapi_putParms()'''
 
     _fields_ = [
         ('pp_genParm', IIAPI_GENPARM),
         ('pp_stmtHandle', II_PTR),
         ('pp_parmCount', II_INT2),
-        ('pp_parmData', ctypes.POINTER(IIAPI_DATAVALUE)),
+        ('pp_parmData', C.POINTER(IIAPI_DATAVALUE)),
         ('pp_moreSegments', II_BOOL),
     ]
 
 
 class IIAPI_QUERYPARM(IIAPI_PARM):
     '''parameter block for IIapi_query()'''
 
@@ -668,39 +670,39 @@
 
 
 class IIAPI_SETCONPRMPARM(IIAPI_PARM):
     '''parameter block for setConnectParam()'''
 
     _fields_ = [
         ('sc_genParm', IIAPI_GENPARM),
-        ('sc_connHandle', ctypes.c_void_p),
-        ('sc_paramID', ctypes.c_int),
-        ('sc_paramValue', ctypes.c_void_p),
+        ('sc_connHandle', C.c_void_p),
+        ('sc_paramID', C.c_int),
+        ('sc_paramValue', C.c_void_p),
     ]
 
 
 class IIAPI_SETDESCRPARM(IIAPI_PARM):
     '''parameter block for IIapi_setDescriptor()'''
 
     _fields_ = [
         ('sd_genParm', IIAPI_GENPARM),
         ('sd_stmtHandle', II_PTR),
         ('sd_descriptorCount', II_INT2),
-        ('sd_descriptor', ctypes.POINTER(IIAPI_DESCRIPTOR)),
+        ('sd_descriptor', C.POINTER(IIAPI_DESCRIPTOR)),
     ]
 
 
 class IIAPI_SETENVPRMPARM(IIAPI_PARM):
     '''parameter block for IIapi_setEnvParam()'''
 
     _fields_ = [
-        ('se_envHandle', ctypes.c_void_p),
-        ('se_paramID', ctypes.c_int),
-        ('se_paramValue', ctypes.c_void_p),
-        ('se_status', ctypes.c_uint),
+        ('se_envHandle', C.c_void_p),
+        ('se_paramID', C.c_int),
+        ('se_paramValue', C.c_void_p),
+        ('se_status', C.c_uint),
     ]
 
 
 class IIAPI_TERMPARM(IIAPI_PARM):
     '''parameter block for terminating the Ingres OpenAPI'''
 
     _fields_ = [('tm_status', IIAPI_STATUS)]
```

### Comparing `pyngres-0.2.0/src/pyngres/asyncio.py` & `pyngres-0.3.0/src/pyngres/asyncio.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from .IIAPI_CONSTANTS import *
 from .IIAPI_PARM import *
 ##  the following functions are synchronous and not awaitable; we just
 ##  import them into the pyngres.asyncio namespace
 from pyngres import ( IIapi_convertData, IIapi_formatData, IIapi_getColumnInfo, 
     IIapi_getErrorInfo, IIapi_initialize, IIapi_registerXID, IIapi_releaseEnv, 
     IIapi_releaseXID, IIapi_setEnvParam, IIapi_terminate ) 
+##  import the callback helper functions
+from pyngres import ( IIapi_callback, IIapi_getCallbackPtr,
+    IIapi_getClosurePtr, IIapi_getClosure ) 
 
 
 ##  the IIAPI_DEV_MODE envar puts pyngres.asyncio in development mode
 _name = __name__
 if 'IIAPI_DEV_MODE' in os.environ:
     IIAPI_DEV_MODE = True
     logger.warning(f'using {_name} in development mode')
```

### Comparing `pyngres-0.2.0/src/pyngres/blocking.py` & `pyngres-0.3.0/src/pyngres/blocking.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from .IIAPI_CONSTANTS import *
 from .IIAPI_PARM import *
 ##  the following functions are fundamentally synchronous; we just
 ##  import them into the pyngres.syncio namespace
 from pyngres import ( IIapi_convertData, IIapi_formatData, IIapi_getColumnInfo, 
     IIapi_getErrorInfo, IIapi_initialize, IIapi_registerXID, IIapi_releaseEnv, 
     IIapi_releaseXID, IIapi_setEnvParam, IIapi_terminate ) 
+##  import the callback helper functions
+from pyngres import ( IIapi_callback, IIapi_getCallbackPtr,
+    IIapi_getClosurePtr, IIapi_getClosure )
 
 
 ##  the IIAPI_DEV_MODE envar puts pyngres.syncio in development mode
 _name = __name__
 if 'IIAPI_DEV_MODE' in os.environ:
     IIAPI_DEV_MODE = True
     logger.warning(f'using {_name} in development mode')
```

