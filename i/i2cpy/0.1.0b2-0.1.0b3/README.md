# Comparing `tmp/i2cpy-0.1.0b2.tar.gz` & `tmp/i2cpy-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2cpy-0.1.0b2.tar", last modified: Sun May 12 16:07:23 2024, max compression
+gzip compressed data, was "i2cpy-0.1.0b3.tar", last modified: Fri May 17 15:21:40 2024, max compression
```

## Comparing `i2cpy-0.1.0b2.tar` & `i2cpy-0.1.0b3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:07:23.949988 i2cpy-0.1.0b2/
--rw-rw-rw-   0        0        0     1073 2024-05-05 19:00:07.000000 i2cpy-0.1.0b2/LICENSE
--rw-rw-rw-   0        0        0     8855 2024-05-12 16:07:23.948989 i2cpy-0.1.0b2/PKG-INFO
--rw-rw-rw-   0        0        0     6994 2024-05-12 16:06:59.000000 i2cpy-0.1.0b2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 16:07:23.916955 i2cpy-0.1.0b2/i2cpy/
--rw-rw-rw-   0        0        0     6706 2024-05-12 16:06:21.000000 i2cpy-0.1.0b2/i2cpy/__init__.py
--rw-rw-rw-   0        0        0       23 2024-05-12 16:06:41.000000 i2cpy-0.1.0b2/i2cpy/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:07:23.933470 i2cpy-0.1.0b2/i2cpy/driver/
--rw-rw-rw-   0        0        0     3232 2024-05-12 06:54:49.000000 i2cpy-0.1.0b2/i2cpy/driver/abc.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:07:23.940981 i2cpy-0.1.0b2/i2cpy/driver/ch341/
--rw-rw-rw-   0        0        0     6836 2024-05-12 14:58:02.000000 i2cpy-0.1.0b2/i2cpy/driver/ch341/__init__.py
--rw-rw-rw-   0        0        0      278 2024-05-05 19:11:06.000000 i2cpy-0.1.0b2/i2cpy/driver/ch341/constants.py
--rw-rw-rw-   0        0        0     1257 2024-05-12 14:58:02.000000 i2cpy-0.1.0b2/i2cpy/driver/ch341/dll.py
--rw-rw-rw-   0        0        0      379 2024-05-07 14:09:07.000000 i2cpy-0.1.0b2/i2cpy/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:07:23.946989 i2cpy-0.1.0b2/i2cpy.egg-info/
--rw-rw-rw-   0        0        0     8855 2024-05-12 16:07:23.000000 i2cpy-0.1.0b2/i2cpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-05-12 16:07:23.000000 i2cpy-0.1.0b2/i2cpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:07:23.000000 i2cpy-0.1.0b2/i2cpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-12 16:07:23.000000 i2cpy-0.1.0b2/i2cpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-12 16:07:23.000000 i2cpy-0.1.0b2/i2cpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2024-05-12 16:04:55.000000 i2cpy-0.1.0b2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 16:07:23.950988 i2cpy-0.1.0b2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-12 16:07:23.943987 i2cpy-0.1.0b2/tests/
--rw-rw-rw-   0        0        0      802 2024-05-12 14:58:02.000000 i2cpy-0.1.0b2/tests/test_i2c.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.317047 i2cpy-0.1.0b3/
+-rw-rw-rw-   0        0        0     1073 2024-05-05 19:00:07.000000 i2cpy-0.1.0b3/LICENSE
+-rw-rw-rw-   0        0        0     8748 2024-05-17 15:21:40.315097 i2cpy-0.1.0b3/PKG-INFO
+-rw-rw-rw-   0        0        0     6887 2024-05-17 15:19:17.000000 i2cpy-0.1.0b3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.256155 i2cpy-0.1.0b3/i2cpy/
+-rw-rw-rw-   0        0        0     6642 2024-05-17 15:18:17.000000 i2cpy-0.1.0b3/i2cpy/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-17 15:21:16.000000 i2cpy-0.1.0b3/i2cpy/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.284153 i2cpy-0.1.0b3/i2cpy/driver/
+-rw-rw-rw-   0        0        0     3734 2024-05-13 11:28:11.000000 i2cpy-0.1.0b3/i2cpy/driver/abc.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.299374 i2cpy-0.1.0b3/i2cpy/driver/ch341/
+-rw-rw-rw-   0        0        0     6347 2024-05-17 15:18:17.000000 i2cpy-0.1.0b3/i2cpy/driver/ch341/__init__.py
+-rw-rw-rw-   0        0        0      278 2024-05-05 19:11:06.000000 i2cpy-0.1.0b3/i2cpy/driver/ch341/constants.py
+-rw-rw-rw-   0        0        0     1282 2024-05-17 15:10:31.000000 i2cpy-0.1.0b3/i2cpy/driver/ch341/dll.py
+-rw-rw-rw-   0        0        0      807 2024-05-17 15:18:17.000000 i2cpy-0.1.0b3/i2cpy/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.313135 i2cpy-0.1.0b3/i2cpy.egg-info/
+-rw-rw-rw-   0        0        0     8748 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2024-05-13 10:18:51.000000 i2cpy-0.1.0b3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:21:40.318026 i2cpy-0.1.0b3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.306255 i2cpy-0.1.0b3/tests/
+-rw-rw-rw-   0        0        0      802 2024-05-12 14:58:02.000000 i2cpy-0.1.0b3/tests/test_i2c.py
+-rw-rw-rw-   0        0        0      792 2024-05-13 10:18:51.000000 i2cpy-0.1.0b3/tests/test_utils.py
```

### Comparing `i2cpy-0.1.0b2/LICENSE` & `i2cpy-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `i2cpy-0.1.0b2/PKG-INFO` & `i2cpy-0.1.0b3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cpy
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Python I2C library supporting multiple driver implementations
 Author-email: Zhenyi Zhou <iynehz@163.com>
 License: Copyright (c) 2024 Zhenyi Zhou
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -34,22 +34,18 @@
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.6.0; python_version < "3.12"
 
 # Python I2C library supporting multiple driver implementations
 
 <div>
    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python"/>
-   <a href="https://pypi.org/project/i2cpy/">
-      <img src="https://img.shields.io/pypi/v/i2cpy.svg" alt="pypi"/>
-   </a>
-   <a href="https://github.com/iynehz/i2cpy/blob/main/LICENSE">
-      <img src="https://img.shields.io/badge/license-MIT-green" alt="license"/>
-   </a>
-   <img src="https://img.shields.io/badge/code%20style-black-black.svg" alt="Code style: black"/>
-   <img src="https://img.shields.io/badge/mypy-checked-green.svg" alt="mypy"/>
+   <a href="https://pypi.org/project/i2cpy/"><img src="https://img.shields.io/pypi/v/i2cpy.svg" alt="pypi"/></a>
+   <a href="https://github.com/iynehz/i2cpy/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-green" alt="license"/></a>
+   <img src="https://readthedocs.org/projects/i2cpy/badge/?version=latest" alt="docs"/>
+   <img src="https://github.com/iynehz/i2cpy/actions/workflows/lint.yml/badge.svg" alt="lint"/>
 </div>
 
 ## Introduction
 
 I2C is a two-wire protocol for communicating between devices. At the
 physical level it consists of 2 wires: SCL and SDA, the clock and data lines
 respectively.
@@ -77,15 +73,15 @@
                                  #   starting at memory address 2 in the peripheral
 ```
 
 ## Class I2C
 
 ### Constructor
 
