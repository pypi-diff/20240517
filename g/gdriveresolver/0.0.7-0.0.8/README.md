# Comparing `tmp/gdriveresolver-0.0.7.tar.gz` & `tmp/gdriveresolver-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdriveresolver-0.0.7.tar", last modified: Wed May 15 22:00:01 2024, max compression
+gzip compressed data, was "gdriveresolver-0.0.8.tar", last modified: Fri May 17 19:42:59 2024, max compression
```

## Comparing `gdriveresolver-0.0.7.tar` & `gdriveresolver-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-15 22:00:01.742163 gdriveresolver-0.0.7/
--rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.7/LICENSE
--rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-15 22:00:01.742008 gdriveresolver-0.0.7/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)      972 2024-05-14 21:11:01.000000 gdriveresolver-0.0.7/README.md
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-15 22:00:01.740959 gdriveresolver-0.0.7/gdriveresolver/
--rw-r--r--   0 harman     (501) staff       (20)       37 2024-05-14 21:11:01.000000 gdriveresolver-0.0.7/gdriveresolver/__init__.py
--rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.7/gdriveresolver/exceptions.py
--rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-15 16:16:16.000000 gdriveresolver-0.0.7/gdriveresolver/model.py
--rw-r--r--   0 harman     (501) staff       (20)     1894 2024-05-15 21:58:42.000000 gdriveresolver-0.0.7/gdriveresolver/resolver.py
--rw-r--r--   0 harman     (501) staff       (20)     2897 2024-05-15 16:16:16.000000 gdriveresolver-0.0.7/gdriveresolver/system_operations.py
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-15 22:00:01.741851 gdriveresolver-0.0.7/gdriveresolver.egg-info/
--rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-15 22:00:01.000000 gdriveresolver-0.0.7/gdriveresolver.egg-info/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)      357 2024-05-15 22:00:01.000000 gdriveresolver-0.0.7/gdriveresolver.egg-info/SOURCES.txt
--rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-15 22:00:01.000000 gdriveresolver-0.0.7/gdriveresolver.egg-info/dependency_links.txt
--rw-r--r--   0 harman     (501) staff       (20)       15 2024-05-15 22:00:01.000000 gdriveresolver-0.0.7/gdriveresolver.egg-info/top_level.txt
--rw-r--r--   0 harman     (501) staff       (20)      683 2024-05-15 21:59:40.000000 gdriveresolver-0.0.7/pyproject.toml
--rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-15 22:00:01.742195 gdriveresolver-0.0.7/setup.cfg
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-15 22:00:01.741550 gdriveresolver-0.0.7/tests/
--rw-r--r--   0 harman     (501) staff       (20)     4547 2024-05-15 20:03:13.000000 gdriveresolver-0.0.7/tests/test_gdrive_resolver.py
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-17 19:42:59.135723 gdriveresolver-0.0.8/
+-rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.8/LICENSE
+-rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-17 19:42:59.135553 gdriveresolver-0.0.8/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      972 2024-05-14 21:11:01.000000 gdriveresolver-0.0.8/README.md
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-17 19:42:59.134575 gdriveresolver-0.0.8/gdriveresolver/
+-rw-r--r--   0 harman     (501) staff       (20)       37 2024-05-14 21:11:01.000000 gdriveresolver-0.0.8/gdriveresolver/__init__.py
+-rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.8/gdriveresolver/exceptions.py
+-rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-15 16:16:16.000000 gdriveresolver-0.0.8/gdriveresolver/model.py
+-rw-r--r--   0 harman     (501) staff       (20)     2210 2024-05-17 19:42:15.000000 gdriveresolver-0.0.8/gdriveresolver/resolver.py
+-rw-r--r--   0 harman     (501) staff       (20)     2897 2024-05-15 16:16:16.000000 gdriveresolver-0.0.8/gdriveresolver/system_operations.py
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-17 19:42:59.135392 gdriveresolver-0.0.8/gdriveresolver.egg-info/
+-rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-17 19:42:59.000000 gdriveresolver-0.0.8/gdriveresolver.egg-info/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      357 2024-05-17 19:42:59.000000 gdriveresolver-0.0.8/gdriveresolver.egg-info/SOURCES.txt
+-rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-17 19:42:59.000000 gdriveresolver-0.0.8/gdriveresolver.egg-info/dependency_links.txt
+-rw-r--r--   0 harman     (501) staff       (20)       15 2024-05-17 19:42:59.000000 gdriveresolver-0.0.8/gdriveresolver.egg-info/top_level.txt
+-rw-r--r--   0 harman     (501) staff       (20)      683 2024-05-17 19:42:32.000000 gdriveresolver-0.0.8/pyproject.toml
+-rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-17 19:42:59.135755 gdriveresolver-0.0.8/setup.cfg
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-17 19:42:59.135234 gdriveresolver-0.0.8/tests/
+-rw-r--r--   0 harman     (501) staff       (20)     4125 2024-05-17 19:35:49.000000 gdriveresolver-0.0.8/tests/test_gdrive_resolver.py
```

### Comparing `gdriveresolver-0.0.7/LICENSE` & `gdriveresolver-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.7/PKG-INFO` & `gdriveresolver-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gdriveresolver-0.0.7/README.md` & `gdriveresolver-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.7/gdriveresolver/model.py` & `gdriveresolver-0.0.8/gdriveresolver/model.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.7/gdriveresolver/resolver.py` & `gdriveresolver-0.0.8/gdriveresolver/resolver.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,31 +19,37 @@
             must_resolve (bool): Whether to raise an error if the file is not found.
 
         Returns:
             Optional[str]: The absolute path if found, else None.
         """
         as_path = Path(path_to_resolve)
 
+        sanitized_path = self.os_type.sanitize_path(path_to_resolve)
+
         # Case 1: If Google Drive path is resolved, check path relative to Google Drive
         if self.drive_path:
-            sanitized_path = self.os_type.sanitize_path(path_to_resolve)
             absolute_path = self.drive_path / sanitized_path
             if absolute_path.exists():
                 return str(absolute_path)
 
         # Case 2: Google Drive path is not resolved, check against absolute path
         if as_path.is_absolute() and as_path.exists():
             return str(as_path)
 
         # Case 3: If Google Drive path is not resolved, check path relative to root search paths
         for root in self.os_type.root_search_paths:
             potential_path = root / as_path
             if potential_path.exists():
                 return str(potential_path)
 
+        # Case 4: User is resolving a stem rather than a full name, so allow it to return to user if they have specified
+        # that it does not need to resolve, and the user can modify the path with the appropriate extension(s)
+        if not must_resolve:
+            return str(self.drive_path / sanitized_path)
+
         return _terminate(must_resolve)
 
 
 def _terminate(must_resolve: bool) -> None:
     if must_resolve:
         raise FileNotFoundError("File not found.")
     print("File not found.")
```

### Comparing `gdriveresolver-0.0.7/gdriveresolver/system_operations.py` & `gdriveresolver-0.0.8/gdriveresolver/system_operations.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.7/gdriveresolver.egg-info/PKG-INFO` & `gdriveresolver-0.0.8/gdriveresolver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gdriveresolver-0.0.7/pyproject.toml` & `gdriveresolver-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gdriveresolver"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="C Harman", email="charman@netrias.com" },
 ]
 description = "A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gdriveresolver-0.0.7/tests/test_gdrive_resolver.py` & `gdriveresolver-0.0.8/tests/test_gdrive_resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,49 +59,40 @@
     def test_resolve_relative_to_root_search_paths(self, mock_get_os):
         """
         Given a relative path
         When the Google Drive path is not resolved
         Then it should check the path relative to root search paths
         """
         # Given
-        mock_os = MagicMock()
-        mock_get_os.return_value = mock_os
-        mock_os.root_search_paths = [Path('/mock/root1'), Path('/mock/root2')]
         self.resolver.drive_path = None
 
         path = 'relative/path/to/file.txt'
         expected_path = '/relative/path/to/file.txt'
 
         # When
         with patch.object(Path, 'is_absolute', return_value=False):
             with patch.object(Path, 'exists', side_effect=[True, False]):
                 result = self.resolver.resolve(path)
 
         # Then
         assert result == expected_path
 
-    @patch('gdriveresolver.resolver.locate_google_drive')
-    @patch('gdriveresolver.resolver.get_operating_system')
-    def test_file_not_found_must_resolve(self, mock_get_os, mock_locate_drive):
+    def test_file_not_found_must_resolve(self):
         """
         Given a non-existent file
         When must_resolve is True
         Then it should raise a FileNotFoundError
         """
         # Given
-        mock_os = MagicMock()
-        mock_get_os.return_value = mock_os
-        mock_os.root_search_paths = [Path('/mock/root1'), Path('/mock/root2')]
-        mock_locate_drive.return_value = None
-
         path = 'nonexistent/file.txt'
 
         # When
         with patch.object(Path, 'is_absolute', return_value=False):
             with patch.object(Path, 'exists', return_value=False):
+                # Then
                 with self.assertRaises(FileNotFoundError):
                     self.resolver.resolve(path, must_resolve=True)
 
     @patch('gdriveresolver.resolver.locate_google_drive')
     @patch('gdriveresolver.resolver.get_operating_system')
     def test_file_not_found_no_must_resolve(self, mock_get_os, mock_locate_drive):
         """
@@ -110,21 +101,21 @@
         Then it should return None
         """
         # Given
         mock_os = MagicMock()
         mock_get_os.return_value = mock_os
         mock_os.root_search_paths = [Path('/mock/root1'), Path('/mock/root2')]
         mock_locate_drive.return_value = None
+        self.resolver.drive_path = Path("")
 
         path = 'nonexistent/file.txt'
 
         # When
         with patch.object(Path, 'is_absolute', return_value=False):
             with patch.object(Path, 'exists', return_value=False):
                 result = self.resolver.resolve(path, must_resolve=False)
-
-        # Then
-        self.assertIsNone(result)
+                # Then
+                assert result == path
 
 
 if __name__ == '__main__':
     unittest.main()
```

