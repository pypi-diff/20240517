# Comparing `tmp/avnet_scotty-2024.4.tar.gz` & `tmp/avnet_scotty-2024.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avnet_scotty-2024.4.tar", last modified: Mon Apr 29 14:11:28 2024, max compression
+gzip compressed data, was "avnet_scotty-2024.5rc1.tar", last modified: Fri May 17 15:15:33 2024, max compression
```

## Comparing `avnet_scotty-2024.4.tar` & `avnet_scotty-2024.5rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.704533 avnet_scotty-2024.4/
--rw-r--r--   0 root         (0) root         (0)    32879 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1370 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    23473 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/avnet_scotty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1370 2024-04-29 14:11:28.000000 avnet_scotty-2024.4/avnet_scotty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      564 2024-04-29 14:11:28.000000 avnet_scotty-2024.4/avnet_scotty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 14:11:28.000000 avnet_scotty-2024.4/avnet_scotty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-29 14:11:28.000000 avnet_scotty-2024.4/avnet_scotty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-29 14:11:28.000000 avnet_scotty-2024.4/avnet_scotty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-29 14:11:28.000000 avnet_scotty-2024.4/avnet_scotty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/bumper/
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/bumper/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4006 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/bumper/__main__.py
--rw-r--r--   0 root         (0) root         (0)      171 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)     6896 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scotty
--rwxr-xr-x   0 root         (0) root         (0)     2370 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scotty-runqemu
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/scotty_test/
--rw-r--r--   0 root         (0) root         (0)     4424 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scotty_test/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/scotty_test/menu/
--rw-r--r--   0 root         (0) root         (0)     2746 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scotty_test/menu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/scotty_test/reporter/
--rw-r--r--   0 root         (0) root         (0)     3101 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scotty_test/reporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/scotty_test/runner/
--rw-r--r--   0 root         (0) root         (0)     9890 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scotty_test/runner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/scotty_test/storage/
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scotty_test/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/scotty_test/utils/
--rw-r--r--   0 root         (0) root         (0)     1526 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scotty_test/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:11:28.700533 avnet_scotty-2024.4/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      811 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scripts/vm_bundle.sh
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/scripts/vm_create.sh.template
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 14:11:28.704533 avnet_scotty-2024.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2338 2024-04-29 14:11:24.000000 avnet_scotty-2024.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/
+-rw-r--r--   0 root         (0) root         (0)    32879 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1433 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    23984 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/avnet_scotty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1433 2024-05-17 15:15:33.000000 avnet_scotty-2024.5rc1/avnet_scotty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      564 2024-05-17 15:15:33.000000 avnet_scotty-2024.5rc1/avnet_scotty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 15:15:33.000000 avnet_scotty-2024.5rc1/avnet_scotty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-17 15:15:33.000000 avnet_scotty-2024.5rc1/avnet_scotty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-17 15:15:33.000000 avnet_scotty-2024.5rc1/avnet_scotty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-17 15:15:33.000000 avnet_scotty-2024.5rc1/avnet_scotty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.762577 avnet_scotty-2024.5rc1/bumper/
+-rw-r--r--   0 root         (0) root         (0)      110 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/bumper/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4006 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/bumper/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)     6902 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scotty
+-rwxr-xr-x   0 root         (0) root         (0)     2370 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scotty-runqemu
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.762577 avnet_scotty-2024.5rc1/scotty_test/
+-rw-r--r--   0 root         (0) root         (0)     4424 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scotty_test/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/scotty_test/menu/
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scotty_test/menu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/scotty_test/reporter/
+-rw-r--r--   0 root         (0) root         (0)     3101 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scotty_test/reporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/scotty_test/runner/
+-rw-r--r--   0 root         (0) root         (0)     9890 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scotty_test/runner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/scotty_test/storage/
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scotty_test/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/scotty_test/utils/
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scotty_test/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      811 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scripts/vm_bundle.sh
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/scripts/vm_create.sh.template
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 15:15:33.766577 avnet_scotty-2024.5rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-05-17 15:15:30.000000 avnet_scotty-2024.5rc1/setup.py
```

### Comparing `avnet_scotty-2024.4/LICENSE` & `avnet_scotty-2024.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/PKG-INFO` & `avnet_scotty-2024.5rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2024.4
+Version: 2024.5rc1
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Project-URL: Documentation, https://simple.embedded.avnet.com/?link=tools/scotty/README.html
 Project-URL: SimpleCore Documentation, https://simple.embedded.avnet.com/
 Project-URL: Source Code, https://github.com/avnet-embedded/simplecore-tools/tree/kirkstone/scotty
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: GitPython~=3.1
 Requires-Dist: azure-storage-blob~=12.16
 Requires-Dist: colorama~=0.4
-Requires-Dist: inquirer~=3.0
+Requires-Dist: inquirer==3.0.*
+Requires-Dist: pillow~=10.3
+Requires-Dist: imagehash~=4.3
 
 
 Scotty is a tool to make the process of building the SimpleCore™ Distro distribution
 reproducible on any Linux and Windows computer (compatible with WSL2). It uses a
 container to setup the same environment used by our continuous integration
 process to ensure that the build on your machine will always be successful for
 any of our standard images. Scotty is based on standard open-source tools such as
