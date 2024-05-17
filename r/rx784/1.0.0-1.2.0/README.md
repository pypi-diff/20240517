# Comparing `tmp/rx784-1.0.0.tar.gz` & `tmp/rx784-1.2.0.tar.gz`

## Comparing `rx784-1.0.0.tar` & `rx784-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 rx784-1.0.0/.gitattributes
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 rx784-1.0.0/rx784/__about__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 rx784-1.0.0/rx784/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 rx784-1.0.0/rx784/button.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 rx784-1.0.0/rx784/command.py
--rw-r--r--   0        0        0    21618 2020-02-02 00:00:00.000000 rx784-1.0.0/rx784/device.py
--rw-r--r--   0        0        0    22964 2020-02-02 00:00:00.000000 rx784-1.0.0/rx784/key_code.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 rx784-1.0.0/rx784/keyboard_led.py
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 rx784-1.0.0/rx784/state.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 rx784-1.0.0/rx784/status.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 rx784-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 rx784-1.0.0/tests/test_smoke.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 rx784-1.0.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 rx784-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 rx784-1.0.0/README.md
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 rx784-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 rx784-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 rx784-1.2.0/.gitattributes
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 rx784-1.2.0/rx784/__about__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 rx784-1.2.0/rx784/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 rx784-1.2.0/rx784/button.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 rx784-1.2.0/rx784/command.py
+-rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 rx784-1.2.0/rx784/device.py
+-rw-r--r--   0        0        0    22964 2020-02-02 00:00:00.000000 rx784-1.2.0/rx784/key_code.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 rx784-1.2.0/rx784/keyboard_led.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 rx784-1.2.0/rx784/state.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 rx784-1.2.0/rx784/status.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 rx784-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 rx784-1.2.0/tests/test_smoke.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 rx784-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 rx784-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 rx784-1.2.0/README.md
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 rx784-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 rx784-1.2.0/PKG-INFO
```

### Comparing `rx784-1.0.0/.gitattributes` & `rx784-1.2.0/.gitattributes`

 * *Files identical despite different names*

### Comparing `rx784-1.0.0/rx784/__init__.py` & `rx784-1.2.0/rx784/__init__.py`

 * *Files identical despite different names*

### Comparing `rx784-1.0.0/rx784/command.py` & `rx784-1.2.0/rx784/command.py`

 * *Files identical despite different names*

### Comparing `rx784-1.0.0/rx784/device.py` & `rx784-1.2.0/rx784/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,17 +150,19 @@
         status = self.__send_packet(Command.GET_BUTTONS_STATE)
         if (status != Status.SUCCESS): return status, None
 
         status, state = self.__recv_packet(Command.GET_BUTTONS_STATE, 1)
         if (status != Status.SUCCESS): return status, None
 
         return Status.SUCCESS, ButtonsState(
-            state[0] & (1 << Button.LEFT)   != 0,
-            state[0] & (1 << Button.RIGHT)  != 0,
-            state[0] & (1 << Button.MIDDLE) != 0,
+            state[0] & (1 << Button.LEFT)    != 0,
+            state[0] & (1 << Button.RIGHT)   != 0,
+            state[0] & (1 << Button.MIDDLE)  != 0,
+            state[0] & (1 << Button.BUTTON4) != 0,
+            state[0] & (1 << Button.BUTTON5) != 0,
         )
 
     def move_rel(self, x: int, y: int) -> Status:
         status = self.__send_packet(Command.MOVE_REL,
                                     x.to_bytes(2, 'little', signed=True) + y.to_bytes(2, 'little', signed=True))
         if status != Status.SUCCESS: return status
 
