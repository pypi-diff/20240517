# Comparing `tmp/container-inspector-32.0.0.tar.gz` & `tmp/container-inspector-32.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container-inspector-32.0.0.tar", last modified: Sat Jul 30 20:58:05 2022, max compression
+gzip compressed data, was "container-inspector-32.0.1.tar", last modified: Sun Jul 31 12:20:47 2022, max compression
```

## Comparing `container-inspector-32.0.0.tar` & `container-inspector-32.0.1.tar`

### file list

```diff
@@ -1,817 +1,817 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.292564 container-inspector-32.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-07-30 20:57:54.000000 container-inspector-32.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.216563 container-inspector-32.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.220563 container-inspector-32.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-07-30 20:57:54.000000 container-inspector-32.0.0/.github/workflows/docs-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-07-30 20:57:54.000000 container-inspector-32.0.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-07-30 20:57:54.000000 container-inspector-32.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-30 20:57:54.000000 container-inspector-32.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-07-30 20:57:54.000000 container-inspector-32.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4872 2022-07-30 20:57:54.000000 container-inspector-32.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-07-30 20:57:54.000000 container-inspector-32.0.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-07-30 20:57:54.000000 container-inspector-32.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-07-30 20:57:54.000000 container-inspector-32.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-07-30 20:58:05.292564 container-inspector-32.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-07-30 20:57:54.000000 container-inspector-32.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-30 20:57:54.000000 container-inspector-32.0.0/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-07-30 20:57:54.000000 container-inspector-32.0.0/azure-pipelines.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)     6310 2022-07-30 20:57:54.000000 container-inspector-32.0.0/configure
--rw-r--r--   0 runner    (1001) docker     (121)     6930 2022-07-30 20:57:54.000000 container-inspector-32.0.0/configure.bat
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-07-30 20:57:54.000000 container-inspector-32.0.0/container-inspector.ABOUT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.220563 container-inspector-32.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-07-30 20:57:54.000000 container-inspector-32.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-07-30 20:57:54.000000 container-inspector-32.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.220563 container-inspector-32.0.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-07-30 20:57:54.000000 container-inspector-32.0.0/docs/scripts/doc8_style_check.sh
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-07-30 20:57:54.000000 container-inspector-32.0.0/docs/scripts/sphinx_build_link_check.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.220563 container-inspector-32.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.220563 container-inspector-32.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     8022 2022-07-30 20:57:54.000000 container-inspector-32.0.0/docs/source/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-07-30 20:57:54.000000 container-inspector-32.0.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.220563 container-inspector-32.0.0/docs/source/contribute/
--rw-r--r--   0 runner    (1001) docker     (121)    10245 2022-07-30 20:57:54.000000 container-inspector-32.0.0/docs/source/contribute/contrib_doc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-30 20:57:54.000000 container-inspector-32.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-07-30 20:57:54.000000 container-inspector-32.0.0/docs/source/skeleton-usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.216563 container-inspector-32.0.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.224563 container-inspector-32.0.0/etc/ci/
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/ci/azure-container-deb.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/ci/azure-container-rpm.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/ci/azure-posix.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/ci/azure-win.yml
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/ci/install_sudo.sh
--rw-r--r--   0 runner    (1001) docker     (121)     8365 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/ci/macports-ci
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/ci/macports-ci.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/ci/mit.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.224563 container-inspector-32.0.0/etc/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3745 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/check_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)     8209 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/fetch_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)     9595 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/gen_pypi_simple.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/gen_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/gen_requirements_dev.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/utils_dejacode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/utils_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)    75964 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/utils_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-07-30 20:57:54.000000 container-inspector-32.0.0/etc/scripts/utils_thirdparty.py.ABOUT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.216563 container-inspector-32.0.0/misc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.224563 container-inspector-32.0.0/misc/docker/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4694 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/docker/download-docker-image.sh
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/docker/download-docker-image.sh.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)    10765 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/docker/download-docker-image.sh.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/docker/download-docker-image.sh.NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.224563 container-inspector-32.0.0/misc/references/
--rw-r--r--   0 runner    (1001) docker     (121)    22439 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/references/docker_image_spec_v1.1.md
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/references/docker_image_spec_v1.1.md.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)    24825 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/references/docker_image_spec_v1.2.md
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/references/docker_image_spec_v1.2.md.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)    20527 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/references/docker_image_spec_v1.md
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-07-30 20:57:54.000000 container-inspector-32.0.0/misc/references/docker_image_spec_v1.md.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-07-30 20:57:54.000000 container-inspector-32.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-07-30 20:57:54.000000 container-inspector-32.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-07-30 20:57:54.000000 container-inspector-32.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-07-30 20:58:05.292564 container-inspector-32.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-07-30 20:57:54.000000 container-inspector-32.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.216563 container-inspector-32.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.224563 container-inspector-32.0.0/src/container_inspector/
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-07-30 20:57:54.000000 container-inspector-32.0.0/src/container_inspector/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5169 2022-07-30 20:57:54.000000 container-inspector-32.0.0/src/container_inspector/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23513 2022-07-30 20:57:54.000000 container-inspector-32.0.0/src/container_inspector/distro.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8834 2022-07-30 20:57:54.000000 container-inspector-32.0.0/src/container_inspector/dockerfile.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    39940 2022-07-30 20:57:54.000000 container-inspector-32.0.0/src/container_inspector/image.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8905 2022-07-30 20:57:54.000000 container-inspector-32.0.0/src/container_inspector/rootfs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6248 2022-07-30 20:57:54.000000 container-inspector-32.0.0/src/container_inspector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.228563 container-inspector-32.0.0/src/container_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-07-30 20:58:05.000000 container-inspector-32.0.0/src/container_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    43982 2022-07-30 20:58:05.000000 container-inspector-32.0.0/src/container_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 20:58:05.000000 container-inspector-32.0.0/src/container_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-07-30 20:58:05.000000 container-inspector-32.0.0/src/container_inspector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 20:58:05.000000 container-inspector-32.0.0/src/container_inspector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-07-30 20:58:05.000000 container-inspector-32.0.0/src/container_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-30 20:58:05.000000 container-inspector-32.0.0/src/container_inspector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.228563 container-inspector-32.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.220563 container-inspector-32.0.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.228563 container-inspector-32.0.0/tests/data/cli/
--rw-r--r--   0 runner    (1001) docker     (121)    12800 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/cli/hello-world.tar
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/cli/hello-world.tar-inventory-from-dir-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/cli/hello-world.tar-inventory-from-tarball-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)    35328 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/cli/she-image_from_scratch-1.0.tar
--rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/cli/she-image_from_scratch-1.0.tar-inventory-from-tarball-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.228563 container-inspector-32.0.0/tests/data/distro/
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/README-chef.md
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/README-nate.md
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/README-zoo.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7048 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/cc0-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/mit.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.220563 container-inspector-32.0.0/tests/data/distro/os-release/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.228563 container-inspector-32.0.0/tests/data/distro/os-release/alpine/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/alpine/alpine-3.8.txt
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/alpine/alpine-3.8.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/alpine/alpine-3.8.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.228563 container-inspector-32.0.0/tests/data/distro/os-release/amazon/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/amazon/amazon-2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/amazon/amazon-2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/amazon/amazon-2.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/amazon/amazon-2018.03.txt
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/amazon/amazon-2018.03.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/amazon/amazon-2018.03.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/amazon/amzon-2016.09.txt
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/amazon/amzon-2016.09.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/amazon/amzon-2016.09.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.228563 container-inspector-32.0.0/tests/data/distro/os-release/antergos/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/antergos/antergos.txt
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/antergos/antergos.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/antergos/antergos.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.232563 container-inspector-32.0.0/tests/data/distro/os-release/arch/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-arm-new.txt
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-arm-new.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-arm-new.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-arm.txt
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-arm.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-arm.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-mini.txt
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-mini.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-mini.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch.txt
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/arch/arch.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.232563 container-inspector-32.0.0/tests/data/distro/os-release/artix/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/artix/artix.txt
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/artix/artix.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/artix/artix.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.232563 container-inspector-32.0.0/tests/data/distro/os-release/centos/
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/centos/centos-7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/centos/centos-7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/centos/centos-7.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.232563 container-inspector-32.0.0/tests/data/distro/os-release/clearlinux/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/clearlinux/clearlinux-1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/clearlinux/clearlinux-1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/clearlinux/clearlinux-1.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.232563 container-inspector-32.0.0/tests/data/distro/os-release/clearos/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/clearos/clearos-7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/clearos/clearos-7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/clearos/clearos-7.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.232563 container-inspector-32.0.0/tests/data/distro/os-release/coreos/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.232563 container-inspector-32.0.0/tests/data/distro/os-release/cumulus/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/cumulus/cumulus-3.7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/cumulus/cumulus-3.7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/cumulus/cumulus-3.7.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.232563 container-inspector-32.0.0/tests/data/distro/os-release/debian/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-11.txt
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-11.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-11.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-7.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-8.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-8.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-9.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-9.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-sid.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-sid.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.236563 container-inspector-32.0.0/tests/data/distro/os-release/distroless/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian11.txt
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian11.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian11.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian9.txt
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian9.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian9.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.236563 container-inspector-32.0.0/tests/data/distro/os-release/elementary/
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-0.4.txt
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-0.4.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-0.4.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-5.1.7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-5.1.7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-5.1.7.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-5.txt
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-5.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-5.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.236563 container-inspector-32.0.0/tests/data/distro/os-release/endless/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/endless/endless-3.2.2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/endless/endless-3.2.2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/endless/endless-3.2.2.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.252563 container-inspector-32.0.0/tests/data/distro/os-release/fedora/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-17.txt
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-17.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-17.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-18.txt
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-18.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-18.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-20.txt
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-20.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-20.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-21.txt
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-21.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-21.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22.txt
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23.txt
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24.txt
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25.txt
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-modular.txt
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-modular.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-modular.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26.txt
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27.txt
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28.txt
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-container.txt
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-container.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-container.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29.txt
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-container.txt
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-container.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-container.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30.txt
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-container.txt
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-container.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-container.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31.txt
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-container.txt
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-container.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-container.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32.txt
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-container.txt
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-container.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-container.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-kde.txt
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-kde.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-kde.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-soas.txt
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-soas.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-soas.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-xfce.txt
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-xfce.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-xfce.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33.txt
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-container.txt
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-container.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-container.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-kde.txt
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-kde.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-kde.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-server.txt
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-server.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-server.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-soas.txt
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-soas.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-soas.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-workstation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-workstation.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-workstation.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-xfce.txt
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-xfce.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-xfce.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34.txt
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-35.txt
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-35.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-35.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-36-pre.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-36-pre.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-36-pre.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.256563 container-inspector-32.0.0/tests/data/distro/os-release/galliumos/
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/galliumos/galliumos-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/galliumos/galliumos-2.1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/galliumos/galliumos-2.1.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.256563 container-inspector-32.0.0/tests/data/distro/os-release/gentoo/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/gentoo/gentoo-new.txt
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/gentoo/gentoo-new.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/gentoo/gentoo-new.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/gentoo/gentoo.txt
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/gentoo/gentoo.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/gentoo/gentoo.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.256563 container-inspector-32.0.0/tests/data/distro/os-release/ios/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ios/ios-xr-6.txt
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ios/ios-xr-6.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ios/ios-xr-6.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.256563 container-inspector-32.0.0/tests/data/distro/os-release/kali/
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kali/kali-2018.4.txt
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kali/kali-2018.4.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kali/kali-2018.4.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kali/kali-2019.2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kali/kali-2019.2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kali/kali-2019.2.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.256563 container-inspector-32.0.0/tests/data/distro/os-release/kaos/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kaos/kaos.txt
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kaos/kaos.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kaos/kaos.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.256563 container-inspector-32.0.0/tests/data/distro/os-release/kdeneon/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.256563 container-inspector-32.0.0/tests/data/distro/os-release/korora/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/korora/korora-24.txt
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/korora/korora-24.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/korora/korora-24.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/korora/korora-26.txt
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/korora/korora-26.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/korora/korora-26.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.256563 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-17.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-17.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-18.2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-18.2.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-19.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-19.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.260563 container-inspector-32.0.0/tests/data/distro/os-release/lirios/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/lirios/lirios.txt
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/lirios/lirios.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/lirios/lirios.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.260563 container-inspector-32.0.0/tests/data/distro/os-release/mageia/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/mageia/mageia-6.txt
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/mageia/mageia-6.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/mageia/mageia-6.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/mageia/mageia-7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/mageia/mageia-7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/mageia/mageia-7.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.260563 container-inspector-32.0.0/tests/data/distro/os-release/manjaro/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/manjaro/manjaro-new.txt
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/manjaro/manjaro-new.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/manjaro/manjaro-new.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/manjaro/manjaro.txt
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/manjaro/manjaro.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/manjaro/manjaro.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.260563 container-inspector-32.0.0/tests/data/distro/os-release/mx-linux/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/mx-linux/mx-linux.txt
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/mx-linux/mx-linux.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/mx-linux/mx-linux.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.260563 container-inspector-32.0.0/tests/data/distro/os-release/nexus/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/nexus/nexus-7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/nexus/nexus-7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/nexus/nexus-7.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.260563 container-inspector-32.0.0/tests/data/distro/os-release/nixos/
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/nixos/nixos.txt
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/nixos/nixos.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/nixos/nixos.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.264563 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-13.2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-13.2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-13.2.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-2015.txt
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-2015.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-2015.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.264563 container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-7.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-8.txt
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-8.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-8.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/oraclelinux-7.6.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/oraclelinux-7.6.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.264563 container-inspector-32.0.0/tests/data/distro/os-release/peppermintos/
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/peppermintos/peppermintos-7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/peppermintos/peppermintos-7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/peppermintos/peppermintos-7.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.264563 container-inspector-32.0.0/tests/data/distro/os-release/photon/
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/photon/photon-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/photon/photon-4.0.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/photon/photon-4.0.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.264563 container-inspector-32.0.0/tests/data/distro/os-release/pop-os/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/pop-os/pop-os-17.04.txt
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/pop-os/pop-os-17.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/pop-os/pop-os-17.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/pop-os/pop-os-20.04.txt
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/pop-os/pop-os-20.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/pop-os/pop-os-20.04.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.264563 container-inspector-32.0.0/tests/data/distro/os-release/rancheros/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/rancheros/rancheros-1.4.txt
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/rancheros/rancheros-1.4.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/rancheros/rancheros-1.4.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.264563 container-inspector-32.0.0/tests/data/distro/os-release/raspbian/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/raspbian/raspbian-10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/raspbian/raspbian-10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/raspbian/raspbian-10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/raspbian/raspbian-8.txt
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/raspbian/raspbian-8.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/raspbian/raspbian-8.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.268563 container-inspector-32.0.0/tests/data/distro/os-release/redhat/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_2.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_3.txt
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_3.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_3.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_4.txt
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_4.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_4.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_5.txt
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_5.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_5.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_6.txt
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_6.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_6.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_7.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_0.txt
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_0.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_0.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_1.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.268563 container-inspector-32.0.0/tests/data/distro/os-release/redhat-ubi/
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.268563 container-inspector-32.0.0/tests/data/distro/os-release/rocky/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/rocky/rocky-8.4.txt
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/rocky/rocky-8.4.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/rocky/rocky-8.4.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.272563 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.1.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.272563 container-inspector-32.0.0/tests/data/distro/os-release/sharklinux/
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.272563 container-inspector-32.0.0/tests/data/distro/os-release/slackware/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/slackware/slackware-14.1
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/slackware/slackware-14.1-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/slackware/slackware-14.1-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/slackware/slackware-14.2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/slackware/slackware-14.2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/slackware/slackware-14.2.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.272563 container-inspector-32.0.0/tests/data/distro/os-release/sled/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sled/sled-12.3.txt
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sled/sled-12.3.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sled/sled-12.3.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sled/sled-15.txt
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sled/sled-15.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sled/sled-15.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.276564 container-inspector-32.0.0/tests/data/distro/os-release/sles/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles11_4.txt
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles11_4.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles11_4.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12.txt
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_1.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_2.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_3.txt
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_3.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_3.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_4.txt
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_4.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_4.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_5.txt
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_5.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles12_5.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles15_0.txt
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles15_0.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles15_0.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles15_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles15_1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles15_1.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_0_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_0_1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_0_1.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_2.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_2.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_3.txt
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_3.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_3.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.276564 container-inspector-32.0.0/tests/data/distro/os-release/solus/
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/solus/solus.txt
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/solus/solus.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/solus/solus.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.284564 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/kylin-16.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/kylin-16.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-12.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-12.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-12.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-12.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-12.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04.5.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04.5.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.04.5.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.04.5.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.04.5.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.04.5.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-artful.txt
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-cosmic.txt
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-disco.txt
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-eoan.txt
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-focal.txt
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-groovy.txt
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-hirsute.txt
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-impish.txt
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-quantal.txt
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-raring.txt
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-saucy.txt
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-utopic.txt
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-vivid.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-wily.txt
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-yakkety.txt
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-zesty.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.284564 container-inspector-32.0.0/tests/data/distro/os-release/xbian/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/xbian/xbian.txt
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/xbian/xbian.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/xbian/xbian.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.284564 container-inspector-32.0.0/tests/data/distro/os-release/xcp/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/xcp/xcp-7.5.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/xcp/xcp-7.5.0.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/xcp/xcp-7.5.0.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.284564 container-inspector-32.0.0/tests/data/distro/os-release/xenserver/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/xenserver/xenserver-7.6.txt
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/xenserver/xenserver-7.6.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/xenserver/xenserver-7.6.txt-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.288564 container-inspector-32.0.0/tests/data/distro/os-release/zorinos/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/zorinos/zorinos-12.txt
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/zorinos/zorinos-12.txt-distro-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release/zorinos/zorinos-12.txt-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release-chef.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release-nate.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/os-release-zoo.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)    18944 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/distro/windows-container-rootfs.tar
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.288564 container-inspector-32.0.0/tests/data/image/
--rw-r--r--   0 runner    (1001) docker     (121)    34304 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image/mini-image_from_scratch-2.0.tar
--rw-r--r--   0 runner    (1001) docker     (121)     5778 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image/mini-image_from_scratch-2.0.tar-relative-expected.json
--rw-r--r--   0 runner    (1001) docker     (121)    35328 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image/she-image_from_scratch-1.0.tar
--rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image/windows-mini-image.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image/windows-mini-image.tar.gz.expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.288564 container-inspector-32.0.0/tests/data/image_templates/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image_templates/Dockerfile.from_tar
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image_templates/Dockerfile.scratch
--rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image_templates/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.288564 container-inspector-32.0.0/tests/data/image_templates/additions/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image_templates/additions/bar
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.288564 container-inspector-32.0.0/tests/data/image_templates/additions/baz/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image_templates/additions/baz/this
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image_templates/additions/foo
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image_templates/hello
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/image_templates/layer.tar
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.288564 container-inspector-32.0.0/tests/data/repos/
--rw-r--r--   0 runner    (1001) docker     (121)    12800 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/hello-world.tar
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/hello-world.tar.flatten.expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/hello-world.tar.registry.expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     6773 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/images.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)    24636 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/images.tar.gz.expected.json
--rw-r--r--   0 runner    (1001) docker     (121)   129536 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/imagesv11.tar
--rw-r--r--   0 runner    (1001) docker     (121)     6672 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/imagesv11.tar.expected.json
--rw-r--r--   0 runner    (1001) docker     (121)    10861 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/imagesv11.tar.registry.expected.json
--rw-r--r--   0 runner    (1001) docker     (121)   139776 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/imagesv11_with_tar_at_root.tar
--rw-r--r--   0 runner    (1001) docker     (121)    10307 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/imagesv11_with_tar_at_root.tar.expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     6543 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/repos/imagesv11_with_tar_at_root.tar.registry.expected.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.288564 container-inspector-32.0.0/tests/data/rootfs/
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/rootfs/find_root.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)    12800 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/rootfs/hello-world.tar
--rw-r--r--   0 runner    (1001) docker     (121)   129536 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/rootfs/imagesv11.tar
--rw-r--r--   0 runner    (1001) docker     (121)    35328 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/rootfs/she-image_from_scratch-1.0.tar
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.288564 container-inspector-32.0.0/tests/data/tar/
--rw-r--r--   0 runner    (1001) docker     (121)    10240 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/tar/absolute_path.tar
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/tar/colon.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)    10240 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/tar/tar_relative.tar
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.292564 container-inspector-32.0.0/tests/data/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    11776 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links.tar
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links.tar.expected-events-skipping.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links.tar.expected-events.json
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links.tar.expected-skipping.json
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links.tar.expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     9728 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links_missing_targets.tar
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links_missing_targets.tar.expected-broken.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links_missing_targets.tar.expected-events-broken.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links_missing_targets.tar.expected-events.json
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/data/utils/layer_with_links_missing_targets.tar.expected.json
--rw-r--r--   0 runner    (1001) docker     (121)     3404 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/test_distro.py
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/test_dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     6693 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     8357 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/test_rootfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/test_skeleton_codestyle.py
--rw-r--r--   0 runner    (1001) docker     (121)     9303 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-07-30 20:57:54.000000 container-inspector-32.0.0/tests/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 20:58:05.292564 container-inspector-32.0.0/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-30 20:57:54.000000 container-inspector-32.0.0/thirdparty/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.536929 container-inspector-32.0.1/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-07-31 12:20:28.000000 container-inspector-32.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.440927 container-inspector-32.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.444927 container-inspector-32.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2022-07-31 12:20:28.000000 container-inspector-32.0.1/.github/workflows/docs-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-07-31 12:20:28.000000 container-inspector-32.0.1/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-07-31 12:20:28.000000 container-inspector-32.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-31 12:20:28.000000 container-inspector-32.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-07-31 12:20:28.000000 container-inspector-32.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5059 2022-07-31 12:20:28.000000 container-inspector-32.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-07-31 12:20:28.000000 container-inspector-32.0.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-07-31 12:20:28.000000 container-inspector-32.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-07-31 12:20:28.000000 container-inspector-32.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-07-31 12:20:47.536929 container-inspector-32.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-07-31 12:20:28.000000 container-inspector-32.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-31 12:20:28.000000 container-inspector-32.0.1/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-07-31 12:20:28.000000 container-inspector-32.0.1/azure-pipelines.yml
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6310 2022-07-31 12:20:28.000000 container-inspector-32.0.1/configure
+-rw-r--r--   0 runner    (1001) docker     (121)     6930 2022-07-31 12:20:28.000000 container-inspector-32.0.1/configure.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-07-31 12:20:28.000000 container-inspector-32.0.1/container-inspector.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.444927 container-inspector-32.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-07-31 12:20:28.000000 container-inspector-32.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2022-07-31 12:20:28.000000 container-inspector-32.0.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.444927 container-inspector-32.0.1/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-07-31 12:20:28.000000 container-inspector-32.0.1/docs/scripts/doc8_style_check.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-07-31 12:20:28.000000 container-inspector-32.0.1/docs/scripts/sphinx_build_link_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.444927 container-inspector-32.0.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.448927 container-inspector-32.0.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     8022 2022-07-31 12:20:28.000000 container-inspector-32.0.1/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-07-31 12:20:28.000000 container-inspector-32.0.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.448927 container-inspector-32.0.1/docs/source/contribute/
+-rw-r--r--   0 runner    (1001) docker     (121)    10245 2022-07-31 12:20:28.000000 container-inspector-32.0.1/docs/source/contribute/contrib_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-31 12:20:28.000000 container-inspector-32.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-07-31 12:20:28.000000 container-inspector-32.0.1/docs/source/skeleton-usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.440927 container-inspector-32.0.1/etc/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.448927 container-inspector-32.0.1/etc/ci/
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/ci/azure-container-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/ci/azure-container-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/ci/azure-posix.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/ci/azure-win.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/ci/install_sudo.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     8365 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/ci/macports-ci
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/ci/macports-ci.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/ci/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.448927 container-inspector-32.0.1/etc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3745 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/check_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8209 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/fetch_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9595 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/gen_pypi_simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/gen_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/gen_requirements_dev.py
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/utils_dejacode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/utils_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (121)    75964 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/utils_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2022-07-31 12:20:28.000000 container-inspector-32.0.1/etc/scripts/utils_thirdparty.py.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.440927 container-inspector-32.0.1/misc/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.448927 container-inspector-32.0.1/misc/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4694 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/docker/download-docker-image.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/docker/download-docker-image.sh.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)    10765 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/docker/download-docker-image.sh.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/docker/download-docker-image.sh.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.452927 container-inspector-32.0.1/misc/references/
+-rw-r--r--   0 runner    (1001) docker     (121)    22439 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/references/docker_image_spec_v1.1.md
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/references/docker_image_spec_v1.1.md.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)    24825 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/references/docker_image_spec_v1.2.md
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/references/docker_image_spec_v1.2.md.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)    20527 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/references/docker_image_spec_v1.md
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-07-31 12:20:28.000000 container-inspector-32.0.1/misc/references/docker_image_spec_v1.md.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-07-31 12:20:28.000000 container-inspector-32.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-07-31 12:20:28.000000 container-inspector-32.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-07-31 12:20:28.000000 container-inspector-32.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-07-31 12:20:47.540929 container-inspector-32.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-07-31 12:20:28.000000 container-inspector-32.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.440927 container-inspector-32.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.452927 container-inspector-32.0.1/src/container_inspector/
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-07-31 12:20:28.000000 container-inspector-32.0.1/src/container_inspector/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5169 2022-07-31 12:20:28.000000 container-inspector-32.0.1/src/container_inspector/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    23513 2022-07-31 12:20:28.000000 container-inspector-32.0.1/src/container_inspector/distro.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8834 2022-07-31 12:20:28.000000 container-inspector-32.0.1/src/container_inspector/dockerfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    39940 2022-07-31 12:20:28.000000 container-inspector-32.0.1/src/container_inspector/image.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10468 2022-07-31 12:20:28.000000 container-inspector-32.0.1/src/container_inspector/rootfs.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6652 2022-07-31 12:20:28.000000 container-inspector-32.0.1/src/container_inspector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.452927 container-inspector-32.0.1/src/container_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-07-31 12:20:47.000000 container-inspector-32.0.1/src/container_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    44037 2022-07-31 12:20:47.000000 container-inspector-32.0.1/src/container_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-31 12:20:47.000000 container-inspector-32.0.1/src/container_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-07-31 12:20:47.000000 container-inspector-32.0.1/src/container_inspector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-31 12:20:47.000000 container-inspector-32.0.1/src/container_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-07-31 12:20:47.000000 container-inspector-32.0.1/src/container_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-31 12:20:47.000000 container-inspector-32.0.1/src/container_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.452927 container-inspector-32.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.444927 container-inspector-32.0.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.452927 container-inspector-32.0.1/tests/data/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)    12800 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/cli/hello-world.tar
+-rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/cli/hello-world.tar-inventory-from-dir-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/cli/hello-world.tar-inventory-from-tarball-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)    35328 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/cli/she-image_from_scratch-1.0.tar
+-rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/cli/she-image_from_scratch-1.0.tar-inventory-from-tarball-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.452927 container-inspector-32.0.1/tests/data/distro/
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/README-chef.md
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/README-nate.md
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/README-zoo.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7048 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/cc0-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.444927 container-inspector-32.0.1/tests/data/distro/os-release/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.456927 container-inspector-32.0.1/tests/data/distro/os-release/alpine/
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/alpine/alpine-3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/alpine/alpine-3.8.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/alpine/alpine-3.8.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.456927 container-inspector-32.0.1/tests/data/distro/os-release/amazon/
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/amazon/amazon-2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/amazon/amazon-2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/amazon/amazon-2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/amazon/amazon-2018.03.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/amazon/amazon-2018.03.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/amazon/amazon-2018.03.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/amazon/amzon-2016.09.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/amazon/amzon-2016.09.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/amazon/amzon-2016.09.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.456927 container-inspector-32.0.1/tests/data/distro/os-release/antergos/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/antergos/antergos.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/antergos/antergos.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/antergos/antergos.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.456927 container-inspector-32.0.1/tests/data/distro/os-release/arch/
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-arm-new.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-arm-new.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-arm-new.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-arm.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-arm.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-arm.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-mini.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-mini.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-mini.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/arch/arch.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.456927 container-inspector-32.0.1/tests/data/distro/os-release/artix/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/artix/artix.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/artix/artix.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/artix/artix.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.456927 container-inspector-32.0.1/tests/data/distro/os-release/centos/
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/centos/centos-7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/centos/centos-7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/centos/centos-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.456927 container-inspector-32.0.1/tests/data/distro/os-release/clearlinux/
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/clearlinux/clearlinux-1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/clearlinux/clearlinux-1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/clearlinux/clearlinux-1.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.456927 container-inspector-32.0.1/tests/data/distro/os-release/clearos/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/clearos/clearos-7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/clearos/clearos-7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/clearos/clearos-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.460927 container-inspector-32.0.1/tests/data/distro/os-release/coreos/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.460927 container-inspector-32.0.1/tests/data/distro/os-release/cumulus/
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/cumulus/cumulus-3.7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/cumulus/cumulus-3.7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/cumulus/cumulus-3.7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.460927 container-inspector-32.0.1/tests/data/distro/os-release/debian/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-11.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-11.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-11.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-7.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-8.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-8.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-9.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-9.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-sid.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-sid.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.460927 container-inspector-32.0.1/tests/data/distro/os-release/distroless/
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian11.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian11.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian11.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian9.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian9.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian9.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.464927 container-inspector-32.0.1/tests/data/distro/os-release/elementary/
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-0.4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-0.4.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-0.4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-5.1.7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-5.1.7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-5.1.7.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-5.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-5.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-5.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.464927 container-inspector-32.0.1/tests/data/distro/os-release/endless/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/endless/endless-3.2.2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/endless/endless-3.2.2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/endless/endless-3.2.2.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.484928 container-inspector-32.0.1/tests/data/distro/os-release/fedora/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-17.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-17.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-17.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-18.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-18.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-18.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-20.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-20.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-20.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-21.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-21.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-21.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-modular.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-modular.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-modular.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      879 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      894 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-container.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-container.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      828 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      946 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-container.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-container.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      811 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-container.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-container.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-container.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-container.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-container.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-container.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-kde.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-kde.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      882 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-kde.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      897 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-soas.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-soas.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-soas.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-xfce.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-xfce.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      865 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-xfce.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-container.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-container.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-kde.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-kde.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-kde.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-server.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-server.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-soas.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-soas.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-soas.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-workstation.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-xfce.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-xfce.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      864 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-xfce.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-35.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-35.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-35.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-36-pre.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-36-pre.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-36-pre.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.484928 container-inspector-32.0.1/tests/data/distro/os-release/galliumos/
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/galliumos/galliumos-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/galliumos/galliumos-2.1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/galliumos/galliumos-2.1.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.484928 container-inspector-32.0.1/tests/data/distro/os-release/gentoo/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/gentoo/gentoo-new.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/gentoo/gentoo-new.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/gentoo/gentoo-new.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/gentoo/gentoo.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/gentoo/gentoo.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/gentoo/gentoo.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.488928 container-inspector-32.0.1/tests/data/distro/os-release/ios/
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ios/ios-xr-6.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      598 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ios/ios-xr-6.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ios/ios-xr-6.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.488928 container-inspector-32.0.1/tests/data/distro/os-release/kali/
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kali/kali-2018.4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kali/kali-2018.4.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kali/kali-2018.4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kali/kali-2019.2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kali/kali-2019.2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kali/kali-2019.2.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.488928 container-inspector-32.0.1/tests/data/distro/os-release/kaos/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kaos/kaos.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kaos/kaos.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kaos/kaos.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.488928 container-inspector-32.0.1/tests/data/distro/os-release/kdeneon/
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.488928 container-inspector-32.0.1/tests/data/distro/os-release/korora/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/korora/korora-24.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/korora/korora-24.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/korora/korora-24.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/korora/korora-26.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/korora/korora-26.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/korora/korora-26.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.488928 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-17.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-17.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-18.2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-18.2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-19.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-19.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.488928 container-inspector-32.0.1/tests/data/distro/os-release/lirios/
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/lirios/lirios.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/lirios/lirios.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/lirios/lirios.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.492928 container-inspector-32.0.1/tests/data/distro/os-release/mageia/
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/mageia/mageia-6.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/mageia/mageia-6.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/mageia/mageia-6.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/mageia/mageia-7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/mageia/mageia-7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/mageia/mageia-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.492928 container-inspector-32.0.1/tests/data/distro/os-release/manjaro/
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/manjaro/manjaro-new.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/manjaro/manjaro-new.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/manjaro/manjaro-new.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/manjaro/manjaro.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/manjaro/manjaro.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/manjaro/manjaro.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.492928 container-inspector-32.0.1/tests/data/distro/os-release/mx-linux/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/mx-linux/mx-linux.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/mx-linux/mx-linux.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/mx-linux/mx-linux.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.492928 container-inspector-32.0.1/tests/data/distro/os-release/nexus/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/nexus/nexus-7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/nexus/nexus-7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/nexus/nexus-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.492928 container-inspector-32.0.1/tests/data/distro/os-release/nixos/
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/nixos/nixos.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/nixos/nixos.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/nixos/nixos.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.496928 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-13.2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-13.2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-13.2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-2015.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-2015.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-2015.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      598 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.496928 container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-7.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-8.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-8.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-8.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/oraclelinux-7.6.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/oraclelinux-7.6.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.496928 container-inspector-32.0.1/tests/data/distro/os-release/peppermintos/
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/peppermintos/peppermintos-7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/peppermintos/peppermintos-7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/peppermintos/peppermintos-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.496928 container-inspector-32.0.1/tests/data/distro/os-release/photon/
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/photon/photon-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/photon/photon-4.0.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/photon/photon-4.0.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.496928 container-inspector-32.0.1/tests/data/distro/os-release/pop-os/
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/pop-os/pop-os-17.04.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/pop-os/pop-os-17.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/pop-os/pop-os-17.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/pop-os/pop-os-20.04.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/pop-os/pop-os-20.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/pop-os/pop-os-20.04.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.500928 container-inspector-32.0.1/tests/data/distro/os-release/rancheros/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/rancheros/rancheros-1.4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/rancheros/rancheros-1.4.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/rancheros/rancheros-1.4.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.500928 container-inspector-32.0.1/tests/data/distro/os-release/raspbian/
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/raspbian/raspbian-10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/raspbian/raspbian-10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/raspbian/raspbian-10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/raspbian/raspbian-8.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/raspbian/raspbian-8.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/raspbian/raspbian-8.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.504928 container-inspector-32.0.1/tests/data/distro/os-release/redhat/
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_3.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_4.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_5.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_5.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_6.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_6.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_6.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_7.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_0.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_1.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.504928 container-inspector-32.0.1/tests/data/distro/os-release/redhat-ubi/
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      906 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.504928 container-inspector-32.0.1/tests/data/distro/os-release/rocky/
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/rocky/rocky-8.4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/rocky/rocky-8.4.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/rocky/rocky-8.4.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.508928 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.508928 container-inspector-32.0.1/tests/data/distro/os-release/sharklinux/
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.508928 container-inspector-32.0.1/tests/data/distro/os-release/slackware/
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/slackware/slackware-14.1
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/slackware/slackware-14.1-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/slackware/slackware-14.1-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/slackware/slackware-14.2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/slackware/slackware-14.2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/slackware/slackware-14.2.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.508928 container-inspector-32.0.1/tests/data/distro/os-release/sled/
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sled/sled-12.3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sled/sled-12.3.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sled/sled-12.3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sled/sled-15.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sled/sled-15.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sled/sled-15.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.512929 container-inspector-32.0.1/tests/data/distro/os-release/sles/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles11_4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles11_4.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles11_4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_3.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_4.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_5.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_5.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles12_5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles15_0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles15_0.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles15_0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles15_1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      503 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles15_1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles15_1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_0_1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_0_1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_0_1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_2.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_3.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_3.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.512929 container-inspector-32.0.1/tests/data/distro/os-release/solus/
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/solus/solus.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/solus/solus.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/solus/solus.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.528929 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/kylin-16.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/kylin-16.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-12.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-12.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-12.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-12.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-12.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.04-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.04-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.04.5.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.04.5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.04.5.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.04.5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.04.5.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.04.5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      649 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-artful.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-cosmic.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-disco.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-eoan.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-focal.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-groovy.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-hirsute.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-impish.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-quantal.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-raring.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-saucy.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-utopic.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-vivid.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-wily.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-yakkety.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-zesty.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.532929 container-inspector-32.0.1/tests/data/distro/os-release/xbian/
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/xbian/xbian.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/xbian/xbian.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/xbian/xbian.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.532929 container-inspector-32.0.1/tests/data/distro/os-release/xcp/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/xcp/xcp-7.5.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/xcp/xcp-7.5.0.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/xcp/xcp-7.5.0.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.532929 container-inspector-32.0.1/tests/data/distro/os-release/xenserver/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/xenserver/xenserver-7.6.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/xenserver/xenserver-7.6.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/xenserver/xenserver-7.6.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.532929 container-inspector-32.0.1/tests/data/distro/os-release/zorinos/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/zorinos/zorinos-12.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/zorinos/zorinos-12.txt-distro-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release/zorinos/zorinos-12.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release-chef.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release-nate.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/os-release-zoo.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (121)    18944 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/distro/windows-container-rootfs.tar
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.532929 container-inspector-32.0.1/tests/data/image/
+-rw-r--r--   0 runner    (1001) docker     (121)    34304 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image/mini-image_from_scratch-2.0.tar
+-rw-r--r--   0 runner    (1001) docker     (121)     5778 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image/mini-image_from_scratch-2.0.tar-relative-expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)    35328 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image/she-image_from_scratch-1.0.tar
+-rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image/windows-mini-image.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image/windows-mini-image.tar.gz.expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.532929 container-inspector-32.0.1/tests/data/image_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image_templates/Dockerfile.from_tar
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image_templates/Dockerfile.scratch
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image_templates/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.532929 container-inspector-32.0.1/tests/data/image_templates/additions/
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image_templates/additions/bar
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.532929 container-inspector-32.0.1/tests/data/image_templates/additions/baz/
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image_templates/additions/baz/this
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image_templates/additions/foo
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image_templates/hello
+-rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/image_templates/layer.tar
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.536929 container-inspector-32.0.1/tests/data/repos/
+-rw-r--r--   0 runner    (1001) docker     (121)    12800 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/hello-world.tar
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/hello-world.tar.flatten.expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/hello-world.tar.registry.expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     6773 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/images.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    24636 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/images.tar.gz.expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)   129536 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/imagesv11.tar
+-rw-r--r--   0 runner    (1001) docker     (121)     6672 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/imagesv11.tar.expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)    10861 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/imagesv11.tar.registry.expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)   139776 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/imagesv11_with_tar_at_root.tar
+-rw-r--r--   0 runner    (1001) docker     (121)    10307 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/imagesv11_with_tar_at_root.tar.expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     6543 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/repos/imagesv11_with_tar_at_root.tar.registry.expected.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.536929 container-inspector-32.0.1/tests/data/rootfs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/rootfs/find_root.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    12800 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/rootfs/hello-world.tar
+-rw-r--r--   0 runner    (1001) docker     (121)   129536 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/rootfs/imagesv11.tar
+-rw-r--r--   0 runner    (1001) docker     (121)    35328 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/rootfs/she-image_from_scratch-1.0.tar
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.536929 container-inspector-32.0.1/tests/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)    10240 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/absolute_path.tar
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/colon.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (121)    11776 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links.tar
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links.tar.expected-events-skipping.json
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links.tar.expected-events.json
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links.tar.expected-skipping.json
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links.tar.expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     9728 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links_missing_targets.tar
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links_missing_targets.tar.expected-broken.json
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links_missing_targets.tar.expected-events-broken.json
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links_missing_targets.tar.expected-events.json
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/layer_with_links_missing_targets.tar.expected.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/tar_relative-with-whiteouts.tar
+-rw-r--r--   0 runner    (1001) docker     (121)    10240 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/data/utils/tar_relative.tar
+-rw-r--r--   0 runner    (1001) docker     (121)     3404 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/test_distro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/test_dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6693 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8357 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/test_rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/test_skeleton_codestyle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10672 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-07-31 12:20:28.000000 container-inspector-32.0.1/tests/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 12:20:47.536929 container-inspector-32.0.1/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-31 12:20:28.000000 container-inspector-32.0.1/thirdparty/README.rst
```

### Comparing `container-inspector-32.0.0/.github/workflows/docs-ci.yml` & `container-inspector-32.0.1/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/.github/workflows/pypi-release.yml` & `container-inspector-32.0.1/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/.gitignore` & `container-inspector-32.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/CHANGELOG.rst` & `container-inspector-32.0.1/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+v32.0.1
+--------
+
+This is a minor release with bug fixes.
+
+- We now correctly process the opaque whiteouts seen in container image layers
+  tarballs.
+
+Thank you to AJ Arena @sig-aarena
+
+
 v32.0.0 
 --------
 
 This is a minor release with bug fixes and an output change.
 
 - We no longer support Python 3.6, only 3.7 and up.
