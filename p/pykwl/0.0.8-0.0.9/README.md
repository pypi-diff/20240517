# Comparing `tmp/pykwl-0.0.8.tar.gz` & `tmp/pykwl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykwl-0.0.8.tar", last modified: Thu May  9 10:17:11 2024, max compression
+gzip compressed data, was "pykwl-0.0.9.tar", last modified: Fri May 17 17:43:22 2024, max compression
```

## Comparing `pykwl-0.0.8.tar` & `pykwl-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.664340 pykwl-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-09 10:17:03.000000 pykwl-0.0.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 10:17:03.000000 pykwl-0.0.8/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 10:17:03.000000 pykwl-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-09 10:17:03.000000 pykwl-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 10:17:11.660340 pykwl-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 10:17:03.000000 pykwl-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 10:17:03.000000 pykwl-0.0.8/cmake/configure_ccache.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 10:17:03.000000 pykwl-0.0.8/dependencies/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/dependencies/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-09 10:17:03.000000 pykwl-0.0.8/dependencies/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.656340 pykwl-0.0.8/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/include/wl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/include/wl/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-09 10:17:03.000000 pykwl-0.0.8/include/wl/details/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-09 10:17:03.000000 pykwl-0.0.8/include/wl/details/weisfeiler_leman.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 10:17:03.000000 pykwl-0.0.8/include/wl/wl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 10:17:03.000000 pykwl-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.656340 pykwl-0.0.8/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/python/src/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/python/src/pykwl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/pykwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/pykwl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-09 10:17:03.000000 pykwl-0.0.8/python/src/pykwl/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/python/src/pykwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 10:17:11.000000 pykwl-0.0.8/python/src/pykwl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:17:11.664340 pykwl-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-09 10:17:03.000000 pykwl-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-09 10:17:03.000000 pykwl-0.0.8/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-09 10:17:03.000000 pykwl-0.0.8/src/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-05-09 10:17:03.000000 pykwl-0.0.8/src/weisfeiler_leman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:03.000000 pykwl-0.0.8/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:11.660340 pykwl-0.0.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:03.000000 pykwl-0.0.8/tests/unit/CMakeLists copy.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:17:03.000000 pykwl-0.0.8/tests/unit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.985301 pykwl-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-17 17:43:14.000000 pykwl-0.0.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-17 17:43:14.000000 pykwl-0.0.9/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 17:43:14.000000 pykwl-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-17 17:43:14.000000 pykwl-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 17:43:22.985301 pykwl-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-17 17:43:14.000000 pykwl-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.981301 pykwl-0.0.9/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-17 17:43:14.000000 pykwl-0.0.9/cmake/configure_ccache.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.981301 pykwl-0.0.9/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-17 17:43:14.000000 pykwl-0.0.9/dependencies/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.981301 pykwl-0.0.9/dependencies/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-17 17:43:14.000000 pykwl-0.0.9/dependencies/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.981301 pykwl-0.0.9/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.981301 pykwl-0.0.9/include/wl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.981301 pykwl-0.0.9/include/wl/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-17 17:43:14.000000 pykwl-0.0.9/include/wl/details/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-17 17:43:14.000000 pykwl-0.0.9/include/wl/details/weisfeiler_leman.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-17 17:43:14.000000 pykwl-0.0.9/include/wl/wl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-17 17:43:14.000000 pykwl-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.981301 pykwl-0.0.9/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.981301 pykwl-0.0.9/python/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-17 17:43:14.000000 pykwl-0.0.9/python/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-17 17:43:14.000000 pykwl-0.0.9/python/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.981301 pykwl-0.0.9/python/src/pykwl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 17:43:14.000000 pykwl-0.0.9/python/src/pykwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-17 17:43:14.000000 pykwl-0.0.9/python/src/pykwl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-17 17:43:14.000000 pykwl-0.0.9/python/src/pykwl/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.985301 pykwl-0.0.9/python/src/pykwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 17:43:22.000000 pykwl-0.0.9/python/src/pykwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-17 17:43:22.000000 pykwl-0.0.9/python/src/pykwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:43:22.000000 pykwl-0.0.9/python/src/pykwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:43:22.000000 pykwl-0.0.9/python/src/pykwl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 17:43:22.000000 pykwl-0.0.9/python/src/pykwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 17:43:22.000000 pykwl-0.0.9/python/src/pykwl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 17:43:22.985301 pykwl-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-17 17:43:14.000000 pykwl-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.985301 pykwl-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-17 17:43:14.000000 pykwl-0.0.9/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-17 17:43:14.000000 pykwl-0.0.9/src/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-17 17:43:14.000000 pykwl-0.0.9/src/weisfeiler_leman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.985301 pykwl-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:14.000000 pykwl-0.0.9/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.985301 pykwl-0.0.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:14.000000 pykwl-0.0.9/tests/unit/CMakeLists copy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:14.000000 pykwl-0.0.9/tests/unit/CMakeLists.txt
```

### Comparing `pykwl-0.0.8/CMakeLists.txt` & `pykwl-0.0.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/Config.cmake.in` & `pykwl-0.0.9/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/LICENSE` & `pykwl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/README.md` & `pykwl-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/cmake/configure_ccache.cmake` & `pykwl-0.0.9/cmake/configure_ccache.cmake`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/dependencies/pybind11/CMakeLists.txt` & `pykwl-0.0.9/dependencies/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/include/wl/details/graph.hpp` & `pykwl-0.0.9/include/wl/details/graph.hpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/include/wl/details/weisfeiler_leman.hpp` & `pykwl-0.0.9/include/wl/details/weisfeiler_leman.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #define WL_DETAILS_WEISFEILER_LEMAN_HPP_
 
 #include "wl/details/graph.hpp"
 
 #include <map>
 #include <tuple>
 #include <vector>
+#include <limits>
 
 namespace wl
 {
 
 using Color = int;
 using AdjacentColor = std::pair<Color, Color>;
 using NodeColorContext = std::tuple<Color, std::vector<AdjacentColor>, std::vector<AdjacentColor>>;
@@ -28,28 +29,28 @@
                                                    const std::vector<Color>& edge_colors,
                                                    const std::vector<int>& edge_indices);
 
     Color get_new_color(NodeColorContext&& color_multiset);
 
     Color get_subgraph_color(int src_node, int dst_node, const Graph& graph);
 
-    std::tuple<int, std::vector<int>, std::vector<int>> k1_fwl(const Graph& graph);
+    std::tuple<int, std::vector<int>, std::vector<int>> k1_fwl(const Graph& graph, size_t max_num_iterations);
 
-    std::tuple<int, std::vector<int>, std::vector<int>> k2_fwl(const Graph& graph);
+    std::tuple<int, std::vector<int>, std::vector<int>> k2_fwl(const Graph& graph, size_t max_num_iterations);
 
 public:
     explicit WeisfeilerLeman(int k);
 
     explicit WeisfeilerLeman(int k, bool ignore_counting);
 
     int get_k() const;
 
     bool get_ignore_counting() const;
 
-    std::tuple<int, std::vector<int>, std::vector<int>> compute_coloring(const Graph& graph);
+    std::tuple<int, std::vector<int>, std::vector<int>> compute_coloring(const Graph& graph, size_t max_num_iterations = std::numeric_limits<size_t>::max());
 
     size_t get_coloring_function_size() const;
 };
 
 }
 
 #endif
```

