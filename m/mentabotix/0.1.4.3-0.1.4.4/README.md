# Comparing `tmp/mentabotix-0.1.4.3.tar.gz` & `tmp/mentabotix-0.1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.4.3.tar", last modified: Thu May 16 15:48:25 2024, max compression
+gzip compressed data, was "mentabotix-0.1.4.4.tar", last modified: Fri May 17 16:49:15 2024, max compression
```

## Comparing `mentabotix-0.1.4.3.tar` & `mentabotix-0.1.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-05-16 15:47:59.154746 mentabotix-0.1.4.3/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-16 15:47:59.154746 mentabotix-0.1.4.3/README.md
--rw-r--r--   0        0        0      680 2024-05-16 15:48:25.338749 mentabotix-0.1.4.3/pyproject.toml
--rw-r--r--   0        0        0     1210 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    67869 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     9471 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     9429 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/tests/find_tests.py
--rw-r--r--   0        0        0    15535 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/tests/test_botix.py
--rw-r--r--   0        0        0    10196 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/tests/test_menta.py
--rw-r--r--   0        0        0     6488 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/tests/test_moving_state.py
--rw-r--r--   0        0        0     5338 2024-05-16 15:47:59.158746 mentabotix-0.1.4.3/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 16:48:50.872905 mentabotix-0.1.4.4/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-17 16:48:50.872905 mentabotix-0.1.4.4/README.md
+-rw-r--r--   0        0        0      680 2024-05-17 16:49:15.237063 mentabotix-0.1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1210 2024-05-17 16:48:50.872905 mentabotix-0.1.4.4/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    69823 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     9471 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     9429 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/find_tests.py
+-rw-r--r--   0        0        0    15535 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_botix.py
+-rw-r--r--   0        0        0    10196 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_menta.py
+-rw-r--r--   0        0        0     7061 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5338 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.4/PKG-INFO
```

### Comparing `mentabotix-0.1.4.3/LICENSE` & `mentabotix-0.1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/README.md` & `mentabotix-0.1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/pyproject.toml` & `mentabotix-0.1.4.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "mentabotix"
-version = "0.1.4.3"
+version = "0.1.4.4"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
     "pyapriltags>=3.3.0.3",
     "terminaltables>=3.1.10",
-    "bdmc>=0.1.5.7",
+    "bdmc>=0.1.5.8",
     "opencv-python-headless>=4.9.0.80",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `mentabotix-0.1.4.3/src/mentabotix/__init__.py` & `mentabotix-0.1.4.4/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/src/mentabotix/modules/botix.py` & `mentabotix-0.1.4.4/src/mentabotix/modules/botix.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     Set,
     Sequence,
     get_type_hints,
 )
 
 import numpy as np
 from bdmc import CloseLoopController
+from numpy.random import random
 from terminaltables import SingleTable
 
 from .exceptions import StructuralError, TokenizeError
 from ..tools.generators import NameGenerator
 
 T_EXPR = TypeVar("T_EXPR", str, list)
 
@@ -394,14 +395,51 @@
                 return cls(-speed, speed)
             case "r":
                 return cls(speed, -speed)
             case _:
                 raise ValueError("Invalid Direction. Must be one of ['l','r']")
 
     @classmethod
+    def rand_turn(
+        cls, con: CloseLoopController, turn_speed: int, used_ctx_varname: str = "direction", turn_left_prob: float = 0.5
+    ) -> Self:
+        """
+        Adds a method for random turning to the CloseLoopController class.
+
+        Parameters:
+            cls: Class method convention parameter, referring to the current class.
+            con: CloseLoopController object, representing the instance to which the random turning control is applied.
+            turn_speed: Turning speed, positive for turning right, negative for turning left.
+            used_ctx_varname: Context variable name used to represent the turn direction, defaults to "direction".
+            turn_left_prob: Probability of turning left, defaults to 0.5, meaning equal chance of turning left or right.
+
+        Returns:
+            None
+        """
+
+        def _dir() -> int:
+            """
+            Internal function to randomly decide the turn direction.
+
+            Returns:
+                int: 1 for turning left, -1 for turning right.
+            """
+            return 1 if random() < turn_left_prob else -1
+
+        # Register a context updater to update the turn direction before entering this behavior.
+        _updater = con.register_context_updater(_dir, output_keys=[used_ctx_varname], input_keys=[])
+
+        # Set speed expressions and actions before entering, implementing random turning.
+        return cls(
+            speed_expressions=(f"{-turn_speed}*{used_ctx_varname}", f"{turn_speed}*{used_ctx_varname}"),
+            used_context_variables=[used_ctx_varname],
+            before_entering=[_updater],
+        )
+
+    @classmethod
     def drift(cls, fixed_axis: Literal["fl", "rl", "rr", "fr"], speed: int) -> Self:
         """
         Create a new instance of the class with the specified drift direction and speed.
         Lets the bot make a drift with the specified direction and speed in place.
 
         Note:
             This movement is achieved by making a wheel fixed, while the others move with the specified speed.
@@ -598,15 +636,23 @@
         else:
             return source.replace(var_name, f"({temp_name}:={func_name}())", 1).replace(var_name, temp_name)
 
     def __hash__(self) -> int:
         return self._identifier
 
     def __eq__(self, other: Self) -> bool:
-        return tuple(self._speeds) == tuple(other._speeds) and self._speed_expressions == other._speed_expressions
+        if self._speeds is None or other._speeds is None:
+            return self._speed_expressions == other._speed_expressions
+        elif self._speeds is None:
+            return False
+        elif other._speeds is None:
+            return False
+        else:
+
+            return all(np.equal(self._speeds, other._speeds)) and self._speed_expressions == other._speed_expressions
 
     def __str__(self):
         return f"{self._identifier}-MovingState{self._speed_expressions or (tuple(self._speeds) if self._speeds is not None else None)}"
 
     def __repr__(self):
         return str(self)
 
@@ -1150,15 +1196,15 @@
 
     def _check_met_requirements(self):
         self.ensure_structure_validity(self.token_pool)
         start_state = self.acquire_unique_start(self.token_pool)
         end_states = self.acquire_end_states(self.token_pool)
         self.ensure_accessibility(self.token_pool, start_state, end_states)
         if self.acquire_loops():
-            raise ValueError("Loops detected! All State-Transition should be implemented using breaker")
+            raise ValueError("Loops detected! All State-Transition should be implemented without loops.")
 
     def _assembly_match_cases(self, match_expression: str | List[str], cases: Dict[KT, str | List[str]]) -> List[str]:
         """
         Assembles a list of strings representing match cases based on the given match expression and cases dictionary.
 
         Parameters:
             match_expression (str): The match expression to be used.
```