```

### Comparing `container-inspector-32.0.0/CODE_OF_CONDUCT.rst` & `container-inspector-32.0.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/NOTICE` & `container-inspector-32.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/PKG-INFO` & `container-inspector-32.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-inspector
-Version: 32.0.0
+Version: 32.0.1
 Summary: Docker, containers, rootfs and virtual machine related software composition analysis (SCA) utilities.
 Home-page: https://github.com/nexB/container-inspector
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities,docker,container,oci,qcow,os-release,virtual-machine,vm,rootfs,scancode
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `container-inspector-32.0.0/README.rst` & `container-inspector-32.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/apache-2.0.LICENSE` & `container-inspector-32.0.1/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/azure-pipelines.yml` & `container-inspector-32.0.1/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/configure` & `container-inspector-32.0.1/configure`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/configure.bat` & `container-inspector-32.0.1/configure.bat`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/docs/Makefile` & `container-inspector-32.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/docs/make.bat` & `container-inspector-32.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/docs/source/_static/theme_overrides.css` & `container-inspector-32.0.1/docs/source/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/docs/source/conf.py` & `container-inspector-32.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/docs/source/contribute/contrib_doc.rst` & `container-inspector-32.0.1/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/docs/source/skeleton-usage.rst` & `container-inspector-32.0.1/docs/source/skeleton-usage.rst`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/ci/azure-container-deb.yml` & `container-inspector-32.0.1/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/ci/azure-container-rpm.yml` & `container-inspector-32.0.1/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/ci/azure-posix.yml` & `container-inspector-32.0.1/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/ci/azure-win.yml` & `container-inspector-32.0.1/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/ci/macports-ci` & `container-inspector-32.0.1/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/ci/macports-ci.ABOUT` & `container-inspector-32.0.1/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/ci/mit.LICENSE` & `container-inspector-32.0.1/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/README.rst` & `container-inspector-32.0.1/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/check_thirdparty.py` & `container-inspector-32.0.1/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/fetch_thirdparty.py` & `container-inspector-32.0.1/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/gen_pypi_simple.py` & `container-inspector-32.0.1/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `container-inspector-32.0.1/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/gen_requirements.py` & `container-inspector-32.0.1/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/gen_requirements_dev.py` & `container-inspector-32.0.1/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `container-inspector-32.0.1/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/test_utils_pypi_supported_tags.py` & `container-inspector-32.0.1/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `container-inspector-32.0.1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/utils_dejacode.py` & `container-inspector-32.0.1/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/utils_pip_compatibility_tags.py` & `container-inspector-32.0.1/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/utils_pypi_supported_tags.py` & `container-inspector-32.0.1/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `container-inspector-32.0.1/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/utils_requirements.py` & `container-inspector-32.0.1/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/utils_thirdparty.py` & `container-inspector-32.0.1/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/etc/scripts/utils_thirdparty.py.ABOUT` & `container-inspector-32.0.1/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/misc/docker/download-docker-image.sh` & `container-inspector-32.0.1/misc/docker/download-docker-image.sh`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/misc/docker/download-docker-image.sh.LICENSE` & `container-inspector-32.0.1/misc/docker/download-docker-image.sh.LICENSE`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/misc/docker/download-docker-image.sh.NOTICE` & `container-inspector-32.0.1/misc/docker/download-docker-image.sh.NOTICE`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/misc/references/docker_image_spec_v1.1.md` & `container-inspector-32.0.1/misc/references/docker_image_spec_v1.1.md`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/misc/references/docker_image_spec_v1.2.md` & `container-inspector-32.0.1/misc/references/docker_image_spec_v1.2.md`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/misc/references/docker_image_spec_v1.md` & `container-inspector-32.0.1/misc/references/docker_image_spec_v1.md`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/pyproject.toml` & `container-inspector-32.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/requirements-dev.txt` & `container-inspector-32.0.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/requirements.txt` & `container-inspector-32.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/setup.cfg` & `container-inspector-32.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/src/container_inspector/__init__.py` & `container-inspector-32.0.1/src/container_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/src/container_inspector/cli.py` & `container-inspector-32.0.1/src/container_inspector/cli.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/src/container_inspector/distro.py` & `container-inspector-32.0.1/src/container_inspector/distro.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/src/container_inspector/dockerfile.py` & `container-inspector-32.0.1/src/container_inspector/dockerfile.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/src/container_inspector/image.py` & `container-inspector-32.0.1/src/container_inspector/image.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/src/container_inspector/utils.py` & `container-inspector-32.0.1/src/container_inspector/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -99,14 +99,31 @@
     # even message
     message: str
 
     def to_string(self):
         return f"{self.type}: {self.message}"
 
 
