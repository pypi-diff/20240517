# Comparing `tmp/pathtemplate-0.1.1.tar.gz` & `tmp/pathtemplate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathtemplate-0.1.1.tar", last modified: Sun Feb 18 13:42:45 2024, max compression
+gzip compressed data, was "pathtemplate-0.1.2.tar", last modified: Fri May 17 10:26:19 2024, max compression
```

## Comparing `pathtemplate-0.1.1.tar` & `pathtemplate-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 voitek     (501) staff       (20)        0 2024-02-18 13:42:45.338913 pathtemplate-0.1.1/
--rw-r--r--   0 voitek     (501) staff       (20)      248 2024-02-18 13:42:45.338540 pathtemplate-0.1.1/PKG-INFO
--rw-r--r--   0 voitek     (501) staff       (20)       15 2024-02-08 12:02:25.000000 pathtemplate-0.1.1/README.md
--rw-r--r--   0 voitek     (501) staff       (20)      506 2024-02-17 00:21:58.000000 pathtemplate-0.1.1/pyproject.toml
--rw-r--r--   0 voitek     (501) staff       (20)       38 2024-02-18 13:42:45.338979 pathtemplate-0.1.1/setup.cfg
-drwxr-xr-x   0 voitek     (501) staff       (20)        0 2024-02-18 13:42:45.306492 pathtemplate-0.1.1/src/
--rw-r--r--   0 voitek     (501) staff       (20)        0 2024-02-08 12:02:25.000000 pathtemplate-0.1.1/src/__init__.py
-drwxr-xr-x   0 voitek     (501) staff       (20)        0 2024-02-18 13:42:45.338141 pathtemplate-0.1.1/src/pathtemplate.egg-info/
--rw-r--r--   0 voitek     (501) staff       (20)      248 2024-02-18 13:42:45.000000 pathtemplate-0.1.1/src/pathtemplate.egg-info/PKG-INFO
--rw-r--r--   0 voitek     (501) staff       (20)      247 2024-02-18 13:42:45.000000 pathtemplate-0.1.1/src/pathtemplate.egg-info/SOURCES.txt
--rw-r--r--   0 voitek     (501) staff       (20)        1 2024-02-18 13:42:45.000000 pathtemplate-0.1.1/src/pathtemplate.egg-info/dependency_links.txt
--rw-r--r--   0 voitek     (501) staff       (20)       22 2024-02-18 13:42:45.000000 pathtemplate-0.1.1/src/pathtemplate.egg-info/top_level.txt
--rw-r--r--   0 voitek     (501) staff       (20)     3507 2024-02-08 12:49:20.000000 pathtemplate-0.1.1/src/pathtemplate.py
-drwxr-xr-x   0 voitek     (501) staff       (20)        0 2024-02-18 13:42:45.332299 pathtemplate-0.1.1/tests/
--rw-r--r--   0 voitek     (501) staff       (20)     2264 2024-02-08 12:53:07.000000 pathtemplate-0.1.1/tests/test_pathtemplate.py
+drwxr-xr-x   0 voitek     (501) staff       (20)        0 2024-05-17 10:26:19.507352 pathtemplate-0.1.2/
+-rw-r--r--   0 voitek     (501) staff       (20)      248 2024-05-17 10:26:19.506722 pathtemplate-0.1.2/PKG-INFO
+-rw-r--r--   0 voitek     (501) staff       (20)       15 2024-02-08 12:02:25.000000 pathtemplate-0.1.2/README.md
+-rw-r--r--   0 voitek     (501) staff       (20)      502 2024-05-17 10:17:19.000000 pathtemplate-0.1.2/pyproject.toml
+-rw-r--r--   0 voitek     (501) staff       (20)       38 2024-05-17 10:26:19.507457 pathtemplate-0.1.2/setup.cfg
+drwxr-xr-x   0 voitek     (501) staff       (20)        0 2024-05-17 10:26:19.504273 pathtemplate-0.1.2/src/
+-rw-r--r--   0 voitek     (501) staff       (20)        0 2024-02-08 12:02:25.000000 pathtemplate-0.1.2/src/__init__.py
+drwxr-xr-x   0 voitek     (501) staff       (20)        0 2024-05-17 10:26:19.506162 pathtemplate-0.1.2/src/pathtemplate.egg-info/
+-rw-r--r--   0 voitek     (501) staff       (20)      248 2024-05-17 10:26:19.000000 pathtemplate-0.1.2/src/pathtemplate.egg-info/PKG-INFO
+-rw-r--r--   0 voitek     (501) staff       (20)      247 2024-05-17 10:26:19.000000 pathtemplate-0.1.2/src/pathtemplate.egg-info/SOURCES.txt
+-rw-r--r--   0 voitek     (501) staff       (20)        1 2024-05-17 10:26:19.000000 pathtemplate-0.1.2/src/pathtemplate.egg-info/dependency_links.txt
+-rw-r--r--   0 voitek     (501) staff       (20)       22 2024-05-17 10:26:19.000000 pathtemplate-0.1.2/src/pathtemplate.egg-info/top_level.txt
+-rw-r--r--   0 voitek     (501) staff       (20)     4276 2024-05-17 09:51:53.000000 pathtemplate-0.1.2/src/pathtemplate.py
+drwxr-xr-x   0 voitek     (501) staff       (20)        0 2024-05-17 10:26:19.505669 pathtemplate-0.1.2/tests/
+-rw-r--r--   0 voitek     (501) staff       (20)     3360 2024-05-17 09:56:44.000000 pathtemplate-0.1.2/tests/test_pathtemplate.py
```

### Comparing `pathtemplate-0.1.1/src/pathtemplate.py` & `pathtemplate-0.1.2/src/pathtemplate.py`

 * *Files 23% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
     def __truediv__(self, other: Union[str, "PathTemplate"]) -> "PathTemplate":
         """
         Concatenate paths
         """
         if isinstance(other, str):
             other = PathTemplate(other)
+
         return PathTemplate(str(self._path / other._path), **self._params)
 
     @property
     def template(self) -> str:
         """
         Return template string
         """
@@ -88,24 +89,46 @@
         c = PathTemplate("model/{var}.rpn")
         c.copy(var="o3")
         """
         c = PathTemplate(self._template, **self._params)
         c.update(**kwargs)
         return c
 
+    def join_format_spec(self, literal_text, field_name, format_spec, conversion):
+        if field_name is None:
+            return literal_text
+
+        if format_spec is None or format_spec == "":
+            spec = ""
+        else:
+            spec = f":{format_spec}"
+        
+        conversion = "" if conversion is None else f"!{conversion}"
+        return f"{literal_text}{{{field_name}{spec}{conversion}}}"
+    
+
     def update_pathstring(self) -> NoReturn:
         """
         Update path string
         """
-        try:
-            self._pathstring = self._formatter.format(self._template, **self._params)
-        except KeyError as e:
-            raise KeyError(f"Value for placeholder {e} not provided.")
+        # if some placeholders are missing, fill them with the same name in brackets
+
+        chunks = list(self._formatter.parse(self._template))
+        new_chunks = []
+
+        for literal_text, field_name, format_spec, conversion in chunks:
+            chunk = self.join_format_spec(literal_text, field_name, format_spec, conversion)
+            if field_name in self._params:
+                chunk = self._formatter.format(chunk, **self._params)
+            new_chunks.append(chunk)
+        
+        self._pathstring = "".join(new_chunks)
         self._path = pathlib.Path(self._pathstring)
 
+
     def update(self, **kwargs: Dict[str, Any]) -> "PathTemplate":
         """
         Update template arguments
         """
         self._params.update(kwargs)
         self.update_pathstring()
         return self
```

