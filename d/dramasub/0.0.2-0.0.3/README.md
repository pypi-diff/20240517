# Comparing `tmp/dramasub-0.0.2.tar.gz` & `tmp/dramasub-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramasub-0.0.2.tar", last modified: Fri Apr  5 03:47:03 2024, max compression
+gzip compressed data, was "dramasub-0.0.3.tar", last modified: Fri May 17 06:31:25 2024, max compression
```

## Comparing `dramasub-0.0.2.tar` & `dramasub-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:47:03.612326 dramasub-0.0.2/
--rw-rw-rw-   0        0        0    34904 2024-03-07 08:39:12.000000 dramasub-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0     2170 2024-04-05 03:47:03.611327 dramasub-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1517 2024-04-05 03:20:27.000000 dramasub-0.0.2/README.md
--rw-rw-rw-   0        0        0      890 2024-04-05 03:44:37.000000 dramasub-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 03:47:03.612326 dramasub-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 03:47:03.588326 dramasub-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 03:47:03.594325 dramasub-0.0.2/src/dramasub/
--rw-rw-rw-   0        0        0        0 2024-02-25 01:53:58.000000 dramasub-0.0.2/src/dramasub/__init__.py
--rw-rw-rw-   0        0        0    16266 2024-04-05 02:14:25.000000 dramasub-0.0.2/src/dramasub/dramasub.py
--rw-rw-rw-   0        0        0      707 2024-04-05 01:15:53.000000 dramasub-0.0.2/src/dramasub/test.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:47:03.609326 dramasub-0.0.2/src/dramasub.egg-info/
--rw-rw-rw-   0        0        0     2170 2024-04-05 03:47:03.000000 dramasub-0.0.2/src/dramasub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-04-05 03:47:03.000000 dramasub-0.0.2/src/dramasub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:47:03.000000 dramasub-0.0.2/src/dramasub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-05 03:47:03.000000 dramasub-0.0.2/src/dramasub.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-05 03:47:03.000000 dramasub-0.0.2/src/dramasub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-05 03:47:03.000000 dramasub-0.0.2/src/dramasub.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 06:31:25.174975 dramasub-0.0.3/
+-rw-rw-rw-   0        0        0    34904 2024-03-07 08:39:12.000000 dramasub-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     2170 2024-05-17 06:31:25.172971 dramasub-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1517 2024-04-05 03:20:27.000000 dramasub-0.0.3/README.md
+-rw-rw-rw-   0        0        0      890 2024-05-17 06:00:37.000000 dramasub-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 06:31:25.174975 dramasub-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 06:31:25.121978 dramasub-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 06:31:25.145980 dramasub-0.0.3/src/dramasub/
+-rw-rw-rw-   0        0        0        0 2024-02-25 01:53:58.000000 dramasub-0.0.3/src/dramasub/__init__.py
+-rw-rw-rw-   0        0        0    18026 2024-05-17 06:29:26.000000 dramasub-0.0.3/src/dramasub/dramasub.py
+-rw-rw-rw-   0        0        0      529 2024-05-16 20:23:25.000000 dramasub-0.0.3/src/dramasub/test.py
+drwxrwxrwx   0        0        0        0 2024-05-17 06:31:25.171972 dramasub-0.0.3/src/dramasub.egg-info/
+-rw-rw-rw-   0        0        0     2170 2024-05-17 06:31:25.000000 dramasub-0.0.3/src/dramasub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2024-05-17 06:31:25.000000 dramasub-0.0.3/src/dramasub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 06:31:25.000000 dramasub-0.0.3/src/dramasub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-17 06:31:25.000000 dramasub-0.0.3/src/dramasub.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-17 06:31:25.000000 dramasub-0.0.3/src/dramasub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-17 06:31:25.000000 dramasub-0.0.3/src/dramasub.egg-info/top_level.txt
```

### Comparing `dramasub-0.0.2/LICENSE.md` & `dramasub-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dramasub-0.0.2/PKG-INFO` & `dramasub-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramasub
-Version: 0.0.2
+Version: 0.0.3
 Summary: script to generate accompanying visuals for voice dramas from .ass subtitle files
 Author: GenericTLAccount
 Project-URL: Homepage, https://github.com/GenericTLAccount/dramasub
 Keywords: drama cd,voice drama,subtitle,.ass,visuals
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dramasub-0.0.2/README.md` & `dramasub-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dramasub-0.0.2/pyproject.toml` & `dramasub-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dramasub"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="GenericTLAccount"},
 ]
 description = "script to generate accompanying visuals for voice dramas from .ass subtitle files"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["wand"]
```

### Comparing `dramasub-0.0.2/src/dramasub/dramasub.py` & `dramasub-0.0.3/src/dramasub/dramasub.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,18 +87,45 @@
         posy = int(font_dict["position_y"])
     except:
         print("Error: " + font_name + " has invalid position!")
         sys.exit(1)
     return [font,fill,pointsize,kerning,align,posx,posy]
 
 