### Comparing `pykwl-0.0.8/pyproject.toml` & `pykwl-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/python/src/pykwl/bindings.cpp` & `pykwl-0.0.9/python/src/pykwl/bindings.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -20,10 +20,10 @@
         .def("add_edge", &Graph::add_edge, py::arg("src_node"), py::arg("dst_node"), py::arg("label") = 0);
 
     py::class_<WeisfeilerLeman>(m, "WeisfeilerLeman")  //
         .def(py::init<int>())
         .def(py::init<int, bool>())
         .def("get_k", &WeisfeilerLeman::get_k)
         .def("get_ignore_counting", &WeisfeilerLeman::get_ignore_counting)
-        .def("compute_coloring", &WeisfeilerLeman::compute_coloring)
+        .def("compute_coloring", &WeisfeilerLeman::compute_coloring, py::arg("graph"), py::arg("max_num_iterations") = std::numeric_limits<size_t>::max())
         .def("get_coloring_function_size", &WeisfeilerLeman::get_coloring_function_size);
 }
```

### Comparing `pykwl-0.0.8/python/src/pykwl.egg-info/SOURCES.txt` & `pykwl-0.0.9/python/src/pykwl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/setup.py` & `pykwl-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import multiprocessing
 
 from pathlib import Path
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
```

### Comparing `pykwl-0.0.8/src/CMakeLists.txt` & `pykwl-0.0.9/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/src/graph.cpp` & `pykwl-0.0.9/src/graph.cpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.8/src/weisfeiler_leman.cpp` & `pykwl-0.0.9/src/weisfeiler_leman.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         m_color_function.emplace(std::move(node_color_context), color);
         return color;
     }
 
     return it->second;
 }
 