@@ -183,17 +185,19 @@
         if (status != Status.SUCCESS): return status, None
 
         status, data = self.__recv_packet(Command.GET_REL_MOUSE_STATE, 1)
         if (status != Status.SUCCESS): return status, None
 
         return Status.SUCCESS, MouseState(
             MouseState.Buttons(
-                data[0] & (1 << Button.LEFT)   != 0,
-                data[0] & (1 << Button.RIGHT)  != 0,
-                data[0] & (1 << Button.MIDDLE) != 0,
+                data[0] & (1 << Button.LEFT)    != 0,
+                data[0] & (1 << Button.RIGHT)   != 0,
+                data[0] & (1 << Button.MIDDLE)  != 0,
+                data[0] & (1 << Button.BUTTON4) != 0,
+                data[0] & (1 << Button.BUTTON5) != 0,
             ),
             MouseState.Axes(0, 0, 0)
         )
 
     def send_rel_mouse_state(self, mouse_state: MouseState, mouse_state_mask: MouseStateMask) -> Status:
         status = self.__send_packet(Command.SEND_REL_MOUSE_STATE,
                                     mouse_state_mask.to_bytes() + mouse_state.to_bytes())
@@ -299,17 +303,19 @@
         if (status != Status.SUCCESS): return status, None
 
         status, data = self.__recv_packet(Command.GET_ABS_MOUSE_STATE, 7)
         if (status != Status.SUCCESS): return status, None
 
         return Status.SUCCESS, MouseState(
             MouseState.Buttons(
-                data[0] & (1 << Button.LEFT)   != 0,
-                data[0] & (1 << Button.RIGHT)  != 0,
-                data[0] & (1 << Button.MIDDLE) != 0,
+                data[0] & (1 << Button.LEFT)    != 0,
+                data[0] & (1 << Button.RIGHT)   != 0,
+                data[0] & (1 << Button.MIDDLE)  != 0,
+                data[0] & (1 << Button.BUTTON4) != 0,
+                data[0] & (1 << Button.BUTTON5) != 0,
             ),
             MouseState.Axes(
                 int.from_bytes(data[1:3], 'little', signed=True),
                 int.from_bytes(data[3:5], 'little', signed=True),
                 int.from_bytes(data[5:7], 'little', signed=True)
             )
         )
```

### Comparing `rx784-1.0.0/rx784/key_code.py` & `rx784-1.2.0/rx784/key_code.py`

 * *Files identical despite different names*

### Comparing `rx784-1.0.0/rx784/state.py` & `rx784-1.2.0/rx784/state.py`

 * *Files 22% similar despite different names*

```diff
@@ -38,40 +38,46 @@
     scroll_lock: bool
     compose:     bool
     kana:        bool
 
 
 @dataclass
 class ButtonsState:
-    left:   bool
-    right:  bool
-    middle: bool
+    left:    bool
+    right:   bool
+    middle:  bool
+    button4: bool
+    button5: bool
 
 
 @dataclass
 class MouseState:
     @dataclass
     class Buttons:
         left:   bool
         right:  bool
         middle: bool
+        button4: bool
+        button5: bool
 
     @dataclass
     class Axes:
         x: int
         y: int
         w: int
 
     buttons: Buttons
     axes:    Axes
 
     def to_bytes(self) -> bytes:
         return (((self.buttons.left   << Button.LEFT)
                | (self.buttons.right  << Button.RIGHT)
-               | (self.buttons.middle << Button.MIDDLE)).to_bytes(1, 'little')
+               | (self.buttons.right  << Button.MIDDLE)
+               | (self.buttons.right  << Button.BUTTON4)
+               | (self.buttons.middle << Button.BUTTON5)).to_bytes(1, 'little')
               + self.axes.x.to_bytes(2, 'little')
               + self.axes.y.to_bytes(2, 'little')
               + self.axes.w.to_bytes(2, 'little'))
 
 
 @dataclass
 class KeyboardStateMask:
```

### Comparing `rx784-1.0.0/.gitignore` & `rx784-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rx784-1.0.0/LICENSE.txt` & `rx784-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rx784-1.0.0/pyproject.toml` & `rx784-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rx784-1.0.0/PKG-INFO` & `rx784-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rx784
-Version: 1.0.0
+Version: 1.2.0
 Project-URL: Documentation, https://github.com/dulong-lab/rx784-py#readme
 Project-URL: Issues, https://github.com/dulong-lab/rx784-py/issues
 Project-URL: Source, https://github.com/dulong-lab/rx784-py
 Author-email: dulong-lab <dulong-lab@outlook.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
```

