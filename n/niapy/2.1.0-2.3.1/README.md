# Comparing `tmp/niapy-2.1.0.tar.gz` & `tmp/niapy-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niapy-2.1.0.tar", max compression
+gzip compressed data, was "niapy-2.3.1.tar", max compression
```

## Comparing `niapy-2.1.0.tar` & `niapy-2.3.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    11241 2023-12-19 17:20:25.526498 niapy-2.1.0/Algorithms.md
--rw-r--r--   0        0        0    48457 2023-12-19 17:20:25.526498 niapy-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      620 2023-12-19 17:20:25.526498 niapy-2.1.0/CITATION.cff
--rw-r--r--   0        0        0     1063 2023-12-19 17:20:25.526498 niapy-2.1.0/LICENSE
--rw-r--r--   0        0        0     1089 2023-12-19 17:20:25.526498 niapy-2.1.0/Problems.md
--rw-r--r--   0        0        0    20827 2023-12-19 17:20:25.526498 niapy-2.1.0/README.md
--rw-r--r--   0        0        0      334 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/__init__.py
--rw-r--r--   0        0        0      447 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/__init__.py
--rw-r--r--   0        0        0    16664 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/algorithm.py
--rw-r--r--   0        0        0     4340 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/__init__.py
--rw-r--r--   0        0        0     7662 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/abc.py
--rw-r--r--   0        0        0     7734 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/ba.py
--rw-r--r--   0        0        0     8114 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/bea.py
--rw-r--r--   0        0        0    12574 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/bfo.py
--rw-r--r--   0        0        0    13291 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/ca.py
--rw-r--r--   0        0        0     9100 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/clonalg.py
--rw-r--r--   0        0        0    16970 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/cro.py
--rw-r--r--   0        0        0     4812 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/cs.py
--rw-r--r--   0        0        0    11288 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/cso.py
--rw-r--r--   0        0        0    38861 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/de.py
--rw-r--r--   0        0        0    17522 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/es.py
--rw-r--r--   0        0        0     5972 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/fa.py
--rw-r--r--   0        0        0    10554 2023-12-19 17:20:25.530498 niapy-2.1.0/niapy/algorithms/basic/foa.py
--rw-r--r--   0        0        0     4836 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/fpa.py
--rw-r--r--   0        0        0    14015 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/fss.py
--rw-r--r--   0        0        0    34125 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/fwa.py
--rw-r--r--   0        0        0    13744 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/ga.py
--rw-r--r--   0        0        0     5969 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/gsa.py
--rw-r--r--   0        0        0    15306 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/gso.py
--rw-r--r--   0        0        0     5591 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/gwo.py
--rw-r--r--   0        0        0     6949 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/hho.py
--rw-r--r--   0        0        0     8026 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/hs.py
--rw-r--r--   0        0        0    19288 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/kh.py
--rw-r--r--   0        0        0    51695 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/loa.py
--rw-r--r--   0        0        0     9691 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/mbo.py
--rw-r--r--   0        0        0     3771 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/mfo.py
--rw-r--r--   0        0        0    19379 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/mke.py
--rw-r--r--   0        0        0    44066 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/pso.py
--rw-r--r--   0        0        0     5760 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/basic/sca.py
--rw-r--r--   0        0        0     1744 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/modified/__init__.py
--rw-r--r--   0        0        0     3705 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/modified/hba.py
--rw-r--r--   0        0        0    17193 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/modified/hde.py
--rw-r--r--   0        0        0     4597 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/modified/hsaba.py
--rw-r--r--   0        0        0     8820 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/modified/jde.py
--rw-r--r--   0        0        0     5272 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/modified/plba.py
--rw-r--r--   0        0        0    14783 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/modified/saba.py
--rw-r--r--   0        0        0    23296 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/modified/shade.py
--rw-r--r--   0        0        0      768 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/other/__init__.py
--rw-r--r--   0        0        0    22524 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/other/aso.py
--rw-r--r--   0        0        0     4712 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/other/hc.py
--rw-r--r--   0        0        0    29712 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/other/mts.py
--rw-r--r--   0        0        0     7027 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/other/nmm.py
--rw-r--r--   0        0        0     3738 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/other/rs.py
--rw-r--r--   0        0        0     6513 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/algorithms/other/sa.py
--rw-r--r--   0        0        0     4669 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/callbacks.py
--rw-r--r--   0        0        0     2688 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/__init__.py
--rw-r--r--   0        0        0     2769 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/ackley.py
--rw-r--r--   0        0        0     4015 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/alpine.py
--rw-r--r--   0        0        0     1910 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/bent_cigar.py
--rw-r--r--   0        0        0     2054 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/chung_reynolds.py
--rw-r--r--   0        0        0     2067 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/cosine_mixture.py
--rw-r--r--   0        0        0     2162 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/csendes.py
--rw-r--r--   0        0        0     1883 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/discus.py
--rw-r--r--   0        0        0     2165 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/dixon_price.py
--rw-r--r--   0        0        0     2152 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/elliptic.py
--rw-r--r--   0        0        0     4885 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/griewank.py
--rw-r--r--   0        0        0     2634 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/happy_cat.py
--rw-r--r--   0        0        0     2496 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/hgbat.py
--rw-r--r--   0        0        0     2388 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/katsuura.py
--rw-r--r--   0        0        0     2593 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/levy.py
--rw-r--r--   0        0        0     2367 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/michalewicz.py
--rw-r--r--   0        0        0     2259 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/perm.py
--rw-r--r--   0        0        0     3249 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/pinter.py
--rw-r--r--   0        0        0     2612 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/powell.py
--rw-r--r--   0        0        0     1912 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/problem.py
--rw-r--r--   0        0        0     2076 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/qing.py
--rw-r--r--   0        0        0     2302 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/quintic.py
--rw-r--r--   0        0        0     2016 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/rastrigin.py
--rw-r--r--   0        0        0     1922 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/ridge.py
--rw-r--r--   0        0        0     2213 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/rosenbrock.py
--rw-r--r--   0        0        0     2331 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/salomon.py
--rw-r--r--   0        0        0     6820 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/schaffer.py
--rw-r--r--   0        0        0     2004 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/schumer_steiglitz.py
--rw-r--r--   0        0        0    10325 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/schwefel.py
--rw-r--r--   0        0        0     5576 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/sphere.py
--rw-r--r--   0        0        0     6088 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/step.py
--rw-r--r--   0        0        0     1946 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/stepint.py
--rw-r--r--   0        0        0     2251 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/styblinski_tang.py
--rw-r--r--   0        0        0     1986 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/sum_squares.py
--rw-r--r--   0        0        0     2020 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/trid.py
--rw-r--r--   0        0        0     2956 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/weierstrass.py
--rw-r--r--   0        0        0     2670 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/whitley.py
--rw-r--r--   0        0        0     2259 2023-12-19 17:20:25.534498 niapy-2.1.0/niapy/problems/zakharov.py
--rw-r--r--   0        0        0     4824 2023-12-19 17:20:25.538498 niapy-2.1.0/niapy/runner.py
--rw-r--r--   0        0        0     9047 2023-12-19 17:20:25.538498 niapy-2.1.0/niapy/task.py
--rw-r--r--   0        0        0      578 2023-12-19 17:20:25.538498 niapy-2.1.0/niapy/util/__init__.py
--rw-r--r--   0        0        0     4596 2023-12-19 17:20:25.538498 niapy-2.1.0/niapy/util/argparser.py
--rw-r--r--   0        0        0     1190 2023-12-19 17:20:25.538498 niapy-2.1.0/niapy/util/array.py
--rw-r--r--   0        0        0      350 2023-12-19 17:20:25.538498 niapy-2.1.0/niapy/util/distances.py
--rw-r--r--   0        0        0     9596 2023-12-19 17:20:25.538498 niapy-2.1.0/niapy/util/factory.py
--rw-r--r--   0        0        0      759 2023-12-19 17:20:25.538498 niapy-2.1.0/niapy/util/random.py
--rw-r--r--   0        0        0     2974 2023-12-19 17:20:25.538498 niapy-2.1.0/niapy/util/repair.py
--rw-r--r--   0        0        0     2554 2023-12-19 17:20:25.538498 niapy-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    22128 1970-01-01 00:00:00.000000 niapy-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11241 2024-05-17 08:31:20.191630 niapy-2.3.1/Algorithms.md
+-rw-r--r--   0        0        0    49325 2024-05-17 08:31:20.191630 niapy-2.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      620 2024-05-17 08:31:20.191630 niapy-2.3.1/CITATION.cff
+-rw-r--r--   0        0        0     1063 2024-05-17 08:31:20.191630 niapy-2.3.1/LICENSE
+-rw-r--r--   0        0        0     1089 2024-05-17 08:31:20.191630 niapy-2.3.1/Problems.md
+-rw-r--r--   0        0        0    20827 2024-05-17 08:31:20.191630 niapy-2.3.1/README.md
+-rw-r--r--   0        0        0      334 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/__init__.py
+-rw-r--r--   0        0        0      447 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/__init__.py
+-rw-r--r--   0        0        0    16664 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/algorithm.py
+-rw-r--r--   0        0        0     4340 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/__init__.py
+-rw-r--r--   0        0        0     7662 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/abc.py
+-rw-r--r--   0        0        0     7734 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/ba.py
+-rw-r--r--   0        0        0     8114 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/bea.py
+-rw-r--r--   0        0        0    12574 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/bfo.py
+-rw-r--r--   0        0        0    13291 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/ca.py
+-rw-r--r--   0        0        0     9100 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/clonalg.py
+-rw-r--r--   0        0        0    16970 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/cro.py
+-rw-r--r--   0        0        0     4812 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/cs.py
+-rw-r--r--   0        0        0    11288 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/cso.py
+-rw-r--r--   0        0        0    38861 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/de.py
+-rw-r--r--   0        0        0    17522 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/es.py
+-rw-r--r--   0        0        0     5972 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/fa.py
+-rw-r--r--   0        0        0    10554 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/foa.py
+-rw-r--r--   0        0        0     4836 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/fpa.py
+-rw-r--r--   0        0        0    14015 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/fss.py
+-rw-r--r--   0        0        0    34125 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/fwa.py
+-rw-r--r--   0        0        0    13744 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/ga.py
+-rw-r--r--   0        0        0     5969 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/gsa.py
+-rw-r--r--   0        0        0    15306 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/gso.py
+-rw-r--r--   0        0        0     5591 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/gwo.py
+-rw-r--r--   0        0        0     6949 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/hho.py
+-rw-r--r--   0        0        0     8026 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/hs.py
+-rw-r--r--   0        0        0    19288 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/kh.py
+-rw-r--r--   0        0        0    51695 2024-05-17 08:31:20.195630 niapy-2.3.1/niapy/algorithms/basic/loa.py
+-rw-r--r--   0        0        0     9691 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/basic/mbo.py
+-rw-r--r--   0        0        0     3771 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/basic/mfo.py
+-rw-r--r--   0        0        0    19379 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/basic/mke.py
+-rw-r--r--   0        0        0    44066 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/basic/pso.py
+-rw-r--r--   0        0        0     5760 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/basic/sca.py
+-rw-r--r--   0        0        0     1744 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/modified/__init__.py
+-rw-r--r--   0        0        0     3705 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/modified/hba.py
+-rw-r--r--   0        0        0    17193 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/modified/hde.py
+-rw-r--r--   0        0        0     4597 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/modified/hsaba.py
+-rw-r--r--   0        0        0     8820 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/modified/jde.py
+-rw-r--r--   0        0        0     5272 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/modified/plba.py
+-rw-r--r--   0        0        0    14783 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/modified/saba.py
+-rw-r--r--   0        0        0    23296 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/modified/shade.py
+-rw-r--r--   0        0        0      768 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/other/__init__.py
+-rw-r--r--   0        0        0    22524 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/other/aso.py
+-rw-r--r--   0        0        0     4712 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/other/hc.py
+-rw-r--r--   0        0        0    29712 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/other/mts.py
+-rw-r--r--   0        0        0     7027 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/other/nmm.py
+-rw-r--r--   0        0        0     3738 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/other/rs.py
+-rw-r--r--   0        0        0     6513 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/algorithms/other/sa.py
+-rw-r--r--   0        0        0     4669 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/callbacks.py
+-rw-r--r--   0        0        0     2688 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/__init__.py
+-rw-r--r--   0        0        0     2769 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/ackley.py
+-rw-r--r--   0        0        0     4015 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/alpine.py
+-rw-r--r--   0        0        0     1910 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/bent_cigar.py
+-rw-r--r--   0        0        0     2054 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/chung_reynolds.py
+-rw-r--r--   0        0        0     2067 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/cosine_mixture.py
+-rw-r--r--   0        0        0     2162 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/csendes.py
+-rw-r--r--   0        0        0     1883 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/discus.py
+-rw-r--r--   0        0        0     2165 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/dixon_price.py
+-rw-r--r--   0        0        0     2152 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/elliptic.py
+-rw-r--r--   0        0        0     4885 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/griewank.py
+-rw-r--r--   0        0        0     2634 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/happy_cat.py
+-rw-r--r--   0        0        0     2496 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/hgbat.py
+-rw-r--r--   0        0        0     2388 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/katsuura.py
+-rw-r--r--   0        0        0     2593 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/levy.py
+-rw-r--r--   0        0        0     2367 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/michalewicz.py
+-rw-r--r--   0        0        0     2259 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/perm.py
+-rw-r--r--   0        0        0     3249 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/pinter.py
+-rw-r--r--   0        0        0     2612 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/powell.py
+-rw-r--r--   0        0        0     1912 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/problem.py
+-rw-r--r--   0        0        0     2076 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/qing.py
+-rw-r--r--   0        0        0     2302 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/quintic.py
+-rw-r--r--   0        0        0     2016 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/rastrigin.py
+-rw-r--r--   0        0        0     1922 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/ridge.py
+-rw-r--r--   0        0        0     2213 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/rosenbrock.py
+-rw-r--r--   0        0        0     2331 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/salomon.py
+-rw-r--r--   0        0        0     6820 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/schaffer.py
+-rw-r--r--   0        0        0     2004 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/schumer_steiglitz.py
+-rw-r--r--   0        0        0    10325 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/schwefel.py
+-rw-r--r--   0        0        0     5576 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/sphere.py
+-rw-r--r--   0        0        0     6088 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/step.py
+-rw-r--r--   0        0        0     1946 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/stepint.py
+-rw-r--r--   0        0        0     2251 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/styblinski_tang.py
+-rw-r--r--   0        0        0     1986 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/sum_squares.py
+-rw-r--r--   0        0        0     2020 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/trid.py
+-rw-r--r--   0        0        0     2956 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/weierstrass.py
+-rw-r--r--   0        0        0     2670 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/whitley.py
+-rw-r--r--   0        0        0     2259 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/problems/zakharov.py
+-rw-r--r--   0        0        0     4824 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/runner.py
+-rw-r--r--   0        0        0     9047 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/task.py
+-rw-r--r--   0        0        0      578 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/util/__init__.py
+-rw-r--r--   0        0        0     4596 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/util/argparser.py
+-rw-r--r--   0        0        0     1190 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/util/array.py
+-rw-r--r--   0        0        0      350 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/util/distances.py
+-rw-r--r--   0        0        0     9596 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/util/factory.py
+-rw-r--r--   0        0        0      759 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/util/random.py
+-rw-r--r--   0        0        0     2974 2024-05-17 08:31:20.199630 niapy-2.3.1/niapy/util/repair.py
+-rw-r--r--   0        0        0     2577 2024-05-17 08:31:20.203630 niapy-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0    22128 1970-01-01 00:00:00.000000 niapy-2.3.1/PKG-INFO
```

### Comparing `niapy-2.1.0/Algorithms.md` & `niapy-2.3.1/Algorithms.md`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/CHANGELOG.md` & `niapy-2.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 # Changelog
 
 <!-- insertion marker -->
+## [2.3.1](https://github.com/NiaOrg/NiaPy/releases/tag/2.3.1) - 2024-05-17
+
+<small>[Compare with v2.3.0](https://github.com/NiaOrg/NiaPy/compare/v2.3.0...2.3.1)</small>
+
+### Fixed
+
+- fix: workflow for publishing to pypi ([9e61439](https://github.com/NiaOrg/NiaPy/commit/9e61439fb080b72deec22e8e96c7bd20772b981a) by Grega Vrbančič).
+
+## [v2.3.0](https://github.com/NiaOrg/NiaPy/releases/tag/v2.3.0) - 2024-05-17
+## [v2.2.0](https://github.com/NiaOrg/NiaPy/releases/tag/v2.2.0) - 2024-05-17
+
+<small>[Compare with 2.1.0](https://github.com/NiaOrg/NiaPy/compare/2.1.0...v2.2.0)</small>
+
+### Added
+
+- add example code ([de3a522](https://github.com/NiaOrg/NiaPy/commit/de3a5229dfd366634ab0321e6421ba9817519450) by zStupan).
+
+### Removed
+
+- Remove TestingTask class ([d783f69](https://github.com/NiaOrg/NiaPy/commit/d783f69f6049c9baa6dc79189c47e1ac16d96a75) by zStupan).
+
 ## [2.1.0](https://github.com/NiaOrg/NiaPy/releases/tag/2.1.0) - 2023-12-19
 
 <small>[Compare with 2.0.5](https://github.com/NiaOrg/NiaPy/compare/2.0.5...2.1.0)</small>
 
 ### Added
 
 - Add repology badge ([6d56ff5](https://github.com/NiaOrg/NiaPy/commit/6d56ff579d42c5a4960f7ff5e7d482628bdb3967) by Iztok Fister Jr).
```

