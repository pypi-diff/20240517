# Comparing `tmp/exploration-0.7.2.tar.gz` & `tmp/exploration-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exploration-0.7.2.tar", last modified: Tue Mar  5 00:22:06 2024, max compression
+gzip compressed data, was "exploration-0.7.4.tar", last modified: Fri May 17 00:40:57 2024, max compression
```

## Comparing `exploration-0.7.2.tar` & `exploration-0.7.4.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 pmwh      (1000) pmwh      (1000)        0 2024-03-05 00:22:06.358874 exploration-0.7.2/
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)     1526 2024-03-01 02:04:24.000000 exploration-0.7.2/LICENSE.txt
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)    15535 2024-03-05 00:22:06.358874 exploration-0.7.2/PKG-INFO
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)    14359 2024-03-04 20:39:39.000000 exploration-0.7.2/README.md
-drwxr-xr-x   0 pmwh      (1000) pmwh      (1000)        0 2024-03-05 00:22:06.358874 exploration-0.7.2/exploration/
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)      837 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/__init__.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)     1130 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/__main__.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)    24588 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/analysis.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)   224242 2024-03-05 00:20:55.000000 exploration-0.7.2/exploration/base.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)    26546 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/commands.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)   422003 2024-03-04 22:04:48.000000 exploration-0.7.2/exploration/core.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)     2287 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/display.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)    48766 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/geographic.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)    25500 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/graphs.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)   240828 2024-03-05 00:15:34.000000 exploration-0.7.2/exploration/journal.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)    30557 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/main.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)   239699 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/parsing.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)        0 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/py.typed
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)     8216 2024-03-01 02:04:24.000000 exploration-0.7.2/exploration/utils.py
-drwxr-xr-x   0 pmwh      (1000) pmwh      (1000)        0 2024-03-05 00:22:06.358874 exploration-0.7.2/exploration.egg-info/
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)    15535 2024-03-05 00:22:06.000000 exploration-0.7.2/exploration.egg-info/PKG-INFO
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)      553 2024-03-05 00:22:06.000000 exploration-0.7.2/exploration.egg-info/SOURCES.txt
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)        1 2024-03-05 00:22:06.000000 exploration-0.7.2/exploration.egg-info/dependency_links.txt
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)       42 2024-03-05 00:22:06.000000 exploration-0.7.2/exploration.egg-info/requires.txt
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)       12 2024-03-05 00:22:06.000000 exploration-0.7.2/exploration.egg-info/top_level.txt
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)      129 2024-03-01 02:04:24.000000 exploration-0.7.2/pyproject.toml
-drwxr-xr-x   0 pmwh      (1000) pmwh      (1000)        0 2024-03-05 00:22:06.358874 exploration-0.7.2/scripts/
--rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)     7712 2024-03-01 02:04:24.000000 exploration-0.7.2/scripts/egtool.py
--rw-r--r--   0 pmwh      (1000) pmwh      (1000)     1223 2024-03-05 00:22:06.358874 exploration-0.7.2/setup.cfg
+drwxr-xr-x   0 pmwh      (1000) pmwh      (1000)        0 2024-05-17 00:40:57.149694 exploration-0.7.4/
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)     1526 2024-03-08 16:13:54.000000 exploration-0.7.4/LICENSE.txt
+-rw-r--r--   0 pmwh      (1000) pmwh      (1000)    16379 2024-05-17 00:40:57.149694 exploration-0.7.4/PKG-INFO
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)    15203 2024-03-18 14:56:43.000000 exploration-0.7.4/README.md
+drwxr-xr-x   0 pmwh      (1000) pmwh      (1000)        0 2024-05-17 00:40:57.139694 exploration-0.7.4/exploration/
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)      837 2024-03-18 14:56:53.000000 exploration-0.7.4/exploration/__init__.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)     1130 2024-03-08 16:13:54.000000 exploration-0.7.4/exploration/__main__.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)    24588 2024-03-08 16:13:54.000000 exploration-0.7.4/exploration/analysis.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)   228170 2024-03-17 15:35:52.000000 exploration-0.7.4/exploration/base.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)    26546 2024-03-08 16:13:54.000000 exploration-0.7.4/exploration/commands.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)   424754 2024-03-17 15:37:38.000000 exploration-0.7.4/exploration/core.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)     2287 2024-03-08 16:13:54.000000 exploration-0.7.4/exploration/display.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)    48766 2024-03-08 16:13:54.000000 exploration-0.7.4/exploration/geographic.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)    25500 2024-03-08 16:13:54.000000 exploration-0.7.4/exploration/graphs.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)   253189 2024-03-19 14:41:37.000000 exploration-0.7.4/exploration/journal.py
+-rw-r--r--   0 pmwh      (1000) pmwh      (1000)      321 2024-04-04 04:08:42.000000 exploration-0.7.4/exploration/journal_guide.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)    30557 2024-03-08 16:13:54.000000 exploration-0.7.4/exploration/main.py
+-rw-r--r--   0 pmwh      (1000) pmwh      (1000)    20560 2024-05-16 23:44:19.000000 exploration-0.7.4/exploration/overview.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)   244680 2024-03-10 02:21:23.000000 exploration-0.7.4/exploration/parsing.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)        0 2024-03-08 16:13:54.000000 exploration-0.7.4/exploration/py.typed
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)     8216 2024-03-08 16:13:54.000000 exploration-0.7.4/exploration/utils.py
+drwxr-xr-x   0 pmwh      (1000) pmwh      (1000)        0 2024-05-17 00:40:57.149694 exploration-0.7.4/exploration.egg-info/
+-rw-r--r--   0 pmwh      (1000) pmwh      (1000)    16379 2024-05-17 00:40:56.000000 exploration-0.7.4/exploration.egg-info/PKG-INFO
+-rw-r--r--   0 pmwh      (1000) pmwh      (1000)      606 2024-05-17 00:40:56.000000 exploration-0.7.4/exploration.egg-info/SOURCES.txt
+-rw-r--r--   0 pmwh      (1000) pmwh      (1000)        1 2024-05-17 00:40:56.000000 exploration-0.7.4/exploration.egg-info/dependency_links.txt
+-rw-r--r--   0 pmwh      (1000) pmwh      (1000)       42 2024-05-17 00:40:56.000000 exploration-0.7.4/exploration.egg-info/requires.txt
+-rw-r--r--   0 pmwh      (1000) pmwh      (1000)       12 2024-05-17 00:40:56.000000 exploration-0.7.4/exploration.egg-info/top_level.txt
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)      129 2024-03-08 16:13:54.000000 exploration-0.7.4/pyproject.toml
+drwxr-xr-x   0 pmwh      (1000) pmwh      (1000)        0 2024-05-17 00:40:57.149694 exploration-0.7.4/scripts/
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)     7712 2024-03-01 02:04:24.000000 exploration-0.7.4/scripts/egtool.py
+-rwxr-xr-x   0 pmwh      (1000) pmwh      (1000)     1223 2024-05-17 00:40:57.149694 exploration-0.7.4/setup.cfg
```

### Comparing `exploration-0.7.2/LICENSE.txt` & `exploration-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/PKG-INFO` & `exploration-0.7.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exploration
-Version: 0.7.2
+Version: 0.7.4
 Summary: Tool for reading, formatting, and manipulating exploration graphs, which are graphs (or graph-sequences) that describe exploration of a game space, principally designed with Metroidvania games in mind.
 Home-page: https://cs.wellesley.edu/~pmwh/mvmap/egtool/docs/exploration
 Author: Peter Mawhorter
 Author-email: pmawhort@wellesley.edu
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 3 - Alpha
@@ -89,14 +89,27 @@
 ## Plans
 
 - Better support for open-world games, where decisions are not as closely
     linked to virtual space structure.
 
 ## Changelog
 
+- v0.7.4 fixes some minor issues:
+    * Fixes a bug with mechanism search where relevant transitions were not
+      being used as the search basis in some cases.
+- v0.7.3 adds a bit more:
+    * Journal support for tagging and annotating zones.
+    * `ReqTag` requirements for requiring the presence of a certain tag
+      (or a certain tag value) on some active decision or zone.
+    * `ReqLevel` requirements for requiring a minimum skill level.
+    * Removes the restriction on entering relative mode in an
+      empty/unstarted graph.
+    * Respects current domain when creating new nodes via warps or when
+      there's no current decision.
+    * Adds 'inventory', 'equivalences', and 'mechanisms' debug options.
 - v0.7.2 offers a few more improvements and more API changes (including
   breaking ones):
     * `replaceUnexplored` is now `replaceUnconfirmed`. `unvisited` tag is
       now `unconfirmed`. `core.DecisionGraph.hasBeenVisited` is now
       `core.DecisionGraph.isConfirmed`. Finally a good naming distinction
       between graph confirmation & exploration visited status.
     * Adds 'inspect' mode to the `egtool.py` script and an `inspect`
@@ -112,14 +125,16 @@
       transitions: When `core.DiscreteExploration.advanceSituation` is
       called, each trigger action at an active decision whose
       requirements are satisfied will have its consequences applied.
     * Prevents using 'a'/'action' to take an existing action, requiring
       the use of 't'/'retrace' with the 'actionPart' target instead
       (typically 'ta'). This helps catch issues with action name
       misspellings, and location confusion, among others.
+    * Endings are now warps by default instead of transitions, use
+      'actionPart' (e.g., 'Ea') to mark a voluntary ending.
 - v0.7.1 fixes major bugs with v0.7 and adds a few more nice/important
   things:
     * Transitions may include outcome specifiers, so that in a journal
       you can annotate taking the same transition multiple times and
       getting different results each time for challenges.
     * A new 'save' effect copies game state, which can be restored (in
       whole or in part) via a new 'revertTo' / 'revert'
```

### Comparing `exploration-0.7.2/README.md` & `exploration-0.7.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,27 @@
 ## Plans
 
 - Better support for open-world games, where decisions are not as closely
     linked to virtual space structure.
 
 ## Changelog
 
+- v0.7.4 fixes some minor issues:
+    * Fixes a bug with mechanism search where relevant transitions were not
+      being used as the search basis in some cases.
+- v0.7.3 adds a bit more:
+    * Journal support for tagging and annotating zones.
+    * `ReqTag` requirements for requiring the presence of a certain tag
+      (or a certain tag value) on some active decision or zone.
+    * `ReqLevel` requirements for requiring a minimum skill level.
+    * Removes the restriction on entering relative mode in an
+      empty/unstarted graph.
+    * Respects current domain when creating new nodes via warps or when
+      there's no current decision.
+    * Adds 'inventory', 'equivalences', and 'mechanisms' debug options.
 - v0.7.2 offers a few more improvements and more API changes (including
   breaking ones):
     * `replaceUnexplored` is now `replaceUnconfirmed`. `unvisited` tag is
       now `unconfirmed`. `core.DecisionGraph.hasBeenVisited` is now
       `core.DecisionGraph.isConfirmed`. Finally a good naming distinction
       between graph confirmation & exploration visited status.
     * Adds 'inspect' mode to the `egtool.py` script and an `inspect`
@@ -85,14 +98,16 @@
       transitions: When `core.DiscreteExploration.advanceSituation` is
       called, each trigger action at an active decision whose
       requirements are satisfied will have its consequences applied.
     * Prevents using 'a'/'action' to take an existing action, requiring
       the use of 't'/'retrace' with the 'actionPart' target instead
       (typically 'ta'). This helps catch issues with action name
       misspellings, and location confusion, among others.
+    * Endings are now warps by default instead of transitions, use
+      'actionPart' (e.g., 'Ea') to mark a voluntary ending.
 - v0.7.1 fixes major bugs with v0.7 and adds a few more nice/important
   things:
     * Transitions may include outcome specifiers, so that in a journal
       you can annotate taking the same transition multiple times and
       getting different results each time for challenges.
     * A new 'save' effect copies game state, which can be restored (in
       whole or in part) via a new 'revertTo' / 'revert'
