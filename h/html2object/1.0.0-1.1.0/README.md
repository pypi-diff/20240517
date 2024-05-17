# Comparing `tmp/html2object-1.0.0.tar.gz` & `tmp/html2object-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2object-1.0.0.tar", last modified: Thu May 16 02:24:00 2024, max compression
+gzip compressed data, was "html2object-1.1.0.tar", last modified: Fri May 17 03:23:42 2024, max compression
```

## Comparing `html2object-1.0.0.tar` & `html2object-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:24:00.273376 html2object-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-16 02:23:51.000000 html2object-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-16 02:24:00.273376 html2object-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-16 02:23:51.000000 html2object-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:24:00.269375 html2object-1.0.0/html2object/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 02:23:51.000000 html2object-1.0.0/html2object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-16 02:23:51.000000 html2object-1.0.0/html2object/html2object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-16 02:23:51.000000 html2object-1.0.0/html2object/html_element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:24:00.273376 html2object-1.0.0/html2object.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-16 02:24:00.000000 html2object-1.0.0/html2object.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-16 02:24:00.000000 html2object-1.0.0/html2object.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:24:00.000000 html2object-1.0.0/html2object.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 02:24:00.000000 html2object-1.0.0/html2object.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:24:00.273376 html2object-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-16 02:23:51.000000 html2object-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:24:00.273376 html2object-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:23:51.000000 html2object-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-16 02:23:51.000000 html2object-1.0.0/tests/test_html2object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-16 02:23:51.000000 html2object-1.0.0/tests/test_html_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:23:42.306003 html2object-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-17 03:23:29.000000 html2object-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-17 03:23:42.306003 html2object-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-17 03:23:29.000000 html2object-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:23:42.302003 html2object-1.1.0/html2object/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-17 03:23:29.000000 html2object-1.1.0/html2object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-17 03:23:29.000000 html2object-1.1.0/html2object/html2object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-17 03:23:29.000000 html2object-1.1.0/html2object/html_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:23:42.306003 html2object-1.1.0/html2object.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-17 03:23:42.000000 html2object-1.1.0/html2object.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-17 03:23:42.000000 html2object-1.1.0/html2object.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:23:42.000000 html2object-1.1.0/html2object.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 03:23:42.000000 html2object-1.1.0/html2object.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:23:42.306003 html2object-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-17 03:23:29.000000 html2object-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:23:42.306003 html2object-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:23:29.000000 html2object-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-17 03:23:29.000000 html2object-1.1.0/tests/test_html2object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-17 03:23:29.000000 html2object-1.1.0/tests/test_html_element.py
```

### Comparing `html2object-1.0.0/LICENSE` & `html2object-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `html2object-1.0.0/PKG-INFO` & `html2object-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2object
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tools to handle the CRUD of .html files as objects.
 Home-page: https://github.com/boterop/html2object
 Author: boterop
 Author-email: boterop22@gmail.com
 Keywords: html,utils,html_utils,html_element,html_parser,html_writer,html_reader,html_crud,html_object,html_file,html_utils.py,html_element.py,html_parser.py,html_writer.py,html_reader.py,html_crud.py,html_object.py,html_file.py,html2object,html2object.py,html2object.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -63,22 +63,30 @@
 - Get element by id
 
   ```py
   image = document.get_element_by_id("image_id")
   image.add_attribute("src", "image_url")
   ```
 
-- Get element by id
+- Get elements by name
 
   ```py
   images = document.get_elements_by_name("image")
   for image in images:
     url_list.append(image.get_attribute("src"))
   ```
 
+- Get elements by class name
+
+  ```py
+  theme_element = document.get_elements_by_class_name("radix-themes")
+  for element in theme_element:
+    print(f"Main color: {element.get_attribute('data-accent-color')}")
+  ```
+
 ## Usage
 
 This project provides a way to manipulate HTML files and update them dynamically. Here's how you can use it:
 
 First, import the necessary classes from this project:
 
 ```sh
```

### Comparing `html2object-1.0.0/README.md` & `html2object-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,22 +42,30 @@
 - Get element by id
 
   ```py
   image = document.get_element_by_id("image_id")
   image.add_attribute("src", "image_url")
   ```
 
-- Get element by id
+- Get elements by name
 
   ```py
   images = document.get_elements_by_name("image")
   for image in images:
     url_list.append(image.get_attribute("src"))
   ```
 
