# Comparing `tmp/continuedfractions-0.12.6.tar.gz` & `tmp/continuedfractions-0.12.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedfractions-0.12.6.tar", last modified: Thu May 16 20:08:41 2024, max compression
+gzip compressed data, was "continuedfractions-0.12.7.tar", last modified: Fri May 17 18:11:14 2024, max compression
```

## Comparing `continuedfractions-0.12.6.tar` & `continuedfractions-0.12.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.6/LICENSE
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.6/LICENSE
--rw-r--r--   0        0        0     3436 2024-05-16 13:59:15.488030 continuedfractions-0.12.6/README.md
--rw-r--r--   0        0        0     3436 2024-05-16 13:59:15.488030 continuedfractions-0.12.6/README.md
--rw-r--r--   0        0        0     3506 2024-05-16 20:08:41.167105 continuedfractions-0.12.6/pyproject.toml
--rw-r--r--   0        0        0    31312 2024-05-15 20:00:55.929517 continuedfractions-0.12.6/src/continuedfractions/continuedfraction.py
--rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.6/src/continuedfractions/lib.py
--rw-r--r--   0        0        0    40762 2024-05-16 20:02:30.426192 continuedfractions-0.12.6/src/continuedfractions/sequences.py
--rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.6/src/continuedfractions/utils.py
--rw-r--r--   0        0        0       23 2024-05-16 12:25:39.833527 continuedfractions-0.12.6/src/continuedfractions/version.py
--rw-r--r--   0        0        0    24420 1970-01-01 00:00:00.000000 continuedfractions-0.12.6/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.7/LICENSE
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.7/LICENSE
+-rw-r--r--   0        0        0     3436 2024-05-16 21:48:47.164813 continuedfractions-0.12.7/README.md
+-rw-r--r--   0        0        0     3436 2024-05-16 21:48:47.164813 continuedfractions-0.12.7/README.md
+-rw-r--r--   0        0        0     3506 2024-05-17 18:11:14.142914 continuedfractions-0.12.7/pyproject.toml
+-rw-r--r--   0        0        0    31312 2024-05-15 20:00:55.929517 continuedfractions-0.12.7/src/continuedfractions/continuedfraction.py
+-rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.7/src/continuedfractions/lib.py
+-rw-r--r--   0        0        0    35383 2024-05-17 18:03:00.181544 continuedfractions-0.12.7/src/continuedfractions/sequences.py
+-rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.7/src/continuedfractions/utils.py
+-rw-r--r--   0        0        0       23 2024-05-17 17:47:35.471630 continuedfractions-0.12.7/src/continuedfractions/version.py
+-rw-r--r--   0        0        0    24420 1970-01-01 00:00:00.000000 continuedfractions-0.12.7/PKG-INFO
```

### Comparing `continuedfractions-0.12.6/LICENSE` & `continuedfractions-0.12.7/LICENSE`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.6/README.md` & `continuedfractions-0.12.7/README.md`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.6/pyproject.toml` & `continuedfractions-0.12.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
-version = "0.12.6"
+version = "0.12.7"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 user = [
     "jupyter",
```

### Comparing `continuedfractions-0.12.6/src/continuedfractions/continuedfraction.py` & `continuedfractions-0.12.7/src/continuedfractions/continuedfraction.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.6/src/continuedfractions/lib.py` & `continuedfractions-0.12.7/src/continuedfractions/lib.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.6/src/continuedfractions/sequences.py` & `continuedfractions-0.12.7/src/continuedfractions/sequences.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,54 +29,54 @@
 from continuedfractions.continuedfraction import ContinuedFraction
 
 KSRMNode: TypeAlias = tuple[int, int]   #: Custom type for nodes of the KSRM coprime pairs tree
 KSRMBranch: NamedCallableProxy          #: Custom type for generating branches of the KSRM coprime pairs tree
 
 
 def _coprime_integers(n: int, /, *, start: int = 1, stop: int = None) -> Generator[int, None, None]:
-    """A private function which generates a sequence of integers :math:`1 \\leq m < n` coprime to the given positive integer :math:`n`.
+    """A private function which generates a sequence of (positive) integers :math:`1 \\leq m < n` coprime to a given positive integer :math:`n`.
 
     The tuple is sorted in descending order of magnitude.
 
     The optional ``start`` and ``stop`` parameters can be used to bound the
-    the range of integers in which integers coprime to the given :math:`n` are
-    sought.
+    the range of (positive) integers in which integers coprime to the given
+    :math:`n` are sought.
 
     For :math:`n = 1, 2` the ``start`` value is effectively ignored, but
     if :math:`n > 2` then the ``start`` value must be an integer in the range
     :math:`1..n - 2`.
 
     The ``stop`` value defaults to ``None``, which is then internally
     initialised to :math:`n`; if :math:`n > 1` and ``stop`` is given then it
     must be an integer in the range :math:`\\text{start} + 1..n`.
 
     Parameters
     ----------
     n : int
-        The positive integer for which coprime integers :math:`m < n` are
-        sought.
+        The positive integer for which (positive) coprime integers
+        :math:`m < n` are sought.
 
     start : int, default=1
-        The lower bound of the range of integers in which integers coprime
-        to the given :math:`n` are sought. For :math:`n = 1, 2` the ``start``
-        value is effectively ignored, but if :math:`n > 2` then the ``start``
-        value must be in the range :math:`1..n - 2`.
+        The lower bound of the range of (positive) integers in which integers
+        coprime to the given :math:`n` are sought. For :math:`n = 1, 2` the
+        ``start`` value is effectively ignored, but if :math:`n > 2` then the
+        ``start`` value must be in the range :math:`1..n - 2`.
 
     stop : int, default=None
-        The upper bound of the range of integers in which integers coprime
-        to the given :math:`n` are sought. The ``stop`` value defaults to
-        ``None``, which is then internally initialised to :math:`n`; if
+        The upper bound of the range of (positive) integers in which integers
+        coprime to the given :math:`n` are sought. The ``stop`` value defaults
+        to ``None``, which is then internally initialised to :math:`n`; if
         :math:`n > 1` and ``stop`` is given then it must be an integer in the
         range :math:`\\text{start} + 1..n`.
 
     Yields
     ------
     int
-        A sequence of integers :math:`1 \\leq m < n` coprime to the given
-        positive integer :math:`n`.
+        A sequence of (positive) integers :math:`1 \\leq m < n` coprime to a
+        given positive integer :math:`n`.
 
     Examples
     --------
     Examples using the default ``start`` and ``stop`` values:
 
     >>> tuple(_coprime_integers(1))
     (1,)
@@ -158,56 +158,56 @@
                 stop = _start - 1
                 q -= 1
                 _start = ((10 ** 3) * q) + 1
 
 
 @functools.cache
 def coprime_integers(n: int, /, *, start: int = 1, stop: int = None) -> tuple[int]:
-    """A function which returns a sequence of integers :math:`1 \\leq m < n` coprime to the given positive integer :math:`n`.
+    """A function which returns a sequence of (positive) integers :math:`1 \\leq m < n` coprime to a given positive integer :math:`n`.
 
     Wrapper for the private :py:class:`~continuedfractions.sequences._coprime_integers`.
 
     The tuple is sorted in descending order of magnitude.
 
     The optional ``start`` and ``stop`` parameters can be used to bound the
-    the range of integers in which integers coprime to the given :math:`n` are
-    sought.
+    the range of (positive) integers in which integers coprime to the given
+    :math:`n` are sought.
 
     For :math:`n = 1, 2` the ``start`` value is effectively ignored, but
     if :math:`n > 2` then the ``start`` value must be an integer in the range
     :math:`1..n - 2`.
 
     The ``stop`` value defaults to ``None``, which is then internally
     initialised to :math:`n`; if :math:`n > 1` and ``stop`` is given then it
     must be an integer in the range :math:`\\text{start} + 1..n`.
 
     Parameters
     ----------
     n : int
-        The positive integer for which coprime integers :math:`m < n` are
-        sought.
+        The positive integer for which (positive) coprime integers
+        :math:`m < n` are sought.
 
     start : int, default=1
-        The lower bound of the range of integers in which integers coprime
-        to the given :math:`n` are sought. For :math:`n = 1, 2` the ``start``
-        value is effectively ignored, but if :math:`n > 2` then the ``start``
-        value must be in the range :math:`1..n - 2`.
+        The lower bound of the range of (positive) integers in which integers
+        coprime to the given :math:`n` are sought. For :math:`n = 1, 2` the
+        ``start`` value is effectively ignored, but if :math:`n > 2` then the
+        ``start`` value must be in the range :math:`1..n - 2`.
 
     stop : int, default=None
-        The upper bound of the range of integers in which integers coprime
-        to the given :math:`n` are sought. The ``stop`` value defaults to
-        ``None``, which is then internally initialised to :math:`n`; if
+        The upper bound of the range of (positive) integers in which integers
+        coprime to the given :math:`n` are sought. The ``stop`` value defaults
+        to ``None``, which is then internally initialised to :math:`n`; if
         :math:`n > 1` and ``stop`` is given then it must be an integer in the
         range :math:`\\text{start} + 1..n`.
 
     Returns
     -------
     tuple
-        A sequence of integers :math:`1 \\leq m < n` coprime to the given
-        positive integer :math:`n`.
+        A sequence of (positive) integers :math:`1 \\leq m < n` coprime to a
+        given positive integer :math:`n`.
 
     Examples
     --------
     Examples using the default ``start`` and ``stop`` values:
 
     >>> coprime_integers(1)
     (1,)
@@ -286,77 +286,16 @@
 
     .. note::
 
        The author could not access the Kanga paper online, but the core result
        is described clearly in the papers of Saunders and Randall, and of
        Mitchell.
 
-    These trees are directly related to so-called `primitive Pythagorean triples <https://en.wikipedia.org/wiki/Pythagorean_triple#Elementary_properties_of_primitive_Pythagorean_triples>`_,
-    but have a fundamental consequence for the generation of coprime pairs: all
-    pairs of (positive) coprime integers :math:`(a, b)`, where
-    :math:`1 \\leq b < a`, can be represented as nodes in one of two ternary
-    trees, the first which has the "parent" node :math:`(2, 1)` and the second
-    which has the parent node :math:`(3, 1)`. Each node has three children
-    given by the relations:
-
-    .. math::
-
-       (a^\\prime, b^\\prime) = \\begin{cases}
-                                (2a - b, a), \\hskip{3em} \\text{ branch #} 1 \\\\
-                                (2a + b, a), \\hskip{3em} \\text{ branch #} 2 \\\\
-                                (a + 2b, b), \\hskip{3em} \\text{ branch #} 3                   
-                                \\end{cases}
-
-    where :math:`1 \\leq b < a` and :math:`(a, b) = 1`.
-
-    Generating coprime pairs can then be implemented by a generative search
-    procedure that starts separately from the parents :math:`(2, 1)` and
-    :math:`(3, 1)`, and applies the functions given by the mappings below to
-    each parent:
-
-    .. math::
-
-       \\begin{align}
-       (a, b) &\\longmapsto (2a - b, a) \\\\
-       (a, b) &\\longmapsto (2a + b, a) \\\\
-       (a, b) &\\longmapsto (a + 2b, b)
-       \\end{align}
-
-    producing the "1st generation" of :math:`3 + 3 = 6` triplets. This can be
-    repeated ad infinitum as required.
-
-    .. note::
-
-       The tree starting at the root :math:`(3, 1)` will only contain pairs of
-       odd coprimes, under the maps described above.
-
-    If we let :math:`k = 0` denote the :math:`0`-th generation consisting only
-    of the two roots :math:`(2, 1)` and :math:`(3, 1)`, then for
-    :math:`k \\geq 1` the :math:`k`-th generation, for either tree, will have a
-    total of :math:`3^k` children, the total number of all members up to and
-    including the :math:`k`-th generation will be
-    :math:`1 + 3 + 3^2 + \\ldots + 3^k = \\frac{3^{k + 1} - 1}{2}`, and the
-    total number of all members in both trees up to and including the
-    :math:`k`-th generation will be :math:`3^{k + 1} - 1`.
-
-    The number of coprime pairs generated for a given :math:`n \\geq 1` is
-    given by:
-
-    .. math::
-
-       \\phi(1) + \\phi(2) + \\cdots + \\phi(n) = \\sum_{k = 1}^n \\phi(k)
-
-    where :math:`\\phi(k)` is `Euler's totient function <https://en.wikipedia.org/wiki/Euler%27s_totient_function>`_.
-
-    This is because if :math:`\\mathcal{C}_n` denotes the set of all coprime
-    pairs :math:`(a, b)`, with :math:`1 \\leq b < a \\leq n`, then it can be
-    partitioned into disjoint subsets :math:`\\mathcal{C}_k`, where
-    :math:`k=1,2,\\ldots,n`, and each :math:`\\mathcal{C}_k` contains
-    :math:`\\phi(k)` pairs :math:`(k, j)`, where
-    :math:`1 \\leq j < k \\leq n` and :math:`(k, j) = 1`.
+    See the `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/sequences.html#ksrm-trees>`_
+    for more details.
     """
 
     # The two slots for the private attributes for the key tree features - the
     # two roots ``(2, 1), (3, 1)``, and the three branch generating functions.
     __slots__ = ('_roots', '_branches')
 
     _roots: tuple[KSRMNode, KSRMNode]
@@ -386,14 +325,16 @@
 
         For more details see the following papers:
 
         * Kanga, A. R. (1990). The Family Tree of Pythagorean Triplets. The Mathematical Gazette, 26(15), 15-17.
         * Mitchell, D. W. (2001). An Alternative Characterisation of All Primitive Pythagorean Triples. The Mathematical Gazette, 85(503), 273-275. https://doi.org/10.2307/3622017
         * Saunders, R., & Randall, T. (1994). The family tree of the Pythagorean triplets revisited. The Mathematical Gazette, 78(482), 190-193. https://doi.org/10.2307/3618576
 
+        or the `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/sequences.html#ksrm-trees>`_.
+
         Examples
         --------
         >>> KSRMTree().roots
         ((2, 1), (3, 1))
         """
         return self._roots
 
@@ -413,14 +354,16 @@
 
         For more details see the following papers:
 
         * Kanga, A. R. (1990). The Family Tree of Pythagorean Triplets. The Mathematical Gazette, 26(15), 15-17.
         * Mitchell, D. W. (2001). An Alternative Characterisation of All Primitive Pythagorean Triples. The Mathematical Gazette, 85(503), 273-275. https://doi.org/10.2307/3622017
         * Saunders, R., & Randall, T. (1994). The family tree of the Pythagorean triplets revisited. The Mathematical Gazette, 78(482), 190-193. https://doi.org/10.2307/3618576
 
+        or the `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/sequences.html#ksrm-trees>`_.
+
         Examples
         --------
         Generating the first two generations of children for the parent
         :math:`(2, 1)`.
 
         >>> tree = KSRMTree()
         >>> tree.branches
@@ -456,41 +399,28 @@
         self,
         n: int,
         visited: list[tuple[KSRMNode, KSRMBranch]],     # noqa: F821
         /,
         *,
         node_bound: int = None
     ) -> tuple[KSRMNode, KSRMBranch, int, KSRMBranch]:  # noqa: F821
-        """Backtracks on the KSRM coprime pairs trees.
+        """Backtracks on the KSRM coprime pairs trees from a failed node to the nearest previously visited node that satisfies the node bound.
 
         A private function that backtracks on the KSRM coprime pairs trees: the
         procedure is that, given a (positive) integer :math:`n > 2`, for which
         coprime pairs are being sought, and a sequence (list) of pairs of
         visited nodes and their associated generating branches in the KSRM
         tree, and assuming that the last element of the visited sequence
         contains the node that "failed", the function identifies the nearest
         previously visited node whose first component satisifes the test
         :math:`< n` **and** and whose associated generating branch is not equal
         to the third branch given by :math:`(x, y) \\longmapsto (x + 2y, y)`.
 
         .. note::
 
-           One key property of the KSRM trees is that, for a given search value
-           :math:`n`, if the current node is :math:`(a, b) = (n, b)` and the
-           successor node on the first branch, :math:`(2a - b, a)`, fails the
-           test :math:`2a - b \\leq n`, then so will the successor nodes on
-           the second and third branches.
-
-           This means in the case of a node failure in the search on the first
-           branch, all three branches of the predecessor node of the failed
-           node can be pruned in the sequence of visited nodes and generating
-           branch pairs.
-
-        .. note::
-
            The function assumes that the last node in the incoming sequence
            of visited nodes and generating branch pairs represents a "failed"
            node, i.e. whose first component failed the test :math:`\\leq n`
            during the search. No attempt is made to validate or verify the
            failed node, and the only purpose of the function is to backtrack
            to the nearest previously visited node which meets the requirements
            listed above.
@@ -584,49 +514,42 @@
             last_branch = visited[cur_index + 1][1]
 
         # Return the current node, generating branch, index and the generating
         # branch of the last visited node before the current node.
         return cur_node, cur_branch, cur_index, last_branch
 
     def search_root(self, n: int, root: KSRMNode, /) -> Generator[KSRMNode, None, None]:
-        """Backtracking depth-first branch-and-bound search (in pre-order, NLMR) of the KSRM coprime pairs trees from the given root node to find all pairs of coprime (positive) integers not exceeding the given integer :math:`n \\geq 1`.
+        """Depth-first branch-and-bound generative search function (in pre-order, NLMR), with backtracking and pruning, on the KSRM coprime pairs trees, starting from the given root node.
 
         The given root node need not be the canonical roots, :math:`(2, 1)`,
         :math:`(3, 1)`, but can be any of their successor nodes.
 
         It is required that :math:`n \\geq 2`, otherwise a
         :py:class:`ValueError` is raised.
 
-        The search implementation is an iterative version of a backtracking
-        depth-first branch-and-bound search (DFS), in which nodes are traversed
-        in NLMR pre-order (root -> left -> mid -> right) and bounds and checks
-        are applied to the nodes, before further traversal or backtracking:
+        The search implementation is an iterative version of a depth-first
+        branch-and-bound search (DFS) procedure, with backtracking and pruning,
+        in which nodes are traversed in NLMR pre-order (root -> left -> mid ->
+        right) and bounds and checks are applied to the nodes, including
+        pruning failed or unnecessary nodes, before further traversal or
+        backtracking:
         
         #. Visit the current node :math:`(a, b)` and check :math:`a \\leq n`.
         #. If the check is successful iteratively traverse the current node's
            first child and its children, then the second child and its 
            children, and then the third child and its children, applying the
            check :math:`a \\leq n` to each visited node.
         #. If a check fails for any node backtrack to the nearest previously
            visited node which meets a stricter check :math:`a < n` and which
            has unvisited child nodes, while pruning all visited intermediate
            nodes after the backtracked target node and leading up to the failed
            node, including the failed node. By design the backtracked target
            node will have untraversed children on at least one branch, and the
            traversal can begin again, as described above.
 
-        .. note::
-
-           One key property of the KSRM trees used in this implementation is
-           that for a given integer :math:`n \\geq 1`, if the current node is
-           :math:`(a, b) = (n, b)` and the child node on the first branch,
-           :math:`(2a - b, a)`, fails the test :math:`2a - b \\leq n`, then
-           so will the child nodes on the second and third branches, and
-           thus all three children can be pruned.
-
         Parameters
         ----------
         n : int
             The positive integer for which coprime pairs :math:`(a, b)`, with
             :math:`1 \\leq b < a \\leq n`, are sought.
 
         root : tuple
@@ -751,21 +674,22 @@
                 continue
 
         # Not strictly required, but this has been inserted to make
         # debugging easier.
         return
 
     def search(self, n: int, /) -> Generator[KSRMNode, None, None]:
-        """Backtracking depth-first branch-and-bound search (in pre-order, NLMR) of the KSRM coprime pairs trees to find all pairs of coprime (positive) integers not exceeding the given integer :math:`n \\geq 1`.
+        """Depth-first branch-and-bound generative search function (in pre-order, NLMR) on the KSRM coprime pairs trees to find all pairs of coprime (positive) integers not exceeding the given integer :math:`n \\geq 1`.
     
         See the :py:meth:`~continuedfractions.sequences.KSRMTree.search_root`
         method for details of the implementation for the root-based search.
 
-        This method mainly calls the root-based search method for the two
-        canonical roots :math:`(2, 1)` and :math:`(3, 1)`.
+        This method mainly calls the root-based search method
+        :py:meth:`~continuedfractions.sequences.KSRMTree.search_root` for the
+        two canonical roots :math:`(2, 1)` and :math:`(3, 1)`.
 
         Parameters
         ----------
         n : int
             The positive integer for which coprime pairs :math:`(a, b)`, with
             :math:`1 \\leq b < a \\leq n`, are sought.
 
@@ -879,62 +803,16 @@
 def farey_sequence(n: int, /) -> tuple[ContinuedFraction]:
     """Returns an (ordered) sequence (tuple) of rational numbers forming the Farey sequence of order :math:`n`.
 
     The elements of the sequence are returned as
     :py:class:`~continuedfractions.continuedfraction.ContinuedFraction`
     instances, in ascending order of magnitude.
 
-    The `Farey sequence <https://en.wikipedia.org/wiki/Farey_sequence>`_
-    :math:`F_n` of order :math:`n` is an (ordered) sequence of rational numbers
-    which is defined recursively as follows:
-
-    .. math::
-
-       \\begin{align}
-       F_1 &= \\left(\\frac{0}{1}, \\frac{1}{1}\\right) \\\\
-       F_k &= \\left(\\frac{a}{b}\\right) \\text{ s.t. } (a, b) = 1 \\text{ and } b \\leq n,
-              \\hskip{3em} k \\geq 2
-       \\end{align}
-
-    If we write the fractions in :math:`F_n` as :math:`\\frac{b}{a}` where
-    :math:`a > b` then the restriction :math:`(a, b) = 1` (meaning :math:`a`
-    and :math:`b` must be coprime), combined with :math:`a \\leq n`, means that
-    for each :math:`a \\leq n` :math:`F_n` contains exactly :math:`\\phi(a)``
-    fractions of the form :math:`\\frac{b}{a}` where :math:`(a, b) = 1`.
-
-    As :math:`F_n` also contains the special fraction :math:`\\frac{0}{1}` it
-    means that the length :math:`|F_n|` of :math:`F_n` is given by:
-
-    .. math::
-
-       |F_n| = 1 + \\phi(1) + \\phi(2) + \\cdots + \\phi(n) = 1 + \\sum_{k = 1}^n \\phi(k)
-
-    where :math:`\\phi(k)` is `Euler's totient function <https://en.wikipedia.org/wiki/Euler%27s_totient_function>`_.
-
-    As :math:`F_n` includes all elements of :math:`F_k` for :math:`k < n` the
-    length :math:`|F_n|` can also be written as:
-
-    .. math::
-
-       |F_n| = |F_{n - 1}| + \\phi(n)
-
-    The first five Farey sequences are:
-
-    .. math::
-
-       \\begin{align}
-       F_1 &= \\left( \\frac{0}{1}, \\frac{1}{1} \\right) \\\\
-       F_2 &= \\left( \\frac{0}{1}, \\frac{1}{2}, \\frac{1}{1} \\right) \\\\
-       F_3 &= \\left( \\frac{0}{1}, \\frac{1}{3}, \\frac{1}{2}, \\frac{2}{3}, \\frac{1}{1} \\right) \\\\
-       F_4 &= \\left( \\frac{0}{1}, \\frac{1}{4}, \\frac{1}{3}, \\frac{1}{2}, \\frac{2}{3}, \\frac{3}{4}, \\frac{1}{1} \\right) \\\\
-       F_5 &= \\left( \\frac{0}{1}, \\frac{1}{5}, \\frac{1}{4}, \\frac{1}{3}, \\frac{2}{5}, \\frac{1}{2}, \\frac{3}{5}, \\frac{2}{3}, \\frac{3}{4}, \\frac{4}{5}, \\frac{1}{1} \\right)
-       \\end{align}
-
-    Farey sequences have quite interesting properties and relations, as
-    described `here <https://en.wikipedia.org/wiki/Farey_sequence>`_.
+    See the `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/sequences.html#sequences-farey-sequences>`_
+    for more details.
 
     Parameters
     ----------
     n : int:
         The order of the Farey sequence.
 
     Returns
```

### Comparing `continuedfractions-0.12.6/src/continuedfractions/utils.py` & `continuedfractions-0.12.7/src/continuedfractions/utils.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.6/PKG-INFO` & `continuedfractions-0.12.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuedfractions
-Version: 0.12.6
+Version: 0.12.7
 Summary: Object-oriented continued fractions with Python.
 Keywords: computational number theory,coprime integers,continued fractions,farey sequences,irrational numbers,mediants,number theory,rational approximation,rational numbers,real numbers
 Author-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 Maintainer-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 License: Mozilla Public License Version 2.0
         ==================================
```

