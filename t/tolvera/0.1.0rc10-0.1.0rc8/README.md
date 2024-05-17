# Comparing `tmp/tolvera-0.1.0rc10.tar.gz` & `tmp/tolvera-0.1.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tolvera-0.1.0rc10.tar", max compression
+gzip compressed data, was "tolvera-0.1.0rc8.tar", max compression
```

## Comparing `tolvera-0.1.0rc10.tar` & `tolvera-0.1.0rc8.tar`

### file list

```diff
@@ -1,38 +1,46 @@
--rw-r--r--   0        0        0    34523 2023-11-23 15:54:16.427339 tolvera-0.1.0rc10/LICENSE
--rw-r--r--   0        0        0     8913 2024-05-16 16:07:05.231292 tolvera-0.1.0rc10/README.md
--rw-r--r--   0        0        0     1390 2024-05-16 16:10:16.204844 tolvera-0.1.0rc10/pyproject.toml
--rw-r--r--   0        0        0      259 2024-05-16 16:07:04.226367 tolvera-0.1.0rc10/src/tolvera/__init__.py
--rw-r--r--   0        0        0     1400 2024-05-16 16:07:04.226491 tolvera-0.1.0rc10/src/tolvera/__main__.py
--rw-r--r--   0        0        0     7859 2024-05-16 16:07:05.231550 tolvera-0.1.0rc10/src/tolvera/context.py
--rw-r--r--   0        0        0     5792 2024-05-16 16:07:05.231724 tolvera-0.1.0rc10/src/tolvera/cv.py
--rw-r--r--   0        0        0    34367 2024-05-16 16:07:04.227212 tolvera-0.1.0rc10/src/tolvera/iml.py
--rw-r--r--   0        0        0      111 2024-05-16 16:07:04.227370 tolvera-0.1.0rc10/src/tolvera/mp/__init__.py
--rw-r--r--   0        0        0     3543 2024-05-16 16:07:04.227495 tolvera-0.1.0rc10/src/tolvera/mp/face.py
--rw-r--r--   0        0        0     6515 2024-05-16 16:07:04.227616 tolvera-0.1.0rc10/src/tolvera/mp/face_mesh.py
--rw-r--r--   0        0        0    35788 2024-05-16 16:07:04.227840 tolvera-0.1.0rc10/src/tolvera/mp/face_mesh_connections.py
--rw-r--r--   0        0        0     9488 2024-05-16 16:07:04.227969 tolvera-0.1.0rc10/src/tolvera/mp/hands.py
--rw-r--r--   0        0        0     5051 2024-05-16 16:07:04.228100 tolvera-0.1.0rc10/src/tolvera/mp/pose.py
--rw-r--r--   0        0        0    17634 2024-05-16 16:07:04.228329 tolvera-0.1.0rc10/src/tolvera/npndarray_dict.py
--rw-r--r--   0        0        0      109 2024-05-16 16:07:04.228454 tolvera-0.1.0rc10/src/tolvera/osc/__init__.py
--rw-r--r--   0        0        0    16592 2024-05-16 16:07:04.228615 tolvera-0.1.0rc10/src/tolvera/osc/maxmsp.py
--rw-r--r--   0        0        0     2172 2024-05-16 16:07:04.228739 tolvera-0.1.0rc10/src/tolvera/osc/osc.py
--rw-r--r--   0        0        0    18115 2024-05-16 16:07:04.228905 tolvera-0.1.0rc10/src/tolvera/osc/oscmap.py
--rw-r--r--   0        0        0    21320 2024-05-16 16:07:04.229104 tolvera-0.1.0rc10/src/tolvera/osc/pd.py
--rw-r--r--   0        0        0     8050 2024-05-16 16:07:04.229230 tolvera-0.1.0rc10/src/tolvera/osc/update.py
--rw-r--r--   0        0        0    18350 2024-05-16 16:07:05.231935 tolvera-0.1.0rc10/src/tolvera/particles.py
--rw-r--r--   0        0        0     8746 2024-05-16 16:07:04.229651 tolvera-0.1.0rc10/src/tolvera/patches.py
--rw-r--r--   0        0        0    20397 2024-05-16 16:07:04.229875 tolvera-0.1.0rc10/src/tolvera/pixels.py
--rw-r--r--   0        0        0    11293 2024-05-16 16:07:04.230076 tolvera-0.1.0rc10/src/tolvera/sketchbook.py
--rw-r--r--   0        0        0     1603 2024-05-16 16:07:04.230224 tolvera-0.1.0rc10/src/tolvera/species.py
--rw-r--r--   0        0        0    15351 2024-05-16 16:07:04.230392 tolvera-0.1.0rc10/src/tolvera/state.py
--rw-r--r--   0        0        0     2753 2024-05-16 16:07:04.230496 tolvera-0.1.0rc10/src/tolvera/taichi_.py
--rw-r--r--   0        0        0     7364 2024-05-16 16:07:04.230628 tolvera-0.1.0rc10/src/tolvera/tolvera_.py
--rw-r--r--   0        0        0    13382 2024-05-16 16:07:04.230814 tolvera-0.1.0rc10/src/tolvera/utils.py
--rw-r--r--   0        0        0     1351 2024-05-16 16:07:04.230978 tolvera-0.1.0rc10/src/tolvera/vera/__init__.py
--rw-r--r--   0        0        0     5117 2024-05-16 16:07:05.232116 tolvera-0.1.0rc10/src/tolvera/vera/flock.py
--rw-r--r--   0        0        0     9569 2024-05-16 16:07:04.231374 tolvera-0.1.0rc10/src/tolvera/vera/forces.py
--rw-r--r--   0        0        0     2618 2024-05-16 16:07:05.232273 tolvera-0.1.0rc10/src/tolvera/vera/particle_life.py
--rw-r--r--   0        0        0     4145 2024-05-16 16:07:05.232439 tolvera-0.1.0rc10/src/tolvera/vera/reaction_diffusion.py
--rw-r--r--   0        0        0     8254 2024-05-16 16:07:04.231781 tolvera-0.1.0rc10/src/tolvera/vera/slime.py
--rw-r--r--   0        0        0     5944 2024-05-16 16:07:04.231918 tolvera-0.1.0rc10/src/tolvera/vera/swarmalators.py
--rw-r--r--   0        0        0    10016 1970-01-01 00:00:00.000000 tolvera-0.1.0rc10/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-11-23 15:54:16.427339 tolvera-0.1.0rc8/LICENSE
+-rw-r--r--   0        0        0     7283 2024-03-12 14:02:15.429456 tolvera-0.1.0rc8/README.md
+-rw-r--r--   0        0        0     1372 2024-04-24 07:26:46.877033 tolvera-0.1.0rc8/pyproject.toml
+-rw-r--r--   0        0        0      257 2024-04-05 15:10:24.578539 tolvera-0.1.0rc8/src/tolvera/__init__.py
+-rw-r--r--   0        0        0     1415 2024-03-12 14:02:15.430630 tolvera-0.1.0rc8/src/tolvera/__main__.py
+-rw-r--r--   0        0        0     7859 2024-04-06 16:34:13.230063 tolvera-0.1.0rc8/src/tolvera/context.py
+-rw-r--r--   0        0        0     5841 2024-03-12 14:02:15.431092 tolvera-0.1.0rc8/src/tolvera/cv.py
+-rw-r--r--   0        0        0    34367 2024-03-12 14:02:15.431395 tolvera-0.1.0rc8/src/tolvera/iml.py
+-rw-r--r--   0        0        0      111 2024-03-16 12:45:28.778553 tolvera-0.1.0rc8/src/tolvera/mp/__init__.py
+-rw-r--r--   0        0        0     3543 2024-03-16 14:14:12.562796 tolvera-0.1.0rc8/src/tolvera/mp/face.py
+-rw-r--r--   0        0        0     6515 2024-03-16 15:10:11.518026 tolvera-0.1.0rc8/src/tolvera/mp/face_mesh.py
+-rw-r--r--   0        0        0    35788 2024-03-16 14:19:01.531491 tolvera-0.1.0rc8/src/tolvera/mp/face_mesh_connections.py
+-rw-r--r--   0        0        0     9488 2024-03-16 14:03:33.168705 tolvera-0.1.0rc8/src/tolvera/mp/hands.py
+-rw-r--r--   0        0        0     5051 2024-03-16 12:44:02.945408 tolvera-0.1.0rc8/src/tolvera/mp/pose.py
+-rw-r--r--   0        0        0    17634 2024-03-12 14:02:15.432183 tolvera-0.1.0rc8/src/tolvera/npndarray_dict.py
+-rw-r--r--   0        0        0      109 2024-03-12 14:02:15.432380 tolvera-0.1.0rc8/src/tolvera/osc/__init__.py
+-rw-r--r--   0        0        0    16592 2024-03-12 14:02:15.432591 tolvera-0.1.0rc8/src/tolvera/osc/maxmsp.py
+-rw-r--r--   0        0        0     2172 2024-03-12 14:02:15.432747 tolvera-0.1.0rc8/src/tolvera/osc/osc.py
+-rw-r--r--   0        0        0    18115 2024-03-12 14:02:15.432951 tolvera-0.1.0rc8/src/tolvera/osc/oscmap.py
+-rw-r--r--   0        0        0    21320 2024-03-12 14:02:15.433176 tolvera-0.1.0rc8/src/tolvera/osc/pd.py
+-rw-r--r--   0        0        0     8050 2024-03-12 14:02:15.433346 tolvera-0.1.0rc8/src/tolvera/osc/update.py
+-rw-r--r--   0        0        0    18350 2024-04-05 19:33:09.067969 tolvera-0.1.0rc8/src/tolvera/particles.py
+-rw-r--r--   0        0        0     8746 2024-03-12 14:02:15.433864 tolvera-0.1.0rc8/src/tolvera/patches.py
+-rw-r--r--   0        0        0    20397 2024-03-13 09:04:51.448910 tolvera-0.1.0rc8/src/tolvera/pixels.py
+-rw-r--r--   0        0        0     8299 2024-04-14 18:45:30.236884 tolvera-0.1.0rc8/src/tolvera/sf/__init__.py
+-rw-r--r--   0        0        0    11293 2024-03-12 14:02:15.434348 tolvera-0.1.0rc8/src/tolvera/sketchbook.py
+-rw-r--r--   0        0        0     1603 2024-03-12 14:02:15.434519 tolvera-0.1.0rc8/src/tolvera/species.py
+-rw-r--r--   0        0        0    15351 2024-03-12 14:02:15.434756 tolvera-0.1.0rc8/src/tolvera/state.py
+-rw-r--r--   0        0        0     2753 2024-03-12 14:02:15.434914 tolvera-0.1.0rc8/src/tolvera/taichi_.py
+-rw-r--r--   0        0        0     7364 2024-03-16 14:25:42.689663 tolvera-0.1.0rc8/src/tolvera/tolvera_.py
+-rw-r--r--   0        0        0    13382 2024-03-12 14:02:15.435388 tolvera-0.1.0rc8/src/tolvera/utils.py
+-rw-r--r--   0        0        0     1641 2024-04-06 20:24:19.369051 tolvera-0.1.0rc8/src/tolvera/vera/__init__.py
+-rw-r--r--   0        0        0     1410 2024-01-28 15:19:14.309793 tolvera-0.1.0rc8/src/tolvera/vera/attractors.py
+-rw-r--r--   0        0        0     1250 2024-04-06 17:13:45.518822 tolvera-0.1.0rc8/src/tolvera/vera/diffline.py
+-rw-r--r--   0        0        0     5117 2024-04-05 19:16:35.354112 tolvera-0.1.0rc8/src/tolvera/vera/flock.py
+-rw-r--r--   0        0        0     6658 2024-03-20 11:17:12.058891 tolvera-0.1.0rc8/src/tolvera/vera/flock2.py
+-rw-r--r--   0        0        0     4933 2024-03-19 11:20:46.646127 tolvera-0.1.0rc8/src/tolvera/vera/flock_shiffman.py
+-rw-r--r--   0        0        0     9569 2024-04-06 20:21:36.901912 tolvera-0.1.0rc8/src/tolvera/vera/forces.py
+-rw-r--r--   0        0        0     1436 2024-04-06 19:11:18.568109 tolvera-0.1.0rc8/src/tolvera/vera/geom.py
+-rw-r--r--   0        0        0     2558 2024-01-18 21:45:30.996549 tolvera-0.1.0rc8/src/tolvera/vera/nca.py
+-rw-r--r--   0        0        0     2618 2024-04-05 18:26:46.699886 tolvera-0.1.0rc8/src/tolvera/vera/particle_life.py
+-rw-r--r--   0        0        0     4145 2024-04-10 08:39:25.013654 tolvera-0.1.0rc8/src/tolvera/vera/reaction_diffusion.py
+-rw-r--r--   0        0        0     8254 2024-03-12 14:02:15.437046 tolvera-0.1.0rc8/src/tolvera/vera/slime.py
+-rw-r--r--   0        0        0     5944 2024-03-12 14:02:15.437195 tolvera-0.1.0rc8/src/tolvera/vera/swarmalators.py
+-rw-r--r--   0        0        0     2761 2024-03-21 11:59:27.308477 tolvera-0.1.0rc8/src/tolvera/vera/viscek.py
+-rw-r--r--   0        0        0     8428 1970-01-01 00:00:00.000000 tolvera-0.1.0rc8/PKG-INFO
```

### Comparing `tolvera-0.1.0rc10/LICENSE` & `tolvera-0.1.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/README.md` & `tolvera-0.1.0rc8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,106 @@
-# Tölvera
+Metadata-Version: 2.1
+Name: tolvera
+Version: 0.1.0rc8
+Summary: Tölvera is a library for exploring music interaction with artificial life and self-organising systems.
+Home-page: https://github.com/Intelligent-Instruments-Lab/tolvera
+License: AGPL-3.0
+Author: Jack Armitage
+Author-email: jack.armitage@me.com
+Requires-Python: >=3.10,<3.12
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: anguilla-iml (>=0.1.0b4,<0.2.0)
+Requires-Dist: iipyper (>=0.1.0b1,<0.2.0)
+Requires-Dist: jsons (>=1.6.3,<2.0.0)
+Requires-Dist: mediapipe (==0.10.9)
+Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
+Requires-Dist: sardine (>=0.0.0b3,<0.0.1)
+Requires-Dist: signalflow (>=0.4.8,<0.5.0)
+Requires-Dist: taichi (>=1.7.0,<2.0.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
+Project-URL: Documentation, https://intelligent-instruments-lab.github.io/tolvera/
+Project-URL: Repository, https://github.com/Intelligent-Instruments-Lab/tolvera
+Description-Content-Type: text/markdown
 
-[Tölvera](https://tolvera.is) is a Python library designed for [composing together](https://arxiv.org/abs/2303.06777) and interacting with [basal](https://royalsocietypublishing.org/doi/full/10.1098/rstb.2019.0750) [agencies](https://link.springer.com/article/10.1007/s00018-023-04790-z), inspired by fields such as artificial life (ALife) and self-organising systems. 
-It provides creative coding-style APIs that allow users to combine and compose various built-in behaviours, such as flocking, slime mold growth, and swarming, and also author their own. 
-With built-in support for Open Sound Control (OSC) via [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper) and interactive machine learning (IML) via [anguilla](https://github.com/Intelligent-Instruments-Lab/anguilla), Tölvera interfaces with and rapidly maps onto existing creative computing software and hardware, striving to be both an accessible and powerful tool for exploring [diverse intelligence](https://www.frontiersin.org/articles/10.3389/fnsys.2022.768201/full) in artistic contexts.
+# Tölvera
 
-Inspired by our lab's location in Iceland, the word Tölvera is an Icelandic [kenning](https://en.wikipedia.org/wiki/Kenning) based on _tölva_ meaning computer, from _tala_ (number) and _völva_ (prophetess), and _vera_ (being), composed together as _number being_.
+[Tölvera](https://tolvera.is) is a library for exploring musical performance with artificial life (ALife) and self-organising systems. The word is an Icelandic [kenning](https://en.wikipedia.org/wiki/Kenning):
 
-We have employed Tölvera in various collaborative artistic works, including musical performances, compositions, and multimedia installations (see [`references.bib`](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib) for peer-reviewed publications).
-Tölvera's role in these pieces has mainly been "mappable behaviour engine", where interface inputs can control Tölvera programs, and Tölvera runtime data can control interface outputs, in practically any combination.
-In this way, and to controllable degrees, Tölvera can contribute to the underlying dynamics of a given interactive scenario.
-It can also add a [visual component](https://www.youtube.com/watch?v=W2c8vFmdANY), and equally has been used without projection in [other works](https://marcodonnarumma.com/works/ex-silens/).
+- Tölva = computer, from tala (number) + völva (prophetess)
+- Vera = being
+- Tölvera = number being
 
-Tölvera makes use of [Taichi](https://www.taichi-lang.org/), a domain-specific language embedded in Python that enables parallelisation, and is experimental software subject to change.
+Tölvera is written in [Taichi](https://www.taichi-lang.org/), a domain-specific language embedded in Python.
 
-We would be happy to have you join us on our [Discord](https://discord.gg/ER7tWds9vM) server!
+This is experimental software and everything is currently subject to change.
 
-## Showcase & Examples
+Join us on the Tölvera [Discord](https://discord.gg/ER7tWds9vM).
 
-Examples can be found at [iil-examples/tolvera](https://github.com/Intelligent-Instruments-Lab/iil-examples/tree/main/tolvera).
-See also the [guide](https://intelligent-instruments-lab.github.io/tolvera/guide), [reference](https://intelligent-instruments-lab.github.io/tolvera/reference) and [experiments](https://intelligent-instruments-lab.github.io/tolvera/experiments) pages.
+## Showcase
 
 [Visit the YouTube Playlist](https://www.youtube.com/embed/ahSXjnYHZLU?&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x) (if you'd like to add a video, please get in touch).
 
 ![type:video](https://www.youtube.com/embed/ahSXjnYHZLU?&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x)
 
 <!-- [![](assets/images/tolvera.jpg)](https://www.youtube.com/watch?v=ahSXjnYHZLU&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x&pp=gAQBiAQB) -->
 
+## Features
+
+- `tv.v`: a collection of "vera" (beings) including Move, Flock, Slime and Swarm, with more being continuously added. Vera can be combined and composed in various ways.
+- `tv.p`: extensible particle system. Particles are divided into multiple species, where each species has a unique relationship with every other species, including itself
+- `tv.s`: n-dimensional state structures that can be used by "vera", including built-in OSC and IML creation (see below).
+- `tv.px`: drawing library including various shapes and blend modes, styled similarly to p5.js etc.
+- `tv.osc`: Open Sound Control (OSC) via [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper), including automated export of OSC schemas to JSON, XML, Pure Data (Pd), Max/MSP (SuperCollider TBC).
+- `tv.iml`: Interactive Machine Learning via [anguilla](https://github.com/Intelligent-Instruments-Lab/anguilla).
+- `tv.ti`: Taichi-based simulation and rendering engine. Can be run "headless" (without graphics).
+- `tv.cv`: computer vision integration based on OpenCV and Mediapipe.
+
+## Examples
+
+Examples can be found at [iil-examples/tolvera](https://github.com/Intelligent-Instruments-Lab/iil-examples/tree/main/tolvera).
+When run as a script, Tölvera program looks like this:
+
+```py
+from tolvera import Tolvera, run
+
+def main(**kwargs):
+    tv = Tolvera(**kwargs)
+
+    @tv.render
+    def _():
+        return tv.px
+
+if __name__ == '__main__':
+    run(main)
+```
+
 ## Install
 
 Taichi [supports numerous operating systems and backends](https://docs.taichi-lang.org/docs/hello_world#supported-systems-and-backends).
 If you plan on using Vulkan for graphics (recommended for macOS), you may need to [install the Vulkan SDK](https://docs.taichi-lang.org/docs/hello_world#supported-systems-and-backends) first and restart your machine.
 
 Tölvera is [registered on PyPI](https://pypi.org/project/tolvera) and can be installed via a Python package manager such as `pip`:
 
 ```sh
 pip install tolvera
 ```
 
 ## Develop
 
-For development, we use [`poetry`](https://python-poetry.org/).
-Fork/clone this repository and install the package with `poetry:
+Fork/clone this repository and install the package with `poetry`:
 
 ```sh
 git clone https://github.com/Intelligent-Instruments-Lab/tolvera # (or clone your own fork)
 cd tolvera
 poetry install
 ```
 
-## Known Issues & Limitations
-
-- Tölvera currently [does not support Python 3.12 and above](https://github.com/taichi-dev/taichi/issues/8365) - a Python 3.11 installation is recommended.
-This can be created in the following way using [miniconda](https://docs.anaconda.com/free/miniconda/index.html):
-```sh
-conda create -n tolvera python=3.11
-conda activate tolvera
-```
-- Tölvera does not support Intel-based Apple devices (due to [`anguilla`](https://github.com/Intelligent-Instruments-Lab/anguilla)'s FAISS dependency, and Mediapipe not supporting Intel Macs).
-- On macOS, [an OpenMP issue](https://github.com/pytorch/pytorch/issues/78490) may prevent Tölvera programs from running, which can be addressed by adding the following environment variable:
-```sh
-export KMP_DUPLICATE_LIB_OK=TRUE
-```
-- Sonification via [SignalFlow](https://signalflow.dev) does not work on Windows.
-- Mediapipe versions [may need to be downgraded](https://github.com/google/mediapipe/issues/5168) in order to work on macOS and Windows.
-
 ## Contribute
 
 We welcome [Pull Requests](https://github.com/Intelligent-Instruments-Lab/tolvera/pulls) across all areas of the project:
 
 - Addressing [Issues](https://github.com/Intelligent-Instruments-Lab/tolvera/issues)
 - Adding features (see [Issues](https://github.com/Intelligent-Instruments-Lab/tolvera/issues) and [Discussion](https://github.com/Intelligent-Instruments-Lab/tolvera/discussion))
 - [Examples](https://github.com/Intelligent-Instruments-Lab/iil-examples/tolvera)
@@ -85,51 +118,62 @@
 Across the project, we follow the [Berlin Code of Conduct](https://berlincodeofconduct.org/). 
 Please get in touch if you experience or witness any conduct issues.
 
 ## Roadmap
 
 See [Discussion](https://github.com/Intelligent-Instruments-Lab/tolvera/discussion).
 
-## Citation
+## Citing
 
-Tölvera is being written about and used in a number of contexts (see [references.bib](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib)).
-The current canonical citation is our [NIME 2024](https://www.nime2024.org/) paper:
+Tölvera is being written about and used in a number of contexts (see [references.bib](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib)), here are a few recent examples:
 
 ```bibtex
-@inproceedings{armitageTolveraComposingBasal2024,
-  title = {T{\"o}lvera: {{Composing With Basal Agencies}}},
-  booktitle = {Proc. {{New Interfaces}} for {{Musical Expression}}},
-  author = {Armitage, Jack and Shepardson, Victor and Magnusson, Thor},
-  year = {2024},
-  address = {Utrecht, NL},
+@inproceedings{armitageAgentialScoresExploring2023,
+  Address = {Boston, Massachusetts, USA},
+  Author = { Jack Armitage and Thor Magnusson },
+  Title = {Agential Scores: Artificial Life for Emergent, Self-Organising and Entangled Music Notation},
+  Booktitle = {Proceedings of the International Conference on Technologies for Music Notation and Representation -- TENOR'2023},
+  Pages = {51 - 61},
+  Year = {2023},
+  Editor = {Anthony Paul De Ritis and Victor Zappi and Jeremy Van Buskirk and John Mallia},
+  Publisher = {Northeastern University},
+  ISBN = {978-0-6481592-7-8}
+}
+
+@inproceedings{armitageStrengjavera2023,
+  title = {Strengjavera},
+  booktitle = {{{AI Music Creativity}} 2023},
+  author = {Armitage, Jack},
+  year = {2023},
+  address = {{University of Sussex, Brighton, UK}},
+  doi = {10.5281/zenodo.8329855},
+  ISBN = {978-0-9957862-9-5},
+  url = {https://zenodo.org/records/8329855}
 }
 ```
 
 ## Inspiration
 
-- [Michael Levin](https://en.wikipedia.org/wiki/Michael_Levin_(biologist))
 - [SwissGL](https://swiss.gl)
 - [Lenia](https://chakazul.github.io/lenia.html)
 - Particle Life (attributed to various, see for example [Clusters](https://www.ventrella.com/Clusters/))
 - [Journey to the Microcosmos](https://www.youtube.com/@journeytomicro)
 - [Complexity Explorables](https://www.complexity-explorables.org/)
 
 ## Contact
 
-Tölvera is developed primarily by [Jack Armitage](https://jackarmitage.com) and [collaborators](https://iil.is/people) at the [Intelligent Instruments Lab](https://iil.is/about). 
-Get in touch to [collaborate](https://iil.is/collaborate):
+`tolvera` is developed by the [Intelligent Instruments Lab](https://iil.is/about). Get in touch to [collaborate](https://iil.is/collaborate):
 
  ◦ <a href="https://iil.is" target="_blank" title="Intelligent Instrumets Lab">iil.is</a> ◦ 
 <a href="https://facebook.com/intelligentinstrumentslab" target="_blank" title="facebook.com">Facebook</a> ◦ 
 <a href="https://instagram.com/intelligentinstruments" target="_blank" title="instagram.com">Instagram</a> ◦ 
 <a href="https://x.com/_iil_is" target="_blank" title="x.com">X (Twitter)</a> ◦ 
 <a href="https://youtube.com/@IntelligentInstruments" target="_blank" title="youtube.com">YouTube</a> ◦ 
 <a href="https://discord.gg/fY9GYMebtJ" target="_blank" title="discord.gg">Discord</a> ◦ 
 <a href="https://github.com/intelligent-instruments-lab" target="_blank" title="github.com">GitHub</a> ◦ 
 <a href="https://www.linkedin.com/company/intelligent-instruments-lab" target="_blank" title="www.linkedin.com">LinkedIn</a> ◦ 
-<a href="mailto:jack@hi.is" target="_blank" title="">Email</a> ◦ 
+<a href="mailto:iil@lhi.is" target="_blank" title="">Email</a> ◦ 
 
-## Acknowledgements
+## Funding
 
-We thank the Taichi community for their wonderful project, that makes Tölvera possible.
+The Intelligent Instruments project (INTENT) is funded by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 101001848).
 
-The [Intelligent Instruments](https://iil.is) project (INTENT) is funded by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 101001848).
```

### Comparing `tolvera-0.1.0rc10/pyproject.toml` & `tolvera-0.1.0rc8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tolvera"
 packages = [{ include = "tolvera", from = "src"}]
-version = "0.1.0-rc10"
+version = "0.1.0-rc8"
 description = "Tölvera is a library for exploring music interaction with artificial life and self-organising systems."
 authors = ["Jack Armitage <jack.armitage@me.com>"]
 readme = "README.md"
 license = "AGPL-3.0"
 repository = "https://github.com/Intelligent-Instruments-Lab/tolvera"
 documentation = "https://intelligent-instruments-lab.github.io/tolvera/"
 
@@ -14,26 +14,26 @@
 taichi = "^1.7.0"
 jsons = "^1.6.3"
 opencv-python = "^4.8.1.78"
 iipyper = "^0.1.0b1"
 anguilla-iml = "^0.1.0b4"
 sardine = "^0.0.0b3"
 mediapipe = "0.10.9"
+signalflow = "^0.4.8"
 torch = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-video = "^1.5.0"
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
 mkdocs-gen-files = "^0.5.0"
 mkdocs-include-markdown-plugin = "^6.0.4"
 mkdocs-material = "^9.4.8"
 mkdocs-material-extensions = "^1.3"
 mkdocs-autorefs = "^0.5.0"
-mkdocs-awesome-pages-plugin = "^2.9.2"
 pytest = "^7.4.3"
 black = "^23.11.0"
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tolvera-0.1.0rc10/src/tolvera/__main__.py` & `tolvera-0.1.0rc8/src/tolvera/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     print("Running demo...")
     tv = Tolvera(**kwargs)
 
     @tv.render
     def _():
         """Render function that draws flocking particles."""
         tv.px.diffuse(0.99)
+        tv.p()
         tv.v.flock(tv.p)
         tv.px.particles(tv.p, tv.s.species, "circle")
         return tv.px
 
 
 def main(**kwargs):
     """Run Tölvera with kwargs.
```

### Comparing `tolvera-0.1.0rc10/src/tolvera/context.py` & `tolvera-0.1.0rc8/src/tolvera/context.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/cv.py` & `tolvera-0.1.0rc8/src/tolvera/cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     def __init__(self, context, **kwargs) -> None:
         self.ctx = context
         self.x, self.y = self.ctx.x, self.ctx.y
         self.px = Pixels(self.ctx, **kwargs)
         self.frame_rgb = np.zeros((self.y, self.x, 3), np.uint8)
         self.ggui_fps_limit = kwargs.get("ggui_fps_limit", 120)
         self.substeps = kwargs.get("substeps", 2)
+        self.invert = kwargs.get("invert", True)
         self.colormode = kwargs.get("colormode", "rgba")
         self.device = kwargs.get("device", 0)
         self._camera = kwargs.get("camera", False)
         self.cc_frame = np.zeros((self.y, self.x, 3), np.uint8)
         self.cc_frame_f32 = np.zeros((self.y, self.x, 3), np.float32)
         self.diff = np.zeros((self.y, self.x, 3), np.uint8)
         self.diff_p = 0.0
```

### Comparing `tolvera-0.1.0rc10/src/tolvera/iml.py` & `tolvera-0.1.0rc8/src/tolvera/iml.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/mp/face.py` & `tolvera-0.1.0rc8/src/tolvera/mp/face.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/mp/face_mesh.py` & `tolvera-0.1.0rc8/src/tolvera/mp/face_mesh.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/mp/face_mesh_connections.py` & `tolvera-0.1.0rc8/src/tolvera/mp/face_mesh_connections.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/mp/hands.py` & `tolvera-0.1.0rc8/src/tolvera/mp/hands.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/mp/pose.py` & `tolvera-0.1.0rc8/src/tolvera/mp/pose.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/npndarray_dict.py` & `tolvera-0.1.0rc8/src/tolvera/npndarray_dict.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/osc/maxmsp.py` & `tolvera-0.1.0rc8/src/tolvera/osc/maxmsp.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/osc/osc.py` & `tolvera-0.1.0rc8/src/tolvera/osc/osc.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/osc/oscmap.py` & `tolvera-0.1.0rc8/src/tolvera/osc/oscmap.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/osc/pd.py` & `tolvera-0.1.0rc8/src/tolvera/osc/pd.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/osc/update.py` & `tolvera-0.1.0rc8/src/tolvera/osc/update.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/particles.py` & `tolvera-0.1.0rc8/src/tolvera/particles.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/patches.py` & `tolvera-0.1.0rc8/src/tolvera/patches.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/pixels.py` & `tolvera-0.1.0rc8/src/tolvera/pixels.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/sketchbook.py` & `tolvera-0.1.0rc8/src/tolvera/sketchbook.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/species.py` & `tolvera-0.1.0rc8/src/tolvera/species.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/state.py` & `tolvera-0.1.0rc8/src/tolvera/state.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/taichi_.py` & `tolvera-0.1.0rc8/src/tolvera/taichi_.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/tolvera_.py` & `tolvera-0.1.0rc8/src/tolvera/tolvera_.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/utils.py` & `tolvera-0.1.0rc8/src/tolvera/utils.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/vera/__init__.py` & `tolvera-0.1.0rc8/src/tolvera/vera/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """The Vera module provides a wrapper for all available forces and behaviours."""
 
 from . import forces
+from . import geom
 from .flock import Flock
+from .flock2 import Flock2
 from .reaction_diffusion import ReactionDiffusion
 from .slime import Slime
 from .particle_life import ParticleLife
 from .swarmalators import Swarmalators
 
 class Vera:
     """The Vera class provides a wrapper for all available forces and behaviours,
@@ -15,23 +17,30 @@
         
         Args:
             tolvera (Tolvera): A Tolvera instance.
             **kwargs: Keyword arguments passed to the Vera.
         """
         self.tv = tolvera
         self.add_forces_to_self()
+        # self.add_geom_to_self()
         self.flock = Flock(tolvera, **kwargs)
+        self.flock2 = Flock2(tolvera, **kwargs)
         self.slime = Slime(tolvera, **kwargs)
         self.rd = ReactionDiffusion(tolvera, **kwargs)
         self.plife = ParticleLife(tolvera, **kwargs)
         self.swarm = Swarmalators(tolvera, **kwargs)
 
     def add_forces_to_self(self):
         """Add all forces to the Vera instance."""
-        for force in forces.__all__:
-            setattr(self, force, getattr(forces, force))
+        for f in forces.__all__:
+            setattr(self, f, getattr(forces, f))
+    
+    def add_geom_to_self(self):
+        """Add all geom functions to the Vera instance."""
+        for g in geom.__all__:
+            setattr(self, g, getattr(geom, g))
 
     def randomise(self):
         """Randomise all forces and behaviours."""
         self.flock.randomise()
         self.slime.randomise()
         self.rd.randomise()
```

### Comparing `tolvera-0.1.0rc10/src/tolvera/vera/flock.py` & `tolvera-0.1.0rc8/src/tolvera/vera/flock.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/vera/forces.py` & `tolvera-0.1.0rc8/src/tolvera/vera/forces.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/vera/particle_life.py` & `tolvera-0.1.0rc8/src/tolvera/vera/particle_life.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/vera/reaction_diffusion.py` & `tolvera-0.1.0rc8/src/tolvera/vera/reaction_diffusion.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/vera/slime.py` & `tolvera-0.1.0rc8/src/tolvera/vera/slime.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/src/tolvera/vera/swarmalators.py` & `tolvera-0.1.0rc8/src/tolvera/vera/swarmalators.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc10/PKG-INFO` & `tolvera-0.1.0rc8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,80 @@
-Metadata-Version: 2.1
-Name: tolvera
-Version: 0.1.0rc10
-Summary: Tölvera is a library for exploring music interaction with artificial life and self-organising systems.
-Home-page: https://github.com/Intelligent-Instruments-Lab/tolvera
-License: AGPL-3.0
-Author: Jack Armitage
-Author-email: jack.armitage@me.com
-Requires-Python: >=3.10,<3.12
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anguilla-iml (>=0.1.0b4,<0.2.0)
-Requires-Dist: iipyper (>=0.1.0b1,<0.2.0)
-Requires-Dist: jsons (>=1.6.3,<2.0.0)
-Requires-Dist: mediapipe (==0.10.9)
-Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
-Requires-Dist: sardine (>=0.0.0b3,<0.0.1)
-Requires-Dist: taichi (>=1.7.0,<2.0.0)
-Requires-Dist: torch (>=2.2.2,<3.0.0)
-Project-URL: Documentation, https://intelligent-instruments-lab.github.io/tolvera/
-Project-URL: Repository, https://github.com/Intelligent-Instruments-Lab/tolvera
-Description-Content-Type: text/markdown
-
 # Tölvera
 
-[Tölvera](https://tolvera.is) is a Python library designed for [composing together](https://arxiv.org/abs/2303.06777) and interacting with [basal](https://royalsocietypublishing.org/doi/full/10.1098/rstb.2019.0750) [agencies](https://link.springer.com/article/10.1007/s00018-023-04790-z), inspired by fields such as artificial life (ALife) and self-organising systems. 
-It provides creative coding-style APIs that allow users to combine and compose various built-in behaviours, such as flocking, slime mold growth, and swarming, and also author their own. 
-With built-in support for Open Sound Control (OSC) via [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper) and interactive machine learning (IML) via [anguilla](https://github.com/Intelligent-Instruments-Lab/anguilla), Tölvera interfaces with and rapidly maps onto existing creative computing software and hardware, striving to be both an accessible and powerful tool for exploring [diverse intelligence](https://www.frontiersin.org/articles/10.3389/fnsys.2022.768201/full) in artistic contexts.
-
-Inspired by our lab's location in Iceland, the word Tölvera is an Icelandic [kenning](https://en.wikipedia.org/wiki/Kenning) based on _tölva_ meaning computer, from _tala_ (number) and _völva_ (prophetess), and _vera_ (being), composed together as _number being_.
+[Tölvera](https://tolvera.is) is a library for exploring musical performance with artificial life (ALife) and self-organising systems. The word is an Icelandic [kenning](https://en.wikipedia.org/wiki/Kenning):
 
-We have employed Tölvera in various collaborative artistic works, including musical performances, compositions, and multimedia installations (see [`references.bib`](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib) for peer-reviewed publications).
-Tölvera's role in these pieces has mainly been "mappable behaviour engine", where interface inputs can control Tölvera programs, and Tölvera runtime data can control interface outputs, in practically any combination.
-In this way, and to controllable degrees, Tölvera can contribute to the underlying dynamics of a given interactive scenario.
-It can also add a [visual component](https://www.youtube.com/watch?v=W2c8vFmdANY), and equally has been used without projection in [other works](https://marcodonnarumma.com/works/ex-silens/).
+- Tölva = computer, from tala (number) + völva (prophetess)
+- Vera = being
+- Tölvera = number being
 
-Tölvera makes use of [Taichi](https://www.taichi-lang.org/), a domain-specific language embedded in Python that enables parallelisation, and is experimental software subject to change.
+Tölvera is written in [Taichi](https://www.taichi-lang.org/), a domain-specific language embedded in Python.
 
-We would be happy to have you join us on our [Discord](https://discord.gg/ER7tWds9vM) server!
+This is experimental software and everything is currently subject to change.
 
-## Showcase & Examples
+Join us on the Tölvera [Discord](https://discord.gg/ER7tWds9vM).
 
-Examples can be found at [iil-examples/tolvera](https://github.com/Intelligent-Instruments-Lab/iil-examples/tree/main/tolvera).
-See also the [guide](https://intelligent-instruments-lab.github.io/tolvera/guide), [reference](https://intelligent-instruments-lab.github.io/tolvera/reference) and [experiments](https://intelligent-instruments-lab.github.io/tolvera/experiments) pages.
+## Showcase
 
 [Visit the YouTube Playlist](https://www.youtube.com/embed/ahSXjnYHZLU?&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x) (if you'd like to add a video, please get in touch).
 
 ![type:video](https://www.youtube.com/embed/ahSXjnYHZLU?&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x)
 
 <!-- [![](assets/images/tolvera.jpg)](https://www.youtube.com/watch?v=ahSXjnYHZLU&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x&pp=gAQBiAQB) -->
 
+## Features
+
+- `tv.v`: a collection of "vera" (beings) including Move, Flock, Slime and Swarm, with more being continuously added. Vera can be combined and composed in various ways.
+- `tv.p`: extensible particle system. Particles are divided into multiple species, where each species has a unique relationship with every other species, including itself
+- `tv.s`: n-dimensional state structures that can be used by "vera", including built-in OSC and IML creation (see below).
+- `tv.px`: drawing library including various shapes and blend modes, styled similarly to p5.js etc.
+- `tv.osc`: Open Sound Control (OSC) via [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper), including automated export of OSC schemas to JSON, XML, Pure Data (Pd), Max/MSP (SuperCollider TBC).
+- `tv.iml`: Interactive Machine Learning via [anguilla](https://github.com/Intelligent-Instruments-Lab/anguilla).
+- `tv.ti`: Taichi-based simulation and rendering engine. Can be run "headless" (without graphics).
+- `tv.cv`: computer vision integration based on OpenCV and Mediapipe.
+
+## Examples
+
+Examples can be found at [iil-examples/tolvera](https://github.com/Intelligent-Instruments-Lab/iil-examples/tree/main/tolvera).
+When run as a script, Tölvera program looks like this:
+
+```py
+from tolvera import Tolvera, run
+
+def main(**kwargs):
+    tv = Tolvera(**kwargs)
+
+    @tv.render
+    def _():
+        return tv.px
+
+if __name__ == '__main__':
+    run(main)
+```
+
 ## Install
 
 Taichi [supports numerous operating systems and backends](https://docs.taichi-lang.org/docs/hello_world#supported-systems-and-backends).
 If you plan on using Vulkan for graphics (recommended for macOS), you may need to [install the Vulkan SDK](https://docs.taichi-lang.org/docs/hello_world#supported-systems-and-backends) first and restart your machine.
 
 Tölvera is [registered on PyPI](https://pypi.org/project/tolvera) and can be installed via a Python package manager such as `pip`:
 
 ```sh
 pip install tolvera
 ```
 
 ## Develop
 
-For development, we use [`poetry`](https://python-poetry.org/).
-Fork/clone this repository and install the package with `poetry:
+Fork/clone this repository and install the package with `poetry`:
 
 ```sh
 git clone https://github.com/Intelligent-Instruments-Lab/tolvera # (or clone your own fork)
 cd tolvera
 poetry install
 ```
 
-## Known Issues & Limitations
-
-- Tölvera currently [does not support Python 3.12 and above](https://github.com/taichi-dev/taichi/issues/8365) - a Python 3.11 installation is recommended.
-This can be created in the following way using [miniconda](https://docs.anaconda.com/free/miniconda/index.html):
-```sh
-conda create -n tolvera python=3.11
-conda activate tolvera
-```
-- Tölvera does not support Intel-based Apple devices (due to [`anguilla`](https://github.com/Intelligent-Instruments-Lab/anguilla)'s FAISS dependency, and Mediapipe not supporting Intel Macs).
-- On macOS, [an OpenMP issue](https://github.com/pytorch/pytorch/issues/78490) may prevent Tölvera programs from running, which can be addressed by adding the following environment variable:
-```sh
-export KMP_DUPLICATE_LIB_OK=TRUE
-```
-- Sonification via [SignalFlow](https://signalflow.dev) does not work on Windows.
-- Mediapipe versions [may need to be downgraded](https://github.com/google/mediapipe/issues/5168) in order to work on macOS and Windows.
-
 ## Contribute
 
 We welcome [Pull Requests](https://github.com/Intelligent-Instruments-Lab/tolvera/pulls) across all areas of the project:
 
 - Addressing [Issues](https://github.com/Intelligent-Instruments-Lab/tolvera/issues)
 - Adding features (see [Issues](https://github.com/Intelligent-Instruments-Lab/tolvera/issues) and [Discussion](https://github.com/Intelligent-Instruments-Lab/tolvera/discussion))
 - [Examples](https://github.com/Intelligent-Instruments-Lab/iil-examples/tolvera)
@@ -110,52 +92,61 @@
 Across the project, we follow the [Berlin Code of Conduct](https://berlincodeofconduct.org/). 
 Please get in touch if you experience or witness any conduct issues.
 
 ## Roadmap
 
 See [Discussion](https://github.com/Intelligent-Instruments-Lab/tolvera/discussion).
 
-## Citation
+## Citing
 
-Tölvera is being written about and used in a number of contexts (see [references.bib](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib)).
-The current canonical citation is our [NIME 2024](https://www.nime2024.org/) paper:
+Tölvera is being written about and used in a number of contexts (see [references.bib](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib)), here are a few recent examples:
 
 ```bibtex
-@inproceedings{armitageTolveraComposingBasal2024,
-  title = {T{\"o}lvera: {{Composing With Basal Agencies}}},
-  booktitle = {Proc. {{New Interfaces}} for {{Musical Expression}}},
-  author = {Armitage, Jack and Shepardson, Victor and Magnusson, Thor},
-  year = {2024},
-  address = {Utrecht, NL},
+@inproceedings{armitageAgentialScoresExploring2023,
+  Address = {Boston, Massachusetts, USA},
+  Author = { Jack Armitage and Thor Magnusson },
+  Title = {Agential Scores: Artificial Life for Emergent, Self-Organising and Entangled Music Notation},
+  Booktitle = {Proceedings of the International Conference on Technologies for Music Notation and Representation -- TENOR'2023},
+  Pages = {51 - 61},
+  Year = {2023},
+  Editor = {Anthony Paul De Ritis and Victor Zappi and Jeremy Van Buskirk and John Mallia},
+  Publisher = {Northeastern University},
+  ISBN = {978-0-6481592-7-8}
+}
+
+@inproceedings{armitageStrengjavera2023,
+  title = {Strengjavera},
+  booktitle = {{{AI Music Creativity}} 2023},
+  author = {Armitage, Jack},
+  year = {2023},
+  address = {{University of Sussex, Brighton, UK}},
+  doi = {10.5281/zenodo.8329855},
+  ISBN = {978-0-9957862-9-5},
+  url = {https://zenodo.org/records/8329855}
 }
 ```
 
 ## Inspiration
 
-- [Michael Levin](https://en.wikipedia.org/wiki/Michael_Levin_(biologist))
 - [SwissGL](https://swiss.gl)
 - [Lenia](https://chakazul.github.io/lenia.html)
 - Particle Life (attributed to various, see for example [Clusters](https://www.ventrella.com/Clusters/))
 - [Journey to the Microcosmos](https://www.youtube.com/@journeytomicro)
 - [Complexity Explorables](https://www.complexity-explorables.org/)
 
 ## Contact
 
-Tölvera is developed primarily by [Jack Armitage](https://jackarmitage.com) and [collaborators](https://iil.is/people) at the [Intelligent Instruments Lab](https://iil.is/about). 
-Get in touch to [collaborate](https://iil.is/collaborate):
+`tolvera` is developed by the [Intelligent Instruments Lab](https://iil.is/about). Get in touch to [collaborate](https://iil.is/collaborate):
 
  ◦ <a href="https://iil.is" target="_blank" title="Intelligent Instrumets Lab">iil.is</a> ◦ 
 <a href="https://facebook.com/intelligentinstrumentslab" target="_blank" title="facebook.com">Facebook</a> ◦ 
 <a href="https://instagram.com/intelligentinstruments" target="_blank" title="instagram.com">Instagram</a> ◦ 
 <a href="https://x.com/_iil_is" target="_blank" title="x.com">X (Twitter)</a> ◦ 
 <a href="https://youtube.com/@IntelligentInstruments" target="_blank" title="youtube.com">YouTube</a> ◦ 
 <a href="https://discord.gg/fY9GYMebtJ" target="_blank" title="discord.gg">Discord</a> ◦ 
 <a href="https://github.com/intelligent-instruments-lab" target="_blank" title="github.com">GitHub</a> ◦ 
 <a href="https://www.linkedin.com/company/intelligent-instruments-lab" target="_blank" title="www.linkedin.com">LinkedIn</a> ◦ 
-<a href="mailto:jack@hi.is" target="_blank" title="">Email</a> ◦ 
-
-## Acknowledgements
-
-We thank the Taichi community for their wonderful project, that makes Tölvera possible.
+<a href="mailto:iil@lhi.is" target="_blank" title="">Email</a> ◦ 
 
-The [Intelligent Instruments](https://iil.is) project (INTENT) is funded by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 101001848).
+## Funding
 
+The Intelligent Instruments project (INTENT) is funded by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 101001848).
```