-std::tuple<int, std::vector<int>, std::vector<int>> WeisfeilerLeman::k1_fwl(const Graph& graph)
+std::tuple<int, std::vector<int>, std::vector<int>> WeisfeilerLeman::k1_fwl(const Graph& graph, size_t max_num_iterations)
 {
     auto num_nodes = graph.get_num_nodes();
     auto current_coloring = std::vector<int>(num_nodes);
     auto next_coloring = std::vector<int>(num_nodes);
 
     for (int node = 0; node < num_nodes; ++node)
     {
@@ -210,14 +210,18 @@
         {
             break;
         }
         else
         {
             std::swap(current_coloring, next_coloring);
         }
+
+        if (num_iterations == max_num_iterations) {
+            break;
+        }
     }
 
     auto [unique, counts] = get_frequencies(current_coloring);
     lexical_sort(unique, counts);
     return { num_iterations, std::move(unique), std::move(counts) };
 }
 
@@ -264,15 +268,15 @@
 
     // Graph labels must be non-negative and colors will always be positive.
     // We make the graph labels negative so that they are not confused with colors.
 
     return get_new_color({ -pairing_function(src_label, dst_label) - 1, std::move(forward_colors), std::move(backward_colors) });
 }
 
-std::tuple<int, std::vector<int>, std::vector<int>> WeisfeilerLeman::k2_fwl(const Graph& graph)
+std::tuple<int, std::vector<int>, std::vector<int>> WeisfeilerLeman::k2_fwl(const Graph& graph, size_t max_num_iterations)
 {
     const auto num_nodes = graph.get_num_nodes();
     auto current_coloring = std::vector<int>(num_nodes * num_nodes);
     auto next_coloring = std::vector<int>(num_nodes * num_nodes);
 
     for (int first_node = 0; first_node < num_nodes; ++first_node)
     {
@@ -317,31 +321,35 @@
         {
             break;
         }
         else
         {
             std::swap(current_coloring, next_coloring);
         }
+
+        if (num_iterations == max_num_iterations) {
+            break;
+        }
     }
 
     auto [unique, counts] = get_frequencies(current_coloring);
     lexical_sort(unique, counts);
     return { num_iterations, std::move(unique), std::move(counts) };
 }
 
-std::tuple<int, std::vector<int>, std::vector<int>> WeisfeilerLeman::compute_coloring(const Graph& graph)
+std::tuple<int, std::vector<int>, std::vector<int>> WeisfeilerLeman::compute_coloring(const Graph& graph, size_t max_num_iterations)
 {
     if (m_k == 1)
     {
-        return k1_fwl(graph);
+        return k1_fwl(graph, max_num_iterations);
     }
 
     if (m_k == 2)
     {
-        return k2_fwl(graph);
+        return k2_fwl(graph, max_num_iterations);
     }
 
     throw std::invalid_argument("k must be either 1 or 2");
 }
 
 size_t WeisfeilerLeman::get_coloring_function_size() const { return m_color_function.size(); }
```

