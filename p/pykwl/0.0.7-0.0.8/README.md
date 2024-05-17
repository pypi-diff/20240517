# Comparing `tmp/pykwl-0.0.7.tar.gz` & `tmp/pykwl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykwl-0.0.7.tar", last modified: Mon Apr 29 10:31:46 2024, max compression
+gzip compressed data, was "pykwl-0.0.8.tar", last modified: Thu May  9 10:17:11 2024, max compression
```

## Comparing `pykwl-0.0.7.tar` & `pykwl-0.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-29 10:31:36.000000 pykwl-0.0.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-29 10:31:36.000000 pykwl-0.0.7/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 10:31:36.000000 pykwl-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-29 10:31:36.000000 pykwl-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 10:31:46.184571 pykwl-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-29 10:31:36.000000 pykwl-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 10:31:36.000000 pykwl-0.0.7/cmake/configure_ccache.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 10:31:36.000000 pykwl-0.0.7/dependencies/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/dependencies/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-29 10:31:36.000000 pykwl-0.0.7/dependencies/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.180570 pykwl-0.0.7/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/include/wl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/include/wl/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-29 10:31:36.000000 pykwl-0.0.7/include/wl/details/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-29 10:31:36.000000 pykwl-0.0.7/include/wl/details/weisfeiler_leman.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 10:31:36.000000 pykwl-0.0.7/include/wl/wl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-29 10:31:36.000000 pykwl-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.180570 pykwl-0.0.7/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/python/src/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/python/src/pykwl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/pykwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/pykwl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/pykwl/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/python/src/pykwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:31:46.184571 pykwl-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-29 10:31:36.000000 pykwl-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-29 10:31:36.000000 pykwl-0.0.7/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-29 10:31:36.000000 pykwl-0.0.7/src/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-29 10:31:36.000000 pykwl-0.0.7/src/weisfeiler_leman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:36.000000 pykwl-0.0.7/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:36.000000 pykwl-0.0.7/tests/unit/CMakeLists copy.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:36.000000 pykwl-0.0.7/tests/unit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.664340 pykwl-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-09 10:17:03.000000 pykwl-0.0.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 10:17:03.000000 pykwl-0.0.8/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 10:17:03.000000 pykwl-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-09 10:17:03.000000 pykwl-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 10:17:11.660340 pykwl-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 10:17:03.000000 pykwl-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 10:17:03.000000 pykwl-0.0.8/cmake/configure_ccache.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 10:17:03.000000 pykwl-0.0.8/dependencies/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/dependencies/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-09 10:17:03.000000 pykwl-0.0.8/dependencies/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.656340 pykwl-0.0.8/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/include/wl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/include/wl/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-09 10:17:03.000000 pykwl-0.0.8/include/wl/details/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-09 10:17:03.000000 pykwl-0.0.8/include/wl/details/weisfeiler_leman.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 10:17:03.000000 pykwl-0.0.8/include/wl/wl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 10:17:03.000000 pykwl-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.656340 pykwl-0.0.8/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/python/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/python/src/pykwl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/pykwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/pykwl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/pykwl/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/python/src/pykwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:17:11.664340 pykwl-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-09 10:17:03.000000 pykwl-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-09 10:17:03.000000 pykwl-0.0.8/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-09 10:17:03.000000 pykwl-0.0.8/src/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-05-09 10:17:03.000000 pykwl-0.0.8/src/weisfeiler_leman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:03.000000 pykwl-0.0.8/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:03.000000 pykwl-0.0.8/tests/unit/CMakeLists copy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:03.000000 pykwl-0.0.8/tests/unit/CMakeLists.txt
```

### Comparing `pykwl-0.0.7/CMakeLists.txt` & `pykwl-0.0.8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/Config.cmake.in` & `pykwl-0.0.8/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/LICENSE` & `pykwl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/README.md` & `pykwl-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/cmake/configure_ccache.cmake` & `pykwl-0.0.8/cmake/configure_ccache.cmake`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/dependencies/pybind11/CMakeLists.txt` & `pykwl-0.0.8/dependencies/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/include/wl/details/graph.hpp` & `pykwl-0.0.8/include/wl/details/graph.hpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/include/wl/details/weisfeiler_leman.hpp` & `pykwl-0.0.8/include/wl/details/weisfeiler_leman.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -42,12 +42,14 @@
     explicit WeisfeilerLeman(int k, bool ignore_counting);
 
     int get_k() const;
 
     bool get_ignore_counting() const;
 
     std::tuple<int, std::vector<int>, std::vector<int>> compute_coloring(const Graph& graph);
+
+    size_t get_coloring_function_size() const;
 };
 
 }
 
 #endif
```