### Comparing `niapy-2.1.0/CITATION.cff` & `niapy-2.3.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/LICENSE` & `niapy-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/Problems.md` & `niapy-2.3.1/Problems.md`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/README.md` & `niapy-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/algorithm.py` & `niapy-2.3.1/niapy/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/__init__.py` & `niapy-2.3.1/niapy/algorithms/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/abc.py` & `niapy-2.3.1/niapy/algorithms/basic/abc.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/ba.py` & `niapy-2.3.1/niapy/algorithms/basic/ba.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/bea.py` & `niapy-2.3.1/niapy/algorithms/basic/bea.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/bfo.py` & `niapy-2.3.1/niapy/algorithms/basic/bfo.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/ca.py` & `niapy-2.3.1/niapy/algorithms/basic/ca.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/clonalg.py` & `niapy-2.3.1/niapy/algorithms/basic/clonalg.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/cro.py` & `niapy-2.3.1/niapy/algorithms/basic/cro.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/cs.py` & `niapy-2.3.1/niapy/algorithms/basic/cs.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/cso.py` & `niapy-2.3.1/niapy/algorithms/basic/cso.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/de.py` & `niapy-2.3.1/niapy/algorithms/basic/de.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/es.py` & `niapy-2.3.1/niapy/algorithms/basic/es.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/fa.py` & `niapy-2.3.1/niapy/algorithms/basic/fa.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/foa.py` & `niapy-2.3.1/niapy/algorithms/basic/foa.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/fpa.py` & `niapy-2.3.1/niapy/algorithms/basic/fpa.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/fss.py` & `niapy-2.3.1/niapy/algorithms/basic/fss.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/fwa.py` & `niapy-2.3.1/niapy/algorithms/basic/fwa.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/ga.py` & `niapy-2.3.1/niapy/algorithms/basic/ga.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/gsa.py` & `niapy-2.3.1/niapy/algorithms/basic/gsa.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/gso.py` & `niapy-2.3.1/niapy/algorithms/basic/gso.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/gwo.py` & `niapy-2.3.1/niapy/algorithms/basic/gwo.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/hho.py` & `niapy-2.3.1/niapy/algorithms/basic/hho.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/hs.py` & `niapy-2.3.1/niapy/algorithms/basic/hs.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/kh.py` & `niapy-2.3.1/niapy/algorithms/basic/kh.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/loa.py` & `niapy-2.3.1/niapy/algorithms/basic/loa.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/mbo.py` & `niapy-2.3.1/niapy/algorithms/basic/mbo.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/mfo.py` & `niapy-2.3.1/niapy/algorithms/basic/mfo.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/mke.py` & `niapy-2.3.1/niapy/algorithms/basic/mke.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/pso.py` & `niapy-2.3.1/niapy/algorithms/basic/pso.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/basic/sca.py` & `niapy-2.3.1/niapy/algorithms/basic/sca.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/modified/__init__.py` & `niapy-2.3.1/niapy/algorithms/modified/__init__.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/modified/hba.py` & `niapy-2.3.1/niapy/algorithms/modified/hba.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/modified/hde.py` & `niapy-2.3.1/niapy/algorithms/modified/hde.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/modified/hsaba.py` & `niapy-2.3.1/niapy/algorithms/modified/hsaba.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/modified/jde.py` & `niapy-2.3.1/niapy/algorithms/modified/jde.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/modified/plba.py` & `niapy-2.3.1/niapy/algorithms/modified/plba.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/modified/saba.py` & `niapy-2.3.1/niapy/algorithms/modified/saba.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/modified/shade.py` & `niapy-2.3.1/niapy/algorithms/modified/shade.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/other/__init__.py` & `niapy-2.3.1/niapy/algorithms/other/__init__.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/other/aso.py` & `niapy-2.3.1/niapy/algorithms/other/aso.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/other/hc.py` & `niapy-2.3.1/niapy/algorithms/other/hc.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/other/mts.py` & `niapy-2.3.1/niapy/algorithms/other/mts.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/other/nmm.py` & `niapy-2.3.1/niapy/algorithms/other/nmm.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/other/rs.py` & `niapy-2.3.1/niapy/algorithms/other/rs.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/algorithms/other/sa.py` & `niapy-2.3.1/niapy/algorithms/other/sa.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/callbacks.py` & `niapy-2.3.1/niapy/callbacks.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/__init__.py` & `niapy-2.3.1/niapy/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/ackley.py` & `niapy-2.3.1/niapy/problems/ackley.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/alpine.py` & `niapy-2.3.1/niapy/problems/alpine.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/bent_cigar.py` & `niapy-2.3.1/niapy/problems/bent_cigar.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/chung_reynolds.py` & `niapy-2.3.1/niapy/problems/chung_reynolds.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/cosine_mixture.py` & `niapy-2.3.1/niapy/problems/cosine_mixture.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/csendes.py` & `niapy-2.3.1/niapy/problems/csendes.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/discus.py` & `niapy-2.3.1/niapy/problems/discus.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/dixon_price.py` & `niapy-2.3.1/niapy/problems/dixon_price.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/elliptic.py` & `niapy-2.3.1/niapy/problems/elliptic.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/griewank.py` & `niapy-2.3.1/niapy/problems/griewank.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/happy_cat.py` & `niapy-2.3.1/niapy/problems/happy_cat.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/hgbat.py` & `niapy-2.3.1/niapy/problems/hgbat.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/katsuura.py` & `niapy-2.3.1/niapy/problems/katsuura.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/levy.py` & `niapy-2.3.1/niapy/problems/levy.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/michalewicz.py` & `niapy-2.3.1/niapy/problems/michalewicz.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/perm.py` & `niapy-2.3.1/niapy/problems/perm.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/pinter.py` & `niapy-2.3.1/niapy/problems/pinter.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/powell.py` & `niapy-2.3.1/niapy/problems/powell.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/problem.py` & `niapy-2.3.1/niapy/problems/problem.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/qing.py` & `niapy-2.3.1/niapy/problems/qing.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/quintic.py` & `niapy-2.3.1/niapy/problems/quintic.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/rastrigin.py` & `niapy-2.3.1/niapy/problems/rastrigin.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/ridge.py` & `niapy-2.3.1/niapy/problems/ridge.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/rosenbrock.py` & `niapy-2.3.1/niapy/problems/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/salomon.py` & `niapy-2.3.1/niapy/problems/salomon.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/schaffer.py` & `niapy-2.3.1/niapy/problems/schaffer.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/schumer_steiglitz.py` & `niapy-2.3.1/niapy/problems/schumer_steiglitz.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/schwefel.py` & `niapy-2.3.1/niapy/problems/schwefel.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/sphere.py` & `niapy-2.3.1/niapy/problems/sphere.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/step.py` & `niapy-2.3.1/niapy/problems/step.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/stepint.py` & `niapy-2.3.1/niapy/problems/stepint.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/styblinski_tang.py` & `niapy-2.3.1/niapy/problems/styblinski_tang.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/sum_squares.py` & `niapy-2.3.1/niapy/problems/sum_squares.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/trid.py` & `niapy-2.3.1/niapy/problems/trid.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/weierstrass.py` & `niapy-2.3.1/niapy/problems/weierstrass.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/whitley.py` & `niapy-2.3.1/niapy/problems/whitley.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/problems/zakharov.py` & `niapy-2.3.1/niapy/problems/zakharov.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/runner.py` & `niapy-2.3.1/niapy/runner.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/task.py` & `niapy-2.3.1/niapy/task.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/util/__init__.py` & `niapy-2.3.1/niapy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/util/argparser.py` & `niapy-2.3.1/niapy/util/argparser.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/util/array.py` & `niapy-2.3.1/niapy/util/array.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/util/factory.py` & `niapy-2.3.1/niapy/util/factory.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/util/random.py` & `niapy-2.3.1/niapy/util/random.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/niapy/util/repair.py` & `niapy-2.3.1/niapy/util/repair.py`

 * *Files identical despite different names*

