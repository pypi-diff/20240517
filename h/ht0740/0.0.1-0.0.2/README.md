# Comparing `tmp/ht0740-0.0.1.tar.gz` & `tmp/ht0740-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ht0740-0.0.1.tar", last modified: Wed Jul 31 14:44:59 2019, max compression
+gzip compressed data, was "dist/ht0740-0.0.2.tar", last modified: Fri Sep 13 09:56:35 2019, max compression
```

## Comparing `ht0740-0.0.1.tar` & `ht0740-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-07-31 14:44:59.000000 ht0740-0.0.1/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-07-31 14:44:59.000000 ht0740-0.0.1/ht0740/
--rw-r--r--   0 pi        (1000) pi        (1000)     3611 2019-07-29 15:23:02.000000 ht0740-0.0.1/ht0740/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1973 2019-07-31 14:44:59.000000 ht0740-0.0.1/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-07-31 14:44:59.000000 ht0740-0.0.1/ht0740.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2019-07-31 14:44:59.000000 ht0740-0.0.1/ht0740.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1973 2019-07-31 14:44:59.000000 ht0740-0.0.1/ht0740.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2019-07-31 14:44:59.000000 ht0740-0.0.1/ht0740.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       10 2019-07-31 14:44:59.000000 ht0740-0.0.1/ht0740.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      235 2019-07-31 14:44:59.000000 ht0740-0.0.1/ht0740.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      108 2019-07-29 15:23:02.000000 ht0740-0.0.1/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)      960 2019-07-29 15:23:02.000000 ht0740-0.0.1/README.rst
--rw-r--r--   0 pi        (1000) pi        (1000)       31 2019-07-29 15:23:02.000000 ht0740-0.0.1/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2019-07-29 15:23:02.000000 ht0740-0.0.1/LICENSE.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      165 2019-07-31 14:44:59.000000 ht0740-0.0.1/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     2159 2019-07-29 15:23:02.000000 ht0740-0.0.1/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-13 09:56:35.000000 ht0740-0.0.2/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-13 09:56:35.000000 ht0740-0.0.2/ht0740/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3669 2019-09-13 09:56:11.000000 ht0740-0.0.2/ht0740/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1642 2019-09-13 09:56:35.000000 ht0740-0.0.2/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-13 09:56:35.000000 ht0740-0.0.2/ht0740.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)        7 2019-09-13 09:56:34.000000 ht0740-0.0.2/ht0740.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     1642 2019-09-13 09:56:34.000000 ht0740-0.0.2/ht0740.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2019-09-13 09:56:34.000000 ht0740-0.0.2/ht0740.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       17 2019-09-13 09:56:34.000000 ht0740-0.0.2/ht0740.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      235 2019-09-13 09:56:34.000000 ht0740-0.0.2/ht0740.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      108 2019-07-29 15:23:02.000000 ht0740-0.0.2/MANIFEST.in
+-rw-r--r--   0 pi        (1000) pi        (1000)      572 2019-09-13 09:56:23.000000 ht0740-0.0.2/README.rst
+-rw-r--r--   0 pi        (1000) pi        (1000)       88 2019-09-13 09:56:11.000000 ht0740-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     1070 2019-07-29 15:23:02.000000 ht0740-0.0.2/LICENSE.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      165 2019-09-13 09:56:35.000000 ht0740-0.0.2/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     2166 2019-09-13 09:56:11.000000 ht0740-0.0.2/setup.py
```

### Comparing `ht0740-0.0.1/ht0740/__init__.py` & `ht0740-0.0.2/ht0740/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 from i2cdevice import Device, Register, BitField
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 
 class IOItem:
-
     def __init__(self, i2c_object, pin_io, inverted=False):
         self.enabled = True
         self.status = False
         self.i2c_object = i2c_object
         self.pin_io = pin_io
         self.inverted = inverted
 
     def state(self):
         if self.inverted:
-            return ~self.i2c_object.OUTPUT.get_value() >> self.pin_io & 1
+            return ~self.i2c_object.get('OUTPUT').value >> self.pin_io & 1
         else:
-            return self.i2c_object.OUTPUT.get_value() >> self.pin_io & 1
+            return self.i2c_object.get('OUTPUT').value >> self.pin_io & 1
 
     def set(self, state):
         if self.enabled:
             if self.inverted:
                 state = 1 - state
-            value = self.i2c_object.OUTPUT.get_value()
+            value = self.i2c_object.get('OUTPUT').value
             mask = 1 << self.pin_io
-            self.i2c_object.OUTPUT.set_value(((value & ~mask) | ((state << self.pin_io) & mask)))
+            self.i2c_object.set('OUTPUT', value=((value & ~mask) | ((state << self.pin_io) & mask)))
 
     def on(self):
         self.set(1)
 
     def off(self):
         self.set(0)
 
     def toggle(self):
         if self.enabled:
-            self.i2c_object.OUTPUT.set_value(self.i2c_object.OUTPUT.get_value() ^ (1 << self.pin_io))
+            self.i2c_object.set('OUTPUT', value=self.i2c_object.OUTPUT.get_value() ^ (1 << self.pin_io))
 
     def disable(self):
-        self.i2c_object.CONFIG.set_value(self.i2c_object.CONFIG.get_value() | 1 << self.pin_io)
+        self.i2c_object.set('CONFIG', value=self.i2c_object.CONFIG.get_value() | 1 << self.pin_io)
         self.enabled = False
 
     def enable(self):
-        self.i2c_object.CONFIG.set_value(self.i2c_object.CONFIG.get_value() & ~(1 << self.pin_io))
+        self.i2c_object.set('CONFIG', value=self.i2c_object.CONFIG.get_value() & ~(1 << self.pin_io))
         self.enabled = True
 
 
 class PCA9554A:
-
     def __init__(self, i2c_addr=0x38, i2c_dev=None):
         self._i2c_addr = i2c_addr
         self._i2c_dev = i2c_dev
         self._is_setup = False
         # Device definition
         self._pca9554a = Device(self._i2c_addr, i2c_dev=self._i2c_dev, bit_width=8, registers=(
             Register('INPUT', 0x00, fields=(
@@ -71,26 +69,27 @@
             Register('CONFIG', 0x03, fields=(
                 BitField('value', 0xFF),
                 BitField('switch', 0b00001000),
                 BitField('led', 0b00000001)
             )),
         ))
         #  Set IO configuration for driving switch and LED
-        self._pca9554a.OUTPUT.set_switch(0)
-        self._pca9554a.OUTPUT.set_led(1)
-        self._pca9554a.CONFIG.set_switch(0)
-        self._pca9554a.CONFIG.set_led(0)
+        self._pca9554a.set('OUTPUT',
+                           switch=0,
+                           led=1)
+        self._pca9554a.set('CONFIG',
+                           switch=0,
+                           led=0)
         self.led_enable = True
         self.switch_enabled = True
         self.led_status = False
         self.switch_status = False
 
 
 class HT0740:
-
     def __init__(self, i2c_addr=0x38, i2c_dev=None):
         self._i2c_addr = i2c_addr
         self._i2c_dev = i2c_dev
         self._is_setup = False
         self.led_io = 0
 
         self.switch_io = 3
```

### Comparing `ht0740-0.0.1/LICENSE.txt` & `ht0740-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ht0740-0.0.1/setup.py` & `ht0740-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,20 +35,20 @@
                'Programming Language :: Python :: 2.7',
                'Programming Language :: Python :: 3',
                'Topic :: Software Development',
                'Topic :: System :: Hardware']
 
 setup(
     name='ht0740',
-    version='0.0.1',
+    version='0.0.2',
     author='Gee Bartlett',
     author_email='gee@pimoroni.com',
     description="""Python library for the HT0740 Switch""",
     long_description=open('README.rst').read() + '\n' + open('CHANGELOG.txt').read(),
     license='MIT',
     keywords='Raspberry Pi',
     url='http://www.pimoroni.com',
     project_urls={'GitHub': 'https://www.github.com/pimoroni/ht0740-python'},
     classifiers=classifiers,
     packages=['ht0740'],
-    install_requires=['i2cdevice']
+    install_requires=['i2cdevice>=0.0.6']
 )
```