### Comparing `pathtemplate-0.1.1/tests/test_pathtemplate.py` & `pathtemplate-0.1.2/tests/test_pathtemplate.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         path = PathTemplate(
             template, datetime=dt.datetime(2020, 1, 1, 12), var="o3"
         )
         assert str(path) == "file_202001_o3.txt"
 
     def test_pathtemplate_emptyvalue(self):
         template = "file_{datetime:%Y%m}_{var}.txt"
-        with pytest.raises(KeyError):
-            path = PathTemplate(template, datetime=dt.datetime(2020, 1, 1, 12))
+        path = PathTemplate(template, datetime=dt.datetime(2020, 1, 1, 12))
+        assert str(path) == "file_202001_{var}.txt"
 
     def test_pathtemplate_update(self):
         template = "file_{datetime:%Y%m}_{var}.txt"
         path = PathTemplate(template, datetime=dt.datetime(2020, 1, 1, 12), var="o3")
         path.update(datetime=dt.datetime(2021, 1, 1, 12), var="temp")
         assert str(path) == "file_202101_temp.txt"
 
@@ -57,7 +57,37 @@
 
     def test_pathtemplate_copy(self):
         template = "file_{var}"
         path = PathTemplate(template, var="o3")
         path2 = path.copy()
         assert str(path2) == "file_o3"
         assert path2 is not path
+
+    def test_pathtemplate_noargs(self):
+        template = "file_{var}"
+        path = PathTemplate(template)
+        assert str(path) == "file_{var}"
+
+    def test_pathtemplate_noargs_with_float(self):
+        template = "file_{var}_{value:.2f}"
+        path = PathTemplate(template)
+        assert str(path) == "file_{var}_{value:.2f}"
+
+    def test_pathtemplate_template_noargs_with_float(self):
+        template = "file_{var}_{value:.2f}"
+        path = PathTemplate(template)
+        assert path._template == "file_{var}_{value:.2f}"
+
+    def test_pathtemplate_template_with_float(self):
+        template = "file_{var}_{value:.2f}"
+        path = PathTemplate(template, value=3.14159)
+        assert str(path) == "file_{var}_3.14"
+
+    def test_noargs_with_conversion(self):
+        template = "file_{var!e}"
+        path = PathTemplate(template)
+        assert str(path) == "file_{var!e}"
+
+    def test_pathtemplate_noargs_with_datetime(self):
+        template = "file_{datetime:%Y%m%d}"
+        path = PathTemplate(template)
+        assert str(path) == "file_{datetime:%Y%m%d}"
```