### Comparing `niapy-2.1.0/pyproject.toml` & `niapy-2.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "niapy"
-version = "2.1.0"
+version = "2.3.1"
 description = "Python micro framework for building nature-inspired algorithms."
 authors = ["NiaOrg <niapy.organization@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/NiaOrg/NiaPy"
 repository = "https://github.com/NiaOrg/NiaPy"
 documentation = "https://niapy.org/en/stable/"
@@ -32,15 +32,15 @@
 python = ">=3.9,<3.13"
 numpy = "^1.26.1"
 pandas = "^2.1.1"
 openpyxl = "^3.1.2"
 matplotlib = "^3.8.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.4.2"
+pytest = ">=7.4.2,<9.0.0"
 pytest-cov = "^4.1.0"
 pytest-randomly = "^3.15.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
@@ -48,20 +48,20 @@
 sphinx-rtd-theme = "^1.3.0"
 
 [tool.poetry.group.release]
 optional = true
 
 [tool.poetry.group.release.dependencies]
 git-changelog = "^2.4.0"
-bump-my-version = "^0.15.3"
+bump-my-version = ">=0.15.3,<0.18.0"
 pandoc = "^2.3"
 
 
 [tool.bumpversion]
-current_version = "2.1.0"
+current_version = "2.3.1"
 allow_dirty = true
 commit = true
 tag = true
 tag_name = "v{new_version}"
 parse = '(?P<major>\d+)\.(?P<minor>\d+)(\.(?P<patch>\d+))(\-?((rc)?(?P<rc>\d+))?)'
 serialize = [
 	"{major}.{minor}.{patch}rc{rc}",
@@ -80,21 +80,27 @@
 
 [[tool.bumpversion.files]]
 filename = "docs/source/conf.py"
 search = "release = u'{current_version}'"
 replace = "release = u'{new_version}'"
 
 
+
+
+
 [tool.git-changelog]
 convention = "basic"
 in-place = true
 marker-line = "<!-- insertion marker -->"
 output = "CHANGELOG.md"
 parse-refs = true
 parse-trailers = true
 repository = "."
 provider = "github"
 template = "keepachangelog"
+
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `niapy-2.1.0/PKG-INFO` & `niapy-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niapy
-Version: 2.1.0
+Version: 2.3.1
 Summary: Python micro framework for building nature-inspired algorithms.
 Home-page: https://github.com/NiaOrg/NiaPy
 License: MIT
 Keywords: nature-inspired algorithms,evolutionary algorithms,swarm intelligence,optimization
 Author: NiaOrg
 Author-email: niapy.organization@gmail.com
 Requires-Python: >=3.9,<3.13
```

