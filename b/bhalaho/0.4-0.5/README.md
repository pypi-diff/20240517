# Comparing `tmp/bhalaho-0.4.tar.gz` & `tmp/bhalaho-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhalaho-0.4.tar", last modified: Fri May 17 08:27:05 2024, max compression
+gzip compressed data, was "bhalaho-0.5.tar", last modified: Fri May 17 17:18:03 2024, max compression
```

## Comparing `bhalaho-0.4.tar` & `bhalaho-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 08:27:05.465032 bhalaho-0.4/
--rw-rw-rw-   0        0        0     1041 2024-05-16 22:19:08.000000 bhalaho-0.4/LICENSE
--rw-rw-rw-   0        0        0       72 2024-05-16 22:19:58.000000 bhalaho-0.4/MANIFEST.in
--rw-rw-rw-   0        0        0       75 2024-05-17 08:27:05.454112 bhalaho-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-05-16 21:22:32.000000 bhalaho-0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 08:27:05.351250 bhalaho-0.4/bhalaho/
--rw-rw-rw-   0        0        0        0 2024-05-16 20:58:36.000000 bhalaho-0.4/bhalaho/__init__.py
--rw-rw-rw-   0        0        0    29888 2024-05-17 08:23:39.000000 bhalaho-0.4/bhalaho/daoa.py
--rw-rw-rw-   0        0        0      756 2024-05-16 21:25:52.000000 bhalaho-0.4/bhalaho/download.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:27:05.441705 bhalaho-0.4/bhalaho.egg-info/
--rw-rw-rw-   0        0        0       75 2024-05-17 08:27:04.000000 bhalaho-0.4/bhalaho.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-17 08:27:04.000000 bhalaho-0.4/bhalaho.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 08:27:04.000000 bhalaho-0.4/bhalaho.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-17 08:27:04.000000 bhalaho-0.4/bhalaho.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 08:27:05.466341 bhalaho-0.4/setup.cfg
--rw-rw-rw-   0        0        0      211 2024-05-17 08:21:02.000000 bhalaho-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:18:03.214503 bhalaho-0.5/
+-rw-rw-rw-   0        0        0     1041 2024-05-16 22:19:08.000000 bhalaho-0.5/LICENSE
+-rw-rw-rw-   0        0        0       72 2024-05-16 22:19:58.000000 bhalaho-0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0       75 2024-05-17 17:18:03.214503 bhalaho-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2024-05-16 21:22:32.000000 bhalaho-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 17:18:03.180209 bhalaho-0.5/bhalaho/
+-rw-rw-rw-   0        0        0        0 2024-05-16 20:58:36.000000 bhalaho-0.5/bhalaho/__init__.py
+-rw-rw-rw-   0        0        0    31309 2024-05-17 17:16:43.000000 bhalaho-0.5/bhalaho/daoa.py
+-rw-rw-rw-   0        0        0      756 2024-05-16 21:25:52.000000 bhalaho-0.5/bhalaho/download.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:18:03.214503 bhalaho-0.5/bhalaho.egg-info/
+-rw-rw-rw-   0        0        0       75 2024-05-17 17:18:02.000000 bhalaho-0.5/bhalaho.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-17 17:18:02.000000 bhalaho-0.5/bhalaho.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 17:18:02.000000 bhalaho-0.5/bhalaho.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 17:18:02.000000 bhalaho-0.5/bhalaho.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 17:18:03.220276 bhalaho-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      211 2024-05-17 17:17:42.000000 bhalaho-0.5/setup.py
```

### Comparing `bhalaho-0.4/LICENSE` & `bhalaho-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bhalaho-0.4/bhalaho/daoa.py` & `bhalaho-0.5/bhalaho/daoa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1109,15 +1109,70 @@
     printJobScheduling(arr, n);
     return 0;
 }
 
 '''
 
 time_complexity = '''
-abhi baki hai daalna bhai , sabar rakho
+
+=>practical exams:
+strassen matrix multiplication :-O(N^2.8074)
+prims algorithm:-O(V^2)
+kruskals algorithm:-O(E * log(E))
+fractional knapsack:- O(n * log(n))
+coin change greedy : O(V)
+dijkstra algorithm:-O(V^2)
+matrix chain multiplication :- O(n ^ 3)
+TSP problem :- O(n ^ 2 * 2 ^ n)
+Coin change dp:- O ( N * sun)
+Longest Common Subsequence :- O(m * n)
+N queen problem :- O(n!)
+sum of subset problem:- O(2 ^ n)
+Job scheduling with Deadlines :- O(N ^ 2)
+15 puzzle problem:-O(n^2 * n!)
+KMP algorithm:- O(N + M)
+
+=>Divide and conquer algorithm:
+
+min-max algorithm:O(N log N)
+merge sort: O(N log N)
+quick sort:O(N ^ 2) = worst and average = O(N log N) same for the best
+
+
+=>greedy algorithm:
+
+activity selection problem:-O(N log n) - unsorted and O(N) -sorted
+
+
+=>dynamic programming:
+
+Fibonacci problem:- O(n)
+0/1 knapsack :- O(N * W)
+Multistage Graph :- O(k * E)k = stage, E = edge
+Floyd Warshall algo:- O(V ^ 3)
+Bellmam Ford Algo :- O(V * E)
+Optimal Binary Search tree :- O(N ^ 3)
+johnson flow shop scheduling :- O(n log n)
+
+
+=>backtracking:
+
+Graph Coloring: O(m ^ V) m = color number and V = number of vector
+Hamiltonian Cycle: O(n!)
+
+=>branch and bound:
+0/1 Knapsack problem:O(2 ^ N)
+TSP using branch and bound: O(2 ^ N)
+Job Sequencing with deadlines : O(n*logn+n⋅2^n)
+
+
+=>string matching algorithm:
+naive string algo = O(N^2)
+Rabin Karp algorithm = O(N*M)
+String matching with finite automata:O(m ^ 2)
 '''
 
 daoaexp = {
     'Prims.c' : prims,
     'Kruskal.c' : kruskal,
     'Dijkstra.c' : dijkstra,
     'Matrix Chain Multiplication.c' : matrix_chain_multiplication,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bhalaho-0.4/bhalaho/download.py` & `bhalaho-0.5/bhalaho/download.py`

 * *Files identical despite different names*