+def is_relative_path(path):
+    """
+    Return True if ``path`` is a relative path.
+    >>> is_relative_path('.wh..wh..opq')
+    False
+    >>> is_relative_path('.wh/../wh..opq')
+    True
+    >>> is_relative_path('..foor')
+    False
+    >>> is_relative_path('../foor')
+    True
+    >>> is_relative_path('.//.foor//..')
+    True
+    """
+    return any(name == '..' for name in path.split('/'))
+
+
 def extract_tar(location, target_dir, as_events=False, skip_symlinks=True, trace=TRACE):
     """
     Extract a tar archive at ``location`` in the ``target_dir`` directory.
     Return a list of ExtractEvent is ``as_events`` is True, or a list of message
     strings otherwise. This list can be empty. Skip symlinks and hardlinks if
     skip_symlinks is True.
 
@@ -129,15 +146,15 @@
             if tarinfo.isdev() or tarinfo.ischr() or tarinfo.isblk() or tarinfo.isfifo() or tarinfo.sparse:
                 msg = f'skipping unsupported {tarinfo.name} file type: block, chr, dev or sparse file'
                 events.append(ExtractEvent(type=ExtractEvent.INFO, source=tarinfo.name, message=msg))
                 if trace:
                     logger.debug(f'extract_tar: {msg}')
                 continue
 
-            if '..' in tarinfo.name:
+            if is_relative_path(tarinfo.name):
                 msg = f'{location}: skipping unsupported {tarinfo.name} with relative path.'
                 events.append(ExtractEvent(type=ExtractEvent.WARNING, source=tarinfo.name, message=msg))
                 if trace:
                     logger.debug(f'extract_tar: {msg}')
                 continue
 
             if skip_symlinks and (tarinfo.islnk() or tarinfo.issym()):
```

### Comparing `container-inspector-32.0.0/src/container_inspector.egg-info/PKG-INFO` & `container-inspector-32.0.1/src/container_inspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-inspector
-Version: 32.0.0
+Version: 32.0.1
 Summary: Docker, containers, rootfs and virtual machine related software composition analysis (SCA) utilities.
 Home-page: https://github.com/nexB/container-inspector
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities,docker,container,oci,qcow,os-release,virtual-machine,vm,rootfs,scancode
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `container-inspector-32.0.0/src/container_inspector.egg-info/SOURCES.txt` & `container-inspector-32.0.1/src/container_inspector.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -715,21 +715,22 @@
 tests/data/repos/imagesv11_with_tar_at_root.tar
 tests/data/repos/imagesv11_with_tar_at_root.tar.expected.json
 tests/data/repos/imagesv11_with_tar_at_root.tar.registry.expected.json
 tests/data/rootfs/find_root.tar.gz
 tests/data/rootfs/hello-world.tar
 tests/data/rootfs/imagesv11.tar
 tests/data/rootfs/she-image_from_scratch-1.0.tar
-tests/data/tar/absolute_path.tar
-tests/data/tar/colon.tar.xz
-tests/data/tar/tar_relative.tar
+tests/data/utils/absolute_path.tar
+tests/data/utils/colon.tar.xz
 tests/data/utils/layer_with_links.tar
 tests/data/utils/layer_with_links.tar.expected-events-skipping.json
 tests/data/utils/layer_with_links.tar.expected-events.json
 tests/data/utils/layer_with_links.tar.expected-skipping.json
 tests/data/utils/layer_with_links.tar.expected.json
 tests/data/utils/layer_with_links_missing_targets.tar
 tests/data/utils/layer_with_links_missing_targets.tar.expected-broken.json
 tests/data/utils/layer_with_links_missing_targets.tar.expected-events-broken.json
 tests/data/utils/layer_with_links_missing_targets.tar.expected-events.json
 tests/data/utils/layer_with_links_missing_targets.tar.expected.json
+tests/data/utils/tar_relative-with-whiteouts.tar
+tests/data/utils/tar_relative.tar
 thirdparty/README.rst
```

### Comparing `container-inspector-32.0.0/tests/data/cli/hello-world.tar` & `container-inspector-32.0.1/tests/data/cli/hello-world.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/cli/hello-world.tar-inventory-from-dir-expected.json` & `container-inspector-32.0.1/tests/data/cli/hello-world.tar-inventory-from-dir-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/cli/hello-world.tar-inventory-from-tarball-expected.json` & `container-inspector-32.0.1/tests/data/cli/hello-world.tar-inventory-from-tarball-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/cli/she-image_from_scratch-1.0.tar` & `container-inspector-32.0.1/tests/data/cli/she-image_from_scratch-1.0.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/cli/she-image_from_scratch-1.0.tar-inventory-from-tarball-expected.json` & `container-inspector-32.0.1/tests/data/cli/she-image_from_scratch-1.0.tar-inventory-from-tarball-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/README-chef.md` & `container-inspector-32.0.1/tests/data/distro/README-chef.md`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/README-zoo.md` & `container-inspector-32.0.1/tests/data/distro/README-zoo.md`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/apache-2.0.LICENSE` & `container-inspector-32.0.1/tests/data/distro/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/cc0-1.0.LICENSE` & `container-inspector-32.0.1/tests/data/distro/cc0-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/mit.LICENSE` & `container-inspector-32.0.1/tests/data/distro/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/alpine/alpine-3.8.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/alpine/alpine-3.8.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/amazon/amazon-2.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/amazon/amazon-2.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/amazon/amazon-2018.03.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/amazon/amazon-2018.03.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/amazon/amzon-2016.09.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/amazon/amzon-2016.09.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/antergos/antergos.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/antergos/antergos.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-arm-new.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-arm-new.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-arm.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-arm.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/arch/arch-mini.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/arch/arch-mini.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/arch/arch.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/arch/arch.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/artix/artix.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/artix/artix.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/centos/centos-7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/centos/centos-7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/clearlinux/clearlinux-1.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/clearlinux/clearlinux-1.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/clearos/clearos-7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/clearos/clearos-7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/cumulus/cumulus-3.7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/cumulus/cumulus-3.7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-11.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-11.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-8.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-8.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-9.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-9.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/debian/debian-sid.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/debian/debian-sid.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian11.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian11.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/distroless/distroless-debian9.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/distroless/distroless-debian9.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-0.4.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-0.4.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-5.1.7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-5.1.7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/elementary/elementary-5.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/elementary/elementary-5.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-17.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-17.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-18.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-18.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-20.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-20.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-21.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-21.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-22.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-22.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-23.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-23.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-24.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-24.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-25.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-25.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-modular.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-modular.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-modular.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-modular.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-26.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-26.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-server.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-server.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-27.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-27.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-server.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-server.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-28.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-28.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-container.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-container.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-container.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-container.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-container.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-container.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-server.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-server.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-29.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-29.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-container.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-container.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-container.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-container.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-container.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-container.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-server.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-server.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-30.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-30.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-container.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-container.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-container.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-container.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-container.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-container.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-server.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-server.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-31.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-31.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-container.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-container.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-container.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-container.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-container.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-container.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-server.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-server.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-32.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-32.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-container.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-container.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-container.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-container.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-container.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-container.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-kde.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-kde.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-kde.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-kde.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-kde.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-kde.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-server.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-server.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-soas.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-soas.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-soas.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-soas.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-soas.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-soas.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-xfce.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-xfce.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-xfce.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-xfce.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33-xfce.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33-xfce.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-33.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-33.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-container.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-container.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-container.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-container.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-container.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-container.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-kde.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-kde.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-kde.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-kde.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-kde.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-kde.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-server.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-server.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-server.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-server.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-server.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-server.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-soas.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-soas.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-soas.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-soas.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-soas.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-soas.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-workstation.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-workstation.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-workstation.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-workstation.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-workstation.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-workstation.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-xfce.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-xfce.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-xfce.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-xfce.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34-xfce.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34-xfce.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-34.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-34.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-35.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-35.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-35.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-35.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-35.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-35.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-36-pre.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-36-pre.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-36-pre.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-36-pre.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/fedora/fedora-36-pre.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/fedora/fedora-36-pre.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/galliumos/galliumos-2.1.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/galliumos/galliumos-2.1.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/gentoo/gentoo-new.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/gentoo/gentoo-new.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/gentoo/gentoo.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/gentoo/gentoo.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ios/ios-xr-6.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ios/ios-xr-6.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/kali/kali-2018.4.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/kali/kali-2018.4.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/kali/kali-2019.2.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/kali/kali-2019.2.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/korora/korora-24.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/korora/korora-24.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/korora/korora-26.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/korora/korora-26.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-17.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-17.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-18.2.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-18.2.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/linuxmint/linuxmint-19.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/linuxmint/linuxmint-19.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/mageia/mageia-6.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/mageia/mageia-6.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/mageia/mageia-7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/mageia/mageia-7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/manjaro/manjaro-new.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/manjaro/manjaro-new.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/manjaro/manjaro.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/manjaro/manjaro.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/mx-linux/mx-linux.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/mx-linux/mx-linux.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/nexus/nexus-7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/nexus/nexus-7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/nixos/nixos.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/nixos/nixos.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-13.2.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-13.2.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-2015.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-2015.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-7.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-7.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-8.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-8.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/ol-8.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/ol-8.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/oraclelinux-7.6.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/oraclelinux-7.6.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/oraclelinux/oraclelinux-7.6.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/oraclelinux/oraclelinux-7.6.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/peppermintos/peppermintos-7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/peppermintos/peppermintos-7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/photon/photon-4.0.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/photon/photon-4.0.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/pop-os/pop-os-17.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/pop-os/pop-os-17.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/pop-os/pop-os-20.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/pop-os/pop-os-20.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/rancheros/rancheros-1.4.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/rancheros/rancheros-1.4.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/raspbian/raspbian-10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/raspbian/raspbian-10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/raspbian/raspbian-8.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/raspbian/raspbian-8.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_2.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_2.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_2.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_2.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_3.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_3.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_3.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_3.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_4.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_4.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_4.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_4.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_4.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_4.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_5.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_5.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_5.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_5.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_5.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_5.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_6.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_6.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_6.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_6.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_6.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_6.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_7.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_7.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel7_7.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel7_7.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_0.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_0.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_0.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_0.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_1.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_1.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat/rhel8_1.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat/rhel8_1.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/rocky/rocky-8.4.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/rocky/rocky-8.4.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.1.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.1.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.1.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.1.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/slackware/slackware-14.1-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/slackware/slackware-14.1-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/slackware/slackware-14.2.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/slackware/slackware-14.2.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_0_1.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_0_1.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/sles/sles4sap12_2.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/sles/sles4sap12_2.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/solus/solus.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/solus/solus.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/kylin-16.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/kylin-16.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.04-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04.5.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.04.5.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.04.5.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.04.5.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.04.5.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.04.5.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/xbian/xbian.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/xbian/xbian.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/xcp/xcp-7.5.0.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/xcp/xcp-7.5.0.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/xenserver/xenserver-7.6.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/xenserver/xenserver-7.6.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release/zorinos/zorinos-12.txt-distro-expected.json` & `container-inspector-32.0.1/tests/data/distro/os-release/zorinos/zorinos-12.txt-distro-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/os-release-chef.ABOUT` & `container-inspector-32.0.1/tests/data/distro/os-release-chef.ABOUT`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/distro/windows-container-rootfs.tar` & `container-inspector-32.0.1/tests/data/distro/windows-container-rootfs.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/image/mini-image_from_scratch-2.0.tar` & `container-inspector-32.0.1/tests/data/image/mini-image_from_scratch-2.0.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/image/mini-image_from_scratch-2.0.tar-relative-expected.json` & `container-inspector-32.0.1/tests/data/image/mini-image_from_scratch-2.0.tar-relative-expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/image/she-image_from_scratch-1.0.tar` & `container-inspector-32.0.1/tests/data/image/she-image_from_scratch-1.0.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/image/windows-mini-image.tar.gz` & `container-inspector-32.0.1/tests/data/image/windows-mini-image.tar.gz`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/image/windows-mini-image.tar.gz.expected.json` & `container-inspector-32.0.1/tests/data/image/windows-mini-image.tar.gz.expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/image_templates/README.rst` & `container-inspector-32.0.1/tests/data/image_templates/README.rst`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/image_templates/layer.tar` & `container-inspector-32.0.1/tests/data/image_templates/layer.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/hello-world.tar` & `container-inspector-32.0.1/tests/data/repos/hello-world.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/hello-world.tar.flatten.expected.json` & `container-inspector-32.0.1/tests/data/repos/hello-world.tar.flatten.expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/hello-world.tar.registry.expected.json` & `container-inspector-32.0.1/tests/data/repos/hello-world.tar.registry.expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/images.tar.gz` & `container-inspector-32.0.1/tests/data/repos/images.tar.gz`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/images.tar.gz.expected.json` & `container-inspector-32.0.1/tests/data/repos/images.tar.gz.expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/imagesv11.tar` & `container-inspector-32.0.1/tests/data/repos/imagesv11.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/imagesv11.tar.expected.json` & `container-inspector-32.0.1/tests/data/repos/imagesv11.tar.expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/imagesv11.tar.registry.expected.json` & `container-inspector-32.0.1/tests/data/repos/imagesv11.tar.registry.expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/imagesv11_with_tar_at_root.tar` & `container-inspector-32.0.1/tests/data/repos/imagesv11_with_tar_at_root.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/imagesv11_with_tar_at_root.tar.expected.json` & `container-inspector-32.0.1/tests/data/repos/imagesv11_with_tar_at_root.tar.expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/repos/imagesv11_with_tar_at_root.tar.registry.expected.json` & `container-inspector-32.0.1/tests/data/repos/imagesv11_with_tar_at_root.tar.registry.expected.json`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/rootfs/find_root.tar.gz` & `container-inspector-32.0.1/tests/data/rootfs/find_root.tar.gz`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/rootfs/hello-world.tar` & `container-inspector-32.0.1/tests/data/rootfs/hello-world.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/rootfs/imagesv11.tar` & `container-inspector-32.0.1/tests/data/rootfs/imagesv11.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/rootfs/she-image_from_scratch-1.0.tar` & `container-inspector-32.0.1/tests/data/rootfs/she-image_from_scratch-1.0.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/tar/absolute_path.tar` & `container-inspector-32.0.1/tests/data/utils/absolute_path.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/tar/tar_relative.tar` & `container-inspector-32.0.1/tests/data/utils/tar_relative.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/utils/layer_with_links.tar` & `container-inspector-32.0.1/tests/data/utils/layer_with_links.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/data/utils/layer_with_links_missing_targets.tar` & `container-inspector-32.0.1/tests/data/utils/layer_with_links_missing_targets.tar`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/test_cli.py` & `container-inspector-32.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/test_distro.py` & `container-inspector-32.0.1/tests/test_distro.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/test_dockerfile.py` & `container-inspector-32.0.1/tests/test_dockerfile.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/test_image.py` & `container-inspector-32.0.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/test_rootfs.py` & `container-inspector-32.0.1/tests/test_rootfs.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/test_skeleton_codestyle.py` & `container-inspector-32.0.1/tests/test_skeleton_codestyle.py`

 * *Files identical despite different names*

### Comparing `container-inspector-32.0.0/tests/test_utils.py` & `container-inspector-32.0.1/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,91 +50,116 @@
         """
         events_results = []
         for e in events:
             ne = e._replace(
                 source=e.source.replace(extract_dir, ''),
                 message=e.message.replace(self.test_data_dir, ''),
             )