### Comparing `mentabotix-0.1.4.3/src/mentabotix/modules/logger.py` & `mentabotix-0.1.4.4/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/src/mentabotix/modules/menta.py` & `mentabotix-0.1.4.4/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/src/mentabotix/tools/composers.py` & `mentabotix-0.1.4.4/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/src/mentabotix/tools/generators.py` & `mentabotix-0.1.4.4/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.4.4/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/tests/find_tests.py` & `mentabotix-0.1.4.4/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/tests/test_botix.py` & `mentabotix-0.1.4.4/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/tests/test_composer.py` & `mentabotix-0.1.4.4/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/tests/test_menta.py` & `mentabotix-0.1.4.4/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/tests/test_moving_state.py` & `mentabotix-0.1.4.4/tests/test_moving_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -148,10 +148,27 @@
 
     def test_str(self):
         state = MovingState(10, 20, 30, 40)
         self.assertEqual(str(state), f"{state.state_id}-MovingState(10, 20, 30, 40)")
         state = MovingState(speed_expressions="var1", used_context_variables=["var1"])
         self.assertEqual(str(state), f"{state.state_id}-MovingState('var1', 'var1', 'var1', 'var1')")
 
+    def test_random_turn(self):
+        from mentabotix import MovingTransition, Botix
+
+        con = CloseLoopController(
+            [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM10", context={"var1": 10, "var2": 20}
+        ).start_msg_sending()
+        state = MovingState.rand_turn(con, 500)
+        print(state)
+        end = MovingState(0)
+        trans = MovingTransition(1, from_states=[state], to_states={0: end})
+
+        b = Botix(controller=con, token_pool=[trans])
+
+        fun = b.compile()
+        fun()
+        con.stop_msg_sending()
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.4.3/tests/test_moving_transition.py` & `mentabotix-0.1.4.4/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.3/PKG-INFO` & `mentabotix-0.1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.4.3
+Version: 0.1.4.4
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pyapriltags>=3.3.0.3
 Requires-Dist: terminaltables>=3.1.10
-Requires-Dist: bdmc>=0.1.5.7
+Requires-Dist: bdmc>=0.1.5.8
 Requires-Dist: opencv-python-headless>=4.9.0.80
 Description-Content-Type: text/markdown
 
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
```