-#### I2C.\_\_init_\_(\*, id=None, driver=None, freq=400000, auto_init=True, \*\*kwargs)
+#### I2C.\_\_init_\_(id=None, \*, driver=None, freq=400000, auto_init=True, \*\*kwargs)
 
 Constructor.
 
 * **Parameters:**
   * **id** (`Union`[`int`, `str`, `None`]) – Identifies a particular I2C peripheral. Allowed values depend
     on the particular driver implementation.
   * **freq** (`int`) – I2C bus baudrate, defaults to 400000
@@ -124,66 +120,66 @@
 ### Standard bus operations
 
 #### I2C.writeto(addr, buf, /)
 
 Write the bytes from buf to the peripheral specified by addr.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral deivce address
+  * **addr** (`int`) – I2C peripheral deivce address
   * **buf** (`Buffer`) – bytes to write
 
 #### I2C.readfrom(addr, nbytes, /)
 
 Read nbytes from the peripheral specified by addr.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
+  * **addr** (`int`) – I2C peripheral device address
   * **nbytes** (`int`) – number of bytes to read
 * **Return type:**
   `bytes`
 * **Returns:**
   the bytes read
 
 ### Memory operations
 
 #### I2C.writeto_mem(addr, memaddr, buf, \*, addrsize=8)
 
 Write buf to the peripheral specified by addr starting from the
 memory address specified by memaddr.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
-  * **memaddr** (`int` | `Buffer`) – memory address
+  * **addr** (`int`) – I2C peripheral device address
+  * **memaddr** (`int`) – memory address
   * **buf** (`Buffer`) – bytes to write
   * **addrsize** (`int`) – \_description_, defaults to 8
 
 #### I2C.readfrom_mem(addr, memaddr, nbytes, \*, addrsize=8)
 
 Read *nbytes* from the peripheral specified by *addr* starting from
 the memory address specified by *memaddr*.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
-  * **memaddr** (`int` | `Buffer`) – memory address
+  * **addr** (`int`) – I2C peripheral device address
+  * **memaddr** (`int`) – memory address
   * **nbytes** (`int`) – number of bytes to read
   * **addrsize** (`int`) – \_description_, defaults to 8
 * **Return type:**
   `bytes`
 * **Returns:**
   the bytes read
 
 #### I2C.readfrom_mem_into(addr, memaddr, buf, \*, addrsize=8)
 
 Read into buf from the peripheral specified by addr starting from the
 memory address specified by memaddr. The number of bytes read is the
 length of buf.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
-  * **memaddr** (`int` | `Buffer`) – memory address
+  * **addr** (`int`) – I2C peripheral device address
+  * **memaddr** (`int`) – memory address
   * **buf** (`bytearray`) – buffer to store the bytes read
   * **addrsize** (`int`) – \_description_, defaults to 8
 
 ## Supported I2C drivers
 
 ### ch341
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: i2cpy Version: 0.1.0b2 Summary: Python I2C library
+Metadata-Version: 2.1 Name: i2cpy Version: 0.1.0b3 Summary: Python I2C library
 supporting multiple driver implementations Author-email: Zhenyi Zhou
 163.com> License: Copyright (c) 2024 Zhenyi Zhou Permission is hereby granted,
 free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
@@ -17,29 +17,29 @@
 Project-URL: Homepage, https://github.com/iynehz/i2cpy Project-URL:
 Documentation, https://i2cpy.readthedocs.io/en/latest/ Project-URL: Repository,
 https://github.com/iynehz/i2cpy Keywords: i2c,ch341,ch341a Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: typing_extensions>=4.6.0; python_version < "3.12" #
 Python I2C library supporting multiple driver implementations
-[python]_[_p_y_p_i_]_[_l_i_c_e_n_s_e_][Code style: black][mypy]
+[python]_[_p_y_p_i_]_[_l_i_c_e_n_s_e_][docs][lint]
 ## Introduction I2C is a two-wire protocol for communicating between devices.
 At the physical level it consists of 2 wires: SCL and SDA, the clock and data
 lines respectively. I2C objects are created attached to a specific bus. They
 can be initialized when created, or initialized later on. This library is
 designed to support different I2C driver implementations. Itâs interface is
 similar to MicroPythonâs `machine.I2C` as well as CircuitPythonâs
 `board.I2C` classes. Example usage: ```python from i2cpy import I2C i2c = I2C()
 # create I2C peripheral i2c.writeto(42, b'123') # write 3 bytes to peripheral
 with 7-bit address 42 i2c.readfrom(42, 4) # read 4 bytes from peripheral with
 7-bit address 42 i2c.readfrom_mem(42, 8, 3) # read 3 bytes from memory of
 peripheral 42, # starting at memory address 8 in the peripheral i2c.writeto_mem
 (42, 2, b'\x10') # write 1 byte to memory of peripheral 42, # starting at
 memory address 2 in the peripheral ``` ## Class I2C ### Constructor ####
