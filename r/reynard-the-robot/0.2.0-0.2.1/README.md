# Comparing `tmp/reynard_the_robot-0.2.0-py3-none-any.whl.zip` & `tmp/reynard_the_robot-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 30407 bytes, number of entries: 20
+Zip file size: 30570 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat       49 b- defN 24-Feb-16 20:52 reynard_the_robot/__init__.py
 -rw-rw-rw-  2.0 fat       64 b- defN 24-Feb-19 04:34 reynard_the_robot/__main__.py
--rw-rw-rw-  2.0 fat     4959 b- defN 24-Feb-19 03:30 reynard_the_robot/ascii_socket.py
+-rw-rw-rw-  2.0 fat     5461 b- defN 24-May-17 04:17 reynard_the_robot/ascii_socket.py
 -rw-rw-rw-  2.0 fat     1695 b- defN 24-Feb-19 05:16 reynard_the_robot/gui.py
 -rw-rw-rw-  2.0 fat     2866 b- defN 24-Feb-19 05:46 reynard_the_robot/main.py
--rw-rw-rw-  2.0 fat    20341 b- defN 24-May-01 03:17 reynard_the_robot/reynard.py
+-rw-rw-rw-  2.0 fat    20823 b- defN 24-May-17 04:16 reynard_the_robot/reynard.py
 -rw-rw-rw-  2.0 fat     4852 b- defN 24-May-01 03:17 reynard_the_robot/robotraconteur.py
 -rw-rw-rw-  2.0 fat     5980 b- defN 24-Feb-16 04:35 reynard_the_robot/web_static/app.js
 -rw-rw-rw-  2.0 fat     2560 b- defN 24-Feb-19 03:40 reynard_the_robot/web_static/index.html
 -rw-rw-rw-  2.0 fat     3234 b- defN 24-Feb-07 04:44 reynard_the_robot/web_static/reynard_arm_link.svg
 -rw-rw-rw-  2.0 fat     5933 b- defN 24-Feb-08 04:28 reynard_the_robot/web_static/reynard_body.svg
 -rw-rw-rw-  2.0 fat     3092 b- defN 24-Feb-08 05:52 reynard_the_robot/web_static/reynard_tool.svg
 -rw-rw-rw-  2.0 fat     4286 b- defN 24-Feb-19 04:21 reynard_the_robot/web_static/rricon.ico
 -rw-rw-rw-  2.0 fat      340 b- defN 24-Feb-19 03:39 reynard_the_robot/web_static/rricon.png
 -rw-rw-rw-  2.0 fat      646 b- defN 24-Feb-08 02:22 reynard_the_robot/web_static/style.css
--rw-rw-rw-  2.0 fat    11554 b- defN 24-May-01 03:33 reynard_the_robot-0.2.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    20720 b- defN 24-May-01 03:33 reynard_the_robot-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-01 03:33 reynard_the_robot-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 24-May-01 03:33 reynard_the_robot-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1824 b- defN 24-May-01 03:33 reynard_the_robot-0.2.0.dist-info/RECORD
-20 files, 95105 bytes uncompressed, 27375 bytes compressed:  71.2%
+-rw-rw-rw-  2.0 fat    11554 b- defN 24-May-17 04:18 reynard_the_robot-0.2.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    20720 b- defN 24-May-17 04:18 reynard_the_robot-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-17 04:18 reynard_the_robot-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 24-May-17 04:18 reynard_the_robot-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1824 b- defN 24-May-17 04:18 reynard_the_robot-0.2.1.dist-info/RECORD
+20 files, 96089 bytes uncompressed, 27538 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: reynard_the_robot/web_static/rricon.png
 Comment: 
 
 Filename: reynard_the_robot/web_static/style.css
 Comment: 
 
-Filename: reynard_the_robot-0.2.0.dist-info/LICENSE.txt
+Filename: reynard_the_robot-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: reynard_the_robot-0.2.0.dist-info/METADATA
+Filename: reynard_the_robot-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: reynard_the_robot-0.2.0.dist-info/WHEEL
+Filename: reynard_the_robot-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: reynard_the_robot-0.2.0.dist-info/top_level.txt
+Filename: reynard_the_robot-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: reynard_the_robot-0.2.0.dist-info/RECORD
+Filename: reynard_the_robot-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reynard_the_robot/ascii_socket.py