+- Get elements by class name
+
+  ```py
+  theme_element = document.get_elements_by_class_name("radix-themes")
+  for element in theme_element:
+    print(f"Main color: {element.get_attribute('data-accent-color')}")
+  ```
+
 ## Usage
 
 This project provides a way to manipulate HTML files and update them dynamically. Here's how you can use it:
 
 First, import the necessary classes from this project:
 
 ```sh
```

### Comparing `html2object-1.0.0/html2object/html2object.py` & `html2object-1.1.0/html2object/html2object.py`

 * *Files identical despite different names*

### Comparing `html2object-1.0.0/html2object/html_element.py` & `html2object-1.1.0/html2object/html_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,24 @@
             elements.append(self)
         if self.children:
             for child in self.children:
                 if isinstance(child, HtmlElement):
                     elements.extend(child.get_elements_by_name(name))
         return elements
 
+    def get_elements_by_class_name(self, class_name: str) -> list:
+        elements = []
+        if "class" in self.attributes and class_name in self.get_attribute("class"):
+            elements.append(self)
+        if self.children:
+            for child in self.children:
+                if isinstance(child, HtmlElement):
+                    elements.extend(child.get_elements_by_class_name(class_name))
+        return elements
+
     def __str__(self) -> str:
         children_html = ""
         children = self.children or []
         for child in children:
             children_html += child if type(child) is str else str(child)
             children_html += "\n"
         children_html = children_html.strip()
```

### Comparing `html2object-1.0.0/html2object.egg-info/PKG-INFO` & `html2object-1.1.0/html2object.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2object
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tools to handle the CRUD of .html files as objects.
 Home-page: https://github.com/boterop/html2object
 Author: boterop
 Author-email: boterop22@gmail.com
 Keywords: html,utils,html_utils,html_element,html_parser,html_writer,html_reader,html_crud,html_object,html_file,html_utils.py,html_element.py,html_parser.py,html_writer.py,html_reader.py,html_crud.py,html_object.py,html_file.py,html2object,html2object.py,html2object.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -63,22 +63,30 @@
 - Get element by id
 
   ```py
   image = document.get_element_by_id("image_id")
   image.add_attribute("src", "image_url")
   ```
 
-- Get element by id
+- Get elements by name
 
   ```py
   images = document.get_elements_by_name("image")
   for image in images:
     url_list.append(image.get_attribute("src"))
   ```
 
+- Get elements by class name
+
+  ```py
+  theme_element = document.get_elements_by_class_name("radix-themes")
+  for element in theme_element:
+    print(f"Main color: {element.get_attribute('data-accent-color')}")
+  ```
+
 ## Usage
 
 This project provides a way to manipulate HTML files and update them dynamically. Here's how you can use it:
 
 First, import the necessary classes from this project:
 
 ```sh
```

### Comparing `html2object-1.0.0/setup.py` & `html2object-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="html2object",
-    version="1.0.0",
+    version="1.1.0",
     author="boterop",
     author_email="boterop22@gmail.com",
     description="Tools to handle the CRUD of .html files as objects.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/boterop/html2object",
     packages=find_packages(),
```

### Comparing `html2object-1.0.0/tests/test_html2object.py` & `html2object-1.1.0/tests/test_html2object.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 
     def test_get_child(self):
         html = "<div><span>Child</span></div>"
         child = get_child(html, name="div")
         self.assertEqual(child, "<span>Child</span>")
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `html2object-1.0.0/tests/test_html_element.py` & `html2object-1.1.0/tests/test_html_element.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,10 +105,16 @@
         element = HtmlElement(name="div", id="myDiv", attributes={"class": "container"})
         self.assertEqual(str(element), "<div id=myDiv class=container/>")
 
         element = HtmlElement(name="div")
         element.add_child("Hello, World!")
         self.assertEqual(str(element), "<div>Hello, World!</div>")
 
+    def test_get_elements_by_class_name(self):
+        document = HtmlElement(self.index_html)
+        elements = document.get_elements_by_class_name("radix-themes")
+        self.assertEqual(len(elements), 1)
+        self.assertEqual(elements[0].get_attribute("data-accent-color"), '"cyan"')
 
-if __name__ == "__main__":
+
+if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