-def layer_img2img(top_img, base_img, output_path):
+def parse_img_offset(img_layer, act_eff_str):
+    offset_x = 0
+    offset_y = 0
+    if "position_x" in img_layer:
+        try:
+            offset_x = int(img_layer["position_x"])
+        except:
+            print("Error: an image layer in " + act_eff_str + " has invalid x position set!")
+            print('Invalid position of "' + str(img_layer["position_x"]) + '"!')
+            sys.exit(1)
+    if "position_y" in img_layer:
+        try:
+            offset_y = int(img_layer["position_y"])
+        except:
+            print("Error: an image layer in " + act_eff_str + " has invalid y position set!")
+            print('Invalid position of "' + str(img_layer["position_y"]) + '"!')
+            sys.exit(1)
+    return [offset_x, offset_y]
+
+
+def layer_img2img(top_img, offset_x, offset_y, base_img, output_path):
     with Image(filename=base_img) as base:
         with Image(filename=top_img) as top:
-            base.composite(top)
+            base.composite(top, offset_x, offset_y)
+        base.save(filename=output_path)
+
+
+def layer_img2blank(top_img, offset_x, offset_y, res_w, res_h, output_path):
+    with Image(width=res_w, height=res_h) as base:
+        with Image(filename=top_img) as top:
+            base.composite(top, offset_x, offset_y)
         base.save(filename=output_path)
 
 
 def layer_txt2img(text, base_img, font_name, output_path):
     [font,fill,pointsize,kerning,align,posx,posy] = parse_font(font_name)
     with Image(filename=base_img) as img:
         draw_text(img,text,font,fill,pointsize,kerning,align,posx,posy)
@@ -126,15 +153,17 @@
             if i in actor_dict:
                 curr_layer = actor_dict[i]
                 if curr_layer and curr_layer["value"]:  # pass if either are None
                     curr_output = kitchen_path / (cook_fn + str(cook_count) + ".png")
                     curr_type = curr_layer["type"]
                     if cook_on_stack:
                         if curr_type == "img":
-                            layer_img2img(curr_layer["value"], curr_output, curr_output)
+                            [offset_x, offset_y] = parse_img_offset(curr_layer, act_eff_str)
+                            layer_img2img(curr_layer["value"], offset_x, offset_y, curr_output, \
+                                           curr_output)
                             last_eff = "img"
                             has_cooked = True
                         elif curr_type == "txt":
                             layer_txt2img(curr_layer["value"], curr_output, curr_layer["font"], \
                                             curr_output)
                             last_eff = "txt"
                             has_cooked = True
@@ -146,21 +175,29 @@
                             last_eff = "ff"
                             cook_on_stack = False
                         else:
                             print('Error: "' + curr_layer + '" of "' + act_eff_str + 'does not have value \
                                 "img", "txt", or "ff"!')
                             sys.exit(1)
                     else:
-                        if curr_type == "img" and stack_len == 1:
-                            cooked_list.append(curr_layer["value"])
-                            last_eff = "img"
-                        elif curr_type == "img":    # probably shouldn't do this but lazy
-                            shutil.copyfile(curr_layer["value"], curr_output)
-                            last_eff = "img"
-                            has_cooked = True
+                        if curr_type == "img":
+                            [offset_x, offset_y] = parse_img_offset(curr_layer, act_eff_str)
+                            if offset_x != 0 or offset_y != 0:
+                                layer_img2blank(curr_layer["value"], offset_x, offset_y, res_w, res_h, \
+                                                curr_output)
+                                last_eff = "img"
+                                has_cooked = True
+                            else:
+                                if stack_len == 1:
+                                    cooked_list.append(curr_layer["value"])
+                                    last_eff = "img"
+                                else:    # probably shouldn't do this but lazy
+                                    shutil.copyfile(curr_layer["value"], curr_output)
+                                    last_eff = "img"
+                                    has_cooked = True
                         elif curr_type == "ff":
                             cooked_list.append(curr_layer["ff"])
                             last_eff = "ff"
                         elif curr_type == "txt":
                             layer_txt2blank(curr_layer["value"], curr_layer["font"], res_w, res_h, curr_output)
                             last_eff = "txt"
                             has_cooked = True
```

### Comparing `dramasub-0.0.2/src/dramasub.egg-info/PKG-INFO` & `dramasub-0.0.3/src/dramasub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramasub
-Version: 0.0.2
+Version: 0.0.3
 Summary: script to generate accompanying visuals for voice dramas from .ass subtitle files
 Author: GenericTLAccount
 Project-URL: Homepage, https://github.com/GenericTLAccount/dramasub
 Keywords: drama cd,voice drama,subtitle,.ass,visuals
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