```diff
@@ -52,25 +52,37 @@
                     assert len(s1) == 4
                     q1 = float(s1[1])
                     q2 = float(s1[2])
                     q3 = float(s1[3])
                     self._reynard.set_arm_position(q1, q2, q3)
                     ret = "OK\n"
                 elif s1[0] == "DRIVE":
-                    assert len(s1) == 3
+                    assert len(s1) >= 3
                     vel_x = float(s1[1])
                     vel_y = float(s1[2])
-                    self._reynard.drive_robot(vel_x, vel_y)
+                    timeout = -1
+                    if len(s1) >= 4:
+                        timeout = float(s1[3])
+                    wait = False
+                    if len(s1) >= 5:
+                        wait = bool(s1[4])
+                    self._reynard.drive_robot(vel_x, vel_y, timeout, wait)
                     ret = "OK\n"
                 elif s1[0] == "DRIVEARM":
-                    assert len(s1) == 4
+                    assert len(s1) >= 4
                     q1 = float(s1[1])
                     q2 = float(s1[2])
                     q3 = float(s1[3])
-                    self._reynard.drive_arm(q1, q2, q3)
+                    timeout = -1
+                    if len(s1) >= 5:
+                        timeout = float(s1[4])
+                    wait = False
+                    if len(s1) >= 6:
+                        wait = bool(s1[5])
+                    self._reynard.drive_arm(q1, q2, q3, timeout, wait)
                     ret = "OK\n"
                 elif s1[0] == "STATE":
                     assert len(s1) == 1
                     t = self._reynard.time
                     p = self._reynard.robot_position
                     a = self._reynard.arm_position
                     ret = f"STATE {t} {p[0]} {p[1]} {a[0]} {a[1]} {a[2]}\n"
```

## reynard_the_robot/reynard.py

```diff
@@ -419,40 +419,50 @@
             await self.aio_set_arm_position(q1, q2, q3)
             return web.Response()
         
         async def api_post_drive_robot(request):
             json = await request.json()
             vel_x = json["vel_x"]
             vel_y = json["vel_y"]
-            await self.aio_drive_robot(vel_x, vel_y)
+            timeout = float(json.get("timeout", -1))
+            wait = bool(json.get("wait", False))
+            await self.aio_drive_robot(vel_x, vel_y, timeout, wait)
             return web.Response()
         
         async def api_post_drive_arm(request):
             json = await request.json()
             q1 = json["q1"]
             q2 = json["q2"]
             q3 = json["q3"]
-            await self.aio_drive_arm(q1, q2, q3)
+            timeout = float(json.get("timeout", -1))
+            wait = bool(json.get("wait", False))
+            await self.aio_drive_arm(q1, q2, q3, timeout, wait)
             return web.Response()
         
         async def api_post_color(request):
             json = await request.json()
             r = json["r"]
             g = json["g"]
             b = json["b"]
             await self.aio_set_color(r, g, b)
             return web.Response()
         
         async def api_get_state(request):
             res = {
+                "time": self.time,
                 "x": self._pos[0],
                 "y": self._pos[1],
                 "q1": self._q[0],
                 "q2": self._q[1],
                 "q3": self._q[2],
+                "vel_x": self._vel[0],
+                "vel_y": self._vel[1],
+                "vel_q1": self._q_vel[0],
+                "vel_q2": self._q_vel[1],
+                "vel_q3": self._q_vel[2]
             }
             return web.json_response(res)
         
         async def api_get_color(request):
             res = {
                 "r": self._color[0],
                 "g": self._color[1],
```

## Comparing `reynard_the_robot-0.2.0.dist-info/LICENSE.txt` & `reynard_the_robot-0.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `reynard_the_robot-0.2.0.dist-info/METADATA` & `reynard_the_robot-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reynard-the-robot
-Version: 0.2.0
+Version: 0.2.1
 Summary: Reyndard the Robot Raconteur educational Robot
 Author-email: John Wason <wason@wasontech.com>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

