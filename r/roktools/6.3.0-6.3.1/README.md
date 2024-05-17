# Comparing `tmp/roktools-6.3.0.tar.gz` & `tmp/roktools-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roktools-6.3.0.tar", max compression
+gzip compressed data, was "roktools-6.3.1.tar", max compression
```

## Comparing `roktools-6.3.0.tar` & `roktools-6.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-05-05 08:08:57.792210 roktools-6.3.0/LICENSE
--rw-r--r--   0        0        0     1665 2024-05-05 08:08:57.792210 roktools-6.3.0/README.md
--rw-r--r--   0        0        0     1162 2024-05-05 08:08:57.792210 roktools-6.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/__init__.py
--rw-r--r--   0        0        0     4509 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/cl.py
--rw-r--r--   0        0        0      133 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/constants.py
--rw-r--r--   0        0        0      491 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/decorator.py
--rw-r--r--   0        0        0      933 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/file.py
--rw-r--r--   0        0        0    33628 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/geodetic.py
--rw-r--r--   0        0        0        0 2024-05-05 08:08:57.844210 roktools-6.3.0/roktools/gnss/__init__.py
--rw-r--r--   0        0        0     1884 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/gnss/edit.py
--rw-r--r--   0        0        0     1644 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/gnss/observables.py
--rw-r--r--   0        0        0     1244 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/gnss/residuals.py
--rw-r--r--   0        0        0     9572 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/gnss/types.py
--rw-r--r--   0        0        0     1479 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/logger.py
--rw-r--r--   0        0        0        0 2024-05-05 08:08:57.844210 roktools-6.3.0/roktools/orbit/__init__.py
--rw-r--r--   0        0        0     1745 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/orbit/kepler.py
--rw-r--r--   0        0        0     5905 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/orbit/tle.py
--rw-r--r--   0        0        0        0 2024-05-05 08:08:57.848209 roktools-6.3.0/roktools/parsers/rtklib/__init__,py
--rw-r--r--   0        0        0     5459 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/parsers/rtklib/stats.py
--rw-r--r--   0        0        0    61432 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/rinex.py
--rwxr-xr-x   0        0        0     1084 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/stats.py
--rwxr-xr-x   0        0        0     1598 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/tensorial.py
--rw-r--r--   0        0        0    11178 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/time.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-05 09:15:25.194556 roktools-6.3.1/LICENSE
+-rw-r--r--   0        0        0     1665 2024-05-05 09:15:25.194556 roktools-6.3.1/README.md
+-rw-r--r--   0        0        0     1162 2024-05-05 09:15:25.194556 roktools-6.3.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/__init__.py
+-rw-r--r--   0        0        0     4509 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/cl.py
+-rw-r--r--   0        0        0      133 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/constants.py
+-rw-r--r--   0        0        0      491 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/decorator.py
+-rw-r--r--   0        0        0      933 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/file.py
+-rw-r--r--   0        0        0    33628 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/geodetic.py
+-rw-r--r--   0        0        0        0 2024-05-05 09:15:25.238555 roktools-6.3.1/roktools/gnss/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/gnss/edit.py
+-rw-r--r--   0        0        0     1644 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/gnss/observables.py
+-rw-r--r--   0        0        0     1244 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/gnss/residuals.py
+-rw-r--r--   0        0        0     9572 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/gnss/types.py
+-rw-r--r--   0        0        0     1479 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/logger.py
+-rw-r--r--   0        0        0        0 2024-05-05 09:15:25.242555 roktools-6.3.1/roktools/orbit/__init__.py
+-rw-r--r--   0        0        0     1745 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/orbit/kepler.py
+-rw-r--r--   0        0        0     5905 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/orbit/tle.py
+-rw-r--r--   0        0        0        0 2024-05-05 09:15:25.242555 roktools-6.3.1/roktools/parsers/rtklib/__init__,py
+-rw-r--r--   0        0        0     5459 2024-05-05 09:15:25.194556 roktools-6.3.1/roktools/parsers/rtklib/stats.py
+-rw-r--r--   0        0        0    61455 2024-05-05 09:15:25.198556 roktools-6.3.1/roktools/rinex.py
+-rwxr-xr-x   0        0        0     1084 2024-05-05 09:15:25.198556 roktools-6.3.1/roktools/stats.py
+-rwxr-xr-x   0        0        0     1598 2024-05-05 09:15:25.198556 roktools-6.3.1/roktools/tensorial.py
+-rw-r--r--   0        0        0    11178 2024-05-05 09:15:25.198556 roktools-6.3.1/roktools/time.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.3.1/PKG-INFO
```

### Comparing `roktools-6.3.0/LICENSE` & `roktools-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/README.md` & `roktools-6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/pyproject.toml` & `roktools-6.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roktools"
-version = "6.3.0"
+version = "6.3.1"
 description = "Package with utilities and tools for GNSS data processing"
 authors = ["Rokubun <info@rokubun.cat>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
```

### Comparing `roktools-6.3.0/roktools/cl.py` & `roktools-6.3.1/roktools/cl.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/file.py` & `roktools-6.3.1/roktools/file.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/geodetic.py` & `roktools-6.3.1/roktools/geodetic.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/gnss/edit.py` & `roktools-6.3.1/roktools/gnss/edit.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/gnss/observables.py` & `roktools-6.3.1/roktools/gnss/observables.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/gnss/residuals.py` & `roktools-6.3.1/roktools/gnss/residuals.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/gnss/types.py` & `roktools-6.3.1/roktools/gnss/types.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/logger.py` & `roktools-6.3.1/roktools/logger.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/orbit/kepler.py` & `roktools-6.3.1/roktools/orbit/kepler.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/orbit/tle.py` & `roktools-6.3.1/roktools/orbit/tle.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/parsers/rtklib/stats.py` & `roktools-6.3.1/roktools/parsers/rtklib/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/rinex.py` & `roktools-6.3.1/roktools/rinex.py`

 * *Files 0% similar despite different names*

```diff
@@ -862,29 +862,29 @@
     satH1: int
     tgd1: float
     tgd2: float
 
     tx_time_tow: float
     aodc: int
 
-    eph_type: EphType
+    eph_type: str
 
     def csv_fields(self) -> str:
         return f"{self.get_type().value},{_SAT_STR},{_EPOCH_STR},\
 {_CLK_BIAS_STR},{_CLK_DRIFT_STR},{_CLK_DRIFT_RATE_STR},\
 {_AODE_STR},{_CRS_STR},{_DELTAN_STR},{_M0_STR},\
 {_CUC_STR},{_E_STR},{_CUS_STR},{_SQRTA_STR},\
 {_TOE_BDT_TOW_STR},{_CIC_STR},{_OMEGA0_STR},{_CIS_STR},\
 {_I0_STR},{_CRC_STR},{_OMEGA_STR},{_OMEGA_DOT_STR},\
 {_IDOT_STR},{_TOE_BDT_WEEK_STR},\
 {_ACCURACY_STR},{_SATH1_STR},{_TGD1_STR},{_TGD2_STR},\
 {_TX_TIME_TOW_STR},{_AODC_STR}"
 
     def get_type(self) -> EphType:
-        return self.eph_type
+        return EphType.from_string(self.eph_type)
 
 
 @dataclass
 class BdsCnv1NavBlock(NavBlock):
     """
     BEIDOU Navigation message on Beidou-3 B1C signal
     """
@@ -1261,15 +1261,15 @@
                             clk_bias, clk_drift, clk_drift_rate,
                             int(aode), crs, deltan, M0,
                             cuc, e, cus, sqrtA,
                             toe_tow, cic, OMEGA0, cis,
                             i0, crc, omega, OMEGA_DOT,
                             idot, int(toe_week),
                             accuracy, int(satH1), tgd1, tgd2,
-                            tx_tm, aodc, eph_type)
+                            tx_tm, aodc, eph_type.value)
 
     def _to_BDS_CNV1(self) -> BdsCnv1NavBlock:
 
         sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
         adot, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
         cuc, e, cus, sqrtA = _parse_nav_orb_line(self.lines[3])
         toe_tow, cic, OMEGA0, cis = _parse_nav_orb_line(self.lines[4])
```

### Comparing `roktools-6.3.0/roktools/stats.py` & `roktools-6.3.1/roktools/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/tensorial.py` & `roktools-6.3.1/roktools/tensorial.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/roktools/time.py` & `roktools-6.3.1/roktools/time.py`

 * *Files identical despite different names*

### Comparing `roktools-6.3.0/PKG-INFO` & `roktools-6.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 6.3.0
+Version: 6.3.1
 Summary: Package with utilities and tools for GNSS data processing
 Author: Rokubun
 Author-email: info@rokubun.cat
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

