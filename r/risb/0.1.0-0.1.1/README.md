# Comparing `tmp/risb-0.1.0.tar.gz` & `tmp/risb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu May 16 06:52:43 2024, max compression
+gzip compressed data, last modified: Fri May 17 10:28:31 2024, max compression
```

## Comparing `risb-0.1.0.tar` & `risb-0.1.1.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0      202 2024-05-16 06:52:43.000000 risb-0.1.0/.dockerignore
--rw-r--r--   0        0        0      124 2024-05-16 06:52:43.000000 risb-0.1.0/.git_archival.txt
--rw-r--r--   0        0        0       98 2024-05-16 06:52:43.000000 risb-0.1.0/.gitattributes
--rw-r--r--   0        0        0     3481 2024-05-16 06:52:43.000000 risb-0.1.0/CITATION
--rw-r--r--   0        0        0      822 2024-05-16 06:52:43.000000 risb-0.1.0/COPYRIGHT
--rw-r--r--   0        0        0     1308 2024-05-16 06:52:43.000000 risb-0.1.0/TODO.md
--rw-r--r--   0        0        0       37 2024-05-16 06:52:43.000000 risb-0.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      223 2024-05-16 06:52:43.000000 risb-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     3302 2024-05-16 06:52:43.000000 risb-0.1.0/.github/actions/setup-triqs/action.yml
--rw-r--r--   0        0        0     2752 2024-05-16 06:52:43.000000 risb-0.1.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1776 2024-05-16 06:52:43.000000 risb-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      382 2024-05-16 06:52:43.000000 risb-0.1.0/docker/Dockerfile
--rw-r--r--   0        0        0     3434 2024-05-16 06:52:43.000000 risb-0.1.0/docker/Dockerfile.dev
--rw-r--r--   0        0        0      608 2024-05-16 06:52:43.000000 risb-0.1.0/docker/Dockerfile.docs
--rw-r--r--   0        0        0      567 2024-05-16 06:52:43.000000 risb-0.1.0/docker/conda.sh
--rw-r--r--   0        0        0      332 2024-05-16 06:52:43.000000 risb-0.1.0/docker/docker-compose-dev.yml
--rw-r--r--   0        0        0      334 2024-05-16 06:52:43.000000 risb-0.1.0/docker/docker-compose-docs.yml
--rw-r--r--   0        0        0      266 2024-05-16 06:52:43.000000 risb-0.1.0/docker/docker-compose.yml
--rw-r--r--   0        0        0       10 2024-05-16 06:52:43.000000 risb-0.1.0/docs/.gitignore
--rw-r--r--   0        0        0     3376 2024-05-16 06:52:43.000000 risb-0.1.0/docs/about.md
--rw-r--r--   0        0        0     2359 2024-05-16 06:52:43.000000 risb-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      422 2024-05-16 06:52:43.000000 risb-0.1.0/docs/index.md
--rw-r--r--   0        0        0      111 2024-05-16 06:52:43.000000 risb-0.1.0/docs/install.md
--rw-r--r--   0        0        0     5636 2024-05-16 06:52:43.000000 risb-0.1.0/docs/explanations/embedding.md
--rw-r--r--   0        0        0      114 2024-05-16 06:52:43.000000 risb-0.1.0/docs/explanations/index.md
--rw-r--r--   0        0        0     2090 2024-05-16 06:52:43.000000 risb-0.1.0/docs/explanations/kweight.md
--rw-r--r--   0        0        0     3176 2024-05-16 06:52:43.000000 risb-0.1.0/docs/explanations/projectors.md
--rw-r--r--   0        0        0     2426 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/diis.md
--rw-r--r--   0        0        0     5629 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/embedding.md
--rw-r--r--   0        0        0      119 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/index.md
--rw-r--r--   0        0        0     2520 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/kweight.md
--rw-r--r--   0        0        0     7176 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/lattice_solver.md
--rw-r--r--   0        0        0     4622 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/projectors.md
--rw-r--r--   0        0        0     9168 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/quadratic_terms.md
--rw-r--r--   0        0        0    13537 2024-05-16 06:52:43.000000 risb-0.1.0/docs/tutorials/hubbard.md
--rw-r--r--   0        0        0       77 2024-05-16 06:52:43.000000 risb-0.1.0/docs/tutorials/index.md
--rw-r--r--   0        0        0     1977 2024-05-16 06:52:43.000000 risb-0.1.0/docs/tutorials/kagome.md
--rw-r--r--   0        0        0    19265 2024-05-16 06:52:43.000000 risb-0.1.0/docs/tutorials/self-consistent.md
--rw-r--r--   0        0        0     4863 2024-05-16 06:52:43.000000 risb-0.1.0/examples/bilayer_hubbard.py
--rw-r--r--   0        0        0     7530 2024-05-16 06:52:43.000000 risb-0.1.0/examples/decorated_honeycomb.py
--rw-r--r--   0        0        0     4620 2024-05-16 06:52:43.000000 risb-0.1.0/examples/hubbard.py
--rw-r--r--   0        0        0     4881 2024-05-16 06:52:43.000000 risb-0.1.0/examples/kagome_hubbard.py
--rw-r--r--   0        0        0      206 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/__init__.py
--rw-r--r--   0        0        0    17127 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/helpers.py
--rw-r--r--   0        0        0    17730 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/helpers_triqs.py
--rw-r--r--   0        0        0    27703 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/solve_lattice.py
--rw-r--r--   0        0        0      411 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/version.py
--rw-r--r--   0        0        0       84 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/embedding/__init__.py
--rw-r--r--   0        0        0     2561 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/embedding/dummy.py
--rw-r--r--   0        0        0    12048 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/embedding/embedding_atom_diag.py
--rw-r--r--   0        0        0       36 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/kweight/__init__.py
--rw-r--r--   0        0        0     1656 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/kweight/from_triqs_hartree.py
--rw-r--r--   0        0        0     4931 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/kweight/kweight.py
--rw-r--r--   0        0        0      234 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/optimize/__init__.py
--rw-r--r--   0        0        0     2969 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/optimize/diis.py
--rw-r--r--   0        0        0      640 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/optimize/linear_mixing.py
--rw-r--r--   0        0        0     6064 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/optimize/solver_newton.py
--rw-r--r--   0        0        0     1506 2024-05-16 06:52:43.000000 risb-0.1.0/tests/common.py
--rw-r--r--   0        0        0    13056 2024-05-16 06:52:43.000000 risb-0.1.0/tests/data_helpers.h5
--rw-r--r--   0        0        0     7541 2024-05-16 06:52:43.000000 risb-0.1.0/tests/test_atomdiag.py
--rw-r--r--   0        0        0     3482 2024-05-16 06:52:43.000000 risb-0.1.0/tests/test_helpers.py
--rw-r--r--   0        0        0     6360 2024-05-16 06:52:43.000000 risb-0.1.0/tests/test_latticesolver.py
--rw-r--r--   0        0        0      230 2024-05-16 06:52:43.000000 risb-0.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2024-05-16 06:52:43.000000 risb-0.1.0/LICENSE
--rw-r--r--   0        0        0     3984 2024-05-16 06:52:43.000000 risb-0.1.0/README.md
--rw-r--r--   0        0        0     1775 2024-05-16 06:52:43.000000 risb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    45795 2024-05-16 06:52:43.000000 risb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      203 2024-05-17 10:28:31.000000 risb-0.1.1/.dockerignore
+-rw-r--r--   0        0        0      125 2024-05-17 10:28:31.000000 risb-0.1.1/.git_archival.txt
+-rw-r--r--   0        0        0       99 2024-05-17 10:28:31.000000 risb-0.1.1/.gitattributes
+-rw-r--r--   0        0        0     1315 2024-05-17 10:28:31.000000 risb-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3480 2024-05-17 10:28:31.000000 risb-0.1.1/CITATION
+-rw-r--r--   0        0        0      821 2024-05-17 10:28:31.000000 risb-0.1.1/COPYRIGHT
+-rw-r--r--   0        0        0     1453 2024-05-17 10:28:31.000000 risb-0.1.1/TODO.md
+-rw-r--r--   0        0        0       38 2024-05-17 10:28:31.000000 risb-0.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      224 2024-05-17 10:28:31.000000 risb-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     3328 2024-05-17 10:28:31.000000 risb-0.1.1/.github/actions/setup-triqs/action.yml
+-rw-r--r--   0        0        0     2820 2024-05-17 10:28:31.000000 risb-0.1.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2084 2024-05-17 10:28:31.000000 risb-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      383 2024-05-17 10:28:31.000000 risb-0.1.1/docker/Dockerfile
+-rw-r--r--   0        0        0     3435 2024-05-17 10:28:31.000000 risb-0.1.1/docker/Dockerfile.dev
+-rw-r--r--   0        0        0      609 2024-05-17 10:28:31.000000 risb-0.1.1/docker/Dockerfile.docs
+-rw-r--r--   0        0        0      568 2024-05-17 10:28:31.000000 risb-0.1.1/docker/conda.sh
+-rw-r--r--   0        0        0      326 2024-05-17 10:28:31.000000 risb-0.1.1/docker/docker-compose-dev.yml
+-rw-r--r--   0        0        0      328 2024-05-17 10:28:31.000000 risb-0.1.1/docker/docker-compose-docs.yml
+-rw-r--r--   0        0        0      260 2024-05-17 10:28:31.000000 risb-0.1.1/docker/docker-compose.yml
+-rw-r--r--   0        0        0       11 2024-05-17 10:28:31.000000 risb-0.1.1/docs/.gitignore
+-rw-r--r--   0        0        0     3437 2024-05-17 10:28:31.000000 risb-0.1.1/docs/about.md
+-rw-r--r--   0        0        0     2400 2024-05-17 10:28:31.000000 risb-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      422 2024-05-17 10:28:31.000000 risb-0.1.1/docs/index.md
+-rw-r--r--   0        0        0      112 2024-05-17 10:28:31.000000 risb-0.1.1/docs/install.md
+-rw-r--r--   0        0        0     5572 2024-05-17 10:28:31.000000 risb-0.1.1/docs/explanations/embedding.md
+-rw-r--r--   0        0        0      113 2024-05-17 10:28:31.000000 risb-0.1.1/docs/explanations/index.md
+-rw-r--r--   0        0        0     2067 2024-05-17 10:28:31.000000 risb-0.1.1/docs/explanations/kweight.md
+-rw-r--r--   0        0        0     3155 2024-05-17 10:28:31.000000 risb-0.1.1/docs/explanations/projectors.md
+-rw-r--r--   0        0        0     2423 2024-05-17 10:28:31.000000 risb-0.1.1/docs/how-to/diis.md
+-rw-r--r--   0        0        0     5580 2024-05-17 10:28:31.000000 risb-0.1.1/docs/how-to/embedding.md
+-rw-r--r--   0        0        0      120 2024-05-17 10:28:31.000000 risb-0.1.1/docs/how-to/index.md
+-rw-r--r--   0        0        0     2523 2024-05-17 10:28:31.000000 risb-0.1.1/docs/how-to/kweight.md
+-rw-r--r--   0        0        0     7125 2024-05-17 10:28:31.000000 risb-0.1.1/docs/how-to/lattice_solver.md
+-rw-r--r--   0        0        0     4591 2024-05-17 10:28:31.000000 risb-0.1.1/docs/how-to/projectors.md
+-rw-r--r--   0        0        0     9120 2024-05-17 10:28:31.000000 risb-0.1.1/docs/how-to/quadratic_terms.md
+-rw-r--r--   0        0        0    13581 2024-05-17 10:28:31.000000 risb-0.1.1/docs/tutorials/hubbard.md
+-rw-r--r--   0        0        0       78 2024-05-17 10:28:31.000000 risb-0.1.1/docs/tutorials/index.md
+-rw-r--r--   0        0        0     1955 2024-05-17 10:28:31.000000 risb-0.1.1/docs/tutorials/kagome.md
+-rw-r--r--   0        0        0    19142 2024-05-17 10:28:31.000000 risb-0.1.1/docs/tutorials/self-consistent.md
+-rw-r--r--   0        0        0     4929 2024-05-17 10:28:31.000000 risb-0.1.1/examples/bilayer_hubbard.py
+-rw-r--r--   0        0        0     8010 2024-05-17 10:28:31.000000 risb-0.1.1/examples/decorated_honeycomb.py
+-rw-r--r--   0        0        0     4778 2024-05-17 10:28:31.000000 risb-0.1.1/examples/hubbard.py
+-rw-r--r--   0        0        0     4735 2024-05-17 10:28:31.000000 risb-0.1.1/examples/kagome_hubbard.py
+-rw-r--r--   0        0        0      340 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/__init__.py
+-rw-r--r--   0        0        0    18576 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/helpers.py
+-rw-r--r--   0        0        0    18968 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/helpers_triqs.py
+-rw-r--r--   0        0        0    29136 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/solve_lattice.py
+-rw-r--r--   0        0        0      411 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/version.py
+-rw-r--r--   0        0        0      172 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/embedding/__init__.py
+-rw-r--r--   0        0        0     2775 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/embedding/dummy.py
+-rw-r--r--   0        0        0    11884 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/embedding/embedding_atom_diag.py
+-rw-r--r--   0        0        0       79 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/kweight/__init__.py
+-rw-r--r--   0        0        0     2104 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/kweight/from_triqs_hartree.py
+-rw-r--r--   0        0        0     4761 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/kweight/kweight.py
+-rw-r--r--   0        0        0      283 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/optimize/__init__.py
+-rw-r--r--   0        0        0     2904 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/optimize/diis.py
+-rw-r--r--   0        0        0      671 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/optimize/linear_mixing.py
+-rw-r--r--   0        0        0     5765 2024-05-17 10:28:31.000000 risb-0.1.1/src/risb/optimize/solver_newton.py
+-rw-r--r--   0        0        0    13056 2024-05-17 10:28:31.000000 risb-0.1.1/tests/data_helpers.h5
+-rw-r--r--   0        0        0     7276 2024-05-17 10:28:31.000000 risb-0.1.1/tests/test_atomdiag.py
+-rw-r--r--   0        0        0     1676 2024-05-17 10:28:31.000000 risb-0.1.1/tests/test_common.py
+-rw-r--r--   0        0        0     3037 2024-05-17 10:28:31.000000 risb-0.1.1/tests/test_helpers.py
+-rw-r--r--   0        0        0     6192 2024-05-17 10:28:31.000000 risb-0.1.1/tests/test_latticesolver.py
+-rw-r--r--   0        0        0      231 2024-05-17 10:28:31.000000 risb-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2024-05-17 10:28:31.000000 risb-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3968 2024-05-17 10:28:31.000000 risb-0.1.1/README.md
+-rw-r--r--   0        0        0     2969 2024-05-17 10:28:31.000000 risb-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    45779 2024-05-17 10:28:31.000000 risb-0.1.1/PKG-INFO
```

### Comparing `risb-0.1.0/CITATION` & `risb-0.1.1/CITATION`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
   year = {2022},
   month = {May},
   publisher = {American Physical Society},
   doi = {10.1103/PhysRevB.105.205119},
   url = {https://link.aps.org/doi/10.1103/PhysRevB.105.205119}
 }
 
-# H. L. Nourse thesis which has details about RISB and our implementation. 
-# It includes other algorithms for RISB that we have used in the past that we 
+# H. L. Nourse thesis which has details about RISB and our implementation.
+# It includes other algorithms for RISB that we have used in the past that we
 # have not reimplemented.
 @phdthesis{nourse2020phd,
   doi = {10.14264/uql.2020.169},
   url = {https://doi.org/10.14264/uql.2020.169},
   publisher = {University of Queensland Library},
   author = {Henry Leonard Nourse},
   title = {Strongly correlated electrons on the decorated honeycomb lattice studied with rotationally invariant slave-boson mean-field theory}
@@ -88,8 +88,8 @@
 	DOI= "10.1051/m2an/2021069",
 	url= "https://doi.org/10.1051/m2an/2021069",
 	journal = {ESAIM: M2AN},
 	year = "2021",
 	volume = "55",
 	number = "6",
 	pages = "2785-2825",
-}
+}
```

### Comparing `risb-0.1.0/COPYRIGHT` & `risb-0.1.1/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Copyright (C) 2022-, H. L. Nourse, B. J. Powell
 Copyright (C) 2016-2022, H. L. Nourse, R. H. McKenzie, B. J. Powell
 
 risb is free software: you can redistribute it and/or modify it under the
 terms of the GNU General Public License as published by the Free Software
 Foundation, either version 3 of the License, or (at your option) any later
 version.
- 
+
 risb is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with
 risb (in the file LICENSE in this directory). If not, see
 <http://www.gnu.org/licenses/>.
```

### Comparing `risb-0.1.0/TODO.md` & `risb-0.1.1/TODO.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # risb
+
 Rotationally invariant slave-bosons.
 
 ### Todo
 
-- Add kweights tests, DIIS tests, multiple cluster tests, complex SOC tests, 
-all helpers functions (make random inputs and store, because current tests
-have too much structure)
+- Add kweights tests, DIIS tests, multiple cluster tests, complex SOC tests,
+  all helpers functions (make random inputs and store, because current tests
+  have too much structure)
 - Add helpers_triqs tests
 - Fix sensitive to initial R, Lambda guess, make more robust
 - Implement initial guess as R, pdensity, as this will likely be more robust.
 - Get static type hints working for mypy
 - Add verbose output to `LatticeSolver`
 - Add verbose output to `DIIS`
 - Maybe? Refactor `DIIS` and `NewtonSolver`
 - Explanation for why the root finders kind of suck.
-- Remove h_emb to real if real in `EmbeddingAtom` when TRIQS bumps from 
-version 3.2.0
+- Remove h_emb to real if real in `EmbeddingAtom` when TRIQS bumps from
+  version 3.2.0
 - Sort out intersphinx linking in docs
 - Helper plot functions
 - Helper functions for calculating free/total energy
 - add linting actions
 - dimer insulator to explain some different insulating states
 - change references in docs to use sphinxcontrib-bibtex
+- pytest filterwarnings are not working. They need to be for risb package only and not promote warnings to errors in third-party packages.
 
 ### In Progress
 
 - symmetry representation tutorial
 - Kagome/projectors tutorial
 - Finish TBmodels in tight-binding how-to
 - Sort out cross-referencing to API in docs
 
 ### Done ✓
+
 - Setup github actions
-- single-orbital Hubbard tutorial 
+- single-orbital Hubbard tutorial
 - action for hatchling version bump (done with tag update action)
 - pipy packaging
-- Green's function helper functions
+- Green's function helper functions
```

### Comparing `risb-0.1.0/.github/actions/setup-triqs/action.yml` & `risb-0.1.1/.github/actions/setup-triqs/action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -20,113 +20,109 @@
     default: "12"
     required: false
 
 runs:
   using: "composite"
 
   steps:
-  - name: Setup Python ${{ inputs.python-version }}
-    uses: actions/setup-python@v5
-    with:
-      python-version: ${{ inputs.python-version }}
-      allow-prereleases: true
- 
-  - name: Install updates
-    shell: bash
-    run: |
-      sudo apt-get update &&
-      sudo apt-get install -y lsb-release wget software-properties-common
-     
-  - name: Install clang
-    shell: bash
-    if: ${{ contains(inputs.cc, 'clang') }}
-    run: 
-      wget -O /tmp/llvm.sh https://apt.llvm.org/llvm.sh &&
-      sudo chmod +x /tmp/llvm.sh &&
-      sudo /tmp/llvm.sh ${{ inputs.llvm }} &&
-      sudo apt-get install -y 
+    - name: Setup Python ${{ inputs.python-version }}
+      uses: actions/setup-python@v5
+      with:
+        python-version: ${{ inputs.python-version }}
+        allow-prereleases: true
+
+    - name: Install updates
+      shell: bash
+      run: |
+        sudo apt-get update &&
+        sudo apt-get install -y lsb-release wget software-properties-common
+
+    - name: Install clang
+      shell: bash
+      if: ${{ contains(inputs.cc, 'clang') }}
+      run: wget -O /tmp/llvm.sh https://apt.llvm.org/llvm.sh &&
+        sudo chmod +x /tmp/llvm.sh &&
+        sudo /tmp/llvm.sh ${{ inputs.llvm }} &&
+        sudo apt-get install -y
         clang-${{ inputs.llvm }}
         lldb-${{ inputs.llvm }}
-        libclang-${{ inputs.llvm }}-dev 
-        libc++-${{ inputs.llvm }}-dev 
-        libc++abi-${{ inputs.llvm }}-dev 
+        libclang-${{ inputs.llvm }}-dev
+        libc++-${{ inputs.llvm }}-dev
+        libc++abi-${{ inputs.llvm }}-dev
         libomp-${{ inputs.llvm }}-dev &&
-      echo "CXXFLAGS=-stdlib=libc++" >> $GITHUB_ENV
-      
-  - name: Install gcc
-    shell: bash
-    if: ${{ contains(inputs.cc, 'gcc') }}
-    run:
-      sudo apt-get install -y 
+        echo "CXXFLAGS=-stdlib=libc++" >> $GITHUB_ENV
+
+    - name: Install gcc
+      shell: bash
+      if: ${{ contains(inputs.cc, 'gcc') }}
+      run: sudo apt-get install -y
         g++-${{ inputs.gcc-version }}
 
-  - name: Install ubuntu dependencies
-    shell: bash
-    run:
-      sudo apt-get install -y 
-        cmake 
-        gfortran 
-        git 
-        hdf5-tools 
-        libfftw3-dev 
-        libgfortran5 
-        libgmp-dev 
-        libhdf5-dev 
-        libblas-dev 
-        liblapack-dev 
-        libboost-dev 
-        libopenmpi-dev 
-        openmpi-bin 
-        openmpi-common 
+    - name: Install ubuntu dependencies
+      shell: bash
+      run: sudo apt-get install -y
+        cmake
+        gfortran
+        git
+        hdf5-tools
+        libfftw3-dev
+        libgfortran5
+        libgmp-dev
+        libhdf5-dev
+        libblas-dev
+        liblapack-dev
+        libboost-dev
+        libopenmpi-dev
+        openmpi-bin
+        openmpi-common
         python3-dev
-      
-  - name: Install python dependencies
-    shell: bash
-    run:
-      python -m pip install 
-        mako 
-        mpi4py 
-        h5py 
-        numpy 
-        scipy 
-        clang 
-
-  - name: Setup clang environment
-    shell: bash
-    if: ${{ contains(inputs.cc, 'clang') }}
-    run: |
-      echo "CC=${{ inputs.cc }}-${{ inputs.llvm }}" >> $GITHUB_ENV
-      echo "CXX=${{ inputs.cxx }}-${{ inputs.llvm }}" >> $GITHUB_ENV
-         
-  - name: Setup gcc environment
-    shell: bash
-    if: ${{ contains(inputs.cc, 'gcc') }}
-    run: |
-      echo "CC=${{ inputs.cc }}-${{ inputs.gcc-version }}" >> $GITHUB_ENV
-      echo "CXX=${{ inputs.cxx }}-${{ inputs.gcc-version }}" >> $GITHUB_ENV
-      
-  - name: Cache build TRIQS
-    id: build-triqs
-    uses: actions/cache@v4
-    with:
-      path: triqs
-      key: triqs-${{ inputs.os }}-${{ inputs.python-version }} ${{ inputs.cc }}-${{ inputs.llvm }}-${{ inputs.gcc-version }}
-
-  - name: Build TRIQS
-    shell: bash
-    if: steps.build-triqs.outputs.cache-hit != 'true'
-    run: |
-      git clone https://github.com/TRIQS/triqs
-      mkdir triqs/build && cd triqs/build
-      cmake .. -DCMAKE_INSTALL_PREFIX=$HOME/triqs_install -DBuild_Documentation=OFF -DBuild_Tests=OFF
-      make -j1 VERBOSE=1
-      cd ../../
-          
-  - name: Install TRIQS
-    shell: bash
-    run: |
-      cd triqs/build && make install && cd ../../
-      echo "TRIQS_INSTALL=$HOME/triqs_install" >> $GITHUB_ENV
+
+    - name: Install python dependencies
+      shell: bash
+      run: python -m pip install
+        mako
+        mpi4py
+        h5py
+        numpy
+        scipy
+        clang
+
+    - name: Setup clang environment
+      shell: bash
+      if: ${{ contains(inputs.cc, 'clang') }}
+      run: |
+        echo "CC=${{ inputs.cc }}-${{ inputs.llvm }}" >> $GITHUB_ENV
+        echo "CXX=${{ inputs.cxx }}-${{ inputs.llvm }}" >> $GITHUB_ENV
+
+    - name: Setup gcc environment
+      shell: bash
+      if: ${{ contains(inputs.cc, 'gcc') }}
+      run: |
+        echo "CC=${{ inputs.cc }}-${{ inputs.gcc-version }}" >> $GITHUB_ENV
+        echo "CXX=${{ inputs.cxx }}-${{ inputs.gcc-version }}" >> $GITHUB_ENV
+
+    - name: Cache build TRIQS
+      id: build-triqs
+      uses: actions/cache@v4
+      with:
+        path: triqs
+        key: triqs-${{ inputs.os }}-${{ inputs.python-version }} ${{ inputs.cc }}-${{ inputs.llvm }}-${{ inputs.gcc-version }}
+
+    - name: Build TRIQS
+      shell: bash
+      if: steps.build-triqs.outputs.cache-hit != 'true'
+      run: |
+        git clone https://github.com/TRIQS/triqs
+        mkdir triqs/build && cd triqs/build
+        cmake .. -DCMAKE_INSTALL_PREFIX=$HOME/triqs_install -DBuild_Documentation=OFF -DBuild_Tests=OFF
+        make -j1 VERBOSE=1
+        cd ../../
+
+    - name: Install TRIQS
+      shell: bash
+      run: |
+        cd triqs/build && make install && cd ../../
+        echo "TRIQS_INSTALL=$HOME/triqs_install" >> $GITHUB_ENV
 
 branding:
   icon: "package"
-  color: "purple"
+  color: "purple"
```

### Comparing `risb-0.1.0/.github/workflows/cd.yml` & `risb-0.1.1/.github/workflows/cd.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,120 +7,119 @@
       - main
 
 concurrency:
   group: "pages"
   cancel-in-progress: true
 
 jobs:
-
   bump-version:
     runs-on: ubuntu-latest
     permissions:
       id-token: write
       contents: write
-    
+
     steps:
-    - uses: actions/checkout@v4
-      with:
-        fetch-depth: 0
-    
-    - name: Bump version and push tag
-      id: tag_version
-      uses: mathieudutour/github-tag-action@v6.2
-      with:
-        github_token: ${{ secrets.GITHUB_TOKEN }}
-
-    - name: Create a GitHub release
-      uses: ncipollo/release-action@v1
-      with:
-        tag: ${{ steps.tag_version.outputs.new_tag }}
-        name: Release ${{ steps.tag_version.outputs.new_tag }}
-        body: ${{ steps.tag_version.outputs.changelog }}
-      
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+
+      - name: Bump version and push tag
+        id: tag_version
+        uses: mathieudutour/github-tag-action@v6.2
+        with:
+          github_token: ${{ secrets.GITHUB_TOKEN }}
+
+      - name: Create a GitHub release
+        uses: ncipollo/release-action@v1
+        with:
+          tag: ${{ steps.tag_version.outputs.new_tag }}
+          name: Release ${{ steps.tag_version.outputs.new_tag }}
+          body: ${{ steps.tag_version.outputs.changelog }}
+
   build-docs:
     needs: [bump-version]
     runs-on: ubuntu-22.04
-    
+
     steps:
-    - uses: actions/checkout@v4
-      with:
-        fetch-depth: 0
-
-    - name: Setup Python 3.10 and TRIQS
-      uses: ./.github/actions/setup-triqs
-      with:
-        python-version: "3.10"
-      
-    - name: Install risb and docs dependencies
-      run: |
-        source $TRIQS_INSTALL/share/triqs/triqsvars.sh
-        python -m pip install .[docs]
-
-    - name: Build docs
-      run: |
-        source $TRIQS_INSTALL/share/triqs/triqsvars.sh
-        sphinx-apidoc -o docs/api --module-first --no-toc --force --separate src/risb
-        sphinx-build -b html -n -T docs docs/_build
-
-    - name: Upload docs artifact
-      uses: actions/upload-artifact@v4
-      with:
-        name: docs-build
-        path: docs/_build
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+
+      - name: Setup Python 3.10 and TRIQS
+        uses: ./.github/actions/setup-triqs
+        with:
+          python-version: "3.10"
+
+      - name: Install risb and docs dependencies
+        run: |
+          source $TRIQS_INSTALL/share/triqs/triqsvars.sh
+          python -m pip install .[docs]
+
+      - name: Build docs
+        run: |
+          source $TRIQS_INSTALL/share/triqs/triqsvars.sh
+          sphinx-apidoc -o docs/api --module-first --no-toc --force --separate src/risb
+          sphinx-build -b html -n -T docs docs/_build
+
+      - name: Upload docs artifact
+        uses: actions/upload-artifact@v4
+        with:
+          name: docs-build
+          path: docs/_build
 
   deploy-docs:
     needs: [build-docs]
     runs-on: ubuntu-latest
     permissions:
       contents: read
       pages: write
       id-token: write
-    
+
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
-    
+
     name: Deploy docs
     steps:
-    - uses: actions/checkout@v4
-      
-    - name: Setup Pages
-      id: pages
-      uses: actions/configure-pages@v5
-
-    - name: Download docs artifact
-      uses: actions/download-artifact@v4
-      with:
-        name: docs-build
-        path: _site
-
-    - name: Upload artifact
-      uses: actions/upload-pages-artifact@v3
-
-    - name: Deploy to GitHub Pages
-      id: deployment
-      uses: actions/deploy-pages@v4
+      - uses: actions/checkout@v4
+
+      - name: Setup Pages
+        id: pages
+        uses: actions/configure-pages@v5
+
+      - name: Download docs artifact
+        uses: actions/download-artifact@v4
+        with:
+          name: docs-build
+          path: _site
+
+      - name: Upload artifact
+        uses: actions/upload-pages-artifact@v3
+
+      - name: Deploy to GitHub Pages
+        id: deployment
+        uses: actions/deploy-pages@v4
 
   dist:
     needs: [bump-version]
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v4
-      with:
-        fetch-depth: 0
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
 
-    - uses: hynek/build-and-inspect-python-package@v2
+      - uses: hynek/build-and-inspect-python-package@v2
 
   publish:
     needs: [dist]
     environment: pypi
     permissions:
       id-token: write
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/download-artifact@v4
         with:
           name: Packages
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@release/v1
+      - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `risb-0.1.0/.github/workflows/ci.yml` & `risb-0.1.1/.github/workflows/ci.yml`

 * *Files 27% similar despite different names*

```diff
@@ -7,50 +7,69 @@
       - main
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
-
   build:
-    
     strategy:
       fail-fast: true
       matrix:
         include:
-          - {os: "ubuntu-22.04", python-version: "3.10", cc: "gcc", cxx: "g++", llvm: "15", gcc-version: "12"}
-          - {os: "ubuntu-22.04", python-version: "3.11", cc: "gcc", cxx: "g++", llvm: "15", gcc-version: "12"}
-          - {os: "ubuntu-22.04", python-version: "3.12", cc: "gcc", cxx: "g++", llvm: "15", gcc-version: "12"}
+          - {
+              os: "ubuntu-22.04",
+              python-version: "3.10",
+              cc: "gcc",
+              cxx: "g++",
+              llvm: "15",
+              gcc-version: "12",
+            }
+          - {
+              os: "ubuntu-22.04",
+              python-version: "3.11",
+              cc: "gcc",
+              cxx: "g++",
+              llvm: "15",
+              gcc-version: "12",
+            }
+          - {
+              os: "ubuntu-22.04",
+              python-version: "3.12",
+              cc: "gcc",
+              cxx: "g++",
+              llvm: "15",
+              gcc-version: "12",
+            }
           #- {os: "ubuntu-22.04", python-version: "3.10", cc: "clang", cxx: "clang++", llvm: "15", gcc-version: "12"}
           #- {os: "ubuntu-22.04", python-version: "3.11", cc: "clang", cxx: "clang++", llvm: "15", gcc-version: "12"}
-  
+
     runs-on: ${{ matrix.os }}
-    
+
     name: Test Python ${{ matrix.python-version }}
     steps:
-    - uses: actions/checkout@v4
-      
-    - name: Setup Python ${{ matrix.python-version }} and TRIQS
-      uses: ./.github/actions/setup-triqs
-      with:
-        python-version: ${{ matrix.python-version }}
-        cc: ${{ matrix.cc }}
-        cxx: ${{ matrix.cxx }}
-        llvm: ${{ matrix.llvm }}
-        gcc-version: ${{ matrix.gcc-version }}
-      
-    - name: Install risb
-      run: |
-        source $TRIQS_INSTALL/share/triqs/triqsvars.sh
-        python -m pip install -e .[test,docs]
-      
-    - name: Test risb
-      run: |
-        source $TRIQS_INSTALL/share/triqs/triqsvars.sh
-        python -m pytest
-    
-    - name: Test docs
-      run: |
-        source $TRIQS_INSTALL/share/triqs/triqsvars.sh
-        sphinx-apidoc -o docs/api --module-first --no-toc --force --separate src/risb
-        sphinx-build -b html -n -T docs docs/_build
+      - uses: actions/checkout@v4
+
+      - name: Setup Python ${{ matrix.python-version }} and TRIQS
+        uses: ./.github/actions/setup-triqs
+        with:
+          python-version: ${{ matrix.python-version }}
+          cc: ${{ matrix.cc }}
+          cxx: ${{ matrix.cxx }}
+          llvm: ${{ matrix.llvm }}
+          gcc-version: ${{ matrix.gcc-version }}
+
+      - name: Install risb
+        run: |
+          source $TRIQS_INSTALL/share/triqs/triqsvars.sh
+          python -m pip install -e .[test,docs]
+
+      - name: Test risb
+        run: |
+          source $TRIQS_INSTALL/share/triqs/triqsvars.sh
+          python -m pytest
+
+      - name: Test docs
+        run: |
+          source $TRIQS_INSTALL/share/triqs/triqsvars.sh
+          sphinx-apidoc -o docs/api --module-first --no-toc --force --separate src/risb
+          sphinx-build -b html -n -T docs docs/_build
```

### Comparing `risb-0.1.0/docker/Dockerfile.dev` & `risb-0.1.1/docker/Dockerfile.dev`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,8 @@
 #RUN nox -s buld_api_docs
 #CMD nox -s docs -- --serve
 EXPOSE 8000
 ENV APPNAME=$APPNAME
 RUN sphinx-apidoc -o $BUILD/$APPNAME/docs/api --module-first --no-toc --force --separate src/risb
 CMD sphinx-autobuild -b html --host 0.0.0.0 --port 8000 -n -T $BUILD/$APPNAME/docs $BUILD/$APPNAME/docs/_build
 
-# I wish autodoc2 made better API documementation !
+# I wish autodoc2 made better API documementation !
```

### Comparing `risb-0.1.0/docker/Dockerfile.docs` & `risb-0.1.1/docker/Dockerfile.docs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 RUN pip install -e .[docs]
 
 # Build documentation
 EXPOSE 8000
 RUN sphinx-apidoc -o $BUILD/$APPNAME/docs/api --module-first --no-toc --force --separate src/risb
 CMD sphinx-autobuild -b html --host 0.0.0.0 --port 8000 -n -T $BUILD/$APPNAME/docs $BUILD/$APPNAME/docs/_build
 
-# I wish autodoc2 made better API documementation !
+# I wish autodoc2 made better API documementation !
```

### Comparing `risb-0.1.0/docker/conda.sh` & `risb-0.1.1/docker/conda.sh`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
 $HOME/miniconda/bin/conda init
 source $HOME/.bashrc
 # Will only work for intel/amd because conda-forge has no aarch64 for TRIQS
 conda install -c conda-forge triqs
 python3 -m pip install -e .
 python3 -m pip install -e .[test]
-python3 -m pip install -e .[docs]
+python3 -m pip install -e .[docs]
```

### Comparing `risb-0.1.0/docs/about.md` & `risb-0.1.1/docs/about.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 ## Authors
 
 Maintained by
 
 [@thenoursehorse](https://github.com/thenoursehorse) H. L. Nourse (Okinawa Institute of Science and Technology)
 
-Originally authored by 
+Originally authored by
 
 H. L. Nourse
 
 with advisors
 
 [B. J. Powell](https://people.smp.uq.edu.au/BenPowell/) (The University of Queensland)
 
 [R. H. McKenzie](https://condensedconcepts.blogspot.com/) (The University of Queensland)
 
 for the PhD thesis
 
-[*Strongly correlated electrons on the decorated honeycomb lattice studied with 
-rotationally invariant slave-boson mean-field theory* (2020)](https://doi.org/10.14264/uql.2020.169)
+[_Strongly correlated electrons on the decorated honeycomb lattice studied with
+rotationally invariant slave-boson mean-field theory_ (2020)](https://doi.org/10.14264/uql.2020.169)
 
 :::{include} ../README.md
 :start-after: <!-- CITATION-START -->
 :end-before: <!-- CITATION-END -->
 :::
 
 You may also find the following papers relevant:
@@ -32,55 +32,60 @@
 
 [H. L. Nourse, Ross H. McKenzie, and B. J. Powell Phys. Rev. B **105**, 205119 (2022)](https://doi.org/10.1103/PhysRevB.105.205119)
 
 % :download:`BibTeX file of citations <risb.bib>`
 
 ## Literature of original theory
 
-Slave-bosons as introduced by Kotliar and Ruckenstein[^Kotliar1986] was 
-extended to the {{RISB}} formalism by Lechermann, 
-et al.[^Lechermann2007]. The implementation in this project uses the 
-embedding construction as introduced by 
-Lanatà, et al.[^Lanata2015] [^Lanata2017]. The above papers should also be 
+Slave-bosons as introduced by Kotliar and Ruckenstein[^Kotliar1986] was
+extended to the {{RISB}} formalism by Lechermann,
+et al.[^Lechermann2007]. The implementation in this project uses the
+embedding construction as introduced by
+Lanatà, et al.[^Lanata2015] [^Lanata2017]. The above papers should also be
 appropriately cited.
 
 ## Embedding solvers
 
 % Fix class links
+
 1. `EmbeddingAtomDiag` uses the [TRIQS](https://triqs.github.io/)[^Parcolett2015] library.
 
-%1. `EmbeddingED` uses [TRIQS](https://triqs.github.io/)[^Parcolett2015] and 
+%1. `EmbeddingED` uses [TRIQS](https://triqs.github.io/)[^Parcolett2015] and
 %[arpack-ng](https://github.com/opencollab/arpack-ng) with the
 %[ezARPACK](https://krivenko.github.io/ezARPACK/) wrapper[^Krivenko2022].
 
 ## License
 
 [GNU General Public License, version 3](http://www.gnu.org/licenses/gpl.html)
 
-
-
-[^Kotliar1986]: [G. Kotliar and A. E. Ruckenstein, 
-*New Functional Integral Approach to Strongly Correlated Fermi Systems: 
-The Gutzwiller Approximation as a Saddle Point*, 
-Phys. Rev. Lett. **57**, 1362 (1986)](https://doi.org/10.1103/PhysRevLett.57.1362)
-
-[^Lechermann2007]: [F. Lechermann, A. Georges, G. Kotliar, and O. Parcollet, 
-*Rotationally invariant slave-boson formalism and momentum dependence of the 
-quasiparticle weight*, 
-Phys. Rev.B **76**, 155102 (2007)](https://doi.org/10.1103/PhysRevB.76.155102)
-
-[^Lanata2015]: [N. Lanatà, Y.-X. Yao, C.-Z. Wang, K.-M. Ho, and G. Kotliar, 
-*Phase Diagram and Electronic Structure of Praseodymium and Plutonium*, 
-Phys. Rev. X **5**, 011008 (2015)](https://doi.org/10.1103/PhysRevX.5.011008)
-
-[^Lanata2017]: [Lanatà, Y.-X. Yao, X. Deng, V. Dobrosavljević, and G. Kotliar, 
-*Slave Boson Theory of Orbital Differentiation with Crystal Field Effects: 
-Application to UO<sub>2</sub>*, 
-Phys. Rev. Lett. **118**, 126401 (2017)](https://doi.org/10.1103/PhysRevLett.118.126401)
-
-[^Parcolett2015]: [O. Parcollet, M. Ferrero, T. Ayral, H. Hafermann, I. Krivenko, 
-L. Messio, and P. Seth, *TRIQS: A toolbox for research on interacting quantum systems*, 
-Comp. Phys. Comm. **196**, 398-415 (2015)](https://doi.org/10.1016/j.cpc.2015.04.023)
-
-[^Krivenko2022]: [I. Krivenko, *ezARPACK - ezARPACK - a C++ ARPACK-NG wrapper 
-compatible with multiple matrix/vector algebra libraries: Release 1.0*, 
-10.5281/zenodo.3930203 (2022).](https://doi.org/10.5281/zenodo.3930202)
+[^Kotliar1986]:
+    [G. Kotliar and A. E. Ruckenstein,
+    _New Functional Integral Approach to Strongly Correlated Fermi Systems:
+    The Gutzwiller Approximation as a Saddle Point_,
+    Phys. Rev. Lett. **57**, 1362 (1986)](https://doi.org/10.1103/PhysRevLett.57.1362)
+
+[^Lechermann2007]:
+    [F. Lechermann, A. Georges, G. Kotliar, and O. Parcollet,
+    _Rotationally invariant slave-boson formalism and momentum dependence of the
+    quasiparticle weight_,
+    Phys. Rev.B **76**, 155102 (2007)](https://doi.org/10.1103/PhysRevB.76.155102)
+
+[^Lanata2015]:
+    [N. Lanatà, Y.-X. Yao, C.-Z. Wang, K.-M. Ho, and G. Kotliar,
+    _Phase Diagram and Electronic Structure of Praseodymium and Plutonium_,
+    Phys. Rev. X **5**, 011008 (2015)](https://doi.org/10.1103/PhysRevX.5.011008)
+
+[^Lanata2017]:
+    [Lanatà, Y.-X. Yao, X. Deng, V. Dobrosavljević, and G. Kotliar,
+    _Slave Boson Theory of Orbital Differentiation with Crystal Field Effects:
+    Application to UO<sub>2</sub>_,
+    Phys. Rev. Lett. **118**, 126401 (2017)](https://doi.org/10.1103/PhysRevLett.118.126401)
+
+[^Parcolett2015]:
+    [O. Parcollet, M. Ferrero, T. Ayral, H. Hafermann, I. Krivenko,
+    L. Messio, and P. Seth, _TRIQS: A toolbox for research on interacting quantum systems_,
+    Comp. Phys. Comm. **196**, 398-415 (2015)](https://doi.org/10.1016/j.cpc.2015.04.023)
+
+[^Krivenko2022]:
+    [I. Krivenko, _ezARPACK - ezARPACK - a C++ ARPACK-NG wrapper
+    compatible with multiple matrix/vector algebra libraries: Release 1.0_,
+    10.5281/zenodo.3930203 (2022).](https://doi.org/10.5281/zenodo.3930202)
```

### Comparing `risb-0.1.0/docs/conf.py` & `risb-0.1.1/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,43 @@
+# ruff: noqa: D100
 from __future__ import annotations
 
 import importlib.metadata
 
 project = "risb"
 copyright = "2016-2023 H. L. Nourse and B. J. Powell, 2016-2022 R. H. McKenzie"
 author = "H. L. Nourse"
 try:
     version = release = importlib.metadata.version("risb")
-except:
+except:  # noqa: E722
     version = release = "0.0.0"
 
 extensions = [
     "myst_parser",
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinx.ext.todo",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     # Type hinting just does not work nicely with such abstract objects
-    #"sphinx_autodoc_typehints",
+    # "sphinx_autodoc_typehints",
     "sphinx_copybutton",
-    #"autodoc2",
+    # "autodoc2",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
 ]
 
-#autodoc2_packages = [
+# autodoc2_packages = [
 #    "../src/risb",
-#]
+# ]
 #
-#autodoc2_hidden_objects = [
+# autodoc2_hidden_objects = [
 #    "private",
-#]
+# ]
 
 # Don't show typehints/annotations
 autodoc_typehints = "none"
 
 source_suffix = [".rst", ".md"]
 exclude_patterns = [
     "_build",
@@ -72,27 +73,27 @@
     "tasklist",
     "linkify",
 ]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
-    "scipy": ('https://docs.scipy.org/doc/scipy/', None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/", None),
     # I don't think TRIQS has intersphinx set up?
-    #"triqs": ('https://triqs.github.io/triqs/latest/documentation/', None),
+    # "triqs": ('https://triqs.github.io/triqs/latest/documentation/', None),
 }
 
 nitpick_ignore = [
     ("py:class", "_io.StringIO"),
     ("py:class", "_io.BytesIO"),
 ]
 
 always_document_param_types = True
 
 myst_substitutions = {
-    'RISB': r"{abbr}`RISB (rotationally invariant slave-bosons)`",
-    'DFT': r"{abbr}`DFT (density functional theory)`",
-    'DMFT': r"{abbr}`DMFT (dynamical mean-field theory)`",
-    'TRIQS': r"[TRIQS](https://triqs.github.io/)",
-    'DIIS': r"{abbr}`DIIS (direct inversion in the iterative subspace)`",
-    'DMRG': r"{abbr}`DMRG (density matrix renormalization group)`",
-}
+    "RISB": r"{abbr}`RISB (rotationally invariant slave-bosons)`",
+    "DFT": r"{abbr}`DFT (density functional theory)`",
+    "DMFT": r"{abbr}`DMFT (dynamical mean-field theory)`",
+    "TRIQS": r"[TRIQS](https://triqs.github.io/)",
+    "DIIS": r"{abbr}`DIIS (direct inversion in the iterative subspace)`",
+    "DMRG": r"{abbr}`DMRG (density matrix renormalization group)`",
+}
```

### Comparing `risb-0.1.0/docs/explanations/embedding.md` & `risb-0.1.1/docs/explanations/embedding.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,136 +1,136 @@
 # About the embedding Hamiltonian
 
-The main reason the `Embedding` classes are separated is because the embedding 
-Hamiltonian is computationally the most expensive part of the {{RISB}} 
-algorithm, and quickly becomes the computational bottleneck because of the 
-exponential scaling of the Hilbert space. Other parts of our implementation 
-are certainly not the most efficient, but solving the embedding Hamiltonian 
+The main reason the `Embedding` classes are separated is because the embedding
+Hamiltonian is computationally the most expensive part of the {{RISB}}
+algorithm, and quickly becomes the computational bottleneck because of the
+exponential scaling of the Hilbert space. Other parts of our implementation
+are certainly not the most efficient, but solving the embedding Hamiltonian
 is the most important part to optimize.
 
 ## Fast track of theory
 
 :::{admonition} TODO
 :class: dropdown
 Add diagram of embedding Hamiltonian.
 :::
 
-Our goal here is to provide you the minimum ingredients needed to solve the 
-embedding Hamiltonian for {{RISB}}, possibly without having to read any of the 
-extended literature. If you have a fast implementation to solve the embedding 
-problem, it should be trivial to slot it into the rest of our {{RISB}} 
+Our goal here is to provide you the minimum ingredients needed to solve the
+embedding Hamiltonian for {{RISB}}, possibly without having to read any of the
+extended literature. If you have a fast implementation to solve the embedding
+problem, it should be trivial to slot it into the rest of our {{RISB}}
 implementation.
 
-The embedding Hamiltonian in correlated subspace $\mathcal{C}_i$ is given by 
+The embedding Hamiltonian in correlated subspace $\mathcal{C}_i$ is given by
 
 $$
 \hat{H}^{\mathrm{emb}}_i = \hat{H}^{\mathrm{loc}}_i
-+ \sum^{M_i}_{\alpha} \sum^{M_i}_{a} \left( [\mathcal{D}_i]_{a\alpha} 
++ \sum^{M_i}_{\alpha} \sum^{M_i}_{a} \left( [\mathcal{D}_i]_{a\alpha}
 \hat{c}^{\dagger}_{i\alpha} \hat{f}^{}_{ia} + \mathrm{H.c.} \right)
-+ \sum^{M_i}_{a} \sum^{M_i}_{b} [\lambda^c_i]_{ab} 
++ \sum^{M_i}_{a} \sum^{M_i}_{b} [\lambda^c_i]_{ab}
 \hat{f}^{}_{ib} \hat{f}^{\dagger}_{ia},
 $$
 
-where $\hat{c}_{i\alpha}$ is an impurity (physical electron) degree of freedom 
-and $\hat{f}_{ia}$ is a bath (quasiparticle) degree of freedom, and 
-$\mathrm{H.c.}$ is the Hermitian conjugate. The Hilbert 
-space of the bath is a copy of the physical space defined by the physical 
-electron, and so the bath is the same size as the impurity. The local 
-Hamiltonian $\hat{H}^{\mathrm{loc}}$ is defined by the problem being solved. 
-The hybridization matrix $\mathbf{D}_i$ and bath coupling matrix 
-$\mathbf{\lambda}^c_i$ are obtained from the mean-field equations in the 
-[self-consistent cycle](../tutorial/self-consistent.md). 
-
-In the normal phase (non-superconducting) {{RISB}} requires solving the ground 
-state of the $M_i$ particle sector at each iteration of the self-consistent 
-loop. Here $M_i$ is the number of degrees of freedom in the impurity 
-(sites, orbitals, and spin in the correlated subspace $\mathcal{C}_i$). Since 
-the bath is a copy of the physical space, this particle sector 
-corresponds to half-filling of the embedding Hamiltonian. Clearly, 
-compared to {{DMFT}}, this is a much simpler and smaller impurity problem to 
+where $\hat{c}_{i\alpha}$ is an impurity (physical electron) degree of freedom
+and $\hat{f}_{ia}$ is a bath (quasiparticle) degree of freedom, and
+$\mathrm{H.c.}$ is the Hermitian conjugate. The Hilbert
+space of the bath is a copy of the physical space defined by the physical
+electron, and so the bath is the same size as the impurity. The local
+Hamiltonian $\hat{H}^{\mathrm{loc}}$ is defined by the problem being solved.
+The hybridization matrix $\mathbf{D}_i$ and bath coupling matrix
+$\mathbf{\lambda}^c_i$ are obtained from the mean-field equations in the
+[self-consistent cycle](../tutorial/self-consistent.md).
+
+In the normal phase (non-superconducting) {{RISB}} requires solving the ground
+state of the $M_i$ particle sector at each iteration of the self-consistent
+loop. Here $M_i$ is the number of degrees of freedom in the impurity
+(sites, orbitals, and spin in the correlated subspace $\mathcal{C}_i$). Since
+the bath is a copy of the physical space, this particle sector
+corresponds to half-filling of the embedding Hamiltonian. Clearly,
+compared to {{DMFT}}, this is a much simpler and smaller impurity problem to
 solve, and is the biggest advantage of {{RISB}}.
 
 ## Exact diagonalization
 
-The simplest way to solve $\hat{H}^{\mathrm{emb}}$ is to use 
-exact diagonalization in the half-filled particle sector. This is what 
-`EmbeddingAtomDiag` does, and orbital sizes up to $M_i = 5$ are possible, but 
-will take a very long time. 
-One can also construct a specialized sparse exact diagonalization solver that 
-takes into account the specific symmetries that the embedding Hamiltonian is 
-allowed to have. Succinctly, only symmetry allowed $\hat{c}$ and $\hat{f}$ 
-degrees of freedom couple. This symmetry can come from, e.g., point-group 
-symmetries, spin or orbital symmetries. This kind of implementation is done in 
+The simplest way to solve $\hat{H}^{\mathrm{emb}}$ is to use
+exact diagonalization in the half-filled particle sector. This is what
+`EmbeddingAtomDiag` does, and orbital sizes up to $M_i = 5$ are possible, but
+will take a very long time.
+One can also construct a specialized sparse exact diagonalization solver that
+takes into account the specific symmetries that the embedding Hamiltonian is
+allowed to have. Succinctly, only symmetry allowed $\hat{c}$ and $\hat{f}$
+degrees of freedom couple. This symmetry can come from, e.g., point-group
+symmetries, spin or orbital symmetries. This kind of implementation is done in
 the `EmbeddingEd`.
 
 ## {{DMRG}}
 
-Another method we have employed in the past is to use {{DMRG}}, which we 
-implemented using [ITensor](https://itensor.org/). Our implementation is 
-currently very out of date and needs to be updated. Given that 
-ITensor is even easier to use now with many more helper functions, a {{DMRG}} 
+Another method we have employed in the past is to use {{DMRG}}, which we
+implemented using [ITensor](https://itensor.org/). Our implementation is
+currently very out of date and needs to be updated. Given that
+ITensor is even easier to use now with many more helper functions, a {{DMRG}}
 solver for the embedding Hamiltonion should be very easy to code.
 
 ## Obvious other avenues
 
-There is a very fast sparse exact diagonalization solver 
-[Pomerol](https://aeantipov.github.io/pomerol/) for finite-temperature 
-interacting fermions and bosons. If the Hilbert space can be restricted 
-to a specific particle sector, this could be a very fast solver for big 
+There is a very fast sparse exact diagonalization solver
+[Pomerol](https://aeantipov.github.io/pomerol/) for finite-temperature
+interacting fermions and bosons. If the Hilbert space can be restricted
+to a specific particle sector, this could be a very fast solver for big
 problems.
 
-The [QuSpin](https://quspin.github.io/QuSpin/) library is another exact 
-diagonalization solver that offers a lot of flexibility. It has Hilbert 
-space restriction and parallelization over cores using OpenMP. Because 
-of the very low-level transparancy in their user_basis class, in principle 
-it should be able to construct a specialized solver for the embedding 
+The [QuSpin](https://quspin.github.io/QuSpin/) library is another exact
+diagonalization solver that offers a lot of flexibility. It has Hilbert
+space restriction and parallelization over cores using OpenMP. Because
+of the very low-level transparancy in their user_basis class, in principle
+it should be able to construct a specialized solver for the embedding
 Hamiltonian, all within python, while still being fast.
 
 Other solvers based on Quantum Monte Carlo (QMC), NISQ devices, etc.
 
 :::{note}
-If you have any ideas for implementation, contact us and we will be happy 
-to collaborate. Or edit this page and add it to the list for someone else 
+If you have any ideas for implementation, contact us and we will be happy
+to collaborate. Or edit this page and add it to the list for someone else
 to try.
 :::
 
 ## To interface with our code
 
 :::{seealso}
-Source code for `EmbeddingAtomDiag` for more details. The code is very 
+Source code for `EmbeddingAtomDiag` for more details. The code is very
 minimal and simple.
 :::
 
-Any implementation can be used with our code provided it has the following 
+Any implementation can be used with our code provided it has the following
 class methods. A method to set the embedding Hamiltonian called as
 
 ```python
 self.set_h_emb(Lambda_c, D, h0_loc_matrix)
 ```
 
-where `Lambda_c`, `D`, and `h0_loc_matrix` are block matrices with the structure 
-dict[ndarray]. The dictionary has keys that define each block matrix stored as 
-a `numpy` array (see `gf_struct` from {{TRIQS}}). 
-`h0_loc_matrix` is a matrix that defines the non-interacting quadratic terms in 
+where `Lambda_c`, `D`, and `h0_loc_matrix` are block matrices with the structure
+dict[ndarray]. The dictionary has keys that define each block matrix stored as
+a `numpy` array (see `gf_struct` from {{TRIQS}}).
+`h0_loc_matrix` is a matrix that defines the non-interacting quadratic terms in
 $\hat{H}^{\mathrm{loc}}$.
 
-A method to solve the Hamiltonian for the ground-state in the half-filled 
-particle sector called as 
+A method to solve the Hamiltonian for the ground-state in the half-filled
+particle sector called as
 
 ```python
 self.solve(**kwargs)
 ```
 
-where `kwargs` are parameters the solver takes. A method to get the density 
-matrix of the $\hat{f}$ degrees of freedom as 
+where `kwargs` are parameters the solver takes. A method to get the density
+matrix of the $\hat{f}$ degrees of freedom as
 
 ```python
 self.get_rho_f(block)
 ```
 
-where `block` is one of the blocks in `Lambda_c` and `D`. A method to get the 
-off-diagonal density matrix of the $\hat{c}$ and $\hat{f}$ degrees of freedom 
-as 
+where `block` is one of the blocks in `Lambda_c` and `D`. A method to get the
+off-diagonal density matrix of the $\hat{c}$ and $\hat{f}$ degrees of freedom
+as
 
 ```
 self.get_rho_cf(block)
-```
+```
```

### Comparing `risb-0.1.0/docs/explanations/kweight.md` & `risb-0.1.1/docs/explanations/kweight.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 # About k-integration
 
 :::{seealso}
 [Using `SmearingKWeight`](../how-to/kweight.md).
 :::
 
-{{RISB}} requires integrating many mean-field matrices as a function of $k$. 
-The way to do this that generalizes to 
-many kinds of $k$-space integration methods is to 
-find the weight of the integral at each $k$-point. This is, e.g., how 
+{{RISB}} requires integrating many mean-field matrices as a function of $k$.
+The way to do this that generalizes to
+many kinds of $k$-space integration methods is to
+find the weight of the integral at each $k$-point. This is, e.g., how
 linear tetrahedron works and smearing methods work.
 
-The reference energy for the integration weights in {{RISB}} are the 
-eigenenergies of the single-particle Hamiltonian $\hat{H}^{\mathrm{qp}}$, 
-which change at every iteration of the self-consistent process. 
+The reference energy for the integration weights in {{RISB}} are the
+eigenenergies of the single-particle Hamiltonian $\hat{H}^{\mathrm{qp}}$,
+which change at every iteration of the self-consistent process.
 The quasiparticle Hamiltonian is given by
 
-
 All of the integrals are in the thermodynamic limit and take the form
 
 $$
-I = \lim_{\mathcal{N} \rightarrow \infty} 
+I = \lim_{\mathcal{N} \rightarrow \infty}
 \frac{1}{\mathcal{N}} \sum_k \mathbf{A}_k f(\mathbf{H}^{\mathrm{qp}}_k),
 $$
 
-where $\mathcal{N}$ is the number of unit cells, $\mathbf{A}_k$ is a matrix 
-of a generic function of $k$, and $f(\mathbf{H}^{\mathrm{qp}})$ is the 
-Fermi-Dirac distribution. The meaning of $f(\mathbf{H}^{\mathrm{qp}}_k)$ is 
+where $\mathcal{N}$ is the number of unit cells, $\mathbf{A}_k$ is a matrix
+of a generic function of $k$, and $f(\mathbf{H}^{\mathrm{qp}})$ is the
+Fermi-Dirac distribution. The meaning of $f(\mathbf{H}^{\mathrm{qp}}_k)$ is
 specifically the operation
 
 $$
-\mathbf{U}^{}_k \mathbf{U}^{\dagger}_k f(\mathbf{H}^{\mathrm{qp}}_k) 
-\mathbf{U}^{}_k \mathbf{U}^{\dagger}_k 
+\mathbf{U}^{}_k \mathbf{U}^{\dagger}_k f(\mathbf{H}^{\mathrm{qp}}_k)
+\mathbf{U}^{}_k \mathbf{U}^{\dagger}_k
 = \mathbf{U}^{}_k f(\xi^{\mathrm{qp}}_{kn}) \mathbf{U}^{\dagger}_k,
 $$
 
-where $\mathbf{U}_k$ is the matrix representation of the unitary that 
-diagonalizes $\hat{H}^{\mathrm{qp}}_k$, $\xi^{\mathrm{qp}}_{kn}$ are 
-the eigenenergies (bands) of $\hat{H}^{\mathrm{qp}}$, and 
-$f(\mathbf{\xi}^{\mathrm{qp}}_{kn})$ is a diagonal matrix of the Fermi-Dirac 
+where $\mathbf{U}_k$ is the matrix representation of the unitary that
+diagonalizes $\hat{H}^{\mathrm{qp}}_k$, $\xi^{\mathrm{qp}}_{kn}$ are
+the eigenenergies (bands) of $\hat{H}^{\mathrm{qp}}$, and
+$f(\mathbf{\xi}^{\mathrm{qp}}_{kn})$ is a diagonal matrix of the Fermi-Dirac
 distribution for each quasiparticle band $n$.
 
-The integral can be converted to a series of finite $k$-points, with an 
-appropriate integration weight such that the integral now takes the form 
+The integral can be converted to a series of finite $k$-points, with an
+appropriate integration weight such that the integral now takes the form
 
 $$
 I = \sum_k A_k w(\xi^{\mathrm{qp}}_{kn}).
 $$
 
-Most $k$-space integration methods can be reduced to different approximations 
-to choose the weighting function $w(\xi^{\mathrm{qp}}_{kn})$. 
+Most $k$-space integration methods can be reduced to different approximations
+to choose the weighting function $w(\xi^{\mathrm{qp}}_{kn})$.
 
-All of our `Solver` classes 
-require a function that takes the quasiparticle eigenenergies 
-$\xi_{kn}^{\mathrm{qp}}$ and returns the weights $w(\xi_{kn})$.
+All of our `Solver` classes
+require a function that takes the quasiparticle eigenenergies
+$\xi_{kn}^{\mathrm{qp}}$ and returns the weights $w(\xi_{kn})$.
```

### Comparing `risb-0.1.0/docs/explanations/projectors.md` & `risb-0.1.1/docs/explanations/projectors.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 # About projectors
 
 :::{seealso}
 [Using projectors](../how-to/projectors.md).
 :::
 
-Sometimes one might want to project onto a correlated subspace 
-$\mathcal{C}_i = \{ |\chi_{Rm} \rangle_i \}$ from a larger set of states 
-$\mathcal{H} = \{ |\Psi_{k \nu} \rangle \}$, where $R$ labels a reference 
+Sometimes one might want to project onto a correlated subspace
+$\mathcal{C}_i = \{ |\chi_{Rm} \rangle_i \}$ from a larger set of states
+$\mathcal{H} = \{ |\Psi_{k \nu} \rangle \}$, where $R$ labels a reference
 unit cell, $i$ labels inequivalent subspaces in the reference cell, $m$ labels
-one of the $M_i$ correlated orbitals in $\mathcal{C}_i$, $k$ labels a reciprocal 
-lattice vector $\vec{k}$, and $\nu$ labels one of the $N$ orbitals in 
-$\mathcal{H}$. It is not a requirement that $N$ is the same for each $k$. 
-
-At each $k$, the projection onto $\mathcal{C}_i$ can be encoded into 
-$M_i \times N$ rectangular matrices $\mathbf{P}_i(k)$. Any single-particle 
-quantity, represented as an $N \times N$ matrix $\mathbf{A}^{\mathcal{H}}(k)$, 
-can be projected from $\mathcal{H}$ into the correlated subspace 
+one of the $M_i$ correlated orbitals in $\mathcal{C}_i$, $k$ labels a reciprocal
+lattice vector $\vec{k}$, and $\nu$ labels one of the $N$ orbitals in
+$\mathcal{H}$. It is not a requirement that $N$ is the same for each $k$.
+
+At each $k$, the projection onto $\mathcal{C}_i$ can be encoded into
+$M_i \times N$ rectangular matrices $\mathbf{P}_i(k)$. Any single-particle
+quantity, represented as an $N \times N$ matrix $\mathbf{A}^{\mathcal{H}}(k)$,
+can be projected from $\mathcal{H}$ into the correlated subspace
 $\mathcal{C}_i$ as
 
 $$
-\mathbf{A}_i^{\mathcal{C}} = \frac{1}{\mathcal{N}} 
+\mathbf{A}_i^{\mathcal{C}} = \frac{1}{\mathcal{N}}
 \sum_k \mathbf{P}_i(k) \mathbf{A}^{\mathcal{H}}(k) \mathbf{P}^{\dagger}_i(k),
 $$
 
-where $\mathcal{N}$ is the number of unit cells on the lattice. The above is 
-called downfolding in {{DMFT}}[^Maier2005]. Assuming homogeneity such that 
-$\mathbf{A}_i^{\mathcal{C}}$ is equivalent in all unit cells, the reverse 
-process from all correlated subspaces $\mathcal{C}_i$ to $\mathcal{H}$ is 
+where $\mathcal{N}$ is the number of unit cells on the lattice. The above is
+called downfolding in {{DMFT}}[^Maier2005]. Assuming homogeneity such that
+$\mathbf{A}_i^{\mathcal{C}}$ is equivalent in all unit cells, the reverse
+process from all correlated subspaces $\mathcal{C}_i$ to $\mathcal{H}$ is
 given by
 
 $$
-\mathbf{A}^{\mathcal{H}}(k) = \sum_i 
+\mathbf{A}^{\mathcal{H}}(k) = \sum_i
 \sum_k \mathbf{P}^{\dagger}_i(k) \mathbf{A}_i^{\mathcal{C}} \mathbf{P}_i(k).
 $$
 
 The above is called upfolding in {{DMFT}}[^Maier2005].
 
-In {{RISB}} the above projectors are used to upfold the renormalization 
+In {{RISB}} the above projectors are used to upfold the renormalization
 matrix $\mathbf{\mathcal{R}}_i$ in each correlated subspace $\mathcal{C}_i$ as
 
 $$
-\mathbf{\mathcal{R}}(k) = \sum_i \sum_k \mathbf{P}^{\dagger}_i(k) 
-\mathbf{\mathcal{R}}_i 
+\mathbf{\mathcal{R}}(k) = \sum_i \sum_k \mathbf{P}^{\dagger}_i(k)
+\mathbf{\mathcal{R}}_i
 \mathbf{P}^{}_i(k),
 $$
 
-and similarly for the correlation potential matrix 
-$\mathbf{\lambda}_i$ to obtain $\mathbf{\lambda}(k)$. 
+and similarly for the correlation potential matrix
+$\mathbf{\lambda}_i$ to obtain $\mathbf{\lambda}(k)$.
 
-The reverse process is used to downfold the quasiparticle density matrix 
-$\Delta^{\mathrm{qp}}$ of $\hat{H}^{\mathrm{qp}}$ into each correlated 
+The reverse process is used to downfold the quasiparticle density matrix
+$\Delta^{\mathrm{qp}}$ of $\hat{H}^{\mathrm{qp}}$ into each correlated
 subspace $\mathcal{C}_i$ as
 
 $$
 \Delta^{\mathrm{qp}}_i = \frac{1}{\mathcal{N}} \sum_k
 \mathbf{P}_i(k)^{} f(\mathbf{H}^{\mathrm{qp}}(k)) \mathbf{P}^{\dagger}_i(k),
 $$
 
-where $f(\xi)$ is the Fermi-Dirac function, 
+where $f(\xi)$ is the Fermi-Dirac function,
 
 $$
-\mathbf{H}^{\mathrm{qp}}(k) = \mathbf{\mathcal{R}}(k) 
+\mathbf{H}^{\mathrm{qp}}(k) = \mathbf{\mathcal{R}}(k)
 \mathbf{H}_0^{\mathrm{kin}}(k) \mathbf{\mathcal{R}}^{\dagger}(k)
 + \mathbf{\lambda}(k),
 $$
 
-is the matrix representation of $\hat{H}^{\mathrm{qp}}$ at each $k$-point, 
-and $\mathbf{H}_{0}^{\mathrm{kin}}(k)$ is the non-interacting dispersion 
-matrix on the lattice that does not include the non-interacting quadratic 
+is the matrix representation of $\hat{H}^{\mathrm{qp}}$ at each $k$-point,
+and $\mathbf{H}_{0}^{\mathrm{kin}}(k)$ is the non-interacting dispersion
+matrix on the lattice that does not include the non-interacting quadratic
 terms in the subspaces $\mathcal{C}_i$.
 
-Similarly, downfolding is used to obtain the lopsided kinetic energy of the 
+Similarly, downfolding is used to obtain the lopsided kinetic energy of the
 quasiparticles as
 
 $$
-E^{c,\mathrm{qp}}_i = \frac{1}{\mathcal{N}} \sum_k 
-\mathbf{P}^{}_i(k) \mathbf{H}_0^{\mathrm{kin}}(k) 
-\mathbf{\mathcal{R}}^{\dagger}(k) f(\mathbf{H}^{\mathrm{qp}}(k)) 
+E^{c,\mathrm{qp}}_i = \frac{1}{\mathcal{N}} \sum_k
+\mathbf{P}^{}_i(k) \mathbf{H}_0^{\mathrm{kin}}(k)
+\mathbf{\mathcal{R}}^{\dagger}(k) f(\mathbf{H}^{\mathrm{qp}}(k))
 \mathbf{P}^{\dagger}_i(k).
 $$
 
-[^Maier2005]: [T. Maier, M. Jarrell, T. Pruschke, and M. H. Hettler, 
-*Quantum cluster theories*, 
-Rev. Mod. Phys. **77**, 1027 (2005)](https://doi.org/10.1016/j.cpc.2015.04.023)
+[^Maier2005]:
+    [T. Maier, M. Jarrell, T. Pruschke, and M. H. Hettler,
+    _Quantum cluster theories_,
+    Rev. Mod. Phys. **77**, 1027 (2005)](https://doi.org/10.1016/j.cpc.2015.04.023)
```

### Comparing `risb-0.1.0/docs/how-to/diis.md` & `risb-0.1.1/docs/how-to/diis.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # Using `DIIS`
 
-This guide shows you how to use and customize :py:class:`DIIS`. This is an 
+This guide shows you how to use and customize :py:class:`DIIS`. This is an
 implementation of algorithms from Ref. [^Chupin2021].
 
 ## Truncating history
 
-Like other quasi-Newton methods, {{DIIS}} uses the history of previous 
-guesses for the vector $x$ that minimizes the loss/root function $f(x)$. If 
-your system requires many iteraions to find a solution this history can become 
-computationally expensive. Sometimes the history also includes old and bad 
+Like other quasi-Newton methods, {{DIIS}} uses the history of previous
+guesses for the vector $x$ that minimizes the loss/root function $f(x)$. If
+your system requires many iteraions to find a solution this history can become
+computationally expensive. Sometimes the history also includes old and bad
 guesses that have too much influence on new gusses for $x$.
 
-To specify how big the history should be 
+To specify how big the history should be
 
 ```python
 from risb.optimize import DIIS
 
 optimize = DIIS(history_size = ...)
 ```
 
-If you want to reset the entire history after $n$ iterations 
+If you want to reset the entire history after $n$ iterations
 
 ```python
 optimize = DIIS(n_restart = ...)
 ```
 
 ## Linear mixing step
 
-Our implementation takes a single linear mixing step every `n_period` 
+Our implementation takes a single linear mixing step every `n_period`
 iterations.
 
 To change how frequently a linear mixing step is taken
 
 ```python
 optimize = DIIS(n_period = ...)
 ```
 
-The size of the linear mixing step $\alpha$ is specified in the `solve()` 
+The size of the linear mixing step $\alpha$ is specified in the `solve()`
 method as
 
 ```python
 optimize.solve(alpha = ...)
 ```
 
 ## Only linear mixing
@@ -55,15 +55,15 @@
 ```
 
 ## Arguments to `solve()`
 
 ```
 optimize.solve(fun = function to minimize,
                x0 = initial guess for x,
-               args = args for fun, 
+               args = args for fun,
                tol = stop solver when the error is less than this,
                maxiter = maxium number of iterations,
                alpha = step size in linear mixing,
 )
 ```
 
 ## Using with `LatticeSolver`
@@ -78,25 +78,24 @@
 from risb import LatticeSolver
 
 S = LatticeSolver(...,
                   root = optimize.solve
 )
 ```
 
-To pass keyword arguments to `optimize.solve()` 
+To pass keyword arguments to `optimize.solve()`
 
 ```python
 S.solve(...,
         tol = ...,
         maxiter = ...,
         alpha = ...,
 )
 ```
 
-If you want to access the default `DIIS` instance that is used it is stored 
+If you want to access the default `DIIS` instance that is used it is stored
 in `S.optimize`.
 
-
-
-[^Chupin2021]: [M. Chupin, M.-S. Dupuy, G. Legendre and É. Séré, 
-*Convergence analysis of adaptive DIIS algorithms with application to electronic ground state calculations*, 
-ESAIM: M2AN **55**, 6, 2785-2825 (2021)](https://doi.org/10.1051/m2an/2021069)
+[^Chupin2021]:
+    [M. Chupin, M.-S. Dupuy, G. Legendre and É. Séré,
+    _Convergence analysis of adaptive DIIS algorithms with application to electronic ground state calculations_,
+    ESAIM: M2AN **55**, 6, 2785-2825 (2021)](https://doi.org/10.1051/m2an/2021069)
```

### Comparing `risb-0.1.0/docs/how-to/embedding.md` & `risb-0.1.1/docs/how-to/embedding.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # Using embedding classes
 
-This guide shows you how to use the embedding classes and describes a little 
+This guide shows you how to use the embedding classes and describes a little
 bit about how they do things.
 
 :::{seealso}
 :class: dropdown
 [About the embedding Hamiltonian](../explanations/embedding.md).
 :::
 
 ## `EmbeddingAtomDiag`
 
-First a `gf_struct` object has to be created that describes the correlated 
-subspace $\mathcal{C}_i$. This object should be constructed in the same way 
-as {{TRIQS}} Green's function objects are created: as a list of tuple pairs 
-describing a symmetry block and its dimension. For example, for the $e_g$ 
-symmetry sector (two orbitals) in a system where spin is conserved, the 
-structure can be encoded as 
+First a `gf_struct` object has to be created that describes the correlated
+subspace $\mathcal{C}_i$. This object should be constructed in the same way
+as {{TRIQS}} Green's function objects are created: as a list of tuple pairs
+describing a symmetry block and its dimension. For example, for the $e_g$
+symmetry sector (two orbitals) in a system where spin is conserved, the
+structure can be encoded as
 
 ```python
 gf_struct = [ ('up_eg', 2),  ('dn_eg', 2)]
 ```
 
-Next a local Hamiltonian has to be constructed. This must 
-be a {{TRIQS}} operator that includes the interaction terms. It can include 
-the local quadratic terms in $\mathcal{C}_i$, but these can also be set 
-later on. It does not make any difference for the solvers. For example, 
-a two-orbital Hubbard model with hopping between the orbitals can be 
+Next a local Hamiltonian has to be constructed. This must
+be a {{TRIQS}} operator that includes the interaction terms. It can include
+the local quadratic terms in $\mathcal{C}_i$, but these can also be set
+later on. It does not make any difference for the solvers. For example,
+a two-orbital Hubbard model with hopping between the orbitals can be
 constructed as
 
 ```python
 from triqs.operators import Operator, c_dag, c, n
 n_orb = 2
 
 U = 1
@@ -41,53 +41,53 @@
 #V = 0.25
 #for s in ['up', 'dn']:
 #    h_int += V * ( c_dag(s, 0) * c(s, 1) + c_dag(s, 1) * c(s, 0) )
 ```
 
 ### Constructor
 
-The solver is instantiated as 
+The solver is instantiated as
 
 ```python
 from risb.embedding import EmbeddingAtomDiag
 embedding = EmbeddingAtomDiag(h_int, gf_struct)
 ```
 
-The interaction Hamiltonian is stored in `embedding.h_int` and the block 
+The interaction Hamiltonian is stored in `embedding.h_int` and the block
 matrix structure is stored in `embedding.gf_struct`.
 
 ### Setting `h_emb`
 
-Next the embedding Hamiltonian `h_emb` has to be set with 
+Next the embedding Hamiltonian `h_emb` has to be set with
 
 ```python
 embedding.set_h_emb(Lambda_c, D)
 ```
 
-where `Lambda_c` and `D` are block matrices that describe the impurity problem 
-with the structure of `gf_struct`. 
-:py:meth:`EmbeddingAtomDiag.set_h_emb` is internally called from within 
-the self-consistent loop in the {{RISB}} `Solver` classes. The hybridzation 
-term from `D` is stored as `embedding.h_hybr` and the bath hopping from 
+where `Lambda_c` and `D` are block matrices that describe the impurity problem
+with the structure of `gf_struct`.
+:py:meth:`EmbeddingAtomDiag.set_h_emb` is internally called from within
+the self-consistent loop in the {{RISB}} `Solver` classes. The hybridzation
+term from `D` is stored as `embedding.h_hybr` and the bath hopping from
 `Lambda_c` stored as `embedding.h_bath` as {{TRIQS}} operators.
 
-If the non-interacting quadratic couplings are not included in `h_int`, then 
-they must be passed as 
+If the non-interacting quadratic couplings are not included in `h_int`, then
+they must be passed as
 
 ```python
 embedding.set_h_emb(Lambda_c, D, h0_loc_matrix)
 ```
 
-where `h0_loc_matrix` is a matrix that describes the couplings, with the same 
-block matrix structure as `Lambda_c` and `D`. This is stored in 
+where `h0_loc_matrix` is a matrix that describes the couplings, with the same
+block matrix structure as `Lambda_c` and `D`. This is stored in
 `embedding.h0_loc` as a {{TRIQS}} operator.
 
 ### Setting `h_int`
 
-If you want to update the interaction terms on the impurity 
+If you want to update the interaction terms on the impurity
 
 ```python
 # A new h_int
 h_int = ...
 
 embedding.set_h_int(h_int)
 ```
@@ -96,90 +96,89 @@
 
 It is solved as
 
 ```python
 embedding.solve()
 ```
 
-There are no arguments. All `solve()` does is call 
-:py:class:`triqs.atom_diag.AtomDiag`, passes it `h_emb` 
-and restricts the Hilbert space to the half-filled particle sector. The 
-instance of this class is stored in `embedding.ad`. See the {{TRIQS}} 
+There are no arguments. All `solve()` does is call
+:py:class:`triqs.atom_diag.AtomDiag`, passes it `h_emb`
+and restricts the Hilbert space to the half-filled particle sector. The
+instance of this class is stored in `embedding.ad`. See the {{TRIQS}}
 documentation for its function.
 
 ### Getting the density matrices
 
-The single-particle density matrix of the $f$ electrons in the embedding 
+The single-particle density matrix of the $f$ electrons in the embedding
 space in one of the blocks specified by `gf_struct` is obtained as
 
 ```python
 embedding.get_rho_f(block)
 ```
 
-The off-diagonal density matrix between the $c$ and $f$ electrons is obtained 
+The off-diagonal density matrix between the $c$ and $f$ electrons is obtained
 as
 
 ```python
 embedding.get_rho_cf(block)
 ```
 
 The density matrix of the $c$ electrons is obtained as
 
 ```python
 embedding.get_rho_c(block)
 ```
 
-The three terms above give the full single-particle density matrix in the 
+The three terms above give the full single-particle density matrix in the
 embedding space.
 
 ### Local expectation values
 
-Any local expectation value of an operator `Op` in the embedding space is 
+Any local expectation value of an operator `Op` in the embedding space is
 obtained as
 
 ```python
 embedding.overlap(Op)
 ```
 
-`Op` must be a {{TRIQS}} operator. See the {{TRIQS}} manual for helper 
-functions to construct some common observables. To get observables 
-in the $f$ electrons, the structure is obtained as 
+`Op` must be a {{TRIQS}} operator. See the {{TRIQS}} manual for helper
+functions to construct some common observables. To get observables
+in the $f$ electrons, the structure is obtained as
 
 ```python
 embedding.gf_struct_bath
 ```
 
 The whole embedding space structure is obtained as
 
 ```python
 embedding.gf_struct_emb
 ```
 
-
 ## `EmbeddingDummy`
 
 If you want to have some correlated subspaces $\mathcal{C}_i$ as inequivalent,
-but they are related by some symmetry, it is not necessary to solve for the 
-ground state in each subspace separately. 
+but they are related by some symmetry, it is not necessary to solve for the
+ground state in each subspace separately.
 
-This class is a copy of another 
-`Embedding` class. For example, to create a copy of 
+This class is a copy of another
+`Embedding` class. For example, to create a copy of
 :py:class:`EmbeddingAtomDiag` it is instantiated as
 
 ```python
 from risb.embedding import EmbeddingDummy
 embedding = EmbeddingDummy(embedding = embedding_atom_diag_instance)
 ```
 
 ### Rotations
 
-If the copy is related by symmetry, you can pass `rotations` as a list of 
-functions that operate in sequence on the block matrices that 
-:py:class:`EmbeddingDummy` returns. For example, if the 
-correlated subspace is equivalent except that the spin is rotated, 
+If the copy is related by symmetry, you can pass `rotations` as a list of
+functions that operate in sequence on the block matrices that
+:py:class:`EmbeddingDummy` returns. For example, if the
+correlated subspace is equivalent except that the spin is rotated,
 like in an antiferromagnetic phase, this can be done with
 
 ```python
 from itertools import deepcopy
 def rotate_spin(A):
     B = deepcopy(A)
     B['up'] = A['dn']
@@ -187,18 +186,18 @@
     return B
 
 embedding = EmbeddingDummy(embedding = ...,
                            rotations = [rotate_spin])
 ```
 
 :::{note}
-`set_h_emb()` and `solve()` are methods that just `pass` and do nothing. 
-The density matrix functions `get_rho_f`, `get_rho_cf`, and `get_rho_c` grab 
-what is stored in `embedding_atom_diag` and rotates according to the list of 
+`set_h_emb()` and `solve()` are methods that just `pass` and do nothing.
+The density matrix functions `get_rho_f`, `get_rho_cf`, and `get_rho_c` grab
+what is stored in `embedding_atom_diag` and rotates according to the list of
 functions in `rotations`.
 :::
 
 :::{warning}
-The operator passed to `overlap` is not rotated. Likely only rotationally 
-invariant quantities make sense to calculate, which are can be obtained from 
+The operator passed to `overlap` is not rotated. Likely only rotationally
+invariant quantities make sense to calculate, which are can be obtained from
 the embedding class that `EmbeddingDummy` copies.
-:::
+:::
```

### Comparing `risb-0.1.0/docs/how-to/kweight.md` & `risb-0.1.1/docs/how-to/kweight.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Using `SmearingKWeight`
 
-This guide shows how to customize the options for the smearing $k$-space 
+This guide shows how to customize the options for the smearing $k$-space
 integration methods.
 
 ## Electron filling
 
 If you want the chemical potential $\mu$ fixed to a specific value
 
 ```python
@@ -29,32 +29,32 @@
 
 # Fixed filling
 n_target = ...
 
 kweight = SmearingKWeight(beta = beta, n_target = n_target)
 ```
 
-The fixed electron filling method uses :py:func:`scipy.optimize.brentq` to 
+The fixed electron filling method uses :py:func:`scipy.optimize.brentq` to
 find a $\mu$ that gives the correct $n$.
 
 ## Getting integration weights
 
 ```python
 # A dict[list] of energies
 energies = ...
 
 weight = kweight.update_weights(energies = energies)
 ```
 
-The method sets the appropriate $\mu$ and returns the integration weight 
+The method sets the appropriate $\mu$ and returns the integration weight
 at each $k$-point as a `dict[list]`, in the same structure as `energies`.
 
 ## Smearing method
 
-There are three smearing functions implemented. Below $\xi$ is an energy and 
+There are three smearing functions implemented. Below $\xi$ is an energy and
 $\mu$ is the chemical potential.
 
 ```python
 kweight = SmearingKWeight(...,
                           method = 'fermi' or 'gaussian' or 'methfessel-paxton',
 )
 ```
@@ -67,27 +67,27 @@
 
 The `gaussian` method is the weighting function
 
 $$
 f(\xi) = \frac{1}{2} \left[ 1 - \mathrm{erf} (\beta (\xi - \mu)) \right],
 $$
 
-where $\mathrm{erf}$ is the error function, and $f(\xi)$ is the 
+where $\mathrm{erf}$ is the error function, and $f(\xi)$ is the
 integral of the Gaussian
 
 $$
 \delta(\xi) = \frac{\beta}{\sqrt{\pi}} \exp \left[ - (\beta (\xi - \mu))^2 \right].
 $$
 
-The `methfessel-paxton` method is the $N=1$ one outlined in 
+The `methfessel-paxton` method is the $N=1$ one outlined in
 Ref. [^Methfessel1989]. You should cite this reference if you use it.
 
 ## Using own smearing function
 
-If you want to change the smearing function 
+If you want to change the smearing function
 
 ```python
 from risb.kweight import SmearingKWeight
 
 def my_smearing_function(energies : numpy.ndarray,
                          beta : float,
                          mu : float,
@@ -96,12 +96,11 @@
     return an array of weights
 
 kweight = SmearingKWeight(beta = ..., mu or n_target = ...)
 
 kweight.smear_function = my_smearing_function
 ```
 
-
-
-[^Methfessel1989]: [M. Methfessel and A. T. Paxton,
-*High-precision sampling for Brillouin-zone integration in metals*, 
-Phys. Rev. B **40**, 3616 (1989)](https://doi.org/10.1103/PhysRevB.40.3616)
+[^Methfessel1989]:
+    [M. Methfessel and A. T. Paxton,
+    _High-precision sampling for Brillouin-zone integration in metals_,
+    Phys. Rev. B **40**, 3616 (1989)](https://doi.org/10.1103/PhysRevB.40.3616)
```

### Comparing `risb-0.1.0/docs/how-to/lattice_solver.md` & `risb-0.1.1/docs/how-to/lattice_solver.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 # Using`LatticeSolver`
 
-If you want to solve a strongly correlated model on a lattice you can use 
-:py:class:`LatticeSolver`. This guide shows you how to use it for most kinds 
+If you want to solve a strongly correlated model on a lattice you can use
+:py:class:`LatticeSolver`. This guide shows you how to use it for most kinds
 of problems you might want to solve.
 
 ## Simple setup
 
-First define a non-interacting coupling matrix that describes electron 
-hopping between sites and orbitals and orbital energies, with some defined 
-block structure. E.g., if spin is a good quantum number and there are 
+First define a non-interacting coupling matrix that describes electron
+hopping between sites and orbitals and orbital energies, with some defined
+block structure. E.g., if spin is a good quantum number and there are
 $N$ orbitals per unit cell
 
 ```python
 h0_k = {'up' : k by N by N ndarray, 'dn' : k by N by N ndarray}
 ```
 
 :::{tip}
 :class: dropdown
-`h0_k` can contain any local hopping terms `h0_loc` that are in the subspace 
-$\mathcal{C}_i$. In {{RISB}} these terms are included in the embedding 
-Hamiltonian and are typically separated out from `h0_k`. `LatticeSolver` works 
-these terms out automatically. But they can be included in 
-the interactions `h_int` by hand if you want. It makes no difference to 
+`h0_k` can contain any local hopping terms `h0_loc` that are in the subspace
+$\mathcal{C}_i$. In {{RISB}} these terms are included in the embedding
+Hamiltonian and are typically separated out from `h0_k`. `LatticeSolver` works
+these terms out automatically. But they can be included in
+the interactions `h_int` by hand if you want. It makes no difference to
 the solver.
 :::
 
-Next define a class that determines the integration weight at each $k$ point 
+Next define a class that determines the integration weight at each $k$ point
 on the lattice, e.g., `class:SmearingKWeight`.
 
 ```python
 kweight = KWeightClass(...)
 ```
 
-It must have a member function `update_weights()` that is called as 
-`update_weights(energies, **kwargs)` where `energies` are a `dict[ndarray]` 
-that are the eigenenergies of `h0_k` in each block (e.g., `'up'` and `'dn'` 
+It must have a member function `update_weights()` that is called as
+`update_weights(energies, **kwargs)` where `energies` are a `dict[ndarray]`
+that are the eigenenergies of `h0_k` in each block (e.g., `'up'` and `'dn'`
 spin blocks).
 
-Next define the local block matrix structure of the correlated subspace 
-as a list of pairs. Each pair is the name of a block `bl` and the number of 
+Next define the local block matrix structure of the correlated subspace
+as a list of pairs. Each pair is the name of a block `bl` and the number of
 orbitals in that block as `n_orb`.
 
 ```python
 gf_struct = [(bl, n_orb), ...]
 ```
 
-Following the block structure of `gf_struct`, construct the interacting 
-Hamiltonian in the correlated subspace $\mathcal{C}_i$. This can include 
+Following the block structure of `gf_struct`, construct the interacting
+Hamiltonian in the correlated subspace $\mathcal{C}_i$. This can include
 the quadratic terms in a cluster if you want.
 
 ```python
 h_int = ...
 ```
 
 :::{tip}
 :class: dropdown
-The {{TRIQS}} library makes it very simple to define 
-`h_int` as second-quantized operators. All of the `Embedding` classes we 
+The {{TRIQS}} library makes it very simple to define
+`h_int` as second-quantized operators. All of the `Embedding` classes we
 provide assume that `h_int` is a {{TRIQS}} operator.
 :::
 
-Next define the class that solves in the correlated subspace $\mathcal{C}_i$ 
+Next define the class that solves in the correlated subspace $\mathcal{C}_i$
 the impurity problem for {{RISB}}.
 
 ```python
 embedding = EmbeddingClass(h_int, gf_struct)
 ```
 
 Finally, set up the solver class and solve
@@ -81,39 +81,39 @@
 ## Multiple clusters
 
 :::{seealso}
 :class: dropdown
 [Using projectors](../how-to/projectors.md) for more details and examples.
 :::
 
-If you want a correlated subspace $\mathcal{C}_i$ for each cluster $i$ you 
+If you want a correlated subspace $\mathcal{C}_i$ for each cluster $i$ you
 must construct a `gf_struct` for each subspace as a list
 
 ```python
 gf_struct = [gf_struct_1, gf_struct_2, ...]
 ```
 
-You must construct an embedding solver for each subspace $\mathcal{C}_i$ as 
-a list 
+You must construct an embedding solver for each subspace $\mathcal{C}_i$ as
+a list
 
 ```python
 embedding = [embedding_1, embedding_2, ...]
 ```
 
-You must construct a projector from the larger space of `h0_k` to each 
+You must construct a projector from the larger space of `h0_k` to each
 subspace $\mathcal{C}_i$ as a list
 
 ```python
 projectors = [projector_1, projector_2, ...]
 ```
 
-(Optional) Depending on how the problem is set up, you might also need to 
-construct a mapping from the block structure defined in each `gf_struct[i]` 
-to the larger block structure space of `h0_k`. For each correlated subspace 
-$\mathcal{C}_i$ `gf_struct_mapping_i` is a dictionary of 
+(Optional) Depending on how the problem is set up, you might also need to
+construct a mapping from the block structure defined in each `gf_struct[i]`
+to the larger block structure space of `h0_k`. For each correlated subspace
+$\mathcal{C}_i$ `gf_struct_mapping_i` is a dictionary of
 `str` $\rightarrow$ `str`
 
 ```python
 gf_struct_mapping_1 = {'bl_in_gf_struct_1' : 'bl_in_h0_k', ...}
 ...
 gf_struct_mapping = [gf_struct_mapping_1, gf_struct_mapping_2, ...]
 ```
@@ -129,35 +129,35 @@
                   ...
 )
 ```
 
 ## Enforcing symmetries
 
 :::{admonition} Thanks <3
-This way to do symmetries is unashamedly taken from 
-[TRIQS/hartree_fock](https://triqs.github.io/hartree_fock). There are other 
-ways to enforce symmetries on the matrices that we also implement at the 
-same time, but this is very easy and quick for a user to cater to their 
+This way to do symmetries is unashamedly taken from
+[TRIQS/hartree_fock](https://triqs.github.io/hartree_fock). There are other
+ways to enforce symmetries on the matrices that we also implement at the
+same time, but this is very easy and quick for a user to cater to their
 specific needs.
 :::
 
-If you want to enforce symmetries this is done through functions that are 
-called at each self-consistent loop. For example, if the block structure in 
+If you want to enforce symmetries this is done through functions that are
+called at each self-consistent loop. For example, if the block structure in
 each cluster is just the spin, paramagnetism can be enforced as
 
 ```python
 def paramagnetism(A):
     n_clusters = len(A)
     for i in range(n_clusters):
         A[i]['up'] = 0.5 * (A[i]['up'] + A[i]['dn'])
         A[i]['dn'] = A[i]['up']
     return A
 ```
 
-If you want to enforce another symmetry then you can define another 
+If you want to enforce another symmetry then you can define another
 function in a similar way
 
 ```python
 def symmetry1(A):
     do something here, maybe only to a single cluster i
     return A
 ```
@@ -171,44 +171,44 @@
 )
 ```
 
 and are called in the sequence they are given in the list.
 
 ## Using other functions to find a root
 
-If you want to change the function that finds the roots of the 
-self-consistent procedure you can specify it with 
+If you want to change the function that finds the roots of the
+self-consistent procedure you can specify it with
 
 ```python
 S = LatticeSolver(...
                   root = root,
                   ...
 )
 ```
 
-`root` is called exactly the same as what :py:func:`scipy.optimize.root` 
-requires. It must be a callable function that takes as input 
-`root(S._target_function, x0, args=, **kwargs)`. Here `S._target_function` 
-by default returns a `tuple[ndarray,ndarray]` of a flattened ndarray `x_new` 
-of a new `Lambda` and `R` matrix and a flattened ndarray `x_err` of the error 
-from the `f1` and `f2` root functions. 
+`root` is called exactly the same as what :py:func:`scipy.optimize.root`
+requires. It must be a callable function that takes as input
+`root(S._target_function, x0, args=, **kwargs)`. Here `S._target_function`
+by default returns a `tuple[ndarray,ndarray]` of a flattened ndarray `x_new`
+of a new `Lambda` and `R` matrix and a flattened ndarray `x_err` of the error
+from the `f1` and `f2` root functions.
 
-If you do not want `S._target_function` to return `x_new` and only return 
+If you do not want `S._target_function` to return `x_new` and only return
 `x_err` then you can specify
 
 ```python
 S = LatticeSolver(...
                   root = root,
                   return_x_new = False,
                   ...
 )
 ```
 
-You can change whether `x_err` is from the root functions `f1` and 
-`f2` or as a recursion from successive changes to `x` as 
+You can change whether `x_err` is from the root functions `f1` and
+`f2` or as a recursion from successive changes to `x` as
 `x_err = x_new - x` with
 
 ```python
 S = LatticeSolver(...
                   root = root,
                   error_fun = 'root' or 'recursion',
                   ...
@@ -224,27 +224,27 @@
                   return_x_new = False,
                   ...
 )
 S.solve(tol = , method = 'broyden1, hybr, krylov, etc', other kwargs = )
 ```
 
 :::{warning}
-In our experience scipy's `root` functions do not work as well as either 
-standard linear mixing or {{DIIS}} (which seems to work very well for 
+In our experience scipy's `root` functions do not work as well as either
+standard linear mixing or {{DIIS}} (which seems to work very well for
 {{RISB}}, and is the default method).
 :::
 
 ## Real or complex?
 
-In general the matrices in {{RISB}} should be complex. If you choose a basis 
-where you know they all will be real and you want to force the matrices to 
+In general the matrices in {{RISB}} should be complex. If you choose a basis
+where you know they all will be real and you want to force the matrices to
 be real you can do that with
 
 ```python
 S = LatticeSolver(...
                   force_real = True,
                   ...
 )
 ```
 
-This will make most `EmbeddingClass` solvers faster, and the other matrix 
-operations faster. For many systems forcing the matrices to be real is fine.
+This will make most `EmbeddingClass` solvers faster, and the other matrix
+operations faster. For many systems forcing the matrices to be real is fine.
```

### Comparing `risb-0.1.0/docs/how-to/projectors.md` & `risb-0.1.1/docs/how-to/projectors.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # Using projectors
 
 This guide shows you how to project onto ineqvuialent correlated subspaces
-$\mathcal{C}_i$. 
+$\mathcal{C}_i$.
 There are two technical choices for projectors.
-Projecting onto subspaces with the same block matrix structure as the larger set 
-of orbitals. Projecting onto subspaces with a different block matrix structure 
+Projecting onto subspaces with the same block matrix structure as the larger set
+of orbitals. Projecting onto subspaces with a different block matrix structure
 than the larger space, e.g., to enforce some local symmetry.
 
 :::{seealso}
 :class: dropdown
-[About projectors](../explanations/projectors.md) for more details and the 
+[About projectors](../explanations/projectors.md) for more details and the
 theory of projectors.
 :::
 
 ## Simple projectors
 
-If you want a correlated model where each inequivalent correlated subspace 
-has the same block structure as the non-interacting model, (e.g., the 
-dispersion matrix `h0_k`) you can construct very simple projection matrices 
+If you want a correlated model where each inequivalent correlated subspace
+has the same block structure as the non-interacting model, (e.g., the
+dispersion matrix `h0_k`) you can construct very simple projection matrices
 by hand.
 
-In this example each subspace $i$ is a site 
-$\alpha \in \{A, B, C\}$ with spin $\sigma$ within the three-site unit cell 
-of the kagome lattice. Hence, you can define six 
-$1 \times 3$ rectangular matrices that project onto these spaces. First 
-define a `gf_struct` for each correlated space $i$ 
+In this example each subspace $i$ is a site
+$\alpha \in \{A, B, C\}$ with spin $\sigma$ within the three-site unit cell
+of the kagome lattice. Hence, you can define six
+$1 \times 3$ rectangular matrices that project onto these spaces. First
+define a `gf_struct` for each correlated space $i$
 
 ```python
 import numpy as np
 
 # The block structure of the non-interacting space
 spin_names = ['up', 'dn']
 
@@ -49,16 +49,16 @@
 P_B = { bl : np.array( [ [0, 1, 0] ] ) for bl in spin_names }
 P_C = { bl : np.array( [ [0, 0, 1] ] ) for bl in spin_names }
 
 # A list holding each projector, 1 for each i in gf_struct
 projectors = [P_A, P_B, P_C]
 ```
 
-You do not need to define the projector for all $k$ because at each $k$ they 
-are equivalent. Next define an embedding solver for each inequivalent cluster 
+You do not need to define the projector for all $k$ because at each $k$ they
+are equivalent. Next define an embedding solver for each inequivalent cluster
 
 ```python
 from ... import EmbeddingClass
 
 # Define h_int for each cluster as a list
 ...
 
@@ -76,42 +76,42 @@
                projectors = projectors,
                ...
 )
 ```
 
 :::{note}
 :class: dropdown
-In this case a correlated subspace for each orbital within a unit cell was 
-defined. This is not a requirement. It is fine if there were multiple orbitals 
-per site and only some of them were treated as correlated, or if only some 
+In this case a correlated subspace for each orbital within a unit cell was
+defined. This is not a requirement. It is fine if there were multiple orbitals
+per site and only some of them were treated as correlated, or if only some
 sites in a unit cell were treated as correlated.
 :::
 
 ## Complicated projectors with `gf_struct_mapping`
 
-If the block matrix structure of the non-interacting Hamiltonian $\hat{H}_0$ 
-(`h0_k` in code) is not the same as the block matrix structure of the 
-correlated subspaces $\mathcal{C}_i$ then you can use a mapping dictionary 
-to go between them. 
-
-This is used if there is some well defined local 
-symmetry in the subspace $\mathcal{C}_i$ that is not valid in the larger 
-space of $\hat{H}_0$. An example is if projecting onto a $d$-orbital subspace 
-of a metal and because of crystal field symmetries the $t_{2g}$ and $e_g$ 
-orbitals make sense as block matrices in the subspace of $\mathcal{C}_i$, 
-but only spin up and spin down block matrices are possible in the larger 
+If the block matrix structure of the non-interacting Hamiltonian $\hat{H}_0$
+(`h0_k` in code) is not the same as the block matrix structure of the
+correlated subspaces $\mathcal{C}_i$ then you can use a mapping dictionary
+to go between them.
+
+This is used if there is some well defined local
+symmetry in the subspace $\mathcal{C}_i$ that is not valid in the larger
+space of $\hat{H}_0$. An example is if projecting onto a $d$-orbital subspace
+of a metal and because of crystal field symmetries the $t_{2g}$ and $e_g$
+orbitals make sense as block matrices in the subspace of $\mathcal{C}_i$,
+but only spin up and spin down block matrices are possible in the larger
 space of $\hat{H}_0$.
 
 The mapping is used as
 
 ```python
 # h0_k is a dict[ndarray] with, e.g., blocks 'up', 'dn'.
-h0_k = 
+h0_k =
 
-# The structure of each correlated subspace 
+# The structure of each correlated subspace
 gf_struct_subspace_1 = [('block_1', n_orb_1), ...]
 ...
 
 # The mapping from a correlated subspace to the space of h0_k
 gf_struct_mapping_1 = {'block_1': 'block_in_h0_k', ...}
 ...
 
@@ -125,21 +125,21 @@
 ```python
 h0_k = {'up' : ..., 'dn' : ...}
 
 gf_struct_d = [('up_eg', 2), ('dn_eg', 2), ('up_t2g', 3), ('dn_t2g', 3)]
 gf_struct_mapping_d  {'up_eg' : 'up', 'up_t2g' : 'up', 'dn_eg' : 'dn', 'dn_t2g' : 'dn'}
 ```
 
-There are several helper functions that might need a `gf_struct_mapping`, 
-either as a list of all correlated subspaces or for a single correlated 
+There are several helper functions that might need a `gf_struct_mapping`,
+either as a list of all correlated subspaces or for a single correlated
 subspace. The documentation will say what is required.
 
-If you need to use the mapping for the `Solver` classes 
+If you need to use the mapping for the `Solver` classes
 
 ```python
 from risb import LatticeSolver
 
 S = LatticeSolver(...,
                   gf_struct = list of gf_struct in each subspace,
                   gf_struct_mapping = list of mappings in each subspace,
 )
-```
+```
```

### Comparing `risb-0.1.0/docs/how-to/quadratic_terms.md` & `risb-0.1.1/docs/how-to/quadratic_terms.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Constructing tight-binding models
 
-This guide shows various methods for constructing the non-interacting 
+This guide shows various methods for constructing the non-interacting
 terms of a model required for {{RISB}}.
 
 ## Constructing `h0_k`
 
 :::{warning}
-The ordering of `k` matters for some $k$-space integration methods, e.g., 
-linear tetrahedron. If that is the case you must permute `h0_k` to the 
+The ordering of `k` matters for some $k$-space integration methods, e.g.,
+linear tetrahedron. If that is the case you must permute `h0_k` to the
 required ordering.
 :::
 
-There are many ways to construct the hopping matrices in $k$-space. Below 
-are a few of them that have been useful. Any method can be used as long 
-as it is possible to return an `numpy.ndarray` indexed as 
-`k, orb_i, orb_j` where `k` is a $k$-point on a meshgrid and `orb_i` is one of 
-the `n_orb` orbitals that corresponds to a site, orbital, or spin in a unit 
+There are many ways to construct the hopping matrices in $k$-space. Below
+are a few of them that have been useful. Any method can be used as long
+as it is possible to return an `numpy.ndarray` indexed as
+`k, orb_i, orb_j` where `k` is a $k$-point on a meshgrid and `orb_i` is one of
+the `n_orb` orbitals that corresponds to a site, orbital, or spin in a unit
 cell. These can possibly be partitioned into symmetry blocks, e.g., by spin.
 
 ### Explicit method
 
-If you have an equation for the matrix representation of $\hat{H}_0$ 
-at each $k$-point, then this is a simple way to code it to have the 
+If you have an equation for the matrix representation of $\hat{H}_0$
+at each $k$-point, then this is a simple way to code it to have the
 correct structure for {{RISB}}.
 
 First construct a Monkhorst-Pack $k$-point mesh in fractional coordinates
 
 ```python
 import numpy as np
 from itertools import product
@@ -39,15 +39,15 @@
 n_k_d = ...
 ...
 n_k_list = [n_k1, ..., n_k_d]
 
 # Total number of k-points
 n_k = np.product(n_k_list)
 
-# Shift to apply to each spatial dimension if want to move it off 
+# Shift to apply to each spatial dimension if want to move it off
 # high symmetry points. It should be a value between 0 and 1 (usually 0.5)
 shift_1 = ...
 ...
 shift_d = ...
 shift_list = [shift_1, ..., shift_d]
 
 # Method 1: Using np.meshgrid
@@ -66,16 +66,16 @@
 # Create empty mesh and populate it
 k_mesh = np.empty(shape=(n_k, d))
 for idx, coords in enumerate(product( *[range(n_k_list[i]) for i in range(len(n_k_list))] )):
     for dim in range(d):
         k_mesh[idx,dim] = (coords[dim] + shift_list[dim]) / n_k_list[dim]
 ```
 
-If your function for $\hat{H}_0$ is in a different basis then you will 
-have to rotate `k_mesh` into this basis. For example, to Cartesian 
+If your function for $\hat{H}_0$ is in a different basis then you will
+have to rotate `k_mesh` into this basis. For example, to Cartesian
 coordinates can be done as
 
 ```python
 # The unit cell lattice vectors
 a_1 = [float_1, ..., float_d]
 ...
 a_d = [float_1, ..., float_d]
@@ -113,29 +113,29 @@
 h0_k[bl_name] = np.zeros([n_k, n_orb, n_orb], dtype=complex)
 for k in range(n_k):
     h0_k[bl_name][k][...] = n_orb by n_orb array that is the function for h0_k in symmetry block bl_name
 ```
 
 ### Using {{TRIQS}} lattice tools
 
-If you know the positions of the orbitals in real-space then there is a 
-(currently poorly documented) way to do this in {{TRIQS}}. Here is some 
+If you know the positions of the orbitals in real-space then there is a
+(currently poorly documented) way to do this in {{TRIQS}}. Here is some
 complimentary information on top of what is provided by {{TRIQS}}.
 
-First specify the lattice vectors as 
+First specify the lattice vectors as
 
 ```python
 units = [a_1, ..., a_d]
 ```
 
 The allowed number of spatial dimensions is one of $d = 1, 2, 3$.
 
-Next give a list of tuples that give the positions of each atom and orbital in 
-the unit cell. The units are in fractional coordinates of the lattice vectors 
-that are specified in `units`, and there are `n_orb` total sites, orbitals, 
+Next give a list of tuples that give the positions of each atom and orbital in
+the unit cell. The units are in fractional coordinates of the lattice vectors
+that are specified in `units`, and there are `n_orb` total sites, orbitals,
 and maybe spin.
 
 ```python
 orbital_positions = [
     (frac of a_1, ... , frac of a_d),     # Position of orbital 1
     ...
     (frac of a_1, ... , frac of a_d),     # Position of orbital n_orb
@@ -155,28 +155,28 @@
 n_k_list = [n_k1, ..., n_k_d]
 
 bl = BravaisLattice(units=units)
 bz = BrillouinZone(bl)
 mk = MeshBrZone(bz, n_k_list)
 ```
 
-Next set up a dictionary of hoppings between orbitals, within a unit cell 
-and between unit cells. 
+Next set up a dictionary of hoppings between orbitals, within a unit cell
+and between unit cells.
 
-Each key in the dictionary is a tuple of the displacement from a reference unit 
+Each key in the dictionary is a tuple of the displacement from a reference unit
 cell at $\mathbf{R} = (0, \ldots, 0_d)$.
-The coordinates for this displacement is in the basis of lattice 
-vectors $\vec{a}_1, \ldots, \vec{a}_d$. For example, in two-dimensions, a 
-displacement by $\vec{a}_1$ is the key `(1,0)`. A displacement by 
-$2\vec{a}_1 + \vec{a}_2$ is the key `(2,1)`. Generally, the displacements are 
+The coordinates for this displacement is in the basis of lattice
+vectors $\vec{a}_1, \ldots, \vec{a}_d$. For example, in two-dimensions, a
+displacement by $\vec{a}_1$ is the key `(1,0)`. A displacement by
+$2\vec{a}_1 + \vec{a}_2$ is the key `(2,1)`. Generally, the displacements are
 `(n,m,p)` where `n`, `m`, and `p` have to be integers.
 
-The value of each key is a matrix of hopping amplitudes from the orbitals 
-in the reference unit cell to the unit cells defined by the displacement key. 
-Hopping between orbitals within a unit cell is encoded as a matrix and indexed 
+The value of each key is a matrix of hopping amplitudes from the orbitals
+in the reference unit cell to the unit cells defined by the displacement key.
+Hopping between orbitals within a unit cell is encoded as a matrix and indexed
 with the key `(0,...,0_d)`.
 
 Here is an example of how this structure looks like in code
 
 ```python
 # Number of sites and orbitals (and maybe spin) in each unit cell
 n_orb = ...
@@ -188,108 +188,108 @@
     (0,...,1_d) : n_orb by n_orb ndarray,
     ...
     (-1,...,0_d) : n_orb by n_orb ndarray
     ...
 }
 ```
 
-Next construct the tight-binding model as 
+Next construct the tight-binding model as
 
 ```
 from triqs.lattice.tight_binding import TBLattice
 tbl = TBLattice(units=units, hoppings=hoppings, orbital_positions=orbital_positions)
 ```
 
 :::{note}
-If `h0_k` has some block structure you want to encode, the above process 
-can be done for each block (by definition of being a block matrix structure 
-there cannot be coupling between orbitals of different blocks). 
-Each `TBLattice` instance must use the same `units` and $k$-space 
+If `h0_k` has some block structure you want to encode, the above process
+can be done for each block (by definition of being a block matrix structure
+there cannot be coupling between orbitals of different blocks).
+Each `TBLattice` instance must use the same `units` and $k$-space
 meshgrid `mk`.
 :::
 
-The last and important part is to Fourier transform the tight-binding model 
+The last and important part is to Fourier transform the tight-binding model
 onto the $k$-space meshgrid `mk` and have it indexed as `k, orb_i, orb_j` for
 the {{RISB}} `Solver` class. This is very easily done as
 
 ```python
 h0_k = dict()
 
 # For each block (a string bl_name) in h0_k
 h0_k[bl_name] = tbl.fourier(mk).data
 ```
 
 :::{warning}
-I have only used this class on hypercubic lattices. It may work poorly for 
-something like kagome, or if the unit cell is very complicated. If this is not 
+I have only used this class on hypercubic lattices. It may work poorly for
+something like kagome, or if the unit cell is very complicated. If this is not
 an issue then let me know and I will remove this warning.
 :::
 
 ### Using [TBmodels](https://github.com/Z2PackDev/TBmodels)
 
 Work in progress.
 
 ## Constructing `h0_loc` as a matrix
 
 :::{seealso}
 [Using projectors](projectors.md).
 :::
 
-If you want to get $\hat{H}_i^{\mathrm{loc}}$ for each correlated 
-space $\mathcal{C}_i$ calculated from `h0_k` then there are some helper 
+If you want to get $\hat{H}_i^{\mathrm{loc}}$ for each correlated
+space $\mathcal{C}_i$ calculated from `h0_k` then there are some helper
 functions.
 
 If there are no projectors and the correlated space is the entire unit cell
 
 ```python
 from risb.helpers import get_h0_loc_matrix
 
 h0_loc_matrix = dict()
 for bl in h0_k.keys():
     h0_loc_matrix[bl] = get_h0_loc_matrix(h0_k[bl])
 ```
 
-If there are multiple correlated spaces, indexed as `i` 
+If there are multiple correlated spaces, indexed as `i`
 
 ```python
 # Total number of clusters on the lattice
 n_clusters = ...
 
 # A list of gf_struct objects in each correlated space
 gf_struct = ...
 
-# A list of mappings of the block structure from each correlated 
+# A list of mappings of the block structure from each correlated
 # subspace to the larger space of h0_k
 gf_struct_mapping = ...
 
 # A list of projectors into each correlated subspace
-projectors = 
+projectors =
 
 h0_loc_matrix = [dict() for i in range(n_clusters)]
 for i in range(n_clusters):
     for bl, bl_size in gf_struct:
         bl_full = gf_struct_mapping[bl]
         h0_loc_matrix[i][bl] = get_h0_loc_matrix(h0_k[bl_full], projectors[i][bl] )
 ```
 
 ### As a {{TRIQS}} operator
 
-If you have a block matrix representation of a single-particle operator and 
-you want it as a {{TRIQS}} operator 
+If you have a block matrix representation of a single-particle operator and
+you want it as a {{TRIQS}} operator
 
 ```python
 from risb.helpers_triqs get_C_Op
 
 # The block matrix
 A = ...
 
 # A gf_struct object of the structure of the space
 gf_struct = ...
 
-# A list/vector of operators 
+# A list/vector of operators
 C_Op = get_C_Op(gf_struct, dagger=False)
 C_dag_Op = get_C_Op(gf_struct, dagger=True)
 
 Op = dict()
 for bl, bl_size in gf_struct:
     Op[bl] = C_dag_Op[bl] @ A[bl] @ C_Op[bl]
 ```
@@ -304,25 +304,25 @@
 
 ## Constructing `h0_kin_k`
 
 :::{seealso}
 [Using projectors](projectors.md).
 :::
 
-If you want only the kinetic terms in `h0_k` with all of the local terms 
-`h0_loc` from $\hat{H}_i^{\mathrm{loc}}$ removed then you can use 
+If you want only the kinetic terms in `h0_k` with all of the local terms
+`h0_loc` from $\hat{H}_i^{\mathrm{loc}}$ removed then you can use
 
 ```python
 from risb.helpers import get_h0_kin_k
 
 # A list of gf_struct objects in each correlated space
 gf_struct = ...
 
-# A list of mappings of the block structure from each correlated 
+# A list of mappings of the block structure from each correlated
 # subspace to the larger space of h0_k
 gf_struct_mapping = ...
 
 # A list of projectors into each correlated subspace
-projectors = 
+projectors =
 
 h0_kin_k = get_h0_kin_k(h0_k, projectors, gf_struct_mapping)
-```
+```
```

### Comparing `risb-0.1.0/docs/tutorials/hubbard.md` & `risb-0.1.1/docs/tutorials/hubbard.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 # Brinkman-Rice metal-insulator transition
 
-In this tutorial you will use `LatticeSolver` and `EmbeddingAtomDiag` to solve 
-the half-filled Hubbard model. This is one of the simplest strongly correlated 
-electron models, yet in general does not have an exact solution. Using this 
-model, you will learn about the Brinkman-Rice [^Brinkman1970] description of 
-a Mott insulator, the quintessential strongly correlated phase of matter. 
-At the end of this tutorial you will have an idea of some of the kinds 
+In this tutorial you will use `LatticeSolver` and `EmbeddingAtomDiag` to solve
+the half-filled Hubbard model. This is one of the simplest strongly correlated
+electron models, yet in general does not have an exact solution. Using this
+model, you will learn about the Brinkman-Rice [^Brinkman1970] description of
+a Mott insulator, the quintessential strongly correlated phase of matter.
+At the end of this tutorial you will have an idea of some of the kinds
 ground states {{RISB}} can capture, and importantly some of its limitations.
 
 :::{seealso}
-[Using `LatticeSolver`](../how-to/lattice_solver.md) for more details on the 
+[Using `LatticeSolver`](../how-to/lattice_solver.md) for more details on the
 {{RISB}} solver class.
 :::
 
 :::{tip}
-In examples/hubbard.py we provide an example if you are stuck. But you will 
+In examples/hubbard.py we provide an example if you are stuck. But you will
 learn a lot more if you try to write everything yourself.
 :::
 
 ## The model
 
 The Hubbard model is given by
 
 $$
-\hat{H} = t \sum_{ij\sigma}  
+\hat{H} = t \sum_{ij\sigma}
 \hat{c}^{\dagger}_{i\sigma} \hat{c}^{}_{j\sigma}
 + U \sum_i \hat{n}^{}_{i\uparrow} \hat{n}^{}_{i\downarrow},
 $$
 
-where $t$ is the hopping amplitude between sites, 
-$\hat{c}^{(\dagger)}_{i\sigma}$ is a (creation) annihilation 
-operator on site $i$ with spin $\sigma \in \{\uparrow, \downarrow\}$, and 
-$\hat{n}_{i\sigma} \equiv \hat{c}^{\dagger}_{i\sigma} \hat{c}^{}_{j\sigma}$ 
+where $t$ is the hopping amplitude between sites,
+$\hat{c}^{(\dagger)}_{i\sigma}$ is a (creation) annihilation
+operator on site $i$ with spin $\sigma \in \{\uparrow, \downarrow\}$, and
+$\hat{n}_{i\sigma} \equiv \hat{c}^{\dagger}_{i\sigma} \hat{c}^{}_{j\sigma}$
 is the number operator.
 
 The non-interacting part is given by the first term
 
 $$
-\hat{H}^0 = t \sum_{ij\sigma}  
-\hat{c}^{\dagger}_{i\sigma} \hat{c}^{}_{j\sigma}, 
+\hat{H}^0 = t \sum_{ij\sigma}
+\hat{c}^{\dagger}_{i\sigma} \hat{c}^{}_{j\sigma},
 $$
 
-which wants to move electrons around and create plane waves on the lattice. 
-The interacting part on every site is the summand in the second term 
+which wants to move electrons around and create plane waves on the lattice.
+The interacting part on every site is the summand in the second term
 
 $$
-\hat{H}_i^{\mathrm{int}} = 
+\hat{H}_i^{\mathrm{int}} =
 U \hat{n}^{}_{i\uparrow} \hat{n}^{}_{i\downarrow},
 $$
 
-which wants to keep electrons at arms length (apart). By themselves, each term 
-can be solved analytically. The headache (and all of the interesting resulting 
+which wants to keep electrons at arms length (apart). By themselves, each term
+can be solved analytically. The headache (and all of the interesting resulting
 physics) happens when the two terms compete.
 
-In the paramagnetic state (where spin rotational symmetry does not break) all 
-single-site {{RISB}} calculations will qualitatively give the same solutions. 
-The differences will occur in larger {{RISB}} clusters, where more spatial 
-correlations are captured, and in magnetic states captured at the single-site 
+In the paramagnetic state (where spin rotational symmetry does not break) all
+single-site {{RISB}} calculations will qualitatively give the same solutions.
+The differences will occur in larger {{RISB}} clusters, where more spatial
+correlations are captured, and in magnetic states captured at the single-site
 level (similar to how magnetic states are captured in Hartree-Fock).
 
 ## Construct the non-interacting terms $\hat{H}^{0}$
 
 :::{seealso}
-[Constructing tight-binding models](../how-to/quadratic_terms.md) for some 
+[Constructing tight-binding models](../how-to/quadratic_terms.md) for some
 other ways to construct $\hat{H}^{0}$.
 :::
 
-In this tutorial, you can pick any single-atom unit cell. But, for simplicity, 
-lets consider the cubic lattice. 
-    
-First create a cubic $k$-space mesh in crystal coordinates with lattice 
+In this tutorial, you can pick any single-atom unit cell. But, for simplicity,
+lets consider the cubic lattice.
+
+First create a cubic $k$-space mesh in crystal coordinates with lattice
 spacing $a = 1$
 
 ```python
 import numpy as np
 
 # Spatial dimensions
 d = 3
@@ -92,19 +92,19 @@
 # Can you figure out the outcome of the pythonic syntax for the first param?
 k_mesh = np.meshgrid(*[k_linear]*3, indexing='ij')
 
 # Reshape to list
 k_mesh = np.reshape(k_mesh, (n_k, d))
 ```
 
-Next create the hopping marix for each spin $\sigma$ in the structure that 
-`LatticeSolver` expects. In general, this is a [numpy.ndarray](numpy.ndarray) 
-indexed as $(k, \mathrm{orb}_i, \mathrm{orb}_j)$, where $k$ is a point on the 
-grid, and $\mathrm{orb}_i$ is an atom, orbital, and/or spin in the unit cell. 
-In this case there is only a single atom, and the two spin orbitals can be 
+Next create the hopping marix for each spin $\sigma$ in the structure that
+`LatticeSolver` expects. In general, this is a [numpy.ndarray](numpy.ndarray)
+indexed as $(k, \mathrm{orb}_i, \mathrm{orb}_j)$, where $k$ is a point on the
+grid, and $\mathrm{orb}_i$ is an atom, orbital, and/or spin in the unit cell.
+In this case there is only a single atom, and the two spin orbitals can be
 treated separately because there is no spin-orbit coupling.
 
 ```python
 # Hopping amplitude
 t = 1
 
 # Number of orbitals on a site
@@ -118,80 +118,80 @@
         h0_k[bl][:, orb, orb] = -2.0 * t * ( np.cos(k_mesh[:,0]) \
                                            + np.cos(k_mesh[:,1]) \
                                            + np.cos(k_mesh[:,2]) )
 ```
 
 ## Local structure on a site
 
-Now set up how the local structure looks like. This follows the same 
+Now set up how the local structure looks like. This follows the same
 conventions as Green's functions in {{TRIQS}}
 
 ```python
 gf_struct = [('up', n_orb), ('dn', n_orb)]
 ```
 
-All single-particle matrices defined on a cluster (a site) will follow this 
-block structure. It basically says that the `'up'` and '`dn'` spins do not 
-have off-diagonal elements between them, and each matrix in each block is a 
+All single-particle matrices defined on a cluster (a site) will follow this
+block structure. It basically says that the `'up'` and '`dn'` spins do not
+have off-diagonal elements between them, and each matrix in each block is a
 $n_{orb} \times n_{orb}$ matrix.
 
-The structure of `gf_structure` also determines what local operators are 
+The structure of `gf_structure` also determines what local operators are
 on a cluster (a site) that you will use in the next section.
 
 ## Construct the interactions $\hat{H}_i^{\mathrm{int}}$
 
-Since you are using `EmbeddingAtomDiag`, you might as well use all of the great 
+Since you are using `EmbeddingAtomDiag`, you might as well use all of the great
 second-quantized operator tools provided by {{TRIQS}}.
 
-Because {{RISB}} will make all equivalent clusters homogenous, you only need to 
-construct the interactions for a single site. 
+Because {{RISB}} will make all equivalent clusters homogenous, you only need to
+construct the interactions for a single site.
 
-Now construct the interaction terms. The Hubbard interaction is simply given 
+Now construct the interaction terms. The Hubbard interaction is simply given
 as
 
 ```python
 from triqs.operators import n
 
 # Hubbard U
 U = 5
 
 h_int = U * n('up', 0) * n('dn', 0)
 ```
 
-There are also some great helper tools for constructing interactions 
-in the `triqs.operators.util.hamiltonians` module provided by {{TRIQS}}. It 
+There are also some great helper tools for constructing interactions
+in the `triqs.operators.util.hamiltonians` module provided by {{TRIQS}}. It
 is completely overkill for this interaction, but let's do it anyway.
 
 ```python
 from triqs.operators.util.hamiltonians import h_int_density
 
 # 2D matrix of U_ij^{sigma sigma} (same spins)
 U = np.zeros(shape = [n_orb, n_orb])
 
 # 2D matrix of U_ij^{sigma nu} (different spins)
 Uprime = np.full(shape = [n_orb, n_orb], fill_value = 5)
 
-h_int = h_int_density(spin_names = ['up', 'dn'], 
-                      n_orb = n_orb, 
-                      U = U, 
-                      Uprime = Uprime, 
+h_int = h_int_density(spin_names = ['up', 'dn'],
+                      n_orb = n_orb,
+                      U = U,
+                      Uprime = Uprime,
                       off_diag=True
 )
 ```
 
 ## Enforce paramagnetism
 
-There will be some numerical noise in the solutions that can make 
-the `'up'` and `'dn'` spin parts of the solution slightly different. It helps 
-the self-consistent process to ensure that this symmetry is strictly enforced. 
+There will be some numerical noise in the solutions that can make
+the `'up'` and `'dn'` spin parts of the solution slightly different. It helps
+the self-consistent process to ensure that this symmetry is strictly enforced.
 You can do this by passing a symmetrization function to the solver
 
 ```python
-# The object LatticeSolver expects is list[dict[ndarray]], where each 
-# item in the list is a cluster. In this case there is only one 
+# The object LatticeSolver expects is list[dict[ndarray]], where each
+# item in the list is a cluster. In this case there is only one
 # cluster.
 def force_paramagnetic(A):
     A[0]['up'] = 0.5 * (A[0]['up'] + A[0]['dn'])
     A[0]['dn'] = A[0]['up']
     return A
 ```
 
@@ -199,52 +199,53 @@
 
 :::{seealso}
 [About k-integration](../explanations/kweight.md).
 
 [Using `SmearKWeight`](../how-to/kweight.md).
 :::
 
-You need to specify a function to `LatticeSolver` that gives the integration 
-weights at each $k$-point on the lattice. The easiest thing to do is to use 
-the `SmearKWeight` class that assumes the weights are given by 
+You need to specify a function to `LatticeSolver` that gives the integration
+weights at each $k$-point on the lattice. The easiest thing to do is to use
+the `SmearKWeight` class that assumes the weights are given by
 Fermi-Dirac functions
 
 ```python
-# The smearing, in units of inverse temperature. It is an approximation 
+# The smearing, in units of inverse temperature. It is an approximation
 # because RISB is at zero temperature
 beta = 40
 
 # 1 electron on average per unit cell, half-filling
 n_target = 1 # half-filling
 
 kweight = SmearingKWeight(beta=beta, n_target=n_target)
 ```
+
 ## Setup the solvers and find a self-consistent solution
 
 :::{seealso}
 [Using embedding classes](../how-to/embedding.md).
 
 [Using `LatticeSolver`](../how-to/lattice_solver.md).
 
 [Constructing the {{RISB}} self-consistent loop](../tutorials/self-consistent.md).
 :::
 
-You need a class that solves the 
-[embedding Hamiltonian](../explanations/embedding.md). A simple one is 
-:py:class:`risb.embedding.EmbeddingAtomDiag` 
+You need a class that solves the
+[embedding Hamiltonian](../explanations/embedding.md). A simple one is
+:py:class:`risb.embedding.EmbeddingAtomDiag`
 
 ```python
 embedding = EmbeddingClass(h_int, gf_struct)
 ```
 
-Next setup the {{RISB}} solver for the self-consistent loop. This will make a 
-guess for some parameters (renormalization matrix $\mathcal{R}$ and 
-correlation potential matrixx $\lambda$) and go through a self-consistent 
-loop until $\mathcal{R}$ and $\lambda$ reach a fixed point. On a lattice 
-the solver is setup as 
+Next setup the {{RISB}} solver for the self-consistent loop. This will make a
+guess for some parameters (renormalization matrix $\mathcal{R}$ and
+correlation potential matrixx $\lambda$) and go through a self-consistent
+loop until $\mathcal{R}$ and $\lambda$ reach a fixed point. On a lattice
+the solver is setup as
 
 ```python
 S = LatticeSolver(h0_k = h0_k,
                   gf_struct = gf_struct,
                   embedding = embedding,
                   update_weights = kweight.update_weights,
                   symmetries = [force_paramagnetic]
@@ -259,137 +260,139 @@
 
 S.solve(tol = tol)
 ```
 
 ## Observables on a site
 
 In {{RISB}} it is very simple to calculate local quantities on a cluster
-(a site). Using {{TRIQS}} there are some simple helper functions to construct 
-some common observables. The main one we are interested in is the total spin 
+(a site). Using {{TRIQS}} there are some simple helper functions to construct
+some common observables. The main one we are interested in is the total spin
 on a site.
 
-The average total spin per cluster $S$ is 
+The average total spin per cluster $S$ is
 the solution to
 
 $$
 S(S+1) = \frac{1}{\mathcal{N}} \sum_i \langle \hat{S}_i^2 \rangle
 $$
 
-where $\hat{S}_i$ is the total spin operator on a cluster (a site). Because 
-the homogenous assumption is used in {{RISB}}, the spin per site is the same 
+where $\hat{S}_i$ is the total spin operator on a cluster (a site). Because
+the homogenous assumption is used in {{RISB}}, the spin per site is the same
 on every site, so you only have to (and only can) calculate it on one site.
 
 In {{TRIQS}} the total spin $\hat{S}^2$ is given by
 
 ```python
 from triqs.operators.util.observables import S2_op
 
 total_spin_Op = S2_op(spin_names, n_orb, off_diag=True)
 ```
 
-To calculate the overlap with the solution {{RISB}} finds 
+To calculate the overlap with the solution {{RISB}} finds
 
 ```python
 total_spin = embedding.overlap(total_spin_Op)
 ```
 
 ## Exercises
 
-1. Solve for a range of $U$ values from $U = 0$ to $U = 12$. You may find 
-`embedding.set_h_int()` useful.
+1.  Solve for a range of $U$ values from $U = 0$ to $U = 12$. You may find
+    `embedding.set_h_int()` useful.
 
-1. Plot the average spin $S$ on a site versus $U$. Plot the quasiparticle 
-weight $Z$ (accessed by `S.Z`) versus $U$. What happens to $S$ and 
-$Z$ for large $U$? 
-
-1. Plot the hybridization coupling $D$ (accessed by `embedding.D`) of the 
-[embedding Hamiltonian](../explanations/embedding.md). What happens to $D$ 
-for large $U$? What does this imply about the impurity and the bath coupling 
-in the embedding Hamiltonian $\hat{H}^{\mathrm{emb}}$?
-
-1. You will notice that $Z$, $S$, and $D$ both have an abrupt change, and then 
-plateau, at some critical interaction strength $U_c$. What is the phase of 
-matter to the left of $U_c$? What is the phase of matter to the right of 
-$U_c$? What type of phase transition occurs at $U_c$?
+1.  Plot the average spin $S$ on a site versus $U$. Plot the quasiparticle
+    weight $Z$ (accessed by `S.Z`) versus $U$. What happens to $S$ and
+    $Z$ for large $U$?
+
+1.  Plot the hybridization coupling $D$ (accessed by `embedding.D`) of the
+    [embedding Hamiltonian](../explanations/embedding.md). What happens to $D$
+    for large $U$? What does this imply about the impurity and the bath coupling
+    in the embedding Hamiltonian $\hat{H}^{\mathrm{emb}}$?
+
+1.  You will notice that $Z$, $S$, and $D$ both have an abrupt change, and then
+    plateau, at some critical interaction strength $U_c$. What is the phase of
+    matter to the left of $U_c$? What is the phase of matter to the right of
+    $U_c$? What type of phase transition occurs at $U_c$?
 
-1. Construct an operator that calculates the number variance
+1.  Construct an operator that calculates the number variance
 
     $$
     \mathrm{Var}(N) = \langle (\hat{N} - \langle N \rangle)^2 \rangle,
     $$
 
-    and total spin variance 
+    and total spin variance
 
     $$
     \mathrm{Var}(N) = \langle (\hat{N} - \langle N \rangle)^2 \rangle,
     $$
 
-    and plot these as a function of $U$. How do they look like to the left 
+    and plot these as a function of $U$. How do they look like to the left
     and right of the critical interaction $\hat{U}_c$?
 
-1. If you know anything about the Mott metal-insulator phase transition, 
-you might find the phase of matter to the right of $U_c$ a bit strange. In the 
-limit $t/U$ is small, a perturbative expansion gives the low-energy effective 
-theory of the half-filled Hubbard model as the Heisenberg model, given by
-
-    $$
-    \hat{H} = J \sum_{i \neq j} \vec{S}_i \cdot \vec{S}_j,
-    $$
-
-    where $\vec{S}_i = (\hat{S}_i^x, \hat{S}_i^y, \hat{S}_i^z)$, and 
-    $J = 4 t^2 / U$. 
-    
-    The above implies that the localized spin-$1/2$s on each site 
-    have a spin-spin exchange interaction between them arising from charge 
-    fluctuations (high-energy virtual processes). In the atomic limit 
-    $t / U \rightarrow 0$ the spin exchange $J \rightarrow 0$, with an 
-    isolated spin-$1/2$ on each site because there is no coupling between 
-    them. 
-    
-    Recalling the observables you calculated to the right of the critical 
-    interaction $U_c$ (which happened at a finite $U$) what does this imply 
-    about the ground state that {{RISB}} predicts in the Mott phase? 
-    
-    What physics is {{RISB}} not capturing that, e.g., {{DMFT}} captures, 
-    and why?
-
-    :::{hint}
-    In {{RISB}} the frequency dependence of the self-energy is linear and 
-    goes like $\Sigma(\omega) \sim (I - Z^{-1}) \omega$, where $I$ is the 
-    identity.
-    :::
+1.  If you know anything about the Mott metal-insulator phase transition,
+    you might find the phase of matter to the right of $U_c$ a bit strange. In the
+    limit $t/U$ is small, a perturbative expansion gives the low-energy effective
+    theory of the half-filled Hubbard model as the Heisenberg model, given by
+
+        $$
+        \hat{H} = J \sum_{i \neq j} \vec{S}_i \cdot \vec{S}_j,
+        $$
+
+        where $\vec{S}_i = (\hat{S}_i^x, \hat{S}_i^y, \hat{S}_i^z)$, and
+        $J = 4 t^2 / U$.
+
+        The above implies that the localized spin-$1/2$s on each site
+        have a spin-spin exchange interaction between them arising from charge
+        fluctuations (high-energy virtual processes). In the atomic limit
+        $t / U \rightarrow 0$ the spin exchange $J \rightarrow 0$, with an
+        isolated spin-$1/2$ on each site because there is no coupling between
+        them.
+
+        Recalling the observables you calculated to the right of the critical
+        interaction $U_c$ (which happened at a finite $U$) what does this imply
+        about the ground state that {{RISB}} predicts in the Mott phase?
+
+        What physics is {{RISB}} not capturing that, e.g., {{DMFT}} captures,
+        and why?
+
+        :::{hint}
+        In {{RISB}} the frequency dependence of the self-energy is linear and
+        goes like $\Sigma(\omega) \sim (I - Z^{-1}) \omega$, where $I$ is the
+        identity.
+        :::
 
 ## Conclusion
 
-You have solved the Hubbard model using the {{RISB}} approximation and found 
-a Brinkman-Rice metal-insulator transition to the Mott insulating phase. 
-In cluster extensions to {{RISB}} this type of transition can also occur. You 
-should now know one of the ways that {{RISB}} captures insulators, and 
-understand the limitations [^GHOST] for the kinds of ground states that {{RISB}} 
+You have solved the Hubbard model using the {{RISB}} approximation and found
+a Brinkman-Rice metal-insulator transition to the Mott insulating phase.
+In cluster extensions to {{RISB}} this type of transition can also occur. You
+should now know one of the ways that {{RISB}} captures insulators, and
+understand the limitations [^GHOST] for the kinds of ground states that {{RISB}}
 can describe.
 
 ## Bonus
 
-In this tutorial you only considered solutions where every site was the same. 
-Construct a two-site super cell of the cubic lattice, and treat the 
-two sites as separate embedding spaces $\mathcal{C}_i$ (see 
-[Using projectors](../how-to/projectors.md)). You will also find a 
-metal-insulator transition (of the Slater type). 
-
-1. How does this differ to the Brinkman-Rice metal-insulator transition? 
-
-1. How does this differ to the mean-field solution (Hartree-Fock) to the 
-Hubbard model on the cubic lattice?
-
-1. Knowing that the Mott insulating state that {{RISB}} captures in the 
-Brinkman-Rice transition should have spin-spin exchange, what is the expected 
-ground state of the Hubbard model on the cubic lattice at half-filling?
-
-[^Brinkman1970]: [W. F. Brinkman and T. M. Rice, 
-*Application of Gutzwiller's Variational Method to the Metal-Insulator Transition*,
-Phys. Rev. B **2**, 4302 (1970)](https://doi.org/10.1103/PhysRevB.2.4302).
-
-[^GHOST]: [N. Lanatà, T.-H. Lee, Y.-X. Yao, and V. Dobrosavljević, 
-*Emergent Bloch excitations in Mott matter*, 
-Phys. Rev. B **96**, 195126 (2017)](https://doi.org/10.1103/PhysRevB.96.195126), 
-and the papers that cite this paper for extensions that improve upon 
-normal {{RISB}}.
+In this tutorial you only considered solutions where every site was the same.
+Construct a two-site super cell of the cubic lattice, and treat the
+two sites as separate embedding spaces $\mathcal{C}_i$ (see
+[Using projectors](../how-to/projectors.md)). You will also find a
+metal-insulator transition (of the Slater type).
+
+1. How does this differ to the Brinkman-Rice metal-insulator transition?
+
+1. How does this differ to the mean-field solution (Hartree-Fock) to the
+   Hubbard model on the cubic lattice?
+
+1. Knowing that the Mott insulating state that {{RISB}} captures in the
+   Brinkman-Rice transition should have spin-spin exchange, what is the expected
+   ground state of the Hubbard model on the cubic lattice at half-filling?
+
+[^Brinkman1970]:
+    [W. F. Brinkman and T. M. Rice,
+    _Application of Gutzwiller's Variational Method to the Metal-Insulator Transition_,
+    Phys. Rev. B **2**, 4302 (1970)](https://doi.org/10.1103/PhysRevB.2.4302).
+
+[^GHOST]:
+    [N. Lanatà, T.-H. Lee, Y.-X. Yao, and V. Dobrosavljević,
+    _Emergent Bloch excitations in Mott matter_,
+    Phys. Rev. B **96**, 195126 (2017)](https://doi.org/10.1103/PhysRevB.96.195126),
+    and the papers that cite this paper for extensions that improve upon
+    normal {{RISB}}.
```

### Comparing `risb-0.1.0/docs/tutorials/kagome.md` & `risb-0.1.1/docs/tutorials/kagome.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 # Multiple clusters on the kagome lattice
 
 :::{admonition} TODO
 Single-site case. Three-site cluster case.
 :::
 
-In this tutorial you will use :py:class:`LatticeSolver` to solve the 
-single-orbital Hubbard model on the kagome lattice. We will do this in two 
-ways. 
-
-First, as three inequivalent correlated subspaces $\mathcal{C}$ for 
-$i \in \{A, B, C\}$. This will ignore spatial correlations within a triangle 
-in a unit cell. Doing it this way requires constructing projectors onto 
+In this tutorial you will use :py:class:`LatticeSolver` to solve the
+single-orbital Hubbard model on the kagome lattice. We will do this in two
+ways.
+
+First, as three inequivalent correlated subspaces $\mathcal{C}$ for
+$i \in \{A, B, C\}$. This will ignore spatial correlations within a triangle
+in a unit cell. Doing it this way requires constructing projectors onto
 the different correlated subspaces.
 
-The second way is take a single three-site cluster and 
-have one correlated subspace $\mathcal{C}$. This will include spatial 
+The second way is take a single three-site cluster and
+have one correlated subspace $\mathcal{C}$. This will include spatial
 correlations within a triangle in a unit cell.
 
 :::{tip}
-In `examples/kagome_hubbard.py` we provide an example if you are stuck. But 
+In `examples/kagome_hubbard.py` we provide an example if you are stuck. But
 you will learn a lot more if you write it yourself.
 :::
 
 ## The model
 
-The tight-binding model on the kagome lattice can be written as 
+The tight-binding model on the kagome lattice can be written as
 
 $$
-\hat{H}^0 = \sum_{k\sigma} 
+\hat{H}^0 = \sum_{k\sigma}
 \vec{c}_{k\sigma}^{\dagger}
-\mathbf{H}_{\sigma}(k) 
+\mathbf{H}_{\sigma}(k)
 \vec{c}_{k\sigma},
 $$
 
 where the second-quantized operators are written as vectors as
 
 $$
-\vec{c}^{\dagger}_{k\sigma} = 
-\left( \hat{c}^{\dagger}_{kA\sigma}, 
-\hat{c}^{\dagger}_{kB\sigma}, 
+\vec{c}^{\dagger}_{k\sigma} =
+\left( \hat{c}^{\dagger}_{kA\sigma},
+\hat{c}^{\dagger}_{kB\sigma},
 \hat{c}^{\dagger}_{kC\sigma} \right),
 $$
 
-where $\hat{c}^{\dagger}_{k\alpha\sigma}$ creates an electron on site 
-$\alpha \in \{A,B,C\}$ with spin $\sigma$ within a unit cell, and the dispersion 
-matrix is given by 
+where $\hat{c}^{\dagger}_{k\alpha\sigma}$ creates an electron on site
+$\alpha \in \{A,B,C\}$ with spin $\sigma$ within a unit cell, and the dispersion
+matrix is given by
 
 $$
 \mathbf{H}_{\sigma}(k) = \begin{pmatrix}
 0                & - 2 t \cos(k_1/2)  & -2 t \cos(k_2/2) \\
 -2 t \cos(k_1/2) & 0                & -2 t \cos(k_3/2) \\
 -2 t \cos(k_2/2) & -2 t \cos(k_3/2) & 0,
-\end{pmatrix} 
+\end{pmatrix}
 $$
 
-where $t$ is the hopping amplitude. For lattice vectors in Cartesian 
+where $t$ is the hopping amplitude. For lattice vectors in Cartesian
 coordinates given by $\vec{a}_1 = (1, 0)$ and $\vec{a}_2 = (1/2, \sqrt{3}/2)$,
-the variables within the cosine functions are given by 
-$k_1 = k_x$, 
-$k_2 = k_x/2 + \sqrt{3} k_y / 2$ and 
+the variables within the cosine functions are given by
+$k_1 = k_x$,
+$k_2 = k_x/2 + \sqrt{3} k_y / 2$ and
 $k_3 = - k_x / 2 + \sqrt{3} k_y / 2$.
 
-## Construct a matrix of the dispersion relations
+## Construct a matrix of the dispersion relations
```

### Comparing `risb-0.1.0/docs/tutorials/self-consistent.md` & `risb-0.1.1/docs/tutorials/self-consistent.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,153 +1,153 @@
 # Constructing the {{RISB}} self-consistent loop
 
-In this tutorial, you will construct the self-consistent loop in rotationally 
-invariant slave-bosons, and use it to solve the bilayer Hubbard model. This 
-will allow you to easily expand upon the algorithms that we provide so that 
+In this tutorial, you will construct the self-consistent loop in rotationally
+invariant slave-bosons, and use it to solve the bilayer Hubbard model. This
+will allow you to easily expand upon the algorithms that we provide so that
 you can tailor-make {{RISB}} for your own research problems.
 
 We will try to reproduce the results of Sec. IIIB of Ref. [^Lechermann2007].
 
 ## Example model: bilayer Hubbard
 
 :::{tip}
-In `examples/bilayer_hubbard.py` we provide an example using the 
+In `examples/bilayer_hubbard.py` we provide an example using the
 `LatticeSolver` class that you can compare your answers to.
 :::
 
 The bilayer Hubbard model on the hypercubic lattice is given by
 
 $$
 \hat{H} = \hat{H}_0^{\mathrm{kin}} + \sum_i \hat{H}_i^{\mathrm{loc}},
 $$
 
 where $i$ indexes a site.
 
-The non-interacting kinetic part of the Hamiltonian that describes hopping 
+The non-interacting kinetic part of the Hamiltonian that describes hopping
 between clusters (sites) on the lattice is given by
 
 $$
-\hat{H}_0^{\mathrm{kin}} = - \frac{1}{d} 
-\sum_{\langle i j \rangle} \sum_{\sigma} \sum_{\alpha=1,2} 
+\hat{H}_0^{\mathrm{kin}} = - \frac{1}{d}
+\sum_{\langle i j \rangle} \sum_{\sigma} \sum_{\alpha=1,2}
 ( t_{\alpha} \hat{c}_{i \alpha \sigma}^{\dagger} \hat{c}_{j \alpha \sigma}
 + \mathrm{H.c.} ),
 $$
 
-where $d$ is the number of spatial dimensions ($d=3$ on the cubic 
-lattice), $\sigma$ is a spin label, $\alpha$ is an orbital label, 
-$\langle i j \rangle$ indicates nearest-neighbor bonds, 
-${\mathrm{H.c.}}$ is Hermitian conjugate, $t_{\alpha}$ is the 
-probability amplitude to move an electron between nearest neighbor sites, and 
+where $d$ is the number of spatial dimensions ($d=3$ on the cubic
+lattice), $\sigma$ is a spin label, $\alpha$ is an orbital label,
+$\langle i j \rangle$ indicates nearest-neighbor bonds,
+${\mathrm{H.c.}}$ is Hermitian conjugate, $t_{\alpha}$ is the
+probability amplitude to move an electron between nearest neighbor sites, and
 $\hat{c}^{(\dagger)}_{i\alpha\sigma}$ is an annihilation (creation) operator.
 
-For degenerate orbitals on the cubic lattice, the dispersion for each 
+For degenerate orbitals on the cubic lattice, the dispersion for each
 orbital is given by
 
 $$
 \varepsilon^{\mathrm{kin}}_{k\alpha} = -\frac{2}{d} t_{\alpha} \sum_{\mu}^d \cos(k_\mu a),
 $$
 
-where $k$ labels a reciprocal lattice vector. Hence, 
-$\hat{H}_{0, k \alpha \beta}^{\mathrm{kin}} = \varepsilon^{\mathrm{kin}}_{k\alpha}$ 
+where $k$ labels a reciprocal lattice vector. Hence,
+$\hat{H}_{0, k \alpha \beta}^{\mathrm{kin}} = \varepsilon^{\mathrm{kin}}_{k\alpha}$
 for $\alpha = \beta$ and zero otherwise.
 
 The local part of the Hamiltonian is given by
 
 $$
-\hat{H}_i^{\mathrm{loc}} = 
-V \sum_{\sigma} (\hat{c}_{i 1 \sigma}^{\dagger} \hat{c}_{i 2 \sigma} 
+\hat{H}_i^{\mathrm{loc}} =
+V \sum_{\sigma} (\hat{c}_{i 1 \sigma}^{\dagger} \hat{c}_{i 2 \sigma}
 + \mathrm{H.c.})
 + U \sum_{\alpha} \hat{n}_{i \alpha \uparrow} \hat{n}_{i \alpha \downarrow},
 $$
 
-where $V$ is the interlayer hopping between the orbitals, $U$ is 
-the local Coulomb repulsion, and 
+where $V$ is the interlayer hopping between the orbitals, $U$ is
+the local Coulomb repulsion, and
 $\hat{n}_{i\alpha\sigma} \equiv \hat{c}^{\dagger}_{i\alpha\sigma} \hat{c}_{i\alpha\sigma}$.
 
 :::{important}
-In {{RISB}} the non-interacting quadratic terms within a cluster $i$ have 
-to be separated from the non-interacting quadratic terms coupling between 
-clusters. That is why the above is split into $\hat{H}^{\mathrm{kin}}_0$ 
+In {{RISB}} the non-interacting quadratic terms within a cluster $i$ have
+to be separated from the non-interacting quadratic terms coupling between
+clusters. That is why the above is split into $\hat{H}^{\mathrm{kin}}_0$
 and $\hat{H}^{\mathrm{loc}}_i$. Note that this is done automatically when
 using `LatticeSolver`.
 :::
 
 ## A: Construct $\hat{H}_0^{\mathrm{kin}}$
 
 :::{seealso}
-[Constructing tight-binding models](../how-to/quadratic_terms.md) for 
+[Constructing tight-binding models](../how-to/quadratic_terms.md) for
 some methods.
 :::
 
-First, construct the dispersion between clusters on the lattice. It should 
-not include the non-interacting quadratic terms within a cluster. 
+First, construct the dispersion between clusters on the lattice. It should
+not include the non-interacting quadratic terms within a cluster.
 
-Notice that the Hamiltonian is block diagonal in spin. Hence, the hopping terms 
-are given by the kinetic Hamiltonian $\hat{H}^{\mathrm{kin}}_{0,k \alpha\beta}[\sigma]$, 
-and we can construct an array for each spin $\sigma$ separately. Each array 
-will be $\mathcal{N} \times n_{\mathrm{orb}} \times n_{\mathrm{orb}}$, where 
-$\mathcal{N}$ is the number of unit cells (sites in this case) on the 
-lattice and $n_{\mathrm{orb}}$ is the number of orbitals in each unit cell. 
-If the Hamiltonian was not block diagonal in spin, we would instead construct a 
-single $\mathcal{N} \times 2 n_{\mathrm{orb}} \times 2 n_{\mathrm{orb}}$ 
+Notice that the Hamiltonian is block diagonal in spin. Hence, the hopping terms
+are given by the kinetic Hamiltonian $\hat{H}^{\mathrm{kin}}_{0,k \alpha\beta}[\sigma]$,
+and we can construct an array for each spin $\sigma$ separately. Each array
+will be $\mathcal{N} \times n_{\mathrm{orb}} \times n_{\mathrm{orb}}$, where
+$\mathcal{N}$ is the number of unit cells (sites in this case) on the
+lattice and $n_{\mathrm{orb}}$ is the number of orbitals in each unit cell.
+If the Hamiltonian was not block diagonal in spin, we would instead construct a
+single $\mathcal{N} \times 2 n_{\mathrm{orb}} \times 2 n_{\mathrm{orb}}$
 array. You can block diagonalize however is appropriate for your problem.
 
-The easiest way to create this is as an array using `numpy`. We will 
-intentionally do this in a computationally slow way. The intention here is to 
-be explicit for clarity. First create the 
+The easiest way to create this is as an array using `numpy`. We will
+intentionally do this in a computationally slow way. The intention here is to
+be explicit for clarity. First create the
 $k$-grid mesh of the Brillouin zone in crystal coordinates
 
 ```python
 import numpy as np
 from itertools import product
 
 def make_kmesh(n_kx = 6, d = 3):
     """
-    Return a shifted Monkhorst-Pack k-space mesh on a hypercubic Bravais 
+    Return a shifted Monkhorst-Pack k-space mesh on a hypercubic Bravais
     lattice.
 
     Parameters
     ----------
     n_kx : int, optional
         Linear dimension of k-mesh in each dimension.
     d : int, optional
         Number of dimensions, e.g., d = 2 is the square lattice.
-    
+
     Returns
     -------
     mesh : numpy.ndarray
         The mesh in fractional coordinates, indexed as k, dim_1, dim_2, ..., dim_d
     """
-    
+
     # Total number of k-points on the mesh
     n_k = n_kx**d
 
     mesh = np.empty(shape=(n_k, d))
     coords = [range(n_kx) for _ in range(d)]
     for idx, coord in enumerate(product(*coords)):
         for i in range(len(coord)):
             mesh[idx,i] = coord[i] / float(n_kx) + 0.5 / float(n_kx)
-    
+
     return mesh
 ```
 
 Now construct $\hat{H}_0^{\mathrm{kin}}$ on this mesh.
 
 ```python
 def make_h0_kin_k(mesh, gf_struct, t = 1, a = 1):
     """
-    Return dispersion of degenerate orbitals on a hypercubic lattice as a 
+    Return dispersion of degenerate orbitals on a hypercubic lattice as a
     dictionary, where each key is the spin.
 
     Parameters
     ----------
     mesh : numpy.ndarray
         The k-space mesh of the Bravais lattice.
     gf_struct : list of pairs [ (str,int), ... ]
-        Structure of matrices. 
+        Structure of matrices.
     t : float, optional
         Hopping amplitude.
     a : float, optional
         Lattice spacing.
 
     Returns
     -------
@@ -161,81 +161,81 @@
         di = np.diag_indices(n_orb)
         h0_kin_k[bl] = np.zeros([n_k, n_orb, n_orb])
         h0_kin_k[bl][:,di[0],di[1]] = -2.0 * t * np.sum(np.cos(2.0 * a * np.pi * mesh), axis=1)[:, None]
 
     return h0_kin_k
 ```
 
-Note that the structure of the matrices is given in the same way as {{TRIQS}} 
+Note that the structure of the matrices is given in the same way as {{TRIQS}}
 Green's functions as
 
 ```python
 gf_struct = [ ("up", 2), ("dn", 2) ]
 ```
 
 ## B: Construct $\hat{H}_i^{\mathrm{loc}}$
 
-Next, construct the local Hamiltonian on each cluster (site) $i$. It has to 
-include all of the many-body interactions on each cluster as well as the 
+Next, construct the local Hamiltonian on each cluster (site) $i$. It has to
+include all of the many-body interactions on each cluster as well as the
 non-interacting quadratic terms that describe orbital energies and
-hopping between orbitals on site $i$. In this case, we use the 
+hopping between orbitals on site $i$. In this case, we use the
 second-quantized operators that the {{TRIQS}} library provides.
 
 ```python
 from triqs.operators import *
 
 def make_h_loc(V = 0.25, U = 4):
     """
     Return the local terms of the bilayer Hubbad model as a TRIQS operator.
-    
+
     Parameters
     ----------
     V : float, optional
         Hopping between orbitals on each cluster.
     U : float, optional
         Local Coulomb repulsion on each site.
 
     Returns
     -------
     h_loc : triqs.operators.Operator
     """
-    
+
     h_loc = Operator()
     for o in range(2):
         h_loc += U * n("up", o) * n("dn", o)
     for bl in ["up", "dn"]:
         h_loc += V * ( c_dag(bl, 0) * c(bl, 1) + c_dag(bl, 1) * c(bl, 0) )
 
     return h_loc
 ```
 
 ## C: Construct $\hat{H}^{\mathrm{qp}}$
 
-The first step in the self-consistent loop is to obtain the mean-field 
+The first step in the self-consistent loop is to obtain the mean-field
 quasiparticle Hamiltonian
 
 $$
-\hat{H}^{\mathrm{qp}} = 
+\hat{H}^{\mathrm{qp}} =
 \mathcal{R} \hat{H}^{\mathrm{kin}} \mathcal{R}^{\dagger}
 + \lambda,
 $$
 
-where $\mathcal{R}$ is the renormalization matrix and $\lambda$ is the 
-correlation potential matrix. They are assumed to be the same on every site, 
+where $\mathcal{R}$ is the renormalization matrix and $\lambda$ is the
+correlation potential matrix. They are assumed to be the same on every site,
 so that they are square matrices whose dimensions are $2 n_{\mathrm{orb}}$.
-It is useful to construct them with a block matrix structure, similarly to how 
+It is useful to construct them with a block matrix structure, similarly to how
 $\hat{H}^{\mathrm{kin}}_0$ was done.
 
-$\mathcal{R}$ and $\mathcal{\lambda}$ are mean-field matrices and are the 
-input initial guesses to the solution to the self-consistent loop. Often a 
-reasonable initial guess is to choose $\mathcal{R}$ as the identity and 
+$\mathcal{R}$ and $\mathcal{\lambda}$ are mean-field matrices and are the
+input initial guesses to the solution to the self-consistent loop. Often a
+reasonable initial guess is to choose $\mathcal{R}$ as the identity and
 $\lambda$ as the zero matrix.
 
-There is a helper function that constructs $\hat{H}^{\mathrm{qp}}$, and 
-it is simple to get its eigenvalues and eigenvectors at each $k$-point on the 
+There is a helper function that constructs $\hat{H}^{\mathrm{qp}}$, and
+it is simple to get its eigenvalues and eigenvectors at each $k$-point on the
 finite grid.
 
 ```python
 from risb import helpers
 
 energies_qp = dict()
 bloch_vector_qp = dict()
@@ -243,45 +243,45 @@
     h_qp = helpers.get_h_qp(R[bl], Lambda[bl], h0_kin_k[bl])
     energies_qp[bl], bloch_vector_qp[bl] = np.linalg.eigh(h_qp)
 ```
 
 ## D: Setup k-integrator function
 
 :::{seealso}
-[About k-integration](../explanations/kweight.md) for the theory of how 
+[About k-integration](../explanations/kweight.md) for the theory of how
 $k$-space integration is numerically done in most condensed matter codes.
 
-[Using `SmearingKWeight`](../how-to/kweight.md) for a class that implements 
+[Using `SmearingKWeight`](../how-to/kweight.md) for a class that implements
 the below weighting factor.
 :::
 
-Next you will need to construct how $k$-space integrals are performed. All 
-integrals are with respect to the eigenenergies $\xi^{\mathrm{qp}}_{kn}$ ($n$ 
+Next you will need to construct how $k$-space integrals are performed. All
+integrals are with respect to the eigenenergies $\xi^{\mathrm{qp}}_{kn}$ ($n$
 is a band index) of $\hat{H}^{\mathrm{qp}}$.
 
-The simplest approximation for the integration weight is to just use the 
-Fermi-Dirac distribution function $f(\xi)$ on a finite grid 
+The simplest approximation for the integration weight is to just use the
+Fermi-Dirac distribution function $f(\xi)$ on a finite grid
 at the inverse temperature $\beta$. That is,
 
 $$
 w(\xi^{\mathrm{qp}}_{kn}) = \frac{1}{\mathcal{N}} f(\xi^{\mathrm{qp}}_{kn}).
 $$
 
 The code to perform this is
 
 ```python
 def update_weights(energies, mu=0, beta=10):
     """
-    Return the integration weights for each band at each 
+    Return the integration weights for each band at each
     k-point on the lattice.
 
     Parameters
     ----------
     energies : dict[numpy.ndarray]
-        Energies at each k-point. Each key is a symmetry block, and its value 
+        Energies at each k-point. Each key is a symmetry block, and its value
         is the energy in each band n, indexed as k, n.
     mu : float, optional
         Chemical potential.
     beta : float, optional
         Inverse temperature.
 
     Returns
@@ -296,78 +296,78 @@
 
 ```python
 kweights = update_weights(energies = energies_qp, mu = ..., beta = ...)
 ```
 
 ## E: Setup mean-field matrices
 
-We now need to initialize the mean-field matrices used in 
-{{RISB}}. In {{RISB}} the homogenous assumption is taken, 
+We now need to initialize the mean-field matrices used in
+{{RISB}}. In {{RISB}} the homogenous assumption is taken,
 so that the matrices are the same on every site.
-Below we describe what each mean-field matrix physically relates to within 
+Below we describe what each mean-field matrix physically relates to within
 the algorithm.
 
-The single-particle quasiparticle density 
-matrix of $\hat{H}^{\mathrm{qp}}$ is $\Delta^{\mathrm{qp}}$ and the lopsided 
+The single-particle quasiparticle density
+matrix of $\hat{H}^{\mathrm{qp}}$ is $\Delta^{\mathrm{qp}}$ and the lopsided
 quasiparticle kinetic energy is $E^{c,\mathrm{qp}}$.
 
-The non-interacting quadratic parts of the embedding Hamiltonian 
-$\hat{H}^{\mathrm{emb}}$ are described by the hybridization matrix 
-$\mathcal{D}$, and the matrix that describes the couplings in the bath 
+The non-interacting quadratic parts of the embedding Hamiltonian
+$\hat{H}^{\mathrm{emb}}$ are described by the hybridization matrix
+$\mathcal{D}$, and the matrix that describes the couplings in the bath
 $\lambda^c$.
 
-The single-particle density matrices of $\hat{H}^{\mathrm{emb}}$ are the 
-density matrix of the f-electrons (the bath, these are quasiparticles) 
-$\Delta^{f}$, 
-the density matrix of the c-electrons (the impurity, these are physical 
-electrons) $\Delta^{c}$, 
-and the off-diagonal density matrix between the c- and f- electrons 
+The single-particle density matrices of $\hat{H}^{\mathrm{emb}}$ are the
+density matrix of the f-electrons (the bath, these are quasiparticles)
+$\Delta^{f}$,
+the density matrix of the c-electrons (the impurity, these are physical
+electrons) $\Delta^{c}$,
+and the off-diagonal density matrix between the c- and f- electrons
 (the impurity and the bath) $\Delta^{cf}$.
 
-```python 
+```python
 # H^qp parameters R and Lambda
 R = dict()
 Lambda = dict()
 for bl, bl_size in gf_struct:
     R[bl] = np.zeros((bl_size, bl_size))
     Lambda[bl] = np.zeros((bl_size, bl_size))
 
 # H^qp single-particle density matrix and (lopsided) kinetic energy
 rho_qp = dict()
 kinetic_energy_qp = dict()
 for bl, bl_size in gf_struct:
     rho_qp[bl] = np.zeros((bl_size, bl_size))
     kinetic_energy_qp[bl] = np.zeros((bl_size, bl_size))
-    
+
 # H^emb hybridization and bath terms
 D = dict()
 Lambda_c = dict()
 for bl, bl_size in gf_struct:
     D[bl] = np.zeros((bl_size, bl_size))
     Lambda_c[bl] = np.zeros((bl_size, bl_size))
-    
+
 # H^emb single-particle density matrices
 rho_f = dict()
 rho_cf = dict()
 rho_c = dict()
 for bl, bl_size in gf_struct:
     rho_f[bl] = np.zeros((bl_size, bl_size))
     rho_cf[bl] = np.zeros((bl_size, bl_size))
-    rho_c[bl] = np.zeros((bl_size, bl_size))   
+    rho_c[bl] = np.zeros((bl_size, bl_size))
 ```
 
 ### Helper functions
 
-As an aside, let me describe how to obtain the above mean-field matrices, which 
-has to be done at each iteration of the self-consistent process. There are 
-helper functions that do this for you. They simply take in numpy arrays 
+As an aside, let me describe how to obtain the above mean-field matrices, which
+has to be done at each iteration of the self-consistent process. There are
+helper functions that do this for you. They simply take in numpy arrays
 and either use `numpy.einsum` or `numpy.dot` arrays together.
 
-Remember that you can check the docstring of a helper function with 
-`help(helpers.function)`, which will even tell you which equation it relates 
+Remember that you can check the docstring of a helper function with
+`help(helpers.function)`, which will even tell you which equation it relates
 to within the [literature](../about.md#literature-of-original-theory).
 
 ```python
 from risb import helpers
 
 # H^qp single-particle density
 for bl, bl_size in gf_struct:
@@ -383,44 +383,43 @@
     D[bl] = helpers.get_d(rho_qp[bl], kinetic_energy_qp[bl])
 
 # H^emb bath
 for bl, bl_size in gf_struct:
     Lambda_c[bl] = helpers.get_lambda_c(rho_qp[bl], R[bl], Lambda[bl], D[bl])
 ```
 
-See [Solving $\hat{H}^{\mathrm{emb}}$](#f-solving-hat-h-mathrm-emb) for the 
+See [Solving $\hat{H}^{\mathrm{emb}}$](#f-solving-hat-h-mathrm-emb) for the
 single-particle density matrices of $\hat{H}^{\mathrm{emb}}$.
 
-
 ## F: Solving $\hat{H}^{\mathrm{emb}}$
 
 :::{seealso}
 [About the embedding Hamiltonian](../explanations/embedding.md).
 
 [Using embedding classes](../how-to/embedding.md).
 :::
 
-Now we have to solve the impurity problem defined by the embedding Hamiltonian 
-$\hat{H}^{\mathrm{emb}}$. There is a simple (but poorly scaled to large 
+Now we have to solve the impurity problem defined by the embedding Hamiltonian
+$\hat{H}^{\mathrm{emb}}$. There is a simple (but poorly scaled to large
 problems) implementation that only uses {{TRIQS}}.
 
 ```python
 from risb.embedding import EmbeddingAtomDiag
 
 embedding = EmbeddingAtomDiag(h_loc, gf_struct)
 ```
 
-Setting the embedding Hamiltonian $\hat{H}^{\mathrm{emb}}$ is done with 
+Setting the embedding Hamiltonian $\hat{H}^{\mathrm{emb}}$ is done with
 
 ```python
 embedding.set_h_emb(Lambda_c, D)
 ```
 
-Solving for the ground state in the $n_{\mathrm{orb}}$ particle sector, which 
-corresponds to the embedding problem being half-filled, is done with 
+Solving for the ground state in the $n_{\mathrm{orb}}$ particle sector, which
+corresponds to the embedding problem being half-filled, is done with
 
 ```python
 embedding.solve()
 ```
 
 The methods to calculate the single-particle density matrices are
 
@@ -429,70 +428,69 @@
     rho_f[bl] = embedding.get_rho_f(bl)
     rho_cf[bl] = embedding.get_rho_cf(bl)
     rho_c[bl] = embedding.get_rho_c(bl)
 ```
 
 ## G: Closing the loop
 
-After the embedding Hamiltonian is solved and the single-particle density 
-matrices of the embedding Hamiltonian are obtained, there are two ways to do 
-the self-consistency loop. The first is to calculate a new guess for 
-$\mathcal{R}$ and $\lambda$ which re-parameterizes $H^{\mathrm{qp}}$. 
+After the embedding Hamiltonian is solved and the single-particle density
+matrices of the embedding Hamiltonian are obtained, there are two ways to do
+the self-consistency loop. The first is to calculate a new guess for
+$\mathcal{R}$ and $\lambda$ which re-parameterizes $H^{\mathrm{qp}}$.
 The helper functions to do this are
 
 ```python
 from risb import helpers
 
 for bl, bl_size in gf_struct:
     Lambda[bl] = helpers.get_lambda(R[bl], D[bl], Lambda_c[bl], rho_f[bl])
     R[bl] = helpers.get_r(rho_cf[bl], rho_f[bl])
 ```
 
 The second is as a root problem, adjusting $\mathcal{R}$ and $\lambda$ to
-ensure that the density matrices from $\hat{H}^{\mathrm{qp}}$ match the 
+ensure that the density matrices from $\hat{H}^{\mathrm{qp}}$ match the
 density matrices from $\hat{H}^{\mathrm{emb}}$.
 
 ```python
 for bl, bl_size in gf_struct:
     f1 = helpers.get_f1(rho_cf[bl], rho_qp[bl], R[bl])
     f2 = helpers.get_f2(rho_f[bl], rho_qp[bl])
 ```
 
-
 ## Exercises
 
-1. Can you match each part above with the self-consistent loop defined in the 
-[literature](../about)?
+1. Can you match each part above with the self-consistent loop defined in the
+   [literature](../about)?
 1. Piece together everything above and write your own code.
 1. Solve for a range of $U$ values at half-filling ($\mu = U / 2$).
 1. How does $\beta$ and the size of the k-space mesh affect the results?
-1. What is the evolution of the quasiparticle weight $Z$ at 
-half-filling (Fig. 7)?
-1. What is the evolution of the electron filling in the 
-bonding/anti-bonding ($\pm$) basis?
-1. Implement a method to solve for the chemical potential $\mu$ at a fixed 
-electron density $n$ (you may find :py:func:`scipy.optimize.brentq` 
-or :py:func:`scipy.optimize.bisect` from :py:mod:`scipy.optimize` useful).
-1. What is the evolution of the quasiparticle weight at electron filling 
-$n = 1.88$ (Fig. 10)?
+1. What is the evolution of the quasiparticle weight $Z$ at
+   half-filling (Fig. 7)?
+1. What is the evolution of the electron filling in the
+   bonding/anti-bonding ($\pm$) basis?
+1. Implement a method to solve for the chemical potential $\mu$ at a fixed
+   electron density $n$ (you may find :py:func:`scipy.optimize.brentq`
+   or :py:func:`scipy.optimize.bisect` from :py:mod:`scipy.optimize` useful).
+1. What is the evolution of the quasiparticle weight at electron filling
+   $n = 1.88$ (Fig. 10)?
 
 ## Conclusion
 
-You have built the self-consistent loop for 
-{{RISB}} and solved a (not so simple) 
-interacting fermion problem. The code in :py:class:`risb.solve_lattice.LatticeSolver` 
-is not much more complicated than what you have done. You should now easily be 
-able to mofify, implement, and contribute to any parts in the library. 
-You also now understand the basic ingredients needed for most self-consistent 
-procedures in much more sophisticated codes for {{DFT}} and {{DMFT}}. 
-Hopefully, you can easily build upon this simple example to do much more 
+You have built the self-consistent loop for
+{{RISB}} and solved a (not so simple)
+interacting fermion problem. The code in :py:class:`risb.solve_lattice.LatticeSolver`
+is not much more complicated than what you have done. You should now easily be
+able to mofify, implement, and contribute to any parts in the library.
+You also now understand the basic ingredients needed for most self-consistent
+procedures in much more sophisticated codes for {{DFT}} and {{DMFT}}.
+Hopefully, you can easily build upon this simple example to do much more
 complicated things.
 
-Below is some code that should be very easy to fill in. But you will understand 
-much more about {{RISB}} if you try to piece everything together from the 
+Below is some code that should be very easy to fill in. But you will understand
+much more about {{RISB}} if you try to piece everything together from the
 self-consistent equations in the [literature](../about).
 
 ## Skeleton code cheat sheet
 
 Below is a simple self-consistent loop that relies on everything we have set up.
 
 ```python
@@ -505,35 +503,35 @@
 n_cycles = 25
 beta = 40
 n_orb = 2
 block_names = ['up','dn']
 gf_struct = [(bl, n_orb) for bl in block_names]
 
 # Implement step A
-h0_kin_k = 
+h0_kin_k =
 
 # Implement step B
-h_loc = 
+h_loc =
 
 # Implement step D
-update_weights = 
+update_weights =
 
 # Implement step E
-initialized_mean_field_matrices = 
+initialized_mean_field_matrices =
 ...
 
 # Implement step F
-embedding = 
+embedding =
 
 # H^qp parameters R and Lambda initialized to the non-interacting values
 for bl, bl_size in gf_struct:
     np.fill_diagonal(Lambda[bl], mu)
     np.fill_diagonal(R[bl], 1)
 
-for cycle in range(n_cycles):    
+for cycle in range(n_cycles):
     # For convergence checking
     norm = 0
     R_old = deepcopy(R)
     Lambda_old = deepcopy(Lambda)
 
     # Step C: construct H^qp
     for bl, bl_size in gf_struct:
@@ -573,19 +571,19 @@
     # Check how close the guess was
     for bl, bl_size in gf_struct:
         norm += np.linalg.norm(R[bl] - R_old[bl])
         norm += np.linalg.norm(Lambda[bl] - Lambda_old[bl])
 
         if norm < 1e-6:
             break
-    
+
 # Quasiparticle weight
 Z = dict()
 for bl, bl_size in gf_struct:
     Z[bl] = R[bl] @ R[bl].conj().T
 ```
 
-
-[^Lechermann2007]: [F. Lechermann, A. Georges, G. Kotliar, and O. Parcollet, 
-*Rotationally invariant slave-boson formalism and momentum dependence of the 
-quasiparticle weight*, 
-Phys. Rev.B **76**, 155102 (2007)](https://doi.org/10.1103/PhysRevB.76.155102)
+[^Lechermann2007]:
+    [F. Lechermann, A. Georges, G. Kotliar, and O. Parcollet,
+    _Rotationally invariant slave-boson formalism and momentum dependence of the
+    quasiparticle weight_,
+    Phys. Rev.B **76**, 155102 (2007)](https://doi.org/10.1103/PhysRevB.76.155102)
```

### Comparing `risb-0.1.0/examples/bilayer_hubbard.py` & `risb-0.1.1/examples/bilayer_hubbard.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,124 +1,156 @@
-import numpy as np
+# ruff: noqa: T201, D100, D103
 
-from triqs.lattice.tight_binding import TBLattice, BravaisLattice, BrillouinZone, MeshBrZone
-from triqs.operators import Operator, c_dag, c, n
+import numpy as np
+from triqs.gf import MeshImFreq, MeshProduct
+from triqs.lattice.tight_binding import (
+    BravaisLattice,
+    BrillouinZone,
+    MeshBrZone,
+    TBLattice,
+)
+from triqs.operators import Operator, n
+from triqs.operators.util.observables import N_op, S2_op
 from triqs.operators.util.op_struct import set_operator_structure
-from triqs.operators.util.observables import S2_op, N_op
-from triqs.gf import BlockGf, MeshImFreq, MeshProduct
 
 from risb import LatticeSolver
-from risb.kweight import SmearingKWeight
 from risb.embedding import EmbeddingAtomDiag
-from risb.helpers_triqs import get_g0_k_w, get_sigma_w, get_g_qp_k_w, get_g_k_w, get_g_w_loc
+from risb.helpers_triqs import (
+    get_g0_k_w,
+    get_g_k_w,
+    get_g_qp_k_w,
+    get_g_w_loc,
+    get_sigma_w,
+)
+from risb.kweight import SmearingKWeight
 
 # Number of orbitals and spin structure
 n_orb = 2
-spin_names = ['up','dn']
+spin_names = ["up", "dn"]
 gf_struct = set_operator_structure(spin_names, n_orb, off_diag=True)
 
 # Non-interacting cubic dispersion on lattice, built using TRIQS
-nkx = 10 # nkx**3 total number of k-points
-t = - 1.0 / 3.0 # hopping amplitude
-V = 0.25 # Bilayer hopping between orbitals on same site
-units = np.eye(3) # lattice vectors, a1, a2, a3 on a cube
+nkx = 10  # nkx**3 total number of k-points
+t = -1.0 / 3.0  # hopping amplitude
+V = 0.25  # Bilayer hopping between orbitals on same site
+units = np.eye(3)  # lattice vectors, a1, a2, a3 on a cube
 hoppings = {}
 for i in range(3):
-    hoppings[ tuple((units[:,i]).astype(int)) ] = np.eye(n_orb) * t
-    hoppings[ tuple((-units[:,i]).astype(int)) ] = np.eye(n_orb) * t
-    hoppings[ (0,0,0) ] = np.array([ [0, V], [V, 0] ])
-tbl = TBLattice(units=units, hoppings=hoppings, orbital_positions=[(0,0,0)]*n_orb)
+    hoppings[tuple((units[:, i]).astype(int))] = np.eye(n_orb) * t
+    hoppings[tuple((-units[:, i]).astype(int))] = np.eye(n_orb) * t
+    hoppings[(0, 0, 0)] = np.array([[0, V], [V, 0]])
+tbl = TBLattice(units=units, hoppings=hoppings, orbital_positions=[(0, 0, 0)] * n_orb)
 bl = BravaisLattice(units=units)
 bz = BrillouinZone(bl)
 mk = MeshBrZone(bz, nkx)
-h0_k = dict()
+h0_k = {}
 for bl, _ in gf_struct:
     h0_k[bl] = tbl.fourier(mk).data
 
-# Hubbard interactions    
+# Hubbard interactions
 U = 4
 h_int = Operator()
 for o in range(n_orb):
-    h_int += U * n("up",o) * n("dn",o)
+    h_int += U * n("up", o) * n("dn", o)
 
 # Set up class to work out k-space integration weights
-beta = 40 # inverse temperature
-n_target = 2 # half-filling
+beta = 40  # inverse temperature
+n_target = 2  # half-filling
 kweight = SmearingKWeight(beta=beta, n_target=n_target)
 # or fix mu = U/2 -> kweight = SmearingKWeight(beta=beta, mu=mu)
 
 # (Optional) set up function to symmetrize mean-field matrices
-#def symmetries(A):
+# def symmetries(A):
 #    n_clusters = len(A)
 #    A_sym = [0 for i in range(n_clusters)]
 #    for i in range(n_clusters):
 #        for bl in A[i]:
 #            A_sym[i] += A[i][bl] / len(A[i])
 #        for bl in A[i]:
 #            A[i][bl] = A_sym[i]
 #    return A
 
 # Set up class to solve embedding problem
 embedding = EmbeddingAtomDiag(h_int, gf_struct)
 
-# Setup RISB solver class  
+# Setup RISB solver class
 # gf_struct and embedding must be for each cluster. In this case
 # there is only one cluster, so a list with one cluster is passed.
-S = LatticeSolver(h0_k=h0_k,
-                  gf_struct=gf_struct,
-                  embedding=embedding,
-                  update_weights=kweight.update_weights)
-                  #symmetries=[symmetries])
+S = LatticeSolver(
+    h0_k=h0_k,
+    gf_struct=gf_struct,
+    embedding=embedding,
+    update_weights=kweight.update_weights,
+)
+# symmetries=[symmetries])
 
 # (Optional) Initialize R and Lambda matrices
-#for bl, bl_size in gf_struct:
+# for bl, bl_size in gf_struct:
 #    np.fill_diagonal(S.R[bl], 1)
 #    np.fill_diagonal(S.Lambda[bl], 0)
 
 # Solve
 S.solve(tol=1e-6)
- 
+
 # Average number of particles on a cluster
 total_number_Op = N_op(spin_names, n_orb, off_diag=True)
 total_number = embedding.overlap(total_number_Op)
 
 # Effective total spin of a cluster
 total_spin_Op = S2_op(spin_names, n_orb, off_diag=True)
 total_spin = embedding.overlap(total_spin_Op)
-        
+
 # Some different ways to construct some Green's functions
 
 # The k-space and frequency mesh of the problem
-iw_mesh = MeshImFreq(beta=beta, S='Fermion', n_max=64)
+iw_mesh = MeshImFreq(beta=beta, S="Fermion", n_max=64)
 k_iw_mesh = MeshProduct(mk, iw_mesh)
 
 mu = kweight.mu
 
 # Gf constructed from local self-energy
 G0_k_iw = get_g0_k_w(gf_struct=gf_struct, mesh=k_iw_mesh, h0_k=h0_k, mu=mu)
-Sigma_iw = get_sigma_w(mesh=iw_mesh, gf_struct=gf_struct, Lambda=S.Lambda[0], R=S.R[0], h0_loc=S.h0_loc_matrix[0], mu=mu)
+Sigma_iw = get_sigma_w(
+    mesh=iw_mesh,
+    gf_struct=gf_struct,
+    Lambda=S.Lambda[0],
+    R=S.R[0],
+    h0_loc=S.h0_loc_matrix[0],
+    mu=mu,
+)
 G_k_iw = get_g_k_w(g0_k_w=G0_k_iw, sigma_w=Sigma_iw)
-        
+
 # Gf constructed from quasiparticle Gf
-G_qp_k_iw = get_g_qp_k_w(gf_struct=gf_struct, mesh=k_iw_mesh, h0_kin_k=S.h0_kin_k, Lambda=S.Lambda[0], R=S.R[0], mu=mu)
+G_qp_k_iw = get_g_qp_k_w(
+    gf_struct=gf_struct,
+    mesh=k_iw_mesh,
+    h0_kin_k=S.h0_kin_k,
+    Lambda=S.Lambda[0],
+    R=S.R[0],
+    mu=mu,
+)
 G_k_iw2 = get_g_k_w(g_qp_k_w=G_qp_k_iw, R=S.R[0])
 
 # Local Green's functions integrated over k
-G0_iw_loc = get_g_w_loc(G0_k_iw) # this is using the correlated chemical potential, so will not have right filling
+G0_iw_loc = get_g_w_loc(
+    G0_k_iw
+)  # this is using the correlated chemical potential, so will not have right filling
 G_qp_iw_loc = get_g_w_loc(G_qp_k_iw)
 G_iw_loc = get_g_w_loc(G_k_iw)
 G_iw_loc2 = get_g_w_loc(G_k_iw2)
-        
+
 # Print out some interesting observables
-#with np.printoptions(formatter={'float': '{: 0.4f}'.format}):
+# with np.printoptions(formatter={'float': '{: 0.4f}'.format}):
 with np.printoptions(precision=4, suppress=True):
     print(f"Filling G0: {G0_iw_loc.total_density().real:.4f}")
     print(f"Filling G_qp: {G_qp_iw_loc.total_density().real:.4f}")
     print(f"Filling G: {G_iw_loc.total_density().real:.4f}")
     print(f"Filling G2: {G_iw_loc2.total_density().real:.4f}")
     for i in range(S.n_clusters):
         for bl, Z in S.Z[i].items():
             print(f"Quasiaprticle weight Z[{bl}] = \n{Z}")
         for bl, Lambda in S.Lambda[i].items():
             print(f"Correlation potential Lambda[{bl}] = \n{Lambda}")
         print(f"Number of partices per cluster N = \n{total_number:0.4f}")
-        print(f"Effective spin of a cluster S = \n{ -0.5 + 0.5 * np.sqrt( 1 + 4*total_spin) : 4f}")
+        print(
+            f"Effective spin of a cluster S = \n{ -0.5 + 0.5 * np.sqrt( 1 + 4*total_spin) : 4f}"
+        )
```

### Comparing `risb-0.1.0/examples/decorated_honeycomb.py` & `risb-0.1.1/examples/decorated_honeycomb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,189 +1,251 @@
-import numpy as np
+# ruff: noqa: T201, D100, D103
 from itertools import product
 
-from triqs.operators import Operator, c_dag, c
-from triqs.operators.util.op_struct import set_operator_structure
-from triqs.operators.util.observables import S2_op
+import numpy as np
+from triqs.operators import Operator, c, c_dag
 from triqs.operators.util.observables import N_op
 
 from risb import LatticeSolver
-from risb.kweight import SmearingKWeight
 from risb.embedding import EmbeddingAtomDiag, EmbeddingDummy
-from risb.helpers import get_h0_kin_k, block_to_full
+from risb.helpers import block_to_full, get_h0_kin_k
 from risb.helpers_triqs import get_h0_loc
+from risb.kweight import SmearingKWeight
+
 
-def get_h0_k(tg=0.5, tk=1.0, nkx=18, spin_names=['up','dn'], basis='trimer'):
-    na = 2 # Break up unit cell into 2 clusters
-    n_orb = 3 # Number of orbitals/sites per cluster
-    phi = 2.0 * np.pi / 3.0 # bloch factor for transforming to trimer orbital basis
-    n_k = nkx**2 # total number of k-points
+def get_h0_k(tg=0.5, tk=1.0, nkx=18, spin_names=None):
+    if spin_names is None:
+        spin_names = ["up", "dn"]
+    na = 2  # Break up unit cell into 2 clusters
+    n_orb = 3  # Number of orbitals/sites per cluster
+    phi = 2.0 * np.pi / 3.0  # bloch factor for transforming to trimer orbital basis
+    n_k = nkx**2  # total number of k-points
 
     # Build shifted 2D mesh
     mesh = np.empty(shape=(n_k, 2))
-    for idx,coords in enumerate(product(range(nkx), range(nkx))):
-        mesh[idx,0] = coords[0]/nkx + 0.5/nkx
-        mesh[idx,1] = coords[1]/nkx + 0.5/nkx
+    for idx, coords in enumerate(product(range(nkx), range(nkx))):
+        mesh[idx, 0] = coords[0] / nkx + 0.5 / nkx
+        mesh[idx, 1] = coords[1] / nkx + 0.5 / nkx
 
     # Unit cell lattice vectors
-    R1 = ( 3.0/2.0, np.sqrt(3.0)/2.0)
-    R2 = ( 3.0/2.0, -np.sqrt(3.0)/2.0)
+    R1 = (3.0 / 2.0, np.sqrt(3.0) / 2.0)
+    R2 = (3.0 / 2.0, -np.sqrt(3.0) / 2.0)
     R = np.array((R1, R2)).T
 
     # Bravais lattice vectors
-    G = 2.0*np.pi*np.linalg.inv(R).T
+    G = 2.0 * np.pi * np.linalg.inv(R).T
 
     # Vectors to inter-triangle nearest neighbors
-    d0 = ( 1.0, 0.0 )
-    d1 = ( -0.5, np.sqrt(3.0)/2.0 )
-    d2 = ( -0.5, -np.sqrt(3.0)/2.0 )
+    d0 = (1.0, 0.0)
+    d1 = (-0.5, np.sqrt(3.0) / 2.0)
+    d2 = (-0.5, -np.sqrt(3.0) / 2.0)
     d_vec = [d0, d1, d2]
-        
+
     h0_k = np.zeros([n_k, na, na, n_orb, n_orb], dtype=complex)
 
-    # Construct in inequivalent block matrix structure  
-    for k,i,j,m,mm in product(range(n_k), range(na), range(na), range(n_orb), range(n_orb)):
-        kay = np.dot(G, mesh[k,:])
+    # Construct in inequivalent block matrix structure
+    for k, i, j, m, mm in product(
+        range(n_k), range(na), range(na), range(n_orb), range(n_orb)
+    ):
+        kay = np.dot(G, mesh[k, :])
 
         # Dispersion terms between clusters
         if (i == 0) and (j == 1):
             for a in range(n_orb):
-                h0_k[k,i,j,m,mm] += - (tg/3.0) * np.exp(1j * kay @ d_vec[a]) * np.exp(1j * phi * (mm-m) * a)
+                h0_k[k, i, j, m, mm] += (
+                    -(tg / 3.0)
+                    * np.exp(1j * kay @ d_vec[a])
+                    * np.exp(1j * phi * (mm - m) * a)
+                )
         elif (i == 1) and (j == 0):
             for a in range(n_orb):
-                h0_k[k,i,j,m,mm] += - (tg/3.0) * np.exp(-1j * kay @ d_vec[a]) * np.exp(-1j * phi * (m-mm) * a)
+                h0_k[k, i, j, m, mm] += (
+                    -(tg / 3.0)
+                    * np.exp(-1j * kay @ d_vec[a])
+                    * np.exp(-1j * phi * (m - mm) * a)
+                )
         # Local terms on a cluster
         elif (i == j) and (m == mm):
-                h0_k[k,i,j,m,mm] = -2.0 * tk * np.cos(m * phi)
+            h0_k[k, i, j, m, mm] = -2.0 * tk * np.cos(m * phi)
         else:
             continue
-        
+
     # Get rid of the inequivalent block structure
-    h0_k_out = dict()
+    h0_k_out = {}
     for bl in spin_names:
-        h0_k_out[bl] = block_to_full( h0_k )
+        h0_k_out[bl] = block_to_full(h0_k)
     return h0_k_out
 
+
 def get_hubb_trimer(spin_names, U=0, tk=0):
     n_orb = 3
-    phi = 2.0 * np.pi / n_orb # bloch factor for transforming to molecular orbital basis
-    block_map = {0:'A', 1:'E1', 2:'E2'}
-    orb_map = {0:0, 1:0, 2:0}
+    phi = (
+        2.0 * np.pi / n_orb
+    )  # bloch factor for transforming to molecular orbital basis
+    block_map = {0: "A", 1: "E1", 2: "E2"}
+    orb_map = {0: 0, 1: 0, 2: 0}
+
     def get_c(s, m, dagger):
         if dagger:
             return c_dag(s + "_" + block_map[m], orb_map[m])
-        else:
-            return c(s + "_" + block_map[m], orb_map[m])
+        return c(s + "_" + block_map[m], orb_map[m])
+
     spin_up = spin_names[0]
     spin_dn = spin_names[1]
-    
+
     h_loc = Operator()
-    for a,m,mm,s in product(range(n_orb), range(n_orb), range(n_orb), spin_names):
-        h_loc += (-tk / float(n_orb)) * get_c(s, m, True) * get_c(s, mm, False) * np.exp(-1j * phi * a * m) * np.exp(1j * phi * np.mod(a+1,n_orb) * mm)
-        h_loc += (-tk / float(n_orb)) * get_c(s, m, True) * get_c(s, mm, False) * np.exp(-1j * phi * np.mod(a+1,n_orb) * m) * np.exp(1j * phi * a * mm)
-
-    for m,mm,mmm in product(range(n_orb), range(n_orb), range(n_orb)):
-        h_loc += (U / float(n_orb)) * get_c(spin_up, m, True) * get_c(spin_up, mm, False) \
-            * get_c(spin_dn, mmm, True) * get_c(spin_dn, np.mod(m+mmm-mm, n_orb), False)
-    
+    for a, m, mm, s in product(range(n_orb), range(n_orb), range(n_orb), spin_names):
+        h_loc += (
+            (-tk / float(n_orb))
+            * get_c(s, m, True)
+            * get_c(s, mm, False)
+            * np.exp(-1j * phi * a * m)
+            * np.exp(1j * phi * np.mod(a + 1, n_orb) * mm)
+        )
+        h_loc += (
+            (-tk / float(n_orb))
+            * get_c(s, m, True)
+            * get_c(s, mm, False)
+            * np.exp(-1j * phi * np.mod(a + 1, n_orb) * m)
+            * np.exp(1j * phi * a * mm)
+        )
+
+    for m, mm, mmm in product(range(n_orb), range(n_orb), range(n_orb)):
+        h_loc += (
+            (U / float(n_orb))
+            * get_c(spin_up, m, True)
+            * get_c(spin_up, mm, False)
+            * get_c(spin_dn, mmm, True)
+            * get_c(spin_dn, np.mod(m + mmm - mm, n_orb), False)
+        )
+
     return h_loc.real
 
+
 # Setup problem and gf_struct for each inequivalent trimer cluster
 n_clusters = 2
 n_orb = 3
-spin_names = ['up','dn']
+spin_names = ["up", "dn"]
 
 # Setup non-interacting Hamiltonian matrix on the lattice
 tg = 0.5
 nkx = 18
 h0_k = get_h0_k(tg=tg, nkx=nkx, spin_names=spin_names)
 
 # Set up class to work out k-space integration weights
-beta = 40 # inverse temperature
-n_target = 8 # 2/3rds filling
+beta = 40  # inverse temperature
+n_target = 8  # 2/3rds filling
 kweight = SmearingKWeight(beta=beta, n_target=n_target)
 
 # Set up gf_structure of clusters
-gf_struct_molecule = [('up_A', 1), ('up_E1', 1), ('up_E2', 1), ('dn_A', 1), ('dn_E1', 1), ('dn_E2', 1)]
-gf_struct_molecule_mapping = {'up_A':'up', 'up_E1':'up', 'up_E2':'up', 'dn_A':'dn', 'dn_E1':'dn', 'dn_E2':'dn'}
+gf_struct_molecule = [
+    ("up_A", 1),
+    ("up_E1", 1),
+    ("up_E2", 1),
+    ("dn_A", 1),
+    ("dn_E1", 1),
+    ("dn_E2", 1),
+]
+gf_struct_molecule_mapping = {
+    "up_A": "up",
+    "up_E1": "up",
+    "up_E2": "up",
+    "dn_A": "dn",
+    "dn_E1": "dn",
+    "dn_E2": "dn",
+}
 gf_struct = [gf_struct_molecule for _ in range(n_clusters)]
 gf_struct_mapping = [gf_struct_molecule_mapping for _ in range(n_clusters)]
 
 # Make projectors onto each trimer cluster
-projectors = [dict() for i in range(n_clusters)]
+projectors = [{} for i in range(n_clusters)]
 for i in range(n_clusters):
-    projectors[i]['up_A'] =  np.eye(n_clusters*n_orb)[0+i*n_orb:1+i*n_orb, :]
-    projectors[i]['dn_A'] =  np.eye(n_clusters*n_orb)[0+i*n_orb:1+i*n_orb, :]
-    projectors[i]['up_E1'] =  np.eye(n_clusters*n_orb)[1+i*n_orb:2+i*n_orb, :]
-    projectors[i]['dn_E1'] =  np.eye(n_clusters*n_orb)[1+i*n_orb:2+i*n_orb, :]
-    projectors[i]['up_E2'] =  np.eye(n_clusters*n_orb)[2+i*n_orb:3+i*n_orb, :]
-    projectors[i]['dn_E2'] =  np.eye(n_clusters*n_orb)[2+i*n_orb:3+i*n_orb, :]
+    projectors[i]["up_A"] = np.eye(n_clusters * n_orb)[0 + i * n_orb : 1 + i * n_orb, :]
+    projectors[i]["dn_A"] = np.eye(n_clusters * n_orb)[0 + i * n_orb : 1 + i * n_orb, :]
+    projectors[i]["up_E1"] = np.eye(n_clusters * n_orb)[
+        1 + i * n_orb : 2 + i * n_orb, :
+    ]
+    projectors[i]["dn_E1"] = np.eye(n_clusters * n_orb)[
+        1 + i * n_orb : 2 + i * n_orb, :
+    ]
+    projectors[i]["up_E2"] = np.eye(n_clusters * n_orb)[
+        2 + i * n_orb : 3 + i * n_orb, :
+    ]
+    projectors[i]["dn_E2"] = np.eye(n_clusters * n_orb)[
+        2 + i * n_orb : 3 + i * n_orb, :
+    ]
 
 # Get the non-interacting kinetic Hamiltonian matrix on the lattice
 h0_kin_k = get_h0_kin_k(h0_k, projectors, gf_struct_mapping=gf_struct_mapping)
 
 # Get the non-interacting local operator terms
-h0_loc = [get_h0_loc(h0_k=h0_k, P=P, gf_struct_mapping=gf_struct_mapping[i]) for i,P in enumerate(projectors)]
+h0_loc = [
+    get_h0_loc(h0_k=h0_k, P=P, gf_struct_mapping=gf_struct_mapping[i])
+    for i, P in enumerate(projectors)
+]
 
 # Get the local interaction operator terms
 U = 4
 h_int = [get_hubb_trimer(spin_names=spin_names, U=U) for i in range(n_clusters)]
 
 # Define the local Hamiltonian
 h_loc = [h0_loc[i] + h_int[i] for i in range(n_clusters)]
 
-# Set up embedding solvers 
-#embedding = [EmbeddingAtomDiag(h_loc[i], gf_struct[i]) for i in range(n_clusters)]
+# Set up embedding solvers
+# embedding = [EmbeddingAtomDiag(h_loc[i], gf_struct[i]) for i in range(n_clusters)]
 embedding = [EmbeddingAtomDiag(h_loc[0], gf_struct[0])]
-for i in range(n_clusters-1):
-    embedding.append( EmbeddingDummy(embedding[0]) )
+for _ in range(n_clusters - 1):
+    embedding.append(EmbeddingDummy(embedding[0]))
+
 
 def symmetries(A):
     n_clusters = len(A)
     # Paramagnetic
     for i in range(n_clusters):
-        A[i]['up_A'] = 0.5 * (A[i]['up_A'] + A[i]['dn_A'])
-        A[i]['dn_A'] = A[i]['up_A']
-        A[i]['up_E1'] = 0.5 * (A[i]['up_E1'] + A[i]['dn_E1'])
-        A[i]['dn_E1'] = A[i]['up_E1']
-        A[i]['up_E2'] = 0.5 * (A[i]['up_E2'] + A[i]['dn_E2'])
-        A[i]['dn_E2'] = A[i]['up_E2']
+        A[i]["up_A"] = 0.5 * (A[i]["up_A"] + A[i]["dn_A"])
+        A[i]["dn_A"] = A[i]["up_A"]
+        A[i]["up_E1"] = 0.5 * (A[i]["up_E1"] + A[i]["dn_E1"])
+        A[i]["dn_E1"] = A[i]["up_E1"]
+        A[i]["up_E2"] = 0.5 * (A[i]["up_E2"] + A[i]["dn_E2"])
+        A[i]["dn_E2"] = A[i]["up_E2"]
     # E1 = E2.conj()
     for i in range(n_clusters):
-        A[i]['up_E2'] = A[i]['up_E1'].conj().T
-        A[i]['dn_E2'] = A[i]['dn_E1'].conj().T
+        A[i]["up_E2"] = A[i]["up_E1"].conj().T
+        A[i]["dn_E2"] = A[i]["dn_E1"].conj().T
     return A
 
-# Setup RISB solver class  
-S = LatticeSolver(h0_k=h0_kin_k,
-                  gf_struct=gf_struct,
-                  embedding=embedding,
-                  update_weights=kweight.update_weights,
-                  projectors=projectors,
-                  symmetries=[symmetries],
-                  gf_struct_mapping=gf_struct_mapping,
+
+# Setup RISB solver class
+S = LatticeSolver(
+    h0_k=h0_kin_k,
+    gf_struct=gf_struct,
+    embedding=embedding,
+    update_weights=kweight.update_weights,
+    projectors=projectors,
+    symmetries=[symmetries],
+    gf_struct_mapping=gf_struct_mapping,
 )
 
 # Solve
 S.solve(tol=1e-4)
-#for i in range(5):
+# for i in range(5):
 #    x = S.solve(one_shot=True)
- 
+
 # Average number of particles on a cluster
 NOp = N_op(spin_names, n_orb, off_diag=True)
-#N = [e.overlap(NOp) for e in embedding]
+# N = [e.overlap(NOp) for e in embedding]
 #
 ## Effective total spin of a cluster
-#S2Op = S2_op(spin_names, n_orb, off_diag=True)
-#S2 = [e.overlap(S2Op) for e in embedding]
+# S2Op = S2_op(spin_names, n_orb, off_diag=True)
+# S2 = [e.overlap(S2Op) for e in embedding]
 #
 # Print out some interesting observables
-with np.printoptions(formatter={'float': '{: 0.4f}'.format}):
+with np.printoptions(formatter={"float": "{: 0.4f}".format}):
     for i in range(S.n_clusters):
         print(f"Cluster {i}:")
         for bl, Z in S.Z[i].items():
             print(f"Quasiaprticle weight Z[{bl}] = \n{Z}")
         for bl, Lambda in S.Lambda[i].items():
             print(f"Correlation potential Lambda[{bl}] = \n{Lambda}")
 #        print(f"Number of partices on cluster N = \n{N[i]:0.4f}")
 #        print(f"Effective spin of cluster S = \n{(0.5 * np.sqrt(4 * (S2[i] + 1)) - 1):0.4f}")
-#        print()
+#        print()
```

### Comparing `risb-0.1.0/examples/hubbard.py` & `risb-0.1.1/examples/hubbard.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,158 @@
+# ruff: noqa: T201, D100, D103
+import matplotlib.pyplot as plt
 import numpy as np
-
-from triqs.lattice.tight_binding import TBLattice, BravaisLattice, BrillouinZone, MeshBrZone
+from triqs.gf import MeshImFreq, MeshProduct
+from triqs.lattice.tight_binding import (
+    BravaisLattice,
+    BrillouinZone,
+    MeshBrZone,
+    TBLattice,
+)
 from triqs.operators import Operator, n
+from triqs.operators.util.observables import N_op, S2_op
 from triqs.operators.util.op_struct import set_operator_structure
-from triqs.operators.util.observables import S2_op, N_op
-from triqs.gf import MeshImFreq, MeshProduct
 
 from risb import LatticeSolver
-from risb.kweight import SmearingKWeight
 from risb.embedding import EmbeddingAtomDiag
-from risb.helpers_triqs import get_g0_k_w, get_sigma_w, get_g_qp_k_w, get_g_k_w, get_g_w_loc
+from risb.helpers_triqs import (
+    get_g0_k_w,
+    get_g_k_w,
+    get_g_qp_k_w,
+    get_g_w_loc,
+    get_sigma_w,
+)
+from risb.kweight import SmearingKWeight
 
-import matplotlib.pyplot as plt
 
 def hubbard(U, n_orb):
     h_int = Operator()
     for o in range(n_orb):
-        h_int += U * n("up",o) * n("dn",o)
+        h_int += U * n("up", o) * n("dn", o)
     return h_int
 
+
 # Number of orbitals and spin structure
 n_orb = 1
-spin_names = ['up', 'dn']
+spin_names = ["up", "dn"]
 gf_struct = set_operator_structure(spin_names, n_orb, off_diag=True)
 
 # Non-interacting cubic dispersion on lattice, built using TRIQS
-nkx = 10 # nkx**3 total number of k-points
-t = - 1.0 / 3.0 # hopping amplitude
-units = np.eye(3) # lattice vectors, a1, a2, a3 on a cube
+nkx = 10  # nkx**3 total number of k-points
+t = -1.0 / 3.0  # hopping amplitude
+units = np.eye(3)  # lattice vectors, a1, a2, a3 on a cube
 hoppings = {}
 for i in range(3):
-    hoppings[ tuple((units[:,i]).astype(int)) ] = np.eye(n_orb) * t
-    hoppings[ tuple((-units[:,i]).astype(int)) ] = np.eye(n_orb) * t
-tbl = TBLattice(units=units, hoppings=hoppings, orbital_positions=[(0,0,0)]*n_orb)
+    hoppings[tuple((units[:, i]).astype(int))] = np.eye(n_orb) * t
+    hoppings[tuple((-units[:, i]).astype(int))] = np.eye(n_orb) * t
+tbl = TBLattice(units=units, hoppings=hoppings, orbital_positions=[(0, 0, 0)] * n_orb)
 bl = BravaisLattice(units=units)
 bz = BrillouinZone(bl)
 mk = MeshBrZone(bz, nkx)
-h0_k = dict()
+h0_k = {}
 for bl, _ in gf_struct:
     h0_k[bl] = tbl.fourier(mk).data
 
 # Hubbard interaction
 h_int = hubbard(U=0, n_orb=n_orb)
 
 # Set up class to work out k-space integration weights
-beta = 40 # inverse temperature
-n_target = 1 # half-filling
+beta = 40  # inverse temperature
+n_target = 1  # half-filling
 kweight = SmearingKWeight(beta=beta, n_target=n_target)
 
+
 # Symmetrize spin blocks to be the same (paramagnetism)
 def force_paramagnetic(A):
     # Paramagnetic
-    A[0]['up'] = 0.5 * (A[0]['up'] + A[0]['dn'])
-    A[0]['dn'] = A[0]['up']
+    A[0]["up"] = 0.5 * (A[0]["up"] + A[0]["dn"])
+    A[0]["dn"] = A[0]["up"]
     return A
 
+
 # Set up class to solve embedding problem
 embedding = EmbeddingAtomDiag(h_int, gf_struct)
 
-# Setup RISB solver class  
-S = LatticeSolver(h0_k=h0_k,
-                  gf_struct=gf_struct,
-                  embedding=embedding,
-                  update_weights=kweight.update_weights,
-                  symmetries=[force_paramagnetic],
-                  force_real=True
+# Setup RISB solver class
+S = LatticeSolver(
+    h0_k=h0_k,
+    gf_struct=gf_struct,
+    embedding=embedding,
+    update_weights=kweight.update_weights,
+    symmetries=[force_paramagnetic],
+    force_real=True,
 )
 
 # Some observables
 total_number_Op = N_op(spin_names, n_orb, off_diag=True)
 total_spin_Op = S2_op(spin_names, n_orb, off_diag=True)
 Z = []
-total_number = [] # Avg particle number per site
-total_spin = [] # Total spin per site
+total_number = []  # Avg particle number per site
+total_spin = []  # Total spin per site
 
-U_arr = np.arange(0, 10+0.1, 0.5)
+U_arr = np.arange(0, 10 + 0.1, 0.5)
 for U in U_arr:
-    embedding.set_h_int( hubbard(U=U, n_orb=n_orb) )
-    
+    embedding.set_h_int(hubbard(U=U, n_orb=n_orb))
+
     # Solve
     S.solve(tol=1e-6)
- 
-    total_number.append( embedding.overlap(total_number_Op) )
-    total_spin.append( embedding.overlap(total_spin_Op) )
-    Z.append(S.Z[0]['up'][0,0])
-    
+
+    total_number.append(embedding.overlap(total_number_Op))
+    total_spin.append(embedding.overlap(total_spin_Op))
+    Z.append(S.Z[0]["up"][0, 0])
+
     if np.abs(U - 3.5) < 1e-10:
         # Some different ways to construct some Green's functions
         mu = kweight.mu
 
         # The k-space and frequency mesh of the problem
-        iw_mesh = MeshImFreq(beta=beta, S='Fermion', n_max=64)
+        iw_mesh = MeshImFreq(beta=beta, S="Fermion", n_max=64)
         k_iw_mesh = MeshProduct(mk, iw_mesh)
 
         mu = kweight.mu
 
         # Gf constructed from local self-energy
         G0_k_iw = get_g0_k_w(gf_struct=gf_struct, mesh=k_iw_mesh, h0_k=h0_k, mu=mu)
-        Sigma_iw = get_sigma_w(mesh=iw_mesh, gf_struct=gf_struct, Lambda=S.Lambda[0], R=S.R[0], h0_loc=S.h0_loc_matrix[0], mu=mu)
+        Sigma_iw = get_sigma_w(
+            mesh=iw_mesh,
+            gf_struct=gf_struct,
+            Lambda=S.Lambda[0],
+            R=S.R[0],
+            h0_loc=S.h0_loc_matrix[0],
+            mu=mu,
+        )
         G_k_iw = get_g_k_w(g0_k_w=G0_k_iw, sigma_w=Sigma_iw)
-                
+
         # Gf constructed from quasiparticle Gf
-        G_qp_k_iw = get_g_qp_k_w(gf_struct=gf_struct, mesh=k_iw_mesh, h0_kin_k=S.h0_kin_k, Lambda=S.Lambda[0], R=S.R[0], mu=mu)
+        G_qp_k_iw = get_g_qp_k_w(
+            gf_struct=gf_struct,
+            mesh=k_iw_mesh,
+            h0_kin_k=S.h0_kin_k,
+            Lambda=S.Lambda[0],
+            R=S.R[0],
+            mu=mu,
+        )
         G_k_iw2 = get_g_k_w(g_qp_k_w=G_qp_k_iw, R=S.R[0])
-        
+
         # Local Gf integrated over k
-        G0_iw_loc = get_g_w_loc(G0_k_iw) # this is using the correlated chemical potential, so will not have right filling
+        G0_iw_loc = get_g_w_loc(
+            G0_k_iw
+        )  # this is using the correlated chemical potential, so will not have right filling
         G_qp_iw_loc = get_g_w_loc(G_qp_k_iw)
         G_iw_loc = get_g_w_loc(G_k_iw)
         G_iw_loc2 = get_g_w_loc(G_k_iw2)
-        
+
         # Filling of physical electron scales with Z
         print(f"Filling G0: {G0_iw_loc.total_density().real:.4f}")
         print(f"Filling G_qp: {G_qp_iw_loc.total_density().real:.4f}")
         print(f"Filling G: {G_iw_loc.total_density().real:.4f}")
         print(f"Filling G2: {G_iw_loc2.total_density().real:.4f}")
         print(f"Filling Z:: {S.Z[0]['up'][0,0]:.4f}")
-        
-fig, axis = plt.subplots(1,2)
-axis[0].plot(U_arr, Z, '-ok')
-axis[0].set_xlabel(r'$U$')
-axis[0].set_ylabel(r'$Z$')
-axis[1].plot(U_arr, -0.5 + 0.5 * np.sqrt( 1 + 4*np.array(total_spin) ), '-ok')
-axis[1].set_xlabel(r'$U$')
-axis[1].set_ylabel(r'$\mathcal{S}$')
-plt.show()
+
+fig, axis = plt.subplots(1, 2)
+axis[0].plot(U_arr, Z, "-ok")
+axis[0].set_xlabel(r"$U$")
+axis[0].set_ylabel(r"$Z$")
+axis[1].plot(U_arr, -0.5 + 0.5 * np.sqrt(1 + 4 * np.array(total_spin)), "-ok")
+axis[1].set_xlabel(r"$U$")
+axis[1].set_ylabel(r"$\mathcal{S}$")
+plt.show()
```

### Comparing `risb-0.1.0/examples/kagome_hubbard.py` & `risb-0.1.1/examples/kagome_hubbard.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,141 @@
-import numpy as np
+# ruff: noqa: T201, D100, D103
 from itertools import product
 
+import numpy as np
 from triqs.operators import n
+from triqs.operators.util.observables import N_op, S2_op
 from triqs.operators.util.op_struct import set_operator_structure
-from triqs.operators.util.observables import S2_op
-from triqs.operators.util.observables import N_op
 
 from risb import LatticeSolver
-from risb.kweight import SmearingKWeight
 from risb.embedding import EmbeddingAtomDiag, EmbeddingDummy
+from risb.kweight import SmearingKWeight
+
 
-def get_h0_k(t=1, nkx=18, spin_names=['up','dn']):
+def get_h0_k(t=1, nkx=18, spin_names=None):
+    if spin_names is None:
+        spin_names = ["up", "dn"]
     n_orb = 3
 
     # Build shifted 2D mesh
     n_k = nkx**2
     mesh = np.empty(shape=(n_k, 2))
-    for idx,coords in enumerate(product(range(nkx), range(nkx))):
-        mesh[idx,0] = coords[0]/nkx + 0.5/nkx
-        mesh[idx,1] = coords[1]/nkx + 0.5/nkx
+    for idx, coords in enumerate(product(range(nkx), range(nkx))):
+        mesh[idx, 0] = coords[0] / nkx + 0.5 / nkx
+        mesh[idx, 1] = coords[1] / nkx + 0.5 / nkx
 
     # Unit cell lattice vectors
-    R1 = ( 1.0, 0 )
-    R2 = ( 0.5, np.sqrt(3.0)/2.0)
+    R1 = (1.0, 0)
+    R2 = (0.5, np.sqrt(3.0) / 2.0)
     R = np.array((R1, R2)).T
 
     # Bravais lattice vectors
-    G = 2.0*np.pi*np.linalg.inv(R).T
+    G = 2.0 * np.pi * np.linalg.inv(R).T
 
     h0_k = np.zeros([n_k, n_orb, n_orb], dtype=complex)
     for k in range(n_k):
-        kay = np.dot(G, mesh[k,:])
+        kay = np.dot(G, mesh[k, :])
         k1 = kay[0]
         k2 = 0.5 * kay[0] + 0.5 * np.sqrt(3) * kay[1]
         k3 = -0.5 * kay[0] + 0.5 * np.sqrt(3) * kay[1]
 
-        h0_k[k][...] = np.array( [ [                         0, -2 * t * np.cos(0.5 * k1), -2 * t * np.cos(0.5 * k2) ],
-                                   [ -2 * t * np.cos(0.5 * k1),                         0, -2 * t * np.cos(0.5 * k3) ],
-                                   [ -2 * t * np.cos(0.5 * k2), -2 * t * np.cos(0.5 * k3),                         0 ] ] 
-                                )
-            
-    h0_k_out = dict()
+        h0_k[k][...] = np.array(
+            [
+                [0, -2 * t * np.cos(0.5 * k1), -2 * t * np.cos(0.5 * k2)],
+                [-2 * t * np.cos(0.5 * k1), 0, -2 * t * np.cos(0.5 * k3)],
+                [-2 * t * np.cos(0.5 * k2), -2 * t * np.cos(0.5 * k3), 0],
+            ]
+        )
+
+    h0_k_out = {}
     for bl in spin_names:
         h0_k_out[bl] = h0_k
     return h0_k_out
 
-# Setup problem and gf_struct. There are three inequivalent clusters with one 
+
+# Setup problem and gf_struct. There are three inequivalent clusters with one
 # orbital per cluster.
 n_clusters = 3
 n_orb = 1
-spin_names = ['up','dn']
-gf_struct = [set_operator_structure(spin_names, n_orb, off_diag=True) for _ in range(n_clusters)]
+spin_names = ["up", "dn"]
+gf_struct = [
+    set_operator_structure(spin_names, n_orb, off_diag=True) for _ in range(n_clusters)
+]
 
 # Setup non-interacting Hamiltonian matrix on the lattice
-h0_k = get_h0_k(t = 1, nkx = 18, spin_names = spin_names)
+h0_k = get_h0_k(t=1, nkx=18, spin_names=spin_names)
 # For testing because on mac it returns nans
-for bl in h0_k.keys():
+for bl in h0_k:
     idx = np.where(np.isnan(h0_k[bl]))
     h0_k[bl][idx] = 0
 
 # Set up class to work out k-space integration weights
-beta = 40 # inverse temperature
-n_target = 3 # half-filling
+beta = 40  # inverse temperature
+n_target = 3  # half-filling
 kweight = SmearingKWeight(beta=beta, n_target=n_target)
 
-# Define the local interaction 
+# Define the local interaction
 U = 10
-h_int = [U * n('up', 0) * n('dn', 0) for _ in range(n_clusters)]
+h_int = [U * n("up", 0) * n("dn", 0) for _ in range(n_clusters)]
 
-# Set up embedding solvers 
-# Assuming all of the sites are equivalent it is sufficient to just solve for 
+# Set up embedding solvers
+# Assuming all of the sites are equivalent it is sufficient to just solve for
 # one site and copy and paste onto the other sites
 embedding = [EmbeddingAtomDiag(h_int[0], gf_struct[0])]
-embedding.append( EmbeddingDummy(embedding[0]) )
-embedding.append( EmbeddingDummy(embedding[0]) )
+embedding.append(EmbeddingDummy(embedding[0]))
+embedding.append(EmbeddingDummy(embedding[0]))
 
 # Setup projectors onto the three correlated spaces in a unit cell
 # Dictionaries of projectors onto each cluster
-P_A = { bl : np.array( [ [1, 0, 0] ] ) for bl in spin_names }
-P_B = { bl : np.array( [ [0, 1, 0] ] ) for bl in spin_names }
-P_C = { bl : np.array( [ [0, 0, 1] ] ) for bl in spin_names }
+P_A = {bl: np.array([[1, 0, 0]]) for bl in spin_names}
+P_B = {bl: np.array([[0, 1, 0]]) for bl in spin_names}
+P_C = {bl: np.array([[0, 0, 1]]) for bl in spin_names}
 projectors = [P_A, P_B, P_C]
 
-# Enforce paramagnetism. This is not really necessary because the primitive 
-# unit cell will not magnetically order. But it helps to stabalize the 
+
+# Enforce paramagnetism. This is not really necessary because the primitive
+# unit cell will not magnetically order. But it helps to stabalize the
 # solver in the insulating state
 def force_paramagnetic(A):
     n_clusters = len(A)
     for i in range(n_clusters):
-        A[i]['up'] = 0.5 * ( A[i]['up'] + A[i]['dn'] )
-        A[i]['dn'] = A[i]['up']
+        A[i]["up"] = 0.5 * (A[i]["up"] + A[i]["dn"])
+        A[i]["dn"] = A[i]["up"]
     return A
 
-# Setup RISB solver class  
-S = LatticeSolver(h0_k=h0_k,
-                  gf_struct=gf_struct,
-                  embedding=embedding,
-                  update_weights=kweight.update_weights,
-                  projectors=projectors,
-                  symmetries=[force_paramagnetic],
+
+# Setup RISB solver class
+S = LatticeSolver(
+    h0_k=h0_k,
+    gf_struct=gf_struct,
+    embedding=embedding,
+    update_weights=kweight.update_weights,
+    projectors=projectors,
+    symmetries=[force_paramagnetic],
 )
 
 # Solve
 S.solve(tol=1e-8)
- 
+
 # Average number of particles on a cluster
 total_number_Op = N_op(spin_names, n_orb, off_diag=True)
 total_number = [e.overlap(total_number_Op) for e in embedding]
 
 # Effective total spin of a cluster
 total_spin_Op = S2_op(spin_names, n_orb, off_diag=True)
 total_spin = [e.overlap(total_spin_Op) for e in embedding]
 
 # Print out some interesting observables
-with np.printoptions(formatter={'float': '{: 0.4f}'.format}):
+with np.printoptions(formatter={"float": "{: 0.4f}".format}):
     print("Observables on each cluster:")
     print(f"Quasiaprticle weight Z = \n{S.Z[0]['up']}")
     print(f"Correlation potential Lambda = \n{S.Lambda[0]['up']}")
     print(f"Density matrix rho_qp = \n{S.rho_qp[0]['up']}")
     print(f"Density matrix rho_f = \n{embedding[0].rho_f['up']}")
     print(f"Density matrix rho_c = \n{embedding[0].get_rho_c('up')}")
     print(f"Density matrix rho_cf = \n{embedding[0].rho_cf['up']}")
     print(f"Bath coupling matrix Lambda_c = \n{S.Lambda_c[0]['up']}")
     print(f"Hybridization matrix D = \n{S.D[0]['up']}")
     print(f"Number of partices on cluster N = \n{total_number[0] : 0.4f}")
-    print(f"Effective spin of cluster S = \n{  -0.5 + 0.5 * np.sqrt( 1 + 4*np.array(total_spin[0]) ) : 0.4f}")
+    print(
+        f"Effective spin of cluster S = \n{  -0.5 + 0.5 * np.sqrt( 1 + 4*np.array(total_spin[0]) ) : 0.4f}"
+    )
```

### Comparing `risb-0.1.0/src/risb/helpers.py` & `risb-0.1.1/src/risb/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,195 +11,219 @@
 # GNU General Public License for more details.
 #
 # You may obtain a copy of the License at
 #     https:#www.gnu.org/licenses/gpl-3.0.txt
 #
 # Authors: H. L. Nourse
 
+"""Helper functions to perform rotationally invariant slave-boson mean-field theory self-consistent loop."""
+
+# from scipy.linalg import pinv
+# from scipy.special import binom
+import warnings
 from copy import deepcopy
+
 import numpy as np
-from scipy.linalg import sqrtm
-from scipy.linalg import inv
-#from scipy.linalg import pinv
-#from scipy.special import binom
-import warnings
+from scipy.linalg import inv, sqrtm
 
 ## Formula is (1-A)^{-1/2} = sum_r=0^{infty} (-1)^r * 1/2 choose r * A^r
-#def one_sqrtm_inv(A, tol=np.finfo(float).eps, N=10000):
+# def one_sqrtm_inv(A, tol=np.finfo(float).eps, N=10000):
 #    # Do r = 0 manually (it is just the identity)
 #    A_r = np.eye(A.shape[0])
 #    out = np.eye(A.shape[0])
 #    for r in range(1,N+1):
 #        old = out.copy()
 #        A_r = A_r @ A
 #        out += (-1)**r * binom(-1/2., r) * A_r
 #        err = np.linalg.norm(out - old)
 #        if err < tol:
 #            break
 #    print(r,err)
 #    return out
 #
-#def get_K_sq_inv(pdensity, hdensity, tol=np.finfo(float).eps, N=10000):
+# def get_K_sq_inv(pdensity, hdensity, tol=np.finfo(float).eps, N=10000):
 #    return one_sqrtm_inv(A=pdensity, tol=tol, N=N) @ one_sqrtm_inv(A=hdensity, tol=tol, N=N)
 
-def get_d(rho_qp : np.ndarray, 
-          ke : np.ndarray) -> np.ndarray:
+
+def get_d(rho_qp: np.ndarray, ke: np.ndarray) -> np.ndarray:
     """
+    Return hybridization matrix of impurity problem.
+
+    Assumes the quasiparticle kinetic energy is lopsided as has not been multiplied
+    by R on the left-hand side.
+
     Parameters
     ----------
     rho_qp : numpy.ndarray
         Quasiparticle density matrix obtained from the mean-field.
     ke : numpy.ndarray
         Lopsided quasiparticle kinetic energy.
 
     Returns
     -------
     D : numpy.ndarray
         Hybridization coupling.
-    
+
     Notes
     -----
     Eq. 35 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
+
     """
     K = rho_qp - rho_qp @ rho_qp
     return inv(sqrtm(K)) @ ke.T
 
-def get_d2(rho_qp : np.ndarray, 
-           ke : np.ndarray,
-           R : np.ndarray) -> np.ndarray:
+
+def get_d2(rho_qp: np.ndarray, ke: np.ndarray, R: np.ndarray) -> np.ndarray:
     """
+    Return hybridization matrix of impurity problem.
+
+    This will invert R, so will not work in a Mott insulator when R is singular.
+
     Parameters
     ----------
     rho_qp : numpy.ndarray
         Quasiparticle density matrix obtained from the mean-field.
     ke : numpy.ndarray
-        Lopsided quasiparticle kinetic energy.
+        Quasiparticle kinetic energy.
     R : numpy.ndarray
         Renormalization matrix from electrons to quasiparticles.
 
     Returns
     -------
     D : numpy.ndarray
         Hybridization coupling.
-    
+
     Notes
     -----
     Eq. 35 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
+
+    The singular nature of R might be fixed by using the pseudo-inverse (untested).
+
     """
     K = rho_qp - rho_qp @ rho_qp
     return inv(sqrtm(K)) @ (inv(R) @ ke).T
 
-def get_lambda_c(rho_qp : np.ndarray, 
-                 R : np.ndarray, 
-                 Lambda: np.ndarray, 
-                 D: np.ndarray) -> np.ndarray:
+
+def get_lambda_c(
+    rho_qp: np.ndarray, R: np.ndarray, Lambda: np.ndarray, D: np.ndarray
+) -> np.ndarray:
     """
+    Return bath matrix of impurity problem.
+
     Parameters
     ----------
     rho_qp : numpy.ndarray
         Quasiparticle density matrix obtained from the mean-field.
     R : numpy.ndarray
         Renormalization matrix from electrons to quasiparticles.
     Lambda : numpy.ndarray
         Correlation potential of quasiparticles.
     D : numpy.ndarray
         Hybridization coupling.
 
     Returns
     -------
     Lambda_c : numpy.ndarray
-        Bath coupling.    
-    
+        Bath coupling.
+
     Notes
     -----
     Eq. 36 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
+
     """
     P = np.eye(rho_qp.shape[0]) - 2.0 * rho_qp
     K = rho_qp - rho_qp @ rho_qp
     K_sq = sqrtm(K)
     K_sq_inv = inv(K_sq)
-    return -np.real( (R @ D).T @ K_sq_inv @ P ).T - Lambda
-    #lhs = ((R @ D).T @ K_sq_inv @ P ).T
-    #return - Lambda - 0.5 * (lhs + lhs.conj())
-
-def get_lambda(R : np.ndarray, 
-               D : np.ndarray, 
-               Lambda_c : np.ndarray, 
-               rho_f : np.ndarray) -> np.ndarray:
+    return -np.real((R @ D).T @ K_sq_inv @ P).T - Lambda
+    # lhs = ((R @ D).T @ K_sq_inv @ P ).T
+    # return - Lambda - 0.5 * (lhs + lhs.conj())
+
+
+def get_lambda(
+    R: np.ndarray, D: np.ndarray, Lambda_c: np.ndarray, rho_f: np.ndarray
+) -> np.ndarray:
     """
+    Return correlation potential matrix from impurity problem parameters and density matrices.
+
     Parameters
     ----------
     R : numpy.ndarray
         Renormalization matrix from electrons to quasiparticles.
     D : numpy.ndarray
         Hybridization coupling.
     Lambda_c : numpy.ndarray
         Bath coupling.
     rho_f : numpy.ndarray
         f-electron density matrix from impurity.
 
     Returns
     -------
     Lambda : numpy.ndarray
-        Correlation potential of quasiparticles. 
-    
+        Correlation potential of quasiparticles.
+
     Notes
     -----
-    Derived from Eq. 36 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__ by 
-    replacing the quasipartice density matrix with the f-electron density 
+    Derived from Eq. 36 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__ by
+    replacing the quasipartice density matrix with the f-electron density
     matrix using Eq. 39.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
+
     """
     P = np.eye(rho_f.shape[0]) - 2.0 * rho_f
     K = rho_f - rho_f @ rho_f
     K_sq = sqrtm(K)
     K_sq_inv = inv(K_sq)
-    return -np.real( (R @ D).T @ K_sq_inv @ P ).T - Lambda_c
-    #lhs = ( (R @ D).T @ K_sq_inv @ P ).T
-    #return - Lambda_c - 0.5 * (lhs + lhs.conj())
+    return -np.real((R @ D).T @ K_sq_inv @ P).T - Lambda_c
+    # lhs = ( (R @ D).T @ K_sq_inv @ P ).T
+    # return - Lambda_c - 0.5 * (lhs + lhs.conj())
+
 
-def get_r(rho_cf : np.ndarray, 
-          rho_f : np.ndarray) -> np.ndarray:
+def get_r(rho_cf: np.ndarray, rho_f: np.ndarray) -> np.ndarray:
     """
+    Return renormalization matrix from impurity problem density matrices.
+
     Parameters
     ----------
     rho_cf : numpy.ndarray
         c,f-electron hybridization density matrix from impurity.
     rho_f : numpy.ndarray
         f-electron density matrix from impurity.
 
     Returns
     -------
     R : numpy.ndarray
         Renormalization matrix from electrons to quasiparticles.
-    
+
     Notes
     -----
-    Derived from Eq. 38 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__ by 
-    replacing the quasiparticle density matrix with the f-electron density 
+    Derived from Eq. 38 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__ by
+    replacing the quasiparticle density matrix with the f-electron density
     matrix using Eq. 39.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
+
     """
     K = rho_f - rho_f @ rho_f
     K_sq = sqrtm(K)
     K_sq_inv = inv(K_sq)
     return (rho_cf @ K_sq_inv).T
 
-def get_f1(rho_cf : np.ndarray, 
-           rho_qp : np.ndarray, 
-           R : np.ndarray) -> np.ndarray:
+
+def get_f1(rho_cf: np.ndarray, rho_qp: np.ndarray, R: np.ndarray) -> np.ndarray:
     """
+    Return the first self-consistent equation of RISB.
+
     Parameters
     ----------
     rho_cf : numpy.ndarray
         c,f-electron hybridization density matrix from impurity.
     rho_qp : numpy.ndarray
         Quasiparticle density matrix obtained from the mean-field.
     R : numpy.ndarray
@@ -211,210 +235,233 @@
         First self-consistency equation.
 
     Notes
     -----
     Eq. 38 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
+
     """
     K = rho_qp - rho_qp @ rho_qp
     K_sq = sqrtm(K)
     return rho_cf - R.T @ K_sq
 
-def get_f2(rho_f : np.ndarray, 
-           rho_qp : np.ndarray) -> np.ndarray:
+
+def get_f2(rho_f: np.ndarray, rho_qp: np.ndarray) -> np.ndarray:
     """
+    Return the second self-consistent equation of RISB.
+
     Parameters
     ----------
     rho_f : numpy.ndarray
         f-electron density matrix from impurity.
     rho_qp : numpy.ndarray
         Quasiparticle density matrix obtained from the mean-field.
 
     Returns
     -------
     f2 : numpy.ndarray
         Second self-consistency equation.
-        
+
     Notes
     -----
     Eq. 39 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
+
     """
     return rho_f - rho_qp.T
 
-def get_h_qp(R : np.ndarray, 
-             Lambda : np.ndarray, 
-             h0_kin_k : np.ndarray, 
-             mu : float = 0) -> tuple[ np.ndarray, np.ndarray ]:
-    """
-    Construct the quasiparticle Hamiltonian.
-    
+
+def get_h_qp(
+    R: np.ndarray, Lambda: np.ndarray, h0_kin_k: np.ndarray, mu: float = 0
+) -> tuple[np.ndarray, np.ndarray]:
+    r"""
+    Construct the quasiparticle Hamiltonian :math:`\hat{H}^{\mathrm{qp}}`.
+
     Parameters
     ----------
     R : numpy.ndarray
         Renormalization matrix) from electrons to quasiparticles
     Lambda : numpy.ndarray
         Correlation potential of quasiparticles.
     h0_kin_k : numpy.ndarray
-        Single-particle dispersion between local clusters. Indexed as 
+        Single-particle dispersion between local clusters. Indexed as
         k, orb_i, orb_j
     mu : float, optional
         Chemical potential
 
     Return
     ------
     h_qp : numpy.ndarray
         Indexed as k, orb_i, orb_j
-    
+
     Notes
     -----
     Eq. A34 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
+
     """
-    #h_qp = np.einsum('ac,cdk,db->kab', R, h0_kin_k, R.conj().T, optimize='optimal') + (Lambda - mu*np.eye(Lambda.shape[0]))
-    h_qp = np.einsum('ac,kcd,db->kab', R, h0_kin_k, R.conj().T) + \
-        (Lambda - mu*np.eye(Lambda.shape[0]))
+    # h_qp = np.einsum('ac,cdk,db->kab', R, h0_kin_k, R.conj().T, optimize='optimal') + (Lambda - mu*np.eye(Lambda.shape[0]))
+    h_qp = np.einsum("ac,kcd,db->kab", R, h0_kin_k, R.conj().T) + (
+        Lambda - mu * np.eye(Lambda.shape[0])
+    )
     if not np.allclose(h_qp, np.swapaxes(h_qp, 1, 2).conj()):
-        warnings.warn("H_qp is not Hermitian !", RuntimeWarning)
-    #eig, vec = np.linalg.eigh(h_qp)
-    #return (eig, vec)
+        warnings.warn("H_qp is not Hermitian !", RuntimeWarning, stacklevel=2)
+    # eig, vec = np.linalg.eigh(h_qp)
+    # return (eig, vec)
     return h_qp
 
-def get_h0_kin_k_R(R : np.ndarray, 
-                   h0_kin_k : np.ndarray, 
-                   vec : np.ndarray) -> np.ndarray:
+
+def get_h0_kin_k_R(R: np.ndarray, h0_kin_k: np.ndarray, vec: np.ndarray) -> np.ndarray:
     """
+    Return the matrix representation of the lopsided kinetic energy term in the quasiparticle Hamiltonian of RISB.
+
     Parameters
     ----------
     R : numpy.ndarray
         Rormalization matrix from electrons to quasiparticles.
     h0_kin_k : numpy.ndarray
-        Single-particle dispersion between local clusters. Indexed as 
+        Single-particle dispersion between local clusters. Indexed as
         k, orb_i, orb_j.
     vec : numpy.ndarray
-        Eigenvectors of quasiparticle Hamiltonian. Indexed as k, each column 
+        Eigenvectors of quasiparticle Hamiltonian. Indexed as k, each column
         an eigenvector.
 
     Returns
     -------
     h0_kin_k_R : numpy.ndarray
-        Matrix representation of lopsided quasiparticle Hamiltonian. 
+        Matrix representation of lopsided quasiparticle Hamiltonian.
 
     Notes
     -----
-    This is equivalent to the kinetic part of ``H^qp`` with the inverse of 
+    This is equivalent to the kinetic part of ``H^qp`` with the inverse of
     the renormalization matrix `R` multiplied on the left.
+
     """
-    return np.einsum('kac,cd,kdb->kab', h0_kin_k, R.conj().T, vec)
+    return np.einsum("kac,cd,kdb->kab", h0_kin_k, R.conj().T, vec)
 
-def get_R_h0_kin_k_R(R : np.ndarray, 
-                     h0_kin_k : np.ndarray, 
-                     vec : np.ndarray) -> np.ndarray:
+
+def get_R_h0_kin_k_R(
+    R: np.ndarray, h0_kin_k: np.ndarray, vec: np.ndarray
+) -> np.ndarray:
     """
+    Return the matrix representation of the kinetic energy term in the quasiparticle Hamiltonian of RISB.
+
     Parameters
     ----------
     R : numpy.ndarray
         Renormalization matrix from quasiparticles to electrons.
     h0_kin_k : numpy.ndarray
-        Single-particle dispersion between local clusters. Indexed as 
+        Single-particle dispersion between local clusters. Indexed as
         k, orb_i, orb_j.
     vec : numpy.ndarray
-        Eigenvectors of quasiparticle Hamiltonian. Indexed as k, each column 
+        Eigenvectors of quasiparticle Hamiltonian. Indexed as k, each column
         an eigenvector.
 
     Returns
     -------
     R_h0_kin_k_R : numpy.ndarray
-        Matrix representation of kinetic part of quasiparticle 
+        Matrix representation of kinetic part of quasiparticle
         Hamiltonian ``H^qp``.
-    """
-    return np.einsum('pa,kac,cd,kdb->kpb', R, h0_kin_k, R.conj().T, vec)
 
-#\sum_n \sum_k [A_k P_k]_{an} [D_k]_n  [P_k^+ B_k]_{nb}
-def get_rho_qp(vec : np.ndarray, 
-               kweights : np.ndarray, 
-               P : np.ndarray | None = None) -> np.ndarray:
     """
+    return np.einsum("pa,kac,cd,kdb->kpb", R, h0_kin_k, R.conj().T, vec)
+
+
+# \sum_n \sum_k [A_k P_k]_{an} [D_k]_n  [P_k^+ B_k]_{nb}
+def get_rho_qp(
+    vec: np.ndarray, kweights: np.ndarray, P: np.ndarray | None = None
+) -> np.ndarray:
+    r"""
+    Return the single-particle density matrix of the quasiparticle Hamiltonian :math:`\hat{H}^{\mathrm{qp}}`.
+
     Parameters
     ----------
     vec : numpy.ndarray
         Eigenvectors of quasiparticle Hamiltonian.
     kweights : numpy.ndarray
         Integration weights at each k-point for each band (eigenvector).
     P : numpy.ndarray, optional
         Projection matrix onto correlated subspace.
 
     Returns
     -------
     rho_qp : numpy.ndarray
         Quasiparticle density matrix from mean-field.
-    
+
     Notes
     -----
-    Eqs. 32 and 34 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__, but not in 
-    the natural-basis gauge. See Eq. 112 in the supplemental of 
+    Eqs. 32 and 34 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__, but not in
+    the natural-basis gauge. See Eq. 112 in the supplemental of
     `10.1103/PhysRevLett.118.126401 <PRL126401_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
     .. _PRL126401: https://doi.org/10.1103/PhysRevLett.118.126401
 
     """
     vec_dag = np.swapaxes(vec.conj(), -1, -2)
     if P is None:
-        return np.einsum('kan,kn,knb->ab', vec, kweights, vec_dag).T
-    else:
-        P_dag = np.swapaxes(P.conj(), -2, -1)
-        middle = np.einsum('kan,kn,knb->kab', vec, kweights, vec_dag)
-        return np.sum(P @ middle @ P_dag, axis=0).T
-
-def get_ke(h0_kin_k_R : np.ndarray, 
-           vec : np.ndarray, 
-           kweights : np.ndarray, 
-           P : np.ndarray | None = None) -> np.ndarray:
+        return np.einsum("kan,kn,knb->ab", vec, kweights, vec_dag).T
+    P_dag = np.swapaxes(P.conj(), -2, -1)
+    middle = np.einsum("kan,kn,knb->kab", vec, kweights, vec_dag)
+    return np.sum(P @ middle @ P_dag, axis=0).T
+
+
+def get_ke(
+    h0_kin_k_R: np.ndarray,
+    vec: np.ndarray,
+    kweights: np.ndarray,
+    P: np.ndarray | None = None,
+) -> np.ndarray:
     """
+    Return average lopsided kinetic energy matrix of the quasiparticle Hamiltonian in RISB.
+
     Parameters
     ----------
     h0_kin_k_R : numpy.ndarray
-        Single-particle dispersion between local clusters with `R` matrix 
+        Single-particle dispersion between local clusters with `R` matrix
         multiplied on the right.
     vec : numpy.ndarray
         Eigenvectors of quasiparticle Hamiltonian.
     kweights : numpy.ndarray
         Integration weights at each k-point for each band (eigenvector).
     P : numpy.ndarray, optional
         Projection matrix onto correlated subspace.
 
     Returns
     -------
     ke : numpy.ndarray
         Lopsided quasiparticle kinetic energy from the mean-field.
-    
+
     Notes
     -----
     Eq. 35 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
 
     """
     vec_dag = np.swapaxes(vec.conj(), -1, -2)
     if P is None:
-        return np.einsum('kan,kn,knb->ab', h0_kin_k_R, kweights, vec_dag)
-    else:
-        P_dag = np.swapaxes(P.conj(), -2, -1)
-        middle = np.einsum('kan,kn,knb->kab', h0_kin_k_R, kweights, vec_dag)
-        return np.sum(P @ middle @ P_dag, axis=0)
-
-def get_ke2(R_h0_kin_k_R : np.ndarray, 
-            vec : np.ndarray, 
-            kweights : np.ndarray, 
-            P : np.ndarray | None = None) -> np.ndarray:
+        return np.einsum("kan,kn,knb->ab", h0_kin_k_R, kweights, vec_dag)
+    P_dag = np.swapaxes(P.conj(), -2, -1)
+    middle = np.einsum("kan,kn,knb->kab", h0_kin_k_R, kweights, vec_dag)
+    return np.sum(P @ middle @ P_dag, axis=0)
+
+
+def get_ke2(
+    R_h0_kin_k_R: np.ndarray,
+    vec: np.ndarray,
+    kweights: np.ndarray,
+    P: np.ndarray | None = None,
+) -> np.ndarray:
     """
+    Return average kinetic energy matrix of the quasiparticle Hamiltonian in RISB.
+
     Parameters
     ----------
     R_h0_kin_k_R : numpy.ndarray
         Kinetic part of quasiparticle Hamiltonain.
     vec : numpy.ndarray
         Eigenvectors of quasiparticle Hamiltonian.
     kweights : numpy.ndarray
@@ -422,127 +469,149 @@
     P : numpy.ndarray, optional
         Projection matrix onto correlated subspace.
 
     Returns
     -------
     ke : numpy.ndarray
         Quasiparticle kinetic energy from the mean-field.
-    
+
     Notes
     -----
     Eq. 35 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
 
     """
     vec_dag = np.swapaxes(vec.conj(), -1, -2)
     if P is None:
-        return np.einsum('kan,kn,knb->ab', R_h0_kin_k_R, kweights, vec_dag)
-    else:
-        P_dag = np.swapaxes(P.conj(), -2, -1)
-        middle = np.einsum('kan,kn,knb->kab', R_h0_kin_k_R, kweights, vec_dag)
-        return np.sum(P @ middle @ P_dag, axis=0)
-
-# FIXME this does not have to be a numpy array, it could
-# be a ragged list of lists if each block has a different size
-# So should not use shape
-def block_to_full(A : np.ndarray) -> np.ndarray:
+        return np.einsum("kan,kn,knb->ab", R_h0_kin_k_R, kweights, vec_dag)
+    P_dag = np.swapaxes(P.conj(), -2, -1)
+    middle = np.einsum("kan,kn,knb->kab", R_h0_kin_k_R, kweights, vec_dag)
+    return np.sum(P @ middle @ P_dag, axis=0)
+
+
+def block_to_full(A: np.ndarray) -> np.ndarray:
     """
+    Return a full block matrix from each block.
+
     Parameters
     ----------
     A : numpy.ndarray
         A block matrix indexed as ``A[...,block1,block2,orb1,orb2]``.
 
     Returns
     -------
     numpy.ndarray
         Matrix `A` of shape ``A[...,block * orb, block * orb]``.
+
+    Notes
+    -----
+    FIXME this does not have to be a numpy array, it could be a ragged list of lists if each block has a different size.
+    So we should not use shape and handle the ragged list differently.
+
     """
     if len(A.shape) < 4:
-        raise ValueError(f'A.shape = {A.shape} must have at least ...,block,block,orb,orb structure !')
+        msg = f"A.shape = {A.shape} must have at least ...,block,block,orb,orb structure !"
+        raise ValueError(msg)
     na = A.shape[-4]
     nb = A.shape[-3]
     if na != nb:
-        raise ValueError(f'Should be same number of blocks in i and j dimesnions, but got {na} and {nb} !')
-    return np.block( [ [A[...,i,j,:,:] for j in range(na)] for i in range(na) ] )
+        msg = f"Should be same number of blocks in i and j dimesnions, but got {na} and {nb} !"
+        raise ValueError(msg)
+    return np.block([[A[..., i, j, :, :] for j in range(na)] for i in range(na)])
+
 
-def get_h0_loc_matrix(h0_k : np.ndarray, 
-                      P : np.ndarray | None = None) -> np.ndarray:
+def get_h0_loc_matrix(h0_k: np.ndarray, P: np.ndarray | None = None) -> np.ndarray:
     """
+    Return a matrix representation of the local terms in a non-interacting dispersion.
+
+    If a projector :attr:`P` onto a local subspace is given the local terms are only in that subspace.
+
     Parameters
     ----------
     h0_k : numpy.ndarray
         Single-particle dispersion.
     P : numpy.ndarray | None, optional
         The projector onto a local cluster within the supercell.
 
     Returns
     -------
     numpy.ndarray
-        The matrix of single-particle hopping/energies on a cluster defined by 
+        The matrix of single-particle hopping/energies on a cluster defined by
         the projector.
+
     """
     n_k = h0_k.shape[0]
     if P is None:
         return np.sum(h0_k, axis=0) / float(n_k)
-    else:
-        return np.sum(P @ h0_k @ P.conj().T, axis=0) / float(n_k)
+    return np.sum(P @ h0_k @ P.conj().T, axis=0) / float(n_k)
+
 
-def get_h0_kin_k_mat(h0_k : np.ndarray, 
-                     P : np.ndarray) -> np.ndarray:
+def get_h0_kin_k_mat(h0_k: np.ndarray, P: np.ndarray) -> np.ndarray:
     """
+    Return a matrix representation of the kinetic terms between clusters/local subspaces of a non-interacting dispersion.
+
+    This function only subtracts off the local terms in a single subspace given by :attr:`P`.
+
     Parameters
     ----------
     h0_k : numpy.ndarray
         Single-particle dispersion.
     P : numpy.ndarray
         The projector onto a local cluster within the supercell.
+
     Returns
     -------
     numpy.ndarray
-        The single-particle hopping without the contribution from the cluster 
+        The single-particle hopping without the contribution from the cluster
         defined by the projector.
+
     """
     h0_loc_matrix = get_h0_loc_matrix(h0_k, P)
     return h0_k - P.conj().T @ h0_loc_matrix @ P
 
-def get_h0_kin_k(h0_k : dict[np.ndarray], 
-                 projectors : list[dict[np.ndarray]] | None = None, 
-                 gf_struct_mapping : list[dict[str,str]] | None = None) -> dict[np.ndarray]:
+
+def get_h0_kin_k(
+    h0_k: dict[np.ndarray],
+    projectors: list[dict[np.ndarray]] | None = None,
+    gf_struct_mapping: list[dict[str, str]] | None = None,
+) -> dict[np.ndarray]:
     """
+    Return a matrix representation of only the kinetic terms between clusters/local subspaces of a non-interacting dispersion.
+
     Parameters
     ----------
     h0_k : dict[numpy.ndarray]
         Single-particle dispersion in each block.
     projectors : list[dict[numpy.ndarray]] | None, optional
-        The projectors onto each subspace of a local cluster within 
+        The projectors onto each subspace of a local cluster within
         the supercell organized into single-particle symmetry blocks.
     gf_struct_mapping : list[dict[str, str]] | None, optional
-        The mapping from the symmetry blocks in the subspace to the 
+        The mapping from the symmetry blocks in the subspace to the
         symmetry blocks of h0_k. Default assumes the keys in `projectors`
         are the same as the keys in `h0_k`.
 
     Returns
     -------
     dict[numpy.ndarray]
-        The single-particle hopping with only the kinetic contribution, 
-        without the single-particle terms from the clusters defined by 
+        The single-particle hopping with only the kinetic contribution,
+        without the single-particle terms from the clusters defined by
         the projectors.
+
     """
     h0_kin_k = deepcopy(h0_k)
-    
+
     if projectors is not None:
         n_clusters = len(projectors)
         if gf_struct_mapping is None:
-            gf_struct_mapping = [{bl:bl for bl in h0_k.keys()} for i in range(n_clusters)]
+            gf_struct_mapping = [{bl: bl for bl in h0_k} for i in range(n_clusters)]
         for i, P in enumerate(projectors):
-            for bl in P.keys():
+            for bl in P:
                 bl_full = gf_struct_mapping[i][bl]
                 h0_loc_matrix = get_h0_loc_matrix(h0_k[bl_full], P[bl])
                 h0_kin_k[bl_full] -= P[bl].conj().T @ h0_loc_matrix @ P[bl]
-                #h0_kin_k[bl_full] = get_h0_kin_k_mat(h0_kin_k[bl_full], P[bl])
+                # h0_kin_k[bl_full] = get_h0_kin_k_mat(h0_kin_k[bl_full], P[bl])
     else:
-        for bl in h0_k.keys():
+        for bl in h0_k:
             h0_kin_k[bl] -= get_h0_loc_matrix(h0_k[bl])
 
     return h0_kin_k
-
```

### Comparing `risb-0.1.0/src/risb/helpers_triqs.py` & `risb-0.1.1/src/risb/helpers_triqs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-# Copyright (c) 2023 H. L. Nourse
+# Copyright (c) 2016-2024 H. L. Nourse
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,424 +11,518 @@
 # GNU General Public License for more details.
 #
 # You may obtain a copy of the License at
 #     https:#www.gnu.org/licenses/gpl-3.0.txt
 #
 # Authors: H. L. Nourse
 
+"""Functions used in RISB based on the TRIQS library."""
+
 import numpy as np
+from triqs.gf import BlockGf, MeshImFreq, MeshProduct, MeshReFreq, inverse
 from triqs.operators import Operator, c, c_dag
-from triqs.gf import BlockGf, inverse, MeshProduct, MeshReFreq, MeshImFreq
+
 from risb.helpers import get_h0_loc_matrix, get_h_qp
 
-def get_C_Op(gf_struct : list[tuple[str,int]], dagger : bool = False) -> dict[list[Operator]]:
+
+def get_C_Op(
+    gf_struct: list[tuple[str, int]], dagger: bool = False
+) -> dict[list[Operator]]:
     """
+    Return all creation operators in Hilbert space.
+
     Parameters
     ----------
     gf_struct : list of pairs [ (str,int), ...]
         Structure of the matrices. It must be a
         list of pairs, each containing the name of the
         matrix block as a string and the size of that block.
         For example: ``[ ('up', 3), ('down', 3) ]``.
     dagger : bool
         Whether to return the creation operator or not.
 
     Returns
     -------
     dict[list[triqs.operators.Operator]]
-        For each block in `gf_struct`, a vector of all creation/annihilation 
+        For each block in `gf_struct`, a vector of all creation/annihilation
         operators in its subspace.
+
     """
-    C_Op = dict()
+    C_Op = {}
     for bl, bl_size in gf_struct:
         if dagger:
             C_Op[bl] = [c_dag(bl, o) for o in range(bl_size)]
         else:
             C_Op[bl] = [c(bl, o) for o in range(bl_size)]
     return C_Op
 
-def matrix_to_Op(A : dict[np.ndarray], gf_struct : list[tuple[str,int]]) -> dict[Operator]:
+
+def matrix_to_Op(
+    A: dict[np.ndarray], gf_struct: list[tuple[str, int]]
+) -> dict[Operator]:
     """
+    Return a TRIQS operator from a matrix representation of quadratic operators.
+
     Parameters
     ----------
     A : dict[numpy.ndarray]
         Single-particle matrix, where each key is a different block.
     gf_struct : list of pairs [ (str,int), ...]
         Structure of the matrices. It must be a
         list of pairs, each containing the name of the
         matrix block as a string and the size of that block.
         For example: ``[ ('up', 3), ('down', 3) ]``.
 
     Returns
     -------
     dict[triqs.operators.Operator]
         The single-particle matrix as a quadratic TRIQS operator.
+
     """
     C_dag_Op = get_C_Op(gf_struct=gf_struct, dagger=True)
     C_Op = get_C_Op(gf_struct=gf_struct, dagger=False)
-    Op = dict()
+    Op = {}
     for bl in A:
         Op[bl] = C_dag_Op[bl] @ A[bl] @ C_Op[bl]
     return Op
 
-def get_h0_loc_blocks(h0_k : dict[np.ndarray], 
-                      P : dict[np.ndarray], 
-                      gf_struct : list[tuple[str,int]] | None = None, 
-                      gf_struct_mapping : dict[str,str] | None = None, 
-                      force_real: bool = True) -> dict[Operator]:
+
+def get_h0_loc_blocks(
+    h0_k: dict[np.ndarray],
+    P: dict[np.ndarray],
+    gf_struct: list[tuple[str, int]] | None = None,
+    gf_struct_mapping: dict[str, str] | None = None,
+    force_real: bool = True,
+) -> dict[Operator]:
     """
+    Return a TRIQS operator of the non-interacting terms in the subspace given by :attr:`P`.
+
+    This function splits the terms into the symmetry blocks given by :attr:`gf_struct`.
+
     Parameters
     ----------
     h0_k : dict[numpy.ndarray]
         Single-particle dispersion in each block.
     P : dict[numpy.ndarray]
         The projector onto a local cluster within the supercell.
     gf_struct : list of pairs [ (str,int), ...] | None, optional
         Structure of the matrices. It must be a
         list of pairs, each containing the name of the
         matrix block as a string and the size of that block.
-        For example: ``[ ('up', 3), ('down', 3) ]``. Default is 
+        For example: ``[ ('up', 3), ('down', 3) ]``. Default is
         structure worked out from the projector P.
     gf_struct_mapping : dict[str, str] | None, optional
-        The mapping from the symmetry blocks in the subspace of P to the 
+        The mapping from the symmetry blocks in the subspace of P to the
         symmetry blocks of h0_k. Default assumes the keys in `P`
         are the same as the keys in `h0_k`.
     force_real : bool
         Whether to make the resulting matrix real or not.
 
     Returns
     -------
     dict[triqs.operators.Operator]
-        For each single-particle symmetry block the non-interacting 
+        For each single-particle symmetry block the non-interacting
         terms in the cluster defined by the projector `P`.
+
     """
     if gf_struct is None:
         gf_struct = [(k, v.shape[-2]) for k, v in P.items()]
     if gf_struct_mapping is None:
-        gf_struct_mapping = {bl:bl for bl in h0_k.keys()}
-    
-    h0_loc_matrix = dict()
-    for bl_sub in P.keys(): # sub = subspace of full space defined by h0_k
+        gf_struct_mapping = {bl: bl for bl in h0_k}
+
+    h0_loc_matrix = {}
+    for bl_sub in P:  # sub = subspace of full space defined by h0_k
         bl = gf_struct_mapping[bl_sub]
         if force_real:
             h0_loc_matrix[bl_sub] = get_h0_loc_matrix(h0_k[bl], P[bl_sub]).real
         else:
             h0_loc_matrix[bl_sub] = get_h0_loc_matrix(h0_k[bl], P[bl_sub])
 
     return matrix_to_Op(A=h0_loc_matrix, gf_struct=gf_struct)
 
-def get_h0_loc(h0_k : dict[np.ndarray], 
-               P : dict[np.ndarray], 
-               gf_struct : list[tuple[str,int]] | None = None, 
-               gf_struct_mapping : dict[str,str] | None = None, 
-               force_real : bool = True) -> Operator:
+
+def get_h0_loc(
+    h0_k: dict[np.ndarray],
+    P: dict[np.ndarray],
+    gf_struct: list[tuple[str, int]] | None = None,
+    gf_struct_mapping: dict[str, str] | None = None,
+    force_real: bool = True,
+) -> Operator:
     """
+    Return a TRIQS operator of the non-interacting terms in the subspace given by :attr:`P`.
+
     Parameters
     ----------
     h0_k : dict[numpy.ndarray]
         Single-particle dispersion in each block.
     P : dict[numpy.ndarray]
         The projector onto a local cluster within the supercell.
     gf_struct : list of pairs [ (str,int), ...] | None, optional
         Structure of the matrices. It must be a
         list of pairs, each containing the name of the
         matrix block as a string and the size of that block.
-        For example: ``[ ('up', 3), ('down', 3) ]``. Default is 
+        For example: ``[ ('up', 3), ('down', 3) ]``. Default is
         structure worked out from the projector P.
     gf_struct_mapping : dict[str, str] | None, optional
-        The mapping from the symmetry blocks in the subspace of P to the 
+        The mapping from the symmetry blocks in the subspace of P to the
         symmetry blocks of h0_k. Default assumes the keys in `P`
         are the same as the keys in `h0_k`.
     force_real : bool
         Whether to make the resulting matrix real or not.
 
     Returns
     -------
     triqs.operators.Operator
         Non-interacting terms in the cluster defined by the projector `P`.
+
     """
-    h0_loc_blocks = get_h0_loc_blocks(h0_k=h0_k, P=P, gf_struct=gf_struct, gf_struct_mapping=gf_struct_mapping, force_real=force_real)
+    h0_loc_blocks = get_h0_loc_blocks(
+        h0_k=h0_k,
+        P=P,
+        gf_struct=gf_struct,
+        gf_struct_mapping=gf_struct_mapping,
+        force_real=force_real,
+    )
     h0_loc = Operator()
     for Op in h0_loc_blocks.values():
         h0_loc += Op
     return h0_loc
 
-def get_gf_struct_from_g(block_gf : BlockGf) -> list[tuple[str,int]]:
+
+def get_gf_struct_from_g(block_gf: BlockGf) -> list[tuple[str, int]]:
     """
+    Return the block structure of a TRIQS Green's function.
+
     Parameters
     ----------
     block_gf : triqs.gf.BlockGf
         Block Green's function.
 
     Returns
     -------
     list[tuple[str,int]]
         Green's function's structure.
+
     """
     gf_struct = []
     for bl, gf in block_gf:
-        gf_struct.append( [bl, gf.data.shape[-1]] )
+        gf_struct.append([bl, gf.data.shape[-1]])
     return gf_struct
 
-# FIXME have to check h0_k shares the same mesh as Gf 
-def get_g0_k_w(gf_struct : list[tuple[str,int]],
-               mesh : MeshProduct,
-               h0_k : dict[np.ndarray] | None = None,
-               h0_k_gf = None,
-               mu : float = 0,
-               use_broadcasting : bool = True) -> BlockGf:
+
+# FIXME have to check h0_k shares the same mesh as Gf
+def get_g0_k_w(
+    gf_struct: list[tuple[str, int]],
+    mesh: MeshProduct,
+    h0_k: dict[np.ndarray] | None = None,
+    h0_k_gf=None,
+    mu: float = 0,
+    use_broadcasting: bool = True,
+) -> BlockGf:
     """
+    Return a TRIQS non-interacting lattice Green's function.
+
     Parameters
     ----------
     gf_struct : list of pairs [ (str,int), ...]
         Structure of the matrices. It must be a
         list of pairs, each containing the name of the
         matrix block as a string and the size of that block.
         For example: ``[ ('up', 3), ('down', 3) ]``.
     mesh : triqs.gf.MeshProduct
         A meshproduct where first index is a triqs.gf.MeshBrZone mesh and
-        the second index is a triqs.gf.MeshReFreq or triqs.gf.MeshImFreq 
+        the second index is a triqs.gf.MeshReFreq or triqs.gf.MeshImFreq
         mesh. MeshProduct is a fancy list.
     h0_k : dict[numpy.ndarray], optional
-        Non-interacting dispersion indexed as k, orb_i, orb_j. 
+        Non-interacting dispersion indexed as k, orb_i, orb_j.
         Each key in dictionary must follow :attr:`gf_struct`.
     h0_k : triqs.gf.BlockGf
         Non-interacting dispersion as a triqs.gf.BlockGf.
-        Must follow the structure given by :attr:`gf_struct`, on 
+        Must follow the structure given by :attr:`gf_struct`, on
         the mesh given by :attr:`mesh`.
     mu : float, optional
         Chemical potential.
     use_broadcasting : bool, optional
-        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray 
-        data structure, or to use iterators over for loops and lazy 
+        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray
+        data structure, or to use iterators over for loops and lazy
         expressions from TRIQS.
 
     Returns
     -------
     triqs.gf.BlockGf
         Non-interacting Green's function from a non-interacting dispersion
         relation :attr:`h0_k`.
+
     """
     g0_k_w = BlockGf(mesh=mesh, gf_struct=gf_struct)
     for bl, gf in g0_k_w:
-        identity = np.eye(*gf.data.shape[-2::]) # Last two indices are the orbital structure
+        identity = np.eye(
+            *gf.data.shape[-2::]
+        )  # Last two indices are the orbital structure
         if use_broadcasting:
             w = np.fromiter(gf.mesh[1].values(), dtype=complex)
             if h0_k is not None:
-                #gf.data[...] = np.linalg.inv( ((w + mu)[:,None,None] * identity[None,:])[None,:,...] - h0_k[bl][:,None,...] )
-                gf.data[...] = ((w + mu)[:,None,None] * identity[None,:])[None,:,...] - h0_k[bl][:,None,...]
+                # gf.data[...] = np.linalg.inv( ((w + mu)[:,None,None] * identity[None,:])[None,:,...] - h0_k[bl][:,None,...] )
+                gf.data[...] = ((w + mu)[:, None, None] * identity[None, :])[
+                    None, :, ...
+                ] - h0_k[bl][:, None, ...]
                 gf.invert()
             elif h0_k_gf is not None:
-                gf.data[...] = ((w + mu)[:,None,None] * identity[None,:])[None,:,...] - h0_k_gf[bl].data[:,None,...]
+                gf.data[...] = ((w + mu)[:, None, None] * identity[None, :])[
+                    None, :, ...
+                ] - h0_k_gf[bl].data[:, None, ...]
                 gf.invert()
             else:
-                msg = 'Require a kwarg of h0_k or h0_k_gf !'
+                msg = "Require a kwarg of h0_k or h0_k_gf !"
                 raise ValueError(msg)
         else:
             if h0_k is not None:
                 for k, w in gf.mesh:
-                    gf[k,w] = inverse(w + mu - h0_k[bl][k.data_index])
+                    gf[k, w] = inverse(w + mu - h0_k[bl][k.data_index])
             elif h0_k_gf is not None:
                 for k, w in gf.mesh:
-                    gf[k,w] = inverse(w + mu - h0_k_gf[bl][k])
+                    gf[k, w] = inverse(w + mu - h0_k_gf[bl][k])
             else:
-                msg = 'Require a kwarg of h0_k or h0_k_gf !'
+                msg = "Require a kwarg of h0_k or h0_k_gf !"
                 raise ValueError(msg)
     return g0_k_w
 
-def get_sigma_w(gf_struct : list[tuple[str,int]],
-                mesh : MeshReFreq | MeshImFreq, 
-                Lambda : dict[np.ndarray], 
-                R : dict[np.ndarray], 
-                mu : float = 0, 
-                h0_loc : dict[np.ndarray] | None = None,
-                use_broadcasting : bool = True) -> BlockGf:
-    """
+
+def get_sigma_w(
+    gf_struct: list[tuple[str, int]],
+    mesh: MeshReFreq | MeshImFreq,
+    Lambda: dict[np.ndarray],
+    R: dict[np.ndarray],
+    mu: float = 0,
+    h0_loc: dict[np.ndarray] | None = None,
+    use_broadcasting: bool = True,
+) -> BlockGf:
+    r"""
+    Return a TRIQS local self-energy from RISB.
+
     Parameters
     ----------
     gf_struct : list of pairs [ (str,int), ...]
         Structure of the matrices. It must be a
         list of pairs, each containing the name of the
         matrix block as a string and the size of that block.
         For example: ``[ ('up', 3), ('down', 3) ]``.
     mesh : triqs.gf.meshes.MeshReFreq | triqs.gf.meshes.MeshImFreq
         Frequency mesh of the returned self-energy.
     Lambda : dict[numpy.ndarray]
         Correlation potential of quasiparticles.
         Each key in dictionary must follow :attr:`gf_struct`.
     R : dict[numpy.ndarray]
-        Rormalization matrix from electrons to quasiparticles. 
+        Rormalization matrix from electrons to quasiparticles.
         Each key in dictionary must follow :attr:`gf_struct`.
     mu : float, optional
         Chemical potential.
     h0_loc : dict[numpy.ndarray], optional
         Matrix of non-interacting hopping terms in each local subspace.
         Each key in dictionary must follow :attr:`gf_struct`.
     use_broadcasting : bool, optional
-        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray 
-        data structure, or to use iterators over for loops and lazy 
+        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray
+        data structure, or to use iterators over for loops and lazy
         expressions from TRIQS.
 
     Returns
     -------
     triqs.gf.BlockGf
         RISB local self-energy :math:`\Sigma(\omega)`.
+
     """
     sigma_w = BlockGf(mesh=mesh, gf_struct=gf_struct)
     for bl, gf in sigma_w:
-        identity = np.eye(*gf.data.shape[-2::]) # Last two indices are the orbital structure
+        identity = np.eye(
+            *gf.data.shape[-2::]
+        )  # Last two indices are the orbital structure
         Z_inv = np.linalg.inv(R[bl] @ R[bl].conj().T)
         hf = np.linalg.inv(R[bl]) @ Lambda[bl] @ np.linalg.inv(R[bl].conj().T)
         if use_broadcasting:
             w = np.fromiter(gf.mesh.values(), dtype=complex)
             if h0_loc is not None:
-                gf.data[...] = (identity - Z_inv) * w[:,None,None] + hf + (identity - Z_inv) * mu - h0_loc[bl]
+                gf.data[...] = (
+                    (identity - Z_inv) * w[:, None, None]
+                    + hf
+                    + (identity - Z_inv) * mu
+                    - h0_loc[bl]
+                )
             else:
-                gf.data[...] = (identity - Z_inv) * w[:,None,None] + hf + (identity - Z_inv) * mu
+                gf.data[...] = (
+                    (identity - Z_inv) * w[:, None, None] + hf + (identity - Z_inv) * mu
+                )
         else:
             if h0_loc is not None:
                 for w in gf.mesh:
-                    gf[w] = (identity - Z_inv) * w + hf + (identity - Z_inv) * mu - h0_loc[bl]
+                    gf[w] = (
+                        (identity - Z_inv) * w
+                        + hf
+                        + (identity - Z_inv) * mu
+                        - h0_loc[bl]
+                    )
             else:
                 for w in gf.mesh:
                     gf[w] = (identity - Z_inv) * w + hf + (identity - Z_inv) * mu
     return sigma_w
 
-# FIXME have to check h0_kin_k shares the same mesh 
+
+# FIXME have to check h0_kin_k shares the same mesh
 # FIXME allow h0_kin_k_gf structure as well?
-def get_g_qp_k_w(gf_struct : list[tuple[str,int]],
-                 mesh : MeshProduct,
-                 h0_kin_k : dict[np.ndarray],
-                 Lambda : dict[np.ndarray], 
-                 R : dict[np.ndarray], 
-                 mu : float = 0,
-                 use_broadcasting : bool = True) -> BlockGf:
-    """
+def get_g_qp_k_w(
+    gf_struct: list[tuple[str, int]],
+    mesh: MeshProduct,
+    h0_kin_k: dict[np.ndarray],
+    Lambda: dict[np.ndarray],
+    R: dict[np.ndarray],
+    mu: float = 0,
+    use_broadcasting: bool = True,
+) -> BlockGf:
+    r"""
+    Return a TRIQS lattice RISB quasiparticle Green's function.
+
     Parameters
     ----------
     gf_struct : list of pairs [ (str,int), ...]
         Structure of the matrices. It must be a
         list of pairs, each containing the name of the
         matrix block as a string and the size of that block.
         For example: ``[ ('up', 3), ('down', 3) ]``.
     mesh : triqs.gf.MeshProduct
         A meshproduct where first index is a triqs.gf.MeshBrZone mesh and
-        the second index is a triqs.gf.MeshReFreq or triqs.gf.MeshImFreq 
+        the second index is a triqs.gf.MeshReFreq or triqs.gf.MeshImFreq
         mesh. MeshProduct is a fancy list.
     h0_kin_k : dict[numpy.ndarray]
-        Single-particle dispersion between local clusters. Indexed as 
+        Single-particle dispersion between local clusters. Indexed as
         k, orb_i, orb_j. Each key in dictionary must follow :attr:`gf_struct`.
     Lambda : dict[numpy.ndarray]
         Correlation potential of quasiparticles.
         Each key in dictionary must follow :attr:`gf_struct`.
     R : dict[numpy.ndarray]
-        Rormalization matrix from electrons to quasiparticles. 
+        Rormalization matrix from electrons to quasiparticles.
         Each key in dictionary must follow :attr:`gf_struct`.
     mu : float, optional
         Chemical potential.
     use_broadcasting : bool, optional
-        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray 
-        data structure, or to use iterators over for loops and lazy 
+        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray
+        data structure, or to use iterators over for loops and lazy
         expressions from TRIQS.
 
     Returns
     -------
     triqs.gf.BlockGf
         Quasiparticle Green's function :math:`G^{\mathrm{qp}}(k,\omega)`.
+
     """
     g_qp_k_w = BlockGf(mesh=mesh, gf_struct=gf_struct)
     for bl, gf in g_qp_k_w:
-        identity = np.eye(*gf.data.shape[-2::]) # Last two indices are the orbital structure
+        identity = np.eye(
+            *gf.data.shape[-2::]
+        )  # Last two indices are the orbital structure
         h_qp = get_h_qp(R=R[bl], Lambda=Lambda[bl], h0_kin_k=h0_kin_k[bl], mu=mu)
         if use_broadcasting:
             w = np.fromiter(gf.mesh[1].values(), dtype=complex)
-            #gf.data[...] = inverse( (w[:,None,None] * identity[None,:])[None,:,...] - h_qp[:,None,...] )
-            gf.data[...] = (w[:,None,None] * identity[None,:])[None,:,...] - h_qp[:,None,...]
+            # gf.data[...] = inverse( (w[:,None,None] * identity[None,:])[None,:,...] - h_qp[:,None,...] )
+            gf.data[...] = (w[:, None, None] * identity[None, :])[None, :, ...] - h_qp[
+                :, None, ...
+            ]
             gf.invert()
         else:
             for k, w in g_qp_k_w.mesh:
-                gf[k,w] = inverse(w - h_qp[k.data_index])
+                gf[k, w] = inverse(w - h_qp[k.data_index])
     return g_qp_k_w
 
-def get_g_k_w(g0_k_w : BlockGf | None = None,
-              sigma_w : BlockGf | None = None,
-              g_qp_k_w : BlockGf | None = None,
-              R : dict[np.ndarray] | None = None,
-              use_broadcasting : bool = True) -> BlockGf:
-    """
+
+def get_g_k_w(
+    g0_k_w: BlockGf | None = None,
+    sigma_w: BlockGf | None = None,
+    g_qp_k_w: BlockGf | None = None,
+    R: dict[np.ndarray] | None = None,
+    use_broadcasting: bool = True,
+) -> BlockGf:
+    r"""
+    Return a TRIQS lattice interacting Green's function, with a local self-energy.
+
+    Must pass g0_k_w and sigma_w, or g_qp_k_w and R. Passing g_qp_k_w and R is specific
+    to RISB. Passing g0_k_w and sigma_w is valid for any interacting theory with a local
+    self-energy (it is just Dyson's equation at each k-point).
+
     Parameters
     ----------
     g0_k_w : triqs.gf.BlockGf, optional
         Non-interacting Green's function on a meshproduct where
         the first index is a triqs.gf.MeshBrZone mesh and
         the second index is a triqs.gf.MeshReFreq or triqs.gf.MeshImFreq mesh.
     sigma_w : triqs.gf.BlockGf, optional
         Local self-energy on a triqs.gf.MeshReFreq or triqs.gf.MeshImFreq mesh.
     gp_k_w : triqs.gf.BlockGf, optional
         Quasiparticle Green's function on a meshproduct where
         the first index is a triqs.gf.MeshBrZone mesh and
         the second index is a triqs.gf.MeshReFreq or triqs.gf.MeshImFreq mesh.
     R : dict[numpy.ndarray], optional
-        Rormalization matrix from electrons to quasiparticles. 
-        Each key in dictionary must follow the gf_struct in 
+        Rormalization matrix from electrons to quasiparticles.
+        Each key in dictionary must follow the gf_struct in
         :attr:`g0_k_w` and :attr:`sigma_w`.
     use_broadcasting : bool, optional
-        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray 
-        data structure, or to use iterators over for loops and lazy 
+        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray
+        data structure, or to use iterators over for loops and lazy
         expressions from TRIQS.
 
     Returns
     -------
     triqs.gf.BlockGf
         Physical c-electrons Green's function :math:`G(k,\omega)`.
+
     """
     if (g0_k_w is not None) and (sigma_w is not None):
         g_k_w = g0_k_w.copy()
         g_k_w.zero()
         for bl, gf in g_k_w:
             if use_broadcasting:
-                gf.data[...] = inverse(g0_k_w[bl]).data - sigma_w[bl].data[None,...]
+                gf.data[...] = inverse(g0_k_w[bl]).data - sigma_w[bl].data[None, ...]
                 gf.invert()
             else:
                 for k, w in gf.mesh:
-                    gf[k,w] = inverse(inverse(g0_k_w[bl][k,w]) - sigma_w[bl][w])
+                    gf[k, w] = inverse(inverse(g0_k_w[bl][k, w]) - sigma_w[bl][w])
     elif (g_qp_k_w is not None) and (R is not None):
         g_k_w = g_qp_k_w.copy()
         g_k_w.zero()
         for bl, gf in g_qp_k_w:
             g_k_w[bl] = R[bl].conj().T @ gf @ R[bl]
     else:
-        msg = 'Required kwargs are one of the pairs g0_k_w and sigma_w, or g_qp_k_w and R !'
+        msg = "Required kwargs are one of the pairs g0_k_w and sigma_w, or g_qp_k_w and R !"
         raise ValueError(msg)
     return g_k_w
 
-def get_g_w_loc(g_k_w : BlockGf,
-                use_broadcasting : bool = True) -> BlockGf:
+
+def get_g_w_loc(g_k_w: BlockGf, use_broadcasting: bool = True) -> BlockGf:
     """
+    Return a TRIQS local Green's function from a lattice Green's function.
+
     Parameters
     ----------
     g_k_w : triqs.gf.BlockGf
         A Green's function on a meshproduct where
         the first index is a triqs.gf.MeshBrZone mesh and
         the second index is a triqs.gf.MeshReFreq or triqs.gf.MeshImFreq mesh.
     use_broadcasting : bool, optional
-        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray 
-        data structure, or to use iterators over for loops and lazy 
+        Whether to treat triqs.gf.Gf with its underlying numpy.ndarray
+        data structure, or to use iterators over for loops and lazy
         expressions from TRIQS.
 
     Returns
     -------
     triqs.gf.BlockGf
         k-integrated Green's function on a triqs.gf.MeshReFreq or triqs.gf.MeshImFreq mesh.
+
     """
     k_mesh = g_k_w.mesh[0]
     w_mesh = g_k_w.mesh[1]
     gf_struct = get_gf_struct_from_g(g_k_w)
     g_w_loc = BlockGf(mesh=w_mesh, gf_struct=gf_struct)
-    for bl, gf in g_w_loc:
+    for bl, gf in g_k_w:
         if use_broadcasting:
-            gf.data[...] = np.sum(g_k_w[bl].data, axis=0)
+            g_w_loc[bl].data[...] = np.sum(gf.data, axis=0)
         else:
             for k in k_mesh:
-                gf += g_k_w[bl][k,:]
-        gf /= np.prod(k_mesh.dims)
-    return g_w_loc
+                g_w_loc[bl] += gf[k, :]
+        g_w_loc[bl] /= np.prod(k_mesh.dims)
+    return g_w_loc
```

### Comparing `risb-0.1.0/src/risb/solve_lattice.py` & `risb-0.1.1/src/risb/solve_lattice.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,249 +11,272 @@
 # GNU General Public License for more details.
 #
 # You may obtain a copy of the License at
 #     https:#www.gnu.org/licenses/gpl-3.0.txt
 #
 # Authors: H. L. Nourse
 
-import numpy as np
+"""Solvers for rotationally invariant slave-boson mean-field theory on a lattice."""
+
+from collections.abc import Callable
 from itertools import product
+from typing import Any, TypeAlias
+
+import numpy as np
 from numpy.typing import ArrayLike
-from typing import Any, Callable, TypeAlias
+
 from risb import helpers
 from risb.optimize import DIIS
 
-GfStructType : TypeAlias = list[tuple[str,int]]
-MFType : TypeAlias = dict[ArrayLike]
+GfStructType: TypeAlias = list[tuple[str, int]]
+MFType: TypeAlias = dict[ArrayLike]
+
 
-# The structure and methods here have been modeled 
+# The structure and methods here have been modeled
 # after github.com/TRIQS/hartree_fock
 class LatticeSolver:
     """
-    Rotationally invariant slave-bosons (RISB) lattice solver with
-    a local interaction on each cluster.
+    Rotationally invariant slave-bosons (RISB) lattice solver with a local interaction on each cluster.
 
     Parameters
     ----------
     h0_k : dict[numpy.ndarray]
-        Single-particle dispersion between local clusters. Each key 
+        Single-particle dispersion between local clusters. Each key
         represents a single-particle symmetry.
     gf_struct : list[ list of pairs [ (str,int), ...] ]
         Structure of the matrices. For each cluster, it must be a
         list of pairs, each containing the name of the
         matrix block as a string and the size of that block.
         For example for a single cluster: ``[ ('up', 3), ('down', 3) ]``.
     embedding : list[class]
-        The class that solves the embedding problem for each cluster. It must 
-        already store the interactiong Hamiltonian ``h_int`` on a cluster, 
-        have a method ``set_h_emb(h0_loc_mat, Lambda_c, D)`` to setup the 
-        impurity problem, a method ``solve(**embedding_param)`` that solves 
-        the impurity problem, and methods ``get_rho_f(block)`` and 
-        ``get_rho_cf(block)`` for the bath and hybridization density matrices. 
+        The class that solves the embedding problem for each cluster. It must
+        already store the interactiong Hamiltonian ``h_int`` on a cluster,
+        have a method ``set_h_emb(h0_loc_mat, Lambda_c, D)`` to setup the
+        impurity problem, a method ``solve(**embedding_param)`` that solves
+        the impurity problem, and methods ``get_rho_f(block)`` and
+        ``get_rho_cf(block)`` for the bath and hybridization density matrices.
         See class :class:`.EmbeddingAtomDiag`.
     update_weights : callable
-        The function that gives the integral weights at each k-point on the 
-        lattice. It is called as ``update_weights(energies, **kweight_param)``, 
-        where the energies are a dictionary with each key a list. 
+        The function that gives the integral weights at each k-point on the
+        lattice. It is called as ``update_weights(energies, **kweight_param)``,
+        where the energies are a dictionary with each key a list.
         See class :class:`.SmearingKWeight`.
     root : callable, optional
         The function that drives the self-consistent procedure. It is called
-        as ``root(fun, x0, args=, tol=, **kwargs)``, where ``x0`` is the initial 
-        guess vector, and ``fun`` is the function to minimize, 
+        as ``root(fun, x0, args=, tol=, **kwargs)``, where ``x0`` is the initial
+        guess vector, and ``fun`` is the function to minimize,
         where ``fun = self._target_function``.
         Defaults to :meth:`.DIIS.solve` method of :class:`.DIIS`.
     projectors : list[dict[numpy.ndarray]], optional
         The projectors onto each subspace of an `embedding` cluster.
     gf_struct_mapping : list[dict[str,str]], optional
-        The mapping from the symmetry blocks of each cluster in `embedding` 
-        to the symmetry blocks of `h0_k`. Default assumes the keys in 
+        The mapping from the symmetry blocks of each cluster in `embedding`
+        to the symmetry blocks of `h0_k`. Default assumes the keys in
         all clusters are the same as the keys in `h0_k`.
     symmetries : list[callable], optional
-        Symmetry functions acting on the mean-field matrices. The argument of 
-        the function must take a list of all clusters. 
+        Symmetry functions acting on the mean-field matrices. The argument of
+        the function must take a list of all clusters.
         E.g., ``[R_cluster1, R_cluster2, ...]``.
     force_real : bool, optional
         True if the mean-field matrices are forced to be real
     error_fun : str, optional
-        At each self-consistent cycle, whether the returned error function is 
+        At each self-consistent cycle, whether the returned error function is
             - 'root' : f1 and f2 root functions
             - 'recursion' : the difference between consecutive :attr:`Lambda` and :attr:`R`.
         Defaults to 'root'.
     return_x_new : bool, optional
-        Whether to return a new guess for ``x`` and the ``error`` at each iteration or 
+        Whether to return a new guess for ``x`` and the ``error`` at each iteration or
         only the ``error``. :func:`scipy.optimize.root` should only use the ``error``.
 
     """
-    def __init__(self, 
-                 h0_k : MFType,
-                 gf_struct : GfStructType,
-                 embedding, 
-                 update_weights,
-                 root = None,
-                 projectors = None,
-                 gf_struct_mapping : list[dict[str,str]] | None = None,
-                 symmetries : list[Callable[[MFType], dict[MFType]]] | None = [],
-                 force_real : bool = False,
-                 error_fun : {'root', 'recursion'} = 'recursion',
-                 return_x_new : bool = True,
-                 ):
+
+    def __init__(
+        self,
+        h0_k: MFType,
+        gf_struct: GfStructType,
+        embedding,
+        update_weights,
+        root=None,
+        projectors=None,
+        gf_struct_mapping: list[dict[str, str]] | None = None,
+        symmetries: list[Callable[[MFType], dict[MFType]]] | None = None,
+        force_real: bool = False,
+        error_fun: str = "recursion",
+        return_x_new: bool = True,
+    ):
+        if symmetries is None:
+            symmetries = []
 
         #: dict[numpy.ndarray] : Non-interacting Hamiltonian in k-space.
         self.h0_k = h0_k
-        
+
         # FIXME is this the best way to make sure gf_struct is a list of gf_struct?
-        if isinstance(gf_struct[0][0], str) or isinstance(gf_struct[0][0], int):
+        if isinstance(gf_struct[0][0], str | int):
             self.gf_struct = [gf_struct]
         else:
             self.gf_struct = gf_struct
-        
+
         #: int : Number of correlated clusters per supercell on the lattice.
         self.n_clusters = len(self.gf_struct)
-        
+
         if isinstance(embedding, list):
             self.embedding = embedding
         else:
             self.embedding = [embedding]
         if len(self.embedding) != self.n_clusters:
-            raise ValueError(f'Need embedded space (got {len(self.embedding)} for each cluster (got {self.n_clusters}) !')
+            msg = f"Need embedded space (got {len(self.embedding)} for each cluster (got {self.n_clusters}) !"
+            raise ValueError(msg)
 
         self._update_weights = update_weights
-        
+
         self._root = root
         if self._root is None:
             self.optimize = DIIS()
             self._root = self.optimize.solve
 
         self.projectors = projectors
         if (self.projectors is not None) and (len(self.projectors) != self.n_clusters):
-            raise ValueError(f'Need a projector (got {len(self.projectors)} for each cluster (got {self.n_clusters}) !')
-                        
+            msg = f"Need a projector (got {len(self.projectors)} for each cluster (got {self.n_clusters}) !"
+            raise ValueError(msg)
+
         if gf_struct_mapping is None:
-            self.gf_struct_mapping = [{bl:bl for bl in h0_k.keys()} for i in range(self.n_clusters)]
+            self.gf_struct_mapping = [
+                {bl: bl for bl in h0_k} for i in range(self.n_clusters)
+            ]
         else:
             self.gf_struct_mapping = gf_struct_mapping
         if len(self.gf_struct_mapping) != self.n_clusters:
-            raise ValueError(f'Need a a gf_struct_mapping (got {len(self.gf_struct_mapping)}) for each cluster (got {self.n_clusters}) !')
- 
+            msg = f"Need a a gf_struct_mapping (got {len(self.gf_struct_mapping)}) for each cluster (got {self.n_clusters}) !"
+            raise ValueError(msg)
+
         self.symmetries = symmetries
         self.force_real = force_real
         self.error_fun = error_fun
         self.return_x_new = return_x_new
 
         # The Hermitian basis in each block of a cluster
         # TODO make H_basis an input
-        self._H_basis = [{bl:self._hermitian_basis(bl_size, self.force_real) for bl, bl_size in self.gf_struct[i]} for i in range(self.n_clusters)]
+        self._H_basis = [
+            {
+                bl: self._hermitian_basis(bl_size, self.force_real)
+                for bl, bl_size in self.gf_struct[i]
+            }
+            for i in range(self.n_clusters)
+        ]
 
-        #: dict[numpy.ndarray] : :attr:`h0_k` with the local couplings from 
-        #; each correlated subspace removed.
+        #: dict[numpy.ndarray] : :attr:`h0_k` with the local couplings from
+        # ; each correlated subspace removed.
         self.h0_kin_k = helpers.get_h0_kin_k(h0_k, projectors, gf_struct_mapping)
 
-        #: list[dict(numpy.ndarray)] : Matrices of non-interacting local hopping 
+        #: list[dict(numpy.ndarray)] : Matrices of non-interacting local hopping
         #: terms and energies in :attr:`h0_k`.
         self.h0_loc_matrix = self._get_h0_loc_matrix()
-        
+
         #: list[dict[numpy.ndarray]] : Renormalization matrix
         #: from c- to f-electrons at the mean-field level for each cluster.
         self.R = self._initialize_block_mf_matrix(self.gf_struct, self.force_real)
-        
+
         for i in range(self.n_clusters):
             for bl_sub, _ in self.gf_struct[i]:
                 np.fill_diagonal(self.R[i][bl_sub], 1)
-        
-        #: list[dict[numpy.ndarray]] : Correlation potential matrix of the quasiparticles 
+
+        #: list[dict[numpy.ndarray]] : Correlation potential matrix of the quasiparticles
         #: for each cluster.
         self.Lambda = self._initialize_block_mf_matrix(self.gf_struct, self.force_real)
-        
+
         #: list[dict[numpy.ndarray]] : Bath coupling of impurity for each cluster.
-        self.Lambda_c = [dict() for i in range(self.n_clusters)]
+        self.Lambda_c = [{} for i in range(self.n_clusters)]
 
         #: list[dict[numpy.ndarray]] : Hybridization of impurity for each cluster.
-        self.D = [dict() for i in range(self.n_clusters)]
+        self.D = [{} for i in range(self.n_clusters)]
 
         #: list[dict[numpy.ndarray]] : Density matrix of quasiparticles for each cluster.
-        self.rho_qp = [dict() for i in range(self.n_clusters)]
-        
+        self.rho_qp = [{} for i in range(self.n_clusters)]
+
         #: list[dict[numpy.ndarray]] : Lopsided kinetic energy of quasiparticles for each cluster.
-        self.lopsided_ke_qp = [dict() for i in range(self.n_clusters)]
-        
+        self.lopsided_ke_qp = [{} for i in range(self.n_clusters)]
+
         #: list[dict[numpy.ndarray]] : Kinetic energy of quasiparticles for each cluster.
-        self.ke_qp = [dict() for i in range(self.n_clusters)]
+        self.ke_qp = [{} for i in range(self.n_clusters)]
 
         #: list[dict[numpy.ndarray]] : Density matrix of cluster for each cluster.
-        self.rho_c = [dict() for i in range(self.n_clusters)]
+        self.rho_c = [{} for i in range(self.n_clusters)]
 
         #: list[dict[numpy.ndarray]] : Density matrix of f-electrons in the impurity of each cluster.
-        self.rho_f = [dict() for i in range(self.n_clusters)]
+        self.rho_f = [{} for i in range(self.n_clusters)]
 
-        #: list[dict[numpy.ndarray]] : Hybridization density matrix between the c- 
+        #: list[dict[numpy.ndarray]] : Hybridization density matrix between the c-
         #: and f-electrons in the impurity for each cluster.
-        self.rho_cf = [dict() for i in range(self.n_clusters)]
-        
+        self.rho_cf = [{} for i in range(self.n_clusters)]
+
         #: list[dict[numpy.ndarray]] : The first root function of the self-consistent loop.
-        self.f1 = [dict() for i in range(self.n_clusters)]
+        self.f1 = [{} for i in range(self.n_clusters)]
 
         #: list[dict[numpy.ndarray]] : The second root function of the self-consistent loop.
-        self.f2 = [dict() for i in range(self.n_clusters)]
+        self.f2 = [{} for i in range(self.n_clusters)]
 
-        #: dict[numpy.ndarray] : k-space integration weights of the 
+        #: dict[numpy.ndarray] : k-space integration weights of the
         #: quasiparticles in each band.
-        self.kweights = dict()
-        
+        self.kweights = {}
+
         #: dict[numpy.ndarray] : Band energy of quasiparticles.
-        self.energies_qp = dict()
+        self.energies_qp = {}
 
         #: dict[numpy.ndarray] : Bloch band vectors of quasiparticles.
-        self.bloch_vector_qp = dict()
-        
+        self.bloch_vector_qp = {}
+
         self.iteration = 0
 
     def root(self, *args, **kwargs) -> np.ndarray:
         """
-        The root function that drives the self-consistent procedure. It 
-        is called the same as :func:`scipy.optimize.root`.
+        Root function that drives the self-consistent procedure. It is called the same as :func:`scipy.optimize.root`.
 
         Returns
         -------
         numpy.ndarray
+
         """
         return self._root(*args, **kwargs)
-    
+
     def update_weights(self, *args, **kwargs) -> dict[np.ndarray]:
         """
-        The function that gives the k-space integration weights. It is 
-        called as ``update_weights(dict[numpy.ndarray], **params)``.
+        Update function that gives k-space integration weights. It is called as ``update_weights(dict[numpy.ndarray], **params)``.
 
         Returns
         -------
         numpy.ndarray
+
         """
         return self._update_weights(*args, **kwargs)
-    
+
     @staticmethod
-    def _hermitian_basis(N : int, is_real : bool = False):
+    def _hermitian_basis(N: int, is_real: bool = False):
         """
+        Return a basis of Hermitian matrices of size N.
+
         Parameters
         ----------
         N : int
             The dimension of the Hermitian matrics
         is_real : bool
             If True spans only symmetric matrices.
 
         Returns
         -------
         list[numpy.ndarray]
-            A list of matrices that define an orthonormal basis tat spans all
+            A list of matrices that define an orthonormal basis that spans all
             Hermitian matrices of dimension `N`.
+
         """
         if is_real:
-            n_basis = int(N + N*(N-1)/2)
-            H_rs = [np.zeros([N,N]) for _ in range(n_basis)]
+            n_basis = int(N + N * (N - 1) / 2)
+            H_rs = [np.zeros([N, N]) for _ in range(n_basis)]
         else:
-            n_basis = int(N + N*(N-1)/2 + N*(N-1)/2)
-            H_rs = [np.zeros([N,N], dtype=complex) for _ in range(n_basis)]
+            n_basis = int(N + N * (N - 1) / 2 + N * (N - 1) / 2)
+            H_rs = [np.zeros([N, N], dtype=complex) for _ in range(n_basis)]
 
         # Construct orthogonal basis
         i = 0
         for r, s in product(range(N), range(N)):
             if r == s:
                 H_rs[i][r, r] = 1
                 i = i + 1
@@ -265,321 +288,421 @@
                 if not is_real:
                     H_rs[i][r, s] = 1j
                     H_rs[i][s, r] = -1j
                     i = i + 1
 
         # Normalize
         for i in range(len(H_rs)):
-            H_rs[i] = H_rs[i] / np.sqrt( np.einsum( 'ij,ji->', H_rs[i].conj().T, H_rs[i] ) )
+            H_rs[i] = H_rs[i] / np.sqrt(np.einsum("ij,ji->", H_rs[i].conj().T, H_rs[i]))
         return H_rs
-    
+
     @staticmethod
-    def _initialize_block_mf_matrix(gf_struct : GfStructType,
-                                    is_real : bool) -> MFType:
+    def _initialize_block_mf_matrix(gf_struct: GfStructType, is_real: bool) -> MFType:
         n_clusters = len(gf_struct)
-        A = [dict() for i in range(n_clusters)]
+        A = [{} for i in range(n_clusters)]
         for i in range(n_clusters):
             for bl, bsize in gf_struct[i]:
                 if is_real:
-                    A[i][bl] = np.zeros((bsize,bsize))
+                    A[i][bl] = np.zeros((bsize, bsize))
                 else:
-                    A[i][bl] = np.zeros((bsize,bsize), dtype=complex)
+                    A[i][bl] = np.zeros((bsize, bsize), dtype=complex)
         return A
 
-    def _flatten_matrix(self, 
-                        A : MFType, 
-                        is_coeff_real : bool):
+    def _flatten_matrix(self, A: MFType, is_coeff_real: bool):
         if len(A) != len(self._H_basis):
-            raise ValueError(f'len(A) = {len(A)} and len(H_basis) = {len(self._H_basis)} must have the same number of clusters !')
+            msg = f"len(A) = {len(A)} and len(H_basis) = {len(self._H_basis)} must have the same number of clusters !"
+            raise ValueError(msg)
         x = []
         for i in range(self.n_clusters):
-            for bl, bl_size in self.gf_struct[i]:
+            for bl, _bl_size in self.gf_struct[i]:
                 for h in self._H_basis[i][bl]:
-                    # To extract a coefficient of a basis that spans a vector 
+                    # To extract a coefficient of a basis that spans a vector
                     # space it is the inner product <basis_vec, vec> = coeff
-                    # if the basis_vec is orthonormal. For matrices the inner 
+                    # if the basis_vec is orthonormal. For matrices the inner
                     # product is <A, B> = Tr(A^+, B).
-                    # Note that einsum is order mag faster than tr(a,b) and 
+                    # Note that einsum is order mag faster than tr(a,b) and
                     # stores no intermediate array
-                    # Could also vectorize both matrices as flatten('F') to 
+                    # Could also vectorize both matrices as flatten('F') to
                     # column-major order and then take normal inner product
-                    coeff = np.einsum('ij,ji->', h.conj().T, A[i][bl])
-                    x.append( coeff.real )
+                    coeff = np.einsum("ij,ji->", h.conj().T, A[i][bl])
+                    x.append(coeff.real)
                     if (not is_coeff_real) and (not self.force_real):
-                        x.append( coeff.imag )
+                        x.append(coeff.imag)
         return x
 
-    def _unflatten_matrix(self,
-                          x : ArrayLike, 
-                          is_coeff_real : bool, 
-                          offset : int = 0) -> tuple[MFType, int]:
+    def _unflatten_matrix(
+        self, x: ArrayLike, is_coeff_real: bool, offset: int = 0
+    ) -> tuple[MFType, int]:
         A = self._initialize_block_mf_matrix(self.gf_struct, self.force_real)
         for i in range(self.n_clusters):
-            for bl, bl_size in self.gf_struct[i]:
+            for bl, _bl_size in self.gf_struct[i]:
                 for h in self._H_basis[i][bl]:
-                    # x stores the coefficients of the basis of Hermitian 
+                    # x stores the coefficients of the basis of Hermitian
                     # matrices defined in self._H_basis.
                     if is_coeff_real or self.force_real:
                         A[i][bl] += x[offset] * h
                         offset = offset + 1
                     else:
-                        A[i][bl] += (x[offset] + 1j*x[offset+1]) * h
+                        A[i][bl] += (x[offset] + 1j * x[offset + 1]) * h
                         offset = offset + 2
         return A, offset
 
     @staticmethod
     # Not really used
     def _make_hermitian(A):
         if isinstance(A, list):
             for i in range(len(A)):
-                for bl in A[i].keys():
+                for bl in A[i]:
                     A[i][bl] = 0.5 * (A[i][bl] + A[i][bl].conj().T)
         elif isinstance(A, dict):
-            for bl in A.keys():
+            for bl in A:
                 A[bl] = 0.5 * (A[bl] + A[bl].conj().T)
         elif isinstance(A, np.ndarray):
             A = 0.5 * (A + A.conj().T)
         else:
-            raise ValueError('A is not a list[dict[ndarray]], dict[ndarray], or ndarray !')
+            msg = "A is not a list[dict[ndarray]], dict[ndarray], or ndarray !"
+            raise ValueError(msg)
         return A
-    
+
     def _get_h0_loc_matrix(self) -> MFType:
-        h0_loc_matrix = self._initialize_block_mf_matrix(self.gf_struct, self.force_real)
-        
+        h0_loc_matrix = self._initialize_block_mf_matrix(
+            self.gf_struct, self.force_real
+        )
+
         for i in range(self.n_clusters):
-            for bl, bl_size in self.gf_struct[i]:
+            for bl, _bl_size in self.gf_struct[i]:
                 bl_full = self.gf_struct_mapping[i][bl]
                 if self.projectors is not None:
-                    h0_loc_matrix[i][bl] = helpers.get_h0_loc_matrix(self.h0_k[bl_full], self.projectors[i][bl] )
+                    h0_loc_matrix[i][bl] = helpers.get_h0_loc_matrix(
+                        self.h0_k[bl_full], self.projectors[i][bl]
+                    )
                 else:
                     h0_loc_matrix[i][bl] = helpers.get_h0_loc_matrix(self.h0_k[bl_full])
 
-        h0_loc_matrix, _ = self._unflatten_matrix( self._flatten_matrix( h0_loc_matrix, is_coeff_real=True ), is_coeff_real=True )
+        h0_loc_matrix, _ = self._unflatten_matrix(
+            self._flatten_matrix(h0_loc_matrix, is_coeff_real=True), is_coeff_real=True
+        )
         for function in self.symmetries:
             h0_loc_matrix = function(h0_loc_matrix)
 
         return h0_loc_matrix
-        
-    def _target_function(self, 
-                        x : ArrayLike, 
-                        embedding_param : list[dict[str, Any]], 
-                        kweight_param : dict[str, Any], 
-                        ) -> np.ndarray | tuple[np.ndarray, np.ndarray]:
-        
+
+    def _target_function(
+        self,
+        x: ArrayLike,
+        embedding_param: list[dict[str, Any]],
+        kweight_param: dict[str, Any],
+    ) -> np.ndarray | tuple[np.ndarray, np.ndarray]:
         self.Lambda, offset = self._unflatten_matrix(x, is_coeff_real=True)
         self.R, _ = self._unflatten_matrix(x, is_coeff_real=False, offset=offset)
-        self.Lambda, self.R, self.f1, self.f2  = self.one_cycle(embedding_param, kweight_param)
-        x_new = np.array( self._flatten_matrix(self.Lambda, is_coeff_real=True) + self._flatten_matrix(self.R, is_coeff_real=False) )
-        
-        if self.error_fun == 'root':
-            x_error = np.array( self._flatten_matrix(self.f2, is_coeff_real=True) + self._flatten_matrix(self.f1, is_coeff_real=False) )
-        elif self.error_fun == 'recursion':
+        self.Lambda, self.R, self.f1, self.f2 = self.one_cycle(
+            embedding_param, kweight_param
+        )
+        x_new = np.array(
+            self._flatten_matrix(self.Lambda, is_coeff_real=True)
+            + self._flatten_matrix(self.R, is_coeff_real=False)
+        )
+
+        if self.error_fun == "root":
+            x_error = np.array(
+                self._flatten_matrix(self.f2, is_coeff_real=True)
+                + self._flatten_matrix(self.f1, is_coeff_real=False)
+            )
+        elif self.error_fun == "recursion":
             x_error = x_new - x
         else:
-            raise ValueError('Unrecognized error functions for root !')
-        
+            msg = "Unrecognized error functions for root !"
+            raise ValueError(msg)
+
         if self.return_x_new:
             return x_new, x_error
-        else:
-            return x_error
-    
-    def one_cycle(self, 
-                  embedding_param : list[dict[str, Any]] | None = None, 
-                  kweight_param : dict[str, Any] = dict()):
-                    #-> tuple[MFType, MFType, MFType, MFType]:
+        return x_error
+
+    def one_cycle(
+        self,
+        embedding_param: list[dict[str, Any]] | None = None,
+        kweight_param: dict[str, Any] | None = None,
+    ):
+        # -> tuple[MFType, MFType, MFType, MFType]:
         """
-        A single iteration of the RISB self-consistent cycle.
+        Single iteration of the RISB self-consistent cycle.
 
         Parameters
         ----------
         embedding_param : list[dict], optional
             The kwarg arguments to pass to the :meth:`embedding.solve` for each cluster.
         kweight_param : dict, optional
             The kwarg arguments to pass to :meth:`update_weights`.
-        
+
         Returns
         -------
         Lambda : list[dict[numpy.ndarray]]
             The new guess for the correlation potential matrix on each cluster.
         R : list[dict[numpy.ndarray]]
             The new guess for the renormalization matrix on each cluster.
         f1 : list[dict[numpy.ndarray]]
-            The return of the fixed-point function that matches the 
+            The return of the fixed-point function that matches the
             quasiparticle density matrices on each cluster.
         f2 : list[dict[numpy.ndarray]]
-            The return of the fixed-point function that matches the 
+            The return of the fixed-point function that matches the
             hybridzation density matrices on each cluster.
-        """
 
+        """
+        if kweight_param is None:
+            kweight_param = {}
         if embedding_param is None:
-            embedding_param = [dict() for i in range(self.n_clusters)]
- 
+            embedding_param = [{} for i in range(self.n_clusters)]
+
         for function in self.symmetries:
             self.R = function(self.R)
             self.Lambda = function(self.Lambda)
-        
+
         # Make R, Lambda in supercell basis from basis of the clusters
         # FIXME check if projectors get broadcast correctly if they are a diff proj at each k
-        self.R_full = {bl:0 for bl in self.h0_kin_k.keys()}
-        self.Lambda_full = {bl:0 for bl in self.h0_kin_k.keys()}
+        self.R_full = {bl: 0 for bl in self.h0_kin_k}
+        self.Lambda_full = {bl: 0 for bl in self.h0_kin_k}
         if self.projectors is not None:
             for i in range(self.n_clusters):
                 for bl, _ in self.gf_struct[i]:
                     bl_full = self.gf_struct_mapping[i][bl]
-                    self.R_full[bl_full] += self.projectors[i][bl].conj().T @ self.R[i][bl] @ self.projectors[i][bl]
-                    self.Lambda_full[bl_full] += self.projectors[i][bl].conj().T @ self.Lambda[i][bl] @ self.projectors[i][bl]
+                    self.R_full[bl_full] += (
+                        self.projectors[i][bl].conj().T
+                        @ self.R[i][bl]
+                        @ self.projectors[i][bl]
+                    )
+                    self.Lambda_full[bl_full] += (
+                        self.projectors[i][bl].conj().T
+                        @ self.Lambda[i][bl]
+                        @ self.projectors[i][bl]
+                    )
         else:
             for bl, _ in self.gf_struct[0]:
                 bl_full = self.gf_struct_mapping[0][bl]
                 self.R_full[bl_full] += self.R[0][bl]
                 self.Lambda_full[bl_full] += self.Lambda[0][bl]
-        
-        h0_k_R = dict()
-        #R_h0_k_R = dict()
-        for bl in self.h0_kin_k.keys():
-            h_qp = helpers.get_h_qp(self.R_full[bl], self.Lambda_full[bl], self.h0_kin_k[bl])
+
+        h0_k_R = {}
+        # R_h0_k_R = dict()
+        for bl in self.h0_kin_k:
+            h_qp = helpers.get_h_qp(
+                self.R_full[bl], self.Lambda_full[bl], self.h0_kin_k[bl]
+            )
             self.energies_qp[bl], self.bloch_vector_qp[bl] = np.linalg.eigh(h_qp)
-            h0_k_R[bl] = helpers.get_h0_kin_k_R(self.R_full[bl], self.h0_kin_k[bl], self.bloch_vector_qp[bl])
-            #R_h0_k_R[bl] = helpers.get_R_h0_kin_kR(R_full[bl], self.h0_kin_k[bl], self.bloch_vector_qp[bl])
-        
+            h0_k_R[bl] = helpers.get_h0_kin_k_R(
+                self.R_full[bl], self.h0_kin_k[bl], self.bloch_vector_qp[bl]
+            )
+            # R_h0_k_R[bl] = helpers.get_R_h0_kin_kR(R_full[bl], self.h0_kin_k[bl], self.bloch_vector_qp[bl])
+
         self.kweights = self.update_weights(self.energies_qp, **kweight_param)
 
         for i in range(self.n_clusters):
             for bl, _ in self.gf_struct[i]:
                 bl_full = self.gf_struct_mapping[i][bl]
                 if self.projectors is not None:
-                    self.rho_qp[i][bl] = helpers.get_rho_qp(self.bloch_vector_qp[bl_full], self.kweights[bl_full], self.projectors[i][bl])
-                    self.lopsided_ke_qp[i][bl] = helpers.get_ke(h0_k_R[bl_full], self.bloch_vector_qp[bl_full], self.kweights[bl_full], self.projectors[i][bl])
+                    self.rho_qp[i][bl] = helpers.get_rho_qp(
+                        self.bloch_vector_qp[bl_full],
+                        self.kweights[bl_full],
+                        self.projectors[i][bl],
+                    )
+                    self.lopsided_ke_qp[i][bl] = helpers.get_ke(
+                        h0_k_R[bl_full],
+                        self.bloch_vector_qp[bl_full],
+                        self.kweights[bl_full],
+                        self.projectors[i][bl],
+                    )
                 else:
-                    self.rho_qp[i][bl] = helpers.get_rho_qp(self.bloch_vector_qp[bl_full], self.kweights[bl_full])
-                    self.lopsided_ke_qp[i][bl] = helpers.get_ke(h0_k_R[bl_full], self.bloch_vector_qp[bl_full], self.kweights[bl_full])
-                #self.ke_qp[i][bl] = helpers.get_ke(R_h0_k_R[bl_full], self.bloch_vector_qp[bl_full], self.kweights[bl_full], self.projectors[i][bl])
-        
-        # FIXME More expensive to do this than just storing and working with the coefficients, but 
+                    self.rho_qp[i][bl] = helpers.get_rho_qp(
+                        self.bloch_vector_qp[bl_full], self.kweights[bl_full]
+                    )
+                    self.lopsided_ke_qp[i][bl] = helpers.get_ke(
+                        h0_k_R[bl_full],
+                        self.bloch_vector_qp[bl_full],
+                        self.kweights[bl_full],
+                    )
+                # self.ke_qp[i][bl] = helpers.get_ke(R_h0_k_R[bl_full], self.bloch_vector_qp[bl_full], self.kweights[bl_full], self.projectors[i][bl])
+
+        # FIXME More expensive to do this than just storing and working with the coefficients, but
         # nothing compared to solving the embedding problem so this is likely fine
         # Enforce matrix structure from symmetries
-        self.rho_qp, _ = self._unflatten_matrix( self._flatten_matrix( self.rho_qp, is_coeff_real=True ), is_coeff_real=True )
-        #self.lopsided_ke_qp, _ = self._unflatten_matrix( self._flatten_matrix( self.lopsided_ke_qp, is_coeff_real=False ), is_coeff_real=False )
+        self.rho_qp, _ = self._unflatten_matrix(
+            self._flatten_matrix(self.rho_qp, is_coeff_real=True), is_coeff_real=True
+        )
+        # self.lopsided_ke_qp, _ = self._unflatten_matrix( self._flatten_matrix( self.lopsided_ke_qp, is_coeff_real=False ), is_coeff_real=False )
         for function in self.symmetries:
             self.rho_qp = function(self.rho_qp)
-            #self.lopsided_ke_qp = function(self.lopsided_ke_qp) # FIXME can I do it to ke as well? It should have same symm as D
-            #self.ke_qp = function(self.ke_qp)
-        
+            # self.lopsided_ke_qp = function(self.lopsided_ke_qp) # FIXME can I do it to ke as well? It should have same symm as D
+            # self.ke_qp = function(self.ke_qp)
+
         for i in range(self.n_clusters):
             for bl, _ in self.gf_struct[i]:
                 if self.force_real:
-                    self.D[i][bl] = helpers.get_d(self.rho_qp[i][bl], self.lopsided_ke_qp[i][bl]).real
-                    #self.D[i][bl] = helpers.get_d2(self.rho_qp[i][bl], self.ke_qp[i][bl], self.R[i][bl]).real
-                    self.Lambda_c[i][bl] = helpers.get_lambda_c(self.rho_qp[i][bl], self.R[i][bl], self.Lambda[i][bl], self.D[i][bl]).real
+                    self.D[i][bl] = helpers.get_d(
+                        self.rho_qp[i][bl], self.lopsided_ke_qp[i][bl]
+                    ).real
+                    # self.D[i][bl] = helpers.get_d2(self.rho_qp[i][bl], self.ke_qp[i][bl], self.R[i][bl]).real
+                    self.Lambda_c[i][bl] = helpers.get_lambda_c(
+                        self.rho_qp[i][bl],
+                        self.R[i][bl],
+                        self.Lambda[i][bl],
+                        self.D[i][bl],
+                    ).real
                 else:
-                    self.D[i][bl] = helpers.get_d(self.rho_qp[i][bl], self.lopsided_ke_qp[i][bl])
-                    #self.D[i][bl] = helpers.get_d2(self.rho_qp[i][bl], self.ke_qp[i][bl], self.R[i][bl])
-                    self.Lambda_c[i][bl] = helpers.get_lambda_c(self.rho_qp[i][bl], self.R[i][bl], self.Lambda[i][bl], self.D[i][bl])
-                    
+                    self.D[i][bl] = helpers.get_d(
+                        self.rho_qp[i][bl], self.lopsided_ke_qp[i][bl]
+                    )
+                    # self.D[i][bl] = helpers.get_d2(self.rho_qp[i][bl], self.ke_qp[i][bl], self.R[i][bl])
+                    self.Lambda_c[i][bl] = helpers.get_lambda_c(
+                        self.rho_qp[i][bl],
+                        self.R[i][bl],
+                        self.Lambda[i][bl],
+                        self.D[i][bl],
+                    )
+
         # Enforce matrix structure from symmetries
-        self.Lambda_c, _ = self._unflatten_matrix( self._flatten_matrix( self.Lambda_c, is_coeff_real=True ), is_coeff_real=True )
-        self.D, _ = self._unflatten_matrix( self._flatten_matrix( self.D, is_coeff_real=False ), is_coeff_real=False )
+        self.Lambda_c, _ = self._unflatten_matrix(
+            self._flatten_matrix(self.Lambda_c, is_coeff_real=True), is_coeff_real=True
+        )
+        self.D, _ = self._unflatten_matrix(
+            self._flatten_matrix(self.D, is_coeff_real=False), is_coeff_real=False
+        )
         for function in self.symmetries:
             self.Lambda_c = function(self.Lambda_c)
             self.D = function(self.D)
 
         for i in range(self.n_clusters):
-            self.embedding[i].set_h_emb(self.Lambda_c[i], self.D[i], self.h0_loc_matrix[i])
+            self.embedding[i].set_h_emb(
+                self.Lambda_c[i], self.D[i], self.h0_loc_matrix[i]
+            )
             self.embedding[i].solve(**embedding_param[i])
             for bl, _ in self.gf_struct[i]:
                 self.rho_f[i][bl] = self.embedding[i].get_rho_f(bl)
                 self.rho_cf[i][bl] = self.embedding[i].get_rho_cf(bl)
-        
+
         ## Enforce matrix structure from symmetries
-        self.rho_f, _ = self._unflatten_matrix( self._flatten_matrix( self.rho_f, is_coeff_real=True ), is_coeff_real=True )
-        self.rho_cf, _ = self._unflatten_matrix( self._flatten_matrix( self.rho_cf, is_coeff_real=False ), is_coeff_real=False )
+        self.rho_f, _ = self._unflatten_matrix(
+            self._flatten_matrix(self.rho_f, is_coeff_real=True), is_coeff_real=True
+        )
+        self.rho_cf, _ = self._unflatten_matrix(
+            self._flatten_matrix(self.rho_cf, is_coeff_real=False), is_coeff_real=False
+        )
         for function in self.symmetries:
             self.rho_f = function(self.rho_f)
             self.rho_cf = function(self.rho_cf)
 
         for i in range(self.n_clusters):
             for bl, _ in self.gf_struct[i]:
-                self.f1[i][bl] = helpers.get_f1(self.rho_cf[i][bl], self.rho_qp[i][bl], self.R[i][bl])
+                self.f1[i][bl] = helpers.get_f1(
+                    self.rho_cf[i][bl], self.rho_qp[i][bl], self.R[i][bl]
+                )
                 self.f2[i][bl] = helpers.get_f2(self.rho_f[i][bl], self.rho_qp[i][bl])
-        
+
         # Enforce matrix structure from symmetries
-        self.f2, _ = self._unflatten_matrix( self._flatten_matrix( self.f2, is_coeff_real=True ), is_coeff_real=True )
-        self.f1, _ = self._unflatten_matrix( self._flatten_matrix( self.f1, is_coeff_real=False ), is_coeff_real=False )
+        self.f2, _ = self._unflatten_matrix(
+            self._flatten_matrix(self.f2, is_coeff_real=True), is_coeff_real=True
+        )
+        self.f1, _ = self._unflatten_matrix(
+            self._flatten_matrix(self.f1, is_coeff_real=False), is_coeff_real=False
+        )
         for function in self.symmetries:
             self.f1 = function(self.f1)
             self.f2 = function(self.f2)
-        
+
         for i in range(self.n_clusters):
             for bl, _ in self.gf_struct[i]:
                 if self.force_real:
-                    self.Lambda[i][bl] = helpers.get_lambda(self.R[i][bl], self.D[i][bl], self.Lambda_c[i][bl], self.rho_f[i][bl]).real
-                    self.R[i][bl] = helpers.get_r(self.rho_cf[i][bl], self.rho_f[i][bl]).real
+                    self.Lambda[i][bl] = helpers.get_lambda(
+                        self.R[i][bl],
+                        self.D[i][bl],
+                        self.Lambda_c[i][bl],
+                        self.rho_f[i][bl],
+                    ).real
+                    self.R[i][bl] = helpers.get_r(
+                        self.rho_cf[i][bl], self.rho_f[i][bl]
+                    ).real
                 else:
-                    self.Lambda[i][bl] = helpers.get_lambda(self.R[i][bl], self.D[i][bl], self.Lambda_c[i][bl], self.rho_f[i][bl])
+                    self.Lambda[i][bl] = helpers.get_lambda(
+                        self.R[i][bl],
+                        self.D[i][bl],
+                        self.Lambda_c[i][bl],
+                        self.rho_f[i][bl],
+                    )
                     self.R[i][bl] = helpers.get_r(self.rho_cf[i][bl], self.rho_f[i][bl])
-        
+
         # Enforce matrix structure from symmetries
-        self.Lambda, _ = self._unflatten_matrix( self._flatten_matrix( self.Lambda, is_coeff_real=True ), is_coeff_real=True )
-        self.R, _ = self._unflatten_matrix( self._flatten_matrix( self.R, is_coeff_real=False ), is_coeff_real=False )
+        self.Lambda, _ = self._unflatten_matrix(
+            self._flatten_matrix(self.Lambda, is_coeff_real=True), is_coeff_real=True
+        )
+        self.R, _ = self._unflatten_matrix(
+            self._flatten_matrix(self.R, is_coeff_real=False), is_coeff_real=False
+        )
         for function in self.symmetries:
             self.Lambda = function(self.Lambda)
             self.R = function(self.R)
 
         self.iteration += 1
 
         return self.Lambda, self.R, self.f1, self.f2
-    
-    def solve(self, 
-              one_shot : bool = False, 
-              embedding_param : list[dict[str, Any]] | None = None, 
-              kweight_param : dict[str, Any] = dict(),
-              **kwargs) -> Any:
-        """ 
-        Solve for the renormalization matrix :attr:`R` and correlation potential
-        matrix :attr:`Lambda`.
+
+    def solve(
+        self,
+        one_shot: bool = False,
+        embedding_param: list[dict[str, Any]] | None = None,
+        kweight_param: dict[str, Any] | None = None,
+        **kwargs,
+    ) -> Any:
+        """
+        Solve for the renormalization matrix :attr:`R` and correlation potential matrix :attr:`Lambda`.
 
         Parameters
         ----------
         one_shot : bool, optional
-            True if the calcualtion is just one shot and not self consistent. 
+            True if the calcualtion is just one shot and not self consistent.
             Default is False.
         embedding_param : list[dict], optional
             kwarg options to pass to :meth:`embedding.solve` for each cluster.
         kweight_param : dict, optional
             kwarg options to pass to :meth:`update_weights`.
         **kwargs
             kwarg options to pass to :meth:`root`.
 
         Returns
         -------
         x
-            The flattened x vector of :attr:`Lambda` and :attr:`R`. If using 
-            :func:`scipy.optimize.root` the :class:`scipy.optimize.OptimizeResult` 
+            The flattened x vector of :attr:`Lambda` and :attr:`R`. If using
+            :func:`scipy.optimize.root` the :class:`scipy.optimize.OptimizeResult`
             object will be returned.
         Also sets the self-consistent solutions :attr:`Lambda` and :attr:`R`.
+
         """
-        
+        if kweight_param is None:
+            kweight_param = {}
         if embedding_param is None:
-            embedding_param = [dict() for i in range(self.n_clusters)]
+            embedding_param = [{} for i in range(self.n_clusters)]
 
         if one_shot:
             self.Lambda, self.R, _, _ = self.one_cycle(embedding_param, kweight_param)
-            x = np.array( self._flatten_matrix(self.Lambda, is_coeff_real=True) + self._flatten_matrix(self.R, is_coeff_real=False) )
-        
+            x = np.array(
+                self._flatten_matrix(self.Lambda, is_coeff_real=True)
+                + self._flatten_matrix(self.R, is_coeff_real=False)
+            )
+
         else:
-            x0 = np.array( self._flatten_matrix(self.Lambda, is_coeff_real=True) + self._flatten_matrix(self.R, is_coeff_real=False) )
-            x = self.root(fun=self._target_function, 
-                          x0=x0,
-                          args=(embedding_param, kweight_param),
-                          **kwargs)
+            x0 = np.array(
+                self._flatten_matrix(self.Lambda, is_coeff_real=True)
+                + self._flatten_matrix(self.R, is_coeff_real=False)
+            )
+            x = self.root(
+                fun=self._target_function,
+                x0=x0,
+                args=(embedding_param, kweight_param),
+                **kwargs,
+            )
         return x
-        
+
     @property
     def Z(self) -> MFType:
-        """
-        list[dict[numpy.ndarray]] : Qausiparticle weight of each cluster.
-        """
-        Z = [dict() for i in range(self.n_clusters)]
+        """Returns the quasiparticle weight matrix Z of each cluster as a list[dict[numpy.ndarray]]."""
+        Z = [{} for i in range(self.n_clusters)]
         for i in range(self.n_clusters):
             for bl, _ in self.gf_struct[i]:
                 Z[i][bl] = self.R[i][bl] @ self.R[i][bl].conj().T
-        return Z
+        return Z
```

### Comparing `risb-0.1.0/src/risb/embedding/dummy.py` & `risb-0.1.1/src/risb/embedding/dummy.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,64 +11,73 @@
 # GNU General Public License for more details.
 #
 # You may obtain a copy of the License at
 #     https:#www.gnu.org/licenses/gpl-3.0.txt
 #
 # Authors: H. L. Nourse
 
+"""Embedding solver that acts as a copy of another solver without calculating anything."""
+
 import numpy as np
 
+
 class EmbeddingDummy:
     """
-    Dummy impurity solver. Does not solve anything and instead references 
-    variables of another embedding solver. This is useful when 
-    some inequivalent clusters are the same up to rotations, so only 
-    a single impurity problem has to be solved and then the single-particle 
+    Dummy impurity solver.
+
+    Does not solve anything and instead references
+    variables of another embedding solver. This is useful when
+    some inequivalent clusters are the same up to rotations, so only
+    a single impurity problem has to be solved and then the single-particle
     matrices are rotated into the relevant basis.
 
     Parameters
     ----------
     embedding : class
         The embedding solver class to reference.
     rotations : list[callable], optional
         A list of rotation functions to apply to matrices.
+
     """
-    def __init__(self, embedding, rotations = []):
+
+    def __init__(self, embedding, rotations=None):
+        if rotations is None:
+            rotations = []
         self.embedding = embedding
         self.rotations = rotations
-    
-    def set_h_emb(self, *args, **kwargs):
+
+    def set_h_emb(self, *args, **kwargs):  # noqa: D102
         pass
-    
-    def solve(self, *args, **kwargs):
+
+    def solve(self, *args, **kwargs):  # noqa: D102
         pass
 
-    def get_rho_f(self, bl : str) -> np.ndarray:
+    def get_rho_f(self, bl: str) -> np.ndarray:  # noqa: D102
         if bl not in self.embedding.rho_f:
             rho_f = self.embedding.get_rho_f(bl)
         else:
             rho_f = self.embedding.rho_f[bl]
         for func in self.rotations:
             rho_f = func(rho_f)
         return rho_f
-    
-    def get_rho_c(self, bl : str) -> np.ndarray:
+
+    def get_rho_c(self, bl: str) -> np.ndarray:  # noqa: D102
         if bl not in self.embedding.rho_c:
             rho_c = self.embedding.get_rho_c(bl)
         else:
             rho_c = self.embedding.rho_c[bl]
         for func in self.rotations:
             rho_c = func(rho_c)
         return rho_c
-    
-    def get_rho_cf(self, bl : str) -> np.ndarray:
+
+    def get_rho_cf(self, bl: str) -> np.ndarray:  # noqa: D102
         if bl not in self.embedding.rho_cf:
             rho_cf = self.embedding.get_rho_cf(bl)
         else:
             rho_cf = self.embedding.rho_cf[bl]
         for func in self.rotations:
             rho_cf = func(rho_cf)
         return rho_cf
-    
+
     # FIXME rotate Op correctly, is this even correctly possible?
-    def overlap(self, Op, force_real : bool = True) -> float | complex:
-        return self.embedding.overlap(Op, force_real)
+    def overlap(self, Op, force_real: bool = True) -> float | complex:  # noqa: D102
+        return self.embedding.overlap(Op, force_real)
```

### Comparing `risb-0.1.0/src/risb/embedding/embedding_atom_diag.py` & `risb-0.1.1/src/risb/embedding/embedding_atom_diag.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,321 +11,331 @@
 # GNU General Public License for more details.
 #
 # You may obtain a copy of the License at
 #     https:#www.gnu.org/licenses/gpl-3.0.txt
 #
 # Authors: H. L. Nourse
 
-import numpy as np
+"""Embedding solver using TRIQS AtomDiag."""
+
 from itertools import product
 from typing import TypeAlias, TypeVar
+
+import numpy as np
 from numpy.typing import ArrayLike
 from triqs.atom_diag import AtomDiag, act
 from triqs.operators import Operator, c, c_dag, dagger
+
 from risb.helpers_triqs import get_C_Op
 
-GfStructType : TypeAlias = list[tuple[str,int]]
-OpType = TypeVar('OpType')
-MFType : TypeAlias = dict[ArrayLike]
+GfStructType: TypeAlias = list[tuple[str, int]]
+OpType = TypeVar("OpType")
+MFType: TypeAlias = dict[ArrayLike]
+
 
 class EmbeddingAtomDiag:
     """
-    Impurity solver of embedding space using :class:`triqs.atom_diag.AtomDiag` 
-    from TRIQS.
+    Impurity solver of embedding space using :class:`triqs.atom_diag.AtomDiag` from TRIQS.
 
     Parameters
     ----------
     h_int : triqs.operators.Operator
         Interaction Hamiltonian in the embedding space.
     gf_struct : list of pairs [ (str,int), ...]
         Structure of the matrices. It must be a
         list of pairs, each containing the name of the
         matrix block as a string and the size of that block.
         For example: ``[ ('up', 3), ('down', 3) ]``.
 
     """
 
-    def __init__(self, 
-                 h_int : OpType, 
-                 gf_struct : GfStructType) -> None:
-        
+    def __init__(self, h_int: OpType, gf_struct: GfStructType) -> None:
         #: triqs.operators.Operator : Interaction Hamiltonian.
         self.h_int = h_int
 
         #: dict[tuple[str,int]] : Block matrix structure of c-electrons.
         self.gf_struct = gf_struct
 
         # Set structure of bath and embedding space
         # FIXME if doing ghost bath and loc are not the same size
 
         #: dict[tuple[str,int]] : Block matrix structure of f-electrons.
-        self.gf_struct_bath = [(self._bl_loc_to_bath(bl), bl_size) for bl, bl_size in self.gf_struct]
+        self.gf_struct_bath = [
+            (self._bl_loc_to_bath(bl), bl_size) for bl, bl_size in self.gf_struct
+        ]
 
-        #: dict[tuple[str,int]] : Block matrix structure entire embedding 
+        #: dict[tuple[str,int]] : Block matrix structure entire embedding
         #: space.
         self.gf_struct_emb = self.gf_struct + self.gf_struct_bath
 
         # Set of fundamental operators
         self.fops = self._fops_from_gf_struct(self.gf_struct)
         self.fops_bath = self._fops_from_gf_struct(self.gf_struct_bath)
         self.fops_emb = self._fops_from_gf_struct(self.gf_struct_emb)
-        
+
         # Do gf_struct as a map
         self.gf_struct_dict = self._dict_gf_struct(self.gf_struct)
         self.gf_struct_bath_dict = self._dict_gf_struct(self.gf_struct_bath)
         self.gf_struct_emb_dict = self._dict_gf_struct(self.gf_struct_emb)
 
-        #: triqs.atom_diag.AtomDiag vacuum : Ground state of the embedding 
+        #: triqs.atom_diag.AtomDiag vacuum : Ground state of the embedding
         #: problem.
         self.gs_vector = None
-        
-        #: The TRIQS AtomDiag instance. See :class:`triqs.atom_diag.AtomDiag` 
+
+        #: The TRIQS AtomDiag instance. See :class:`triqs.atom_diag.AtomDiag`
         #: in the TRIQS manual.
         self.ad = None
 
         #: triqs.operators.Operator : Embedding Hamiltonian. It is the sum of
         #: :attr:`h0_loc`, :attr:`h_int`, :attr:`h_hybr`, and :attr:`h_bath`.
-        self.h_emb : OpType = Operator()
+        self.h_emb: OpType = Operator()
 
-        #: triqs.operators.Operator : Single-particle quadratic couplings of 
+        #: triqs.operators.Operator : Single-particle quadratic couplings of
         #: c-electron terms in ::attr:`h_emb`.
-        self.h0_loc : OpType = Operator()
-        
+        self.h0_loc: OpType = Operator()
+
         #: triqs.operators.Operator : Bath terms in :attr:`h_emb`.
-        self.h_bath : OpType = Operator()
-        
+        self.h_bath: OpType = Operator()
+
         #: triqs.operators.Operator : Hybridization terms in :attr:`h_emb`.
-        self.h_hybr : OpType = Operator()
-        
+        self.h_hybr: OpType = Operator()
+
         #: dict[numpy.ndarray] : f-electron density matrix.
-        self.rho_f = dict()
+        self.rho_f = {}
 
         #: dict[numpy.ndarray] : c-electron density matrix.
-        self.rho_c = dict()
-        
-        #: dict[numpy.ndarray] : Density matrix of hybridization terms 
+        self.rho_c = {}
+
+        #: dict[numpy.ndarray] : Density matrix of hybridization terms
         #: (c- and f-electrons).
-        self.rho_cf = dict()
+        self.rho_cf = {}
 
     @staticmethod
-    def _bl_loc_to_bath(bl : str) -> str:
-        return 'bath_'+bl
-    
+    def _bl_loc_to_bath(bl: str) -> str:
+        return "bath_" + bl
+
     @staticmethod
-    def _bl_bath_to_loc(bl : str) -> str:
-        return bl.replace('bath_', '')
-    
+    def _bl_bath_to_loc(bl: str) -> str:
+        return bl.replace("bath_", "")
+
     @staticmethod
-    def _fops_from_gf_struct(gf_struct : GfStructType) -> list[tuple[str, int]]:
-        return [(bl,i) for bl, bl_size in gf_struct for i in range(bl_size)]
-    
+    def _fops_from_gf_struct(gf_struct: GfStructType) -> list[tuple[str, int]]:
+        return [(bl, i) for bl, bl_size in gf_struct for i in range(bl_size)]
+
     @staticmethod
-    def _dict_gf_struct(gf_struct : GfStructType) -> dict[str, int]:
-        return {bl: bl_size for bl, bl_size in gf_struct}
-    
-    def set_h0_loc(self, h0_loc_matrix : MFType) -> None:
-        """
-        Sets the single-particle quadratic couplings of the c-electrons in the 
-        embedding Hamiltonian.
-        
+    def _dict_gf_struct(gf_struct: GfStructType) -> dict[str, int]:
+        return dict(gf_struct)
+
+    def set_h0_loc(self, h0_loc_matrix: MFType) -> None:
+        """
+        Set the single-particle quadratic couplings of the c-electrons in the embedding Hamiltonian.
+
         Parameters
         ----------
         h0_loc_matrix : dict of ndarray, optional
-            Quadratic terms as a matrix. Each key in dictionary must follow 
+            Quadratic terms as a matrix. Each key in dictionary must follow
             :attr:`gf_struct`.
+
         """
         C_Op = get_C_Op(self.gf_struct, dagger=False)
         C_dag_Op = get_C_Op(self.gf_struct, dagger=True)
-        self.h0_loc : OpType = Operator()
-        for bl, bl_size in self.gf_struct:
+        self.h0_loc: OpType = Operator()
+        for bl, _bl_size in self.gf_struct:
             self.h0_loc += C_dag_Op[bl] @ h0_loc_matrix[bl] @ C_Op[bl]
 
-    def set_h_int(self, h_int : OpType) -> None:
+    def set_h_int(self, h_int: OpType) -> None:
         """
-        Sets the interaction terms of the c-electrons in the embedding 
-        Hamiltonian.
-        
+        Set the interaction terms of the c-electrons in the embedding Hamiltonian.
+
         Parameters
         ----------
         h_int : triqs.operators.Operator
             Interaction Hamiltonian in the embedding space.
+
         """
         self.h_int = h_int
-    
-    def set_h_bath(self, Lambda_c : MFType) -> None:
+
+    def set_h_bath(self, Lambda_c: MFType) -> None:
         """
-        Sets the bath terms in the impurity Hamiltonian.
-        
+        Set the bath terms in the impurity Hamiltonian.
+
         Parameters
         ----------
         Lambda_c : dict of ndarray, optional
-            Bath coupling. Each key in dictionary must follow 
+            Bath coupling. Each key in dictionary must follow
             :attr:`gf_struct`.
+
         """
         C_Op = get_C_Op(self.gf_struct_bath, dagger=False)
         C_dag_Op = get_C_Op(self.gf_struct_bath, dagger=True)
-        self.h_bath : OpType = Operator()
-        for bl_bath, bl_bath_size in self.gf_struct_bath:
+        self.h_bath: OpType = Operator()
+        for bl_bath, _bl_bath_size in self.gf_struct_bath:
             bl = self._bl_bath_to_loc(bl_bath)
             self.h_bath += C_Op[bl_bath] @ Lambda_c[bl] @ C_dag_Op[bl_bath]
 
-    def set_h_hybr(self, D : MFType) -> None:
+    def set_h_hybr(self, D: MFType) -> None:
         """
-        Sets the hybridization terms in the impurity Hamiltonian.
-        
+        Set the hybridization terms in the impurity Hamiltonian.
+
         Parameters
         ----------
         D : dict[numpy.ndarray]
-            Hybridization coupling. Each key in dictionary must follow 
+            Hybridization coupling. Each key in dictionary must follow
             :attr:`gf_struct`.
+
         """
         C_Op = get_C_Op(self.gf_struct_bath, dagger=False)
         C_dag_Op = get_C_Op(self.gf_struct, dagger=True)
-        self.h_hybr : OpType = Operator()
-        for bl, loc_size in self.gf_struct:
+        self.h_hybr: OpType = Operator()
+        for bl, _loc_size in self.gf_struct:
             bl_bath = self._bl_loc_to_bath(bl)
             tmp = C_dag_Op[bl] @ D[bl] @ C_Op[bl_bath]
             self.h_hybr += tmp + dagger(tmp)
-        
-    def set_h_emb(self, 
-                  Lambda_c : MFType, 
-                  D : MFType, 
-                  h0_loc_matrix : MFType | None = None,
-                  mu : float | None = None) -> None:
-        """
-        Sets the terms in the impurity Hamiltonian to solve the embedding 
-        problem.
-        
+
+    def set_h_emb(
+        self,
+        Lambda_c: MFType,
+        D: MFType,
+        h0_loc_matrix: MFType | None = None,
+        mu: float | None = None,
+    ) -> None:
+        """
+        Set the terms in the impurity Hamiltonian to solve the embedding problem.
+
         Parameters
         ----------
         Lambda_c : dict[numpy.ndarray]
-            Bath coupling. Each key in dictionary must follow 
+            Bath coupling. Each key in dictionary must follow
             :attr:`gf_struct`.
         D : dict[numpy.ndarray]
-            Hybridization coupling. Each key in dictionary must follow 
+            Hybridization coupling. Each key in dictionary must follow
             :attr:`gf_struct`.
         h0_loc_matrix : dict[numpy.ndarray], optional
-            Single-particle quadratic couplings of the c-electrons. Each key 
+            Single-particle quadratic couplings of the c-electrons. Each key
             in dictionary must follow :attr:`gf_struct`.
+
         """
         if h0_loc_matrix is not None:
             self.set_h0_loc(h0_loc_matrix)
         self.set_h_bath(Lambda_c)
         self.set_h_hybr(D)
 
         # For operators equal is copy, not a view
         self.h_emb = self.h0_loc + self.h_int + self.h_bath + self.h_hybr
 
-        # NOTE h_bath must have + mu*np.eye()*f_a*f_a^dag to remove mu's 
+        # NOTE h_bath must have + mu*np.eye()*f_a*f_a^dag to remove mu's
         # contribution
         if mu is not None:
             for bl, bl_size in self.gf_struct:
                 for alpha in range(bl_size):
-                    self.h_emb -= mu * c_dag(bl,alpha) * c(bl,alpha)
+                    self.h_emb -= mu * c_dag(bl, alpha) * c(bl, alpha)
 
     # TODO other restrictions, like none, for testing
     # but it has been tested against sparse embedding and is the same answer
     # TODO what about superconductivity, ghosts?
     def solve(self) -> None:
-        """
-        Solve for the groundstate in the half-filled number sector of the 
-        embedding problem.
-        """
+        """Solve for the groundstate in the half-filled number sector of the embedding problem."""
         M = int(len(self.fops_emb) / 2)
         # term is an array holding info of term as monomial, last index is its value
         if any(np.iscomplex(term[-1]) for term in self.h_emb):
             self.ad = AtomDiag(self.h_emb, self.fops_emb, n_min=M, n_max=M)
         else:
             self.ad = AtomDiag(self.h_emb.real, self.fops_emb, n_min=M, n_max=M)
         self.gs_vector = self.ad.vacuum_state
         self.gs_vector[0] = 1
 
-    def get_rho_f(self, bl : str) -> np.ndarray:
+    def get_rho_f(self, bl: str) -> np.ndarray:
         """
+        Return f-electron densitym atrix.
+
         Parameters
         ----------
         bl : str
             Which block in :attr:`gf_struct` to return.
 
         Returns
         -------
         numpy.ndarray
             The f-electron density matrix :attr:`rho_f` from impurity.
+
         """
         bl_bath = self._bl_loc_to_bath(bl)
         bl_size = self.gf_struct_bath_dict[bl_bath]
         self.rho_f[bl] = np.zeros([bl_size, bl_size], dtype=complex)
         for a, b in product(range(bl_size), range(bl_size)):
             Op = c(bl_bath, b) * c_dag(bl_bath, a)
-            self.rho_f[bl][a,b] = self.overlap(Op, force_real=False)
+            self.rho_f[bl][a, b] = self.overlap(Op, force_real=False)
         return self.rho_f[bl]
-    
-    def get_rho_c(self, bl : str) -> np.ndarray:
+
+    def get_rho_c(self, bl: str) -> np.ndarray:
         """
+        Return c-electron density matrix.
+
         Parameters
         ----------
         bl : str
             Which block in :attr:`gf_struct` to return.
-        
+
         Returns
         -------
         numpy.ndarray
             The c-electron density matrix :attr:`rho_c` from impurity.
+
         """
         bl_size = self.gf_struct_dict[bl]
         self.rho_c[bl] = np.zeros([bl_size, bl_size], dtype=complex)
         for alpha, beta in product(range(bl_size), range(bl_size)):
             Op = c_dag(bl, alpha) * c(bl, beta)
-            self.rho_c[bl][alpha,beta] = self.overlap(Op, force_real=False)
+            self.rho_c[bl][alpha, beta] = self.overlap(Op, force_real=False)
         return self.rho_c[bl]
-    
-    def get_rho_cf(self, bl : str) -> np.ndarray:
+
+    def get_rho_cf(self, bl: str) -> np.ndarray:
         """
+        Return the cf hybridization (off-diagonal) density matrix.
+
         Parameters
         ----------
         bl : str
             Which block in :attr:`gf_struct` to return.
 
         Returns
         -------
         numpy.ndarray
-            The c,f-electron hybridization density matrix :attr:`rho_cf` from 
+            The c,f-electron hybridization density matrix :attr:`rho_cf` from
             impurity.
+
         """
         bl_bath = self._bl_loc_to_bath(bl)
         bath_size = self.gf_struct_bath_dict[bl_bath]
         loc_size = self.gf_struct_dict[bl]
         self.rho_cf[bl] = np.zeros([loc_size, bath_size], dtype=complex)
         for alpha, a in product(range(loc_size), range(bath_size)):
             Op = c_dag(bl, alpha) * c(bl_bath, a)
-            self.rho_cf[bl][alpha,a] = self.overlap(Op, force_real=False)
+            self.rho_cf[bl][alpha, a] = self.overlap(Op, force_real=False)
         return self.rho_cf[bl]
-    
-    def overlap(self, Op : OpType, force_real : bool = True) -> float | complex:
+
+    def overlap(self, Op: OpType, force_real: bool = True) -> float | complex:
         """
-        Calculate the expectation value of an operator against the ground 
-        state of the embedding problem.
+        Calculate the expectation value of an operator against the ground state of the embedding problem.
 
         Parameters
         ----------
         Op : triqs.operators.Operator
             Operator to take expectation of.
         force_real : bool, optional
             Whether the result should be real or complex.
 
         Returns
         -------
         triqs.operators.Operator
             Expectation value.
+
         """
         res = self.gs_vector @ act(Op, self.gs_vector, self.ad)
         if force_real:
             return res.real
-        else:
-            return res
-            
+        return res
+
     @property
     def gs_energy(self) -> float:
-        """
-        float : Ground state energy of impurity problem.
-        """
-        return self.ad.gs_energy
+        """Return ground state energy of impurity problem."""
+        return self.ad.gs_energy
```

### Comparing `risb-0.1.0/src/risb/kweight/kweight.py` & `risb-0.1.1/src/risb/kweight/kweight.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,130 +11,138 @@
 # GNU General Public License for more details.
 #
 # You may obtain a copy of the License at
 #     https:#www.gnu.org/licenses/gpl-3.0.txt
 #
 # Authors: H. L. Nourse
 
+"""k-space integrator on a grid using smearing functions."""
+
 import numpy as np
 from numpy.typing import ArrayLike
-from .from_triqs_hartree import update_mu, fermi
+
+from .from_triqs_hartree import fermi, update_mu
+
 
 class SmearingKWeight:
     """
     Obtain weights for k-space integrals using smearing functions.
-        
+
     Parameters
     ----------
     beta : float
         Inverse temperature
     mu : float or None, optional
         Chemical potential. One of :attr:`mu` or :attr:`n_target` needs to be provided.
     n_target : float or None, optional
-        Target lattice filling per unit cell. One of :attr:`mu` or :attr:`n_target` 
+        Target lattice filling per unit cell. One of :attr:`mu` or :attr:`n_target`
         needs to be provided.
     method : str, 'fermi' | 'gaussian' | 'methfessel-paxton'
         Smearing method.
+
     """
-    
-    def __init__(self, 
-                 beta: float, 
-                 mu: float | None = None, 
-                 n_target: float | None = None, 
-                 method : str = 'fermi') -> None:
-        
+
+    def __init__(
+        self,
+        beta: float,
+        mu: float | None = None,
+        n_target: float | None = None,
+        method: str = "fermi",
+    ) -> None:
         #: float : Inverse temperature
         self.beta = beta
-        
+
         #: float : Chemical potential.
         self.mu = mu
-        
+
         #: float : Target lattice filling per unit cell.
         self.n_target = n_target
 
         #: dict[numpy.ndarray] : Energies in each band at each k-point.
-        self.energies : dict[ArrayLike]
-        
+        self.energies: dict[ArrayLike]
+
         #: dict[numpy.ndarray] : Integration weights at each k-point in the same shape as energies.
-        self.weight : dict[ArrayLike]
-        
+        self.weight: dict[ArrayLike]
+
         #: int : Number of k-points.
-        self.n_k : int
-        
-        if method == 'fermi':
+        self.n_k: int
+
+        if method == "fermi":
             self.smear_function = self._fermi
-        elif method == 'gaussian':
+        elif method == "gaussian":
             self.smear_function = self._gaussian
-        elif method == 'methfessel-paxton':
+        elif method == "methfessel-paxton":
             self.smear_function = self._methfessel_paxton
         else:
-            raise ValueError('Unrecognized smearing function !')
-        
+            msg = "Unrecognized smearing function !"
+            raise ValueError(msg)
+
     @staticmethod
-    def _fermi(energies : ArrayLike, 
-               beta : float, 
-               mu : float) -> ArrayLike:
+    def _fermi(energies: ArrayLike, beta: float, mu: float) -> ArrayLike:
         e = energies - mu
         return fermi(e, beta)
-    
+
     @staticmethod
-    def _gaussian(energies : ArrayLike, 
-                  beta : float, 
-                  mu : float) -> ArrayLike:
+    def _gaussian(energies: ArrayLike, beta: float, mu: float) -> ArrayLike:
         from scipy.special import erfc
-        return 0.5 * erfc( beta * (energies - mu) )
 
-    @staticmethod    
-    def _methfessel_paxton(energies : ArrayLike, 
-                           beta : float, 
-                           mu : float, 
-                           N : int = 1) -> ArrayLike:
-        from scipy.special import erfc
-        from scipy.special import factorial
-        from scipy.special import hermite
+        return 0.5 * erfc(beta * (energies - mu))
+
+    @staticmethod
+    def _methfessel_paxton(
+        energies: ArrayLike, beta: float, mu: float, N: int = 1
+    ) -> ArrayLike:
+        from scipy.special import erfc, factorial, hermite
+
         def A_n(n):
-            return (-1)**n / ( factorial(n) * 4**n * np.sqrt(np.pi) )
-        
+            return (-1) ** n / (factorial(n) * 4**n * np.sqrt(np.pi))
+
         x = beta * (energies - mu)
-        
-        S = 0.5 * erfc(x) # S_0
-        for n in range(1,N+1):
-            H_n = hermite(2*n-1)
-            S += A_n(n) * H_n(x) * np.exp(-x**2)
+
+        S = 0.5 * erfc(x)  # S_0
+        for n in range(1, N + 1):
+            H_n = hermite(2 * n - 1)
+            S += A_n(n) * H_n(x) * np.exp(-(x**2))
         return S
-    
+
     def _update_n_k(self) -> int:
         if isinstance(self.energies, dict):
             first_key = next(iter(self.energies))
             self.n_k = self.energies[first_key].shape[0]
             for en in self.energies.values():
                 if self.n_k != en.shape[0]:
                     # FIXME Must they? I don't see why, but its weird to not
-                    raise ValueError('Blocks must be on the same sized grid !')
+                    msg = "Blocks must be on the same sized grid !"
+                    raise ValueError(msg)
         else:
             self.n_k = self.energies.shape[0]
         return self.n_k
-    
-    def update_weights(self, energies : dict[ArrayLike]) -> dict[ArrayLike]:
+
+    def update_weights(self, energies: dict[ArrayLike]) -> dict[ArrayLike]:
         """
         Update the integral weighting factors at each k-point.
 
         Parameters
         ----------
         energies : dict[numpy.ndarray]
             Energies at each k-point. Each key in dictionary is a different
             symmetry block, and its associated value is a list of energies.
-        
+
         Returns
         -------
         dict[numpy.ndarray]
             Integration weights at each k-point in each band.
+
         """
         self.energies = energies
         self._update_n_k()
         if self.n_target is not None:
-            self.mu = update_mu(self.n_target, self.energies, self.beta, self.n_k, self.smear_function)
+            self.mu = update_mu(
+                self.n_target, self.energies, self.beta, self.n_k, self.smear_function
+            )
 
-        self.weights = dict()
+        self.weights = {}
         for bl in self.energies:
-            self.weights[bl] = self.smear_function(self.energies[bl], self.beta, self.mu) / self.n_k
-        return self.weights 
+            self.weights[bl] = (
+                self.smear_function(self.energies[bl], self.beta, self.mu) / self.n_k
+            )
+        return self.weights
```

### Comparing `risb-0.1.0/src/risb/optimize/diis.py` & `risb-0.1.1/src/risb/optimize/diis.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,84 +11,85 @@
 # GNU General Public License for more details.
 #
 # You may obtain a copy of the License at
 #     https:#www.gnu.org/licenses/gpl-3.0.txt
 #
 # Authors: H. L. Nourse
 
+"""DIIS optimizers."""
+
 import numpy as np
 import scipy
 from numpy.typing import ArrayLike
-from . import NewtonSolver
+
+from .solver_newton import NewtonSolver
+
 
 class DIIS(NewtonSolver):
-    '''
+    """
     Direct inversion in the iterative subspace to minimize a function.
-    
+
     Parameters
     ----------
     n_period : int, optional
-        Take a single linear mixing step afer this many iterations. Default 
+        Take a single linear mixing step afer this many iterations. Default
         round(history_size / 2).
 
     Notes
     -----
     Algorithm 2 (Anderson type) in `10.1051/m2an/2021069 <hal-02492983v5_>`__.
 
     .. _hal-02492983v5: https://doi.org/10.1051/m2an/2021069
-    '''
-    def __init__(self, /, 
-                 n_period : int = 0, 
-                 **kwargs) -> None:
+
+    """
+
+    def __init__(self, /, n_period: int = 0, **kwargs) -> None:
         super().__init__(**kwargs)
-        
+
         if n_period == 0:
-            self.n_period = int(np.round(self.history_size/2.0))
+            self.n_period = int(np.round(self.history_size / 2.0))
         else:
             self.n_period = n_period
 
         self.solve = super().solve
 
     @staticmethod
-    def extrapolate(x : list[ArrayLike], 
-                    g_x : list[ArrayLike], 
-                    error : list[ArrayLike]) -> np.ndarray:
-        """
-        The DIIS extrapolation algorithm for the new guess for :attr:`x`.
-        """
-        
+    def extrapolate(
+        x: list[ArrayLike], g_x: list[ArrayLike], error: list[ArrayLike]
+    ) -> np.ndarray:
+        """DIIS extrapolation algorithm for the new guess for :attr:`x`."""
         # Construct the B matrix
         m = len(error)
-        B = np.empty(shape=(m,m))
+        B = np.empty(shape=(m, m))
         for i in range(m):
             for j in range(m):
-                B[i,j] = np.dot(error[i], error[j])
+                B[i, j] = np.dot(error[i], error[j])
 
         # Add the constraint lambda
-        B = np.column_stack( ( B, -np.ones(B.shape[0]) ) )
-        B = np.vstack( ( B, -np.ones(B.shape[1]) ) )
-        B[m,m] = 0.
-            
+        B = np.column_stack((B, -np.ones(B.shape[0])))
+        B = np.vstack((B, -np.ones(B.shape[1])))
+        B[m, m] = 0.0
+
         # Solve for the c coefficients (last element in c gives lambda constraint)
         rhs = np.zeros(B.shape[0])
-        rhs[-1] = -1.
-        
+        rhs[-1] = -1.0
+
         c = np.dot(scipy.linalg.pinv(B), rhs)
-        
+
         # Calculate optimal x(n)
         x_opt = np.zeros(x[0].shape)
         for i in range(m):
             x_opt += c[i] * g_x[i]
         return x_opt
 
-    # x_i, error(x_i), g(x_i) where g(x_i) is the fixed-point function 
+    # x_i, error(x_i), g(x_i) where g(x_i) is the fixed-point function
     # that gives a new x_i
-    def update_x(self, alpha : float = 1.0) -> np.ndarray:
-                
-        if ((self.n+1) % self.n_period == 0):
+    def update_x(self, alpha: float = 1.0) -> np.ndarray:
+        """Return a new guess for the vector x."""
+        if (self.n + 1) % self.n_period == 0:
             # Do linear mixing
-            x_opt = self.x[0] + alpha*(self.g_x[0] - self.x[0])
+            x_opt = self.x[0] + alpha * (self.g_x[0] - self.x[0])
         else:
             # Do DIIS
             x_opt = self.extrapolate(self.x, self.g_x, self.error)
 
-        return x_opt
+        return x_opt
```

### Comparing `risb-0.1.0/src/risb/optimize/solver_newton.py` & `risb-0.1.1/src/risb/optimize/solver_newton.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,179 +11,180 @@
 # GNU General Public License for more details.
 #
 # You may obtain a copy of the License at
 #     https:#www.gnu.org/licenses/gpl-3.0.txt
 #
 # Authors: H. L. Nourse
 
+"""Abstract base class for quasi-Newton methods."""
+
+import logging
+from abc import ABC, abstractmethod
+from collections.abc import Callable
 from copy import deepcopy
+from typing import Any
+
 import numpy as np
-from abc import ABC, abstractmethod
-from typing import Any, Callable
 from numpy.typing import ArrayLike
 
+logger = logging.getLogger(__name__)
+
+
 # TODO fix up verbose messages
 class NewtonSolver(ABC):
     """
     Base class for quasi-Newton methods to find the root of a function.
 
     Parameters
     ----------
     history_size : int, optional
         Maximum size of subspace.
     n_restart : int, optional
         Fully reset subspace after this many iterations.
-    verbose : bool, optional
-        Whether to report information during optimization.
-    
+
     Notes
     -----
     :meth:`update_x` must be defined in the inherited class.
+
     """
-    def __init__(self, 
-                 history_size : int = 6, 
-                 n_restart : float = np.inf, 
-                 verbose : bool = False) -> None:
 
+    def __init__(self, history_size: int = 6, n_restart: float = np.inf) -> None:
         self.history_size = history_size
         self.n_restart = n_restart
-        self.verbose = verbose
         self.initialized = False
 
         #: list[numpy.ndarray] : History of guesses to the root problem.
-        self.x : list[ArrayLike] = []
+        self.x: list[ArrayLike] = []
 
         #: list[numpy.ndarray] : History of fixed point function with ``x`` as the input.
-        self.g_x : list[ArrayLike] = [] 
+        self.g_x: list[ArrayLike] = []
 
         #: list[numpy.ndarray] : History of error vector of ``x``.
-        self.error : list[ArrayLike] = []
+        self.error: list[ArrayLike] = []
 
         #: int : Iteration counter for solver.
-        self.n : int = 0
-        
+        self.n: int = 0
+
         #: bool : Whether the solver converged to within tolerance.
-        self.success : bool = False
-        
+        self.success: bool = False
+
         # float : 2-norm of :attr:`error`.
-        self.norm : float = np.inf
+        self.norm: float = np.inf
 
     @staticmethod
-    def _load_history(x : list[ArrayLike], 
-                      error : list[ArrayLike], 
-                      max_size : int) -> tuple[ list[ArrayLike], list[ArrayLike] ]:
-
+    def _load_history(
+        x: list[ArrayLike], error: list[ArrayLike], max_size: int
+    ) -> tuple[list[ArrayLike], list[ArrayLike]]:
         if (len(x) != len(error)) and (len(x) != (len(error) + 1)):
-            raise ValueError('x and error are the wrong lengths !')
+            msg = "x and error are the wrong lengths !"
+            raise ValueError(msg)
 
         x_out = deepcopy(x)
         error_out = deepcopy(error)
 
         while len(x_out) >= max_size:
             x_out.pop()
         while len(error_out) >= max_size:
             error_out.pop()
 
         return x_out, error_out
 
     @staticmethod
-    def _insert_vector(vec : list[ArrayLike], 
-                       vec_new : ArrayLike, 
-                       max_size : int | None = None) -> None:
-
+    def _insert_vector(
+        vec: list[ArrayLike], vec_new: ArrayLike, max_size: int | None = None
+    ) -> None:
         # Note these operations are mutable on input list
         vec.insert(0, vec_new)
-        if max_size is not None:
-            if len(vec) >= max_size:
-                vec.pop()
-    
+        if max_size is not None and len(vec) >= max_size:
+            vec.pop()
+
     @abstractmethod
-    def update_x(self, 
-                 **kwargs) -> np.ndarray:
+    def update_x(self, **kwargs) -> np.ndarray:
         """
-        A single iteration for the new guess for :attr:`x`.
-        
+        Return a single iteration for the new guess for :attr:`x`.
+
         Parameters
         ----------
         **kwargs : dict
             Keyword arguments specific to the solver implementation.
 
         Returns
         -------
         numpy.ndarray
             New guess for x to add to history.
+
         """
-        pass
 
-    def solve(self, 
-              fun : Callable[..., ArrayLike],
-              x0 : ArrayLike, 
-              args : tuple[Any, ...] = (), 
-              tol : float = 1e-12, 
-              maxiter : int = 1000,
-              options : dict = {}) -> ArrayLike:
+    def solve(
+        self,
+        fun: Callable[..., ArrayLike],
+        x0: ArrayLike,
+        args: tuple[Any, ...] = (),
+        tol: float = 1e-12,
+        maxiter: int = 1000,
+        options: dict | None = None,
+    ) -> ArrayLike:
         """
-        Find the root of a function. It is called similarly to 
-        :func:scipy.optimize.root
+        Find the root of a function. It is called similarly to :func:scipy.optimize.root.
 
         Parameters
         ----------
-
         fun : callable
-            The function to find the root of. It must be callable as 
+            The function to find the root of. It must be callable as
             ``fun(x, *args)``.
         x0 : numpy.ndarray
-            Initial guess of the parameters. This does not neccessarily have to 
+            Initial guess of the parameters. This does not neccessarily have to
             be flattened, but it usually is.
         args : tuple, optional
             Additional arguments to pass to ``fun``.
         tol : float, optional
-            The tolerance. When the 2-norm difference of the return of ``fun`` 
+            The tolerance. When the 2-norm difference of the return of ``fun``
             is less than this, the solver stops.
         maxiter : int, optional
             Maximum number of iterations.
         options : dict, optional
             keyword arguments to pass to :meth:`update_x`.
-        
+
         Returns
         -------
         numpy.ndarray
             Root of ``fun``.
-        """
 
+        """
+        if options is None:
+            options = {}
         self.success = False
         x = deepcopy(x0)
         if self.history_size > 0:
             self._insert_vector(self.x, x, self.history_size)
 
         for self.n in range(maxiter):
-        
             g_x, error = fun(x, *args)
-            
+
             if self.history_size > 0:
                 self._insert_vector(self.g_x, g_x, self.history_size)
                 self._insert_vector(self.error, error, self.history_size)
 
             self.norm = np.linalg.norm(error)
-            if self.verbose:
-                print(f"n: {self.n}, rms(risb): {self.norm}")
+            logger.info(f"n: {self.n}, rms(risb): {self.norm}")
             if self.norm < tol:
                 self.success = True
                 break
 
             x = self.update_x(**options)
-                            
+
             if (self.n % self.n_restart) == 0:
                 self.x = []
                 self.g_x = []
                 self.error = []
-            
-            if self.history_size > 0: 
+
+            if self.history_size > 0:
                 self._insert_vector(self.x, x, self.history_size)
-                    
-        if self.verbose:
-            if self.success:
-                print(f"The solution converged. nit: {self.n}, tol: {self.norm}")
-            else:
-                print(f"The solution did NOT converge. nit: {self.n} tol: {self.norm}")
-        
-        return x
+
+        if self.success:
+            logger.info(f"The solution converged. nit: {self.n}, tol: {self.norm}")
+        else:
+            logger.info(
+                f"The solution did NOT converge. nit: {self.n} tol: {self.norm}"
+            )
+
+        return x
```

### Comparing `risb-0.1.0/tests/data_helpers.h5` & `risb-0.1.1/tests/data_helpers.h5`

 * *Files identical despite different names*

### Comparing `risb-0.1.0/tests/test_atomdiag.py` & `risb-0.1.1/tests/test_atomdiag.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,171 +1,254 @@
-import numpy as np
+# ruff: noqa: T201, D100, D103
 from itertools import product
+
+import numpy as np
 import pytest
-from pytest import approx
+from triqs.operators import Operator, c, c_dag, n
+from triqs.operators.util.observables import N_op, S2_op
 
 from risb.embedding import EmbeddingAtomDiag
-from triqs.operators import Operator, n, c_dag, c
-from triqs.operators.util.observables import S2_op, N_op
 
-def do_assert(subtests, rho_f, rho_cf, rho_c, gs_energy, N, S2, 
-              rho_f_expected, rho_cf_expected, rho_c_expected, gs_energy_expected, N_expected, S2_expected):
+
+def do_assert(
+    subtests,
+    rho_f,
+    rho_cf,
+    rho_c,
+    gs_energy,
+    N,
+    S2,
+    rho_f_expected,
+    rho_cf_expected,
+    rho_c_expected,
+    gs_energy_expected,
+    N_expected,
+    S2_expected,
+):
     abs = 1e-12
     with subtests.test(msg="rho_f"):
-        for bl in rho_f.keys():
-            assert rho_f[bl] == approx(rho_f_expected, abs=abs)
+        for bl in rho_f:
+            assert rho_f[bl] == pytest.approx(rho_f_expected, abs=abs)
     with subtests.test(msg="rho_cf"):
-        for bl in rho_cf.keys():
-            assert rho_cf[bl] == approx(rho_cf_expected, abs=abs)
+        for bl in rho_cf:
+            assert rho_cf[bl] == pytest.approx(rho_cf_expected, abs=abs)
     with subtests.test(msg="rho_c"):
-        for bl in rho_c.keys():
-            assert rho_c[bl] == approx(rho_c_expected, abs=abs)
+        for bl in rho_c:
+            assert rho_c[bl] == pytest.approx(rho_c_expected, abs=abs)
     with subtests.test(msg="gs_energy"):
-        assert gs_energy == approx(gs_energy_expected, abs=abs)
+        assert gs_energy == pytest.approx(gs_energy_expected, abs=abs)
     with subtests.test(msg="N"):
-        assert N == approx(N_expected, abs=abs)
+        assert pytest.approx(N_expected, abs=abs) == N
     with subtests.test(ms="S2"):
-        assert S2 == approx(S2_expected, abs=abs)
+        assert pytest.approx(S2_expected, abs=abs) == S2
 
-@pytest.fixture
+
+@pytest.fixture()
 def one_band():
     U = 1
-    mu = U / 2.0 # half-filling
+    mu = U / 2.0  # half-filling
     n_orb = 1
-    spin_names = ['up', 'dn']
-    h_int = U * n('up', 0) * n('dn', 0)
-    Lambda_c = dict()
-    D = dict()
-    h0_loc_mat = dict()
+    spin_names = ["up", "dn"]
+    h_int = U * n("up", 0) * n("dn", 0)
+    Lambda_c = {}
+    D = {}
+    h0_loc_mat = {}
     for bl in spin_names:
-        Lambda_c[bl] = np.array([ [ -mu ] ])
-        D[bl] = np.array([ [ -0.3333 ] ])
-        h0_loc_mat[bl] = np.array([ [ 0 ] ])
+        Lambda_c[bl] = np.array([[-mu]])
+        D[bl] = np.array([[-0.3333]])
+        h0_loc_mat[bl] = np.array([[0]])
     return spin_names, n_orb, Lambda_c, D, h0_loc_mat, h_int
 
-@pytest.fixture
+
+@pytest.fixture()
 def one_band_expected():
     rho_f_expected = np.array([[0.5]])
     rho_cf_expected = np.array([[0.4681588161332029]])
     rho_c_expected = np.array([[0.5]])
     gs_energy_expected = -0.9619378905494498
     N_expected = 1.0
     S2_expected = 0.5066828353209953
-    return rho_f_expected, rho_cf_expected, rho_c_expected, gs_energy_expected, N_expected, S2_expected
+    return (
+        rho_f_expected,
+        rho_cf_expected,
+        rho_c_expected,
+        gs_energy_expected,
+        N_expected,
+        S2_expected,
+    )
+
 
-@pytest.fixture
+@pytest.fixture()
 def bilayer():
     U = 1
     V = 0.25
     J = 0
-    mu = U / 2.0 # half-filling
+    mu = U / 2.0  # half-filling
     n_orb = 2
-    spin_names = ['up','dn']
+    spin_names = ["up", "dn"]
     h_int = Operator()
     for o in range(n_orb):
-        h_int += U * n("up",o) * n("dn",o)
-    for s1,s2 in product(spin_names,spin_names):
-        h_int += 0.5 * J * c_dag(s1,0) * c(s2,0) * c_dag(s2,1) * c(s1,1)
-    Lambda_c = dict()
-    D = dict()
-    h0_loc_mat = dict()
+        h_int += U * n("up", o) * n("dn", o)
+    for s1, s2 in product(spin_names, spin_names):
+        h_int += 0.5 * J * c_dag(s1, 0) * c(s2, 0) * c_dag(s2, 1) * c(s1, 1)
+    Lambda_c = {}
+    D = {}
+    h0_loc_mat = {}
     for bl in spin_names:
-        Lambda_c[bl] = np.array([ [ -mu        , -0.00460398 ],
-                                  [-0.00460398, -mu         ] ])
-        D[bl] = np.array([ [ -2.59694448e-01, 0               ],
-                           [ 0              , -2.59694448e-01 ] ])
-        h0_loc_mat[bl] = np.array([ [ 0, V ],
-                                    [ V, 0 ] ] )
+        Lambda_c[bl] = np.array([[-mu, -0.00460398], [-0.00460398, -mu]])
+        D[bl] = np.array([[-2.59694448e-01, 0], [0, -2.59694448e-01]])
+        h0_loc_mat[bl] = np.array([[0, V], [V, 0]])
     return spin_names, n_orb, Lambda_c, D, h0_loc_mat, h_int
 
-@pytest.fixture
+
+@pytest.fixture()
 def bilayer_expected():
-    rho_f_expected = np.array([ [ 0.5                , -0.1999913941210893 ],
-                                [ -0.1999913941210893, 0.5                 ] ])
-    rho_cf_expected = np.array([ [ 0.42326519677453511, 0                   ],
-                                 [ 0,                   0.42326519677453511 ] ])
-    rho_c_expected = np.array([ [ 0.5                , -0.1836332097072352 ],
-                                [ -0.1836332097072352, 0.5                 ] ])
+    rho_f_expected = np.array([[0.5, -0.1999913941210893], [-0.1999913941210893, 0.5]])
+    rho_cf_expected = np.array([[0.42326519677453511, 0], [0, 0.42326519677453511]])
+    rho_c_expected = np.array([[0.5, -0.1836332097072352], [-0.1836332097072352, 0.5]])
     gs_energy_expected = -1.7429249197415944
     N_expected = 2.0
     S2_expected = 0.8247577338845973
-    return rho_f_expected, rho_cf_expected, rho_c_expected, gs_energy_expected, N_expected, S2_expected
+    return (
+        rho_f_expected,
+        rho_cf_expected,
+        rho_c_expected,
+        gs_energy_expected,
+        N_expected,
+        S2_expected,
+    )
+
 
-@pytest.fixture
+@pytest.fixture()
 def dh_trimer():
     # At two-thirds filling
     U = 1
     tk = 1
     n_orb = 3
-    spin_names = ['up','dn']
-    def hubb_N(tk, U, n_orb, spin_names):
+    spin_names = ["up", "dn"]
+
+    def hubb_N(tk, U, n_orb, spin_names):  # noqa: ARG001
         # hopping
-        #phi = 2.0 * np.pi / n_orb
-        #for a,m,mm,s in product(range(n_orb),range(n_orb),range(n_orb), spin_names):
+        # phi = 2.0 * np.pi / n_orb
+        # for a,m,mm,s in product(range(n_orb),range(n_orb),range(n_orb), spin_names):
         #    h0_loc += (-tk / n_orb) * c_dag(s,m) * c(s,mm) * np.exp(-1j * phi * a * m) * np.exp(1j * phi * np.mod(a+1,n_orb) * mm)
         #    h0_loc += (-tk / n_orb) * c_dag(s,m) * c(s,mm) * np.exp(-1j * phi * np.mod(a+1,n_orb) * m) * np.exp(1j * phi * a * mm)
         # hubbard U
         h_int = Operator()
-        for m,mm,mmm in product(range(n_orb),range(n_orb),range(n_orb)):
-            h_int += (U / n_orb) * c_dag("up",m) * c("up",mm) * c_dag("dn",mmm) * c("dn",np.mod(m+mmm-mm,n_orb))
+        for m, mm, mmm in product(range(n_orb), range(n_orb), range(n_orb)):
+            h_int += (
+                (U / n_orb)
+                * c_dag("up", m)
+                * c("up", mm)
+                * c_dag("dn", mmm)
+                * c("dn", np.mod(m + mmm - mm, n_orb))
+            )
         return h_int.real
+
     h_int = hubb_N(tk, U, n_orb, spin_names)
-    Lambda_c = dict()
-    D = dict()
+    Lambda_c = {}
+    D = {}
     h0_loc_mat = {bl: np.zeros([n_orb, n_orb]) for bl in spin_names}
     for bl in spin_names:
-        Lambda_c[bl] = np.array([ [ -1.91730088, -0.        , -0.         ],
-                                  [ -0.        , -1.69005946, -0.         ],
-                                  [ -0.        , -0.        , -1.69005946 ] ])
-        D[bl] = np.array([ [ -0.26504931,  0.        ,  0.        ],
-                           [ 0.        , -0.39631238,  0.         ],
-                           [ 0.        ,  0.        , -0.39631238 ] ])
-        h0_loc_mat[bl][0,0] = -2 * tk
-        h0_loc_mat[bl][1,1] = tk
-        h0_loc_mat[bl][2,2] = tk
+        Lambda_c[bl] = np.array(
+            [
+                [-1.91730088, -0.0, -0.0],
+                [-0.0, -1.69005946, -0.0],
+                [-0.0, -0.0, -1.69005946],
+            ]
+        )
+        D[bl] = np.array(
+            [[-0.26504931, 0.0, 0.0], [0.0, -0.39631238, 0.0], [0.0, 0.0, -0.39631238]]
+        )
+        h0_loc_mat[bl][0, 0] = -2 * tk
+        h0_loc_mat[bl][1, 1] = tk
+        h0_loc_mat[bl][2, 2] = tk
     return spin_names, n_orb, Lambda_c, D, h0_loc_mat, h_int
 
-@pytest.fixture
+
+@pytest.fixture()
 def dh_trimer_expected():
-    rho_f_expected = np.array([ [ 0.9932309740187902, 0.                , 0.                 ],
-                                [ 0.                , 0.5033842231804342, 0.                 ],
-                                [ 0.                , 0.                , 0.5033842231804342 ] ])
-    rho_cf_expected = np.array([ [ 0.0811187181751014, 0.                , 0.                 ],
-                                 [ 0.                , 0.4910360103357626, 0.                 ],
-                                 [ 0.                , 0.                , 0.4910360103357626 ] ])
-    rho_c_expected = np.array([ [ 0.9909259681893234, 0.                , 0.                ],
-                                [ 0.                , 0.5045367260951683, 0.                ],
-                                [ 0.                , 0.                , 0.5045367260951683] ])
+    rho_f_expected = np.array(
+        [
+            [0.9932309740187902, 0.0, 0.0],
+            [0.0, 0.5033842231804342, 0.0],
+            [0.0, 0.0, 0.5033842231804342],
+        ]
+    )
+    rho_cf_expected = np.array(
+        [
+            [0.0811187181751014, 0.0, 0.0],
+            [0.0, 0.4910360103357626, 0.0],
+            [0.0, 0.0, 0.4910360103357626],
+        ]
+    )
+    rho_c_expected = np.array(
+        [
+            [0.9909259681893234, 0.0, 0.0],
+            [0.0, 0.5045367260951683, 0.0],
+            [0.0, 0.0, 0.5045367260951683],
+        ]
+    )
     gs_energy_expected = -9.555511743344764
     N_expected = 3.99999884075932
     S2_expected = 0.9171025003755656
-    return rho_f_expected, rho_cf_expected, rho_c_expected, gs_energy_expected, N_expected, S2_expected
-
-
-@pytest.mark.parametrize('model, model_expected', [
-    ('one_band', 'one_band_expected'),
-    ('bilayer', 'bilayer_expected'),
-    ('dh_trimer', 'dh_trimer_expected'),
-])
+    return (
+        rho_f_expected,
+        rho_cf_expected,
+        rho_c_expected,
+        gs_energy_expected,
+        N_expected,
+        S2_expected,
+    )
+
+
+@pytest.mark.parametrize(
+    ("model", "model_expected"),
+    [
+        ("one_band", "one_band_expected"),
+        ("bilayer", "bilayer_expected"),
+        ("dh_trimer", "dh_trimer_expected"),
+    ],
+)
 def test_solve(subtests, request, model, model_expected):
     model = request.getfixturevalue(model)
     model_expected = request.getfixturevalue(model_expected)
     spin_names, n_orb, Lambda_c, D, h0_loc_mat, h_int = model
-    rho_f_expected, rho_cf_expected, rho_c_expected, gs_energy_expected, N_expected, S2_expected = model_expected
-    gf_struct = [ (bl, n_orb) for bl in spin_names ]
+    (
+        rho_f_expected,
+        rho_cf_expected,
+        rho_c_expected,
+        gs_energy_expected,
+        N_expected,
+        S2_expected,
+    ) = model_expected
+    gf_struct = [(bl, n_orb) for bl in spin_names]
     embedding = EmbeddingAtomDiag(h_int, gf_struct)
     embedding.set_h_emb(Lambda_c, D, h0_loc_mat)
     embedding.solve()
-    rho_f = dict()
-    rho_cf = dict()
-    rho_c = dict()
-    for bl, bl_size in gf_struct:
+    rho_f = {}
+    rho_cf = {}
+    rho_c = {}
+    for bl, _bl_size in gf_struct:
         rho_f[bl] = embedding.get_rho_f(bl)
         rho_cf[bl] = embedding.get_rho_cf(bl)
         rho_c[bl] = embedding.get_rho_c(bl)
     gs_energy = embedding.gs_energy
     NOp = N_op(spin_names, n_orb, off_diag=True)
     S2Op = S2_op(spin_names, n_orb, off_diag=True)
     N = embedding.overlap(NOp)
     S2 = embedding.overlap(S2Op)
-    do_assert(subtests, rho_f, rho_cf, rho_c, gs_energy, N, S2, 
-              rho_f_expected, rho_cf_expected, rho_c_expected, gs_energy_expected, N_expected, S2_expected)
+    do_assert(
+        subtests,
+        rho_f,
+        rho_cf,
+        rho_c,
+        gs_energy,
+        N,
+        S2,
+        rho_f_expected,
+        rho_cf_expected,
+        rho_c_expected,
+        gs_energy_expected,
+        N_expected,
+        S2_expected,
+    )
```

### Comparing `risb-0.1.0/tests/test_helpers.py` & `risb-0.1.1/tests/test_helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,101 +1,105 @@
-#!/usr/bin/env python
+# ruff: noqa: T201, D100, D103
+
+from pathlib import Path
 
-import os
-import numpy as np
-from pytest import approx
 import h5py
+import numpy as np
+import pytest
+
 from risb import helpers
 
 # FIXME finish helpers: lambda, r, f1, f2
 
 abs = 1e-12
-helpers_filename = os.path.dirname(__file__) + "/" "/data_helpers.h5"
+helpers_filename = Path(__file__).parent / Path("data_helpers.h5")
+
 
 def test_get_h_qp(subtests):
     with h5py.File(helpers_filename, "r") as f:
-        h0_k = f['h0_k'][:]
-        eig_expected = f['eig'][:]
-        vec_expected = f['vec'][:]
-    R = np.zeros(shape=(2,2))
+        h0_k = f["h0_k"][:]
+        eig_expected = f["eig"][:]
+        vec_expected = f["vec"][:]
+    R = np.zeros(shape=(2, 2))
     np.fill_diagonal(R, 1)
-    Lambda = np.zeros(shape=(2,2))
+    Lambda = np.zeros(shape=(2, 2))
     np.fill_diagonal(Lambda, 0.5)
     h_qp = helpers.get_h_qp(R, Lambda, h0_k)
     eig, vec = np.linalg.eigh(h_qp)
     with subtests.test(msg="eigenvalues"):
-        assert eig == approx(eig_expected, abs=abs)
+        assert eig == pytest.approx(eig_expected, abs=abs)
     with subtests.test(msg="eigenvectors"):
-        assert vec == approx(vec_expected, abs=abs)
+        assert vec == pytest.approx(vec_expected, abs=abs)
+
 
 def test_get_h0_kin_k_R():
-    R = np.zeros(shape=(2,2))
+    R = np.zeros(shape=(2, 2))
     np.fill_diagonal(R, 1)
     with h5py.File(helpers_filename, "r") as f:
-        h0_k = f['h0_k'][:]
-        vec = f['vec'][:]
-        h0_k_R_expected = f['h0_R'][:]    
+        h0_k = f["h0_k"][:]
+        vec = f["vec"][:]
+        h0_k_R_expected = f["h0_R"][:]
     h0_k_R = helpers.get_h0_kin_k_R(R, h0_k, vec)
-    assert h0_k_R == approx(h0_k_R_expected, abs=abs)
-    
+    assert h0_k_R == pytest.approx(h0_k_R_expected, abs=abs)
+
+
 def test_get_ke():
     with h5py.File(helpers_filename, "r") as f:
-        h0_k_R = f['h0_R'][:]
-        vec = f['vec'][:]
-        wks = f['wks'][:]    
-    ke = helpers.get_ke(h0_k_R, vec, wks)    
-    ke_expected = np.array([ [ -0.36035732126514364, 0                    ],
-                             [ 0                   , -0.36035732126514364 ] ])
-    assert ke == approx(ke_expected, abs=abs)
-    
+        h0_k_R = f["h0_R"][:]
+        vec = f["vec"][:]
+        wks = f["wks"][:]
+    ke = helpers.get_ke(h0_k_R, vec, wks)
+    ke_expected = np.array([[-0.36035732126514364, 0], [0, -0.36035732126514364]])
+    assert ke == pytest.approx(ke_expected, abs=abs)
+
+
 def test_get_rho_qp():
     with h5py.File(helpers_filename, "r") as f:
-        vec = f['vec'][:]
-        wks = f['wks'][:]
+        vec = f["vec"][:]
+        wks = f["wks"][:]
     rho_qp = helpers.get_rho_qp(vec, wks)
-    rho_qp_expected = np.array([ [ 0.30667105643085796, 0                   ],
-                                 [ 0                  , 0.30667105643085796 ] ])
-    assert rho_qp == approx(rho_qp_expected, abs=abs)
+    rho_qp_expected = np.array([[0.30667105643085796, 0], [0, 0.30667105643085796]])
+    assert rho_qp == pytest.approx(rho_qp_expected, abs=abs)
+
 
 def test_get_d():
-    rho_qp = np.array([ [ 0.19618454, 0.         ],
-                        [ 0.        , 0.19618454 ] ])
-    ke = np.array([ [ -0.13447044,  0.        ],
-                    [ 0.        , -0.13447044 ] ])
+    rho_qp = np.array([[0.19618454, 0.0], [0.0, 0.19618454]])
+    ke = np.array([[-0.13447044, 0.0], [0.0, -0.13447044]])
     D = helpers.get_d(rho_qp, ke)
-    D_expected = np.array([ [ -0.33862284815908383,  0.                  ],
-                            [ 0.                  , -0.33862284815908383 ] ])
-    assert D == approx(D_expected, abs=abs)
-        
-def test_get_lambda_c(): 
-    Lambda = np.array([ [ 0.5, 0.  ],
-                        [ 0. , 0.5 ] ])
-    R = np.array([ [ 1., 0. ],
-                   [ 0., 1. ] ])
-    rho_qp = np.array([ [ 0.19618454, 0.         ],
-                        [ 0.        , 0.19618454 ] ])
-    D = np.array([ [ -0.33862285,  0.         ],
-                   [  0.        , -0.33862285 ] ])
+    D_expected = np.array([[-0.33862284815908383, 0.0], [0.0, -0.33862284815908383]])
+    assert pytest.approx(D_expected, abs=abs) == D
+
+
+def test_get_lambda_c():
+    Lambda = np.array([[0.5, 0.0], [0.0, 0.5]])
+    R = np.array([[1.0, 0.0], [0.0, 1.0]])
+    rho_qp = np.array([[0.19618454, 0.0], [0.0, 0.19618454]])
+    D = np.array([[-0.33862285, 0.0], [0.0, -0.33862285]])
     Lambda_c = helpers.get_lambda_c(rho_qp, R, Lambda, D)
-    Lambda_c_expected = np.array([ [ 0.018138135818154377, 0.                   ],
-                                   [ 0.                  , 0.018138135818154377 ] ])
-    assert Lambda_c == approx(Lambda_c_expected, abs=abs)
+    Lambda_c_expected = np.array(
+        [[0.018138135818154377, 0.0], [0.0, 0.018138135818154377]]
+    )
+    assert Lambda_c == pytest.approx(Lambda_c_expected, abs=abs)
+
 
 def test_get_lambda():
-    #R = np.zeros(shape=(2,2))
-    #np.fill_diagonal(R, 1.0)
-    #Lambda = helpers.get_lambda(R, D, Lambda_c, rho_f) 
+    # R = np.zeros(shape=(2,2))
+    # np.fill_diagonal(R, 1.0)
+    # Lambda = helpers.get_lambda(R, D, Lambda_c, rho_f)
     pass
 
+
 def test_get_R():
-    #R = helpers.get_r(rho_cf, rho_f)
+    # R = helpers.get_r(rho_cf, rho_f)
     pass
 
+
 def test_get_f1():
-    #R = np.zeros(shape=(2,2))
-    #np.fill_diagonal(R, 1.0)
-    #f1 = helpers.get_f1(rho_cf, rho_qp, R)
+    # R = np.zeros(shape=(2,2))
+    # np.fill_diagonal(R, 1.0)
+    # f1 = helpers.get_f1(rho_cf, rho_qp, R)
     pass
 
+
 def test_get_f2():
-    #f2 = helpers.get_f2(rho_f, rho_qp)
-    pass
+    # f2 = helpers.get_f2(rho_f, rho_qp)
+    pass
```

### Comparing `risb-0.1.0/tests/test_latticesolver.py` & `risb-0.1.1/tests/test_latticesolver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,162 +1,188 @@
-#!/usr/bin/env python
+# ruff: noqa: T201, D100, D103
+
 
 import numpy as np
-from itertools import product
 import pytest
-from pytest import approx
-
-from common import build_cubic_h0_k, symmetrize_blocks
-from triqs.operators import Operator, c_dag, c, n
+from test_common import build_cubic_h0_k, symmetrize_blocks
+from triqs.operators import Operator, n
 from triqs.operators.util.hamiltonians import h_int_kanamori
 from triqs.operators.util.op_struct import set_operator_structure
+
 from risb import LatticeSolver
-from risb.kweight import SmearingKWeight
 from risb.embedding import EmbeddingAtomDiag
+from risb.kweight import SmearingKWeight
 
 # FIXME add one_shot test
 
-def do_assert(subtests, mu, Lambda, Z, 
-              mu_expected, Lambda_expected, Z_expected):
+
+def do_assert(subtests, mu, Lambda, Z, mu_expected, Lambda_expected, Z_expected):
     n_clusters = len(Lambda)
     abs = 1e-10
     with subtests.test(msg="mu"):
-        assert mu == approx(mu_expected, abs=abs)
+        assert mu == pytest.approx(mu_expected, abs=abs)
     with subtests.test(msg="Lambda"):
         for i in range(n_clusters):
-            for bl in Lambda[i].keys():
-                assert Lambda[i][bl] == approx(Lambda_expected, abs=abs)
+            for bl in Lambda[i]:
+                assert Lambda[i][bl] == pytest.approx(Lambda_expected, abs=abs)
     with subtests.test(msg="Z"):
         for i in range(n_clusters):
-            for bl in Z[i].keys():
-                assert Z[i][bl] == approx(Z_expected, abs=abs)
+            for bl in Z[i]:
+                assert Z[i][bl] == pytest.approx(Z_expected, abs=abs)
 
-@pytest.fixture
+
+@pytest.fixture()
 def one_band():
     n_orb = 1
     spatial_dim = 3
     nkx = 10
     beta = 40
     U = 4
-    mu = U / 2 # half-filling
+    mu = U / 2  # half-filling
     n_target = 1
-    gf_struct = [ (bl, n_orb) for bl in ['up', 'dn'] ]
+    gf_struct = [(bl, n_orb) for bl in ["up", "dn"]]
     h0_k = build_cubic_h0_k(gf_struct=gf_struct, nkx=nkx, spatial_dim=spatial_dim)
-    h_int = U * n('up',0) * n('dn',0)
+    h_int = U * n("up", 0) * n("dn", 0)
     embedding = EmbeddingAtomDiag(h_int, gf_struct)
-    #kweight = SmearingKWeight(beta=beta, mu=mu)
+    # kweight = SmearingKWeight(beta=beta, mu=mu)
     kweight = SmearingKWeight(beta=beta, n_target=n_target)
     Lambda_expected = np.array([[2.0]])
     Z_expected = np.array([[0.437828801025]])
     return gf_struct, h0_k, embedding, kweight, mu, Lambda_expected, Z_expected
 
-@pytest.fixture
+
+@pytest.fixture()
 def bilayer():
     U = 4
     V = 0.25
-    mu = U / 2.0 # half-filling
+    mu = U / 2.0  # half-filling
     n_target = 2
     n_orb = 2
     spatial_dim = 3
     nkx = 10
     beta = 40
-    spin_names = ['up','dn']
+    spin_names = ["up", "dn"]
     gf_struct = set_operator_structure(spin_names, n_orb, off_diag=True)
     h0_k = build_cubic_h0_k(gf_struct=gf_struct, nkx=nkx, spatial_dim=spatial_dim)
-    for bl in h0_k.keys():
-        h0_k[bl][:,0,1] += V
-        h0_k[bl][:,1,0] += V
+    for bl in h0_k:
+        h0_k[bl][:, 0, 1] += V
+        h0_k[bl][:, 1, 0] += V
     h_int = Operator()
     for o in range(n_orb):
-        h_int += U * n("up",o) * n("dn",o)
+        h_int += U * n("up", o) * n("dn", o)
     embedding = EmbeddingAtomDiag(h_int, gf_struct)
-    #kweight = SmearingKWeight(beta=beta, mu=mu)
+    # kweight = SmearingKWeight(beta=beta, mu=mu)
     kweight = SmearingKWeight(beta=beta, n_target=n_target)
-    Lambda_expected = np.array([[2.0, 0.114569681915],[0.114569681915, 2.0]])
-    Z_expected = np.array([[0.452846149446, 0],[0, 0.452846149446]])
+    Lambda_expected = np.array([[2.0, 0.114569681915], [0.114569681915, 2.0]])
+    Z_expected = np.array([[0.452846149446, 0], [0, 0.452846149446]])
     return gf_struct, h0_k, embedding, kweight, mu, Lambda_expected, Z_expected
 
-@pytest.fixture
+
+@pytest.fixture()
 def kanamori():
     coeff = 0.2
     U = 3
     J = coeff * U
-    Up = U - 2*J
-    mu = 0.5*U + 0.5*Up + 0.5*(Up-J) # half-filling
+    Up = U - 2 * J
+    mu = 0.5 * U + 0.5 * Up + 0.5 * (Up - J)  # half-filling
     n_target = 2
-    #mu = -0.81 + (0.6899-1.1099*coeff)*U + (-0.02548+0.02709*coeff-0.1606*coeff**2)*U**2 # quarter-filling DMFT result
+    # mu = -0.81 + (0.6899-1.1099*coeff)*U + (-0.02548+0.02709*coeff-0.1606*coeff**2)*U**2 # quarter-filling DMFT result
     n_orb = 2
     spatial_dim = 3
     nkx = 10
     beta = 40
-    spin_names = ['up','dn']
+    spin_names = ["up", "dn"]
     gf_struct = set_operator_structure(spin_names, n_orb, off_diag=True)
     h0_k = build_cubic_h0_k(gf_struct=gf_struct, nkx=nkx, spatial_dim=spatial_dim)
-    h_int = h_int_kanamori(spin_names=spin_names,
-                           n_orb=n_orb,
-                           U=np.array([[0, Up-J], [Up-J, 0]]),
-                           Uprime=np.array([[U, Up], [Up, U]]),
-                           J_hund=J,
-                           off_diag=True)
+    h_int = h_int_kanamori(
+        spin_names=spin_names,
+        n_orb=n_orb,
+        U=np.array([[0, Up - J], [Up - J, 0]]),
+        Uprime=np.array([[U, Up], [Up, U]]),
+        J_hund=J,
+        off_diag=True,
+    )
     embedding = EmbeddingAtomDiag(h_int, gf_struct)
     kweight = SmearingKWeight(beta=beta, mu=mu)
     kweight = SmearingKWeight(beta=beta, n_target=n_target)
-    Lambda_expected = np.array([[3.0, 0.0],[0.0, 3.0]])
-    Z_expected = np.array([[0.574940323948, 0.0],[0.0, 0.574940323948]])
+    Lambda_expected = np.array([[3.0, 0.0], [0.0, 3.0]])
+    Z_expected = np.array([[0.574940323948, 0.0], [0.0, 0.574940323948]])
     return gf_struct, h0_k, embedding, kweight, mu, Lambda_expected, Z_expected
- 
-@pytest.mark.parametrize('model', ['one_band', 'bilayer', 'kanamori'])
+
+
+@pytest.mark.parametrize("model", ["one_band", "bilayer", "kanamori"])
 def test_diis_symmetrize(subtests, request, model):
     model = request.getfixturevalue(model)
-    gf_struct, h0_k, embedding, kweight, mu_expected, Lambda_expected, Z_expected = model
-    S = LatticeSolver(h0_k=h0_k,
-                      gf_struct=[gf_struct],
-                      embedding=[embedding],
-                      update_weights=kweight.update_weights,
-                      symmetries=[symmetrize_blocks])
+    gf_struct, h0_k, embedding, kweight, mu_expected, Lambda_expected, Z_expected = (
+        model
+    )
+    S = LatticeSolver(
+        h0_k=h0_k,
+        gf_struct=[gf_struct],
+        embedding=[embedding],
+        update_weights=kweight.update_weights,
+        symmetries=[symmetrize_blocks],
+    )
     for i in range(S.n_clusters):
         for bl, _ in S.gf_struct[i]:
             np.fill_diagonal(S.Lambda[i][bl], mu_expected)
     S.solve()
     mu_calculated = kweight.mu
-    do_assert(subtests, mu_calculated, S.Lambda, S.Z, 
-              mu_expected, Lambda_expected, Z_expected)
+    do_assert(
+        subtests, mu_calculated, S.Lambda, S.Z, mu_expected, Lambda_expected, Z_expected
+    )
+
 
-@pytest.mark.parametrize('model', ['one_band', 'bilayer', 'kanamori'])
+@pytest.mark.parametrize("model", ["one_band", "bilayer", "kanamori"])
 def test_diis_nosymmetrize(subtests, request, model):
     model = request.getfixturevalue(model)
-    gf_struct, h0_k, embedding, kweight, mu_expected, Lambda_expected, Z_expected = model
-    S = LatticeSolver(h0_k=h0_k,
-                      gf_struct=[gf_struct],
-                      embedding=[embedding],
-                      update_weights=kweight.update_weights)
+    gf_struct, h0_k, embedding, kweight, mu_expected, Lambda_expected, Z_expected = (
+        model
+    )
+    S = LatticeSolver(
+        h0_k=h0_k,
+        gf_struct=[gf_struct],
+        embedding=[embedding],
+        update_weights=kweight.update_weights,
+    )
     for i in range(S.n_clusters):
         for bl, _ in S.gf_struct[i]:
             np.fill_diagonal(S.Lambda[i][bl], mu_expected)
-    S.solve() 
+    S.solve()
     mu_calculated = kweight.mu
-    do_assert(subtests, mu_calculated, S.Lambda, S.Z, 
-              mu_expected, Lambda_expected, Z_expected)
+    do_assert(
+        subtests, mu_calculated, S.Lambda, S.Z, mu_expected, Lambda_expected, Z_expected
+    )
+
 
-@pytest.mark.parametrize('model, root_method', [
-    ('one_band', 'krylov'),
-    ('bilayer', 'krylov'),
-    ('kanamori', 'krylov'), 
-])   
+@pytest.mark.parametrize(
+    ("model", "root_method"),
+    [
+        ("one_band", "krylov"),
+        ("bilayer", "krylov"),
+        ("kanamori", "krylov"),
+    ],
+)
 def test_scipy_root(subtests, request, model, root_method):
     model = request.getfixturevalue(model)
-    gf_struct, h0_k, embedding, kweight, mu_expected, Lambda_expected, Z_expected = model
+    gf_struct, h0_k, embedding, kweight, mu_expected, Lambda_expected, Z_expected = (
+        model
+    )
     from scipy.optimize import root as root_fun
-    S = LatticeSolver(h0_k=h0_k,
-                      gf_struct=[gf_struct],
-                      embedding=[embedding],
-                      update_weights=kweight.update_weights,
-                      symmetries=[symmetrize_blocks],
-                      root=root_fun,
-                      return_x_new = False)
+
+    S = LatticeSolver(
+        h0_k=h0_k,
+        gf_struct=[gf_struct],
+        embedding=[embedding],
+        update_weights=kweight.update_weights,
+        symmetries=[symmetrize_blocks],
+        root=root_fun,
+        return_x_new=False,
+    )
     for i in range(S.n_clusters):
         for bl, _ in S.gf_struct[i]:
             np.fill_diagonal(S.Lambda[i][bl], mu_expected)
     S.solve(method=root_method, tol=1e-12)
     mu_calculated = kweight.mu
-    do_assert(subtests, mu_calculated, S.Lambda, S.Z, 
-              mu_expected, Lambda_expected, Z_expected)
+    do_assert(
+        subtests, mu_calculated, S.Lambda, S.Z, mu_expected, Lambda_expected, Z_expected
+    )
```

### Comparing `risb-0.1.0/LICENSE` & `risb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `risb-0.1.0/README.md` & `risb-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 Copyright (C) 2016-2023 H. L. Nourse and B. J. Powell, 2016-2022 R. H. McKenzie
 
 <!-- INDEX-START -->
 
 ## What is risb?
 
-Tools to solve strongly correlated many-body electronic problems using 
-rotationally invariant slave-bosons (RISB), an auxilliary particle method. 
-RISB is like dynamical mean-field theory (DMFT), but solves problems in a 
+Tools to solve strongly correlated many-body electronic problems using
+rotationally invariant slave-bosons (RISB), an auxilliary particle method.
+RISB is like dynamical mean-field theory (DMFT), but solves problems in a
 fraction of the time, with hopefully not a fraction of the accuracy.
 
 ## Where to start?
 
-If you want to learn how to solve some common strongly correlated lattice 
-models, and how RISB is implemented, then start with the 
-[tutorials](https://thenoursehorse.github.io/risb/tutorials). 
+If you want to learn how to solve some common strongly correlated lattice
+models, and how RISB is implemented, then start with the
+[tutorials](https://thenoursehorse.github.io/risb/tutorials).
 
-If you want to quickly see a calculation, then start with the `examples/` 
-folder in this repository and refer to the 
+If you want to quickly see a calculation, then start with the `examples/`
+folder in this repository and refer to the
 [how-to guides](https://thenoursehorse.github.io/risb/how-to/).
 
 <!-- INDEX-END -->
 
 <!-- CITATION-START -->
 
 ## Citation
@@ -45,22 +45,22 @@
 
 Lastly, the appropriate original theory outlined in the [documentation](https://thenoursehorse.github.io/risb/about.html#original-theory) should be cited.
 
 <!-- INSTALL-START -->
 
 ## Dependencies
 
-* [python](https://www.python.org/) version `> 3.10`
-* [numpy](https://numpy.org/)
-* [scipy](https://scipy.org/)
-* [TRIQS](https://triqs.github.io/) version `3.2.x` if using :class:`EmbeddingAtomDiag`
+- [python](https://www.python.org/) version `> 3.10`
+- [numpy](https://numpy.org/)
+- [scipy](https://scipy.org/)
+- [TRIQS](https://triqs.github.io/) version `3.2.x` if using :class:`EmbeddingAtomDiag`
 
 ## Installation
 
-(Optional) Create a 
+(Optional) Create a
 [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments).
 
 Install
 
 ```shell
 pip install risb
 ```
@@ -69,35 +69,35 @@
 
 ```
 pip uninstall risb
 ```
 
 ### Docker
 
-There is a `Dockerfile` and `docker-compose.yml` inside the `docker` folder. 
-The `Dockerfile` will pull the 
-[TRIQS docker image](https://hub.docker.com/r/flatironinstitute/triqs) 
+There is a `Dockerfile` and `docker-compose.yml` inside the `docker` folder.
+The `Dockerfile` will pull the
+[TRIQS docker image](https://hub.docker.com/r/flatironinstitute/triqs)
 from the hub and install risb. Using the image will be the same as outlined in
 the [install instructions](https://triqs.github.io/triqs/latest/install.html#docker).
-To connect to the [Jupyter](https://jupyter.org/) notebook it is 
+To connect to the [Jupyter](https://jupyter.org/) notebook it is
 
 ```shell
 localhost:8888/?token=put/token/here
 ```
 
-You can find the token by attaching a shell to the container 
+You can find the token by attaching a shell to the container
 and running
 
 ```shell
 jupyter server list
 ```
 
-There is also a development `Dockerfile.dev` and the corresponding 
-`docker-compose-dev.yml` in order to have a container to develop code. It 
-installs [TRIQS](https://triqs.github.io/) from source, and works on 
+There is also a development `Dockerfile.dev` and the corresponding
+`docker-compose-dev.yml` in order to have a container to develop code. It
+installs [TRIQS](https://triqs.github.io/) from source, and works on
 Apple M1/M2 (arm64, aarch64), and any amd64 system.
 
 ## Tests
 
 The tests require a working [TRIQS](https://triqs.github.io/) installation.
 
 Clone source
@@ -144,8 +144,8 @@
 
 ```shell
 sphinx-autobuild -b html docs docs/_build
 ```
 
 Access through a browser at `http://127.0.0.1:8000`.
 
-<!-- INSTALL-END -->
+<!-- INSTALL-END -->
```

### Comparing `risb-0.1.0/pyproject.toml` & `risb-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -69,7 +69,50 @@
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 
 [[tool.mypy.overrides]]
 module = [ "numpy.*", "scipy.*", "triqs.*", "nox.*"]
 ignore_missing_imports = true
+
+[tool.ruff]
+src = ["src"]
+
+[tool.ruff.format]
+docstring-code-format = true
+
+[tool.ruff.lint]
+extend-select = [
+  "B",           # flake8-bugbear
+  "I",           # isort
+  "ARG",         # flake8-unused-arguments
+  "C4",          # flake8-comprehensions
+  "EM",          # flake8-errmsg
+  "ICN",         # flake8-import-conventions
+  "PGH",         # pygrep-hooks
+  "PIE",         # flake8-pie
+  "PL",          # pylint
+  "PT",          # flake8-pytest-style
+  "PTH",         # flake8-use-pathlib
+  "RET",         # flake8-return
+  "RUF",         # Ruff-specific
+  "SIM",         # flake8-simplify
+  "TID251",      # flake8-tidy-imports.banned-api
+  "T20",         # flake8-print
+  "UP",          # pyupgrade
+  "YTT",         # flake8-2020
+  "D",           # pydocstyle
+  "D204",        # one-blank-line-after-class
+  "D301",        # escape-sequence-in-docstring
+  "D413",        # blank-line-after-last-section
+]
+ignore = [
+  "PLR",    # Design related pylint codes
+  "PT004",  # Incorrect check, usefixtures is the correct way to do this
+  "RUF012", # Would require a lot of ClassVar's
+]
+
+[tool.ruff.lint.pycodestyle]
+max-line-length = 100
+
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
```

### Comparing `risb-0.1.0/PKG-INFO` & `risb-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: risb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Rotationally invariant slave boson mean-field theory.
 Project-URL: Homepage, https://github.com/thenoursehorse/risb
 Project-URL: Documentation, https://thenoursehorse.github.io/risb
 Author: H. L. Nourse
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -709,27 +709,27 @@
 
 Copyright (C) 2016-2023 H. L. Nourse and B. J. Powell, 2016-2022 R. H. McKenzie
 
 <!-- INDEX-START -->
 
 ## What is risb?
 
-Tools to solve strongly correlated many-body electronic problems using 
-rotationally invariant slave-bosons (RISB), an auxilliary particle method. 
-RISB is like dynamical mean-field theory (DMFT), but solves problems in a 
+Tools to solve strongly correlated many-body electronic problems using
+rotationally invariant slave-bosons (RISB), an auxilliary particle method.
+RISB is like dynamical mean-field theory (DMFT), but solves problems in a
 fraction of the time, with hopefully not a fraction of the accuracy.
 
 ## Where to start?
 
-If you want to learn how to solve some common strongly correlated lattice 
-models, and how RISB is implemented, then start with the 
-[tutorials](https://thenoursehorse.github.io/risb/tutorials). 
+If you want to learn how to solve some common strongly correlated lattice
+models, and how RISB is implemented, then start with the
+[tutorials](https://thenoursehorse.github.io/risb/tutorials).
 
-If you want to quickly see a calculation, then start with the `examples/` 
-folder in this repository and refer to the 
+If you want to quickly see a calculation, then start with the `examples/`
+folder in this repository and refer to the
 [how-to guides](https://thenoursehorse.github.io/risb/how-to/).
 
 <!-- INDEX-END -->
 
 <!-- CITATION-START -->
 
 ## Citation
@@ -750,22 +750,22 @@
 
 Lastly, the appropriate original theory outlined in the [documentation](https://thenoursehorse.github.io/risb/about.html#original-theory) should be cited.
 
 <!-- INSTALL-START -->
 
 ## Dependencies
 
-* [python](https://www.python.org/) version `> 3.10`
-* [numpy](https://numpy.org/)
-* [scipy](https://scipy.org/)
-* [TRIQS](https://triqs.github.io/) version `3.2.x` if using :class:`EmbeddingAtomDiag`
+- [python](https://www.python.org/) version `> 3.10`
+- [numpy](https://numpy.org/)
+- [scipy](https://scipy.org/)
+- [TRIQS](https://triqs.github.io/) version `3.2.x` if using :class:`EmbeddingAtomDiag`
 
 ## Installation
 
-(Optional) Create a 
+(Optional) Create a
 [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments).
 
 Install
 
 ```shell
 pip install risb
 ```
@@ -774,35 +774,35 @@
 
 ```
 pip uninstall risb
 ```
 
 ### Docker
 
-There is a `Dockerfile` and `docker-compose.yml` inside the `docker` folder. 
-The `Dockerfile` will pull the 
-[TRIQS docker image](https://hub.docker.com/r/flatironinstitute/triqs) 
+There is a `Dockerfile` and `docker-compose.yml` inside the `docker` folder.
+The `Dockerfile` will pull the
+[TRIQS docker image](https://hub.docker.com/r/flatironinstitute/triqs)
 from the hub and install risb. Using the image will be the same as outlined in
 the [install instructions](https://triqs.github.io/triqs/latest/install.html#docker).
-To connect to the [Jupyter](https://jupyter.org/) notebook it is 
+To connect to the [Jupyter](https://jupyter.org/) notebook it is
 
 ```shell
 localhost:8888/?token=put/token/here
 ```
 
-You can find the token by attaching a shell to the container 
+You can find the token by attaching a shell to the container
 and running
 
 ```shell
 jupyter server list
 ```
 
-There is also a development `Dockerfile.dev` and the corresponding 
-`docker-compose-dev.yml` in order to have a container to develop code. It 
-installs [TRIQS](https://triqs.github.io/) from source, and works on 
+There is also a development `Dockerfile.dev` and the corresponding
+`docker-compose-dev.yml` in order to have a container to develop code. It
+installs [TRIQS](https://triqs.github.io/) from source, and works on
 Apple M1/M2 (arm64, aarch64), and any amd64 system.
 
 ## Tests
 
 The tests require a working [TRIQS](https://triqs.github.io/) installation.
 
 Clone source
@@ -849,8 +849,8 @@
 
 ```shell
 sphinx-autobuild -b html docs docs/_build
 ```
 
 Access through a browser at `http://127.0.0.1:8000`.
 
-<!-- INSTALL-END -->
+<!-- INSTALL-END -->
```