```

### Comparing `avnet_scotty-2024.4/README.rst` & `avnet_scotty-2024.5rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -58,23 +58,23 @@
 
   .. code-block:: console
 
     echo 'export PATH="$(systemd-path user-binaries):$PATH"' >> ~/.bashrc
 
   .. note::
 
-    A reboot is required for the setting to become effective
+    A reboot is required for the setting to become effective.
 
   You can also install ``scotty`` with
 
   .. code-block:: console
 
     sudo pip install avnet-scotty
 
-  but that requires you to have ``sudo`` rights on your system
+  but that requires you to have ``sudo`` rights on your system.
 
 
 Alternatively, the current development version can be obtained by cloning
 `<https://github.com/avnet-embedded/simplecore-tools>`_.
 
 .. admonition:: Potential pitfall
   :class: ATTENTION
@@ -160,15 +160,15 @@
 
 .. note::
 
   .. code-block:: bash
 
     $ scotty setup --force
 
-  Will allow you to redo the configuration at any point
+  Will allow you to redo the configuration at any point.
 
 
 Building a full image
 ---------------------
 
 A single command is enough to download the sources and build an image:
 
@@ -192,15 +192,15 @@
   .. code-block:: bash
 
     $ scotty info images
 
 Recommended hardware setup
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-For building software pacakges with ``Scotty`` we recommend the following minimal hardware setup
+For building software pacakges with ``Scotty`` we recommend the following minimal hardware setup:
 
 For base images
 
 - 4 Cores / 8 threads CPU
 - 16GB RAM
 - 200GB HDD
 
@@ -208,15 +208,15 @@
 
 - 16 Cores / 32 threads CPU
 - 64Gb RAM
 - 500GB HDD
 
 .. note::
 
-  Other combinations do work as well, but keep in mind that we at least require 2GB of RAM per available CPU thread
+  Other combinations do work as well, but keep in mind that we at least require 2GB of RAM per available CPU thread.
 
 Using Scotty as a helper
 ------------------------
 
 ``Scotty`` can be used to open a shell with a sourced Yocto environment:
 
 .. code-block:: bash
@@ -303,16 +303,16 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 - ``DISTRO``: Can be used to select the Yocto distro and skip selection menu.
 - ``MACHINE``: Can be used to select the Yocto machine and skip selection menu.
 - ``ACCEPT_FSL_EULA``: Can be used to set the Freescale/NXP EULA status and skip
   selection menu if applicable).
 - ``LICENSE_FLAGS_ACCEPTED``: Can be use to allow e.g. commercial licenses in the resulting images.
-- ``UBOOT_ENV_VARS``: Can be use to prepopulate the used u-boot environment (expects a key value list, separated by new lines). To disable pass " "
-- ``SCOTTY_FEATURE_LAYERS``: A space separated list of feature layers (alternative to ``scotty setup --features-layers-set`` - CLI flags have always precedence)
+- ``UBOOT_ENV_VARS``: Can be use to prepopulate the used u-boot environment (expects a key value list, separated by new lines). To disable pass " ".
+- ``SCOTTY_FEATURE_LAYERS``: A space separated list of feature layers (alternative to ``scotty setup --features-layers-set`` - CLI flags have always precedence).
 
 Example
 ^^^^^^^
 
 .. code-block:: bash
 
    $ export ACCEPT_FSL_EULA=1
@@ -343,17 +343,17 @@
 ^^^^^^^^^^^^
 
 .. admonition:: The following will need Administator permission
   :class: ATTENTION
 
   - enable and install ``Windows subsystem for Linux 2`` like decribed `here <https://learn.microsoft.com/en-us/windows/wsl/install>`_.
 
-    We recommend to use the ``Ubuntu`` virtual machine for WSL2
+    We recommend to use the ``Ubuntu`` virtual machine for WSL2.
 
-    **NOTE** only version 2 of WSL is supported
+    **NOTE** only version 2 of WSL is supported.
 
 - install `docker on WSL2 <https://dev.to/bowmanjd/install-docker-on-windows-wsl-without-docker-desktop-34m9>`_
 - install ``openssh``
 
 .. code-block:: console
 
   $ sudo apt update
@@ -418,15 +418,15 @@
 
 after that you can launch your WSL VM and start using ``scotty``.
 
 SSH keys
 ^^^^^^^^
 
 For ``scotty`` to work properly you'll need to create and reference SSH keys for Github, like
-described `on this page <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>`_
+described `on this page <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>`_.
 
 Reusing your SSH keys from Windows
 ##################################
 
 In case you want to reuse your SSH keys from windows just run
 
 .. code-block:: console
@@ -506,31 +506,38 @@
 The tool will download the necessary images and SDKs, run the tests and create a Markdown report that will
 be pushed to the `simplecore-tools repository <https://github.com/avnet-embedded/simplecore-tools>`_.
 
 scotty-layers.yaml
 ==================
 
 All the information ``scotty`` uses is defined in ``scotty-layers.yaml`` in the ``manifest`` repository.