-I2C.\_\_init_\_(\*, id=None, driver=None, freq=400000, auto_init=True,
+I2C.\_\_init_\_(id=None, \*, driver=None, freq=400000, auto_init=True,
 \*\*kwargs) Constructor. * **Parameters:** * **id** (`Union`[`int`, `str`,
 `None`]) â Identifies a particular I2C peripheral. Allowed values depend on
 the particular driver implementation. * **freq** (`int`) â I2C bus baudrate,
 defaults to 400000 * **driver** (`Optional`[`str`]) â I2C driver name. It
 corresponds to the I2C driver sub module name shipped with this library. For
 example âfooâ means module âi2cpy.driver.fooâ. If not specified, it
 looks at environment variable âI2CPY_DRIVERâ. And if thatâs not defined
@@ -49,36 +49,35 @@
 I2C.scan(start=8, stop=119) Scan all I2C addresses between start and stop
 inclusive and return a list of those that respond. A device responds if it
 pulls the SDA line low after its address (including a write bit) is sent on the
 bus. * **Parameters:** * **start** (`int`) â start address, defaults to 0x08
 * **stop** (`int`) â stop address, defaults to 0x77 * **Return type:** `List`
 [`int`] * **Returns:** a list of addresses that respond to scan ### Standard
 bus operations #### I2C.writeto(addr, buf, /) Write the bytes from buf to the
-peripheral specified by addr. * **Parameters:** * **addr** (`int` | `Buffer`)
-â I2C peripheral deivce address * **buf** (`Buffer`) â bytes to write ####
+peripheral specified by addr. * **Parameters:** * **addr** (`int`) â I2C
+peripheral deivce address * **buf** (`Buffer`) â bytes to write ####
 I2C.readfrom(addr, nbytes, /) Read nbytes from the peripheral specified by
-addr. * **Parameters:** * **addr** (`int` | `Buffer`) â I2C peripheral device
-address * **nbytes** (`int`) â number of bytes to read * **Return type:**
-`bytes` * **Returns:** the bytes read ### Memory operations ####
-I2C.writeto_mem(addr, memaddr, buf, \*, addrsize=8) Write buf to the peripheral
-specified by addr starting from the memory address specified by memaddr. *
-**Parameters:** * **addr** (`int` | `Buffer`) â I2C peripheral device address
-* **memaddr** (`int` | `Buffer`) â memory address * **buf** (`Buffer`) â
-bytes to write * **addrsize** (`int`) â \_description_, defaults to 8 ####
-I2C.readfrom_mem(addr, memaddr, nbytes, \*, addrsize=8) Read *nbytes* from the
-peripheral specified by *addr* starting from the memory address specified by
-*memaddr*. * **Parameters:** * **addr** (`int` | `Buffer`) â I2C peripheral
-device address * **memaddr** (`int` | `Buffer`) â memory address * **nbytes**
-(`int`) â number of bytes to read * **addrsize** (`int`) â \_description_,
-defaults to 8 * **Return type:** `bytes` * **Returns:** the bytes read ####
-I2C.readfrom_mem_into(addr, memaddr, buf, \*, addrsize=8) Read into buf from
-the peripheral specified by addr starting from the memory address specified by
-memaddr. The number of bytes read is the length of buf. * **Parameters:** *
-**addr** (`int` | `Buffer`) â I2C peripheral device address * **memaddr**
-(`int` | `Buffer`) â memory address * **buf** (`bytearray`) â buffer to
+addr. * **Parameters:** * **addr** (`int`) â I2C peripheral device address *
+**nbytes** (`int`) â number of bytes to read * **Return type:** `bytes` *
+**Returns:** the bytes read ### Memory operations #### I2C.writeto_mem(addr,
+memaddr, buf, \*, addrsize=8) Write buf to the peripheral specified by addr
+starting from the memory address specified by memaddr. * **Parameters:** *
+**addr** (`int`) â I2C peripheral device address * **memaddr** (`int`) â
+memory address * **buf** (`Buffer`) â bytes to write * **addrsize** (`int`)
+â \_description_, defaults to 8 #### I2C.readfrom_mem(addr, memaddr, nbytes,
+\*, addrsize=8) Read *nbytes* from the peripheral specified by *addr* starting
+from the memory address specified by *memaddr*. * **Parameters:** * **addr**
+(`int`) â I2C peripheral device address * **memaddr** (`int`) â memory
+address * **nbytes** (`int`) â number of bytes to read * **addrsize** (`int`)
+â \_description_, defaults to 8 * **Return type:** `bytes` * **Returns:** the
+bytes read #### I2C.readfrom_mem_into(addr, memaddr, buf, \*, addrsize=8) Read
+into buf from the peripheral specified by addr starting from the memory address
+specified by memaddr. The number of bytes read is the length of buf. *
+**Parameters:** * **addr** (`int`) â I2C peripheral device address *
+**memaddr** (`int`) â memory address * **buf** (`bytearray`) â buffer to
 store the bytes read * **addrsize** (`int`) â \_description_, defaults to 8
 ## Supported I2C drivers ### ch341 The CH341 series chip (like CH341A) is USB
 bus converter which converts USB to UART, parallel port, and common synchronous
 serial communication interfaces (I2C, SPI). The chip is manufactured by the
 company [Qinheng Microelectronics](https://wch-ic.com/). The ch341 driver
 shipped with this library is a Python interface to CH341âs official DLLs. You
 need the driver DLL files, which are downloadable from Qinhengâs website.
```

### Comparing `i2cpy-0.1.0b2/README.md` & `i2cpy-0.1.0b3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # Python I2C library supporting multiple driver implementations
 
 <div>
    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python"/>
-   <a href="https://pypi.org/project/i2cpy/">
-      <img src="https://img.shields.io/pypi/v/i2cpy.svg" alt="pypi"/>
-   </a>
-   <a href="https://github.com/iynehz/i2cpy/blob/main/LICENSE">
-      <img src="https://img.shields.io/badge/license-MIT-green" alt="license"/>
-   </a>
-   <img src="https://img.shields.io/badge/code%20style-black-black.svg" alt="Code style: black"/>
-   <img src="https://img.shields.io/badge/mypy-checked-green.svg" alt="mypy"/>
+   <a href="https://pypi.org/project/i2cpy/"><img src="https://img.shields.io/pypi/v/i2cpy.svg" alt="pypi"/></a>
+   <a href="https://github.com/iynehz/i2cpy/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-green" alt="license"/></a>
+   <img src="https://readthedocs.org/projects/i2cpy/badge/?version=latest" alt="docs"/>
+   <img src="https://github.com/iynehz/i2cpy/actions/workflows/lint.yml/badge.svg" alt="lint"/>
 </div>
 
 ## Introduction
 
 I2C is a two-wire protocol for communicating between devices. At the
 physical level it consists of 2 wires: SCL and SDA, the clock and data lines
 respectively.
@@ -41,15 +37,15 @@
                                  #   starting at memory address 2 in the peripheral
 ```
 
 ## Class I2C
 
 ### Constructor
 
-#### I2C.\_\_init_\_(\*, id=None, driver=None, freq=400000, auto_init=True, \*\*kwargs)
+#### I2C.\_\_init_\_(id=None, \*, driver=None, freq=400000, auto_init=True, \*\*kwargs)
 
 Constructor.
 
 * **Parameters:**
   * **id** (`Union`[`int`, `str`, `None`]) – Identifies a particular I2C peripheral. Allowed values depend
     on the particular driver implementation.
   * **freq** (`int`) – I2C bus baudrate, defaults to 400000
@@ -88,66 +84,66 @@
 ### Standard bus operations
 
 #### I2C.writeto(addr, buf, /)
 
 Write the bytes from buf to the peripheral specified by addr.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral deivce address
+  * **addr** (`int`) – I2C peripheral deivce address
   * **buf** (`Buffer`) – bytes to write
 
 #### I2C.readfrom(addr, nbytes, /)
 
 Read nbytes from the peripheral specified by addr.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
+  * **addr** (`int`) – I2C peripheral device address
   * **nbytes** (`int`) – number of bytes to read
 * **Return type:**
   `bytes`
 * **Returns:**
   the bytes read
 
 ### Memory operations
 
 #### I2C.writeto_mem(addr, memaddr, buf, \*, addrsize=8)
 
 Write buf to the peripheral specified by addr starting from the
 memory address specified by memaddr.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
-  * **memaddr** (`int` | `Buffer`) – memory address
+  * **addr** (`int`) – I2C peripheral device address
+  * **memaddr** (`int`) – memory address
   * **buf** (`Buffer`) – bytes to write
   * **addrsize** (`int`) – \_description_, defaults to 8
 
 #### I2C.readfrom_mem(addr, memaddr, nbytes, \*, addrsize=8)
 
 Read *nbytes* from the peripheral specified by *addr* starting from
 the memory address specified by *memaddr*.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
-  * **memaddr** (`int` | `Buffer`) – memory address
+  * **addr** (`int`) – I2C peripheral device address
+  * **memaddr** (`int`) – memory address
   * **nbytes** (`int`) – number of bytes to read
   * **addrsize** (`int`) – \_description_, defaults to 8
 * **Return type:**
   `bytes`
 * **Returns:**
   the bytes read
 
 #### I2C.readfrom_mem_into(addr, memaddr, buf, \*, addrsize=8)
 
 Read into buf from the peripheral specified by addr starting from the
 memory address specified by memaddr. The number of bytes read is the
 length of buf.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
-  * **memaddr** (`int` | `Buffer`) – memory address
+  * **addr** (`int`) – I2C peripheral device address
+  * **memaddr** (`int`) – memory address
   * **buf** (`bytearray`) – buffer to store the bytes read
   * **addrsize** (`int`) – \_description_, defaults to 8
 
 ## Supported I2C drivers
 
 ### ch341
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
 # Python I2C library supporting multiple driver implementations
-[python]_[_p_y_p_i_]_[_l_i_c_e_n_s_e_][Code style: black][mypy]
+[python]_[_p_y_p_i_]_[_l_i_c_e_n_s_e_][docs][lint]
 ## Introduction I2C is a two-wire protocol for communicating between devices.
 At the physical level it consists of 2 wires: SCL and SDA, the clock and data
 lines respectively. I2C objects are created attached to a specific bus. They
 can be initialized when created, or initialized later on. This library is
 designed to support different I2C driver implementations. Itâs interface is
 similar to MicroPythonâs `machine.I2C` as well as CircuitPythonâs
 `board.I2C` classes. Example usage: ```python from i2cpy import I2C i2c = I2C()
 # create I2C peripheral i2c.writeto(42, b'123') # write 3 bytes to peripheral
 with 7-bit address 42 i2c.readfrom(42, 4) # read 4 bytes from peripheral with
 7-bit address 42 i2c.readfrom_mem(42, 8, 3) # read 3 bytes from memory of
 peripheral 42, # starting at memory address 8 in the peripheral i2c.writeto_mem
 (42, 2, b'\x10') # write 1 byte to memory of peripheral 42, # starting at
 memory address 2 in the peripheral ``` ## Class I2C ### Constructor ####
-I2C.\_\_init_\_(\*, id=None, driver=None, freq=400000, auto_init=True,
+I2C.\_\_init_\_(id=None, \*, driver=None, freq=400000, auto_init=True,
 \*\*kwargs) Constructor. * **Parameters:** * **id** (`Union`[`int`, `str`,
 `None`]) â Identifies a particular I2C peripheral. Allowed values depend on
 the particular driver implementation. * **freq** (`int`) â I2C bus baudrate,
 defaults to 400000 * **driver** (`Optional`[`str`]) â I2C driver name. It
 corresponds to the I2C driver sub module name shipped with this library. For
 example âfooâ means module âi2cpy.driver.fooâ. If not specified, it
 looks at environment variable âI2CPY_DRIVERâ. And if thatâs not defined
@@ -27,36 +27,35 @@
 I2C.scan(start=8, stop=119) Scan all I2C addresses between start and stop
 inclusive and return a list of those that respond. A device responds if it
 pulls the SDA line low after its address (including a write bit) is sent on the
 bus. * **Parameters:** * **start** (`int`) â start address, defaults to 0x08
 * **stop** (`int`) â stop address, defaults to 0x77 * **Return type:** `List`
 [`int`] * **Returns:** a list of addresses that respond to scan ### Standard
 bus operations #### I2C.writeto(addr, buf, /) Write the bytes from buf to the
-peripheral specified by addr. * **Parameters:** * **addr** (`int` | `Buffer`)
-â I2C peripheral deivce address * **buf** (`Buffer`) â bytes to write ####
+peripheral specified by addr. * **Parameters:** * **addr** (`int`) â I2C
+peripheral deivce address * **buf** (`Buffer`) â bytes to write ####
 I2C.readfrom(addr, nbytes, /) Read nbytes from the peripheral specified by
-addr. * **Parameters:** * **addr** (`int` | `Buffer`) â I2C peripheral device
-address * **nbytes** (`int`) â number of bytes to read * **Return type:**
-`bytes` * **Returns:** the bytes read ### Memory operations ####
-I2C.writeto_mem(addr, memaddr, buf, \*, addrsize=8) Write buf to the peripheral
-specified by addr starting from the memory address specified by memaddr. *
-**Parameters:** * **addr** (`int` | `Buffer`) â I2C peripheral device address
-* **memaddr** (`int` | `Buffer`) â memory address * **buf** (`Buffer`) â
-bytes to write * **addrsize** (`int`) â \_description_, defaults to 8 ####
-I2C.readfrom_mem(addr, memaddr, nbytes, \*, addrsize=8) Read *nbytes* from the
-peripheral specified by *addr* starting from the memory address specified by
-*memaddr*. * **Parameters:** * **addr** (`int` | `Buffer`) â I2C peripheral
-device address * **memaddr** (`int` | `Buffer`) â memory address * **nbytes**
-(`int`) â number of bytes to read * **addrsize** (`int`) â \_description_,
-defaults to 8 * **Return type:** `bytes` * **Returns:** the bytes read ####
-I2C.readfrom_mem_into(addr, memaddr, buf, \*, addrsize=8) Read into buf from
-the peripheral specified by addr starting from the memory address specified by
-memaddr. The number of bytes read is the length of buf. * **Parameters:** *
-**addr** (`int` | `Buffer`) â I2C peripheral device address * **memaddr**
-(`int` | `Buffer`) â memory address * **buf** (`bytearray`) â buffer to
+addr. * **Parameters:** * **addr** (`int`) â I2C peripheral device address *
+**nbytes** (`int`) â number of bytes to read * **Return type:** `bytes` *
+**Returns:** the bytes read ### Memory operations #### I2C.writeto_mem(addr,
+memaddr, buf, \*, addrsize=8) Write buf to the peripheral specified by addr
+starting from the memory address specified by memaddr. * **Parameters:** *
+**addr** (`int`) â I2C peripheral device address * **memaddr** (`int`) â
+memory address * **buf** (`Buffer`) â bytes to write * **addrsize** (`int`)
+â \_description_, defaults to 8 #### I2C.readfrom_mem(addr, memaddr, nbytes,
+\*, addrsize=8) Read *nbytes* from the peripheral specified by *addr* starting
+from the memory address specified by *memaddr*. * **Parameters:** * **addr**
+(`int`) â I2C peripheral device address * **memaddr** (`int`) â memory
+address * **nbytes** (`int`) â number of bytes to read * **addrsize** (`int`)
+â \_description_, defaults to 8 * **Return type:** `bytes` * **Returns:** the
+bytes read #### I2C.readfrom_mem_into(addr, memaddr, buf, \*, addrsize=8) Read
+into buf from the peripheral specified by addr starting from the memory address
+specified by memaddr. The number of bytes read is the length of buf. *
+**Parameters:** * **addr** (`int`) â I2C peripheral device address *
+**memaddr** (`int`) â memory address * **buf** (`bytearray`) â buffer to
 store the bytes read * **addrsize** (`int`) â \_description_, defaults to 8
 ## Supported I2C drivers ### ch341 The CH341 series chip (like CH341A) is USB
 bus converter which converts USB to UART, parallel port, and common synchronous
 serial communication interfaces (I2C, SPI). The chip is manufactured by the
 company [Qinheng Microelectronics](https://wch-ic.com/). The ch341 driver
 shipped with this library is a Python interface to CH341âs official DLLs. You
 need the driver DLL files, which are downloadable from Qinhengâs website.
```

### Comparing `i2cpy-0.1.0b2/i2cpy/__init__.py` & `i2cpy-0.1.0b3/i2cpy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,29 +36,29 @@
 from typing import List, Optional
 
 try:
     from collections.abc import Buffer
 except ImportError:
     from typing_extensions import Buffer
 
-from i2cpy.driver.abc import i2c_addr_byte, to_buffer
-from i2cpy.errors import *
+from i2cpy.driver.abc import memaddr_to_bytes
+from i2cpy.errors import I2CInvalidDriverError
 
 
-from i2cpy._version import __version__
+from i2cpy._version import __version__  # noqa: F401
 
 
 log = logging.getLogger(__name__)
 
 
 class I2C:
     def __init__(
         self,
-        *,
         id: Optional[int | str] = None,
+        *,
         driver: Optional[str] = None,
         freq: int = 400000,
         auto_init: bool = True,
         **kwargs,
     ):
         """Constructor.
 
@@ -90,44 +90,44 @@
         """Initialize the I2C bus."""
         self.driver.init()
 
     def deinit(self):
         """Close the I2C bus."""
         self.driver.deinit()
 
-    def readfrom(self, addr: int | Buffer, nbytes: int, /) -> bytes:
+    def readfrom(self, addr: int, nbytes: int, /) -> bytes:
         """Read nbytes from the peripheral specified by addr.
 
         :param addr: I2C peripheral device address
         :param nbytes: number of bytes to read
         :return: the bytes read
         """
         return self.driver.readfrom(addr, nbytes)
 
-    def readfrom_into(self, addr: int | Buffer, buf: bytearray, /):
+    def readfrom_into(self, addr: int, buf: bytearray, /):
         """Read into buf from the peripheral specified by addr.
         The number of bytes read will be the length of buf.
 
         :param addr: I2C peripheral device address
         :param buf: buffer to store the bytes read
         """
         return self.driver.readfrom_into(addr, buf)
 
-    def writeto(self, addr: int | Buffer, buf: Buffer, /):
+    def writeto(self, addr: int, buf: Buffer, /):
         """Write the bytes from buf to the peripheral specified by addr.
 
         :param addr: I2C peripheral deivce address
         :param buf: bytes to write
         """
         return self.driver.writeto(addr, buf)
 
     def readfrom_mem_into(
         self,
-        addr: int | Buffer,
-        memaddr: int | Buffer,
+        addr: int,
+        memaddr: int,
         buf: bytearray,
         *,
         addrsize: int = 8,
     ):
         """Read into buf from the peripheral specified by addr starting from the
         memory address specified by memaddr. The number of bytes read is the
         length of buf.
@@ -137,50 +137,50 @@
         :param buf: buffer to store the bytes read
         :param addrsize: _description_, defaults to 8
         """
         return self.driver.readfrom_mem_into(addr, memaddr, buf, addrsize=addrsize)
 
     def readfrom_mem(
         self,
-        addr: int | Buffer,
-        memaddr: int | Buffer,
+        addr: int,
+        memaddr: int,
         nbytes: int,
         *,
         addrsize: int = 8,
     ) -> bytes:
         """Read *nbytes* from the peripheral specified by *addr* starting from
         the memory address specified by *memaddr*.
 
         :param addr: I2C peripheral device address
         :param memaddr: memory address
         :param nbytes: number of bytes to read
         :param addrsize: _description_, defaults to 8
         :return: the bytes read
         """
         buf = bytearray(nbytes)
-        self.readfrom_mem_into(addr, memaddr, buf, addrsize=addrsize)
+        self.readfrom_mem_into(addr, memaddr, buf)
         return bytes(buf)
 
     def writeto_mem(
         self,
-        addr: int | Buffer,
-        memaddr: int | Buffer,
+        addr: int,
+        memaddr: int,
         buf: Buffer,
         *,
         addrsize: int = 8,
     ):
         """Write buf to the peripheral specified by addr starting from the
         memory address specified by memaddr.
 
         :param addr: I2C peripheral device address
         :param memaddr: memory address
         :param buf: bytes to write
         :param addrsize: _description_, defaults to 8
         """
-        wbuf = bytes(to_buffer(memaddr)) + buf
+        wbuf = memaddr_to_bytes(memaddr, addrsize) + buf
         self.writeto(addr, wbuf)
 
     def scan(self, start: int = 0x08, stop: int = 0x77) -> List[int]:
         """Scan all I2C addresses between `start` and `stop` inclusive
         and return a list of those that respond.
         A device responds if it pulls the SDA line low after its address
         (including a write bit) is sent on the bus.
```

### Comparing `i2cpy-0.1.0b2/i2cpy/driver/abc.py` & `i2cpy-0.1.0b3/i2cpy/driver/abc.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from typing import List, TypeVar
 
 try:
     from collections.abc import Buffer
 except ImportError:
     from typing_extensions import Buffer
 
+from ..errors import I2CMemoryAddressSizeError
+
 
 def i2c_addr_byte(addr: int | Buffer, is_read: bool = False) -> bytes:
     """Convert 7-bit I2C peripheral address to bytes.
 
     :param addr: 7-bit peripheral address
     :param is_read: True for read
     :return: 1-byte `bytes` that can be written to I2C bus
@@ -34,14 +36,28 @@
     if isinstance(x, Buffer):
         return x
     if isinstance(x, list):
         return bytes(x)
     return bytes([x])
 
 
+def memaddr_to_bytes(memaddr: int, addrsize: int = 8) -> bytes:
+    """Convert memory address to `bytes`.
+
+    :param memaddr: memory address in integer.
+    :param addrsize: must be one of 8, 16, 24, 32. Default is 8.
+    :return: memory address in `bytes`
+    """
+    if addrsize & 0x7 != 0 or addrsize > 32 or addrsize < 8:
+        raise I2CMemoryAddressSizeError(addrsize)
+    return bytes(
+        to_buffer([(memaddr >> i) & 0xFF for i in range(addrsize - 8, -1, -8)])
+    )
+
+
 class I2CDriverBase(ABC):
     @abstractmethod
     def __init__(
         self,
         id: int = 0,
         *,
         freq: int = 400000,
@@ -70,46 +86,46 @@
         :return: the data read
         """
         buf = bytearray(nbytes)
         self.readfrom_into(addr, buf)
         return bytes(buf)
 
     @abstractmethod
-    def readfrom_into(self, addr: int | Buffer, buf: bytearray):
+    def readfrom_into(self, addr: int, buf: bytearray):
         """Read into buf from the peripheral specified by addr.
         The number of bytes read will be the length of buf.
 
         :param addr: I2C peripheral device address
         :param buf: buffer to store the bytes read
         """
 
     @abstractmethod
-    def writeto(self, addr: int | Buffer, buf: Buffer):
+    def writeto(self, addr: int, buf: Buffer):
         """Write the bytes from buf to the peripheral specified by addr.
 
         :param addr: I2C peripheral deivce address
         :param buf: bytes to write
         """
 
     @abstractmethod
     def readfrom_mem_into(
         self,
-        addr: int | Buffer,
-        memaddr: int | Buffer,
+        addr: int,
+        memaddr: int,
         buf: bytearray,
         *,
         addrsize: int = 8,
     ):
         """Read into buf from the peripheral specified by addr starting from the
         memory address specified by memaddr. The number of bytes read is the
         length of buf.
         """
 
     @abstractmethod
-    def check_device(self, addr: int | Buffer) -> bool:
+    def check_device(self, addr: int) -> bool:
         """Checks if I2C peripheral device exists at given address.
 
         :param addr: I2C peripheral device address
         :return: True if device responds.
         """
```

### Comparing `i2cpy-0.1.0b2/i2cpy/driver/ch341/dll.py` & `i2cpy-0.1.0b3/i2cpy/driver/ch341/dll.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import sys
 import os
 import re
 
-if os.name == "nt":
+if sys.platform == "win32":
     from ctypes import windll, CDLL
 else:
     from ctypes import cdll, CDLL, c_char_p, c_int32, c_uint8
 
 
 def load() -> CDLL:
     dll_name = os.getenv("CH341DLL")
     if dll_name is None:
-        if os.name == "nt":
+        if sys.platform == "win32":
             dll_name = "CH341DLLA64.dll" if sys.maxsize > 2147483647 else "CH341DLL.dll"
         else:
             dll_name = "libch347.so"
 
-    if os.name == "nt":
+    if sys.platform == "win32":
         return windll.LoadLibrary(dll_name)
     else:
         dll = cdll.LoadLibrary(dll_name)
 
         funcs = [
             "CH341OpenDevice",
             "CH341CloseDevice",
             "CH341SetStream",
             "CH341StreamI2C",
             "CH341WriteData",
-            "CH341WriteRead"
+            "CH341WriteRead",
         ]
 
         for fname in funcs:
             if not getattr(dll, fname, None):
                 fname2 = re.sub(r"^CH341", "CH34x", fname)
                 f = getattr(dll, fname2)
                 setattr(dll, fname, f)
```

### Comparing `i2cpy-0.1.0b2/i2cpy.egg-info/PKG-INFO` & `i2cpy-0.1.0b3/i2cpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cpy
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Python I2C library supporting multiple driver implementations
 Author-email: Zhenyi Zhou <iynehz@163.com>
 License: Copyright (c) 2024 Zhenyi Zhou
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -34,22 +34,18 @@
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.6.0; python_version < "3.12"
 
 # Python I2C library supporting multiple driver implementations
 
 <div>
    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python"/>
-   <a href="https://pypi.org/project/i2cpy/">
-      <img src="https://img.shields.io/pypi/v/i2cpy.svg" alt="pypi"/>
-   </a>
-   <a href="https://github.com/iynehz/i2cpy/blob/main/LICENSE">
-      <img src="https://img.shields.io/badge/license-MIT-green" alt="license"/>
-   </a>
-   <img src="https://img.shields.io/badge/code%20style-black-black.svg" alt="Code style: black"/>
-   <img src="https://img.shields.io/badge/mypy-checked-green.svg" alt="mypy"/>
+   <a href="https://pypi.org/project/i2cpy/"><img src="https://img.shields.io/pypi/v/i2cpy.svg" alt="pypi"/></a>
+   <a href="https://github.com/iynehz/i2cpy/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-green" alt="license"/></a>
+   <img src="https://readthedocs.org/projects/i2cpy/badge/?version=latest" alt="docs"/>
+   <img src="https://github.com/iynehz/i2cpy/actions/workflows/lint.yml/badge.svg" alt="lint"/>
 </div>
 
 ## Introduction
 
 I2C is a two-wire protocol for communicating between devices. At the
 physical level it consists of 2 wires: SCL and SDA, the clock and data lines
 respectively.
@@ -77,15 +73,15 @@
                                  #   starting at memory address 2 in the peripheral
 ```
 
 ## Class I2C
 
 ### Constructor
 
-#### I2C.\_\_init_\_(\*, id=None, driver=None, freq=400000, auto_init=True, \*\*kwargs)
+#### I2C.\_\_init_\_(id=None, \*, driver=None, freq=400000, auto_init=True, \*\*kwargs)
 
 Constructor.
 
 * **Parameters:**
   * **id** (`Union`[`int`, `str`, `None`]) – Identifies a particular I2C peripheral. Allowed values depend
     on the particular driver implementation.
   * **freq** (`int`) – I2C bus baudrate, defaults to 400000
@@ -124,66 +120,66 @@
 ### Standard bus operations
 
 #### I2C.writeto(addr, buf, /)
 
 Write the bytes from buf to the peripheral specified by addr.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral deivce address
+  * **addr** (`int`) – I2C peripheral deivce address
   * **buf** (`Buffer`) – bytes to write
 
 #### I2C.readfrom(addr, nbytes, /)
 
 Read nbytes from the peripheral specified by addr.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
+  * **addr** (`int`) – I2C peripheral device address
   * **nbytes** (`int`) – number of bytes to read
 * **Return type:**
   `bytes`
 * **Returns:**
   the bytes read
 
 ### Memory operations
 
 #### I2C.writeto_mem(addr, memaddr, buf, \*, addrsize=8)
 
 Write buf to the peripheral specified by addr starting from the
 memory address specified by memaddr.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
-  * **memaddr** (`int` | `Buffer`) – memory address
+  * **addr** (`int`) – I2C peripheral device address
+  * **memaddr** (`int`) – memory address
   * **buf** (`Buffer`) – bytes to write
   * **addrsize** (`int`) – \_description_, defaults to 8
 
 #### I2C.readfrom_mem(addr, memaddr, nbytes, \*, addrsize=8)
 
 Read *nbytes* from the peripheral specified by *addr* starting from
 the memory address specified by *memaddr*.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
-  * **memaddr** (`int` | `Buffer`) – memory address
+  * **addr** (`int`) – I2C peripheral device address
+  * **memaddr** (`int`) – memory address
   * **nbytes** (`int`) – number of bytes to read
   * **addrsize** (`int`) – \_description_, defaults to 8
 * **Return type:**
   `bytes`
 * **Returns:**
   the bytes read
 
 #### I2C.readfrom_mem_into(addr, memaddr, buf, \*, addrsize=8)
 
 Read into buf from the peripheral specified by addr starting from the
 memory address specified by memaddr. The number of bytes read is the
 length of buf.
 
 * **Parameters:**
-  * **addr** (`int` | `Buffer`) – I2C peripheral device address
-  * **memaddr** (`int` | `Buffer`) – memory address
+  * **addr** (`int`) – I2C peripheral device address
+  * **memaddr** (`int`) – memory address
   * **buf** (`bytearray`) – buffer to store the bytes read
   * **addrsize** (`int`) – \_description_, defaults to 8
 
 ## Supported I2C drivers
 
 ### ch341
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: i2cpy Version: 0.1.0b2 Summary: Python I2C library
+Metadata-Version: 2.1 Name: i2cpy Version: 0.1.0b3 Summary: Python I2C library
 supporting multiple driver implementations Author-email: Zhenyi Zhou
 163.com> License: Copyright (c) 2024 Zhenyi Zhou Permission is hereby granted,
 free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
@@ -17,29 +17,29 @@
 Project-URL: Homepage, https://github.com/iynehz/i2cpy Project-URL:
 Documentation, https://i2cpy.readthedocs.io/en/latest/ Project-URL: Repository,
 https://github.com/iynehz/i2cpy Keywords: i2c,ch341,ch341a Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: typing_extensions>=4.6.0; python_version < "3.12" #
 Python I2C library supporting multiple driver implementations
-[python]_[_p_y_p_i_]_[_l_i_c_e_n_s_e_][Code style: black][mypy]
+[python]_[_p_y_p_i_]_[_l_i_c_e_n_s_e_][docs][lint]
 ## Introduction I2C is a two-wire protocol for communicating between devices.
 At the physical level it consists of 2 wires: SCL and SDA, the clock and data
 lines respectively. I2C objects are created attached to a specific bus. They
 can be initialized when created, or initialized later on. This library is
 designed to support different I2C driver implementations. Itâs interface is
 similar to MicroPythonâs `machine.I2C` as well as CircuitPythonâs
 `board.I2C` classes. Example usage: ```python from i2cpy import I2C i2c = I2C()
 # create I2C peripheral i2c.writeto(42, b'123') # write 3 bytes to peripheral
 with 7-bit address 42 i2c.readfrom(42, 4) # read 4 bytes from peripheral with
 7-bit address 42 i2c.readfrom_mem(42, 8, 3) # read 3 bytes from memory of
 peripheral 42, # starting at memory address 8 in the peripheral i2c.writeto_mem
 (42, 2, b'\x10') # write 1 byte to memory of peripheral 42, # starting at
 memory address 2 in the peripheral ``` ## Class I2C ### Constructor ####
-I2C.\_\_init_\_(\*, id=None, driver=None, freq=400000, auto_init=True,
+I2C.\_\_init_\_(id=None, \*, driver=None, freq=400000, auto_init=True,
 \*\*kwargs) Constructor. * **Parameters:** * **id** (`Union`[`int`, `str`,
 `None`]) â Identifies a particular I2C peripheral. Allowed values depend on
 the particular driver implementation. * **freq** (`int`) â I2C bus baudrate,
 defaults to 400000 * **driver** (`Optional`[`str`]) â I2C driver name. It
 corresponds to the I2C driver sub module name shipped with this library. For
 example âfooâ means module âi2cpy.driver.fooâ. If not specified, it
 looks at environment variable âI2CPY_DRIVERâ. And if thatâs not defined
@@ -49,36 +49,35 @@
 I2C.scan(start=8, stop=119) Scan all I2C addresses between start and stop
 inclusive and return a list of those that respond. A device responds if it
 pulls the SDA line low after its address (including a write bit) is sent on the
 bus. * **Parameters:** * **start** (`int`) â start address, defaults to 0x08
 * **stop** (`int`) â stop address, defaults to 0x77 * **Return type:** `List`
 [`int`] * **Returns:** a list of addresses that respond to scan ### Standard
 bus operations #### I2C.writeto(addr, buf, /) Write the bytes from buf to the
-peripheral specified by addr. * **Parameters:** * **addr** (`int` | `Buffer`)
-â I2C peripheral deivce address * **buf** (`Buffer`) â bytes to write ####
+peripheral specified by addr. * **Parameters:** * **addr** (`int`) â I2C
+peripheral deivce address * **buf** (`Buffer`) â bytes to write ####
 I2C.readfrom(addr, nbytes, /) Read nbytes from the peripheral specified by
-addr. * **Parameters:** * **addr** (`int` | `Buffer`) â I2C peripheral device
-address * **nbytes** (`int`) â number of bytes to read * **Return type:**
-`bytes` * **Returns:** the bytes read ### Memory operations ####
-I2C.writeto_mem(addr, memaddr, buf, \*, addrsize=8) Write buf to the peripheral
-specified by addr starting from the memory address specified by memaddr. *
-**Parameters:** * **addr** (`int` | `Buffer`) â I2C peripheral device address
-* **memaddr** (`int` | `Buffer`) â memory address * **buf** (`Buffer`) â
-bytes to write * **addrsize** (`int`) â \_description_, defaults to 8 ####
-I2C.readfrom_mem(addr, memaddr, nbytes, \*, addrsize=8) Read *nbytes* from the
-peripheral specified by *addr* starting from the memory address specified by
-*memaddr*. * **Parameters:** * **addr** (`int` | `Buffer`) â I2C peripheral
-device address * **memaddr** (`int` | `Buffer`) â memory address * **nbytes**
-(`int`) â number of bytes to read * **addrsize** (`int`) â \_description_,
-defaults to 8 * **Return type:** `bytes` * **Returns:** the bytes read ####
-I2C.readfrom_mem_into(addr, memaddr, buf, \*, addrsize=8) Read into buf from
-the peripheral specified by addr starting from the memory address specified by
-memaddr. The number of bytes read is the length of buf. * **Parameters:** *
-**addr** (`int` | `Buffer`) â I2C peripheral device address * **memaddr**
-(`int` | `Buffer`) â memory address * **buf** (`bytearray`) â buffer to
+addr. * **Parameters:** * **addr** (`int`) â I2C peripheral device address *
+**nbytes** (`int`) â number of bytes to read * **Return type:** `bytes` *
+**Returns:** the bytes read ### Memory operations #### I2C.writeto_mem(addr,
+memaddr, buf, \*, addrsize=8) Write buf to the peripheral specified by addr
+starting from the memory address specified by memaddr. * **Parameters:** *
+**addr** (`int`) â I2C peripheral device address * **memaddr** (`int`) â
+memory address * **buf** (`Buffer`) â bytes to write * **addrsize** (`int`)
+â \_description_, defaults to 8 #### I2C.readfrom_mem(addr, memaddr, nbytes,
+\*, addrsize=8) Read *nbytes* from the peripheral specified by *addr* starting
+from the memory address specified by *memaddr*. * **Parameters:** * **addr**
+(`int`) â I2C peripheral device address * **memaddr** (`int`) â memory
+address * **nbytes** (`int`) â number of bytes to read * **addrsize** (`int`)
+â \_description_, defaults to 8 * **Return type:** `bytes` * **Returns:** the
+bytes read #### I2C.readfrom_mem_into(addr, memaddr, buf, \*, addrsize=8) Read
+into buf from the peripheral specified by addr starting from the memory address
+specified by memaddr. The number of bytes read is the length of buf. *
+**Parameters:** * **addr** (`int`) â I2C peripheral device address *
+**memaddr** (`int`) â memory address * **buf** (`bytearray`) â buffer to
 store the bytes read * **addrsize** (`int`) â \_description_, defaults to 8
 ## Supported I2C drivers ### ch341 The CH341 series chip (like CH341A) is USB
 bus converter which converts USB to UART, parallel port, and common synchronous
 serial communication interfaces (I2C, SPI). The chip is manufactured by the
 company [Qinheng Microelectronics](https://wch-ic.com/). The ch341 driver
 shipped with this library is a Python interface to CH341âs official DLLs. You
 need the driver DLL files, which are downloadable from Qinhengâs website.
```

### Comparing `i2cpy-0.1.0b2/pyproject.toml` & `i2cpy-0.1.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `i2cpy-0.1.0b2/tests/test_i2c.py` & `i2cpy-0.1.0b3/tests/test_i2c.py`

 * *Files identical despite different names*