### Comparing `pykwl-0.0.7/pyproject.toml` & `pykwl-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/python/src/pykwl/bindings.cpp` & `pykwl-0.0.8/python/src/pykwl/bindings.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -20,9 +20,10 @@
         .def("add_edge", &Graph::add_edge, py::arg("src_node"), py::arg("dst_node"), py::arg("label") = 0);
 
     py::class_<WeisfeilerLeman>(m, "WeisfeilerLeman")  //
         .def(py::init<int>())
         .def(py::init<int, bool>())
         .def("get_k", &WeisfeilerLeman::get_k)
         .def("get_ignore_counting", &WeisfeilerLeman::get_ignore_counting)
-        .def("compute_coloring", &WeisfeilerLeman::compute_coloring);
+        .def("compute_coloring", &WeisfeilerLeman::compute_coloring)
+        .def("get_coloring_function_size", &WeisfeilerLeman::get_coloring_function_size);
 }
```

### Comparing `pykwl-0.0.7/python/src/pykwl.egg-info/SOURCES.txt` & `pykwl-0.0.8/python/src/pykwl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/setup.py` & `pykwl-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import multiprocessing
 
 from pathlib import Path
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
```

### Comparing `pykwl-0.0.7/src/CMakeLists.txt` & `pykwl-0.0.8/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/src/graph.cpp` & `pykwl-0.0.8/src/graph.cpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.7/src/weisfeiler_leman.cpp` & `pykwl-0.0.8/src/weisfeiler_leman.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,48 @@
 #include <cstddef>
 #include <cstdlib>
 #include <stdexcept>
 #include <tuple>
 #include <unordered_map>
 #include <utility>
 #include <vector>
+#include <limits>
+#include <climits>
 
 namespace wl
 {
 
-inline static int pairing_function(int x, int y)
-{
-    // Szudzik's pairing function
-    return std::abs(x >= y ? x * x + x + y : y * y + x);
+inline static int safe_multiply(int x, int y) {
+    if (x != 0 && (y > INT_MAX / x || y < INT_MIN / x)) {
+        throw std::overflow_error("Overflow detected in multiplication");
+    }
+    return x * y;
+}
+
+inline static int pairing_function(int x, int y) {
+    int x_sq, y_sq;
+    if (x >= y) {
+        x_sq = safe_multiply(x, x);  // Safe multiplication
+        int x_sq_plus_x = x_sq + x;  // Add x
+        if (x_sq_plus_x < x_sq) throw std::overflow_error("Overflow in addition");
+        return x_sq_plus_x + y;  // Add y
+    } else {
+        y_sq = safe_multiply(y, y);  // Safe multiplication
+        if (y_sq < y) throw std::overflow_error("Overflow in addition");
+        return y_sq + x;  // Add x
+    }
 }
 
+
+//inline static int pairing_function(int x, int y)
+//{
+//    // Szudzik's pairing function
+//    return std::abs(x >= y ? x * x + x + y : y * y + x);
+//}
+
 inline static void lexical_sort(std::vector<int>& items1, std::vector<int>& items2)
 {
     assert(items1.size() == items2.size());
 
     std::vector<std::pair<int, int>> paired_items(items1.size());
     for (size_t i = 0; i < items1.size(); ++i)
     {
@@ -315,8 +339,10 @@
     {
         return k2_fwl(graph);
     }
 
     throw std::invalid_argument("k must be either 1 or 2");
 }
 
+size_t WeisfeilerLeman::get_coloring_function_size() const { return m_color_function.size(); }
+
 }
```

