# Comparing `tmp/annonition-0.0.6.tar.gz` & `tmp/annonition-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annonition-0.0.6.tar", last modified: Mon May 13 03:14:29 2024, max compression
+gzip compressed data, was "annonition-0.0.7.tar", last modified: Fri May 17 15:17:48 2024, max compression
```

## Comparing `annonition-0.0.6.tar` & `annonition-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 03:14:28.820000 annonition-0.0.6/
--rw-rw-rw-   0        0        0      452 2024-05-13 03:14:30.000000 annonition-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-05-07 21:46:06.000000 annonition-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 03:14:28.850000 annonition-0.0.6/annonition/
--rw-rw-rw-   0        0        0       77 2024-05-12 22:40:06.000000 annonition-0.0.6/annonition/__init__.py
--rw-rw-rw-   0        0        0     4795 2024-05-13 03:02:46.000000 annonition-0.0.6/annonition/logger.py
--rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.0.6/annonition/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 03:14:28.870000 annonition-0.0.6/annonition.egg-info/
--rw-rw-rw-   0        0        0      452 2024-05-13 03:14:30.000000 annonition-0.0.6/annonition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-13 03:14:30.000000 annonition-0.0.6/annonition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 03:14:30.000000 annonition-0.0.6/annonition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-13 03:14:30.000000 annonition-0.0.6/annonition.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 03:14:30.000000 annonition-0.0.6/annonition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 03:14:30.000000 annonition-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      843 2024-05-13 03:14:00.000000 annonition-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:17:48.520000 annonition-0.0.7/
+-rw-rw-rw-   0        0        0      452 2024-05-17 15:17:50.000000 annonition-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-05-07 21:46:06.000000 annonition-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 15:17:48.540000 annonition-0.0.7/annonition/
+-rw-rw-rw-   0        0        0       77 2024-05-12 22:40:06.000000 annonition-0.0.7/annonition/__init__.py
+-rw-rw-rw-   0        0        0     4796 2024-05-17 15:13:50.000000 annonition-0.0.7/annonition/logger.py
+-rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.0.7/annonition/main.py
+-rw-rw-rw-   0        0        0      930 2024-05-17 15:16:14.000000 annonition-0.0.7/annonition/t.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:17:48.560000 annonition-0.0.7/annonition.egg-info/
+-rw-rw-rw-   0        0        0      452 2024-05-17 15:17:50.000000 annonition-0.0.7/annonition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-17 15:17:50.000000 annonition-0.0.7/annonition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:17:50.000000 annonition-0.0.7/annonition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-17 15:17:50.000000 annonition-0.0.7/annonition.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 15:17:50.000000 annonition-0.0.7/annonition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:17:50.000000 annonition-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      843 2024-05-17 15:17:22.000000 annonition-0.0.7/setup.py
```

### Comparing `annonition-0.0.6/annonition/logger.py` & `annonition-0.0.7/annonition/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,104 +197,104 @@
 00000c40: 2020 2020 6465 6620 5f5f 6e65 775f 5f28      def __new__(
 00000c50: 636c 732c 206c 6576 656c 3d22 494e 464f  cls, level="INFO
 00000c60: 222c 206e 616d 653d 2777 6572 6b7a 6575  ", name='werkzeu
 00000c70: 6727 2c20 6967 6e6f 7265 3d4e 6f6e 652c  g', ignore=None,
 00000c80: 2069 6e63 6c75 6465 5f64 6174 653d 5472   include_date=Tr
 00000c90: 7565 2c20 696e 636c 7564 655f 6c65 7665  ue, include_leve
 00000ca0: 6c3d 5472 7565 2c20 6461 7465 5f63 6f6c  l=True, date_col
-00000cb0: 6f72 3d27 626c 6163 6b27 293a 0d0a 2020  or='black'):..  
-00000cc0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00000cd0: 2020 2043 7265 6174 6573 2061 6e64 2072     Creates and r
-00000ce0: 6574 7572 6e73 2061 206e 6577 206c 6f67  eturns a new log
-00000cf0: 6765 7220 696e 7374 616e 6365 2077 6974  ger instance wit
-00000d00: 6820 7370 6563 6966 6965 6420 636f 6e66  h specified conf
-00000d10: 6967 7572 6174 696f 6e73 2e0d 0a0d 0a20  igurations..... 
-00000d20: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00000d30: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000d40: 6e61 6d65 2028 7374 7229 3a20 5468 6520  name (str): The 
-00000d50: 6e61 6d65 206f 6620 7468 6520 6c6f 6767  name of the logg
-00000d60: 6572 2e20 4465 6661 756c 7420 6973 2027  er. Default is '
-00000d70: 7765 726b 7a65 7567 272e 0d0a 2020 2020  werkzeug'...    
-00000d80: 2020 2020 2020 2020 6967 6e6f 7265 2028          ignore (
-00000d90: 6c69 7374 206f 6620 7374 722c 206f 7074  list of str, opt
-00000da0: 696f 6e61 6c29 3a20 4120 6c69 7374 206f  ional): A list o
-00000db0: 6620 6d65 7373 6167 6520 7375 6273 7472  f message substr
-00000dc0: 696e 6773 2074 6f20 6967 6e6f 7265 2069  ings to ignore i
-00000dd0: 6e20 7468 6520 6c6f 6773 2e0d 0a20 2020  n the logs...   
-00000de0: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-00000df0: 5f64 6174 6520 2862 6f6f 6c2c 206f 7074  _date (bool, opt
-00000e00: 696f 6e61 6c29 3a20 5768 6574 6865 7220  ional): Whether 
-00000e10: 746f 2069 6e63 6c75 6465 2074 6865 2064  to include the d
-00000e20: 6174 6520 696e 2074 6865 206c 6f67 206d  ate in the log m
-00000e30: 6573 7361 6765 732e 2044 6566 6175 6c74  essages. Default
-00000e40: 2069 7320 5472 7565 2e0d 0a20 2020 2020   is True...     
-00000e50: 2020 2020 2020 2069 6e63 6c75 6465 5f6c         include_l
-00000e60: 6576 656c 2028 626f 6f6c 2c20 6f70 7469  evel (bool, opti
-00000e70: 6f6e 616c 293a 2057 6865 7468 6572 2074  onal): Whether t
-00000e80: 6f20 696e 636c 7564 6520 7468 6520 6c6f  o include the lo
-00000e90: 6720 6c65 7665 6c20 696e 2074 6865 206c  g level in the l
-00000ea0: 6f67 206d 6573 7361 6765 732e 2044 6566  og messages. Def
-00000eb0: 6175 6c74 2069 7320 5472 7565 2e0d 0a0d  ault is True....
-00000ec0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00000ed0: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
-00000ee0: 6f67 6769 6e67 2e4c 6f67 6765 723a 2041  ogging.Logger: A
-00000ef0: 2063 6f6e 6669 6775 7265 6420 6c6f 6767   configured logg
-00000f00: 6572 2069 6e73 7461 6e63 6520 7769 7468  er instance with
-00000f10: 2063 6f6c 6f72 6564 206c 6f67 7320 616e   colored logs an
-00000f20: 6420 656e 6470 6f69 6e74 2066 696c 7465  d endpoint filte
-00000f30: 7269 6e67 2e0d 0a20 2020 2020 2020 2022  ring...        "
-00000f40: 2222 0d0a 2020 2020 2020 2020 6966 2069  ""..        if i
-00000f50: 676e 6f72 6520 6973 204e 6f6e 653a 0d0a  gnore is None:..
-00000f60: 2020 2020 2020 2020 2020 2020 6967 6e6f              igno
-00000f70: 7265 203d 205b 5d0d 0a20 2020 2020 2020  re = []..       
-00000f80: 2076 6572 626f 7365 6c6f 6773 2e69 6e73   verboselogs.ins
-00000f90: 7461 6c6c 2829 0d0a 2020 2020 2020 2020  tall()..        
-00000fa0: 6c6f 6767 696e 672e 5645 5242 4f53 4520  logging.VERBOSE 
-00000fb0: 3d20 7665 7262 6f73 656c 6f67 732e 5645  = verboselogs.VE
-00000fc0: 5242 4f53 450d 0a20 2020 2020 2020 206c  RBOSE..        l
-00000fd0: 6f67 6769 6e67 2e53 5041 4d20 3d20 7665  ogging.SPAM = ve
-00000fe0: 7262 6f73 656c 6f67 732e 5350 414d 0d0a  rboselogs.SPAM..
-00000ff0: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00001000: 4e4f 5449 4345 203d 2076 6572 626f 7365  NOTICE = verbose
-00001010: 6c6f 6773 2e4e 4f54 4943 450d 0a20 2020  logs.NOTICE..   
-00001020: 2020 2020 206c 6f67 6769 6e67 2e53 5543       logging.SUC
-00001030: 4345 5353 203d 2076 6572 626f 7365 6c6f  CESS = verboselo
-00001040: 6773 2e53 5543 4345 5353 0d0a 0d0a 2020  gs.SUCCESS....  
-00001050: 2020 2020 2020 6c6f 6767 6572 203d 206c        logger = l
-00001060: 6f67 6769 6e67 2e67 6574 4c6f 6767 6572  ogging.getLogger
-00001070: 286e 616d 6529 0d0a 2020 2020 2020 2020  (name)..        
-00001080: 6c6f 6767 6572 2e61 6464 4669 6c74 6572  logger.addFilter
-00001090: 2845 6e64 706f 696e 7446 696c 7465 7228  (EndpointFilter(
-000010a0: 6967 6e6f 7265 2929 0d0a 0d0a 2020 2020  ignore))....    
-000010b0: 2020 2020 666f 726d 6174 5f65 6c65 6d65      format_eleme
-000010c0: 6e74 7320 3d20 5b5d 0d0a 2020 2020 2020  nts = []..      
-000010d0: 2020 6966 2069 6e63 6c75 6465 5f64 6174    if include_dat
-000010e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000010f0: 666f 726d 6174 5f65 6c65 6d65 6e74 732e  format_elements.
-00001100: 6170 7065 6e64 2827 2528 6173 6374 696d  append('%(asctim
-00001110: 6529 7327 290d 0a20 2020 2020 2020 2069  e)s')..        i
-00001120: 6620 696e 636c 7564 655f 6c65 7665 6c3a  f include_level:
-00001130: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00001140: 726d 6174 5f65 6c65 6d65 6e74 732e 6170  rmat_elements.ap
-00001150: 7065 6e64 2827 2528 6c65 7665 6c6e 616d  pend('%(levelnam
-00001160: 6529 7327 290d 0a20 2020 2020 2020 2066  e)s')..        f
-00001170: 6f72 6d61 745f 656c 656d 656e 7473 2e61  ormat_elements.a
-00001180: 7070 656e 6428 2725 286d 6573 7361 6765  ppend('%(message
-00001190: 2973 2729 0d0a 2020 2020 2020 2020 6c6f  )s')..        lo
-000011a0: 675f 666f 726d 6174 203d 2027 2027 2e6a  g_format = ' '.j
-000011b0: 6f69 6e28 666f 726d 6174 5f65 6c65 6d65  oin(format_eleme
-000011c0: 6e74 7329 0d0a 2020 2020 2020 2020 6669  nts)..        fi
-000011d0: 656c 645f 7374 796c 6573 203d 207b 2761  eld_styles = {'a
-000011e0: 7363 7469 6d65 273a 207b 2763 6f6c 6f72  sctime': {'color
-000011f0: 273a 2064 6174 655f 636f 6c6f 722c 2027  ': date_color, '
-00001200: 626f 6c64 273a 2046 616c 7365 7d7d 0d0a  bold': False}}..
-00001210: 0d0a 2020 2020 2020 2020 636f 6c6f 7265  ..        colore
-00001220: 646c 6f67 732e 696e 7374 616c 6c28 6c6f  dlogs.install(lo
-00001230: 6767 6572 3d6c 6f67 6765 722c 2069 7361  gger=logger, isa
-00001240: 7474 793d 5472 7565 2c20 666d 743d 6c6f  tty=True, fmt=lo
-00001250: 675f 666f 726d 6174 2c20 6c65 7665 6c3d  g_format, level=
-00001260: 6c65 7665 6c2e 7570 7065 7228 292c 2066  level.upper(), f
-00001270: 6965 6c64 5f73 7479 6c65 733d 6669 656c  ield_styles=fiel
-00001280: 645f 7374 796c 6573 290d 0a20 2020 2020  d_styles)..     
-00001290: 2020 2072 6574 7572 6e20 4175 746f 466f     return AutoFo
-000012a0: 726d 6174 4164 6170 7465 7228 6c6f 6767  rmatAdapter(logg
-000012b0: 6572 290d 0a20 2020 200d 0a              er)..    ..
+00000cb0: 6f72 3d27 7965 6c6c 6f77 2729 3a0d 0a20  or='yellow'):.. 
+00000cc0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00000cd0: 2020 2020 4372 6561 7465 7320 616e 6420      Creates and 
+00000ce0: 7265 7475 726e 7320 6120 6e65 7720 6c6f  returns a new lo
+00000cf0: 6767 6572 2069 6e73 7461 6e63 6520 7769  gger instance wi
+00000d00: 7468 2073 7065 6369 6669 6564 2063 6f6e  th specified con
+00000d10: 6669 6775 7261 7469 6f6e 732e 0d0a 0d0a  figurations.....
+00000d20: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00000d30: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
+00000d40: 206e 616d 6520 2873 7472 293a 2054 6865   name (str): The
+00000d50: 206e 616d 6520 6f66 2074 6865 206c 6f67   name of the log
+00000d60: 6765 722e 2044 6566 6175 6c74 2069 7320  ger. Default is 
+00000d70: 2777 6572 6b7a 6575 6727 2e0d 0a20 2020  'werkzeug'...   
+00000d80: 2020 2020 2020 2020 2069 676e 6f72 6520           ignore 
+00000d90: 286c 6973 7420 6f66 2073 7472 2c20 6f70  (list of str, op
+00000da0: 7469 6f6e 616c 293a 2041 206c 6973 7420  tional): A list 
+00000db0: 6f66 206d 6573 7361 6765 2073 7562 7374  of message subst
+00000dc0: 7269 6e67 7320 746f 2069 676e 6f72 6520  rings to ignore 
+00000dd0: 696e 2074 6865 206c 6f67 732e 0d0a 2020  in the logs...  
+00000de0: 2020 2020 2020 2020 2020 696e 636c 7564            includ
+00000df0: 655f 6461 7465 2028 626f 6f6c 2c20 6f70  e_date (bool, op
+00000e00: 7469 6f6e 616c 293a 2057 6865 7468 6572  tional): Whether
+00000e10: 2074 6f20 696e 636c 7564 6520 7468 6520   to include the 
+00000e20: 6461 7465 2069 6e20 7468 6520 6c6f 6720  date in the log 
+00000e30: 6d65 7373 6167 6573 2e20 4465 6661 756c  messages. Defaul
+00000e40: 7420 6973 2054 7275 652e 0d0a 2020 2020  t is True...    
+00000e50: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+00000e60: 6c65 7665 6c20 2862 6f6f 6c2c 206f 7074  level (bool, opt
+00000e70: 696f 6e61 6c29 3a20 5768 6574 6865 7220  ional): Whether 
+00000e80: 746f 2069 6e63 6c75 6465 2074 6865 206c  to include the l
+00000e90: 6f67 206c 6576 656c 2069 6e20 7468 6520  og level in the 
+00000ea0: 6c6f 6720 6d65 7373 6167 6573 2e20 4465  log messages. De
+00000eb0: 6661 756c 7420 6973 2054 7275 652e 0d0a  fault is True...
+00000ec0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00000ed0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00000ee0: 6c6f 6767 696e 672e 4c6f 6767 6572 3a20  logging.Logger: 
+00000ef0: 4120 636f 6e66 6967 7572 6564 206c 6f67  A configured log
+00000f00: 6765 7220 696e 7374 616e 6365 2077 6974  ger instance wit
+00000f10: 6820 636f 6c6f 7265 6420 6c6f 6773 2061  h colored logs a
+00000f20: 6e64 2065 6e64 706f 696e 7420 6669 6c74  nd endpoint filt
+00000f30: 6572 696e 672e 0d0a 2020 2020 2020 2020  ering...        
+00000f40: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+00000f50: 6967 6e6f 7265 2069 7320 4e6f 6e65 3a0d  ignore is None:.
+00000f60: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
+00000f70: 6f72 6520 3d20 5b5d 0d0a 2020 2020 2020  ore = []..      
+00000f80: 2020 7665 7262 6f73 656c 6f67 732e 696e    verboselogs.in
+00000f90: 7374 616c 6c28 290d 0a20 2020 2020 2020  stall()..       
+00000fa0: 206c 6f67 6769 6e67 2e56 4552 424f 5345   logging.VERBOSE
+00000fb0: 203d 2076 6572 626f 7365 6c6f 6773 2e56   = verboselogs.V
+00000fc0: 4552 424f 5345 0d0a 2020 2020 2020 2020  ERBOSE..        
+00000fd0: 6c6f 6767 696e 672e 5350 414d 203d 2076  logging.SPAM = v
+00000fe0: 6572 626f 7365 6c6f 6773 2e53 5041 4d0d  erboselogs.SPAM.
+00000ff0: 0a20 2020 2020 2020 206c 6f67 6769 6e67  .        logging
+00001000: 2e4e 4f54 4943 4520 3d20 7665 7262 6f73  .NOTICE = verbos
+00001010: 656c 6f67 732e 4e4f 5449 4345 0d0a 2020  elogs.NOTICE..  
+00001020: 2020 2020 2020 6c6f 6767 696e 672e 5355        logging.SU
+00001030: 4343 4553 5320 3d20 7665 7262 6f73 656c  CCESS = verbosel
+00001040: 6f67 732e 5355 4343 4553 530d 0a0d 0a20  ogs.SUCCESS.... 
+00001050: 2020 2020 2020 206c 6f67 6765 7220 3d20         logger = 
+00001060: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
+00001070: 7228 6e61 6d65 290d 0a20 2020 2020 2020  r(name)..       
+00001080: 206c 6f67 6765 722e 6164 6446 696c 7465   logger.addFilte
+00001090: 7228 456e 6470 6f69 6e74 4669 6c74 6572  r(EndpointFilter
+000010a0: 2869 676e 6f72 6529 290d 0a0d 0a20 2020  (ignore))....   
+000010b0: 2020 2020 2066 6f72 6d61 745f 656c 656d       format_elem
+000010c0: 656e 7473 203d 205b 5d0d 0a20 2020 2020  ents = []..     
+000010d0: 2020 2069 6620 696e 636c 7564 655f 6461     if include_da
+000010e0: 7465 3a0d 0a20 2020 2020 2020 2020 2020  te:..           
+000010f0: 2066 6f72 6d61 745f 656c 656d 656e 7473   format_elements
+00001100: 2e61 7070 656e 6428 2725 2861 7363 7469  .append('%(ascti
+00001110: 6d65 2973 2729 0d0a 2020 2020 2020 2020  me)s')..        
+00001120: 6966 2069 6e63 6c75 6465 5f6c 6576 656c  if include_level
+00001130: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+00001140: 6f72 6d61 745f 656c 656d 656e 7473 2e61  ormat_elements.a
+00001150: 7070 656e 6428 2725 286c 6576 656c 6e61  ppend('%(levelna
+00001160: 6d65 2973 2729 0d0a 2020 2020 2020 2020  me)s')..        
+00001170: 666f 726d 6174 5f65 6c65 6d65 6e74 732e  format_elements.
+00001180: 6170 7065 6e64 2827 2528 6d65 7373 6167  append('%(messag
+00001190: 6529 7327 290d 0a20 2020 2020 2020 206c  e)s')..        l
+000011a0: 6f67 5f66 6f72 6d61 7420 3d20 2720 272e  og_format = ' '.
+000011b0: 6a6f 696e 2866 6f72 6d61 745f 656c 656d  join(format_elem
+000011c0: 656e 7473 290d 0a20 2020 2020 2020 2066  ents)..        f
+000011d0: 6965 6c64 5f73 7479 6c65 7320 3d20 7b27  ield_styles = {'
+000011e0: 6173 6374 696d 6527 3a20 7b27 636f 6c6f  asctime': {'colo
+000011f0: 7227 3a20 6461 7465 5f63 6f6c 6f72 2c20  r': date_color, 
+00001200: 2762 6f6c 6427 3a20 4661 6c73 657d 7d0d  'bold': False}}.
+00001210: 0a0d 0a20 2020 2020 2020 2063 6f6c 6f72  ...        color
+00001220: 6564 6c6f 6773 2e69 6e73 7461 6c6c 286c  edlogs.install(l
+00001230: 6f67 6765 723d 6c6f 6767 6572 2c20 6973  ogger=logger, is
+00001240: 6174 7479 3d54 7275 652c 2066 6d74 3d6c  atty=True, fmt=l
+00001250: 6f67 5f66 6f72 6d61 742c 206c 6576 656c  og_format, level
+00001260: 3d6c 6576 656c 2e75 7070 6572 2829 2c20  =level.upper(), 
+00001270: 6669 656c 645f 7374 796c 6573 3d66 6965  field_styles=fie
+00001280: 6c64 5f73 7479 6c65 7329 0d0a 2020 2020  ld_styles)..    
+00001290: 2020 2020 7265 7475 726e 2041 7574 6f46      return AutoF
+000012a0: 6f72 6d61 7441 6461 7074 6572 286c 6f67  ormatAdapter(log
+000012b0: 6765 7229 0d0a 2020 2020 0d0a            ger)..    ..
```

### Comparing `annonition-0.0.6/setup.py` & `annonition-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(path.join(working_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="annonition",
-    version="0.0.6",
+    version="0.0.7",
     author="Abtin Turing",
     author_email="abtinturing@gmail.com",
     description="Beginning of a new era in annotation tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/abtinturing/anno",
     packages=find_packages(),
```