```

### Comparing `exploration-0.7.2/exploration/__init__.py` & `exploration-0.7.4/exploration/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 (see `exploration.journal`), and this version contains nascent code for
 dealing with open-world exploration in terms of geographic features (see
 `geographic.py`). See ../README.md (or
 [https://pypi.org/project/exploration/](https://pypi.org/project/exploration/))
 for project README.
 """
 
-__version__ = "0.7.2"
+__version__ = "0.7.4"
 
 # Imports define what's available when you do `import exploration`
 from .core import *  # noqa
 from . import (  # noqa F401
     base,
     commands,
     parsing,
```

### Comparing `exploration-0.7.2/exploration/__main__.py` & `exploration-0.7.4/exploration/__main__.py`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/exploration/analysis.py` & `exploration-0.7.4/exploration/analysis.py`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/exploration/base.py` & `exploration-0.7.4/exploration/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 - `Domain`
 - `Zone`
 - `DecisionID`
 - `DecisionName`
 - `DecisionSpecifier`
 - `AnyDecisionSpecifier`
-- `ZoneInfo`
-- `DefaultZone`
 - `Transition`
 - `TransitionWithOutcomes`
 - `Capability`
 - `Token`
 - `TokenCount`
 - `Skill`
 - `Level`
@@ -59,14 +57,16 @@
     - `ReqImpossible`
 - `Tag`
 - `TagValueTypes`
 - `TagValue`
 - `NoTagValue`
 - `TagUpdateFunction`
 - `Annotations`
+- `ZoneInfo`
+- `DefaultZone`
 - `ExplorationActionType`
 - `ExplorationAction`
 - `DecisionType`
 - `Situation`
 - `PointID`
 - `Coords`
 - `AnyPoint`
@@ -237,39 +237,14 @@
 
 class InvalidMechanismSpecifierError(ValueError):
     """
     An error used when a mechanism specifier is invalid.
     """
 
 
-class ZoneInfo(NamedTuple):
-    """
-    Zone info holds a level integer (starting from 0 as the level directly
-    above decisions), a set of parent zones, and a set of child decisions
-    and/or zones. Zones at a particular level may only contain zones in lower
-    levels, although zones at any level may also contain decisions directly.
-    The norm is for zones at level 0 to contain decisions, while zones at
-    higher levels contain zones from the level directly below them.
-
-    Note that zones may have multiple parents, because one sub-zone may be
-    contained within multiple super-zones.
-    """
-    level: int
-    parents: Set[Zone]
-    contents: Set[Union[DecisionID, Zone]]
-
-
-class DefaultZone:
-    """
-    Default argument for a `Zone` when `None` is used to mean "Do not add
-    to the zone you normally would."
-    """
-    pass
-
-
 Transition: 'TypeAlias' = str
 """
 A type alias: transitions are defined by their names.
 
 A transition represents a means of travel from one decision to another.
 Outgoing transition names have to be unique at each decision, but not
 globally.
@@ -662,15 +637,15 @@
         primary decision that is being considered in this state. Whereas
         the focalization structures can and often will indicate multiple
         active decisions, whichever decision the player just arrived at
         via the transition selected in a previous state will be the most
         relevant, and we track that here. Of course, for some states
         (like a pre-starting initial state) there is no primary
         decision.
-    - 'mechanisms': A dictionary mapping `Mechanism` names to
+    - 'mechanisms': A dictionary mapping `Mechanism` IDs to
         `MechanismState` strings.
     - 'exploration': A dictionary mapping decision IDs to exploration
         statuses, which tracks how much knowledge the player has of
         different decisions.
     - 'effectCounts': A dictionary mapping `EffectSpecifier`s to
         integers specifying how many times that effect has been
         triggered since the beginning of the exploration (including
@@ -1312,14 +1287,16 @@
     >>> rg, rs = revertedState((g2, s1), (g, s0), {'graph'})
     >>> rg == g
     True
     >>> rg is g
     False
 
     TODO: More tests for various other reversion aspects
+    TODO: Implement per-token-type / per-capability / per-mechanism /
+    per-skill reversion.
     """
     # Expand custom references
     expandedAspects = set()
     queue = list(revisionAspects)
     if len(queue) == 0:
         queue = [  # don't revert skills, exploration, and graph
             "common-capabilities",
@@ -1775,15 +1752,16 @@
         result['value'] = gain
     elif lose is not None:
         result['type'] = 'lose'
         result['value'] = lose
     elif set is not None:
         result['type'] = 'set'
         if (
-            isinstance(set[0], MechanismName)
+            len(set) == 2
+        and isinstance(set[0], MechanismName)
         and isinstance(set[1], MechanismState)
         ):
             result['value'] = (
                 MechanismSpecifier(None, None, None, set[0]),
                 set[1]
             )
         else:
@@ -4001,14 +3979,143 @@
                 mspec += zone + '::'
             if decision is not None:
                 mspec += decision + '::'
             mspec += mechanism
             return f'{mspec}:{self.reqState}'
 
 
+class ReqLevel(Requirement):
+    """
+    A tag requirement satisfied if a specific skill is at or above the
+    specified level.
+    """
+    def __init__(
+        self,
+        skill: Skill,
+        minLevel: Level,
+    ) -> None:
+        self.skill = skill
+        self.minLevel = minLevel
+
+    def __hash__(self) -> int:
+        return (
+            (79 * hash(self.skill))
+          + (55 * hash(self.minLevel))
+        )
+
+    def __eq__(self, other: Any) -> bool:
+        return (
+            isinstance(other, ReqLevel)
+        and other.skill == self.skill
+        and other.minLevel == self.minLevel
+        )
+
+    def __repr__(self):
+        sRep = repr(self.skill)
+        lRep = repr(self.minLevel)
+        return f"ReqLevel({sRep}, {lRep})"
+
+    def satisfied(
+        self,
+        context: RequirementContext,
+        dontRecurse: Optional[
+            Set[Union[Capability, Tuple[MechanismID, MechanismState]]]
+        ] = None
+    ) -> bool:
+        return getSkillLevel(context.state, self.skill) >= self.minLevel
+
+    def walk(self) -> Generator[Requirement, None, None]:
+        yield self
+
+    def asEffectList(self) -> List[Effect]:
+        """
+        Returns a list containing a single 'set' effect which sets the
+        required skill to the minimum required level. Note that this may
+        reduce a skill level that was more than sufficient to meet the
+        requirement.
+        """
+        return [effect(set=("skill", self.skill, self.minLevel))]
+
+    def unparse(self) -> str:
+        return f'{self.skill}^{self.minLevel}'
+
+
+class ReqTag(Requirement):
+    """
+    A tag requirement satisfied if there is any active decision that has
+    the specified value for the given tag (default value is 1 for tags
+    where a value wasn't specified). Zone tags also satisfy the
+    requirement if they're applied to zones that include active
+    decisions.
+    """
+    def __init__(
+        self,
+        tag: "Tag",
+        value: "TagValue",
+    ) -> None:
+        self.tag = tag
+        self.value = value
+
+    def __hash__(self) -> int:
+        return (
+            (71 * hash(self.tag))
+          + (43 * hash(self.value))
+        )
+
+    def __eq__(self, other: Any) -> bool:
+        return (
+            isinstance(other, ReqTag)
+        and other.tag == self.tag
+        and other.value == self.value
+        )
+
+    def __repr__(self):
+        tRep = repr(self.tag)
+        vRep = repr(self.value)
+        return f"ReqTag({tRep}, {vRep})"
+
+    def satisfied(
+        self,
+        context: RequirementContext,
+        dontRecurse: Optional[
+            Set[Union[Capability, Tuple[MechanismID, MechanismState]]]
+        ] = None
+    ) -> bool:
+        active = combinedDecisionSet(context.state)
+        graph = context.graph
+        zones = set()
+        for decision in active:
+            tags = graph.decisionTags(decision)
+            if self.tag in tags and tags[self.tag] == self.value:
+                return True
+            zones |= graph.zoneAncestors(decision)
+        for zone in zones:
+            zTags = graph.zoneTags(zone)
+            if self.tag in zTags and zTags[self.tag] == self.value:
+                return True
+
+        return False
+
+    def walk(self) -> Generator[Requirement, None, None]:
+        yield self
+
+    def asEffectList(self) -> List[Effect]:
+        """
+        Returns a list containing a single 'set' effect which sets the
+        required mechanism to the required state.
+        """
+        raise TypeError(
+            "Cannot convert ReqTag into an effect list:"
+            " effects cannot apply/remove/change tags"
+        )
+
+    def unparse(self) -> str:
+        return f'{self.tag}~{self.value!r}'
+
+
 class ReqNothing(Requirement):
     """
     A requirement representing that something doesn't actually have a
     requirement. This requirement is always satisfied.
     """
     def __hash__(self) -> int:
         return 127942
@@ -4210,14 +4317,46 @@
 """
 
 
 Annotation: 'TypeAlias' = str
 "A type alias: annotations are strings."
 
 
+#-------#
+# Zones #
+#-------#
+
+class ZoneInfo(NamedTuple):
+    """
+    Zone info holds a level integer (starting from 0 as the level directly
+    above decisions), a set of parent zones, a set of child decisions
+    and/or zones, and zone tags and annotations. Zones at a particular
+    level may only contain zones in lower levels, although zones at any
+    level may also contain decisions directly.  The norm is for zones at
+    level 0 to contain decisions, while zones at higher levels contain
+    zones from the level directly below them.
+
+    Note that zones may have multiple parents, because one sub-zone may be
+    contained within multiple super-zones.
+    """
+    level: int
+    parents: Set[Zone]
+    contents: Set[Union[DecisionID, Zone]]
+    tags: Dict[Tag, TagValue]
+    annotations: List[Annotation]
+
+
+class DefaultZone:
+    """
+    Default argument for a `Zone` when `None` is used to mean "Do not add
+    to the zone you normally would."
+    """
+    pass
+
+
 #----------------------------------#
 # Exploration actions & Situations #
 #----------------------------------#
 
 ExplorationActionType = Literal[
     'noAction',
     'start',
```

### Comparing `exploration-0.7.2/exploration/commands.py` & `exploration-0.7.4/exploration/commands.py`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/exploration/core.py` & `exploration-0.7.4/exploration/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,19 +426,14 @@
 
         self.unknownCount: int = 0
         """
         Number of unknown decisions that have been created (not number
         of current unknown decisions, which is likely lower)
         """
 
-        self.zoneTagDicts: Dict[base.Zone, Dict[base.Tag, base.TagValue]] = {}
-        """
-        Tags applied to zones, rather than decisions or edges.
-        """
-
         self.equivalences: base.Equivalences = {}
         """
         See `base.Equivalences`. Determines what capabilities and/or
         mechanism states can count as active based on alternate
         requirements.
         """
 
@@ -499,18 +494,14 @@
             if self.unknownCount != other.unknownCount:
                 return False
 
             # Check zones
             if self.zones != other.zones:
                 return False
 
-            # Check zone tags
-            if self.zoneTagDicts != other.zoneTagDicts:
-                return False
-
             # Check equivalences
             if self.equivalences != other.equivalences:
                 return False
 
             # Check reversion types
             if self.reversionTypes != other.reversionTypes:
                 return False
@@ -635,18 +626,14 @@
             if self.unknownCount != other.unknownCount:
                 yield "unknown count is different"
 
             # Check zones
             if self.zones != other.zones:
                 yield "zones are different"
 
-            # Check zoneTagDicts
-            if self.zoneTagDicts != other.zoneTagDicts:
-                yield "zoneTagDicts are different"
-
             # Check equivalences
             if self.equivalences != other.equivalences:
                 yield "equivalences are different"
 
             # Check reversion types
             if self.reversionTypes != other.reversionTypes:
                 yield "reversionTypes are different"
@@ -743,19 +730,22 @@
         >>> g.addDecision('C')
         2
         >>> g.addDecision('A')
         3
         >>> g.addDecision('B', 'menu')
         4
         >>> g.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('Z2', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('Zup', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addDecisionToZone(0, 'Z')
         >>> g.addDecisionToZone(1, 'Z')
         >>> g.addDecisionToZone(2, 'Z')
         >>> g.addDecisionToZone(3, 'Z2')
         >>> g.addZoneToZone('Z', 'Zup')
         >>> g.addZoneToZone('Z2', 'Zup')
         >>> g.resolveDecision(1)
@@ -1023,19 +1013,22 @@
         >>> g.addDecision('C')
         2
         >>> g.namesListing(['A', 'C', 'B'])
         '  0 (A)\\n  2 (C)\\n  1 (B)\\n'
         >>> g.namesListing([])
         '  (none)\\n'
         >>> g.createZone('zone', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('zone2', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('zoneUp', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addDecisionToZone(0, 'zone')
         >>> g.addDecisionToZone(1, 'zone')
         >>> g.addDecisionToZone(1, 'zone2')
         >>> g.addDecisionToZone(2, 'zoneUp')  # won't be listed: it's level-1
         >>> g.namesListing(['A', 'C', 'B'])
         '  0 (zone::A)\\n  2 (C)\\n  1 ([zone, zone2]::B)\\n'
         """
@@ -1082,15 +1075,16 @@
         >>> g.destinationsListing(g.destinationsFrom('A'))
         '  north to 1 (B)\\n  northeast to 2 (C)\\n'
         >>> g.destinationsListing(g.destinationsFrom('B'))
         '  south to 0 (A)\\n  east to 2 (C)\\n'
         >>> g.destinationsListing({})
         '  (none)\\n'
         >>> g.createZone('zone', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addDecisionToZone(0, 'zone')
         >>> g.destinationsListing(g.destinationsFrom('B'))
         '  south to 0 (zone::A)\\n  east to 2 (C)\\n'
         """
         ind = ' ' * indent
         if len(destinations) == 0:
             return ind + '(none)\n'
@@ -1829,14 +1823,43 @@
         dest = self.destination(dID, transition)
         info = cast(
             TransitionProperties,
             self.edges[dID, dest, transition]  # type:ignore
         )
         return info['annotations']
 
+    def annotateZone(
+        self,
+        zone: base.Zone,
+        annotations: Union[base.Annotation, Sequence[base.Annotation]]
+    ) -> None:
+        """
+        Adds an annotation (or many annotations from a sequence) to a
+        zone.
+
+        Raises a `MissingZoneError` if the specified zone does not exist.
+        """
+        if zone not in self.zones:
+            raise MissingZoneError(
+                f"Can't add annotation(s) to zone {zone!r} because that"
+                f" zone doesn't exist yet."
+            )
+
+        if isinstance(annotations, base.Annotation):
+            annotations = [ annotations ]
+
+        self.zones[zone].annotations.extend(annotations)
+
+    def zoneAnnotations(self, zone: base.Zone) -> List[base.Annotation]:
+        """
+        Returns the list of annotations for the specified zone (empty if
+        none have been added yet).
+        """
+        return self.zones[zone].annotations
+
     def tagZone(
         self,
         zone: base.Zone,
         tagOrTags: Union[base.Tag, Dict[base.Tag, base.TagValue]],
         tagValue: Union[
             base.TagValue,
             type[base.NoTagValue]
@@ -1867,15 +1890,15 @@
 
         elif tagValue is not base.NoTagValue:
             raise ValueError(
                 "Provided a dictionary to update multiple tags, but"
                 " also a tag value."
             )
 
-        tagsAlready = self.zoneTagDicts.setdefault(zone, {})
+        tagsAlready = self.zones[zone].tags
         tagsAlready.update(tagOrTags)
 
     def untagZone(
         self,
         zone: base.Zone,
         tag: base.Tag
     ) -> Union[base.TagValue, type[base.NoTagValue]]:
@@ -1887,61 +1910,58 @@
         Raises a `MissingZoneError` if the specified zone does not exist.
         """
         if zone not in self.zones:
             raise MissingZoneError(
                 f"Can't remove tag {tag!r} from zone {zone!r} because"
                 f" that zone doesn't exist yet."
             )
-        target = self.zoneTagDicts.setdefault(zone, {})
+        target = self.zones[zone].tags
         try:
             return target.pop(tag)
         except KeyError:
             return base.NoTagValue
 
     def zoneTags(
         self,
         zone: base.Zone
     ) -> Dict[base.Tag, base.TagValue]:
         """
         Returns the dictionary of tags for a zone. Edits to the returned
-        value will be applied to the graph. Creates and returns an empty
-        tags dictionary if called on a zone that didn't have any tags
-        previously, but raises a `MissingZoneError` if attempting to tag
-        a zone which does not exist.
+        value will be applied to the graph. Returns an empty tags
+        dictionary if called on a zone that didn't have any tags
+        previously, but raises a `MissingZoneError` if attempting to get
+        tags for a zone which does not exist.
 
         For example:
 
         >>> g = DecisionGraph()
         >>> g.addDecision('A')
         0
         >>> g.addDecision('B')
         1
         >>> g.createZone('Zone')
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.tagZone('Zone', 'color', 'blue')
         >>> g.tagZone(
         ...     'Zone',
         ...     {'shape': 'square', 'color': 'red', 'sound': 'loud'}
         ... )
         >>> g.untagZone('Zone', 'sound')
         'loud'
         >>> g.zoneTags('Zone')
         {'color': 'red', 'shape': 'square'}
         """
-        # TODO: Merge this in with ZoneInfo? That would be cleaner
-        if zone in self.zoneTagDicts:
-            return self.zoneTagDicts.setdefault(zone, {})
-        else:
-            if zone not in self.zones:
-                raise MissingZoneError(
-                    f"Tags for zone {zone!r} don't exist because that"
-                    f" zone has not been created yet."
-                )
-            else:
-                return self.zoneTagDicts.setdefault(zone, {})
+        if zone in self.zones:
+            return self.zones[zone].tags
+        else:
+            raise MissingZoneError(
+                f"Tags for zone {zone!r} don't exist because that"
+                f" zone has not been created yet."
+            )
 
     def createZone(self, zone: base.Zone, level: int = 0) -> base.ZoneInfo:
         """
         Creates an empty zone with the given name at the given level
         (default 0). Raises a `ZoneCollisionError` if that zone name is
         already in use (at any level), including if it's in use by a
         decision.
@@ -1950,19 +1970,22 @@
 
         Returns the `ZoneInfo` for the new blank zone.
 
         For example:
 
         >>> d = DecisionGraph()
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('Z2', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('Z3', -1)  # level -1 is not valid (must be >= 0)
         Traceback (most recent call last):
         ...
         exploration.core.InvalidLevelError...
         >>> d.createZone('Z2')  # Name Z2 is already in use
         Traceback (most recent call last):
         ...
@@ -1978,35 +2001,41 @@
             raise ZoneCollisionError(
                 f"A decision named {zone!r} already exists, so a zone"
                 f" with that name cannot be created."
             )
         info: base.ZoneInfo = base.ZoneInfo(
             level=level,
             parents=set(),
-            contents=set()
+            contents=set(),
+            tags={},
+            annotations=[]
         )
         self.zones[zone] = info
         return info
 
     def getZoneInfo(self, zone: base.Zone) -> Optional[base.ZoneInfo]:
         """
         Returns the `ZoneInfo` (level, parents, and contents) for the
         specified zone, or `None` if that zone does not exist.
 
         For example:
 
         >>> d = DecisionGraph()
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('Z2', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.getZoneInfo('Z2')
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         """
         return self.zones.get(zone)
 
     def deleteZone(self, zone: base.Zone) -> base.ZoneInfo:
         """
         Deletes the specified zone, returning a `ZoneInfo` object with
         the information on the level, parents, and contents of that zone.
@@ -2014,19 +2043,22 @@
         Raises a `MissingZoneError` if the zone in question does not
         exist.
 
         For example:
 
         >>> d = DecisionGraph()
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.deleteZone('Z')
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.getZoneInfo('Z') is None  # no info any more
         True
         >>> d.deleteZone('Z')  # can't re-delete
         Traceback (most recent call last):
         ...
         exploration.core.MissingZoneError...
         """
@@ -2060,21 +2092,24 @@
         >>> d.addDecision('A')
         0
         >>> d.addDecision('B')
         1
         >>> d.addDecision('C')
         2
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addDecisionToZone('A', 'Z')
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents=set(), contents={0})
+        ZoneInfo(level=0, parents=set(), contents={0}, tags={},\
+ annotations=[])
         >>> d.addDecisionToZone('B', 'Z')
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents=set(), contents={0, 1})
+        ZoneInfo(level=0, parents=set(), contents={0, 1}, tags={},\
+ annotations=[])
         """
         dID = self.resolveDecision(decision)
 
         if zone not in self.zones:
             raise MissingZoneError(f"Zone {zone!r} does not exist.")
 
         self.zones[zone].contents.add(dID)
@@ -2100,21 +2135,25 @@
 
         >>> g = DecisionGraph()
         >>> g.addDecision('A')
         0
         >>> g.addDecision('B')
         1
         >>> g.createZone('level0', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level1', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level2', 2)
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level3', 3)
-        ZoneInfo(level=3, parents=set(), contents=set())
+        ZoneInfo(level=3, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addDecisionToZone('A', 'level0')
         >>> g.addDecisionToZone('B', 'level0')
         >>> g.addZoneToZone('level0', 'level1')
         >>> g.addZoneToZone('level1', 'level2')
         >>> g.addZoneToZone('level2', 'level3')
         >>> g.addDecisionToZone('B', 'level2')  # Direct w/ skips
         >>> g.removeDecisionFromZone('A', 'level1')
@@ -2176,42 +2215,53 @@
         >>> d.addDecision('A')
         0
         >>> d.addDecision('B')
         1
         >>> d.addDecision('C')
         2
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addDecisionToZone('A', 'Z')
         >>> d.addDecisionToZone('B', 'Z')
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents=set(), contents={0, 1})
+        ZoneInfo(level=0, parents=set(), contents={0, 1}, tags={},\
+ annotations=[])
         >>> d.createZone('Z2', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addDecisionToZone('B', 'Z2')
         >>> d.addDecisionToZone('C', 'Z2')
         >>> d.getZoneInfo('Z2')
-        ZoneInfo(level=0, parents=set(), contents={1, 2})
+        ZoneInfo(level=0, parents=set(), contents={1, 2}, tags={},\
+ annotations=[])
         >>> d.createZone('l1Z', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('l2Z', 2)
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addZoneToZone('Z', 'l1Z')
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents={'l1Z'}, contents={0, 1})
+        ZoneInfo(level=0, parents={'l1Z'}, contents={0, 1}, tags={},\
+ annotations=[])
         >>> d.getZoneInfo('l1Z')
-        ZoneInfo(level=1, parents=set(), contents={'Z'})
+        ZoneInfo(level=1, parents=set(), contents={'Z'}, tags={},\
+ annotations=[])
         >>> d.addZoneToZone('l1Z', 'l2Z')
         >>> d.getZoneInfo('l1Z')
-        ZoneInfo(level=1, parents={'l2Z'}, contents={'Z'})
+        ZoneInfo(level=1, parents={'l2Z'}, contents={'Z'}, tags={},\
+ annotations=[])
         >>> d.getZoneInfo('l2Z')
-        ZoneInfo(level=2, parents=set(), contents={'l1Z'})
+        ZoneInfo(level=2, parents=set(), contents={'l1Z'}, tags={},\
+ annotations=[])
         >>> d.addZoneToZone('Z2', 'l2Z')
         >>> d.getZoneInfo('Z2')
-        ZoneInfo(level=0, parents={'l2Z'}, contents={1, 2})
+        ZoneInfo(level=0, parents={'l2Z'}, contents={1, 2}, tags={},\
+ annotations=[])
         >>> l2i = d.getZoneInfo('l2Z')
         >>> l2i.level
         2
         >>> l2i.parents
         set()
         >>> sorted(l2i.contents)
         ['Z2', 'l1Z']
@@ -2224,18 +2274,20 @@
         >>> zi.level
         0
         >>> sorted(zi.parents)
         ['l1Z', 'l1Z2']
         >>> sorted(zi.contents)
         [0, 1]
         >>> d.getZoneInfo('l1Z2')
-        ZoneInfo(level=1, parents=set(), contents={'Z'})
+        ZoneInfo(level=1, parents=set(), contents={'Z'}, tags={},\
+ annotations=[])
         >>> d.addZoneToZone('NZ', 'l1Z')
         >>> d.getZoneInfo('NZ')
-        ZoneInfo(level=0, parents={'l1Z'}, contents=set())
+        ZoneInfo(level=0, parents={'l1Z'}, contents=set(), tags={},\
+ annotations=[])
         >>> zi = d.getZoneInfo('l1Z')
         >>> zi.level
         1
         >>> zi.parents
         {'l2Z'}
         >>> sorted(zi.contents)
         ['NZ', 'Z']
@@ -2293,41 +2345,52 @@
         if that zone had been in that zone, and False if it was not in
         that zone, including if either zone did not exist.
 
         For example:
 
         >>> d = DecisionGraph()
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('Z2', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('l1Z', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('l2Z', 2)
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addZoneToZone('Z', 'l1Z')
         >>> d.addZoneToZone('l1Z', 'l2Z')
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents={'l1Z'}, contents=set())
+        ZoneInfo(level=0, parents={'l1Z'}, contents=set(), tags={},\
+ annotations=[])
         >>> d.getZoneInfo('l1Z')
-        ZoneInfo(level=1, parents={'l2Z'}, contents={'Z'})
+        ZoneInfo(level=1, parents={'l2Z'}, contents={'Z'}, tags={},\
+ annotations=[])
         >>> d.getZoneInfo('l2Z')
-        ZoneInfo(level=2, parents=set(), contents={'l1Z'})
+        ZoneInfo(level=2, parents=set(), contents={'l1Z'}, tags={},\
+ annotations=[])
         >>> d.removeZoneFromZone('l1Z', 'l2Z')
         True
         >>> d.getZoneInfo('l1Z')
-        ZoneInfo(level=1, parents=set(), contents={'Z'})
+        ZoneInfo(level=1, parents=set(), contents={'Z'}, tags={},\
+ annotations=[])
         >>> d.getZoneInfo('l2Z')
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.removeZoneFromZone('Z', 'l1Z')
         True
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.getZoneInfo('l1Z')
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.removeZoneFromZone('Z', 'l1Z')
         False
         >>> d.removeZoneFromZone('Z', 'madeup')
         False
         >>> d.removeZoneFromZone('nope', 'madeup')
         False
         >>> d.removeZoneFromZone('nope', 'l1Z')
@@ -2363,33 +2426,38 @@
         >>> d.addDecision('A')
         0
         >>> d.addDecision('B')
         1
         >>> d.addDecision('C')
         2
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addDecisionToZone('A', 'Z')
         >>> d.addDecisionToZone('B', 'Z')
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents=set(), contents={0, 1})
+        ZoneInfo(level=0, parents=set(), contents={0, 1}, tags={},\
+ annotations=[])
         >>> d.decisionsInZone('Z')
         {0, 1}
         >>> d.createZone('Z2', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addDecisionToZone('B', 'Z2')
         >>> d.addDecisionToZone('C', 'Z2')
         >>> d.getZoneInfo('Z2')
-        ZoneInfo(level=0, parents=set(), contents={1, 2})
+        ZoneInfo(level=0, parents=set(), contents={1, 2}, tags={},\
+ annotations=[])
         >>> d.decisionsInZone('Z')
         {0, 1}
         >>> d.decisionsInZone('Z2')
         {1, 2}
         >>> d.createZone('l1Z', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addZoneToZone('Z', 'l1Z')
         >>> d.decisionsInZone('Z')
         {0, 1}
         >>> d.decisionsInZone('l1Z')
         set()
         >>> d.decisionsInZone('madeup')
         Traceback (most recent call last):
@@ -2421,19 +2489,21 @@
 
         The returned set is a copy, not a live editable set.
 
         For example:
 
         >>> d = DecisionGraph()
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.subZones('Z')
         set()
         >>> d.createZone('l1Z', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addZoneToZone('Z', 'l1Z')
         >>> d.subZones('Z')
         set()
         >>> d.subZones('l1Z')
         {'Z'}
         >>> s = d.subZones('l1Z')
         >>> s.add('Q')  # doesn't affect the zone
@@ -2471,39 +2541,45 @@
         >>> d.addDecision('A')
         0
         >>> d.addDecision('B')
         1
         >>> d.addDecision('C')
         2
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addDecisionToZone('A', 'Z')
         >>> d.addDecisionToZone('B', 'Z')
         >>> d.getZoneInfo('Z')
-        ZoneInfo(level=0, parents=set(), contents={0, 1})
+        ZoneInfo(level=0, parents=set(), contents={0, 1}, tags={},\
+ annotations=[])
         >>> d.decisionsInZone('Z')
         {0, 1}
         >>> d.allDecisionsInZone('Z')
         {0, 1}
         >>> d.createZone('Z2', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addDecisionToZone('B', 'Z2')
         >>> d.addDecisionToZone('C', 'Z2')
         >>> d.getZoneInfo('Z2')
-        ZoneInfo(level=0, parents=set(), contents={1, 2})
+        ZoneInfo(level=0, parents=set(), contents={1, 2}, tags={},\
+ annotations=[])
         >>> d.decisionsInZone('Z')
         {0, 1}
         >>> d.decisionsInZone('Z2')
         {1, 2}
         >>> d.allDecisionsInZone('Z2')
         {1, 2}
         >>> d.createZone('l1Z', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('l2Z', 2)
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addZoneToZone('Z', 'l1Z')
         >>> d.addZoneToZone('l1Z', 'l2Z')
         >>> d.addZoneToZone('Z2', 'l2Z')
         >>> d.decisionsInZone('Z')
         {0, 1}
         >>> d.decisionsInZone('Z2')
         {1, 2}
@@ -2536,19 +2612,22 @@
         Raises a `MissingZoneError` if the specified zone does not
         exist.
 
         For example:
 
         >>> d = DecisionGraph()
         >>> d.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('l1Z', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('l5Z', 5)
-        ZoneInfo(level=5, parents=set(), contents=set())
+        ZoneInfo(level=5, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.zoneHierarchyLevel('Z')
         0
         >>> d.zoneHierarchyLevel('l1Z')
         1
         >>> d.zoneHierarchyLevel('l5Z')
         5
         >>> d.zoneHierarchyLevel('madeup')
@@ -2579,21 +2658,25 @@
 
         >>> g = DecisionGraph()
         >>> g.addDecision('A')
         0
         >>> g.addDecision('B')
         1
         >>> g.createZone('level0', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level1', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level2', 2)
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level3', 3)
-        ZoneInfo(level=3, parents=set(), contents=set())
+        ZoneInfo(level=3, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addDecisionToZone('A', 'level0')
         >>> g.addDecisionToZone('B', 'level0')
         >>> g.addZoneToZone('level0', 'level1')
         >>> g.addZoneToZone('level1', 'level2')
         >>> g.addZoneToZone('level2', 'level3')
         >>> g.addDecisionToZone('B', 'level2')  # Direct w/ skips
         >>> sorted(g.zoneParents(0))
@@ -2634,21 +2717,25 @@
 
         >>> g = DecisionGraph()
         >>> g.addDecision('A')
         0
         >>> g.addDecision('B')
         1
         >>> g.createZone('level0', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level1', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level2', 2)
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level3', 3)
-        ZoneInfo(level=3, parents=set(), contents=set())
+        ZoneInfo(level=3, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addDecisionToZone('A', 'level0')
         >>> g.addDecisionToZone('B', 'level0')
         >>> g.addZoneToZone('level0', 'level1')
         >>> g.addZoneToZone('level1', 'level2')
         >>> g.addZoneToZone('level2', 'level3')
         >>> g.addDecisionToZone('B', 'level2')  # Direct w/ skips
         >>> sorted(g.zoneAncestors(0))
@@ -2702,17 +2789,19 @@
         3
         >>> g.addTransition('A', 'up', 'B', 'down')
         >>> g.addTransition('B', 'right', 'C', 'left')
         >>> g.addTransition('C', 'down', 'D', 'up')
         >>> g.addTransition('D', 'left', 'A', 'right')
         >>> g.addTransition('A', 'tunnel', 'C', 'tunnel')
         >>> g.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('ZZ', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addZoneToZone('Z', 'ZZ')
         >>> g.addDecisionToZone('A', 'Z')
         >>> g.addDecisionToZone('B', 'Z')
         >>> g.addDecisionToZone('D', 'ZZ')
         >>> outgoing, incoming = g.zoneEdges('Z')  # TODO: Sort for testing
         >>> sorted(outgoing)
         [(0, 'right'), (0, 'tunnel'), (1, 'right')]
@@ -2805,23 +2894,28 @@
 
         >>> g = DecisionGraph()
         >>> g.addDecision('decision')
         0
         >>> g.addDecision('alternate')
         1
         >>> g.createZone('zone0', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('zone1', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('zone2.1', 2)
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('zone2.2', 2)
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('zone3', 3)
-        ZoneInfo(level=3, parents=set(), contents=set())
+        ZoneInfo(level=3, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addDecisionToZone('decision', 'zone0')
         >>> g.addDecisionToZone('alternate', 'zone0')
         >>> g.addZoneToZone('zone0', 'zone1')
         >>> g.addZoneToZone('zone1', 'zone2.1')
         >>> g.addZoneToZone('zone1', 'zone2.2')
         >>> g.addZoneToZone('zone2.1', 'zone3')
         >>> g.addZoneToZone('zone2.2', 'zone3')
@@ -2934,21 +3028,25 @@
 
         >>> g = DecisionGraph()
         >>> g.addDecision('A')
         0
         >>> g.addDecision('B')
         1
         >>> g.createZone('level0', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level1', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level2', 2)
-        ZoneInfo(level=2, parents=set(), contents=set())
+        ZoneInfo(level=2, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.createZone('level3', 3)
-        ZoneInfo(level=3, parents=set(), contents=set())
+        ZoneInfo(level=3, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addDecisionToZone('B', 'level0')
         >>> g.addZoneToZone('level0', 'level1')
         >>> g.addZoneToZone('level1', 'level2')
         >>> g.addZoneToZone('level2', 'level3')
         >>> g.addDecisionToZone('A', 'level3') # missing some zone levels
         >>> g.zoneHierarchyLevel('level3')
         3
@@ -3914,19 +4012,22 @@
         >>> d.addMechanism('switch', 'C')
         2
         >>> d.addMechanism('lever', 'D')
         3
         >>> d.addMechanism('lever', None)  # global
         4
         >>> d.createZone('Z1', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('Z2', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.createZone('Zup', 1)
-        ZoneInfo(level=1, parents=set(), contents=set())
+        ZoneInfo(level=1, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> d.addDecisionToZone('A', 'Z1')
         >>> d.addDecisionToZone('B', 'Z1')
         >>> d.addDecisionToZone('C', 'Z2')
         >>> d.addDecisionToZone('D', 'Z2')
         >>> d.addDecisionToZone('E', 'Z1')
         >>> d.addZoneToZone('Z1', 'Zup')
         >>> d.addZoneToZone('Z2', 'Zup')
@@ -7514,15 +7615,15 @@
         state at the specified step if a step index is given). `where`
         may be provided as a set of decision IDs to indicate where to
         search for the named mechanism, or a mechanism ID may be provided
         in the first place. Mechanism states are properties of a `State`
         but are not associated with focal contexts.
         """
         situation = self.getSituation(step)
-        mID = situation.graph.resolveMechanism(mechanism)
+        mID = situation.graph.resolveMechanism(mechanism, startFrom=where)
         return situation.state['mechanisms'].get(
             mID,
             base.DEFAULT_MECHANISM_STATE
         )
 
     def setMechanismStateNow(
         self,
@@ -7538,15 +7639,15 @@
 
         The mechanism can be any kind of mechanism specifier (see
         `base.AnyMechanismSpecifier`). If it's not a mechanism ID and
         doesn't have its own position information, the 'where' argument
         can be used to hint where to search for the mechanism.
         """
         now = self.getSituation()
-        mID = now.graph.resolveMechanism(mechanism, where)
+        mID = now.graph.resolveMechanism(mechanism, startFrom=where)
         if mID is None:
             raise MissingMechanismError(
                 f"Couldn't find mechanism for {repr(mechanism)}."
             )
         now.state['mechanisms'][mID] = toState
 
     def skillLevel(
@@ -7882,15 +7983,15 @@
                 mechanism, states = cast(
                     Tuple[
                         base.AnyMechanismSpecifier,
                         List[base.MechanismState]
                     ],
                     value
                 )
-                currentState = self.mechanismState(mechanism, searchFrom)
+                currentState = self.mechanismState(mechanism, where=searchFrom)
                 if len(states) == 1:
                     if currentState == states[0]:
                         # default alternate state
                         self.setMechanismStateNow(
                             mechanism,
                             base.DEFAULT_MECHANISM_STATE,
                             searchFrom
@@ -8866,15 +8967,16 @@
             activeEndings = [
                 d
                 for d in self.getActiveDecisions()
                 if newGraph.domainFor(d) == ENDINGS_DOMAIN
             ]
             raise InvalidActionError(
                 f"Attempted to {action[0]!r} while an ending was"
-                f" active. Active endings are:\n{activeEndings}"
+                f" active. Active endings are:"
+                f"\n{newGraph.namesListing(activeEndings)}"
             )
 
         if action == ('noAction',):
             # No updates needed
             pass
 
         elif (
@@ -10371,15 +10473,16 @@
         exploration.core.TransitionCollisionError...
         >>> e.observe('start', 'right2', 'B', 'left')  # repeat reciprocal
         Traceback (most recent call last):
         ...
         exploration.core.TransitionCollisionError...
         >>> g = e.getSituation().graph
         >>> g.createZone('Z', 0)
-        ZoneInfo(level=0, parents=set(), contents=set())
+        ZoneInfo(level=0, parents=set(), contents=set(), tags={},\
+ annotations=[])
         >>> g.addDecisionToZone('start', 'Z')
         >>> e.observe('start', 'down', 'C', 'up')
         4
         >>> g.destinationsFrom('start')
         {'up': 1, 'left': 2, 'up2': 1, 'right': 3, 'down': 4}
         >>> g.identityOf('C')
         '4 (C)'
```

### Comparing `exploration-0.7.2/exploration/display.py` & `exploration-0.7.4/exploration/display.py`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/exploration/geographic.py` & `exploration-0.7.4/exploration/geographic.py`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/exploration/graphs.py` & `exploration-0.7.4/exploration/graphs.py`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/exploration/journal.py` & `exploration-0.7.4/exploration/journal.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # TODO: Base current decision on primary decision when reverting, and
 # maybe at other points!
 
 from __future__ import annotations
 
 from typing import (
     Optional, List, Tuple, Dict, Union, Collection, get_args, cast,
-    Sequence, Literal, Set, TypedDict
+    Sequence, Literal, Set, TypedDict, get_type_hints
 )
 
 import sys
 import re
 import warnings
 import textwrap
 
@@ -228,22 +228,22 @@
     `True`, regardless of whether they're added to the graph before or
     after the transition they are associated with. Also, certain effects
     like 'bounce' cannot be applied retroactively.
 
 - 'g' / 'tag': Applies one or more tags to the current exploration step,
     or to the current decision if 'decisionPart' is specified, or to
     either the most-recently-taken transition or its reciprocal if
-    'transitionPart' or 'reciprocalPart' is specified. Tags may have
-    values associated with them; without a value provided the default
-    value is the number 1.
+    'transitionPart' or 'reciprocalPart' is specified. May also tag a
+    zone by using 'zonePart'. Tags may have values associated with them;
+    without a value provided the default value is the number 1.
 
 - 'n' / 'annotate': Like 'tag' but applies an annotation, which is just a
     piece of text attached to. Certain annotations will trigger checks of
-    various exploration state and emit warnings if the checks fail.
-    Annotations which begin with:
+    various exploration state when applied to a step, and will emit
+    warnings if the checks fail.Step annotations which begin with:
         * 'at:' - checks that the current primary decision matches the
             decision identified by the rest of the annotation.
         * 'active:' - checks that a decision is currently in the active
             decision set.
         * 'has:' - checks that the player has a specific amount of a
             certain token (write 'token*amount' after 'has:', as in "has:
             coins*3"). Will fail if the player doesn't have that amount,
@@ -323,18 +323,19 @@
     leads to an unknown decision which is not otherwise connected to
     anything, this will also delete that decision (even if it already
     has tags or annotations or the like). Can also be used (with a
     decision target) to delete a decision, which will delete all
     transitions touching that decision. Note that usually, 'unify' is
     easier to manage than extinguish for manipulating decisions.
 
-- 'C' / 'complicate': Takes a transition between two known decisions and
-    adds a new known decision in the middle of it. The old ends of the
-    transition both connect to the new decision, and new names are given
-    to their new reciprocals. Does not change the player's position.
+- 'C' / 'complicate': Takes a transition between two confirmed decisions
+    and adds a new confirmed decision in the middle of it. The old ends
+    of the transition both connect to the new decision, and new names are
+    given to their new reciprocals. Does not change the player's
+    position.
 
 - '.' / 'status': Sets the exploration status of the current decision
     (argument should be a `base.ExplorationStatus`). Without an
     argument, sets the status to 'explored'. When 'unfinishedPart' is
     given as a target specifier (once or twice), this instead prevents
     the decision from being automatically marked as 'explored' when we
     leave it.
@@ -383,71 +384,77 @@
 cases. For example, by default 'g' as an entry type means 'tag', and 't'
 as a target type means 'transition'. So 'gt' as an entry type means 'tag
 transition' and applies the relevant tag to the most-recently-created
 transition instead of the most-recently-created decision. The
 `targetSeparator` character (default '@') is used to combine an entry
 type with a target type when the entry type is written without
 abbreviation. In that case, the target specifier may drop the suffix
-'Part' (e.g., tag@transition in place of `gt`). The available target
+'Part' (e.g., `tag@transition` in place of `gt`). The available target
 parts are each valid only for specific entry types. The target parts are:
 
 - 'decisionPart' - Use to specify that the entry applies to a decision
     when it would normally apply to something else.
 - 'transitionPart' - Use to specify that the entry applies to a
     transition instead of a decision.
 - 'reciprocalPart' - Use to specify that the entry applies to a
     reciprocal transition instead of a decision or the normal
     transition.
 - 'bothPart' - Use to specify that the entry applies to both of two
     possibilities, such as to a transition and its reciprocal.
-- 'zonePart' - Use only for re-zoning to indicate the hierarchy level. May
+- 'zonePart' - Use for re-zoning to indicate the hierarchy level. May
     be repeated; each instance increases the hierarchy level by 1
-    starting from 0.
+    starting from 0. In the long form to specify a hierarchy level, use
+    the letter 'z' followed by an integer, as in 'z3' for level 3. Also
+    used in the same way for tagging or annotating zones.
 - 'actionPart' - Use for the 'observe' or 'retrace' entries to specify
     that the observed/retraced transition is an action (i.e., its
     destination is the same as its source) rather than a real transition
     (whose destination would be a new, unknown node).
 - 'endingPart' - Use only for the 'observe' entry to specify that the
     observed transition goes to an ending rather than a normal decision.
 - 'unfinishedPart' - Use only for the 'status' entry (and use either
-    once or twice) to specify that a decision should NOT be finalized
-    when we leave it.
+    once or twice in the short form) to specify that a decision should
+    NOT be finalized when we leave it.
 
 The entry types where a target specifier can be applied are:
 
 - 'requirement': By default these are applied to transitions, but the
     'reciprocalPart' target can be used to apply to a reciprocal
     instead. Use `bothPart` to apply the same requirement to both the
     transition and its reciprocal.
 - 'effect': Same as 'requirement'.
 - 'apply': Same as 'effect' (and see above).
-- 'tag': Applies the tag to the specified target instead of the
-    most-recently-created decision, which is the default.
-- 'annotation': Same as 'tag', but can also use a decision-part target
-    to annotate the current decision (default is to annotate the
-    exploration step).
+- 'tag': Applies the tag to the specified target instead of the current
+    exploration step. When targeting zones using 'zonePart', if there are
+    multiple zones that apply at a certain hierarchy level we target the
+    smallest one (breaking ties alphabetically by name). TODO: target the
+    most-recently asserted one. The 'zonePart' may be repeated to specify
+    a hierarchy level, as in 'gzz' for level 1 instead of level 0, and
+    you may also use 'z' followed by an integer, as in 'gz3' for level 3.
+- 'annotation': Same as 'tag'.
 - 'unify': By default applies to a decision, but can be applied to a
     transition or reciprocal instead.
 - 'extinguish': By default applies to a transition and its reciprocal,
     but can be applied to just one or the other, or to a decision.
 - 'relative': Only 'transition' applies here and changes the
     most-recent-transition value when entering relative mode instead of
     just changing the current-decision value. Can be used within
     relative mode to pick out an existing transition as well.
-- 'zone': This is the only place where the 'zonePart' target type
+- 'zone': This is the main place where the 'zonePart' target type
     applies, and it can actually be applied as many times as you want.
     Each application makes the zone specified apply to a higher level in
     the hierarchy of zones, so that instead of swapping the level-0 zone
     using 'z', the level-1 zone can be changed using 'zz' or the level 2
-    zone using 'zzz', etc. In lieu of using 'z's, you can also just write
-    as an integer the level you want to use (e.g., z0 for a level-0 zone,
-    or z1 for a level-1 zone). When using a long-form entry type, the
-    target may be given as the string 'zone' in which case the level-1
-    zone is used. To use a different zone level with a long-form entry
-    type, use multiple 'z's, or an integer.
+    zone using 'zzz', etc. In lieu of using multiple 'z's, you can also
+    just write one 'z' followed by an integer for the level you want to
+    use (e.g., z0 for a level-0 zone, or z1 for a level-1 zone). When
+    using a long-form entry type, the target may be given as the string
+    'zone' in which case the level-1 zone is used. To use a different
+    zone level with a long-form entry type, repeat the 'z' followed by an
+    integer, or use multiple 'z's.
 - 'observe': Uses the 'actionPart' and 'endingPart' target types, and
     those are the only applicable target types.  Applying `actionPart`
     turns the observed transition into an action; applying `endingPart`
     turns it into an transition to an ending.
 - 'retrace': Uses 'actionPart' or not to distinguish what kind of
     transition is being taken. Riases a `JournalParseError` if the type
     of edge (external vs. self destination) doesn't match this
@@ -635,15 +642,18 @@
     'here',
     'transition',
     'destinations',
     'steps',
     'decisions',
     'active',
     'primary',
-    'saved'
+    'saved',
+    'inventory',
+    'mechanisms',
+    'equivalences',
 ]
 """
 The different kinds of debugging commands.
 """
 
 
 class JournalParseFormat(parsing.ParseFormat):
@@ -780,15 +790,15 @@
         type.
         """
         return self.journalMarkers[markerType]
 
     def determineEntryType(self, entryBits: List[str]) -> Tuple[
         JournalEntryType,
         base.DecisionType,
-        Union[None, JournalTargetType, int],
+        Union[None, JournalTargetType, Tuple[JournalTargetType, int]],
         List[str]
     ]:
         """
         Given a sequence of strings that specify a command, returns a
         tuple containing the entry type, decision type, target part, and
         list of arguments for that command. The default decision type is
         'active' but others can be specified with decision type
@@ -813,22 +823,34 @@
         ('explore', 'unintended', None, ['down', 'pit', 'up'])
         >>> pf.determineEntryType(['imposed/explore', 'down', 'pit', 'up'])
         ('explore', 'imposed', None, ['down', 'pit', 'up'])
         >>> pf.determineEntryType(['~x', 'down', 'pit', 'up'])
         ('explore', 'consequence', None, ['down', 'pit', 'up'])
         >>> pf.determineEntryType(['>x', 'down', 'pit', 'up'])
         ('explore', 'imposed', None, ['down', 'pit', 'up'])
+        >>> pf.determineEntryType(['gzz', 'tag'])
+        ('tag', 'active', ('zonePart', 1), ['tag'])
+        >>> pf.determineEntryType(['gz4', 'tag'])
+        ('tag', 'active', ('zonePart', 4), ['tag'])
+        >>> pf.determineEntryType(['zone@z2', 'ZoneName'])
+        ('zone', 'active', ('zonePart', 2), ['ZoneName'])
+        >>> pf.determineEntryType(['zzz', 'ZoneName'])
+        ('zone', 'active', ('zonePart', 2), ['ZoneName'])
         """
         # Get entry specifier
         entrySpecifier = entryBits[0]
         entryArgs = entryBits[1:]
 
         # Defaults
         entryType: Optional[JournalEntryType] = None
-        entryTarget: Union[None, JournalTargetType, int] = None
+        entryTarget: Union[
+            None,
+            JournalTargetType,
+            Tuple[JournalTargetType, int]
+        ] = None
         entryDecisionType: base.DecisionType = 'active'
 
         # Check for a decision type specifier and process+remove it
         for decisionType in get_args(base.DecisionType):
             marker = self.markerFor(decisionType)
             lm = len(marker)
             if (
@@ -861,123 +883,145 @@
         and not entrySpecifier.startswith(targetMarker)
             # Because the targetMarker is also a valid entry type!
         ):
             specifierBits = entrySpecifier.split(targetMarker)
             if len(specifierBits) != 2:
                 raise JournalParseError(
                     f"When a long-form entry specifier contains a"
-                    f" colon, it must contain exactly one (to split the"
-                    f" entry type from the entry target). We got"
+                    f" target separator, it must contain exactly one (to"
+                    f" split the entry type from the entry target). We got"
                     f" {entrySpecifier!r}."
                 )
             entryTypeGuess: str
             entryTargetGuess: Optional[str]
             entryTypeGuess, entryTargetGuess = specifierBits
             if entryTypeGuess not in validEntryTypes:
                 raise JournalParseError(
                     f"Invalid long-form entry type: {entryType!r}"
                 )
             else:
                 entryType = cast(JournalEntryType, entryTypeGuess)
 
-            if entryType == 'zone':
-                if entryTargetGuess.isdigit():
-                    entryTarget = int(entryTargetGuess)
-                elif entryTargetGuess in 'zone':
-                    entryTarget = 1
+            # Special logic for zone part
+            handled = False
+            if entryType in ('zone', 'tag', 'annotate'):
+                handled = True
+                if entryType == 'zone' and entryTargetGuess.isdigit():
+                    entryTarget = ('zonePart', int(entryTargetGuess))
+                elif entryTargetGuess == 'zone':
+                    entryTarget = ('zonePart', 1 if entryType == 'zone' else 0)
+                elif (
+                    entryTargetGuess.startswith('z')
+                and entryTargetGuess[1:].isdigit()
+                ):
+                    entryTarget = ('zonePart', int(entryTargetGuess[1:]))
                 elif (
                     len(entryTargetGuess) > 0
                 and set(entryTargetGuess) != {'z'}
                 ):
-                    raise JournalParseError(
-                        f"Invalid target specifier for"
-                        f" zone:\n{entryTargetGuess}"
-                    )
+                    if entryType == 'zone':
+                        raise JournalParseError(
+                            f"Invalid target specifier for"
+                            f" zone entry:\n{entryTargetGuess}"
+                        )
+                    else:
+                        handled = False
                 else:
-                    entryTarget = len(entryTargetGuess)
+                    entryTarget = ('zonePart', len(entryTargetGuess))
 
-            elif entryTargetGuess in validEntryTargets:
-                entryTarget = cast(JournalTargetType, entryTargetGuess)
-
-            else:
+            if not handled:
                 if entryTargetGuess + 'Part' in validEntryTargets:
                     entryTarget = cast(
                         JournalTargetType,
                         entryTargetGuess + 'Part'
                     )
                 else:
                     origGuess = entryTargetGuess
                     entryTargetGuess = self.targetMap.get(
+                        entryTargetGuess,
                         entryTargetGuess
                     )
                     if entryTargetGuess not in validEntryTargets:
                         raise JournalParseError(
                             f"Invalid long-form entry target:"
                             f" {origGuess!r}"
                         )
                     else:
                         entryTarget = cast(
                             JournalTargetType,
                             entryTargetGuess
                         )
 
         elif entrySpecifier in validEntryTypes:
-            # Might be a long-form specifier without a colon
+            # Might be a long-form specifier without a separator
             entryType = cast(JournalEntryType, entrySpecifier)
             entryTarget = None
             if entryType == 'zone':
-                entryTarget = 0
+                entryTarget = ('zonePart', 0)
 
         else:  # parse a short-form entry specifier
             typeSpecifier = entrySpecifier[0]
             if typeSpecifier not in self.entryMap:
                 raise JournalParseError(
                     f"Entry does not begin with a recognized entry"
                     f" marker:\n{entryBits}"
                 )
             entryType = self.entryMap[typeSpecifier]
 
             # Figure out the entry target from second+ character(s)
             targetSpecifiers = entrySpecifier[1:]
+            specifiersSet = set(targetSpecifiers)
             if entryType == 'zone':
-                specifiers = set(targetSpecifiers)
                 if targetSpecifiers.isdigit():
-                    entryTarget = int(targetSpecifiers)
+                    entryTarget = ('zonePart', int(targetSpecifiers))
                 elif (
-                    len(specifiers) > 0
-                and specifiers != {self.journalMarkers['zonePart']}
+                    len(specifiersSet) > 0
+                and specifiersSet != {self.journalMarkers['zonePart']}
                 ):
                     raise JournalParseError(
                         f"Invalid target specifier for zone:\n{entryBits}"
                     )
                 else:
-                    entryTarget = len(targetSpecifiers)
+                    entryTarget = ('zonePart', len(targetSpecifiers))
             elif entryType == 'status':
                 if len(targetSpecifiers) > 0:
                     if any(
                         x != self.journalMarkers['unfinishedPart']
                         for x in targetSpecifiers
                     ):
                         raise JournalParseError(
                             f"Invalid target specifier for"
                             f" status:\n{entryBits}"
                         )
                     entryTarget = 'unfinishedPart'
                 else:
                     entryTarget = None
             elif len(targetSpecifiers) > 0:
-                if len(targetSpecifiers) > 1:
-                    raise JournalParseError(
-                        f"Entry has too many target specifiers:\n{entryBits}"
+                if (
+                    targetSpecifiers[1:].isdigit()
+                and targetSpecifiers[0] in self.targetMap
+                ):
+                    entryTarget = (
+                        self.targetMap[targetSpecifiers[0]],
+                        int(targetSpecifiers[1:])
                     )
-                elif targetSpecifiers not in self.targetMap:
+                elif len(specifiersSet) > 1:
                     raise JournalParseError(
-                        f"Unrecognized target specifier:\n{entryBits}"
+                        f"Entry has too many target specifiers:\n{entryBits}"
                     )
-                entryTarget = self.targetMap[targetSpecifiers]
+                else:
+                    specifier = list(specifiersSet)[0]
+                    copies = len(targetSpecifiers)
+                    if specifier not in self.targetMap:
+                        raise JournalParseError(
+                            f"Unrecognized target specifier in:\n{entryBits}"
+                        )
+                    entryTarget = self.targetMap[specifier]
+                    if copies > 1:
+                        entryTarget = (entryTarget, copies - 1)
         # else entryTarget remains None
 
         return (entryType, entryDecisionType, entryTarget, entryArgs)
 
     def argsString(self, pieces: List[str]) -> str:
         """
         Recombines pieces of a journal argument (such as those produced
@@ -1342,27 +1386,39 @@
     Specifies global preferences for exploration observation. Values are
     either strings or booleans. The keys are:
 
     - 'reciprocals': A boolean specifying whether transitions should
         come with reciprocals by default. Normally this is `True`, but
         it can be set to `False` instead.
         TODO: implement this.
+    - 'revertAspects': A set of strings specifying which aspects of the
+        game state should be reverted when a 'revert' action is taken and
+        specific aspects to revert are not specified. See
+        `base.revertedState` for a list of the available reversion
+        aspects.
     """
     reciprocals: bool
+    revertAspects: Set[str]
 
 
 def observationPreferences(
-    reciprocals=True
+    reciprocals: bool=True,
+    revertAspects: Optional[Set[str]] = None
 ) -> ObservationPreferences:
     """
     Creates an observation preferences dictionary, using default values
     for any preferences not specified as arguments.
     """
     return {
-        'reciprocals': reciprocals
+        'reciprocals': reciprocals,
+        'revertAspects': (
+            revertAspects
+            if revertAspects is not None
+            else set()
+        )
     }
 
 
 class JournalObserver:
     """
     Keeps track of extra state needed when parsing a journal in order to
     produce a `core.DiscreteExploration` object. The methods of this
@@ -1409,15 +1465,15 @@
 
     ## Examples
 
     >>> obs = JournalObserver()
     >>> e = obs.getExploration()
     >>> len(e) # blank starting state
     1
-    >>> e.getActiveDecisions(0) # no active decisions before starting
+    >>> e.getActiveDecisions(0)  # no active decisions before starting
     set()
     >>> obs.definiteDecisionTarget()
     Traceback (most recent call last):
     ...
     exploration.core.MissingDecisionError...
     >>> obs.currentDecisionTarget() is None
     True
@@ -1928,21 +1984,21 @@
             *target
         )
 
     def checkFormat(
         self,
         entryType: str,
         decisionType: base.DecisionType,
-        target: Union[None, JournalTargetType, int],
+        target: Union[None, JournalTargetType, Tuple[JournalTargetType, int]],
         pieces: List[str],
         expectedTargets: Union[
             None,
-            type[int],
+            JournalTargetType,
             Collection[
-                Union[None, JournalTargetType, int]
+                Union[None, JournalTargetType]
             ]
         ],
         expectedPieces: Union[None, int, Collection[int]]
     ) -> None:
         """
         Does format checking for a journal entry after
         `determineEntryType` is called. Checks that:
@@ -1976,28 +2032,34 @@
             )
 
         if expectedTargets is None:
             if target is not None:
                 raise JournalParseError(
                     f"{entryType} entry may not specify a target."
                 )
-        elif expectedTargets is int:
-            if not isinstance(target, int):
+        else:
+            if isinstance(expectedTargets, str):
+                expected = cast(
+                    Collection[Union[None, JournalTargetType]],
+                    [expectedTargets]
+                )
+            else:
+                expected = cast(
+                    Collection[Union[None, JournalTargetType]],
+                    expectedTargets
+                )
+            tType = target
+            if isinstance(tType, tuple):
+                tType = tType[0]
+
+            if tType not in expected:
                 raise JournalParseError(
-                    f"{entryType} entry must have an integer target."
+                    f"{entryType} entry had invalid target {target!r}."
+                    f" Expected one of:\n{expected}"
                 )
-        elif target not in cast(
-            Collection[
-                Union[None, JournalTargetType, int]
-            ],
-            expectedTargets
-        ):
-            raise JournalParseError(
-                f"{entryType} entry had invalid target {target!r}."
-            )
 
         if expectedPieces is None:
             # No restriction
             pass
         elif isinstance(expectedPieces, int):
             if len(pieces) != expectedPieces:
                 raise JournalParseError(
@@ -2285,30 +2347,32 @@
                         dType,
                         eTarget,
                         eParts,
                         None,
                         2
                     )
                     pref = eParts[0]
-                    opAnn = ObservationPreferences.__annotations__
+                    opAnn = get_type_hints(ObservationPreferences)
                     if pref not in opAnn:
                         raise JournalParseError(
                             f"Invalid preference name {pref!r}."
                         )
 
-                    prefVal: Union[None, str, bool]
+                    prefVal: Union[None, str, bool, Set[str]]
                     if opAnn[pref] is bool:
                         prefVal = pf.onOff(eParts[1])
                         if prefVal is None:
                             self.warn(
                                 f"On/off value {eParts[1]!r} is neither"
                                 f" {pf.markerFor('on')!r} nor"
                                 f" {pf.markerFor('off')!r}. Assuming"
                                 f" 'off'."
                             )
+                    elif opAnn[pref] == Set[str]:
+                        prefVal = set(' '.join(eParts[1:]).split())
                     else:  # we assume it's a string
                         assert opAnn[pref] is str
                         prefVal = eParts[1]
 
                     # Set the preference value (type checked above)
                     self.preferences[pref] = prefVal  # type: ignore [literal-required] # noqa: E501
 
@@ -2682,15 +2746,16 @@
                         self.recordAdditionalTransitionConsequence(
                             toApply
                         )
                     else:
                         # Otherwise just apply the consequence
                         self.exploration.applyExtraneousConsequence(
                             toApply,
-                            self.context['transition']
+                            where=self.context['transition'],
+                            moveWhich=self.context['focus']
                         )
                         # Note: no situation-based variables need
                         # updating here
 
                 elif eType == 'tag':
                     self.checkFormat(
                         "tag",
@@ -2698,43 +2763,31 @@
                         eTarget,
                         eParts,
                         (
                             None,
                             'decisionPart',
                             'transitionPart',
                             'reciprocalPart',
-                            'bothPart'
+                            'bothPart',
+                            'zonePart'
                         ),
                         None
                     )
                     tag: base.Tag
                     value: base.TagValue
                     if len(eParts) == 0:
                         raise JournalParseError(
                             "tag entry must include at least a tag name."
                         )
                     elif len(eParts) == 1:
                         tag = eParts[0]
                         value = 1
                     elif len(eParts) == 2:
                         tag, value = eParts
-                        if value == 'True':
-                            value = True
-                        elif value == 'False':
-                            value = False
-                        elif value == 'None':
-                            value = None
-                        else:
-                            try:
-                                value = int(value)
-                            except ValueError:
-                                try:
-                                    value = float(value)
-                                except ValueError:
-                                    pass
+                        value = pf.parseTagValue(value)
                     else:
                         raise JournalParseError(
                             f"tag entry has too many parts (only a tag"
                             f" name and a tag value are allowed). Got:"
                             f" {eParts}"
                         )
 
@@ -2745,14 +2798,23 @@
                     elif eTarget == "transitionPart":
                         self.recordTagTranstion(tag, value)
                     elif eTarget == "reciprocalPart":
                         self.recordTagReciprocal(tag, value)
                     elif eTarget == "bothPart":
                         self.recordTagTranstion(tag, value)
                         self.recordTagReciprocal(tag, value)
+                    elif eTarget == "zonePart":
+                        self.recordTagZone(0, tag, value)
+                    elif (
+                        isinstance(eTarget, tuple)
+                    and len(eTarget) == 2
+                    and eTarget[0] == "zonePart"
+                    and isinstance(eTarget[1], int)
+                    ):
+                        self.recordTagZone(eTarget[1] - 1, tag, value)
                     else:
                         raise JournalParseError(
                             f"Invalid tag target type {eTarget!r}."
                         )
 
                 elif eType == 'annotate':
                     self.checkFormat(
@@ -2769,25 +2831,35 @@
                         ),
                         None
                     )
                     if len(eParts) == 0:
                         raise JournalParseError(
                             "annotation may not be empty."
                         )
+                    combined = ' '.join(eParts)
                     if eTarget is None:
-                        self.recordAnnotateStep(' '.join(eParts))
+                        self.recordAnnotateStep(combined)
                     elif eTarget == "decisionPart":
-                        self.recordAnnotateDecision(' '.join(eParts))
+                        self.recordAnnotateDecision(combined)
                     elif eTarget == "transitionPart":
-                        self.recordAnnotateTranstion(' '.join(eParts))
+                        self.recordAnnotateTranstion(combined)
                     elif eTarget == "reciprocalPart":
-                        self.recordAnnotateReciprocal(' '.join(eParts))
+                        self.recordAnnotateReciprocal(combined)
                     elif eTarget == "bothPart":
-                        self.recordAnnotateTranstion(' '.join(eParts))
-                        self.recordAnnotateReciprocal(' '.join(eParts))
+                        self.recordAnnotateTranstion(combined)
+                        self.recordAnnotateReciprocal(combined)
+                    elif eTarget == "zonePart":
+                        self.recordAnnotateZone(0, combined)
+                    elif (
+                        isinstance(eTarget, tuple)
+                    and len(eTarget) == 2
+                    and eTarget[0] == "zonePart"
+                    and isinstance(eTarget[1], int)
+                    ):
+                        self.recordAnnotateZone(eTarget[1] - 1, combined)
                     else:
                         raise JournalParseError(
                             f"Invalid annotation target type {eTarget!r}."
                         )
 
                 elif eType == 'context':
                     self.checkFormat(
@@ -2866,20 +2938,26 @@
 
                 elif eType == 'zone':
                     self.checkFormat(
                         "zone",
                         dType,
                         eTarget,
                         eParts,
-                        int,
+                        (None, 'zonePart'),
                         1
                     )
                     if eTarget is None:
-                        eTarget = 0
-                    self.recordZone(cast(int, eTarget), eParts[0])
+                        level = 0
+                    elif eTarget == 'zonePart':
+                        level = 1
+                    else:
+                        assert isinstance(eTarget, tuple)
+                        assert len(eTarget) == 2
+                        level = eTarget[1]
+                    self.recordZone(level, eParts[0])
 
                 elif eType == 'unify':
                     self.checkFormat(
                         "unify",
                         dType,
                         eTarget,
                         eParts,
@@ -3050,19 +3128,18 @@
                     aspects: List[str]
                     if len(eParts) == 0:
                         slot = base.DEFAULT_SAVE_SLOT
                         aspects = []
                     else:
                         slot = eParts[0]
                         aspects = eParts[1:]
-                    self.recordRevert(
-                        slot,
-                        set(aspects),
-                        decisionType=dType
-                    )
+                    aspectsSet = set(aspects)
+                    if len(aspectsSet) == 0:
+                        aspectsSet = self.preferences['revertAspects']
+                    self.recordRevert(slot, aspectsSet, decisionType=dType)
 
                 elif eType == 'fulfills':
                     self.checkFormat(
                         "fulfills",
                         dType,
                         eTarget,
                         eParts,
@@ -3101,31 +3178,25 @@
                         "relative",
                         dType,
                         eTarget,
                         eParts,
                         (None, 'transitionPart'),
                         (0, 1, 2)
                     )
-                    try:
-                        if (
-                            len(eParts) == 1
-                        and eParts[0] == self.parseFormat.markerFor(
-                                'relative'
-                            )
-                        ):
-                            self.relative()
-                        elif eTarget == 'transitionPart':
-                            self.relative(None, *eParts)
-                        else:
-                            self.relative(*eParts)
-                    except core.BadStart:
-                        raise JournalParseError(
-                            "You cannot enter relative mode before the"
-                            " 'start' entry."
+                    if (
+                        len(eParts) == 1
+                    and eParts[0] == self.parseFormat.markerFor(
+                            'relative'
                         )
+                    ):
+                        self.relative()
+                    elif eTarget == 'transitionPart':
+                        self.relative(None, *eParts)
+                    else:
+                        self.relative(*eParts)
 
                 else:
                     raise NotImplementedError(
                         f"Unrecognized event type {eType!r}."
                     )
         except Exception as e:
             raise LocatedJournalParseError(
@@ -3230,15 +3301,17 @@
             based on the `ObservationContext`, or will generate an error
             if there is none. This is the current decision at the moment
             the alias is deployed, NOT based on steps within the alias up
             to the substitution point.
         - '__hereName__' will substitute the name of the current
             decision.
         - '__zone__' will substitute the name of the alphabetically
-            first zone parent of the current decision.
+            first level-0 zone ancestor of the current decision.
+        - '__region__' will substitute the name of the alphabetically
+            first level-1 zone ancestor of the current decision.
         - '__transition__' will substitute to the name of the current
             transition, or will generate an error if there is none. Note
             that the current transition is sometimes NOT a valid
             transition from the current decision, because when you take
             a transition, that transition's name is current but the
             current decision is its destination.
         - '__reciprocal__' will substitute to the name of the reciprocal
@@ -3291,25 +3364,41 @@
         if '{__here__}' in commands and '__here__' not in firstWave:
             firstWave['__here__'] = self.definiteDecisionTarget()
         if '{__hereName__}' in commands and '__hereName__' not in firstWave:
             firstWave['__hereName__'] = graph.nameFor(
                 self.definiteDecisionTarget()
             )
         if '{__zone__}' in commands and '__zone__' not in firstWave:
+            baseDecision = self.definiteDecisionTarget()
             parents = sorted(
-                graph.zoneParents(self.definiteDecisionTarget())
+                ancestor
+                for ancestor in graph.zoneAncestors(baseDecision)
+                if graph.zoneHierarchyLevel(ancestor) == 0
             )
             if len(parents) == 0:
                 raise JournalParseError(
-                    f"Use __zone__ in a macro, but the current"
-                    f" decision"
-                    f" {graph.identityOf(self.definiteDecisionTarget())}"
-                    f" is not in any zones."
+                    f"Used __zone__ in a macro, but the current"
+                    f" decision {graph.identityOf(baseDecision)} is not"
+                    f" in any level-0 zones."
                 )
             firstWave['__zone__'] = parents[0]
+        if '{__region__}' in commands and '__region__' not in firstWave:
+            baseDecision = self.definiteDecisionTarget()
+            grandparents = sorted(
+                ancestor
+                for ancestor in graph.zoneAncestors(baseDecision)
+                if graph.zoneHierarchyLevel(ancestor) == 1
+            )
+            if len(grandparents) == 0:
+                raise JournalParseError(
+                    f"Used __region__ in a macro, but the current"
+                    f" decision {graph.identityOf(baseDecision)} is not"
+                    f" in any level-1 zones."
+                )
+            firstWave['__region__'] = grandparents[0]
         if (
             '{__transition__}' in commands
         and '__transition__' not in firstWave
         ):
             ctxTr = self.currentTransitionTarget()
             if ctxTr is None:
                 raise JournalParseError(
@@ -3422,14 +3511,19 @@
         - 'active': prints out the names listing of all currently active
             decisions.
         - 'primary': prints out the identity of the current primary
             decision, or None if there is none.
         - 'saved': prints out the primary decision for the state saved in
             the default save slot, or for a specific save slot if a
             second argument is given.
+        - 'inventory': Displays all current capabilities, tokens, and
+            skills.
+        - 'mechanisms': Displays all current mechanisms and their states.
+        - 'equivalences': Displays all current equivalences, along with
+            whether or not they're active.
         """
         graph = self.exploration.getSituation().graph
         if arg != '' and action not in ('destinations', 'saved'):
             raise JournalParseError(
                 f"Invalid debug command {action!r} with arg {arg!r}:"
                 f" Only 'destination' and 'saved' actions may include a"
                 f" second argument."
@@ -3611,14 +3705,120 @@
                 print(f"Slot {slot!r} has no saved data.", file=sys.stderr)
             else:
                 savedGraph, savedState = saved
                 savedPrimary = savedGraph.identityOf(
                     savedState['primaryDecision']
                 )
                 print(f"Saved at decision: {savedPrimary}", file=sys.stderr)
+        elif action == "inventory":
+            now = self.exploration.getSituation()
+            commonCap = now.state['common']['capabilities']
+            activeCap = now.state['contexts'][now.state['activeContext']][
+                'capabilities'
+            ]
+            merged = base.mergeCapabilitySets(commonCap, activeCap)
+            capCount = len(merged['capabilities'])
+            tokCount = len(merged['tokens'])
+            skillCount = len(merged['skills'])
+            print(
+                (
+                    f"{capCount} capability/ies, {tokCount} token type(s),"
+                    f" and {skillCount} skill(s)"
+                ),
+                file=sys.stderr
+            )
+            if capCount > 0:
+                print("Capabilities (alphabetical order):", file=sys.stderr)
+                for cap in sorted(merged['capabilities']):
+                    print(f"  {cap!r}", file=sys.stderr)
+            if tokCount > 0:
+                print("Tokens (alphabetical order):", file=sys.stderr)
+                for tok in sorted(merged['tokens']):
+                    print(
+                        f"  {tok!r}: {merged['tokens'][tok]}",
+                        file=sys.stderr
+                    )
+            if skillCount > 0:
+                print("Skill levels (alphabetical order):", file=sys.stderr)
+                for skill in sorted(merged['skills']):
+                    print(
+                        f"  {skill!r}: {merged['skills'][skill]}",
+                        file=sys.stderr
+                    )
+        elif action == "mechanisms":
+            now = self.exploration.getSituation()
+            grpah = now.graph
+            mechs = now.state['mechanisms']
+            inGraph = set(graph.mechanisms) - set(mechs)
+            print(
+                (
+                    f"{len(mechs)} mechanism(s) in known states;"
+                    f" {len(inGraph)} additional mechanism(s) in the"
+                    f" default state"
+                ),
+                file=sys.stderr
+            )
+            if len(mechs) > 0:
+                print("Mechanism(s) in known state(s):", file=sys.stderr)
+                for mID in sorted(mechs):
+                    mState = mechs[mID]
+                    whereID, mName = graph.mechanisms[mID]
+                    if whereID is None:
+                        whereStr = " (global)"
+                    else:
+                        domain = graph.domainFor(whereID)
+                        whereStr = f" at {graph.identityOf(whereID)}"
+                    print(
+                        f"  {mName}:{mState!r} - {mID}{whereStr}",
+                        file=sys.stderr
+                    )
+            if len(inGraph) > 0:
+                print("Mechanism(s) in the default state:", file=sys.stderr)
+                for mID in sorted(inGraph):
+                    whereID, mName = graph.mechanisms[mID]
+                    if whereID is None:
+                        whereStr = " (global)"
+                    else:
+                        domain = graph.domainFor(whereID)
+                        whereStr = f" at {graph.identityOf(whereID)}"
+                    print(f"  {mID} - {mName}){whereStr}", file=sys.stderr)
+        elif action == "equivalences":
+            now = self.exploration.getSituation()
+            eqDict = now.graph.equivalences
+            if len(eqDict) > 0:
+                print(f"{len(eqDict)} equivalences:", file=sys.stderr)
+                for hasEq in eqDict:
+                    if isinstance(hasEq, tuple):
+                        assert len(hasEq) == 2
+                        assert isinstance(hasEq[0], base.MechanismID)
+                        assert isinstance(hasEq[1], base.MechanismState)
+                        mID, mState = hasEq
+                        mDetails = now.graph.mechanismDetails(mID)
+                        assert mDetails is not None
+                        mWhere, mName = mDetails
+                        if mWhere is None:
+                            whereStr = " (global)"
+                        else:
+                            whereStr = f" at {graph.identityOf(mWhere)}"
+                        eqStr = f"{mName}:{mState!r} - {mID}{whereStr}"
+                    else:
+                        assert isinstance(hasEq, base.Capability)
+                        eqStr = hasEq
+                    eqSet = eqDict[hasEq]
+                    print(
+                        f"  {eqStr} has {len(eqSet)} equivalence(s):",
+                        file=sys.stderr
+                    )
+                    for eqReq in eqDict[hasEq]:
+                        print(f"    {eqReq}", file=sys.stderr)
+            else:
+                print(
+                    "There are no equivalences right now.",
+                    file=sys.stderr
+                )
         else:
             raise JournalParseError(
                 f"Invalid debug command: {action!r}"
             )
 
     def recordStart(
         self,
@@ -3688,18 +3888,14 @@
         and the reciprocal transition is named (with three arguments).
 
         When a name or decision specifier is used for the destination,
         the domain and/or level-0 zone of the current decision are
         filled in if the specifier is a name or doesn't have domain
         and/or zone info. The first alphabetical level-0 zone is used if
         the current decision is in more than one.
-
-        TODO: If we do this with a destination and that doesn't add zone
-        info, later when we return we should add zone info... OR we
-        should add it now.
         """
         here = self.definiteDecisionTarget()
 
         # Our observation matches `DiscreteExploration.observe` args
         obs: Union[
             Tuple[base.Transition],
             Tuple[base.Transition, base.AnyDecisionSpecifier],
@@ -4931,15 +5127,15 @@
 
     def recordTagTranstion(
         self,
         tag: base.Tag,
         value: Union[base.TagValue, type[base.NoTagValue]] = base.NoTagValue
     ) -> None:
         """
-        Records tags to be applied to the most-recently-defined or
+        Records a tag to be applied to the most-recently-defined or
         -taken transition.
         """
         target = self.currentTransitionTarget()
         if target is None:
             raise JournalParseError(
                 "Cannot tag a transition because there is no current"
                 " transition."
@@ -4950,27 +5146,80 @@
 
     def recordTagReciprocal(
         self,
         tag: base.Tag,
         value: Union[base.TagValue, type[base.NoTagValue]] = base.NoTagValue
     ) -> None:
         """
-        Records tags to be applied to the reciprocal of the
+        Records a tag to be applied to the reciprocal of the
         most-recently-defined or -taken transition.
         """
         target = self.currentReciprocalTarget()
         if target is None:
             raise JournalParseError(
                 "Cannot tag a transition because there is no current"
                 " transition."
             )
 
         now = self.exploration.getSituation()
         now.graph.tagTransition(*target, tag, value)
 
+    def currentZoneAtLevel(self, level: int) -> base.Zone:
+        """
+        Returns a zone in the current graph that applies to the current
+        decision which is at the specified hierarchy level. If there is
+        no such zone, raises a `JournalParseError`. If there are
+        multiple such zones, returns the zone which includes the fewest
+        decisions, breaking ties alphabetically by zone name.
+        """
+        here = self.definiteDecisionTarget()
+        graph = self.exploration.getSituation().graph
+        ancestors = graph.zoneAncestors(here)
+        candidates = [
+            ancestor
+            for ancestor in ancestors
+            if graph.zoneHierarchyLevel(ancestor) == level
+        ]
+        if len(candidates) == 0:
+            raise JournalParseError(
+                (
+                    f"Cannot find any level-{level} zones for the"
+                    f" current decision {graph.identityOf(here)}. That"
+                    f" decision is"
+                ) + (
+                    " in the following zones:"
+                  + '\n'.join(
+                        f"  level {graph.zoneHierarchyLevel(z)}: {z!r}"
+                        for z in ancestors
+                    )
+                ) if len(ancestors) > 0 else (
+                    " not in any zones."
+                )
+            )
+        candidates.sort(
+            key=lambda zone: (len(graph.allDecisionsInZone(zone)), zone)
+        )
+        return candidates[0]
+
+    def recordTagZone(
+        self,
+        level: int,
+        tag: base.Tag,
+        value: Union[base.TagValue, type[base.NoTagValue]] = base.NoTagValue
+    ) -> None:
+        """
+        Records a tag to be applied to one of the zones that the current
+        decision is in, at a specific hierarchy level. There must be at
+        least one zone ancestor of the current decision at that hierarchy
+        level; if there are multiple then the tag is applied to the
+        smallest one, breaking ties by alphabetical order.
+        """
+        applyTo = self.currentZoneAtLevel(level)
+        self.exploration.getSituation().graph.tagZone(applyTo, tag, value)
+
     def recordAnnotateStep(
         self,
         *annotations: base.Annotation
     ) -> None:
         """
         Records annotations to be applied to the current exploration
         step.
@@ -5058,16 +5307,16 @@
                         self.warn(
                             f"'level' annotation expects skill {ea[1]!r}"
                             f" to be at level {ea[2]} but the current"
                             f" level for that skill is {levelNow}."
                         )
                 else:
                     self.warn(
-                        f"'level' annotation expects tokens {a[6:]!r} but"
-                        f" that's not a (token, count) pair."
+                        f"'level' annotation expects skill {a[6:]!r} but"
+                        f" that's not a (skill, level) pair."
                     )
             elif a.startswith("can:"):
                 try:
                     req = pf.parseRequirement(a[4:])
                 except parsing.ParseError:
                     self.warn(
                         f"'can' annotation expects requirement {a[4:]!r}"
@@ -5174,14 +5423,31 @@
                 " current transition or because it doens't have a"
                 " reciprocal."
             )
 
         now = self.exploration.getSituation()
         now.graph.annotateTransition(*target, annotations)
 
+    def recordAnnotateZone(
+        self,
+        level,
+        *annotations: base.Annotation
+    ) -> None:
+        """
+        Records annotations to be applied to the zone at the specified
+        hierarchy level which contains the current decision. If there are
+        multiple such zones, it picks the smallest one, breaking ties
+        alphabetically by zone name (see `currentZoneAtLevel`).
+        """
+        applyTo = self.currentZoneAtLevel(level)
+        self.exploration.getSituation().graph.annotateZone(
+            applyTo,
+            annotations
+        )
+
     def recordContextSwap(
         self,
         targetContext: Optional[base.FocalContextName]
     ) -> None:
         """
         Records a swap of the active focal context, and/or a swap into
         "common"-context mode where all effects modify the common focal
@@ -5705,27 +5971,30 @@
         The current decision & transition information is not updated.
 
         Returns the decision ID for the new node.
         """
         now = self.exploration.getSituation()
         graph = now.graph
         here = self.definiteDecisionTarget()
+        domain = graph.domainFor(here)
 
         oldDest = graph.destination(here, target)
         oldReciprocal = graph.getReciprocal(here, target)
 
         # Create the new decision:
-        newID = graph.addDecision(newDecision)
+        newID = graph.addDecision(newDecision, domain=domain)
         # Note that the new decision is NOT an unknown decision
         # We copy the exploration status from the current decision
         self.exploration.setExplorationStatus(
             newID,
             self.exploration.getExplorationStatus(here)
         )
-        # TODO: Copy over zone/domain info
+        # Copy over zone info
+        for zp in graph.zoneParents(here):
+            graph.addDecisionToZone(newID, zp)
 
         # Retarget the transitions
         graph.retargetTransition(
             here,
             target,
             newID,
             swapReciprocal=False
@@ -5996,26 +6265,19 @@
         transition is set to whatever it was before relative mode was
         entered.
 
         Raises a `TypeError` if a transition is specified without
         specifying a decision. Raises a `ValueError` if given no
         arguments and the exploration does not have a current position.
         Also raises a `ValueError` if told to target a specific
-        transition which does not exist. Raises a `core.BadStart` error
-        if called before the exploration is started.
+        transition which does not exist.
 
         TODO: Example here!
         """
         # TODO: Not this?
-        if len(self.exploration.getSituation().graph) == 0:
-            raise core.BadStart(
-                "Cannot enter relative mode before the exploration is"
-                " started (call `recordStart` first)."
-            )
-
         if where is None:
             if transition is None and self.inRelativeMode:
                 # If we're in relative mode, cancel it
                 self.inRelativeMode = False
 
                 # Here we restore saved sate
                 if self.storedContext is None:
@@ -6089,26 +6351,33 @@
             whereSpec: Optional[base.DecisionSpecifier] = None
             if isinstance(where, str):
                 where = self.parseFormat.parseDecisionSpecifier(where)
                 # might turn it into a DecisionID
 
             if isinstance(where, base.DecisionID):
                 whereID = where
-            else:
+            elif isinstance(where, base.DecisionSpecifier):
                 # Add in current zone + domain info if those things
                 # aren't explicit
-                where = base.spliceDecisionSpecifiers(
-                    where,
-                    self.decisionTargetSpecifier()
-                )
-                whereID = now.graph.getDecision(where)
-                if isinstance(where, base.DecisionSpecifier):
-                    whereSpec = where
-                else:
-                    raise TypeError(f"Invalid decision specifier: {where!r}")
+                if self.currentDecisionTarget() is not None:
+                    where = base.spliceDecisionSpecifiers(
+                        where,
+                        self.decisionTargetSpecifier()
+                    )
+                elif where.domain is None:
+                    # Splice in current domain if needed
+                    where = base.DecisionSpecifier(
+                        domain=self.context['domain'],
+                        zone=where.zone,
+                        name=where.name
+                    )
+                whereID = now.graph.getDecision(where)  # might be None
+                whereSpec = where
+            else:
+                raise TypeError(f"Invalid decision specifier: {where!r}")
 
             # Create a new decision if necessary
             if whereID is None:
                 if transition is not None:
                     raise TypeError(
                         f"Cannot specify a target transition when"
                         f" entering relative mode at previously"
```

### Comparing `exploration-0.7.2/exploration/main.py` & `exploration-0.7.4/exploration/main.py`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/exploration/parsing.py` & `exploration-0.7.4/exploration/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         'tokenCount',
         'effectCharges',
         'sepOrDelay',
         'consequenceSeparator',
         'inCommon',
         'isHidden',
         'skillLevel',
-        'inverseSkill',
+        'wigglyLine',
         'withDetails',
         'reciprocalSeparator',
         'mechanismSeparator',
         'openCurly',
         'closeCurly',
         'openParen',
         'closeParen',
@@ -84,15 +84,15 @@
     Lexeme.tokenCount: '*',
     Lexeme.effectCharges: '=',
     Lexeme.sepOrDelay: ',',
     Lexeme.consequenceSeparator: ';',
     Lexeme.inCommon: '+c',
     Lexeme.isHidden: '+h',
     Lexeme.skillLevel: '^',
-    Lexeme.inverseSkill: '~',
+    Lexeme.wigglyLine: '~',
     Lexeme.withDetails: '%',
     Lexeme.reciprocalSeparator: '/',
     Lexeme.mechanismSeparator: ':',
     Lexeme.openCurly: '{',
     Lexeme.closeCurly: '}',
     Lexeme.openParen: '(',
     Lexeme.closeParen: ')',
@@ -787,14 +787,73 @@
             return self.focalizationNames[word]
         except KeyError:
             raise ParseError(
                 f"Invalid domain focalization name {repr(word)}. Valid"
                 f" name are: {repr(list(self.focalizationNames))}'."
             )
 
+    def parseTagValue(self, value: str) -> base.TagValue:
+        """
+        Converts a string to a tag value, following these rules:
+
+        1. If the string is exactly one of 'None', 'True', or 'False', we
+            convert it to the corresponding Python value.
+        2. If the string can be converted to an integer without raising a
+            ValueError, we use that integer.
+        3. If the string can be converted to a float without raising a
+            ValueError, we use that float.
+        4. Otherwise, it remains a string.
+
+        Note that there is currently no syntax for using list, dictionary,
+        Requirement, or Consequence tag values.
+        TODO: Support those types?
+
+        Examples:
+
+        >>> pf = ParseFormat()
+        >>> pf.parseTagValue('hi')
+        'hi'
+        >>> pf.parseTagValue('3')
+        3
+        >>> pf.parseTagValue('3.0')
+        3.0
+        >>> pf.parseTagValue('True')
+        True
+        >>> pf.parseTagValue('False')
+        False
+        >>> pf.parseTagValue('None') is None
+        True
+        >>> pf.parseTagValue('none')
+        'none'
+        """
+        # TODO: Allow these keywords to be redefined?
+        if value == 'True':
+            return True
+        elif value == 'False':
+            return False
+        elif value == 'None':
+            return None
+        else:
+            try:
+                return int(value)
+            except ValueError:
+                try:
+                    return float(value)
+                except ValueError:
+                    return value
+
+    def unparseTagValue(self, value: base.TagValue) -> str:
+        """
+        Converts a tag value into a string that would be parsed back into a
+        tag value via `parseTagValue`. Currently does not work for list,
+        dictionary, Requirement, or Consequence values.
+        TODO: Those
+        """
+        return str(value)
+
     def hasZoneParts(self, name: str) -> bool:
         """
         Returns true if the specified name contains zone parts (using
         the `zoneSeparator`).
         """
         return self.formatDict[Lexeme.zoneSeparator] in name
 
@@ -2170,14 +2229,18 @@
         ...         base.MechanismSpecifier(None, None, None, 'door'),
         ...         'open'
         ...     )
         ... )
         True
         >>> pf.parseEffect("set coins*10") == base.effect(set=('coins', 10))
         True
+        >>> pf.parseEffect("set agility^3") == base.effect(
+        ...     set=('skill', 'agility', 3)
+        ... )
+        True
         """
         return self.parseEffectFromTokens(self.lex(effectStr))
 
     def unparseEffect(self, effect: base.Effect) -> str:
         """
         The opposite of `parseEffect`; turns an effect back into a
         string reprensentation.
@@ -3360,14 +3423,25 @@
         ...         Lexeme.zoneSeparator,
         ...         'm'
         ...     ],
         ...     4
         ... )
         (MechanismSpecifier(domain=None, zone=None, decision='c',\
  name='m'), 6)
+        >>> pf.parseMechanismSpecifierFromTokens(
+        ...     [
+        ...         'roomB',
+        ...         Lexeme.zoneSeparator,
+        ...         'switch',
+        ...         Lexeme.mechanismSeparator,
+        ...         'on'
+        ...     ]
+        ... )
+        (MechanismSpecifier(domain=None, zone=None, decision='roomB',\
+ name='switch'), 2)
         """
         start, tEnd, nLeft = normalizeEnds(tokens, start, -1)
 
         try:
             dSpec, dEnd = self.parseDecisionSpecifierFromTokens(
                 tokens,
                 start
@@ -3518,25 +3592,14 @@
         Also turns each leaf part into a `Requirement`.
 
         TODO: Make this actually reasonably efficient T_T
 
         Examples:
 
         >>> pf = ParseFormat()
-        >>> pf.parseMechanismSpecifierFromTokens(
-        ...     [
-        ...         'roomB',
-        ...         Lexeme.zoneSeparator,
-        ...         'switch',
-        ...         Lexeme.mechanismSeparator,
-        ...         'on'
-        ...     ]
-        ... )
-        (MechanismSpecifier(domain=None, zone=None, decision='roomB',\
- name='switch'), 2)
         >>> r = pf.parseRequirement('capability&roomB::switch:on')
         >>> pf.groupReqTokensByPrecedence(
         ...     [
         ...         ['jump', Lexeme.orBar, 'climb'],
         ...         Lexeme.ampersand,
         ...         Lexeme.notMarker,
         ...         'coin',
@@ -3610,53 +3673,85 @@
                         raise ParseError("Not a mechanism requirement.")
                     leavesConverted.append(base.ReqMechanism(mSpec, mState))
                     i = mEnd + 2  # + 1 will happen automatically below
                 except ParseError:
                     following = subgrouped[i + 1]
                     if following in (
                         Lexeme.tokenCount,
-                        Lexeme.mechanismSeparator
+                        Lexeme.mechanismSeparator,
+                        Lexeme.wigglyLine,
+                        Lexeme.skillLevel
                     ):
-                        if i == len(subgrouped) - 2:
-                            raise ParseError(
-                                f"Lexeme at end of requirement. Grouped"
-                                f" tokens:\n{tokenGroups}"
-                            )
-                        afterwards = subgrouped[i + 2]
-                        if not isinstance(afterwards, str):
-                            raise ParseError(
-                                f"Lexeme after token or mechanism"
-                                f" separator at index {i}."
-                                f" Grouped tokens:\n{tokenGroups}"
-                            )
-                        i += 2  # another +1 automatic below
-                        if following == Lexeme.tokenCount:
-                            try:
-                                tCount = int(afterwards)
-                            except ValueError:
+                        if (
+                            i == len(subgrouped) - 2
+                         or isinstance(subgrouped[i + 2], Lexeme)
+                        ):
+                            if following == Lexeme.wigglyLine:
+                                # Default tag value is 1
+                                leavesConverted.append(base.ReqTag(gItem, 1))
+                                i += 1  # another +1 automatic below
+                            else:
                                 raise ParseError(
-                                    f"Token count could not be parsed as an"
-                                    f" integer: {afterwards!r}."
-                                    f" Grouped tokens:\n{tokenGroups}"
+                                    f"Lexeme at end of requirement. Grouped"
+                                    f" tokens:\n{tokenGroups}"
                                 )
-                            leavesConverted.append(
-                                base.ReqTokens(gItem, tCount)
-                            )
                         else:
-                            assert following == Lexeme.mechanismSeparator
-                            leavesConverted.append(
-                                base.ReqMechanism(gItem, afterwards)
-                            )
+                            afterwards = subgrouped[i + 2]
+                            if not isinstance(afterwards, str):
+                                raise ParseError(
+                                    f"Lexeme after token/mechanism/tag/skill"
+                                    f" separator at index {i}."
+                                    f" Grouped tokens:\n{tokenGroups}"
+                                )
+                            i += 2  # another +1 automatic below
+                            if following == Lexeme.tokenCount:
+                                try:
+                                    tCount = int(afterwards)
+                                except ValueError:
+                                    raise ParseError(
+                                        f"Token count could not be"
+                                        f" parsed as an integer:"
+                                        f" {afterwards!r}. Grouped"
+                                        f" tokens:\n{tokenGroups}"
+                                    )
+                                leavesConverted.append(
+                                    base.ReqTokens(gItem, tCount)
+                                )
+                            elif following == Lexeme.mechanismSeparator:
+                                leavesConverted.append(
+                                    base.ReqMechanism(gItem, afterwards)
+                                )
+                            elif following == Lexeme.wigglyLine:
+                                tVal = self.parseTagValue(afterwards)
+                                leavesConverted.append(
+                                    base.ReqTag(gItem, tVal)
+                                )
+                            else:
+                                assert following == Lexeme.skillLevel
+                                try:
+                                    sLevel = int(afterwards)
+                                except ValueError:
+                                    raise ParseError(
+                                        f"Skill level could not be"
+                                        f" parsed as an integer:"
+                                        f" {afterwards!r}. Grouped"
+                                        f" tokens:\n{tokenGroups}"
+                                    )
+                                leavesConverted.append(
+                                    base.ReqLevel(gItem, sLevel)
+                                )
                     else:
                         if gItem == 'X':
                             leavesConverted.append(base.ReqImpossible())
                         elif gItem == 'O':
                             leavesConverted.append(base.ReqNothing())
                         else:
-                            leavesConverted.append(base.ReqCapability(gItem))
+                            leavesConverted.append(
+                                base.ReqCapability(gItem)
+                            )
 
             # Finally, increment our index:
             i += 1
 
         # Now group all NOT operators
         i = 0
         notsGrouped: GroupedRequirementParts = []
@@ -3980,14 +4075,23 @@
  decision=None, name='mechanism'), 'state')
         >>> pf.parseRequirement('where::mechanism:state')
         ReqMechanism(MechanismSpecifier(domain=None, zone=None,\
  decision='where', name='mechanism'), 'state')
         >>> pf.parseRequirement('zone::where::mechanism:state')
         ReqMechanism(MechanismSpecifier(domain=None, zone='zone',\
  decision='where', name='mechanism'), 'state')
+        >>> pf.parseRequirement('tag~')
+        ReqTag('tag', 1)
+        >>> pf.parseRequirement('tag~&tag2~')
+        ReqAll([ReqTag('tag', 1), ReqTag('tag2', 1)])
+        >>> pf.parseRequirement('tag~value|tag~3|tag~3.5|skill^3')
+        ReqAny([ReqTag('tag', 'value'), ReqTag('tag', 3),\
+ ReqTag('tag', 3.5), ReqLevel('skill', 3)])
+        >>> pf.parseRequirement('tag~True|tag~False|tag~None')
+        ReqAny([ReqTag('tag', True), ReqTag('tag', False), ReqTag('tag', None)])
 
         Precedence examples:
 
         >>> pf.parseRequirement('A|B&C')
         ReqAny([ReqCapability('A'), ReqAll([ReqCapability('B'),\
  ReqCapability('C')])])
         >>> pf.parseRequirement('A&B|C')
@@ -4086,16 +4190,16 @@
         ... ]
         >>> pf.parseSkillCombinationFromTokens(tokens)
         BestSkill('brains', 'brawn')
         >>> tokens[2] = '3'  # not a lexeme so it's a string
         >>> pf.parseSkillCombinationFromTokens(tokens)
         BestSkill(3, 'brawn')
         >>> tokens = [
-        ...     Lexeme.inverseSkill,
-        ...     Lexeme.inverseSkill,
+        ...     Lexeme.wigglyLine,
+        ...     Lexeme.wigglyLine,
         ...     'yes',
         ... ]
         >>> pf.parseSkillCombinationFromTokens(tokens)
         InverseSkill(InverseSkill('yes'))
         """
         start, end, nTokens = normalizeEnds(tokens, start, end)
 
@@ -4108,15 +4212,15 @@
                 except ValueError:
                     return base.BestSkill(first)
             else:
                 raise ParseError(
                     "Invalid SkillCombination:\n{tokens[start:end + 1]"
                 )
 
-        if first == Lexeme.inverseSkill:
+        if first == Lexeme.wigglyLine:
             inv = self.parseSkillCombinationFromTokens(
                 tokens,
                 start + 1,
                 end
             )
             if isinstance(inv, base.BestSkill) and len(inv.skills) == 1:
                 return base.InverseSkill(inv.skills[0])
@@ -5331,25 +5435,25 @@
     Converts a `graphviz` dot-format string into a `core.DecisionGraph`.
     A custom `ParseFormat` may be specified if desired; the default
     `ParseFormat` is used if not. Note that this relies on specific
     indentation schemes used by `toDot` so a hand-edited dot-format
     graph will probably not work. A `DotParseError` is raised if the
     provided string can't be parsed. Example
 
-    >>> parseDotNode(' 3 [ name="A = \\\\"grate:open\\\\"" ]')
-    (3, [('name', 'A = "grate:open"')])
+    >>> parseDotNode(' 3 [ label="A = \\\\"grate:open\\\\"" ]')
+    (3, [('label', 'A = "grate:open"')])
     >>> sg = '''\
     ... subgraph __requirements__ {
-    ...   3 [ name="A = \\\\"grate:open\\\\"" ]
-    ...   4 [ name="B = \\\\"!(helmet)\\\\"" ]
-    ...   5 [ name="C = \\\\"helmet\\\\"" ]
+    ...   3 [ label="A = \\\\"grate:open\\\\"" ]
+    ...   4 [ label="B = \\\\"!(helmet)\\\\"" ]
+    ...   5 [ label="C = \\\\"helmet\\\\"" ]
     ... }'''
     >>> parseDotGraphContents(sg.splitlines()[1:])
-    ({'nodes': [(3, [('name', 'A = "grate:open"')]),\
- (4, [('name', 'B = "!(helmet)"')]), (5, [('name', 'C = "helmet"')])],\
+    ({'nodes': [(3, [('label', 'A = "grate:open"')]),\
+ (4, [('label', 'B = "!(helmet)"')]), (5, [('label', 'C = "helmet"')])],\
  'edges': [], 'attrs': [], 'subgraphs': []}, [])
     >>> from . import core
     >>> dg = core.DecisionGraph.example('simple')
     >>> encoded = toDot(dg)
     >>> reconstructed = parseDot(encoded)
     >>> for diff in dg.listDifferences(reconstructed):
     ...     print(diff)
@@ -5366,21 +5470,21 @@
     >>> tg.addDecision('A')
     0
     >>> tg.addDecision('B')
     1
     >>> tg.addTransition('A', 'up', 'B', 'down')
     >>> same = parseDot('''
     ... digraph {
-    ...     0 [ name=A ]
+    ...     0 [ name=A label=A ]
     ...       0 -> 1 [
     ...         label=up
     ...         fullLabel=up
     ...         reciprocal=down
     ...       ]
-    ...     1 [ name=B ]
+    ...     1 [ name=B label=B ]
     ...       1 -> 0 [
     ...         label=down
     ...         fullLabel=down
     ...         reciprocal=up
     ...       ]
     ... }''')
     >>> for diff in tg.listDifferences(same):
@@ -5392,15 +5496,15 @@
     >>> tg.setConsequence(
     ...     'B',
     ...     'down',
     ...     [base.effect(gain="one")]
     ... )
     >>> test = parseDot('''
     ...   digraph {
-    ...     0 [ name="A = \\\\"one|two\\\\"" ]
+    ...     0 [ name="A = \\\\"one|two\\\\"" label="A = \\\\"one|two\\\\"" ]
     ...   }
     ... ''')
     >>> list(test.nodes)
     [0]
     >>> test.nodes[0]['name']
     'A = "one|two"'
     >>> eff = (
@@ -5409,15 +5513,15 @@
     ...   r' \\\\\\"value\\\\\\": \\\\\\"one\\\\\\",'
     ...   r' \\\\\\"charges\\\\\\": null, \\\\\\"hidden\\\\\\": false,'
     ...   r' \\\\\\"delay\\\\\\": null}]\\""'
     ... )
     >>> utils.unquoted(eff)[1]
     ''
     >>> test2 = parseDot(
-    ...     'digraph {\\n 0 [ name=' + eff + ' ]\\n}'
+    ...     'digraph {\\n 0 [ name=' + eff + ' label=' + eff + ' ]\\n}'
     ... )
     >>> s = test2.nodes[0]['name']
     >>> s[:25]
     'A = "[{\\\\"type\\\\": \\\\"gain\\\\"'
     >>> s[25:50]
     ', \\\\"applyTo\\\\": \\\\"active\\\\"'
     >>> s[50:70]
@@ -5432,33 +5536,33 @@
     >>> uq, after = utils.unquoted(ae)
     >>> after
     ''
     >>> fromJSON(uq) == [base.effect(gain="one")]
     True
     >>> same = parseDot('''
     ... digraph {
-    ...   0 [ name=A ]
+    ...   0 [ name=A label=A ]
     ...     0 -> 1 [
     ...       label=up
     ...       fullLabel=up
     ...       reciprocal=down
     ...       req=A
     ...     ]
-    ...   1 [ name=B ]
+    ...   1 [ name=B label=B ]
     ...     1 -> 0 [
     ...       label=down
     ...       fullLabel=down
     ...       reciprocal=up
     ...       consequence=A
     ...     ]
     ...   subgraph __requirements__ {
-    ...     2 [ name="A = \\\\"one|two\\\\"" ]
+    ...     2 [ label="A = \\\\"one|two\\\\"" ]
     ...   }
     ...   subgraph __consequences__ {
-    ...     3 [ name=''' + eff + ''' ]
+    ...     3 [ label=''' + eff + ''' ]
     ...   }
     ... }''')
     >>> c = {'tags': {}, 'annotations': [], 'reciprocal': 'up', 'consequence': [{'type': 'gain', 'applyTo': 'active', 'value': 'one', 'delay': None, 'charges': None}]}['consequence']  # noqa
 
     >>> for diff in tg.listDifferences(same):
     ...     print(diff)
     >>> same == tg
@@ -5791,14 +5895,16 @@
         name: Optional[str] = None
         annotations = []
         tags: Dict[base.Tag, base.TagValue] = {}
         zones = []
         for attr, aVal in attrs:
             if attr == 'name':  # it's the name
                 name = aVal
+            elif attr == 'label':  # zone + name; redundant
+                pass
             elif attr.startswith('t_'):  # it's a tag
                 tagName = attr[2:]
                 try:
                     tagAny = fromJSON(aVal)
                 except json.decoder.JSONDecodeError:
                     raise DotParseError(
                         f"Error in JSON for tag attr '{attr}' of node"
@@ -6004,15 +6110,14 @@
                 result.nextMechanismID = int(value)
             except ValueError:
                 raise DotParseError(
                     f"Invalid 'nextMechanismID' value:"
                     f"\n  {repr(value)}"
                 )
         elif name in (
-            "zoneTagDicts",
             "equivalences",
             "reversionTypes",
             "mechanisms",
             "globalMechanisms",
             "nameLookup"
         ):
             try:
@@ -6064,14 +6169,16 @@
     zones at those levels should be cluster-style subgraphs. This
     will prefix the subgraph names with 'cluster_' instead of just
     '_'.
 
     TODO: Check edge cases for quotes in capability names, tag names,
     transition names, annotations, etc.
 
+    TODO: At least colons not allowed in tag names!
+
     TODO: Spaces in decision/transition names? Other special
     characters in those names?
     """
     # Set up result including unknownCount and nextID
     result = (
         f"digraph {{"
         f"\n  unknownCount={graph.unknownCount}"
@@ -6093,14 +6200,22 @@
     decision: base.DecisionID  # TODO: Fix Multidigraph type stubs
     for decision in graph.nodes:
         nodeInfo = graph.nodes[decision]
         tags = nodeInfo.get('tags', {})
         annotations = toJSON(nodeInfo.get('annotations', []))
         zones = nodeInfo.get('zones', set())
         nodeAttrs = f"\n    name={utils.quoted(nodeInfo['name'])}"
+        immediateZones = [z for z in zones if graph.zoneHierarchyLevel(z) == 0]
+        if len(immediateZones) > 0:
+            useZone = sorted(immediateZones)[0]
+            # TODO: Don't hardcode :: here?
+            withZone = useZone + "::" + nodeInfo['name']
+            nodeAttrs += f"\n    label={utils.quoted(withZone)}"
+        else:
+            nodeAttrs += f"\n    label={utils.quoted(nodeInfo['name'])}"
         for tag, value in tags.items():
             rep = utils.quoted(toJSON(value))
             nodeAttrs += f"\n    t_{tag}={rep}"
         for z in sorted(zones):
             nodeAttrs += f"\n    z_{z}=1"
         if annotations:
             nodeAttrs += '\n    annotations=' + utils.quoted(annotations)
@@ -6182,15 +6297,14 @@
         for decision in sorted(graph.allDecisionsInZone(z)):
             zoneSubgraph += f'\n    {decision}'
         zoneSubgraph += '\n  }'
         result += zoneSubgraph
 
     # Add equivalences, mechanisms, etc.
     for attr in [
-        "zoneTagDicts",
         "equivalences",
         "reversionTypes",
         "mechanisms",
         "globalMechanisms",
         "nameLookup"
     ]:
         aRep = utils.quoted(toJSON(getattr(graph, attr)))
@@ -6199,39 +6313,39 @@
     # Add legend subgraphs to represent abbreviations
     useID = graph.nextID
     if reqKeys:
         result += '\n  subgraph __requirements__ {'
         for rrepr, ab in reqKeys.items():
             nStr = utils.quoted(ab + ' = ' + rrepr)
             result += (
-                f"\n    {useID} [ name={nStr} ]"
+                f"\n    {useID} [ label={nStr} ]"
             )
             useID += 1
         result += '\n  }'
 
     if consequenceKeys:
         result += '\n  subgraph __consequences__ {'
         for erepr, ab in consequenceKeys.items():
             nStr = utils.quoted(ab + ' = ' + erepr)
             result += (
-                f"\n    {useID} [ name={nStr} ]"
+                f"\n    {useID} [ label={nStr} ]"
             )
             useID += 1
         result += '\n  }'
 
     if graph.mechanisms:
         result += '\n  subgraph __mechanisms__ {'
         mID: base.MechanismID
         mWhere: Optional[base.DecisionID]
         mName: base.MechanismName
         for (mID, (mWhere, mName)) in graph.mechanisms.items():
             qName = utils.quoted(mName)
             nStr = utils.quoted(f"{mID}@{mWhere}:{qName}")
             result += (
-                f"\n    {useID} [ name={nStr} ]"
+                f"\n    {useID} [ label={nStr} ]"
             )
             useID += 1
         result += '\n  }'
 
     result += "\n}\n"
     return result
 
@@ -6313,22 +6427,25 @@
     True
     >>> dg = core.DecisionGraph.example('simple')
     >>> fromJSON(toJSON(dg)) == dg
     True
     >>> dg = core.DecisionGraph.example('abc')
     >>> zi = dg.getZoneInfo('upZone')
     >>> zi
-    ZoneInfo(level=1, parents=set(), contents={'zoneA'})
+    ZoneInfo(level=1, parents=set(), contents={'zoneA'}, tags={},\
+ annotations=[])
     >>> zj = toJSON(zi)
     >>> zj
     '{"^^d": "namedtuple", "name": "ZoneInfo", "values":\
  {"level": 1, "parents": {"^^d": "set", "values": []},\
- "contents": {"^^d": "set", "values": ["zoneA"]}}}'
+ "contents": {"^^d": "set", "values": ["zoneA"]}, "tags": {},\
+ "annotations": []}}'
     >>> fromJSON(toJSON(zi))
-    ZoneInfo(level=1, parents=set(), contents={'zoneA'})
+    ZoneInfo(level=1, parents=set(), contents={'zoneA'}, tags={},\
+ annotations=[])
     >>> fromJSON(toJSON(zi)) == zi
     True
     >>> toJSON({'a': 'b', 1: 2})
     '{"^^d": "dict", "items": [["a", "b"], [1, 2]]}'
     >>> toJSON(((1, 2), (3, 4)))
     '{"^^d": "tuple", "values": [{"^^d": "tuple", "values": [1, 2]},\
  {"^^d": "tuple", "values": [3, 4]}]}'
@@ -6478,36 +6595,41 @@
     ... ' [1, {"right": 0, "up_right": 0}],'
     ... ' [2, {"up": 0, "grab_helmet": 2, "pull_lever": 2}]]},'
     ... ' "zones": {"zoneA":'
     ... ' {"^^d": "namedtuple", "name": "ZoneInfo",'
     ... ' "values": {'
     ... '"level": 0,'
     ... ' "parents": {"^^d": "set", "values": ["upZone"]},'
-    ... ' "contents": {"^^d": "set", "values": [0, 2]}'
+    ... ' "contents": {"^^d": "set", "values": [0, 2]},'
+    ... ' "tags": {},'
+    ... ' "annotations": []'
     ... '}'
     ... '},'
     ... ' "zoneB":'
     ... ' {"^^d": "namedtuple", "name": "ZoneInfo",'
     ... ' "values": {'
     ... '"level": 0,'
     ... ' "parents": {"^^d": "set", "values": []},'
-    ... ' "contents": {"^^d": "set", "values": [1]}'
+    ... ' "contents": {"^^d": "set", "values": [1]},'
+    ... ' "tags": {},'
+    ... ' "annotations": []'
     ... '}'
     ... '},'
     ... ' "upZone":'
     ... ' {"^^d": "namedtuple", "name": "ZoneInfo",'
     ... ' "values": {'
     ... '"level": 1,'
     ... ' "parents": {"^^d": "set", "values": []},'
-    ... ' "contents": {"^^d": "set", "values": ["zoneA"]}'
+    ... ' "contents": {"^^d": "set", "values": ["zoneA"]},'
+    ... ' "tags": {},'
+    ... ' "annotations": []'
     ... '}'
     ... '}'
     ... '},'
     ... ' "unknownCount": 0,'
-    ... ' "zoneTagDicts": {},'
     ... ' "equivalences": {"^^d": "dict", "items": ['
     ... '[{"^^d": "tuple", "values": [0, "open"]},'
     ... ' {"^^d": "set", "values": ['
     ... '{"^^d": "Requirement", "value": "helmet"}]}]'
     ... ']},'
     ... ' "reversionTypes": {},'
     ... ' "nextMechanismID": 1,'
@@ -6528,16 +6650,14 @@
     >>> rec = fromJSON(j)
     >>> rec.nodes == dg.nodes
     True
     >>> rec.edges == dg.edges
     True
     >>> rec.unknownCount == dg.unknownCount
     True
-    >>> rec.zoneTagDicts == dg.zoneTagDicts
-    True
     >>> rec.equivalences == dg.equivalences
     True
     >>> rec.reversionTypes == dg.reversionTypes
     True
     >>> rec._byEdge == dg._byEdge
     True
     >>> rec.zones == dg.zones
@@ -6654,15 +6774,14 @@
             return {
                 '^^d': 'DecisionGraph',
                 'props': self.default(o.graph),  # type:ignore [attr-defined]
                 'node_links': self.default(networkx.node_link_data(o)),
                 '_byEdge': self.default(o._byEdge),
                 'zones': self.default(o.zones),
                 'unknownCount': o.unknownCount,
-                'zoneTagDicts': self.default(o.zoneTagDicts),
                 'equivalences': self.default(o.equivalences),
                 'reversionTypes': self.default(o.reversionTypes),
                 'nextMechanismID': o.nextMechanismID,
                 'mechanisms': self.default(o.mechanisms),
                 'globalMechanisms': self.default(o.globalMechanisms),
                 'nameLookup': self.default(o.nameLookup)
             }
@@ -6749,21 +6868,24 @@
     >>> o = {1, 2, 'hi'}
     >>> s = toJSON(o)
     >>> s
     '{"^^d": "set", "values": [1, 2, "hi"]}'
     >>> l = fromJSON(s)
     >>> o == l
     True
-    >>> zi = base.ZoneInfo(1, set(), set())
+    >>> zi = base.ZoneInfo(1, set(), set(), {}, [])
     >>> s = toJSON(zi)
     >>> c = (
     ... '{"^^d": "namedtuple", "name": "ZoneInfo", "values": {'
     ... '"level": 1,'
     ... ' "parents": {"^^d": "set", "values": []},'
-    ... ' "contents": {"^^d": "set", "values": []}}}'
+    ... ' "contents": {"^^d": "set", "values": []},'
+    ... ' "tags": {},'
+    ... ' "annotations": []'
+    ... '}}'
     ... )
     >>> s == c
     True
 
     TODO: SkillCombination example
     """
     def __init__(self, *args, **kwargs):
@@ -6864,15 +6986,14 @@
                 storedByEdge = obj['_byEdge']
                 graphResult._byEdge = {
                     int(k): storedByEdge[k]
                     for k in storedByEdge
                 }
                 graphResult.zones = obj['zones']
                 graphResult.unknownCount = obj['unknownCount']
-                graphResult.zoneTagDicts = obj['zoneTagDicts']
                 graphResult.equivalences = obj['equivalences']
                 graphResult.reversionTypes = obj['reversionTypes']
                 graphResult.nextMechanismID = obj['nextMechanismID']
                 graphResult.mechanisms = {
                     int(k): v
                     for k, v in
                     obj['mechanisms'].items()
```

### Comparing `exploration-0.7.2/exploration/utils.py` & `exploration-0.7.4/exploration/utils.py`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/exploration.egg-info/PKG-INFO` & `exploration-0.7.4/exploration.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exploration
-Version: 0.7.2
+Version: 0.7.4
 Summary: Tool for reading, formatting, and manipulating exploration graphs, which are graphs (or graph-sequences) that describe exploration of a game space, principally designed with Metroidvania games in mind.
 Home-page: https://cs.wellesley.edu/~pmwh/mvmap/egtool/docs/exploration
 Author: Peter Mawhorter
 Author-email: pmawhort@wellesley.edu
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 3 - Alpha
@@ -89,14 +89,27 @@
 ## Plans
 
 - Better support for open-world games, where decisions are not as closely
     linked to virtual space structure.
 
 ## Changelog
 
+- v0.7.4 fixes some minor issues:
+    * Fixes a bug with mechanism search where relevant transitions were not
+      being used as the search basis in some cases.
+- v0.7.3 adds a bit more:
+    * Journal support for tagging and annotating zones.
+    * `ReqTag` requirements for requiring the presence of a certain tag
+      (or a certain tag value) on some active decision or zone.
+    * `ReqLevel` requirements for requiring a minimum skill level.
+    * Removes the restriction on entering relative mode in an
+      empty/unstarted graph.
+    * Respects current domain when creating new nodes via warps or when
+      there's no current decision.
+    * Adds 'inventory', 'equivalences', and 'mechanisms' debug options.
 - v0.7.2 offers a few more improvements and more API changes (including
   breaking ones):
     * `replaceUnexplored` is now `replaceUnconfirmed`. `unvisited` tag is
       now `unconfirmed`. `core.DecisionGraph.hasBeenVisited` is now
       `core.DecisionGraph.isConfirmed`. Finally a good naming distinction
       between graph confirmation & exploration visited status.
     * Adds 'inspect' mode to the `egtool.py` script and an `inspect`
@@ -112,14 +125,16 @@
       transitions: When `core.DiscreteExploration.advanceSituation` is
       called, each trigger action at an active decision whose
       requirements are satisfied will have its consequences applied.
     * Prevents using 'a'/'action' to take an existing action, requiring
       the use of 't'/'retrace' with the 'actionPart' target instead
       (typically 'ta'). This helps catch issues with action name
       misspellings, and location confusion, among others.
+    * Endings are now warps by default instead of transitions, use
+      'actionPart' (e.g., 'Ea') to mark a voluntary ending.
 - v0.7.1 fixes major bugs with v0.7 and adds a few more nice/important
   things:
     * Transitions may include outcome specifiers, so that in a journal
       you can annotate taking the same transition multiple times and
       getting different results each time for challenges.
     * A new 'save' effect copies game state, which can be restored (in
       whole or in part) via a new 'revertTo' / 'revert'
```

### Comparing `exploration-0.7.2/exploration.egg-info/SOURCES.txt` & `exploration-0.7.4/exploration.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 exploration/base.py
 exploration/commands.py
 exploration/core.py
 exploration/display.py
 exploration/geographic.py
 exploration/graphs.py
 exploration/journal.py
+exploration/journal_guide.py
 exploration/main.py
+exploration/overview.py
 exploration/parsing.py
 exploration/py.typed
 exploration/utils.py
 exploration.egg-info/PKG-INFO
 exploration.egg-info/SOURCES.txt
 exploration.egg-info/dependency_links.txt
 exploration.egg-info/requires.txt
```

### Comparing `exploration-0.7.2/scripts/egtool.py` & `exploration-0.7.4/scripts/egtool.py`

 * *Files identical despite different names*

### Comparing `exploration-0.7.2/setup.cfg` & `exploration-0.7.4/setup.cfg`

 * *Files identical despite different names*