-This file is a ``yaml`` file containing the following sections
+This file is a ``yaml`` file containing the following sections:
 
 base section
 ------------
 
 Allowed number of sections in the ``yaml``: 1
 
 This section defines the layers that are **always** used in any setup.
 
 +-------------+--------+----------------------------+--------------------------------------+
 | Key         | Type   | Description                | Example                              |
 +=============+========+============================+======================================+
 | description | string | Human readable description | description: "My base layers"        |
 +-------------+--------+----------------------------+--------------------------------------+
 | layers      | list   | Paths to layers to be used | layers:                              |
-|             |        |                            |    ? "meta-openembedded/meta-oe"     | 
+|             |        |                            |    ? "meta-openembedded/meta-oe"     |
 +-------------+--------+----------------------------+--------------------------------------+
+| licenses    | list   | additional EULA/licenses   | licenses:                            |
+|             |        | to be accepted by the user |    - path: "meta-layer/EULA.txt"     |
+|             |        |                            |      env: "META_VAR"                 |
+|             |        |                            |      description: "Some explantion"  |
++-------------+--------+----------------------------+--------------------------------------+
+
+**NOTE**: ``licenses`` is optional
 
 distro_* section
 ----------------
 
 Allowed number of sections in the ``yaml``: 1..n
 
 These sections define the possible selections for Yocto’s ``DISTRO`` setting.
```

### Comparing `avnet_scotty-2024.4/avnet_scotty.egg-info/PKG-INFO` & `avnet_scotty-2024.5rc1/avnet_scotty.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2024.4
+Version: 2024.5rc1
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Project-URL: Documentation, https://simple.embedded.avnet.com/?link=tools/scotty/README.html
 Project-URL: SimpleCore Documentation, https://simple.embedded.avnet.com/
 Project-URL: Source Code, https://github.com/avnet-embedded/simplecore-tools/tree/kirkstone/scotty
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: GitPython~=3.1
 Requires-Dist: azure-storage-blob~=12.16
 Requires-Dist: colorama~=0.4
-Requires-Dist: inquirer~=3.0
+Requires-Dist: inquirer==3.0.*
+Requires-Dist: pillow~=10.3
+Requires-Dist: imagehash~=4.3
 
 
 Scotty is a tool to make the process of building the SimpleCore™ Distro distribution
 reproducible on any Linux and Windows computer (compatible with WSL2). It uses a
 container to setup the same environment used by our continuous integration
 process to ensure that the build on your machine will always be successful for
 any of our standard images. Scotty is based on standard open-source tools such as
```

### Comparing `avnet_scotty-2024.4/avnet_scotty.egg-info/SOURCES.txt` & `avnet_scotty-2024.5rc1/avnet_scotty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/bumper/__main__.py` & `avnet_scotty-2024.5rc1/bumper/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/scotty` & `avnet_scotty-2024.5rc1/scotty`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 	TERM \
 	UBOOT_ENV_VARS \
 	"
 # SCOTTY_FEATURES_LAYERS REPO_URL SCOTTY_MACHINE_DIR BUILDDIR
 declare -r scotty_whitelist=${SCOTTY_WHITELIST:-${scotty_whitelist_default}}
 
 if [ "${SCOTTY_DOCKER_IMAGE:-1}" == "1" ]; then
-    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:2024.4"
+    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:2024.5rc1"
 else
     declare -r docker_default_image="${SCOTTY_DOCKER_IMAGE}"
 fi
 
-export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2024.4"
+export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2024.5rc1"
 export SCOTTY_DEFAULT_MANIFEST_NAME="default-release.xml"
 
 debug() {
 	if [ "${SCOTTY_DEBUG:-0}" == "1" ]; then
 		echo -e "\033[1;38m${*}\033[0m"
 	fi
 }
```

### Comparing `avnet_scotty-2024.4/scotty-runqemu` & `avnet_scotty-2024.5rc1/scotty-runqemu`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/scotty_test/__main__.py` & `avnet_scotty-2024.5rc1/scotty_test/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/scotty_test/menu/__init__.py` & `avnet_scotty-2024.5rc1/scotty_test/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/scotty_test/reporter/__init__.py` & `avnet_scotty-2024.5rc1/scotty_test/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/scotty_test/runner/__init__.py` & `avnet_scotty-2024.5rc1/scotty_test/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/scotty_test/storage/__init__.py` & `avnet_scotty-2024.5rc1/scotty_test/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/scotty_test/utils/__init__.py` & `avnet_scotty-2024.5rc1/scotty_test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/scripts/vm_bundle.sh` & `avnet_scotty-2024.5rc1/scripts/vm_bundle.sh`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/scripts/vm_create.sh.template` & `avnet_scotty-2024.5rc1/scripts/vm_create.sh.template`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.4/setup.py` & `avnet_scotty-2024.5rc1/setup.py`

 * *Files identical despite different names*