## Comparing `reynard_the_robot-0.2.0.dist-info/RECORD` & `reynard_the_robot-0.2.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 reynard_the_robot/__init__.py,sha256=Lh8k1Cp_vTHr8jrYspxmCuviwnc4yD3xBLMb_qYngOA,49
 reynard_the_robot/__main__.py,sha256=hFzZjadLlcOuoLM7D8wFiFVO8mqF7vMuo9y-9xfIhRc,64
-reynard_the_robot/ascii_socket.py,sha256=tPpcwwLHUnD9cfH7RpDANLV3cUqRmK_4Vj3J4rWTfyc,4959
+reynard_the_robot/ascii_socket.py,sha256=ATtJgrH6b6xApINw1LsI4qLULFSnufmgm1Cgs5z_bNg,5461
 reynard_the_robot/gui.py,sha256=4GGuhPD_0fcg7DSyX9s98o7tuMTae5xSKd6PgxhAQqo,1695
 reynard_the_robot/main.py,sha256=e5Bt5i-mgGwsPyIIwlZxQFoSCr4yaGIlJgWhRihoRT8,2866
-reynard_the_robot/reynard.py,sha256=or8o7JNXB-Gtoi-fAJKFehwK_XIxD42JW8YBrPFq8yo,20341
+reynard_the_robot/reynard.py,sha256=zrHqQ2l8Dm5JIyzFPieMqLA0IJYKgBNpY-fHTLsP4Ak,20823
 reynard_the_robot/robotraconteur.py,sha256=YfE_CynsGfxklhGdoVDV074IGUtEaF5T9-sK6ELgC9g,4852
 reynard_the_robot/web_static/app.js,sha256=2CLEPb1mn-1dy_jvP3SOdQpLrDL8iM91AxmzqrRqdaI,5980
 reynard_the_robot/web_static/index.html,sha256=a5Vg4QJD1tdEdkx6JbDZhPPand9fp4QZ4F4mBVLjS1o,2560
 reynard_the_robot/web_static/reynard_arm_link.svg,sha256=JC3GWRGmjQRdzrMIuT_2zAqr1pDRd5fVRmelXjidTJk,3234
 reynard_the_robot/web_static/reynard_body.svg,sha256=L0_yKddlqcASYX3DqLgDIie5Z1X0EL9rHbAv7J4QdrM,5933
 reynard_the_robot/web_static/reynard_tool.svg,sha256=McejHY1MtYfY-fN5u2hifqI1XMwysvmVKjj8gQF0xlY,3092
 reynard_the_robot/web_static/rricon.ico,sha256=TgJ6A1w-1wUoQ3Qq3Ct-10ctFSNdNTMDu9y1vLlyCFE,4286
 reynard_the_robot/web_static/rricon.png,sha256=1FkN-Q66Pc91I8IrTGPmYoLIeCCchp08pGrrNbkFhBI,340
 reynard_the_robot/web_static/style.css,sha256=2ETT6VVwBCrG1NDk4_plBsOrgshN6Rv4r5n2DisVws0,646
-reynard_the_robot-0.2.0.dist-info/LICENSE.txt,sha256=Tl1tRxWGtrUEp-8aQr9k8kNBVeVc0FnOcSY8m7eKPfc,11554
-reynard_the_robot-0.2.0.dist-info/METADATA,sha256=T8DtIek8W8CJmLs49GCapnr-Ag5-vipk1FqH0r_T48o,20720
-reynard_the_robot-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-reynard_the_robot-0.2.0.dist-info/top_level.txt,sha256=0stdw0pwkwSnxcFlc8IImz5lmbItFyZHF6R7Aa1Vu6Y,18
-reynard_the_robot-0.2.0.dist-info/RECORD,,
+reynard_the_robot-0.2.1.dist-info/LICENSE.txt,sha256=Tl1tRxWGtrUEp-8aQr9k8kNBVeVc0FnOcSY8m7eKPfc,11554
+reynard_the_robot-0.2.1.dist-info/METADATA,sha256=oF3CNmk_iem-G_YNdAazYmi8XTFPmmjPuD1FL8ebDlk,20720
+reynard_the_robot-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+reynard_the_robot-0.2.1.dist-info/top_level.txt,sha256=0stdw0pwkwSnxcFlc8IImz5lmbItFyZHF6R7Aa1Vu6Y,18
+reynard_the_robot-0.2.1.dist-info/RECORD,,
```