-            events_results.append(ne._asdict())
-
-        return events_results
+            events_results.append(ne)
+        events_results = sorted(events_results, key=lambda x: x.source)
+        return [dict(ne._asdict()) for ne in events_results]
 
     def clean_paths(self, extract_dir):
         return sorted([p.replace(extract_dir, '') for p in
             fileutils.resource_iter(
                 location=extract_dir,
                 with_dirs=True,
                 follow_symlinks=True)]
         )
 
     def test_extract_tree_with_colon_in_filenames(self):
         expected = (
             'colon/libc6:amd64.list',
         )
-        test_dir = self.get_test_loc('tar/colon.tar.xz')
+        test_dir = self.get_test_loc('utils/colon.tar.xz')
         extract_dir = self.get_temp_dir()
         events = utils.extract_tar(location=test_dir, target_dir=extract_dir)
         check_files(target_dir=extract_dir, expected=expected)
         assert not events
 
     def test_extract_tar_relative(self):
         expected = ()
-        test_dir = self.get_test_loc('tar/tar_relative.tar')
+        test_dir = self.get_test_loc('utils/tar_relative.tar')
         extract_dir = self.get_temp_dir()
         events = utils.extract_tar(location=test_dir, target_dir=extract_dir, as_events=True)
         check_files(target_dir=extract_dir, expected=expected)
         events = self.clean_events(extract_dir, events)
         expected_events = [
-            {'message': '/tar/tar_relative.tar: skipping unsupported ../a_parent_folder.txt with relative path.',
-             'source': '../a_parent_folder.txt',
-             'type': 'warning'},
-            {'message': '/tar/tar_relative.tar: skipping unsupported ../../another_folder/b_two_root.txt with relative path.',
+            {'message': '/utils/tar_relative.tar: skipping unsupported ../../another_folder/b_two_root.txt with relative path.',
              'source': '../../another_folder/b_two_root.txt',
              'type': 'warning'},
-            {'message': '/tar/tar_relative.tar: skipping unsupported ../folder/subfolder/b_subfolder.txt with relative path.',
+            {'message': '/utils/tar_relative.tar: skipping unsupported ../a_parent_folder.txt with relative path.',
+             'source': '../a_parent_folder.txt',
+             'type': 'warning'},
+            {'message': '/utils/tar_relative.tar: skipping unsupported ../folder/subfolder/b_subfolder.txt with relative path.',
              'source': '../folder/subfolder/b_subfolder.txt',
              'type': 'warning'},
         ]
 
         assert events == expected_events
 
+    def test_extract_tar_relative_with_whiteouts(self):
+        expected = (
+            '.wh..wh..opq',
+            '.wh..wh..plnk',
+            '.wh.foo.txt'
+        )
+        test_dir = self.get_test_loc('utils/tar_relative-with-whiteouts.tar')
+        extract_dir = self.get_temp_dir()
+        events = utils.extract_tar(location=test_dir, target_dir=extract_dir, as_events=True)
+        check_files(target_dir=extract_dir, expected=expected)
+        events = self.clean_events(extract_dir, events)
+        expected_events = [
+            {'message': '/utils/tar_relative-with-whiteouts.tar: skipping unsupported ../../another_folder/.wh..wh..opq with relative path.',
+             'source': '../../another_folder/.wh..wh..opq',
+             'type': 'warning'},
+            {'message': '/utils/tar_relative-with-whiteouts.tar: skipping unsupported ../.wh..wh..opq with relative path.',
+             'source': '../.wh..wh..opq',
+             'type': 'warning'},
+            {'message': '/utils/tar_relative-with-whiteouts.tar: skipping unsupported ../folder/subfolder/.wh..wh..opq with relative path.',
+             'source': '../folder/subfolder/.wh..wh..opq',
+             'type': 'warning'},
+        ]
+
+        assert events == expected_events
+
     def test_extract_tar_relative_as_strings(self):
         expected = ()
-        test_dir = self.get_test_loc('tar/tar_relative.tar')
+        test_dir = self.get_test_loc('utils/tar_relative.tar')
         extract_dir = self.get_temp_dir()
         events = utils.extract_tar(location=test_dir, target_dir=extract_dir, as_events=False)
         check_files(target_dir=extract_dir, expected=expected)
 
         events = [e.replace(self.test_data_dir, '') for e in events]
         expected_events = [
-            'warning: /tar/tar_relative.tar: skipping unsupported ../a_parent_folder.txt with relative path.',
-            'warning: /tar/tar_relative.tar: skipping unsupported ../../another_folder/b_two_root.txt with relative path.',
-            'warning: /tar/tar_relative.tar: skipping unsupported ../folder/subfolder/b_subfolder.txt with relative path.',
+            'warning: /utils/tar_relative.tar: skipping unsupported ../a_parent_folder.txt with relative path.',
+            'warning: /utils/tar_relative.tar: skipping unsupported ../../another_folder/b_two_root.txt with relative path.',
+            'warning: /utils/tar_relative.tar: skipping unsupported ../folder/subfolder/b_subfolder.txt with relative path.',
             ]
         assert events == expected_events
 
     def test_extract_tar_absolute(self):
         expected = (
             'tmp/subdir/a.txt',
             'tmp/subdir/b.txt',
         )
-        test_dir = self.get_test_loc('tar/absolute_path.tar')
+        test_dir = self.get_test_loc('utils/absolute_path.tar')
         extract_dir = self.get_temp_dir()
         events = utils.extract_tar(location=test_dir, target_dir=extract_dir, as_events=True)
         check_files(target_dir=extract_dir, expected=expected)
 
         events = self.clean_events(extract_dir, events)
         expected_events = [
-            {'message': '/tar/absolute_path.tar: absolute path name: /tmp/subdir transformed in relative path.',
+            {'message': '/utils/absolute_path.tar: absolute path name: /tmp/subdir transformed in relative path.',
              'source': '/tmp/subdir',
              'type': 'warning'},
-            {'message': '/tar/absolute_path.tar: absolute path name: /tmp/subdir/a.txt transformed in relative path.',
+            {'message': '/utils/absolute_path.tar: absolute path name: /tmp/subdir/a.txt transformed in relative path.',
              'source': '/tmp/subdir/a.txt',
              'type': 'warning'},
-            {'message': '/tar/absolute_path.tar: absolute path name: /tmp/subdir/b.txt transformed in relative path.',
+            {'message': '/utils/absolute_path.tar: absolute path name: /tmp/subdir/b.txt transformed in relative path.',
              'source': '/tmp/subdir/b.txt',
              'type': 'warning'},
         ]
 
         assert events == expected_events
 
     def test_extract_tar_not_skipping_links(self):
```

### Comparing `container-inspector-32.0.0/tests/utilities.py` & `container-inspector-32.0.1/tests/utilities.py`

 * *Files identical despite different names*

