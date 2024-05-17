# Comparing `tmp/opengate-10.0b7.tar.gz` & `tmp/opengate-10.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengate-10.0b7.tar", last modified: Thu Jan 11 12:27:59 2024, max compression
+gzip compressed data, was "opengate-10.0b8.tar", last modified: Fri May 17 11:11:54 2024, max compression
```

## Comparing `opengate-10.0b7.tar` & `opengate-10.0b8.tar`

### file list

```diff
@@ -1,362 +1,691 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:59.000307 opengate-10.0b7/
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-01-11 12:24:14.000000 opengate-10.0b7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-01-11 12:24:14.000000 opengate-10.0b7/DesignGuidelines.md
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-01-11 12:24:14.000000 opengate-10.0b7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-11 12:24:14.000000 opengate-10.0b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-01-11 12:27:59.000307 opengate-10.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-01-11 12:24:14.000000 opengate-10.0b7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-11 12:24:14.000000 opengate-10.0b7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.948307 opengate-10.0b7/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.948307 opengate-10.0b7/core/external/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.956307 opengate-10.0b7/core/external/fmt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.956307 opengate-10.0b7/core/external/fmt/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-11 12:24:32.000000 opengate-10.0b7/core/external/fmt/.github/issue_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-11 12:24:32.000000 opengate-10.0b7/core/external/fmt/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-11 12:24:32.000000 opengate-10.0b7/core/external/fmt/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.948307 opengate-10.0b7/core/external/fmt/support/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.956307 opengate-10.0b7/core/external/fmt/support/bazel/
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-01-11 12:24:32.000000 opengate-10.0b7/core/external/fmt/support/bazel/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.948307 opengate-10.0b7/core/external/fmt/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.956307 opengate-10.0b7/core/external/fmt/test/fuzzing/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-11 12:24:32.000000 opengate-10.0b7/core/external/fmt/test/fuzzing/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.956307 opengate-10.0b7/core/external/pybind11/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.956307 opengate-10.0b7/core/external/pybind11/.github/
--rw-r--r--   0 runner    (1001) docker     (127)    15285 2024-01-11 12:24:32.000000 opengate-10.0b7/core/external/pybind11/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-11 12:24:32.000000 opengate-10.0b7/core/external/pybind11/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-11 12:24:32.000000 opengate-10.0b7/core/external/pybind11/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.948307 opengate-10.0b7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.956307 opengate-10.0b7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)    33861 2024-01-11 12:24:14.000000 opengate-10.0b7/docs/source/developer_guide.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-11 12:24:14.000000 opengate-10.0b7/docs/source/user_guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-01-11 12:24:14.000000 opengate-10.0b7/docs/source/user_guide_1_intro.md
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-01-11 12:24:14.000000 opengate-10.0b7/docs/source/user_guide_2_0_simulation.md
--rw-r--r--   0 runner    (1001) docker     (127)    20195 2024-01-11 12:24:14.000000 opengate-10.0b7/docs/source/user_guide_2_1_volumes.md
--rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-01-11 12:24:14.000000 opengate-10.0b7/docs/source/user_guide_2_2_sources.md
--rw-r--r--   0 runner    (1001) docker     (127)    15510 2024-01-11 12:24:14.000000 opengate-10.0b7/docs/source/user_guide_2_3_physics.md
--rw-r--r--   0 runner    (1001) docker     (127)    13010 2024-01-11 12:24:14.000000 opengate-10.0b7/docs/source/user_guide_2_4_actors.md
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-11 12:24:14.000000 opengate-10.0b7/docs/source/user_guide_3_addons.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.960307 opengate-10.0b7/opengate/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.964307 opengate-10.0b7/opengate/actors/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actors/actorbuilders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actors/arfactors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actors/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    26589 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actors/digitizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    25564 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actors/doseactors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actors/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/actors/miscactors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17598 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.964307 opengate-10.0b7/opengate/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/dose_rate
--rwxr-xr-x   0 runner    (1001) docker     (127)     3687 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/ideal_timed_spect_reconstruction.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      126 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/opengate_info
--rwxr-xr-x   0 runner    (1001) docker     (127)     4616 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/opengate_tests
--rwxr-xr-x   0 runner    (1001) docker     (127)     1539 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/opengate_tests_utils
--rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/opengate_user_info
--rwxr-xr-x   0 runner    (1001) docker     (127)     1633 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/opengate_visu
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/readme.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1177 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/split_spect_projections
--rwxr-xr-x   0 runner    (1001) docker     (127)     3697 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/bin/voxelize_iec_phantom
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.964307 opengate-10.0b7/opengate/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)    26203 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/GateMaterials.db
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.964307 opengate-10.0b7/opengate/contrib/beamlines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/beamlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/beamlines/ionbeamline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.964307 opengate-10.0b7/opengate/contrib/dose/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/dose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/dose/dose_rate_test1.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     3995 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/dose/doserate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.964307 opengate-10.0b7/opengate/contrib/linacs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/linacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/linacs/elekta_synergy_materials.db
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/linacs/elektasynergy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/linacs/modified_elekta_synergy_materials.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.968307 opengate-10.0b7/opengate/contrib/pet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/pet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/pet/philipsvereos.py
--rw-r--r--   0 runner    (1001) docker     (127)    22685 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/pet/siemens_biograph_materials.db
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/pet/siemensbiograph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.968307 opengate-10.0b7/opengate/contrib/phantoms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/phantoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/phantoms/necr.py
--rw-r--r--   0 runner    (1001) docker     (127)    18143 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/phantoms/nemaiec.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.968307 opengate-10.0b7/opengate/contrib/spect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/spect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18178 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/spect/genm670.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/spect/spect_ge_nm670_materials.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.968307 opengate-10.0b7/opengate/contrib/tps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/tps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28920 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/tps/ionbeamtherapy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/contrib/tps/treatmentPlanPhsSource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.968307 opengate-10.0b7/opengate/data/
--rw-r--r--   0 runner    (1001) docker     (127)   524746 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/data/OpticalProperties.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    56289 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/engines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.968307 opengate-10.0b7/opengate/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22382 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/geometry/materials.py
--rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/geometry/solids.py
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/geometry/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    33890 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/geometry/volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.968307 opengate-10.0b7/opengate/mac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/mac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/mac/default_visu_commands.mac
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/mac/default_visu_commands_gdml.mac
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/mac/default_visu_commands_vrml.mac
--rw-r--r--   0 runner    (1001) docker     (127)    51235 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15646 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/physics.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/runtiming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/sources/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/beamsources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.952307 opengate-10.0b7/opengate/sources/beta_plus_spectra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/sources/beta_plus_spectra/C11/
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/beta_plus_spectra/C11/beta+_C11_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/sources/beta_plus_spectra/F18/
--rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/beta_plus_spectra/F18/beta+_F18_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/sources/beta_plus_spectra/Ga68/
--rw-r--r--   0 runner    (1001) docker     (127)    17616 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/beta_plus_spectra/Ga68/beta+_Ga68_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/sources/beta_plus_spectra/N13/
--rw-r--r--   0 runner    (1001) docker     (127)    17490 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/beta_plus_spectra/N13/beta+_N13_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/sources/beta_plus_spectra/Na22/
--rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/beta_plus_spectra/Na22/beta+_Na22_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/sources/beta_plus_spectra/O15/
--rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/beta_plus_spectra/O15/beta+_O15_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/sources/beta_plus_spectra/Rb82/
--rw-r--r--   0 runner    (1001) docker     (127)    15685 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/beta_plus_spectra/Rb82/beta+_Rb82_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/sources/beta_plus_spectra/Zr89/
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/beta_plus_spectra/Zr89/beta+_Zr89_tot.bs
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/gansources.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/phspsources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/sources/voxelsources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-11 12:27:57.000000 opengate-10.0b7/opengate/tests/HEAD
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/tests/log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/log/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.972307 opengate-10.0b7/opengate/tests/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:59.000307 opengate-10.0b7/opengate/tests/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2158 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test001_g4threevector.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      484 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test002_g4string.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test003_g4material.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4730 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test004_simple.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2604 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test004_simple_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1325 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test004_simple_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1908 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test004_simple_visu_gdml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4325 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test004_simple_visu_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1856 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test004_simple_visu_qt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1549 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test004_simple_visu_vrml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2603 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test004_simple_visu_vrml_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2133 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test004_simulation_stats_actor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1892 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test005_proton.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2915 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test006_runs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6705 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test007_volumes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3900 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test008_dose_actor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6381 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test008_geometry_dose_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3896 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test009_voxels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4563 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test009_voxels_hu.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4444 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test010_generic_source.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4056 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test010_generic_source_confine.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3911 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test010_generic_source_thetaphi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2123 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test011_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3364 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test012_mt_dose_actor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3649 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test013_half_life.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1641 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test013_phys_lists_1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1284 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test013_phys_lists_2_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1776 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test013_phys_lists_3_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1629 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test013_phys_lists_4.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1964 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test013_phys_lists_5_wip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test013_phys_lists_6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test013_phys_lists_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test014_engine_1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      535 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test014_engine_2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test014_engine_3_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test014_engine_4_mt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test014_engine_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test015_iec_phantom_1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2587 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test015_iec_phantom_2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2347 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test015_iec_phantom_3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test015_iec_phantom_4_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3794 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test016_bool_volumes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3453 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test017_repeater.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1919 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test018_pet_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test019_linac_phsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test019_linac_phsp_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      184 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test019_linac_phsp_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1092 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test019_linac_phsp_pdgcode.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test019_linac_phsp_source.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      853 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test019_linac_phsp_source_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      445 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test019_linac_phsp_visu.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3078 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test019_phsp_actor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3463 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test020_profiling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4213 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test021_voxel_source1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4903 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test021_voxel_source2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5723 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test021_voxel_source_old_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5299 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test022_half_life.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1670 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test022_half_life_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4928 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test022_half_life_ion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      284 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test022_half_life_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test023_filters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5587 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test023_filters_attribute.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4959 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test023_filters_attribute_bool.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2781 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test023_filters_iec_phantom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3122 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test023_filters_material.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1382 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test024_py_actor_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      220 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test025_hits_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test025_hits_collection_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      220 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test025_hits_collection_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test026_simple_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5050 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test027_fake_spect_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2864 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_1_colli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2895 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_1_colli_visu.py
--rw-r--r--   0 runner    (1001) docker     (127)    12476 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_2_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_2_hits.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      535 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_2_hits_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1005 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_3_proj.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2659 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_3_proj_blur.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      805 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_3_proj_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      653 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      653 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      685 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_ze.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      586 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_noaa.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1744 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test029_volume_time_rotation_1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1459 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test029_volume_time_rotation_1_process.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test029_volume_time_rotation_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test029_volume_time_rotation_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3961 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test030_dose_motion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5991 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test031_beta_plus_spectrum.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2674 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test032_create_voxelized_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4859 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test032_voxel_vs_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1955 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test032_voxelized_volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test033_rotation_spect_aa_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      526 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test033_rotation_spect_aa_se.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      539 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test033_rotation_spect_aa_se_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      584 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test033_rotation_spect_aa_ze.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      581 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test033_rotation_spect_noaa.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      594 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test033_rotation_spect_noaa_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4009 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test034_gan_phsp_linac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2101 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test035_dose_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test036_adder_depth_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      444 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test036_adder_depth_param.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      446 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test036_adder_depth_repeat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test037_digi_attributes_list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2164 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test037_pet_hits_singles_1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2284 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test037_pet_hits_singles_1_visu.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2769 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test037_pet_hits_singles_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test037_pet_hits_singles_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2493 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_aa.py
--rw-r--r--   0 runner    (1001) docker     (127)    13331 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      750 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_se.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      750 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_ze.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5543 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_training_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      406 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test039_hits_memory_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test039_hits_memory_check_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      406 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test039_hits_memory_check_mp_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4169 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test040_gan_phsp_pet_aref.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13625 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test040_gan_phsp_pet_gan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5335 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test040_gan_phsp_pet_training_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3775 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test041_dose_actor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4933 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test042_gauss_gps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4430 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test043_distances.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5417 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test043_garf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3264 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test043_garf_analog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test043_garf_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4967 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test043_garf_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3935 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test043_garf_training_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3190 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test043_garf_training_dataset_full_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5727 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test044_pbs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6382 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test044_pbs_rot_transl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5835 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test044_pbs_source_to_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6469 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test044_pbs_unfocused.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5997 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test044_pbs_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test045_gan_phsp_pet_gan_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3256 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test045_speedup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3069 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test045_speedup_all_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2466 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test046_rad.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4824 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test047_gan_vox_source_cond.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1488 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test047_voxelization.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1538 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test048_split_spect_projections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_v1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1787 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_v2_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2381 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_v3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2444 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_v4.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6297 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test050_let_actor_letd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4224 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test051_adder_time_difference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3042 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test052_tac_activity_source.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9105 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test053_production_cuts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8610 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test053_step_limiter_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3855 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test054_parallel_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test056_template_source.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4797 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test057_digit_efficiency.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6257 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test058_calc_uncertainty_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4413 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test058_iec_six_spheres.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6056 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test059_tpsource_abs_dose.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6863 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test059_tpsource_gantry_rot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7625 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test059_tpsource_optics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7198 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test059_tpsource_optics_vbl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5092 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test059_tpsource_range_ref.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5926 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test059_tpsource_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test060_phsp_source_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1156 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test060_phsp_source_particletype_direct.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1196 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test060_phsp_source_particletype_fromphs_particlename_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1183 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test060_phsp_source_particletype_fromphs_pdgcode.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1723 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test060_phsp_source_rotation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test060_phsp_source_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test060_phsp_source_untilNextPrimary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test061_TPPhsSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test061_TPPhsSource_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test061_user_event_info_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      684 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test061_user_event_info_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test062_apply_g4_cmds.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3739 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test063_em_switches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3769 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test064_kill_actor_mt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3047 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test065_sim_as_dict.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test065_sim_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test066_phspsource_activity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1935 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_0_orientation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2277 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_1_reference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2144 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2744 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_3_standalone.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1739 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_4_analyse1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1747 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_5_analyse2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2978 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test067_cbct_fluence_actor_mt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test068_rotation_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test069_rotation_DICOM_RT_plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51085 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/src/test069_rotation_DICOM_RT_plan_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    53680 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/tests/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/uisessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/userelement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/userhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-01-11 12:24:14.000000 opengate-10.0b7/opengate/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:27:58.960307 opengate-10.0b7/opengate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-01-11 12:27:58.000000 opengate-10.0b7/opengate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-01-11 12:27:58.000000 opengate-10.0b7/opengate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 12:27:58.000000 opengate-10.0b7/opengate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-11 12:27:58.000000 opengate-10.0b7/opengate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-11 12:27:58.000000 opengate-10.0b7/opengate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-11 12:24:14.000000 opengate-10.0b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 12:27:59.000307 opengate-10.0b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-01-11 12:24:14.000000 opengate-10.0b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.419329 opengate-10.0b8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-17 11:04:44.000000 opengate-10.0b8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-17 11:04:44.000000 opengate-10.0b8/DesignGuidelines.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-17 11:04:44.000000 opengate-10.0b8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-17 11:04:44.000000 opengate-10.0b8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-05-17 11:11:54.419329 opengate-10.0b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-17 11:04:44.000000 opengate-10.0b8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 11:04:44.000000 opengate-10.0b8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.311330 opengate-10.0b8/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.303330 opengate-10.0b8/core/external/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.311330 opengate-10.0b8/core/external/fmt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.311330 opengate-10.0b8/core/external/fmt/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.311330 opengate-10.0b8/core/external/fmt/doc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4938 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/doc/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.315330 opengate-10.0b8/core/external/fmt/support/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.315330 opengate-10.0b8/core/external/fmt/support/bazel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/support/bazel/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2064 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/support/build-docs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1590 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/support/compute-powers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/support/docopt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11495 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/support/manage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6109 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/support/printable.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3958 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/support/rst2md.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.315330 opengate-10.0b8/core/external/fmt/support/rtd/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/support/rtd/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.303330 opengate-10.0b8/core/external/fmt/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.315330 opengate-10.0b8/core/external/fmt/test/fuzzing/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/fmt/test/fuzzing/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.315330 opengate-10.0b8/core/external/pybind11/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.315330 opengate-10.0b8/core/external/pybind11/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)    15285 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.315330 opengate-10.0b8/core/external/pybind11/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/docs/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.315330 opengate-10.0b8/core/external/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.327330 opengate-10.0b8/core/external/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.327330 opengate-10.0b8/core/external/pybind11/tests/extra_python_package/
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.327330 opengate-10.0b8/core/external/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17243 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_chrono.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.327330 opengate-10.0b8/core/external/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_const_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29150 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_eigen_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.327330 opengate-10.0b8/core/external/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16491 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_iostream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18426 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22892 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_python_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25066 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_type_caster_pyobject_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_unnamed_namespace_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_unnamed_namespace_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_vector_unique_ptr_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12913 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tests/test_virtual_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.327330 opengate-10.0b8/core/external/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2047 2024-05-17 11:04:50.000000 opengate-10.0b8/core/external/pybind11/tools/make_changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.327330 opengate-10.0b8/core/opengate_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-17 11:04:44.000000 opengate-10.0b8/core/opengate_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-05-17 11:04:44.000000 opengate-10.0b8/core/opengate_core/g4DataSetup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.327330 opengate-10.0b8/core/opengate_core/g4_bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/core/opengate_core/g4_bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.327330 opengate-10.0b8/core/opengate_core/opengate_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/core/opengate_core/opengate_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-17 11:04:44.000000 opengate-10.0b8/core/opengate_core/qt5Setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-17 11:04:44.000000 opengate-10.0b8/core/opengate_core/testsDataSetup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6001 2024-05-17 11:04:44.000000 opengate-10.0b8/core/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.307330 opengate-10.0b8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.331330 opengate-10.0b8/docs/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7662 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50561 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/developer_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/user_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/user_guide_1_intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/user_guide_2_0_simulation.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21495 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/user_guide_2_1_volumes.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16406 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/user_guide_2_2_sources.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27945 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/user_guide_2_3_physics.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/user_guide_2_4_actors.md
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/user_guide_3_addons.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-05-17 11:04:44.000000 opengate-10.0b8/docs/source/user_guide_4_contrib.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.335330 opengate-10.0b8/opengate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.339330 opengate-10.0b8/opengate/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/actorbuilders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/arfactors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/coincidences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26614 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31175 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/doseactors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/dynamicactors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/actors/miscactors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22811 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.339330 opengate-10.0b8/opengate/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/dose_rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3727 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/ideal_timed_spect_reconstruction.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      148 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/opengate_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1521 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/opengate_library_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4616 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/opengate_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1521 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/opengate_tests_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/opengate_user_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1633 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/opengate_visu.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2603 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/phid_atomic_relaxation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5755 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/phid_gammas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      716 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/phid_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2099 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/phid_isomeric_transition.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1631 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/phid_tac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/readme.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1177 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/split_spect_projections.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3697 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/bin/voxelize_iec_phantom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.339330 opengate-10.0b8/opengate/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)    26203 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/GateMaterials.db
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.339330 opengate-10.0b8/opengate/contrib/beamlines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/beamlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/beamlines/ionbeamline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.343330 opengate-10.0b8/opengate/contrib/dose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/dose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/dose/dose_rate_test1.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3981 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/dose/doserate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.343330 opengate-10.0b8/opengate/contrib/linacs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/linacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/linacs/dicomrtplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/linacs/elekta_synergy_materials.db
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/linacs/elekta_versa_materials.db
+-rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/linacs/elektasynergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37940 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/linacs/elektaversa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.343330 opengate-10.0b8/opengate/contrib/pet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/pet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/pet/philipsvereos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22685 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/pet/siemens_biograph_materials.db
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/pet/siemensbiograph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.343330 opengate-10.0b8/opengate/contrib/phantoms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/phantoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/phantoms/necr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/phantoms/nemaiec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.343330 opengate-10.0b8/opengate/contrib/spect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/spect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/spect/ge_discovery_nm670.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31516 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/spect/siemens_intevo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/spect/spect_ge_nm670_materials.db
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/spect/spect_siemens_intevo_materials.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.343330 opengate-10.0b8/opengate/contrib/tps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/tps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/tps/ionbeamtherapy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/contrib/tps/treatmentPlanPhsSource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.347329 opengate-10.0b8/opengate/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   524746 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/OpticalProperties.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/Schneider2000DensitiesTable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/Schneider2000MaterialsTable.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8091 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/SurfaceProperties.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.359330 opengate-10.0b8/opengate/data/atomic_relaxation/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/ac-225.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/ac-226.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/ac-227.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/at-211.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/at-217.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/at-218.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/at-219.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/bi-207.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/bi-209.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/bi-210.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/bi-211.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/bi-212.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/bi-213.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/bi-214.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/bi-215.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/cf-251.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/cm-247.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/dy-161.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/eu-145.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/eu-149.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/fm-255.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/fr-221.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/fr-222.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/fr-223.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/gd-149.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/hf-177.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/hg-206.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/i-131.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/lu-177.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/nd-145.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pb-206.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pb-207.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pb-208.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pb-209.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pb-210.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pb-211.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pb-212.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pb-214.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pm-145.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/po-210.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/po-211.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/po-212.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/po-213.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/po-214.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/po-215.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/po-216.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/po-218.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/pr-141.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/ra-222.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/ra-223.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/ra-224.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/ra-226.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/rn-218.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/rn-219.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/rn-220.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/rn-222.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/ru-99.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/sm-145.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/sm-149.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/tb-149.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/tb-161.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/tc-99.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/th-226.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/th-227.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/tl-206.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/tl-207.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/tl-208.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/tl-209.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/tl-210.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/xe-131.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/atomic_relaxation/xe-131m.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.371329 opengate-10.0b8/opengate/data/isomeric_transition/
+-rw-r--r--   0 runner    (1001) docker     (127)    25536 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/ac-225.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/ac-226.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13831 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/ac-227.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/am-243.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/at-211.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/at-217.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/at-218.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/at-219.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/bi-207.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/bi-209.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/bi-210.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/bi-211.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/bi-212.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/bi-213.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    55857 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/bi-214.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/bi-215.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/cf-251.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/cm-247.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/dy-161.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21738 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/eu-145.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/eu-149.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22253 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/fm-255.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/fr-221.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14194 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/fr-222.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23716 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/fr-223.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19385 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/gd-149.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/hf-177.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/hg-206.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/i-131.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/lu-177.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/nd-145.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/np-239.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19950 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pa-231.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pb-206.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pb-207.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pb-208.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pb-209.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pb-210.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pb-211.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pb-212.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pb-214.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pm-145.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/po-210.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/po-211.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/po-212.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/po-213.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/po-214.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/po-215.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/po-216.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/po-218.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pr-141.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    40689 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pu-239.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/pu-243.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/ra-222.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16011 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/ra-223.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/ra-224.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/ra-226.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/rn-218.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/rn-219.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/rn-220.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/rn-222.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/ru-99.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/sm-145.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/sm-149.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    57425 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/tb-149.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/tb-161.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/tc-99.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/tc-99m.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/th-226.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    45641 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/th-227.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/th-231.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/tl-206.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/tl-207.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/tl-208.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/tl-209.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/tl-210.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/u-235.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/u-235m.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/xe-131.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/data/isomeric_transition/xe-131m.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53955 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/engines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.371329 opengate-10.0b8/opengate/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/geometry/materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18163 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/geometry/solids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/geometry/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41206 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/geometry/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13831 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.371329 opengate-10.0b8/opengate/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/mac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/mac/default_visu_commands.mac
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/mac/default_visu_commands_gdml.mac
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/mac/default_visu_commands_vrml.mac
+-rw-r--r--   0 runner    (1001) docker     (127)    58326 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29923 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/runtiming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.375329 opengate-10.0b8/opengate/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beamsources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.311330 opengate-10.0b8/opengate/sources/beta_plus_spectra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.375329 opengate-10.0b8/opengate/sources/beta_plus_spectra/C11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/C11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13835 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/C11/beta+_C11_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.375329 opengate-10.0b8/opengate/sources/beta_plus_spectra/F18/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/F18/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/F18/beta+_F18_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.375329 opengate-10.0b8/opengate/sources/beta_plus_spectra/Ga68/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/Ga68/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/Ga68/beta+_Ga68_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.375329 opengate-10.0b8/opengate/sources/beta_plus_spectra/N13/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/N13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17074 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/N13/beta+_N13_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.375329 opengate-10.0b8/opengate/sources/beta_plus_spectra/Na22/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/Na22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/Na22/beta+_Na22_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.375329 opengate-10.0b8/opengate/sources/beta_plus_spectra/O15/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/O15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14899 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/O15/beta+_O15_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.375329 opengate-10.0b8/opengate/sources/beta_plus_spectra/Rb82/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/Rb82/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15312 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/Rb82/beta+_Rb82_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.375329 opengate-10.0b8/opengate/sources/beta_plus_spectra/Zr89/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/Zr89/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/beta_plus_spectra/Zr89/beta+_Zr89_tot.bs
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/gansources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19389 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42908 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/phidsources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/phspsources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/sources/voxelsources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.379329 opengate-10.0b8/opengate/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 11:11:50.000000 opengate-10.0b8/opengate/tests/HEAD
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.379329 opengate-10.0b8/opengate/tests/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/log/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.379329 opengate-10.0b8/opengate/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.419329 opengate-10.0b8/opengate/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1518 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/demo_code_2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2158 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test001_g4threevector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      484 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test002_g4string.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test003_g4material.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4739 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test004_simple.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2604 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test004_simple_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1325 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test004_simple_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1908 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test004_simple_visu_gdml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4334 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test004_simple_visu_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1856 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test004_simple_visu_qt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1549 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test004_simple_visu_vrml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2603 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test004_simple_visu_vrml_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2133 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test004_simulation_stats_actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1893 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test005_proton.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2915 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test006_runs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6492 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test007_volumes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3841 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test008_dose_actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6381 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test008_geometry_dose_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3911 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test009_voxels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4336 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test009_voxels_dynamic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4575 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test009_voxels_hu.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4442 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test010_generic_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3676 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test010_generic_source_angular_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4092 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test010_generic_source_confine.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3911 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test010_generic_source_thetaphi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2123 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test011_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3368 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test012_mt_dose_actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3642 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test013_half_life.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1641 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test013_phys_lists_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1284 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test013_phys_lists_2_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1785 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test013_phys_lists_3_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1629 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test013_phys_lists_4.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1964 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test013_phys_lists_5_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2402 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test013_phys_lists_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test013_phys_lists_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test014_engine_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      535 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test014_engine_2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test014_engine_3_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test014_engine_4_mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test014_engine_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test015_iec_phantom_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2587 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test015_iec_phantom_2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2412 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test015_iec_phantom_3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2632 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test015_iec_phantom_4_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3794 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test016_bool_volumes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3490 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test017_repeater.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1919 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test018_pet_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3477 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_elekta_synergy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3499 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_elekta_versa.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5170 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_elekta_versa_rt_plan_isocenter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_elekta_versa_with_mlc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5861 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_elekta_versa_with_mlc_phsp_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7702 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_elekta_versa_with_mlc_rt_plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_phsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_phsp_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      184 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_phsp_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1092 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_phsp_pdgcode.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_phsp_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      853 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_phsp_source_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      445 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_linac_phsp_visu.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3078 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test019_phsp_actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3484 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test020_profiling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4267 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test021_voxel_source1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4988 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test021_voxel_source2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5847 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test021_voxel_source_old_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5299 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test022_half_life.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test022_half_life_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4931 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test022_half_life_ion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      284 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test022_half_life_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3489 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test023_filters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5587 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test023_filters_attribute.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4959 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test023_filters_attribute_bool.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2817 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test023_filters_iec_phantom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3161 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test023_filters_material.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1382 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test024_py_actor_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      220 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test025_hits_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test025_hits_collection_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      220 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test025_hits_collection_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1792 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test026_simple_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5050 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test027_fake_spect_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2874 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_1_colli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2898 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_1_colli_visu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_2_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_2_hits.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      535 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_2_hits_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1005 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_3_proj.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2659 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_3_proj_blur.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      805 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_3_proj_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      655 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      653 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      685 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_ze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      586 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_noaa.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1744 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test029_volume_time_rotation_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1459 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test029_volume_time_rotation_1_process.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test029_volume_time_rotation_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test029_volume_time_rotation_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3925 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test030_dose_motion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3857 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test030_dose_motion_dynamic_param.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7190 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test030_dose_motion_dynamic_param_custom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4263 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test030_dose_motion_runtime_overhead.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5991 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test031_beta_plus_spectrum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2674 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test032_create_voxelized_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4906 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test032_voxel_vs_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1958 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test032_voxelized_volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test033_rotation_spect_aa_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      526 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test033_rotation_spect_aa_se.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      539 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test033_rotation_spect_aa_se_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      584 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test033_rotation_spect_aa_ze.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      581 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test033_rotation_spect_noaa.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      594 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test033_rotation_spect_noaa_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4036 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test034_gan_phsp_linac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2101 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test035_dose_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test036_adder_depth_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      444 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test036_adder_depth_param.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      446 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test036_adder_depth_repeat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test037_digi_attributes_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2164 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test037_pet_hits_singles_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2284 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test037_pet_hits_singles_1_visu.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2769 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test037_pet_hits_singles_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test037_pet_hits_singles_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2493 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_aa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      750 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_se.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      750 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_ze.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5543 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_training_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      409 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test039_hits_memory_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test039_hits_memory_check_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      409 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test039_hits_memory_check_mp_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4168 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test040_gan_phsp_pet_aref.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13625 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test040_gan_phsp_pet_gan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5335 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test040_gan_phsp_pet_training_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4214 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test041_dose_actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8601 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test041_dose_actor_dose_to_water_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5218 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test041_dose_actor_mt_cp_images_Nthreads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7888 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test041_dose_actor_mt_standard_error_of_mean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4978 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test042_gauss_gps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4438 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test043_distances.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5420 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test043_garf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3274 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test043_garf_analog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test043_garf_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4970 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test043_garf_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3945 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test043_garf_training_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3193 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test043_garf_training_dataset_full_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5886 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test044_pbs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6513 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test044_pbs_rot_transl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5931 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test044_pbs_source_to_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6595 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test044_pbs_unfocused.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6066 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test044_pbs_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test045_gan_phsp_pet_gan_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3324 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test045_speedup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3069 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test045_speedup_all_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2477 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test046_rad.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4894 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test047_gan_vox_source_cond.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1488 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test047_voxelization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1538 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test048_split_spect_projections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_v1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1787 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_v2_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2381 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_v3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2444 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_v4.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7523 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test050_let_actor_letd_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4234 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test051_adder_time_difference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3045 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test052_tac_activity_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2967 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_01_gammas_at211_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      808 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_02_bi213_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      854 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_03_fr221_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4053 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_04_tac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1590 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_05_it_ref_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1844 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_06_it_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1911 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_08_ar_ref_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1892 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_09_ar_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1846 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_10_all_ref_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1989 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_11_all_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1976 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_12_all_model_mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_helpers1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_phid_helpers2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9105 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_production_cuts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8610 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test053_step_limiter_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3855 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test054_parallel_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test056_template_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4797 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test057_digit_efficiency.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6309 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test058_calc_uncertainty_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6558 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test058_calc_uncertainty_mt_ste_mean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4413 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test058_iec_six_spheres.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5481 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test058_uncertainty_flags_over_multiple_runs_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5977 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test059_tpsource_abs_dose.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9322 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test059_tpsource_flat_generation_flag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7122 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test059_tpsource_gantry_rot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7388 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test059_tpsource_optics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6950 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test059_tpsource_optics_vbl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4858 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test059_tpsource_range_ref.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5953 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test059_tpsource_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test060_phsp_source_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1156 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test060_phsp_source_particletype_direct.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1196 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test060_phsp_source_particletype_fromphs_particlename_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1183 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test060_phsp_source_particletype_fromphs_pdgcode.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1723 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test060_phsp_source_rotation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test060_phsp_source_translation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2855 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test060_phsp_source_untilNextPrimary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2207 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test061_TPPhsSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test061_TPPhsSource_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test061_user_event_info_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      684 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test061_user_event_info_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test062_apply_g4_cmds.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3739 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test063_em_switches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3772 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test064_kill_actor_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5995 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test065_dose2water_from_edep2water_ct.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5997 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test065_dose_from_edep_ct.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5511 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test065_dose_from_edep_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3047 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test065_sim_as_dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1393 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test065_sim_from_dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3475 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test066_phspsource_activity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1913 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_0_orientation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2277 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_1_reference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2144 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2755 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_3_standalone.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1739 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_4_analyse1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1747 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_5_analyse2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5489 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test066_stop_simulation_criteria_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3013 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test067_cbct_fluence_actor_mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test067_stl_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5852 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test068_rotation_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3887 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test070_4d_proton_dose.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4768 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test070_test_operator_brem_splitting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3143 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test071_custom_geometry_changer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6901 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test071_operator_russian_roulette.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7892 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test071_test_operator_compt_splitting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5363 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test072_back_to_back_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4085 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test072_coinc_sorter_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1610 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test072_coinc_sorter_2keepAll.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1595 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test072_coinc_sorter_2removeMultiples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test073_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2355 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test073_test1_intevo_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2449 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test073_test2_intevo_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1389 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test073_test3_intevo_tc99m_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1396 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test073_test4_intevo_lu177_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test073_test5_discovery_lu177_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test073_test5_discovery_tc99m_mt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3943 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test074_optical_surfaces_pet_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12458 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/src/test0_HFU_SOBP_wip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56528 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/tests/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/uisessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/userelement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/userhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-17 11:04:44.000000 opengate-10.0b8/opengate/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:11:54.419329 opengate-10.0b8/opengate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-05-17 11:11:54.000000 opengate-10.0b8/opengate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-17 11:11:54.000000 opengate-10.0b8/opengate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:11:54.000000 opengate-10.0b8/opengate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 11:11:54.000000 opengate-10.0b8/opengate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:11:53.000000 opengate-10.0b8/opengate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-17 11:11:54.000000 opengate-10.0b8/opengate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-17 11:11:54.000000 opengate-10.0b8/opengate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-17 11:04:44.000000 opengate-10.0b8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:11:54.419329 opengate-10.0b8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-17 11:04:44.000000 opengate-10.0b8/setup.py
```

### Comparing `opengate-10.0b7/CHANGELOG.md` & `opengate-10.0b8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/DesignGuidelines.md` & `opengate-10.0b8/DesignGuidelines.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/LICENSE.md` & `opengate-10.0b8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/PKG-INFO` & `opengate-10.0b8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,21 @@
-Metadata-Version: 2.1
-Name: opengate
-Version: 10.0b7
-Summary: Simulation for Medical Physics
-Home-page: https://github.com/OpenGATE/opengate
-Author: Opengate collaboration
-Author-email: david.sarrut@creatis.insa-lyon.fr
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/OpenGATE/opengate?logo=github)
+[![Read the Docs](https://img.shields.io/readthedocs/opengate-python?logo=read-the-docs&style=plastic)](https://opengate-python.readthedocs.io/)
 [![CI](https://github.com/OpenGATE/opengate/actions/workflows/main.yml/badge.svg)](https://github.com/OpenGATE/opengate/actions/workflows/main.yml)
 [![cirrus CI](https://api.cirrus-ci.com/github/OpenGATE/opengate.svg)](https://cirrus-ci.com/github/OpenGATE/opengate)
-[![Read the Docs](https://img.shields.io/readthedocs/opengate-python?logo=read-the-docs&style=plastic)](https://opengate-python.readthedocs.io/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/OpenGATE/opengate/master.svg)](https://results.pre-commit.ci/latest/github/OpenGATE/opengate/master)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OpenGATE/gam-gate/c65a0d55c616748454f066470aa836331eb107ac)
-
-See the [User Guide](https://opengate-python.readthedocs.io/en/latest/user_guide.html).
 
-# New since July 2023: there is a Windows version!
+## This is GATE10 **beta** version. The first non-beta release will be officially announced end of May 2024.
 
-Opengate is now available on Windows. For the moment, MultiThreading, Qt visualization and the "spawn new subprocess" are not (yet) available.
+See the [User Guide](https://opengate-python.readthedocs.io/en/latest/user_guide.html). The current version uses [Geant4 11.1.1](https://geant4.web.cern.ch).
 
-# How to install (short version)
 
-Compatible with Python 3.8, 3.9, 3.10, 3.11.
+### How to install (short version)
 
-**Warning** not available for MacOS Intel with python 3.11 yet.
+*Compatible with Python 3.8, 3.9, 3.10, 3.11. Not available for Python 3.12 yet. On Windows multithreading, Qt visualization and the "spawn new subprocess" are not (yet) available.*
 
 First, create an environment (not mandatory but highly advised)
 
 ```
 python -m venv opengate_env
 source opengate_env/bin/activate
 ```
@@ -43,15 +23,15 @@
 or you can use the conda environment.
 
 ```
 conda create --name opengate_env python=3.9
 conda activate opengate_env
 ```
 
-Then install the package opengate. The package opengate_core is automatically downloaded. opengate_core installs Geant4 v11.1.1 librairies.
+Then install the package opengate. The package ```opengate_core``` is automatically downloaded. ```opengate_core``` installs Geant4 librairies.
 ```
 pip install --upgrade pip
 pip install --pre opengate
 ```
 
 If you already installed the packages and want to upgrade to the latest version:
 
@@ -75,14 +55,10 @@
 ````
 pip install torch
 pip install gaga-phsp
 ````
 
 The documentation is here: https://opengate-python.readthedocs.io/en/latest/user_guide.html
 
-# How to install (long version, for developers)
-
-See the documentation : https://opengate-python.readthedocs.io/en/latest/developer_guide.html#installation-for-developers
-
-WARNING : need [Geant4 11.1.1](https://geant4.web.cern.ch/download/11.1.1.html)
-
+### How to install (long version, for developers)
 
+See the documentation: https://opengate-python.readthedocs.io/en/latest/developer_guide.html#installation-for-developers
```

### Comparing `opengate-10.0b7/core/external/fmt/CONTRIBUTING.md` & `opengate-10.0b8/core/external/fmt/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/core/external/fmt/support/bazel/README.md` & `opengate-10.0b8/core/external/fmt/support/bazel/README.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/core/external/fmt/test/fuzzing/README.md` & `opengate-10.0b8/core/external/fmt/test/fuzzing/README.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/core/external/pybind11/.github/CONTRIBUTING.md` & `opengate-10.0b8/core/external/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/core/external/pybind11/.github/pull_request_template.md` & `opengate-10.0b8/core/external/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/core/external/pybind11/SECURITY.md` & `opengate-10.0b8/core/external/pybind11/SECURITY.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/docs/source/developer_guide.md` & `opengate-10.0b8/docs/source/developer_guide.md`

 * *Files 25% similar despite different names*

```diff
@@ -4,30 +4,41 @@
 
 The source code is divided into two main modules, one in C++, the second in Python. The first module is used to access the Geant4 engine and for the tasks that demand speed during the run of a simulation. The second module manages user interface (the way an user create a simulation) and most tasks performed at initialization (before the run).
 
 - `opengate_core` (C++) contains C++ Geant4 bindings and a C++ library that uses Geant4. The two components form a single Python module called `opengate_core` that can interact with Geant4 library and expose to Python functions and classes. Sources: [opengate_core](https://github.com/OpenGATE/opengate/tree/master/core)
 - `opengate` (Python) is the main Python module that form the interface to the user.
   Sources: [opengate](https://github.com/OpenGATE/opengate/tree/master/opengate)
 
-**WARNING** it is highly, highly, *highly* advised to first create a python environment, for example with [venv](https://docs.python.org/3/library/venv.html#module-venv) or [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#).
+:warning: It is highly, highly, *highly* recommended to create a python environment prior to the installation, for example with [venv](https://docs.python.org/3/library/venv.html#module-venv).
 
-To **develop**, you need 1) to compile and create the first `opengate_core` module and 2) pip install the second (Python only) `opengate` module.
+:warning: If you use [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#) instead to create your environment, be sure to instruct conda to install python when creating your environment. You do so by adding 'python' after the new environment name. Optionally, you can select a specific python version by adding '=3.XX'.
 
-First, clone the unique repository that contains both modules:
+Example: You can create a new conda environment with Python 3.10 installed in it via:
+
+```bash
+  conda create --name opengate_env python=3.10
+  conda activate opengate_env
+```
+
+To **develop** in GATE 10, you need 1) to compile and create the `opengate_core` subpackage (this is the hardest part) and 2) install the main  `opengate` package (Python only, fast and easy).
+
+First, clone the unique repository that contains both packages:
 
 ```bash
 git clone --recurse-submodules https://github.com/OpenGATE/opengate
 ```
 
-Note that you need to also clone the included submodules (pybind11, all data for tests etc). If you forget the `--recurse-submodules` you can still use `git submodule update --init --recursive` after the clone.
+Note that you also need to clone the included subpackages (pybind11, all data for tests etc). If you forget the `--recurse-submodules`, you can still use `git submodule update --init --recursive` after the clone.
 
-First step: compile `opengate_core` (this is the hardest part). You need to set the path to build Geant4 and ITK libraries ; it means you need first to download and compile both [Geant4](https://geant4.web.cern.ch) and [ITK](https://itk.org).
+The subpackage `opengate_core` depends on the ITK and Geant4 libraries. Therefore, you first need to download and compile both [Geant4](https://geant4.web.cern.ch) and [ITK](https://itk.org). Note: In the user install, this step is not necessary because Geant4 and ITK are shipped pre-compiled via pip.
 
 #### STEP 1 - Geant4 and Qt
 
+:warning: When using conda, be sure to activate your environment before compiling Geant4. The reason is that conda comes with its own compiler and you will likely have mismatched libraries, e.g. lib c++, if not all installation steps involving compilaton are performed in the same conda environment.
+
 Installing QT is optional. Currently, QT visualisation is not working on all architectures.
 
 If you wish to use QT, you must install qt5 **before** installing Geant4 so that Geant4 can find the correct qt lib. It can be done for example with conda:
 
 ```bash
   conda install qt=5
 ```
@@ -46,18 +57,21 @@
       -DGEANT4_BUILD_MULTITHREADED=ON \
       ../geant4
 make -j 32
 ```
 
 Change the QT flag (GEANT4_USE_QT) to OFF if you did not install QT.
 
-WARNING : from June 2023, [Geant4 11.1.1](https://geant4.web.cern.ch/download/11.1.1.html) is needed.
+WARNING : since June 2023, [Geant4 11.1.1](https://geant4.web.cern.ch/download/11.1.1.html) is needed.
 
 #### STEP 2 - ITK
 
+**WARNING** When using conda, be sure to activate your environment before compiling Geant4. The reason is that conda comes with its own compiler and you will likely have mismatched libraries, e.g. lib c++, if not all installation steps involving compilaton are performed in the same conda environment.
+
+
 For **ITK**, you need to compile with the following options:
 
 ```bash
 git clone --branch v5.2.1 https://github.com/InsightSoftwareConsortium/ITK.git --depth 1
 mkdir itk-build
 cd itk-build
 cmake -DCMAKE_CXX_FLAGS=-std=c++17 \
@@ -122,15 +136,15 @@
 pip install torch
 pip install gaga-phsp
 pip install garf
 ```
 
 ## How to contribute (for developers)
 
-We are really happy if you want to propose a new feature or changes in Gate. Please contact us and share your ideas with us - this is how Gate was born and how it will keep growing!
+We are really happy if you want to propose a new feature or changes in GATE. Please contact us and share your ideas with us - this is how Gate was born and how it will keep growing!
 
 ### Propose a pull request:
 1) Fork the opengate repository into your own github.
 2)  Create a branch for the feature you want to contribute, starting from the current opengate master branch.
 3)  Start implementing your ideas in your newly created branch (locally) and keep committing changes as you move forward.
 4)  Prefer several small commits with clear comments over huge commits involving many files and changes.
 5)  Push changes to your github repo. Also pull changes from the upstream/master (opengate's master branch) regularly to stayed synced.
@@ -138,15 +152,15 @@
 7)  We will then see your branch as PR in the opengate repository and can better understand what you are working on, and help you out if needed.
 8)  Ideally, go to the opengate repository and open your own pull request. You should see a checkbox below on the right side saying "Allow edits and access to secrets by maintainers". Please tick it. In this way, we can directly commit changes into your branch - of course we'll be in touch with you.
 ​
 
 More info about [Pull Requests on github](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
 
 
-### Tests and docmentation
+### Tests and documentation
 It is important to make sure that Gate keeps working consistently and that simulation outcome is reliable as we keep developing the code. Therefore, we have a large set of tests which are regularly run. If you propose new features or make changes to the inner workings of Gate, please create a little test simulation that goes with it. It should be imlpemented in such a way that it checks whether the feature works as expected. This might be a check of Geant4 parameters, e.g. if production cuts are set correctly, or based on simulation outcome, such as a dose maps or a particle phase space. Best is to look at the folder `tests` in the source code.
 
 
 Your test will also serve other users as example on how the new feature is used.
 
 
 There is a set of functions useful for tests in `opengate/tests/utility.py` which you can, e.g., import as
@@ -166,14 +180,42 @@
 # then move to the opengate folder and do:
 pre-commit install
 ```
 
 Do not worry, if you forget to install it - you/we will see the error during the automatic testing (Continuous Integration) in Github and can fix it then through another commit.
 
 
+## GATE architecture: Managers and Engines
+
+GATE 10 has two distinct kinds of classes which handle a simulation. Managers provide an interface to the user to set-up and configure a simulation and collect and organize user parameters in a structured way. Engines provide the interface with Geant4 and are responsible for creating all Geant4 objects. Managers and engines are divided in sub-managers and sub-engines responsible for certain logical parts of a simulation. Additionally, many objects in GATE are now implemented as classes which provide interfaces to the managers and engines.
+
+The `Simulation` class is the main manager with which the user interacts. It collects general parameters, e.g. about verbosity and visualization and it manages the way the simulation is run (in a subprocess or not). Sub-managers are: `VolumeManager`, `PhysicsManager` , `ActorManager`, `SourceManager`. These managers can be thought of as bookkeepers. For example, the `VolumeManager` keeps a dictionary with all the volumes added to a simulation, a dictionary with all the parallel world volumes, etc. But it also provides the user with methods to perform certain tasks, e.g. `VolumeManager.add_parallel_world()`.
+
+The `SimulationEngine` is the main driver of the Geant4 simulation: every time the user calls `sim.run()`, the `Simulation` object (here assumed to be called `sim`) creates a new `SimulationEngine` which in turn creates all the sub-engines: `VolumeEngine`, `PhysicsEngine`, `SourceEngine`, `ActorEngine`, `ActionEngine`.
+The method `SimulationEngine.run_engine()` actually triggers the construction and run of the Geant4 simulation. It takes the role of the `main.cc` in a pure Geant4 simulation.
+When the Geant4 simulation has terminated, `SimulationEngine.run_engine()` returns the simulation output which is then collect by the `Simulation` object and remains accessible via `sim.output`.
+
+It is important to understand that the engines only exist while the GATE/Geant4 simulation is running, while the managers exist during the entire duration of the python interpreter session in which the user is setting up the simulation.
+
+The managers and engines are explained in more detail below.
+
+### References among managers and engines
+
+Managers and engines frequently need to access attributes of other managers and engines. They therefore need references to each other. In GATE, these references follow a hierarchical pattern:
+
+- Sub-managers keep a references to the `Simulation` (the main manager). Sub-sub-managers keep references to the sub-manager above them. For example: `PhysicsManager.simulation` refers to the `Simulation` object which created it, and `PhysicsListManager.physics_manager` refers to the `PhysicsManager` which created it.
+- Objects created through a manager keep a reference to the creating manager. For example: all volumes have an attribute `volume_manager`.
+- In a similar fashion, sub-engines keep a references to the `SimulationEngine` from which they originate.
+- The `SimulationEngine` itself keeps a reference to the `Simulation` which created it.
+
+This hierarchical network of references allows reaching objects from any other object. For example: a `Region` object is managed by the `PhysicsManager`, so from a region, a volume can be reached via:
+```python
+my_volume = region.physics_manager.simulation.volume_manager.get_volume('my_volume')
+```
+
 ---
 ## Geant4 bindings
 
 This repository contains C++ source code that maps some (not all!) Geant4 classes into one single Python module. It also contains additional C++ classes that extends Geant4 functionalities (also mapped to Python). At the end of the compilation process a single Python module is available, named `opengate_core` and is ready to use from the Python side.
 
 The source files are divided into two folders: `g4_bindings` and `opengate_lib`. The first contains pure Geant4 Python bindings allow to expose in Python a (small) part of Geant4 classes and functions. The bindings are done with the [pybind11](https://github.com/pybind/pybind11) library. The second folder contains specific opengate functionalities.
 
@@ -186,14 +228,113 @@
 - In this function, indicate all functions/members that you want to expose.
 - Declare and call this init function in the `opengate_core.cpp` file.
 
 ### Misc
 
 - Not clear if G4RunManager should be destructed at the end of the simulation. For the moment we use `py::nodelete` to prevent deletion because seg fault after the run.
 
+
+## Philosophy behind objects implemented as GateObject
+
+Generally, the idea is to encapsulate functionality into classes rather than spreading out the code across managers and engines. The advantage is that the code structure remains less cluttered. Good examples are the `Region` class and, although more complex, the volume classes. In the following, we explain the rationale and design concept. For instructions on how to implement or extend a class, see [here](#how-a-class-in-gate-10-is-usually-set-up).
+
+The GATE classes representing and a Geant4 object (or multiple Geant4 objects combined) are meant to do multiple things:
+1) Be a storage for user parameters. Exmample: the `Region` class holds the user_info `user_limits`, `production_cuts`, and `em_switches`.
+2) Provide interface functions to manager classes (and the user) to configure the object or inquire about it. Examples: `Region.associate_volume()`, `Region.need_step_limiter()`
+3) Provide interface functions such as `initialize()` and `close()` to the engines to handle the Geant4 objects.
+4) Provide convenience functionality such as dumping as dictionary (`to_dictionary()`, `from_dictionary()`), dump info about the object (e.g. `Region.dump_production_cuts()`), clone itself.
+5) Handle technical aspects such as pickling (for subprocesses) in a unified way ([via the method `__getstate__()`](#implement-a-getstate-method-if-needed))
+
+The managers and engines, on the other hand, remain quite sleek and clean. For example, if you look at the `PhysicsEngine` class, you find the method
+```python
+    def initialize_regions(self):
+        for region in self.physics_manager.regions.values():
+            region.initialize()
+```
+which really just iterates over the regions and initializes them.
+
+The advantage of this becomes evident especially if there are multiple variants of a class (via inheritance), such as for volumes. In this case, the `VolumeEngine` does not care about the specific type of volume because it always calls the same interface. For example, `VolumeEngine.Construct()` (which is triggered by the G4RunManager, not GATE) iterates over the volumes and calls `volume.construct()`. The volume object then takes care of taking the correct actions. If the code inside each volume's `construct()` method were implemented inside  `VolumeEngine.Construct()`, it would be cluttered with if statements to pick what should be done.
+
+> **Note**\
+> For now, only a part of GATE implements objects based on the GateObject base class. Actors and Sources still need to be refactored.
+
+## How a class in GATE 10 is (usually) set up:
+
+### Naming convention
+- Use small letters and underscores for python variables. Do **not** use capital letters and camelcase.
+- Use capital letters and camel case for overloaded C++ variables if the class inherits from a base class implemented in C++.
+- All attributes pointing to Geant4 objects should have a “g4_” prepended for easy identification. Example: `self.g4_logical_volume`.
+- Group the `g4_***` definitions in one block for better visual reference.
+
+### `__init__()` method
+- Define all attributes of the object in the `__init__()` method even if their value is set only later/elsewhere.
+- If no value is set in `__init__()`, do:
+  ```python
+  self.my_attribute = None
+  ```
+- By defining all attributes in the `__init__()` method, other developers can easily inspect the class without reading through the entire class. Think of it as a C++ header file.
+
+- If your class inherits from another class, and in particular from `GateObject` or `DynamicGateObject`, include wild card arguments and keyword arguments in your `__init__()` method:
+
+  ```python
+  def __init__(self, your_specific_arguments, *args, your_specific_kwargs, **kwargs):
+      super().__init__(*args, **kwargs)
+      # ... YOUR CODE...
+  ```
+
+### User info: handling parameters set by the user
+If your class handles user input, let it inherit from GateObject, or DynamicGateObject if applicable. Define and configure user input via the `user_info_defaults` class attribute. See section XXX.
+
+**Important**: User input defined and configured in the `user_info_defaults` dictionary should generally not be handled manually in your `__init__()` method. They are passed on to the superclass inside the `kwargs` dictionary. See section XXX for more detail.
+
+### Initialization of Geant4 objects
+Implement an `initialize()` method if Geant4 objects need to be created by the SimulationEngine (or a sub-engine) when the simulation is launched. The `initialize()` method should not take any arguments, but only rely on object attributes (`self.xyz`) which were previously set.
+
+Exception: G4RunManager has an initializatin sequence which GATE relies on. In certain classes, the `g4_XXX` componentes are initialized as part of this sequence on the C++ side. Example: All volumes implement a `construct()` method which is called when the G4RunManager calls the overloaded `Construct()` method of the VolumeEngine.
+
+### Implement a `close()` method if needed
+Explanation: If your class has attributes that point to Geant4 objects which are deleted by the G4RunManager at the end of a simulation, your class must get rid of these references when the SimulationEngine closes down. This is achieved by a hierarchy of calls to a close() method, starting from `SimulationEngine.close()`. In your `close()` method, set all attributes pointing to Geant4 objects which the G4RunManafger will delete to `None`. If your class manages a list of other objects which themselves need to call their `close()` method, add a loop to your `close()` method and close down the list members. If you inherit from another class, do not forget to call the `close()` method from the superclass via `super().close()`.
+Take a look at `VolumeManager.close()` and the volumes classes or `PhysicsManager.close()` and the `Region` class for examples.
+
+### Implement a `__getstate__()` method if needed.
+Explanation: When a GATE simulation is run in a subprocess, all objects need to be serialized so they can be sent to the subprocess, where they are deserialized. The serialization is currently handled by the `pickle` module. If your class contains attributes which refer to objects which cannot be pickled, the serialization will fail. This typically concerns Geant4 objects. To make your class pickleable, you should implement a `__getstate__()` method. This is essentially a hook called within the serialization pipeline which returns a representation of your object (usually a dictionary). You should remove items which cannot be pickled from this dictionary.
+
+**Example**: Assume your class has an attribute `self.g4_funny_object` referring to a Geant4 object. Your `__getstate__()` method should do something like this:
+
+```python
+def __getstate__(self):
+	return_dict = self.__dict__
+	return_dict['g4_funny_object'] = None
+	return return_dict
+```
+
+If your class inherits from another one, e.g. from GateObject, you should call the `__getstate__()` method from the superclass:
+
+```python
+def __getstate__(self):
+	return_dict = super().__getstate__()
+	return_dict['g4_funny_object'] = None
+	return return_dict
+```
+
+**Important**: The `__getstate__()` method should **not** change your object, but only modify the dictionary to be returned. Therefore, avoid `self.g4_funny_object = None` as this also alters your object.
+
+Important: Do **not** use the `close()` method in your `__getstate__()` method. The `close()` method is part of [another mechanism](#implement-a-close-method-if-needed-) and these mechanisms should not be entangled. And: the `close()` method would alter your object and not only the returned dictionary representation.
+
+### Optional: Implement a `__str__()` method
+You might consider implementing a `__str__()` method which, by construction, is required to return a string. If implemented, this method is called when the user places your object inside a `print()` statement: `print(my_object)`. You could implement the `__str__()` method to provide useful information about your object. If your object inherits from another class, call the superclass:
+```python
+def __str__(self):
+	s = super().__str__()
+	s += "*** Additional info: ***\n"
+	s += f"The object as an attribute 'xyz' of value {self.xyz}.\n"
+	return s
+```
+In particular, the GateObject superclass (and variants) implement a `__str__()` method which lists all user_info of the object.
+
 ---
 ## Helpers
 
 Error handling. Use the following to fail with an exception and trace:
 
 ```python
 import opengate as gate
@@ -201,42 +342,98 @@
 gate.raise_except('There is bug')
 gate.exception.fatal('This is a fatal error')
 gate.exception.warning('This is a warning')
 ```
 
 There are several levels: `WARNING INFO DEBUG`. The last one print more information. Logging is handled with logger in `helpers_log.py`.
 
-## OPENGATE Simulation
+## Engines
+As explained [above](#gate-architecture-managers-and-engines), the Engine classes drive the actual Geant4 simulation. This section explains the engines in detail.
 
-Main object:
+### SimulationEngine
+The `SimulationEngine` is the main engine class. Upon instantiation (i.e., in the `__init__()` method), all sub-engines are created which drive the different parts if the Geant4 simulation. The sub-engines keep a reference to the `SimulationEngine` which created them.
 
-```python
-sim = gate.Simulation()
-ui = sim.user_info
-ui.verbose_level = gate.DEBUG
-ui.g4_verbose = False
-ui.g4_verbose_level = 1
-ui.visu = False
-ui.random_engine = 'MersenneTwister'
-ui.random_seed = 'auto'
-```
+The three main methods of the `SimulationEngine` are `SimulationEngine.run_engine()`, `SimulationEngine.initialize()` and `SimulationEngine.start_and_stop()`, where the latter two are called by the former.
+The method `SimulationEngine.run_engine()` essentially takes the role of the `main.cc` in a pure Geant4 simulation. It first initializes the simulation with `SimulationEngine.initialize()` and then starts event loop with `SimulationEngine.start_and_stop()` via the `SourceEngine`.
+
+The `SimulationEngine` uses the `G4RunManager` via a pybind11 wrapping and many Geant4 objects are created by the `G4RunManager`. In short: The `G4RunManager` is informed about the geometry, physics, and sources via its `SetUserInitialization()` method. The Geant4 initialization procedure is then triggered by `g4_RunManager.Initialize()`, just as a regular Geant4 simulation would.
+For details, please consult the Geant4 user guide.
+
+Note that there are subtleties concerning the way the `G4RunManager` works in singlethread and multithread mode which we do not cover in this guide.
+
+Complementary to the `g4_RunManager.Initialize()`, there are expicit calls to `initialize()` methods of the sub-engines, some of them before `g4_RunManager.Initialize()` and some afterwards.
+
+The `SimulationEngine` is implemented as what is known in python as *context manager*. This means, in can be created in a *with-clause*: `with SimulationEngine(self) as se: ...` (see `SimulationEngine._run_simulation_engine()`). What it does is that the `SimulationEngine` object only exists as long as the commands inside the *with-clause* are executed. At the end of the *with-clause*, python calls the method `SimulationEngine.__exit__()` (like an exit hook) which triggers the method `SimulationEngine.close()`. The purpose of the `close()` method is to prepare all python objects that are part of the GATE simulation for the deletion of the `G4RunManager`. In particular, it makes sure that references to those Geant4 objects which the destructor of the `G4RunManager` will delete are set to `None`. Otherwise, segmentation faults will occur. We do not go into further detail here, but it is useful to understand this background of the `close()` mechanism triggered by the *with-clause* because you, as a developer, might need to implement a `close()` method in your class or extend the `close()` in an existing class which your are enhancing (see the section on [how a class is set up in GATE](#how-a-class-in-gate-10-is-usually-set-up-).
+
+It is worth noting that you have probably already come across *context managers* in python elsewhere. For example, when opening a file, you typically do `with open('my_file.txt', 'w') as f: ...`. When the *with-clause* ends, python automatically calls `f.close()`, i.e. closes the IO pipeline.
+
+### VolumeEngine
+
+
+### PhysicsEngine
+
+
+### ActorEngine
+
+
+### SourceEngine
+
+
+### ActionEngine
+
+[//]: # ()
+[//]: # (## OPENGATE Simulation)
+
+[//]: # ()
+[//]: # (Main object:)
+
+[//]: # ()
+[//]: # (```python)
+
+[//]: # (sim = gate.Simulation&#40;&#41;)
+
+[//]: # (ui = sim.user_info)
+
+[//]: # (ui.verbose_level = gate.DEBUG)
+
+[//]: # (ui.g4_verbose = False)
+
+[//]: # (ui.g4_verbose_level = 1)
+
+[//]: # (ui.visu = False)
+
+[//]: # (ui.random_engine = 'MersenneTwister')
+
+[//]: # (ui.random_seed = 'auto')
+
+[//]: # (```)
+
+[//]: # ()
+[//]: # (The `Simulation` class contains:)
+
+[//]: # ()
+[//]: # (- some global properties such as verbose, visualisation, multithread. All options are stored in `user_info` variable &#40;a kind of dict&#41;)
+
+[//]: # (- some managers: volume, source, actor, physics)
+
+[//]: # (- some G4 objects &#40;RunManager, RandomEngine etc&#41;)
+
+[//]: # (- some variables for internal state)
+
+[//]: # ()
+[//]: # (And the following methods:)
 
-The `Simulation` class contains:
+[//]: # ()
+[//]: # (- some methods for print and dump)
 
-- some global properties such as verbose, visualisation, multithread. All options are stored in `user_info` variable (a kind of dict)
-- some managers: volume, source, actor, physics
-- some G4 objects (RunManager, RandomEngine etc)
-- some variables for internal state
+[//]: # (- `initialize`)
 
-And the following methods:
+[//]: # (- `apply_g4_command`)
 
-- some methods for print and dump
-- `initialize`
-- `apply_g4_command`
-- `start`
+[//]: # (- `start`)
 
 ---
 ## OPENGATE elements: volumes, physic, sources, actors
 
 A simulation is composed of several elements: some volumes, some sources, some actors and some physics properties. The parameters that can be defined by the user (the person that develop the simulation) are managed by simple dict-like structure. No Geant4 objects are build until the initialization phase. This allows (relative) simplicity in the development.
 
 ### UserInfo (before initialisation)
```

### Comparing `opengate-10.0b7/docs/source/user_guide_1_intro.md` & `opengate-10.0b8/docs/source/user_guide_1_intro.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 - Use of Python as the primary scripting language for creating simulations
 - Multithreading support for efficient simulation execution
 - Native integration with ITK for image management
 - Compatibility with Linux, Mac, and potentially Windows operating systems
 - Convenient installation via a single pip install opengate command
 - ...
 
-
 ### Installation (for users, not for developers)
 
 You only have to install the Python module with, the --pre option is mandatory to have the latest release:
 
     pip install --pre opengate
 
 Then, you can create a simulation using the opengate module (see below). For **developers**, please look the [developer guide](developer_guide) for the developer installation.
@@ -63,30 +62,31 @@
 
     pip install --upgrade pip
 
 If you already installed opengate, just upgrade it with:
 
     pip install --upgrade --pre opengate
 
-Once installed, we recommend to check the installation by running the tests:
+Once installed, we recommend to check the installation by printing GATE information and running the tests:
 
+    opengate_info
     opengate_tests
 
 **WARNING 1** The first time a simulation is executed, the Geant4 data must be downloaded and installed. This step is automated but can take some times according to your bandwidth. Note that this is only done once. Running `opengate_info` will print some details and the path of the data.
 
 **WARNING 2** With some linux systems (not all), you may encounter an error similar to "cannot allocate memory in static TLS block". In that case, you must add a specific path to the linker as follows:
 
     export LD_PRELOAD=<path to libG4processes>:<path to libG4geometry>:${LD_PRELOAD}
 
 The libraries (libG4processes and libG4geometry) are usually found in the Geant4 folder, something like ```~/build-geant4.11.0.2/BuildProducts/lib64```.
 
 ### Additional command lines tools
 
-There is some additional commands lines tools that can also be used. First, type ```opengate_info```, it will print some information about the current installation (Geant4 version, ITK version etc). Also, ```opengate_user_info``` is useful to print all default and possible parameters, see next section.
+There is some additional commands lines tools that can also be used, see the [addons section](user_guide_3_addons.md).
 
-### Some (temporary) teaching materials
+### Teaching resources and examples
 
-Here is a video recorded on 2022-07-28 : [video](https://drive.google.com/file/d/1fdqmzhX0DFZUIO4Ds0PQZ-44obCqWb8R/view?usp=sharing). Please note, it was recorded at early stage of the project, so maybe outdated.
+*Warning* they are only updated infrequently, you may have to adapt them to changes in the gate version.
 
-### Notebooks, myBinder (experimental)
+-  [exercices](https://gitlab.in2p3.fr/davidsarrut/gate_exercices_2) (initially developed for DQPRM, French medical physics diploma)
 
-You can try the examples without any installation using myBinder. On the [GitHub page](https://github.com/OpenGATE/opengate), click on the myBinder icon to start running a remote notebook. When the jupyter notebook is started (it can take some times), you have access to all examples in the repository: `notebook/notebook`.
+- [exercices](https://drive.google.com/drive/folders/1bcIS5OPLOBzhLo0NvrLJL5IxVQidNYCF) (initially developed for Opengate teaching)
```

### Comparing `opengate-10.0b7/docs/source/user_guide_2_0_simulation.md` & `opengate-10.0b8/docs/source/user_guide_2_0_simulation.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 Any simulation starts by defining the (unique) `Simulation` object. The generic options can be set with the `user_info` data structure (a kind of dictionary), as follows. You can print this `user_info` data structure to see all available options with the default value `print(sim.user_info)`.
 
 ```python
 sim = gate.Simulation()
 ui = sim.user_info
 print(ui)
-ui.verbose_level = gate.DEBUG
-ui.running_verbose_level = gate.EVENT
+ui.verbose_level = gate.LOG_DEBUG
+ui.running_verbose_level = gate.LOG_EVENT
 ui.g4_verbose = False
 ui.g4_verbose_level = 1
 ui.visu = False
 ui.visu_verbose = False
 ui.random_engine = 'MersenneTwister'
 ui.random_seed = 'auto'
 ui.number_of_threads = 1
@@ -134,15 +134,15 @@
 
 This behavior may change in the future.
 
 #### Multiprocessing (advanced use)
 
 The Geant4 simulation engine has a limitation where it can only run one single simulation and cannot be reused in the same process. This can be a problem in certain contexts, such as when using Python Notebooks. To overcome this limitation, multiprocessing can be used to run the simulation in a separate process (not a thread) with its own memory space. The following option can be used to achieve this:
 
-    output = sim.start(True)
+    output = sim.start(start_new_process=True)
 
 When this option is used, the Geant4 engine will be created and run in a separate process, which will be terminated after the simulation is finished. The output of the simulation will be copied back to the main process that called the `start()` function. This allows for the use of Gate in Python Notebooks, as long as this option is not forgotten.
 
 For advanced usage, you can explicitly create the engine for the simulation with:
 
     se = gate.SimulationEngine(sim)
     se.start_new_process = True
```

### Comparing `opengate-10.0b7/docs/source/user_guide_2_1_volumes.md` & `opengate-10.0b8/docs/source/user_guide_2_1_volumes.md`

 * *Files 3% similar despite different names*

```diff
@@ -189,14 +189,37 @@
 1) An existing simulation (here `sim`)
 2) The density tolerance (in g/cm3)
 3) The path to a file containing a list of reference *materials*
 4) The path to a file containing a list of reference *densities*
 
 Examples of such files can be found in the `opengate/tests/data` folder. See test `test009` as example.
 
+
+### Tesselated (STL) volumes
+
+It is possible to create a tesselated volume shape based on an Standard Triangle Language (STL) data file. Such a file contains a mesh of triangles for one object. It is a typical output format of Computer Aided Design (CAD) software.
+To create such a volume add a volume of type "Tesselated". Please keep in mind, that no material information is provided, it has to be specified by the user. A Tesselated volume inherits the the same basic options as other solids described above such as translation or rotation. A basic example how to import an STL file into a geometry "MyTesselatedVolume" and assign the material G4_WATER to it can be found below. In order to verify the correct generation of the solid, one could look at the volume.
+
+
+```python
+import opengate as gate
+sim = gate.Simulation()
+tes = sim.add_volume("Tesselated", name="MyTesselatedVolume")
+tes.material = "G4_WATER"
+tes.mother = "world"  # by default
+tes.file_name = "myTesselatedVolume.stl"
+#to read the volume of the generated solid
+print("volume: ",sim.volume_manager.get_volume(
+        "MyTesselatedVolume"
+    ).solid_info.cubic_volume)
+#an alternative way read the volume of the generated solid
+print("same volume: ",tes.solid_info.cubic_volume)
+```
+See test test067_stl_volume for example.
+
 ### Repeated volumes
 
 The first method, described in this section, is controlled via the `translation` and `rotation` parameters. To instruct Geant4 to repeat a volume in multiple locations, it is sufficient to provide a list of translation vectors to the volume parameter `translation`. Gate will make sure that a G4PhysicalVolume is created for each entry. Consequently, the length of the list of translations determines the number of copies. If only a single rotation matrix is provided as volume parameter `rotation`, this will be used for all copies. If each copies requires a separate individual rotation, e.g. when repeating volume around a circle, then the volume parameter `rotation` should receive a list of rotation matrices. Obviously, the number of rotations and translation should match.
 
 Each volume copy corresponds to a G4PhysicalVolume in Geant4 with its own unique name. Gate automatically generates this name. It can be obtained from a given copy index (counting starts at 0) via the method `get_repetition_name_from_index()`. Or vice versa, the copy index can be obtained from the copy name via `get_repetition_index_from_name()`.
 
 Gate comes with utility functions to generate translation and rotation parameters for common types of volume repetitions - see below.
```

### Comparing `opengate-10.0b7/docs/source/user_guide_2_2_sources.md` & `opengate-10.0b8/docs/source/user_guide_2_2_sources.md`

 * *Files 20% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 ```python
 source = sim.add_source('Generic', 'Default')
 source.particle = 'e+'
 source.energy.type = 'F18'  # F18 or Ga68 or C11 ...
 ```
 
-It means the positrons will be generated following the (approximated) energy spectrum of the F18 ion. Source code is `GateSPSEneDistribution.cpp`. Energy spectrum for beta+ emitters are available : F18, Ga68, Zr89, Na22, C11, N13, O15, Rb82. See http://www.lnhb.fr/nuclear-data/module-lara. One example is available in `test031`.
+It means the positrons will be generated following the (approximated) energy spectrum of the F18 ion. Source code is `GateSPSEneDistribution.cpp`. Energy spectrum for beta+ emitters are available : F18, Ga68, Zr89, Na22, C11, N13, O15, Rb82. See [http://www.lnhb.fr/nuclear-data/module-lara](http://www.lnhb.fr/nuclear-data/module-lara). One example is available in `test031`.
 
 There is a `confine` option that allows to generate particles only if their starting position is within a given volume. See `phantom_nema_iec_body` in the contrib folder. Note that the source volume MUST be larger than the volume it is confined in. Also, note that no particle source will be generated in the daughters of the confine volume.
 
 All options have a default values and can be printed with `print(source)`.
 
 ### Voxelized sources
 
@@ -157,15 +157,15 @@
 Alternatively, by setting ```source.particle = None``` the particle type is read from the phase space file using the PDGCode. ```source.PDGCode_key = PDGCode``` specifies the name of the entry in the phase space file.
 Full listing:
 ```python
 source.PDGCode_key = "PDGCode"
 source.particle = None
 ```
 
-The PDGCode is defined by the particle data group (see https://pdg.lbl.gov/2023/web/viewer.html?file=../reviews/rpp2022-rev-monte-carlo-numbering.pdf).
+The PDGCode is defined by the particle data group (see [https://pdg.lbl.gov/2023/web/viewer.html?file=../reviews/rpp2022-rev-monte-carlo-numbering.pdf](https://pdg.lbl.gov/2023/web/viewer.html?file=../reviews/rpp2022-rev-monte-carlo-numbering.pdf)).
 Here is a short overview of common particle types and its corresponding PDG Code
 ```
 proton: 2212
 neutron: 2211
 electron: 11
 gamma: 22
 carbon ion C12: 1000060120
@@ -218,10 +218,87 @@
 - `test040` : GAN for PET
 
 1) generate training dataset
 2) train GAN
 3) use GAN as source ; compare to reference
 
 
+### PHID source (Photon from Ion Decay)
+
+PHID (Photon from Ion Decay) is a virtual source model that generates photons emitted in the complex decay chain process of alpha-emitter radionuclides, typically for use during simulation of SPECT image acquisition. Given an alpha-emitter radionuclide, the model extracts from Geant4 databases the photon emission lines from all decaying daughters for both isometric transition and atomic relaxation processes. According to a given time range, abundances and activities in the decay chain are considered thanks to the Bateman equations, taking into account the decay rates and the initial abundances. It generates photons with the correct energy and temporal distribution, avoiding the costly Monte Carlo simulation of the complete decay chain. Photons emitted from Bremsstrahlung are ignored, but are not significant for SPECT imaging. Also, the model is not expected to be correct for gammas below 20-30 keV.
+
+See Sarrut et al 2024 Phys. Med. Biol. [https://doi.org/10.1088/1361-6560/ad3881](https://doi.org/10.1088/1361-6560/ad3881)
+
+To use such a source, declare a "PhotonFromIonDecaySource" with an ion as particle name, like the "GenericSource". Only the gammas emitted by atomic relaxation and isomeric transition will be created and tracked. The timing is taken into account by using a TAC (Time Activity Curve) automatically computed from the start and end time of the simulation. The TAC is then binned and the number of bins can be modified. See tests 053.
+
+```python
+source = sim.add_source("PhotonFromIonDecaySource", "my_source")
+source.particle = f"ion 89 225"
+source.position.type = "sphere"
+source.position.radius = 1 * nm
+source.direction.type = "iso"
+source.activity = 10 * kBq
+source.atomic_relaxation_flag = True
+source.isomeric_transition_flag = True
+source.tac_bins = 200
+source.dump_log = "phid_log.txt"
+source.verbose = True
+```
+
+Also, several command lines tools are provided :
+
+```bash
+# print information about a radionuclide bi213, pb212, etc.
+phid_info ac225
+
+# plot time activity curve of a radionuclide. Options may by set to adapt the timing
+phid_tac
+
+# plot gammas lines from a radionuclide (whatever the time)
+phid_gammas ac225
+phid_atomic_relaxation ac225
+phid_isomeric_transition ac225
+```
+
+![image](figures/ac225_info.png)
+![image](figures/ac225_tac.png)
+![image](figures/ac225_gammas.png)
+
+
 ### Pencil Beam sources
 
-(documentation TODO), test044
+The Pencil Beam source inherits from the Generic source, and retains therefore the same settings.
+The main difference consists in the sampling of the position and direction of the particles, which are not sampled independently, but are correlated. In fact, the Pencil Beam source is meant to describe a beam that can converge or diverge. This behaviour is modeled according to the Fermi-Eyges theory (Techniques of Proton Radiotherapy: Transport Theory B. Gottschalk May 1, 2012), that describes the
+correlated momentum spread of the particle with 4 parameters (each for x and y direction, assuming a beam directed as z):
+- spot size  𝜎
+- divergence  𝜃
+- emittance  𝜀
+- convergence flag  [1,0]
+The parameters must satisfy the condition:
+```python
+pi * sigma * theta >= epsilon
+```
+![image](https://github.com/OpenGATE/opengate/assets/74096483/8b3d2077-b9e8-4d39-b027-3fa2089b597d)
+
+The user can set the beam parameters as shown in the example below, for a 120 MeV/n carbon ion beam.
+```python
+source = sim.add_source("IonPencilBeamSource", "mysource")
+source.energy.mono = 1440 * MeV
+source.particle = "ion 6 12"  # carbon
+source.position.translation = [100 * mm, 0 * mm, 0 * cm]
+source.n = 20000
+source.direction.partPhSp_x = [
+    2.3335754 * mm,
+    2.3335754 * mrad,
+    0.00078728 * mm * mrad,
+    0,
+]
+source.direction.partPhSp_y = [
+    1.96433431 * mm,
+    0.00079118 * mrad,
+    0.00249161 * mm * mrad,
+    0,
+]
+```
+NOTE: the Pencil Beam source is created by default directed as the positive z axis. To rotate the source, use the source.position.rotation option.
+
+Check all test044 for usage examples.
```

### Comparing `opengate-10.0b7/opengate/__init__.py` & `opengate-10.0b8/opengate/__init__.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/actions.py` & `opengate-10.0b8/opengate/actions.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/actors/actorbuilders.py` & `opengate-10.0b8/opengate/actors/actorbuilders.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 )
 from .miscactors import (
     MotionVolumeActor,
     SimulationStatisticsActor,
     SourceInfoActor,
     TestActor,
     KillActor,
+    BremSplittingActor,
+    ComptSplittingActor,
 )
+from .dynamicactors import DynamicGeometryActor
 from ..utility import make_builders
 
 
 actor_type_names = {
     SimulationStatisticsActor,
     DoseActor,
     FluenceActor,
@@ -37,9 +40,12 @@
     DigitizerSpatialBlurringActor,
     DigitizerEfficiencyActor,
     MotionVolumeActor,
     ARFActor,
     ARFTrainingDatasetActor,
     TestActor,
     KillActor,
+    BremSplittingActor,
+    ComptSplittingActor,
+    DynamicGeometryActor,
 }
 actor_builders = make_builders(actor_type_names)
```

### Comparing `opengate-10.0b7/opengate/actors/arfactors.py` & `opengate-10.0b8/opengate/actors/arfactors.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import itk
 import threading
 import opengate_core as g4
 from ..utility import g4_units, ensure_filename_is_str
 from ..exception import fatal
 from .digitizers import DigitizerHitsCollectionActor
 from .base import ActorBase
+from ..image import write_itk_image
 
 
 def import_garf():
     # Try to import torch
     try:
         import torch
     except:
@@ -293,14 +294,14 @@
         castImageFilter = itk.CastImageFilter[InputImageType, OutputImageType].New()
         castImageFilter.SetInput(self.output_image)
         castImageFilter.Update()
         self.output_image = castImageFilter.GetOutput()
 
         # write ?
         if self.user_info.output:
-            itk.imwrite(
+            write_itk_image(
                 self.output_image, ensure_filename_is_str(self.user_info.output)
             )
 
         # debug
         # print(f"{self.debug_nb_hits_before=}")
         # print(f"{self.debug_nb_hits=}")
```

### Comparing `opengate-10.0b7/opengate/actors/base.py` & `opengate-10.0b8/opengate/actors/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,23 +54,24 @@
         The engines (volume, actor, etc.) and G4 objects are also removed if exists.
         """
         if self.verbose_getstate:
             warning(
                 f"Getstate ActorBase {self.user_info.type_name} {self.user_info.name}"
             )
         # do not pickle engines and g4 objects
-        for v in self.__dict__:
-            if "_engine" in v or "g4_" in v:
-                self.__dict__[v] = None
+        for k in self.__dict__:
+            if "_engine" in k or "g4_" in k:
+                self.__dict__[k] = None
         try:
             self.__dict__["simulation"] = None
         except KeyError:
             print("No simulation to be removed while pickling Actor")
         # we remove the filter that trigger a pickle error
         # (to be modified)
+        # FIXME: the filters should implement their __getstate__ method to be pickleable
         self.filters_list = []
         return self.__dict__
 
     def initialize(self, simulation_engine_wr=None):
         self.simulation_engine_wr = simulation_engine_wr
         self.volume_engine = self.simulation_engine_wr().volume_engine
         if self.user_info.filters_boolean_operator not in ["and", "or"]:
```

### Comparing `opengate-10.0b7/opengate/actors/digitizers.py` & `opengate-10.0b8/opengate/actors/digitizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ..utility import g4_units, ensure_filename_is_str
 from ..image import (
     align_image_with_physical_volume,
     update_image_py_to_cpp,
     get_cpp_image,
     get_info_from_image,
     create_3d_image,
+    write_itk_image,
 )
 
 
 def ene_win_peak(name, energy, energy_width_percent):
     energy_width_percent = energy * energy_width_percent / 2
     e_min = energy - energy_width_percent
     e_max = energy + energy_width_percent
@@ -644,15 +645,15 @@
         if self.user_info.origin_as_image_center:
             origin = -info.size * info.spacing / 2.0 + info.spacing / 2.0
         spacing[2] = 1
         origin[2] = 0
         self.output_image.SetSpacing(spacing)
         self.output_image.SetOrigin(origin)
         if self.user_info.output:
-            itk.imwrite(
+            write_itk_image(
                 self.output_image, ensure_filename_is_str(self.user_info.output)
             )
 
 
 class DigitizerReadoutActor(g4.GateDigitizerReadoutActor, ActorBase):
     """
     This actor is a DigitizerAdderActor + a discretization step:
```

### Comparing `opengate-10.0b7/opengate/actors/doseactors.py` & `opengate-10.0b8/opengate/actors/doseactors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import itk
 import numpy as np
 import opengate_core as g4
 from .base import ActorBase
 from ..exception import fatal, warning
-from ..utility import g4_units, ensure_filename_is_str
+from ..utility import (
+    g4_units,
+    ensure_filename_is_str,
+    standard_error_c4_correction,
+)
 from ..image import (
     create_3d_image,
     align_image_with_physical_volume,
     update_image_py_to_cpp,
     create_image_like,
     get_info_from_image,
     get_origin_wrt_images_g4_position,
     get_cpp_image,
     itk_image_view_from_array,
     divide_itk_images,
+    scale_itk_image,
+    write_itk_image,
 )
+from ..geometry.materials import create_mass_img, create_density_img
 
 
 class DoseActor(g4.GateDoseActor, ActorBase):
     """
     DoseActor: compute a 3D edep/dose map for deposited
     energy/absorbed dose in the attached volume
 
@@ -50,26 +57,40 @@
         user_info.spacing = [1 * mm, 1 * mm, 1 * mm]
         user_info.output = "edep.mhd"  # FIXME change to 'output' ?
         user_info.translation = [0, 0, 0]
         user_info.img_coord_system = None
         user_info.output_origin = None
         user_info.uncertainty = True
         user_info.square = False
-        user_info.gray = False
         user_info.physical_volume_index = None
         user_info.hit_type = "random"
 
+        user_info.dose = False
+        user_info.to_water = False
+        user_info.use_more_ram = False
+        user_info.ste_of_mean = False
+        user_info.ste_of_mean_unbiased = False
+
+        # stop simulation when stat goal reached
+        user_info.goal_uncertainty = 0
+        user_info.thresh_voxel_edep_for_unc_calc = 0.7
+
+        user_info.dose_calc_on_the_fly = True  # dose calculation in stepping action c++
+
     def __init__(self, user_info):
         ActorBase.__init__(self, user_info)
+        if user_info.ste_of_mean_unbiased or user_info.ste_of_mean:
+            self.user_info.ste_of_mean = True
+            self.user_info.use_more_ram = True
         g4.GateDoseActor.__init__(self, user_info.__dict__)
         # attached physical volume (at init)
         self.g4_phys_vol = None
         # default image (py side)
         self.py_edep_image = None
-        self.py_dose_image = None
+        # self.py_dose_image = None
         self.py_temp_image = None
         self.py_square_image = None
         self.py_last_id_image = None
         # default uncertainty
         self.uncertainty_image = None
         # internal states
         self.img_origin_during_run = None
@@ -82,33 +103,68 @@
         return s
 
     def __getstate__(self):
         # superclass getstate
         ActorBase.__getstate__(self)
         # do not pickle itk images
         self.py_edep_image = None
-        self.py_dose_image = None
+        # self.py_dose_image = None
         self.py_temp_image = None
         self.py_square_image = None
         # self.py_last_id_image = None
         self.uncertainty_image = None
         return self.__dict__
 
     def initialize(self, volume_engine=None):
         """
         At the start of the run, the image is centered according to the coordinate system of
         the mother volume. This function computes the correct origin = center + translation.
         Note that there is a half-pixel shift to align according to the center of the pixel,
         like in ITK.
         """
+
+        if (
+            self.user_info.goal_uncertainty < 0.0
+            or self.user_info.goal_uncertainty > 1.0
+        ):
+            raise ValueError("goal uncertainty must be > 0 and < 1")
+
+        if self.user_info.ste_of_mean_unbiased:
+            self.user_info.ste_of_mean = True
+
+        if self.user_info.ste_of_mean:
+            self.user_info.use_more_RAM = True
+
+        if (
+            self.user_info.ste_of_mean == True
+            and self.simulation.user_info.number_of_threads <= 4
+        ):
+            raise ValueError(
+                "number_of_threads should be > 4 when using dose actor with ste_of_mean flag enabled"
+            )
+
+        if self.user_info.goal_uncertainty:
+            if (
+                self.user_info.uncertainty == False
+                and self.user_info.ste_of_mean == False
+            ):
+                raise ValueError(
+                    "To set an uncertainty goal, set at least one of this flags to True: uncertainty, ste_of_mean"
+                )
+
+        if self.user_info.uncertainty == True and self.user_info.ste_of_mean == True:
+            raise ValueError(
+                "select only one way to calculate uncertainty: uncertainty or ste_of_mean"
+            )
+
         super().initialize(volume_engine)
         # create itk image (py side)
         size = np.array(self.user_info.size)
         spacing = np.array(self.user_info.spacing)
-        self.py_edep_image = create_3d_image(size, spacing)
+        self.py_edep_image = create_3d_image(size, spacing, pixel_type="double")
         # compute the center, using translation and half pixel spacing
         self.img_origin_during_run = (
             -size * spacing / 2.0 + spacing / 2.0 + self.user_info.translation
         )
         # for initialization during the first run
         self.first_run = True
 
@@ -142,25 +198,24 @@
         # FIXME for multiple run and motion
         if not self.first_run:
             warning(f"Not implemented yet: DoseActor with several runs")
         # send itk image to cpp side, copy data only the first run.
         update_image_py_to_cpp(self.py_edep_image, self.cpp_edep_image, self.first_run)
 
         # for uncertainty and square dose image
-        if self.user_info.uncertainty or self.user_info.square:
-            self.py_square_image = create_image_like(self.py_edep_image)
-            update_image_py_to_cpp(
-                self.py_square_image, self.cpp_square_image, self.first_run
+        if (
+            self.user_info.uncertainty
+            or self.user_info.square
+            or self.user_info.ste_of_mean
+        ):
+            self.py_square_image = create_image_like(
+                self.py_edep_image, pixel_type="double"
             )
-
-        # for dose in Gray
-        if self.user_info.gray:
-            self.py_dose_image = create_image_like(self.py_edep_image)
             update_image_py_to_cpp(
-                self.py_dose_image, self.cpp_dose_image, self.first_run
+                self.py_square_image, self.cpp_square_image, self.first_run
             )
 
         # now, indicate the next run will not be the first
         self.first_run = False
 
         # If attached to a voxelized volume, we may want to use its coord system.
         # So, we compute in advance what will be the final origin of the dose map
@@ -206,83 +261,165 @@
         # Currently a copy. Maybe later as_pyarray ?
         self.py_edep_image = get_cpp_image(self.cpp_edep_image)
 
         # set the property of the output image:
         # in the coordinate system of the attached volume
         # FIXME no direction for the moment ?
         self.py_edep_image.SetOrigin(self.output_origin)
+        self.user_info.output = self.simulation.get_output_path(self.user_info.output)
+
+        # dose in gray
+        if self.user_info.dose:
+            self.user_info.output = self.simulation.get_output_path(
+                self.user_info.output, suffix="dose"
+            )
+            if not self.user_info.dose_calc_on_the_fly:
+                self.user_info.output = self.simulation.get_output_path(
+                    self.user_info.output, suffix="postprocessing"
+                )
+
+        else:
+            self.user_info.output = self.simulation.get_output_path(
+                self.user_info.output, suffix="edep"
+            )
+
+        if self.user_info.to_water:
+            self.user_info.output = self.simulation.get_output_path(
+                self.user_info.output, suffix="ToWater"
+            )
+
         # Uncertainty stuff need to be called before writing edep (to terminate temp events)
-        out_p = ensure_filename_is_str(
-            self.simulation.get_output_path(self.user_info.output)
-        )
-        if self.user_info.uncertainty:
-            self.compute_uncertainty()
-            n = out_p.replace(".mhd", "_uncertainty.mhd")
-            itk.imwrite(self.uncertainty_image, n)
+        if self.user_info.uncertainty or self.user_info.ste_of_mean:
+            self.create_uncertainty_img()
+            self.user_info.output_uncertainty = self.simulation.get_output_path(
+                self.user_info.output, suffix="uncertainty"
+            )
+            write_itk_image(self.uncertainty_image, self.user_info.output_uncertainty)
 
         # Write square image too
         if self.user_info.square:
-            self.compute_square()
-            n = out_p.replace(".mhd", "-Squared.mhd")
-            itk.imwrite(self.py_square_image, n)
+            self.fetch_square_image_from_cpp()
+            n = self.simulation.get_output_path(self.user_info.output, suffix="Squared")
+            write_itk_image(self.py_square_image, n)
 
-        # dose in gray
-        if self.user_info.gray:
-            self.py_dose_image = get_cpp_image(self.cpp_dose_image)
-            self.py_dose_image.SetOrigin(self.output_origin)
-            n = out_p.replace(".mhd", "_dose.mhd")
-            itk.imwrite(self.py_dose_image, n)
+        if not self.user_info.dose_calc_on_the_fly and self.user_info.dose:
+            self.compute_dose_from_edep_img()
 
         # write the image at the end of the run
         # FIXME : maybe different for several runs
         if self.user_info.output:
-            itk.imwrite(self.py_edep_image, out_p)
+            write_itk_image(self.py_edep_image, self.user_info.output)
 
-    def compute_square(self):
+    def compute_dose_from_edep_img(self):
+        """
+        * create mass image:
+            - from ct HU units, if dose actor attached to ImageVolume.
+            - from material density, if standard volume
+        * compute dose as edep_image /  mass_image
+        """
+        vol = self.simulation.volume_manager.get_volume(self.user_info.mother)
+        spacing = np.array(self.user_info.spacing)
+        voxel_volume = spacing[0] * spacing[1] * spacing[2]
+        Gy = g4_units.Gy
+        gcm3 = g4_units.g_cm3
+
+        if vol.volume_type == "ImageVolume":
+            material_database = (
+                self.simulation.volume_manager.material_database.g4_materials
+            )
+            if self.user_info.to_water:
+                # for dose to water, divide by density of water and not density of material
+                self.py_edep_image = scale_itk_image(
+                    self.py_edep_image, 1 / (1.0 * gcm3)
+                )
+            else:
+                density_img = create_density_img(vol, material_database)
+                self.py_edep_image = divide_itk_images(
+                    img1_numerator=self.py_edep_image,
+                    img2_denominator=density_img,
+                    filterVal=0,
+                    replaceFilteredVal=0,
+                )
+            # divide by voxel volume and convert unit
+            self.py_edep_image = scale_itk_image(
+                self.py_edep_image, 1 / (Gy * voxel_volume)
+            )
+
+        else:
+            if self.user_info.to_water:
+                # for dose 2 water, divide by density of water and not density of material
+                density = 1.0 * gcm3
+            else:
+                density = vol.g4_material.GetDensity()
+            self.py_edep_image = scale_itk_image(
+                self.py_edep_image, 1 / (voxel_volume * density * Gy)
+            )
+
+    def fetch_square_image_from_cpp(self):
         if self.py_square_image == None:
             self.py_square_image = get_cpp_image(self.cpp_square_image)
             self.py_square_image.SetOrigin(self.output_origin)
             self.py_square_image.CopyInformation(self.py_edep_image)
 
-    def compute_uncertainty(self):
-        NbOfEvent = self.NbOfEvent
-        self.compute_square()
+    def compute_std_from_sample(self, N, val, val_squared, correct_bias=False):
+        unc = np.ones_like(val)
+        if N > 1:
+            # unc = np.sqrt(1 / (N - 1) * (square / N - np.power(edep / N, 2)))
+            unc = 1 / (N - 1) * (val_squared / N - np.power(val / N, 2))
+            unc = np.ma.masked_array(
+                unc, unc < 0
+            )  # this function leaves unc<0 values untouched! what do we do with < 0 values?
+            unc = np.ma.sqrt(unc)
+            if correct_bias:
+                """Standard error is biased (to underestimate the error); this option allows to correct for the bias - assuming normal distribution. For few N this influence is huge, but for N>8 the difference is minimal"""
+                unc /= standard_error_c4_correction(N)
+            unc = np.divide(unc, val / N, out=np.ones_like(unc), where=val != 0)
+
+        else:
+            # unc += 1 # we init with 1.
+            warning(
+                "You try to compute statistical errors with only one or zero event ! The uncertainty value for all voxels has been fixed at 1"
+            )
+        return unc
+
+    def create_uncertainty_img(self):
+        N = self.NbOfEvent
+        if self.user_info.ste_of_mean:
+            """
+            Standard error of mean, where each thread is considered one subsample.
+            """
+            N = self.simulation.user_info.number_of_threads
+
+        self.fetch_square_image_from_cpp()
 
         edep = itk.array_view_from_image(self.py_edep_image)
         square = itk.array_view_from_image(self.py_square_image)
 
         self.py_edep_image_tmp = itk_image_view_from_array(edep)
         self.py_edep_image_tmp.CopyInformation(self.py_edep_image)
         self.py_edep_image = self.py_edep_image_tmp
         del self.py_edep_image_tmp
 
         # uncertainty image
-        self.uncertainty_image = create_image_like(self.py_edep_image)
-        unc = itk.array_view_from_image(self.uncertainty_image)
-        N = NbOfEvent
-        if N != 1:
-            # unc = np.sqrt(1 / (N - 1) * (square / N - np.power(edep / N, 2)))
-            unc = 1 / (N - 1) * (square / N - np.power(edep / N, 2))
-            unc = np.ma.masked_array(unc, unc < 0)
-            unc = np.ma.sqrt(unc)
-            unc = np.divide(unc, edep / N, out=np.ones_like(unc), where=edep != 0)
+        self.uncertainty_image = create_image_like(
+            self.py_edep_image, pixel_type="double"
+        )
+        # unc = itk.array_view_from_image(self.uncertainty_image)
 
-        else:
-            unc += 1
-            warning(
-                "You try to compute statistical errors with only one event ! The uncertainty value for all voxels has been fixed at 1"
-            )
+        unc = self.compute_std_from_sample(
+            N, edep, square, correct_bias=self.user_info.ste_of_mean_unbiased
+        )
         self.uncertainty_image = itk_image_view_from_array(unc)
         self.uncertainty_image.CopyInformation(self.py_edep_image)
         self.uncertainty_image.SetOrigin(self.output_origin)
         # debug
-        """itk.imwrite(self.py_square_image, "square.mhd")
-        itk.imwrite(self.py_temp_image, "temp.mhd")
-        itk.imwrite(self.py_last_id_image, "lastid.mhd")
-        itk.imwrite(self.uncertainty_image, "uncer.mhd")"""
+        """write_itk_image(self.py_square_image, "square.mhd")
+        write_itk_image(self.py_temp_image, "temp.mhd")
+        write_itk_image(self.py_last_id_image, "lastid.mhd")
+        write_itk_image(self.uncertainty_image, "uncer.mhd")"""
 
 
 class LETActor(g4.GateLETActor, ActorBase):
     """
     LETActor: compute a 3D edep/dose map for deposited
     energy/absorbed dose in the attached volume
 
@@ -428,15 +565,17 @@
         self.py_denominator_image = create_image_like(
             self.py_numerator_image, pixel_type="double"
         )
         update_image_py_to_cpp(
             self.py_denominator_image, self.cpp_denominator_image, self.first_run
         )
 
-        self.py_output_image = create_image_like(self.py_numerator_image)
+        self.py_output_image = create_image_like(
+            self.py_numerator_image, pixel_type="double"
+        )
 
         # now, indicate the next run will not be the first
         self.first_run = False
 
         # If attached to a voxelized volume, we may want to use its coord system.
         # So, we compute in advance what will be the final origin of the dose map
         vol = self.simulation.volume_manager.volumes[self.user_info.mother]
@@ -502,22 +641,26 @@
             # self.output = fPath
             self.py_LETd_image = divide_itk_images(
                 img1_numerator=self.py_numerator_image,
                 img2_denominator=self.py_denominator_image,
                 filterVal=0,
                 replaceFilteredVal=0,
             )
-            itk.imwrite(self.py_LETd_image, ensure_filename_is_str(fPath))
+            write_itk_image(self.py_LETd_image, fPath)
 
             # for parallel computation we need to provide both outputs
             if self.user_info.separate_output:
-                fPath = fPath.replace(".mhd", "_numerator.mhd")
-                itk.imwrite(self.py_numerator_image, ensure_filename_is_str(fPath))
-                fPath = fPath.replace("_numerator", "_denominator")
-                itk.imwrite(self.py_denominator_image, ensure_filename_is_str(fPath))
+                fPath = self.simulation.get_output_path(
+                    self.user_info.output, suffix="numerator"
+                )
+                write_itk_image(self.py_numerator_image, fPath)
+                fPath = self.simulation.get_output_path(
+                    self.user_info.output, suffix="denominator"
+                )
+                write_itk_image(self.py_denominator_image, fPath)
 
 
 class FluenceActor(g4.GateFluenceActor, ActorBase):
     """
     FluenceActor: compute a 3D map of fluence
 
     FIXME: add scatter order and uncertainty
```

### Comparing `opengate-10.0b7/opengate/actors/filters.py` & `opengate-10.0b8/opengate/actors/filters.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/actors/miscactors.py` & `opengate-10.0b8/opengate/actors/miscactors.py`

 * *Files 13% similar despite different names*

```diff
@@ -423,7 +423,57 @@
 
     def set_default_user_info(user_info):
         ActorBase.set_default_user_info(user_info)
 
     def __init__(self, user_info):
         ActorBase.__init__(self, user_info)
         g4.GateKillActor.__init__(self, user_info.__dict__)
+
+
+"""
+class ComptonSplittingActor(g4.GateComptonSplittingActor,ActorBase):
+    type_name = "ComptonSplittingActor"
+    def set_default_user_info(user_info):
+        ActorBase.set_default_user_info(user_info)
+        user_info.SplittingFactor = 0
+
+    def __init__(self, user_info):
+        ActorBase.__init__(self, user_info)
+        g4.GateComptonSplittingActor.__init__(self, user_info.__dict__)
+"""
+
+
+class ComptSplittingActor(g4.GateOptrComptSplittingActor, ActorBase):
+    type_name = "ComptSplittingActor"
+
+    def set_default_user_info(user_info):
+        ActorBase.set_default_user_info(user_info)
+        deg = g4_units.deg
+        user_info.splitting_factor = 1
+        user_info.weight_threshold = 0
+        user_info.bias_primary_only = True
+        user_info.min_weight_of_particle = 0
+        user_info.bias_only_once = True
+        user_info.processes = ["compt"]
+        user_info.russian_roulette = False
+        user_info.rotation_vector_director = False
+        user_info.vector_director = [0, 0, 1]
+        user_info.max_theta = 90 * deg
+
+    def __init__(self, user_info):
+        ActorBase.__init__(self, user_info)
+        g4.GateOptrComptSplittingActor.__init__(self, user_info.__dict__)
+
+
+class BremSplittingActor(g4.GateBOptrBremSplittingActor, ActorBase):
+    type_name = "BremSplittingActor"
+
+    def set_default_user_info(user_info):
+        ActorBase.set_default_user_info(user_info)
+        user_info.splitting_factor = 1
+        user_info.bias_primary_only = True
+        user_info.bias_only_once = True
+        user_info.processes = ["eBrem"]
+
+    def __init__(self, user_info):
+        ActorBase.__init__(self, user_info)
+        g4.GateBOptrBremSplittingActor.__init__(self, user_info.__dict__)
```

### Comparing `opengate-10.0b7/opengate/base.py` & `opengate-10.0b8/opengate/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from .exception import fatal, warning
 from .definitions import (
     __gate_list_objects__,
     __gate_dictionary_objects__,
     __one_indent__,
 )
+from .decorators import requires_fatal
+from .logger import log
 
 
 # META CLASSES
 class MetaUserInfo(type):
     _created_classes = {}
 
     def __call__(cls, *args, **kwargs):
@@ -244,32 +246,40 @@
     """
 
     def __new__(cls, *args, **kwargs):
         new_instance = super(GateObjectClass, cls).__new__(cls)
         return new_instance
 
     def __init__(self, *args, **kwargs):
-        self.user_info = Box()
+        # prefill user info with defaults
+        self.user_info = Box(
+            [
+                (k, copy.deepcopy(v[0]))
+                for k, v in self.inherited_user_info_defaults.items()
+            ]
+        )
+        # now iterate over them and check if kwargs provide user-specific values
         for k, v in self.inherited_user_info_defaults.items():
             default_value = v[0]
             options = v[1]
             if k in kwargs:
                 # if "check_func" in options.keys():
                 #     user_info_value = options["check_func"](kwargs[k])
                 # else:
                 user_info_value = kwargs[k]
                 # check_property(k, user_info_value, default_value)
+                if "setter_hook" in options:
+                    user_info_value = options["setter_hook"](self, user_info_value)
+                self.user_info[k] = user_info_value
                 kwargs.pop(k)
             else:
                 if "required" in options.keys() and options["required"] is True:
                     fatal(
                         f"No value provided for argument '{k}', but required when constructing a {type(self).__name__} object."
                     )
-                user_info_value = copy.deepcopy(default_value)
-            self.user_info[k] = user_info_value
         super(GateObjectClass, self).__init__()
 
     def __str__(self):
         ret_string = (
             f"***\n"
             f"{type(self).__name__} named {self.name} "
             f"with the following parameters:\n"
@@ -277,44 +287,55 @@
         for k, v in self.user_info.items():
             if k != "name":
                 ret_string += f"{__one_indent__}{k}:\n{2*__one_indent__}{v}\n"
         ret_string += "***\n"
         return ret_string
 
     def __getstate__(self):
-        """Method needed for pickling. Maybe be overridden in inheriting classes."""
+        """Method needed for pickling. May be be overridden in inheriting classes."""
         return self.__dict__
 
     def __setstate__(self, d):
-        """Method needed for pickling. Maybe be overridden in inheriting classes."""
+        """Method needed for pickling. May be be overridden in inheriting classes."""
         self.__dict__ = d
 
     def __reduce__(self):
         """This method is called when the object is pickled.
         Usually, pickle works well without this custom __reduce__ method,
-        but object handling user_infos need a custom __reduce__ to make sure
+        but objects handling user_infos need a custom __reduce__ to make sure
         the properties linked to the user_infos are properly created as per the meta class
 
         The return arguments are:
         1) A callable used to create the instance when unpickling
         2) A tuple of arguments to be passed to the callable in 1
         3) The dictionary of the objects properties to be passed to the __setstate__ method (if defined)
         """
+        state_dict = self.__getstate__()
         return (
             restore_userinfo_properties,
-            (self.__class__, self.__getstate__()),
-            self.__getstate__(),
+            (self.__class__, state_dict),
+            state_dict,
         )
 
+    def close(self):
+        """Dummy implementation for inherited classes which do not implement this method."""
+        pass
+
+    def release_g4_references(self):
+        """Dummy implementation for inherited classes which do not implement this method."""
+        pass
+
     GateObjectClass.__new__ = __new__
     GateObjectClass.__init__ = __init__
     GateObjectClass.__str__ = __str__
     GateObjectClass.__getstate__ = __getstate__
     GateObjectClass.__setstate__ = __setstate__
     GateObjectClass.__reduce__ = __reduce__
+    GateObjectClass.close = close
+    GateObjectClass.release_g4_references = release_g4_references
 
 
 # GateObject classes
 class GateObjectSingleton(metaclass=MetaUserInfoSingleton):
     user_info_defaults = {
         "name": (
             None,
@@ -325,15 +346,15 @@
 
 attach_methods(GateObjectSingleton)
 
 
 class GateObject(metaclass=MetaUserInfo):
     user_info_defaults = {"name": (None, {"required": True})}
 
-    def clone_user_info(self, other_obj):
+    def copy_user_info(self, other_obj):
         for k in self.user_info.keys():
             if k not in ["name", "_name"]:
                 try:
                     self.user_info[k] = other_obj.user_info[k]
                 except KeyError:
                     pass
 
@@ -373,14 +394,117 @@
                         f"Could not find user info {k} while populating object {self.name} of type {type(self).__name__} from dictionary."
                     )
 
 
 attach_methods(GateObject)
 
 
+class DynamicGateObject(GateObject):
+    user_info_defaults = {
+        "dynamic_params": (
+            None,
+            {
+                "doc": "List of dictionaries, where each dictionary specifies how the parameters "
+                "of this object should evolve over time during the simulation. "
+                "If None, the object is static (default).",
+                "read_only": True,
+            },
+        )
+    }
+
+    @property
+    def is_dynamic(self):
+        if self.dynamic_params is None:
+            return False
+        elif len(self.dynamic_params) == 0:
+            return False
+        else:
+            return True
+
+    @property
+    def dynamic_user_info(self):
+        return [
+            k
+            for k in self.user_info
+            if "dynamic" in self.inherited_user_info_defaults[k][1]
+            and self.inherited_user_info_defaults[k][1]["dynamic"] is True
+        ]
+
+    @requires_fatal("simulation")
+    def process_dynamic_parametrisation(self, params):
+        # create a dictionary to store params which to not correspond to dynamic user info
+        # i.e. extra parameters for auxiliary purpose
+        extra_params = {}
+        extra_params["auto_changer"] = params.pop(
+            "auto_changer", True
+        )  # True of key not found (default)
+        if extra_params["auto_changer"] not in (False, True):
+            fatal(
+                f"Received wrong value type for 'auto_changer': got {type(extra_params['auto_changer'])}, "
+                f"expected: True or False."
+            )
+        for k in set(params).difference(set(self.dynamic_user_info)):
+            extra_params[k] = params.pop(k)
+        # apply params which are functions to the timing intervals of the simulation to get the sample quantities
+        for k, v in params.items():
+            if callable(v):
+                params[k] = v(self.simulation.run_timing_intervals)
+        # check that the length of all parameter lists match the simulation's timing intervals
+        params_with_incorrect_length = []
+        for k, v in params.items():
+            if len(v) != len(self.simulation.run_timing_intervals):
+                params_with_incorrect_length.append((k, len(v)))
+        if len(params_with_incorrect_length) > 0:
+            s = (
+                f"The length of the following dynamic parameters "
+                f"does not match the number of timing intervals of the simulation:\n"
+            )
+            for p in params_with_incorrect_length:
+                s += f"{p[0]}: {p[1]}\n"
+            s += (
+                f"The simulation's timing intervals are: {self.simulation.run_timing_intervals} and "
+                f"can be adjusted via the simulation parameter 'run_timing_intervals'. "
+            )
+            fatal(s)
+        return params, extra_params
+
+    def _add_dynamic_parametrisation_to_userinfo(self, params, name):
+        """This base class implementation only acts as a setter.
+        Classes inheriting from this class should implement an
+        add_dynamic_parametrisation() method which actually does something
+        with the parameters and then call super().add_dynamic_parametrisation().
+        Inheriting classes should avoid calling this method directly.
+        """
+        if name not in self.user_info["dynamic_params"]:
+            self.user_info["dynamic_params"][name] = params
+        else:
+            fatal(
+                f"A dynamic parametrisation with name {name} already exists in volume '{self.name}'."
+            )
+
+    def add_dynamic_parametrisation(self, name=None, **params):
+        if self.user_info["dynamic_params"] is None:
+            self.user_info["dynamic_params"] = {}
+        processed_params, extra_params = self.process_dynamic_parametrisation(params)
+        processed_params["extra_params"] = extra_params
+        # if user provided no name, create one
+        if name is None:
+            name = f"parametrisation_{len(self.dynamic_params)}"
+        self._add_dynamic_parametrisation_to_userinfo(processed_params, name)
+        # issue debugging message
+        s = f"Added the folowing dynamic parametrisation to {type(self).__name__} '{self.name}': \n"
+        for k, v in processed_params.items():
+            s += f"{k}: {v}\n"
+        log.debug(s)
+
+    def create_changers(self):
+        # this base class implementation is here to keep inheritance intact.
+        return []
+
+
 # DICTIONARY HANDLING
 def recursive_userinfo_to_dict(obj):
     """Walk recursively across entries of user_info and convert to appropriate structure.
     Dictionary-like structures are mapped to dictionary and walked across recursively.
     List-like structures are mapped to lists and walked across recursively.
     GateObject-like objects are converted through their to_dictionary() method.
     All other input (presumably common data types including numpy structures) is left untouched.
```

### Comparing `opengate-10.0b7/opengate/bin/dose_rate` & `opengate-10.0b8/opengate/bin/dose_rate.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/bin/ideal_timed_spect_reconstruction.py` & `opengate-10.0b8/opengate/bin/ideal_timed_spect_reconstruction.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import gatetools
 import click
 import itk
 import numpy as np
 import os
 import scipy
+from ..image import write_itk_image
 
 
 def compute_positions(phsp, keys, e_min):
     # get speed of light in mm/s
     c = scipy.constants.speed_of_light * 1000  # in mm
 
     # loop on x ; check energy
@@ -110,13 +111,13 @@
     # create the image
     a = np.zeros(size)
     for x in pix:
         a[x[0], x[1], x[2]] += 1
     img = itk.image_from_array(a)
     img.SetSpacing(spacing.tolist())
     img.SetOrigin(offset)
-    itk.imwrite(img, output)
+    write_itk_image(img, output)
 
 
 # --------------------------------------------------------------------------
 if __name__ == "__main__":
     go()
```

### Comparing `opengate-10.0b7/opengate/bin/opengate_tests` & `opengate-10.0b8/opengate/bin/opengate_tests.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/bin/opengate_tests_utils` & `opengate-10.0b8/opengate/bin/opengate_library_path.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 
 # -----------------------------------------------------------------------------
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.option("--path", "-p", default="", help="Path", required=True)
-def utils_paths(path):
+def go(path):
     """
     Tool to have the path of folders
     """
     if path == "libG4processes":
         get_libG4processes_path()
     elif path == "libG4geometry":
         get_libG4geometry_path()
     elif path == "site_packages":
         get_site_packages_dir()
 
 
 # -----------------------------------------------------------------------------
 if __name__ == "__main__":
-    utils_paths()
+    go()
```

### Comparing `opengate-10.0b7/opengate/bin/opengate_user_info` & `opengate-10.0b8/opengate/bin/opengate_user_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     for element in user_info.__dict__:
         val = str(user_info.__dict__[element])
         val = val.replace("\n", "")
         print(f"    {element:<25}     {val}")
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
-def opengate_user_info():
+def go():
     """
     Print information about all available user parameters
     """
 
     print()
     print(f"Volumes")
     print()
@@ -41,8 +41,8 @@
     print(f"Actors")
     print()
     for v in actor_type_names:
         print_one(v, "Actor")
 
 
 if __name__ == "__main__":
-    opengate_user_info()
+    go()
```

### Comparing `opengate-10.0b7/opengate/bin/opengate_visu` & `opengate-10.0b8/opengate/bin/opengate_visu.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/bin/split_spect_projections` & `opengate-10.0b8/opengate/bin/split_spect_projections.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/bin/voxelize_iec_phantom` & `opengate-10.0b8/opengate/bin/voxelize_iec_phantom.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/contrib/GateMaterials.db` & `opengate-10.0b8/opengate/contrib/GateMaterials.db`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/contrib/beamlines/ionbeamline.py` & `opengate-10.0b8/opengate/contrib/beamlines/ionbeamline.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/contrib/dose/dose_rate_test1.json` & `opengate-10.0b8/opengate/contrib/dose/dose_rate_test1.json`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/contrib/dose/doserate.py` & `opengate-10.0b8/opengate/contrib/dose/doserate.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,19 @@
     - radionuclide
     - activity_bq
     """
     # create the simulation
     sim = Simulation()
 
     # main options
-    ui = sim.user_info
-    ui.g4_verbose = False
-    ui.visu = param.visu
-    ui.visu_type = "vrml"
-    ui.number_of_threads = param.number_of_threads
-    ui.verbose_level = INFO
+    sim.g4_verbose = False
+    sim.visu = param.visu
+    sim.visu_type = "vrml"
+    sim.number_of_threads = param.number_of_threads
+    sim.verbose_level = INFO
 
     param.output_folder = pathlib.Path(param.output_folder)
 
     # units
     m = g4_units.m
     mm = g4_units.mm
     keV = g4_units.keV
@@ -44,21 +43,21 @@
     gcm3 = g4_units.g_cm3
 
     #  change world size
     world = sim.world
     world.size = [2 * m, 2 * m, 2 * m]
 
     # CT image
-    if ui.visu:
+    if sim.visu:
         ct = sim.add_volume("Box", "ct")
         info = read_image_info(param.ct_image)
         ct.size = info.size
         ct.material = "G4_WATER"
         ct.color = [0, 0, 1, 1]
-        ui.number_of_threads = 1
+        sim.number_of_threads = 1
     else:
         ct = sim.add_volume("Image", "ct")
         ct.image = param.ct_image
         ct.material = "G4_AIR"  # material used by default
         tol = param.density_tolerance_gcm3 * gcm3
         ct.voxel_materials, materials = HounsfieldUnit_to_material(
             sim, tol, param.table_mat, param.table_density
@@ -82,15 +81,15 @@
 
     # Activity source from an image
     source = sim.add_source("VoxelsSource", "vox")
     source.mother = ct.name
     source.particle = "ion"
     source.ion.Z = rad_list[param.radionuclide]["Z"]
     source.ion.A = rad_list[param.radionuclide]["A"]
-    source.activity = param.activity_bq * Bq / ui.number_of_threads
+    source.activity = param.activity_bq * Bq / sim.number_of_threads
     source.image = param.activity_image
     source.direction.type = "iso"
     source.energy.mono = 0 * keV
     # compute the translation to align the source with CT
     # (considering they are in the same physical space)
     source.position.translation = get_translation_between_images_center(
         param.ct_image, param.activity_image
@@ -108,15 +107,15 @@
     dose.output = param.output_folder / "edep.mhd"
     dose.mother = ct.name
     dose.size = source_info.size
     dose.spacing = source_info.spacing
     # translate the dose the same way as the source
     dose.translation = source.position.translation
     # set the origin of the dose like the source
-    if not ui.visu:
+    if not sim.visu:
         dose.img_coord_system = True
     dose.hit_type = "random"
     dose.uncertainty = False
 
     # add stat actor
     stats = sim.add_actor("SimulationStatisticsActor", "Stats")
     stats.track_types_flag = True
```

### Comparing `opengate-10.0b7/opengate/contrib/linacs/elekta_synergy_materials.db` & `opengate-10.0b8/opengate/contrib/linacs/elekta_synergy_materials.db`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/contrib/linacs/modified_elekta_synergy_materials.db` & `opengate-10.0b8/opengate/contrib/linacs/elekta_versa_materials.db`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/contrib/pet/siemens_biograph_materials.db` & `opengate-10.0b8/opengate/contrib/pet/siemens_biograph_materials.db`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/contrib/pet/siemensbiograph.py` & `opengate-10.0b8/opengate/contrib/pet/siemensbiograph.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/contrib/phantoms/necr.py` & `opengate-10.0b8/opengate/contrib/phantoms/necr.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 
 def add_necr_source_debug(sim, name):
     """
     The source is described according to the world
     """
 
     mm = g4_units.mm
-    cm = g4_units.cm
     MeV = g4_units.MeV
     src = sim.add_source("GenericSource", name)
 
     src.particle = "gamma"
     src.energy.type = "mono"
     src.energy.mono = 0.511 * MeV
     src.position.type = "sphere"
```

### Comparing `opengate-10.0b7/opengate/contrib/phantoms/nemaiec.py` & `opengate-10.0b8/opengate/contrib/phantoms/nemaiec.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
     # 21.4/2 = 10.7 interior height (top_interior)
     h = 21.4 / 2 * cm - thickness_z
     cap.dz = (h - h_relative - rad - sph_thick) / 2.0
     cap.translation[2] = h_relative + rad + sph_thick + cap.dz
 
     # capillary outer shell
     caps = sim.add_volume("Tubs", f"{name}_capillary_shell_{d}")
-    caps.clone_user_info(cap)
+    caps.copy_user_info(cap)
     caps.material = iec_plastic
     caps.rmax = cap_thick
     caps.rmin = cap.rmax
 
 
 def add_spheres_sources(
     simulation,
@@ -376,16 +376,14 @@
     source.particle = "e+"
     source.energy.type = "F18"
     source.direction.type = "iso"
     source.activity = activity_Bq_mL * s.cubic_volume
     source.position.type = "sphere"
     source.position.radius = diameter / 2 * mm
     source.position.translation = [0, 0, 0]
-    # print(f"Sphere volume {s.cubic_volume} cc")
-
     return source
 
 
 def add_central_cylinder_source(
     simulation, iec_name, src_name, activity_Bq_mL, verbose=False
 ):
     # source
```

### Comparing `opengate-10.0b7/opengate/contrib/spect/genm670.py` & `opengate-10.0b8/opengate/contrib/spect/ge_discovery_nm670.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import pathlib
-from opengate.exception import fatal
-from opengate.utility import g4_units
 from opengate.managers import Simulation
 from opengate.geometry.volumes import RepeatParametrisedVolume, HexagonVolume
 from opengate.geometry.utility import (
     translate_point_to_volume,
     get_transform_orbiting,
     vec_g4_as_np,
 )
+from opengate.actors.digitizers import *
 from scipy.spatial.transform import Rotation
 from box import Box
 
 
 def get_collimator(rad):
-    radionuclides = ["Tc99m", "Lu177", "In111", "I131"]
+    radionuclides = ["tc99m", "lu177", "in111", "i131"]
     ref_collimators = ["lehr", "megp", "megp", "hegp"]
+    rad = rad.lower()
     if rad not in radionuclides:
         fatal(f'The radionuclide "{rad}" is unknown. Known are: {radionuclides}')
     return ref_collimators[radionuclides.index(rad)]
 
 
-def add_ge_nm67_fake_spect_head(sim, name="spect"):
+def add_fake_spect_head(sim, name="spect"):
     white = [1, 1, 1, 1]
     cm = g4_units.cm
     spect_length = 19 * cm
     head = sim.add_volume("Box", name)
     head.material = "G4_AIR"
     head.size = [57.6 * cm, 44.6 * cm, spect_length]
     head.color = white
     return head
 
 
-def get_orientation_for_CT(colli_type, table_shift, radius):
+def get_orientation_for_ct(colli_type, table_shift, radius):
     nm = g4_units.nm
     pos, crystal_distance, psdd = get_plane_position_and_distance_to_crystal(colli_type)
     pos += 1 * nm
     p = [0, table_shift, -(radius + psdd)]
     return get_transform_orbiting(p, "x", 90)
 
 
-def add_ge_nm67_spect_head(sim, name="spect", collimator_type="lehr", debug=False):
+def add_spect_head(sim, name="spect", collimator_type="lehr", debug=False):
     """
     Collimators:
     - False : no collimator
     - lehr : holes length 35 mm, diam 1.5 mm, septal thickness : 0.2 mm
     - megp : holes length 58 mm, diam 3 mm,   septal thickness : 1.05 mm
     - hegp : holes length 66 mm, diam 4 mm,   septal thickness : 1.8 mm
 
@@ -57,36 +57,37 @@
     if fdb not in sim.volume_manager.material_database.filenames:
         sim.volume_manager.add_material_database(fdb)
 
     # check overlap
     sim.g4_check_overlap_flag = False  # set to True for debug
 
     # spect head
-    head, lead_cover = add_ge_nm670_spect_box(sim, name, collimator_type)
+    head, lead_cover = add_spect_box(sim, name)
 
     # spect head
-    crystal = add_ge_nm670_spect_crystal(sim, name, lead_cover)
+    crystal = add_crystal(sim, name, lead_cover)
 
     # spect collimator
+    colli = None
     if collimator_type:
-        add_ge_nm670_spect_collimator(sim, name, head, collimator_type, debug)
+        colli = add_collimator(sim, name, head, collimator_type, debug)
 
-    return head, crystal
+    return head, colli, crystal
 
 
 def distance_to_center_of_crystal(sim, name="spect"):
     lead_cover = sim.volume_manager.volumes[f"{name}_lead_cover"]
     crystal = sim.volume_manager.volumes[f"{name}_crystal"]
     # distance from center to center of crystal
     shielding = sim.volume_manager.volumes[f"{name}_shielding"]
     d = shielding.translation[2] + lead_cover.translation[2] + crystal.translation[2]
     return d
 
 
-def add_ge_nm670_spect_box(sim, name, collimator_type):
+def add_spect_box(sim, name):
     cm = g4_units.cm
 
     # colors
     blue = [0.5, 0.5, 1, 0.8]
     gray = [0.5, 0.5, 0.5, 1]
     white = [1, 1, 1, 1]
     yellow = [1, 1, 0, 1]
@@ -143,29 +144,29 @@
     backside.translation = [0, 0, -0.13375 * cm]
     backside.material = "Pyrex66"
     backside.color = blue
 
     return head, lead_cover
 
 
-def add_ge_nm670_spect_crystal(sim, name, lead_cover):
+def add_crystal(sim, name, lead_cover):
     cm = g4_units.cm
     yellow = [1, 1, 0, 1]
     # mono-bloc crystal thickness 3/8 of inch = 0.9525 cm
     # (if 5/8 inch = 1.5875 ; but probably need to translate elements)
     crystal = sim.add_volume("Box", f"{name}_crystal")
     crystal.mother = lead_cover.name
     crystal.size = [54 * cm, 40 * cm, 0.9525 * cm]
     crystal.translation = [0, 0, 4.4625 * cm]
     crystal.material = "NaITl"
     crystal.color = yellow
     return crystal
 
 
-def add_ge_nm670_spect_collimator(sim, name, head, collimator_type, debug):
+def add_collimator(sim, name, head, collimator_type, debug):
     """
     Start with default lehr collimator description,
     then change some parameters for the other types
     """
     cm = g4_units.cm
 
     # colors
@@ -333,38 +334,15 @@
     # do it twice, with the following offset
     holep.offset_nb = 2
     holep.offset = [1.47224 * mm, 0.85 * mm, 0]
 
     return holep
 
 
-def UNUSED_megp_collimator_repeater_parametrised(sim, name, core, debug):
-    """# because this volume will be parameterised, we need to prevent
-    # the creation of the physical volume
-    hole.build_physical_volume = False
-
-    # parameterised holes
-    holep = sim.add_volume('RepeatParametrised', f'{name}_collimator_hole_param')
-    holep.mother = core.name
-    holep.translation = None
-    holep.rotation = None
-    holep.repeated_volume_name = hole.name
-    # number of repetition
-    holep.linear_repeat = [183, 235, 1]
-    if debug:
-        holep.linear_repeat = [10, 10, 1]
-    # translation for each repetition
-    holep.translation = [2.94449 * mm, 1.7 * mm, 0]
-    # starting position
-    holep.start = [-(holep.linear_repeat[0] * holep.translation[0]) / 2.0,
-                   -(holep.linear_repeat[1] * holep.translation[1]) / 2.0, 0]
-    """
-
-
-def add_simplified_digitizer_Tc99m(
+def add_simplified_digitizer_tc99m(
     sim, crystal_volume_name, output_name, scatter_flag=False
 ):
     # units
     keV = g4_units.keV
     # default  channels
     channels = []
     if scatter_flag:
@@ -432,14 +410,120 @@
     cc.mother = sc.mother
     cc.input_digi_collection = sc.name
     cc.channels = channels
     cc.output = ""  # No output
     return cc
 
 
+def add_digitizer_tc99m(sim, crystal_name, name):
+    # create main chain
+    mm = g4_units.mm
+    digitizer = Digitizer(sim, crystal_name, name)
+
+    # Singles
+    sc = digitizer.add_module("DigitizerAdderActor", f"{name}_singles")
+    sc.group_volume = None
+    sc.policy = "EnergyWinnerPosition"
+
+    # detection efficiency
+    ea = digitizer.add_module("DigitizerEfficiencyActor")
+    ea.efficiency = 0.86481  # FAKE
+
+    # energy blurring
+    keV = g4_units.keV
+    eb = digitizer.add_module("DigitizerBlurringActor")
+    eb.blur_attribute = "TotalEnergyDeposit"
+    eb.blur_method = "InverseSquare"
+    eb.blur_resolution = 0.063  # FAKE
+    eb.blur_reference_value = 140.57 * keV
+
+    # spatial blurring
+    sb = digitizer.add_module("DigitizerSpatialBlurringActor")
+    sb.blur_attribute = "PostPosition"
+    sb.blur_fwhm = 7.6 * mm  # FAKE
+    sb.keep_in_solid_limits = True
+
+    # energy windows (Energy range. 35-588 keV)
+    cc = digitizer.add_module("DigitizerEnergyWindowsActor", f"{name}_energy_window")
+    channels = [
+        {"name": f"spectrum", "min": 3 * keV, "max": 160 * keV},
+        {"name": f"scatter", "min": 108.57749938965 * keV, "max": 129.5924987793 * keV},
+        {"name": f"peak140", "min": 129.5924987793 * keV, "max": 150.60751342773 * keV},
+    ]
+    cc.channels = channels
+
+    # projection
+    proj = digitizer.add_module("DigitizerProjectionActor", f"{name}_projection")
+    channel_names = [c["name"] for c in channels]
+    proj.input_digi_collections = channel_names
+    proj.spacing = [2.21 * mm * 2, 2.21 * mm * 2]
+    proj.size = [128, 128]
+
+    # end
+    return digitizer
+
+
+def add_digitizer_lu177(sim, crystal_name, name):
+    # create main chain
+    mm = g4_units.mm
+    digitizer = Digitizer(sim, crystal_name, name)
+
+    # Singles
+    sc = digitizer.add_module("DigitizerAdderActor", f"{name}_singles")
+    sc.group_volume = None
+    sc.policy = "EnergyWinnerPosition"
+
+    # detection efficiency
+    ea = digitizer.add_module("DigitizerEfficiencyActor")
+    ea.efficiency = 0.86481  # FAKE
+
+    # energy blurring
+    keV = g4_units.keV
+    eb = digitizer.add_module("DigitizerBlurringActor")
+    eb.blur_attribute = "TotalEnergyDeposit"
+    eb.blur_method = "InverseSquare"
+    eb.blur_resolution = 0.063  # FAKE
+    eb.blur_reference_value = 140.57 * keV
+    # eb.blur_resolution = 0.13
+    # eb.blur_reference_value = 80 * keV
+    # eb.blur_slope = -0.09 * 1 / MeV  # fixme unsure about unit
+
+    # spatial blurring
+    # Source: HE4SPECS - FWHM = 3.9 mm
+    # FWHM = 2.sigma.sqrt(2ln2) -> sigma = 1.656 mm
+    sb = digitizer.add_module("DigitizerSpatialBlurringActor")
+    sb.blur_attribute = "PostPosition"
+    sb.blur_fwhm = 7.6 * mm  # FAKE
+    sb.keep_in_solid_limits = True
+
+    # energy windows (Energy range. 35-588 keV)
+    cc = digitizer.add_module("DigitizerEnergyWindowsActor", f"{name}_energy_window")
+    keV = g4_units.keV
+    # 112.9498 keV  = 6.20 %
+    # 208.3662 keV  = 10.38 %
+    p1 = 112.9498 * keV
+    p2 = 208.3662 * keV
+    channels = [
+        {"name": "spectrum", "min": 35 * keV, "max": 588 * keV},
+        *energy_windows_peak_scatter("peak113", "scatter1", "scatter2", p1, 0.2, 0.1),
+        *energy_windows_peak_scatter("peak208", "scatter3", "scatter4", p2, 0.2, 0.1),
+    ]
+    cc.channels = channels
+
+    # projection
+    proj = digitizer.add_module("DigitizerProjectionActor", f"{name}_projection")
+    channel_names = [c["name"] for c in channels]
+    proj.input_digi_collections = channel_names
+    proj.spacing = [2.21 * mm * 2, 2.21 * mm * 2]
+    proj.size = [128, 128]
+
+    # end
+    return digitizer
+
+
 # FIXME : put this elsewhere
 def get_volume_position_in_head(sim, spect_name, vol_name, pos="max", axis=2):
     vol = sim.volume_manager.volumes[f"{spect_name}_{vol_name}"]
     pMin, pMax = vol.bounding_limits
     x = pMax
     if pos == "min":
         x = pMin
@@ -448,15 +532,15 @@
     x = vec_g4_as_np(x)
     x = translate_point_to_volume(sim, vol, spect_name, x)
     return x[axis]
 
 
 def compute_plane_position_and_distance_to_crystal(collimator_type):
     sim = Simulation()
-    spect, crystal = add_ge_nm67_spect_head(sim, "spect", collimator_type, debug=True)
+    spect, colli, crystal = add_spect_head(sim, "spect", collimator_type, debug=True)
     pos = get_volume_position_in_head(sim, "spect", "collimator_psd", "max")
     y = get_volume_position_in_head(sim, "spect", "crystal", "center")
     crystal_distance = pos - y
     psd = spect.size[2] / 2.0 - pos
     return pos, crystal_distance, psd
```

### Comparing `opengate-10.0b7/opengate/contrib/spect/spect_ge_nm670_materials.db` & `opengate-10.0b8/opengate/contrib/spect/spect_ge_nm670_materials.db`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/contrib/tps/ionbeamtherapy.py` & `opengate-10.0b8/opengate/contrib/tps/ionbeamtherapy.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # -----------------------------------------------------------------------------
 
 import pydicom
 import os
 import re
 import numpy as np
 from scipy.spatial.transform import Rotation
-
+import opengate as gate
 
 # from utils.dose_info import dose_info
 import logging
 
 logger = logging.getLogger(__name__)
 
 
@@ -35,64 +35,95 @@
             name, len(seq), nmin, nmax
         )
     )
     assert len(seq) >= nmin
     assert nmax == 0 or len(seq) <= nmax
 
 
-def spots_info_from_txt(txtFile, ionType):
+def spots_info_from_txt(txtFile, ionType, beam_nr):
     # initialize empty variables
-    nFields = 0
-    ntot = []
-    energies = []
-    nSpots = []
-    spots = []
+
+    beam_data = dict()
+    beam_data["n_fields"] = 0
+    beam_data["plan_name"] = ""
+    beam_data["msw_beam"] = 0
+    beam_data["energies"] = []
+    beam_data["nb_spots"] = []
+    beam_data["spots"] = []
+    beam_data["gantry_angle"] = 0
+    beam_data["couch_angle"] = 0
+    beam_data["isocenter"] = []
+    found_field = False
     start_index = []
-    G = 0
 
     # read  content
     with open(txtFile, "r") as f:
         lines = f.readlines()
 
     # get plan's info
+    # TODO: make function to check line tag
     for i, line in enumerate(lines):
-        if line.startswith("###GantryAngle"):
-            l = lines[i + 1].split("\n")[0]
-            G = int(l)
-        if line.startswith("##NumberOfFields"):
-            l = lines[i + 1].split("\n")[0]
-            nFields = int(l)
-        if line.startswith("###FinalCumulativeMeterSetWeight"):
+        if check_plan_tag(line, "PlanName"):
             l = lines[i + 1].split("\n")[0]
-            ntot.append(float(l))
-        if line.startswith("####Energy"):
+            beam_data["plan_name"] = l
+        if check_plan_tag(line, "NumberOfFields"):
             l = lines[i + 1].split("\n")[0]
-            energies.append(float(l))
-        if line.startswith("####NbOfScannedSpots"):
-            l = lines[i + 1].split("\n")[0]
-            nSpots.append(int(l))
-        if line.startswith("####X Y Weight"):
-            start_index.append(i + 1)
-
-    np = sum(ntot)
-    for k in range(nFields):
-        # np = ntot[k]
-        for i in range(len(energies)):
-            e = energies[i]
-            print(f"ENERGY: {e}")
-            start = start_index[i]
-            end = start_index[i] + nSpots[i]
-            for j in range(start, end):
-                l = lines[j].split("\n")[0].split()
-                spot = SpotInfo(float(l[0]), float(l[1]), float(l[2]), e)
-                spot.beamFraction = float(l[2]) / np
-                spot.particle_name = ionType
-                spots.append(spot)
+            beam_data["n_fields"] = int(l)
+            if beam_nr > beam_data["n_fields"]:
 
-    return spots, np, energies, G
+                raise ValueError(
+                    "requested beam number higher than number of beams in the beamset"
+                )
+        if check_plan_tag(line, "FIELD-DESCRIPTION"):
+            found_field = False
+        if check_plan_tag(line, "FieldID"):
+            fieldID = int(lines[i + 1].split("\n")[0])
+            if fieldID == beam_nr:
+                found_field = True
+        if found_field:
+            if check_plan_tag(line, "GantryAngle"):
+                l = lines[i + 1].split("\n")[0]
+                beam_data["gantry_angle"] = float(l)
+            if check_plan_tag(line, "PatientSupportAngle"):
+                l = lines[i + 1].split("\n")[0]
+                beam_data["couch_angle"] = float(l)
+            if check_plan_tag(line, "IsocenterPosition"):
+                l = lines[i + 1].split("\n")[0]
+                beam_data["isocenter"] = [float(i) for i in l.split()]
+            if check_plan_tag(line, "FinalCumulativeMeterSetWeight"):
+                l = lines[i + 1].split("\n")[0]
+                beam_data["msw_beam"] = float(l)
+            if check_plan_tag(line, "Energy"):
+                l = lines[i + 1].split("\n")[0]
+                beam_data["energies"].append(float(l))
+            if check_plan_tag(line, "NbOfScannedSpots"):
+                l = lines[i + 1].split("\n")[0]
+                beam_data["nb_spots"].append(int(l))
+            if check_plan_tag(line, "X Y Weight"):
+                start_index.append(i + 1)
+
+    for i in range(len(beam_data["energies"])):
+        e = beam_data["energies"][i]
+        # print(f"ENERGY: {e}")
+        start = start_index[i]
+        end = start_index[i] + beam_data["nb_spots"][i]
+        for j in range(start, end):
+            l = lines[j].split("\n")[0].split()
+            spot = SpotInfo(float(l[0]), float(l[1]), float(l[2]), e)
+            spot.beamFraction = float(l[2]) / beam_data["msw_beam"]
+            spot.particle_name = ionType
+            beam_data["spots"].append(spot)
+
+    return beam_data
+
+
+def check_plan_tag(txt_line, tag):
+    txt_line = txt_line.strip().lower()
+    tag = tag.strip().lower()
+    return tag in txt_line
 
 
 def get_spots_from_beamset(beamset):
     rad_type = beamset.bs_info["Radiation Type Opengate"]
     spots_array = []
     mswtot = beamset.mswtot
     for beam in beamset.beams:
@@ -104,14 +135,30 @@
                     nPlannedSpot / mswtot
                 )  # nr particles planned for the spot/tot particles planned for the beam
                 spot.particle_name = rad_type
                 spots_array.append(spot)
     return spots_array
 
 
+def get_spots_from_beamset_beam(beamset, beam_nr):
+    rad_type = beamset.bs_info["Radiation Type Opengate"]
+    spots_array = []
+    beam = beamset.beams[beam_nr - 1]
+    mswtot = beam.mswtot
+    for energy_layer in beam.layers:
+        for spot in energy_layer.spots:
+            nPlannedSpot = spot.w
+            spot.beamFraction = (
+                nPlannedSpot / mswtot
+            )  # nr particles planned for the spot/tot particles planned for the beam
+            spot.particle_name = rad_type
+            spots_array.append(spot)
+    return spots_array
+
+
 # FIXME: IonSpotInfo
 class SpotInfo(object):
     def __init__(self, xiec, yiec, w, e):
         self.xiec = xiec
         self.yiec = yiec
         self.w = w
         self.energy = e
@@ -637,17 +684,19 @@
                 for a in self.plan_req_attrs
             ]
         )
         opts = dict(
             [
                 (
                     a,
-                    "NA"
-                    if not hasattr(self._rp, a.replace(" ", ""))
-                    else str(getattr(self._rp, a.replace(" ", ""))),
+                    (
+                        "NA"
+                        if not hasattr(self._rp, a.replace(" ", ""))
+                        else str(getattr(self._rp, a.replace(" ", "")))
+                    ),
                 )
                 for a in self.plan_opt_attrs
             ]
         )
         reqs.update(opts)
         return reqs
 
@@ -711,50 +760,60 @@
 
     def set_particles_to_simulate(self, n_sim):
         self.n_sim = n_sim
 
     def set_spots(self, spots):
         self.spots = spots
 
-    def set_spots_from_rtplan(self, rt_plan_path):
+    def set_spots_from_rtplan(self, rt_plan_path, beam_nr=1):
         beamset = BeamsetInfo(rt_plan_path)
-        gantry_angle = beamset.beam_angles[0]
-        spots = get_spots_from_beamset(beamset)
+        gantry_angle = beamset.beam_angles[beam_nr - 1]
+        spots = get_spots_from_beamset_beam(beamset, beam_nr)
         self.spots = spots
         self.rotation = Rotation.from_euler("z", gantry_angle, degrees=True)
 
     def set_beamline_model(self, beamline):
         self.beamline_model = beamline
 
-    def initialize_tpsource(self):
+    def initialize_tpsource(self, flat_generation=False, activity=False):
         # some alias
+        Bq = gate.g4_units.Bq
         spots_array = self.spots
         sim = self.sim
         nSim = self.n_sim
         beamline = self.beamline_model
         self.d_nozzle_to_iso = beamline.distance_nozzle_iso
         self.d_stearMag_to_iso_x = beamline.distance_stearmag_to_isocenter_x
         self.d_stearMag_to_iso_y = beamline.distance_stearmag_to_isocenter_y
 
         # mapping factors between iso center plane and nozzle plane (due to steering magnets)
-        cal_proportion_factor = (
-            lambda d_magnet_iso: 1
+        cal_proportion_factor = lambda d_magnet_iso: (
+            1
             if (d_magnet_iso == float("inf"))
             else (d_magnet_iso - self.d_nozzle_to_iso) / d_magnet_iso
         )
         self.proportion_factor_x = cal_proportion_factor(self.d_stearMag_to_iso_x)
         self.proportion_factor_y = cal_proportion_factor(self.d_stearMag_to_iso_y)
         tot_sim_particles = 0
+
+        n_part_spots_V = self._sample_n_particles_spots(flat_generation=flat_generation)
+
         # initialize a pencil beam for each spot
         for i, spot in enumerate(spots_array):
-            # simulate a fraction of the beam particles for this spot
-            nspot = np.round(spot.beamFraction * nSim)
+            # if flat_generation:
+            #     # simualte same number of particles for each spot
+            #     nspot = nSim / len(spots_array)
+            # else:
+            #     # simulate a fraction of the beam particles for this spot
+            #     nspot = spot.beamFraction * nSim
+
+            nspot = n_part_spots_V[i]
             if nspot == 0:
                 continue
-            tot_sim_particles += nspot
+
             source = sim.add_source("IonPencilBeamSource", f"{self.name}_spot_{i}")
 
             # set energy
             source.energy.type = "gauss"
             source.energy.mono = beamline.get_energy(nominal_energy=spot.energy)
             source.energy.sigma_gauss = beamline.get_sigma_energy(
                 nominal_energy=spot.energy
@@ -770,16 +829,26 @@
             # POSITION:
             source.position.translation = self._get_pbs_position(spot)
 
             # ROTATION:
             source.position.rotation = self._get_pbs_rotation(spot)
 
             # add weight
-            # source.weight = -1
-            source.n = nspot
+            if flat_generation:
+                source.weight = spot.beamFraction * len(spots_array)
+                print(f"{source.weight = }")
+
+            # set number of particles
+            if activity:
+                source.activity = nspot * Bq
+            else:
+                # nspot = np.round(nspot)
+                source.n = nspot
+
+            tot_sim_particles += nspot
 
             # set optics parameters
             source.direction.partPhSp_x = [
                 beamline.get_sigma_x(spot.energy),
                 beamline.get_theta_x(spot.energy),
                 beamline.get_epsilon_x(spot.energy),
                 beamline.conv_x,
@@ -789,16 +858,33 @@
                 beamline.get_theta_y(spot.energy),
                 beamline.get_epsilon_y(spot.energy),
                 beamline.conv_y,
             ]
 
         self.actual_sim_particles = tot_sim_particles
 
+    def _sample_n_particles_spots(self, flat_generation=False):
+        if flat_generation:
+            pdf = [1 / len(self.spots) for spot in self.spots]
+        else:
+            pdf = [spot.beamFraction for spot in self.spots]
+
+        # normalize vector, to assure the probabilities sum up to 1
+        pdf = pdf / np.sum(pdf)
+
+        n_spots = len(self.spots)
+        n_part_spots_V = np.zeros(n_spots)
+        for i in range(int(self.n_sim)):
+            bin = np.random.choice(np.arange(0, n_spots), p=pdf)
+            n_part_spots_V[bin] += 1
+
+        return n_part_spots_V
+
     def _get_pbs_position(self, spot):
-        # (x,y) refer to isocenter plane.
+        # (x,y) referr to isocenter plane.
         # Need to be corrected to referr to nozzle plane
         pos = [
             (spot.xiec) * self.proportion_factor_x,
             (spot.yiec) * self.proportion_factor_y,
             self.d_nozzle_to_iso,
         ]
         # Gantry angle = 0 -> source comes from +y and is positioned along negative side of y-axis
```

### Comparing `opengate-10.0b7/opengate/contrib/tps/treatmentPlanPhsSource.py` & `opengate-10.0b8/opengate/contrib/tps/treatmentPlanPhsSource.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,16 @@
         # verify the phase space list
         self.verify_phs_files_exist(self.phaseSpaceList)
         spots_array = self.spots
         sim = self.sim
         nSim = self.n_sim
 
         # mapping factors between iso center plane and nozzle plane (due to steering magnets)
-        cal_proportion_factor = (
-            lambda d_magnet_iso: 1
+        cal_proportion_factor = lambda d_magnet_iso: (
+            1
             if (d_magnet_iso == float("inf"))
             else (d_magnet_iso - self.d_nozzle_to_iso) / d_magnet_iso
         )
         self.proportion_factor_x = cal_proportion_factor(self.d_stearMag_to_iso_x)
         self.proportion_factor_y = cal_proportion_factor(self.d_stearMag_to_iso_y)
 
         tot_sim_particles = 0
```

### Comparing `opengate-10.0b7/opengate/data/OpticalProperties.xml` & `opengate-10.0b8/opengate/data/OpticalProperties.xml`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/decorators.py` & `opengate-10.0b8/opengate/decorators.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/definitions.py` & `opengate-10.0b8/opengate/definitions.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/element.py` & `opengate-10.0b8/opengate/element.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/engines.py` & `opengate-10.0b8/opengate/engines.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,44 +3,47 @@
 import sys
 import os
 
 # from multiprocessing import Process, set_start_method, Manager
 # import queue
 import weakref
 from box import Box
-import xml.etree.ElementTree as ET
 from anytree import PreOrderIter
 
 import opengate_core as g4
 
 from .exception import fatal, warning
 from .decorators import requires_fatal, requires_warning
 from .logger import log
 from .runtiming import assert_run_timing
 from .uisessions import UIsessionSilent, UIsessionVerbose
 from .exception import ExceptionHandler
-from .utility import g4_units, get_material_name_variants
 from .element import new_element
 from .physics import (
     UserLimitsPhysics,
-    translate_particle_name_gate2G4,
+    translate_particle_name_gate_to_geant4,
     cut_particle_names,
+    create_g4_optical_properties_table,
+    load_optical_properties_from_xml,
 )
 
 
 class EngineBase:
     """
     Base class for all engines (SimulationEngine, VolumeEngine, etc.)
     """
 
     def __init__(self, simulation_engine):
         self.simulation_engine = simulation_engine
         # debug verbose
-        self.verbose_getstate = simulation_engine.simulation.verbose_getstate
-        self.verbose_close = simulation_engine.simulation.verbose_close
+        self.verbose_getstate = simulation_engine.verbose_getstate
+        self.verbose_close = simulation_engine.verbose_close
+
+    def close(self):
+        pass  # nothing do to, but kept as dummy for the future
 
 
 class SourceEngine(EngineBase):
     """
     Source Engine manages the G4 objects of sources at runtime
     """
 
@@ -77,14 +80,15 @@
         # FIXME: Why is this separate dictionary needed? Would be better to access the source manager directly
         self.source_manager_options = Box()
 
     def close(self):
         if self.verbose_close:
             warning(f"Closing SourceEngine")
         self.release_g4_references()
+        super().close()
 
     def release_g4_references(self):
         self.g4_master_source_manager = None
         self.g4_thread_source_managers = None
         self.g4_particle_table = None
         # a source object contains a reference to a G4 source
         self.sources = None
@@ -123,15 +127,15 @@
         created after physics initialization
         """
         ms = g4.GateSourceManager()
         # create all sources for this source manager (for all threads)
         source_manager = self.simulation_engine.simulation.source_manager
         for vu in source_manager.user_info_sources.values():
             source = new_element(vu, self.simulation_engine.simulation)
-            ms.AddSource(source.g4_source)
+            source.add_to_source_manager(ms)
             source.initialize(self.run_timing_intervals)
             self.sources.append(source)
 
         # Copy visualization parameters
         for k, v in self.simulation_engine.simulation.user_info.items():
             if "visu" in k:
                 self.source_manager_options[k] = v
@@ -159,184 +163,71 @@
         self.g4_master_source_manager.StartMasterThread()
 
         # once terminated, packup the sources (if needed)
         for source in self.sources:
             source.prepare_output()
 
 
-def load_optical_properties_from_xml(optical_properties_file, material_name):
-    """This function parses an xml file containing optical material properties.
-    Fetches property elements and property vector elements.
-
-    Returns a dictionary with the properties or None if the material is not found in the file.
-    """
-    try:
-        xml_tree = ET.parse(optical_properties_file)
-    except FileNotFoundError:
-        fatal(f"Could not find the optical_properties_file {optical_properties_file}.")
-    xml_root = xml_tree.getroot()
-
-    xml_entry_material = None
-    for m in xml_root.findall("material"):
-        # FIXME: some names might follow different conventions, e.g. 'Water' vs. 'G4_WATER'
-        # using variants of the name is a possible solution, but this should be reviewed
-        if str(m.get("name")) in get_material_name_variants(material_name):
-            xml_entry_material = m
-            break
-    if xml_entry_material is None:
-        warning(
-            f"Could not find any optical material properties for material {material_name} "
-            f"in file {optical_properties_file}."
-        )
-        return
-
-    material_properties = {"constant_properties": {}, "vector_properties": {}}
-
-    for ptable in xml_entry_material.findall("propertiestable"):
-        # Handle property elements in XML document
-        for prop in ptable.findall("property"):
-            property_name = prop.get("name")
-            property_value = float(prop.get("value"))
-            property_unit = prop.get("unit")
-
-            # apply unit if applicable
-            if property_unit is not None:
-                if len(property_unit.split("/")) == 2:
-                    unit = property_unit.split("/")[1]
-                else:
-                    unit = property_unit
-                property_value *= g4_units[unit]
-
-            material_properties["constant_properties"][property_name] = {
-                "property_value": property_value,
-                "property_unit": property_unit,
-            }
-
-        # Handle propertyvector elements
-        for prop_vector in ptable.findall("propertyvector"):
-            prop_vector_name = prop_vector.get("name")
-            prop_vector_value_unit = prop_vector.get("unit")
-            prop_vector_energy_unit = prop_vector.get("energyunit")
-
-            if prop_vector_value_unit is not None:
-                value_unit = g4_units[prop_vector_value_unit]
-            else:
-                value_unit = 1.0
-
-            if prop_vector_energy_unit is not None:
-                energy_unit = g4_units[prop_vector.get("energyunit")]
-            else:
-                energy_unit = 1.0
-
-            # Handle ve elements inside propertyvector
-            ve_energy_list = []
-            ve_value_list = []
-            for ve in prop_vector.findall("ve"):
-                ve_energy_list.append(float(ve.get("energy")) * energy_unit)
-                ve_value_list.append(float(ve.get("value")) * value_unit)
-
-            material_properties["vector_properties"][prop_vector_name] = {
-                "prop_vector_value_unit": prop_vector_value_unit,
-                "prop_vector_energy_unit": prop_vector_energy_unit,
-                "ve_energy_list": ve_energy_list,
-                "ve_value_list": ve_value_list,
-            }
-
-    return material_properties
-
-
-def create_g4_optical_properties_table(material_properties_dictionary):
-    """Creates and fills a G4MaterialPropertiesTable with values from a dictionary created by a parsing function,
-    e.g. from an xml file.
-    Returns G4MaterialPropertiesTable.
-    """
-
-    g4_material_table = g4.G4MaterialPropertiesTable()
-
-    for property_name, data in material_properties_dictionary[
-        "constant_properties"
-    ].items():
-        # check whether the property is already present
-        create_new_key = (
-            property_name not in g4_material_table.GetMaterialConstPropertyNames()
-        )
-        if create_new_key is True:
-            warning(
-                f"Found property {property_name} in optical properties file which is not known to Geant4. "
-                f"I will create the property for you, but you should verify whether physics are correctly modeled."
-            )
-        g4_material_table.AddConstProperty(
-            g4.G4String(property_name), data["property_value"], create_new_key
-        )
-
-    for property_name, data in material_properties_dictionary[
-        "vector_properties"
-    ].items():
-        # check whether the property is already present
-        create_new_key = (
-            property_name not in g4_material_table.GetMaterialPropertyNames()
-        )
-        if create_new_key is True:
-            warning(
-                f"Found property {property_name} in optical properties file which is not known to Geant4. "
-                f"I will create the property for you, but you should verify whether physics are correctly modeled."
-            )
-        g4_material_table.AddProperty(
-            g4.G4String(property_name),
-            data["ve_energy_list"],
-            data["ve_value_list"],
-            create_new_key,
-            False,
-        )
-
-    return g4_material_table
-
-
 class PhysicsEngine(EngineBase):
     """
     Class that contains all the information and mechanism regarding physics
     to actually run a simulation. It is associated with a simulation engine.
 
     """
 
-    def __init__(self, simulation_engine):
-        super().__init__(simulation_engine)
-        # Keep a short cut reference to the current physics_manager
-        self.physics_manager = simulation_engine.simulation.physics_manager
+    def __init__(self, *args):
+        super().__init__(*args)
+        # Keep a shortcut reference to the current physics_manager
+        self.physics_manager = self.simulation_engine.simulation.physics_manager
 
         # Register this engine with the regions
         for region in self.physics_manager.regions.values():
             region.physics_engine = self
 
+        for optical_surface in self.physics_manager.optical_surfaces.values():
+            optical_surface.physics_engine = self
+
         # main g4 physic list
         self.g4_physics_list = None
         self.g4_decay = None
         self.g4_radioactive_decay = None
         self.g4_cuts_by_regions = []
         self.g4_em_parameters = None
         self.g4_parallel_world_physics = []
         self.g4_optical_material_tables = {}
+        self.g4_physical_volumes = []
+        self.g4_surface_properties = None
 
         # physics constructors implement on the Gate/python side
         self.gate_physics_constructors = []
 
+        self.optical_surfaces_properties_dict = {}
+
     def close(self):
         if self.verbose_close:
             warning(f"Closing PhysicsEngine")
         self.close_physics_constructors()
         self.release_g4_references()
+        self.release_optical_surface_g4_references()
+        super().close()
 
     def release_g4_references(self):
         self.g4_physics_list = None
         self.g4_decay = None
         self.g4_radioactive_decay = None
         self.g4_cuts_by_regions = None
         self.g4_em_parameters = None
         self.g4_parallel_world_physics = []
         self.g4_optical_material_tables = {}
+        self.g4_physical_volumes = []
+        self.g4_surface_properties = None
+
+    def release_optical_surface_g4_references(self):
+        for optical_surface in self.physics_manager.optical_surfaces.values():
+            optical_surface.release_g4_references()
 
     @requires_fatal("simulation_engine")
     @requires_warning("g4_physics_list")
     def close_physics_constructors(self):
         """This method removes PhysicsConstructors defined in python from the physics list.
 
         It should be called after a simulation run, i.e. when a simulation engine closes,
@@ -372,14 +263,15 @@
         # Cuts need to be set *after*
         # G4RunManager.Initialize() is called.
         # Reason: The Initialize() sequence would otherwise override
         # the global cuts with the physics list defaults.
         self.initialize_global_cuts()
         self.initialize_regions()
         self.initialize_optical_material_properties()
+        self.initialize_optical_surfaces()
 
     def initialize_parallel_world_physics(self):
         for (
             world
         ) in self.physics_manager.simulation.volume_manager.parallel_world_names:
             pwp = g4.G4ParallelWorldPhysics(world, True)
             self.g4_parallel_world_physics.append(pwp)
@@ -420,15 +312,15 @@
         else:
             for pname, value in ui.global_production_cuts.items():
                 # ignore 'all', as that's already treated above
                 if pname == "all":
                     continue
                 if value is not None and value not in ("default", "Default"):
                     self.g4_physics_list.SetCutValue(
-                        value, translate_particle_name_gate2G4(pname)
+                        value, translate_particle_name_gate_to_geant4(pname)
                     )
 
     def initialize_g4_em_parameters(self):
         self.g4_em_parameters = g4.G4EmParameters.Instance()
 
         self.g4_em_parameters.SetApplyCuts(self.physics_manager.apply_cuts)
 
@@ -483,27 +375,36 @@
                 vol
             ) in self.simulation_engine.simulation.volume_manager.volumes.values():
                 material_name = vol.g4_material.GetName()
                 material_properties = load_optical_properties_from_xml(
                     self.physics_manager.optical_properties_file, material_name
                 )
                 if material_properties is not None:
-                    self.g4_optical_material_tables[
-                        str(material_name)
-                    ] = create_g4_optical_properties_table(material_properties)
+                    self.g4_optical_material_tables[str(material_name)] = (
+                        create_g4_optical_properties_table(material_properties)
+                    )
                     vol.g4_material.SetMaterialPropertiesTable(
                         self.g4_optical_material_tables[str(material_name)]
                     )
                 else:
                     warning(
                         f"Could not load the optical material properties for material {material_name} "
                         f"found in volume {vol.name} from file {self.physics_manager.optical_properties_file}."
                     )
 
     @requires_fatal("physics_manager")
+    def initialize_optical_surfaces(self):
+        """Calls initialize() method of each OpticalSurface instance."""
+
+        # Call the initialize() method in OpticalSurface class to
+        # create the related G4 instances.
+        for optical_surface in self.physics_manager.optical_surfaces.values():
+            optical_surface.initialize()
+
+    @requires_fatal("physics_manager")
     def initialize_user_limits_physics(self):
         need_step_limiter = False
         need_user_special_cut = False
         for r in self.physics_manager.regions.values():
             if r.need_step_limiter() is True:
                 need_step_limiter = True
             if r.need_user_special_cut() is True:
@@ -521,18 +422,14 @@
     Main object to manage all actions during a simulation.
     """
 
     def __init__(self, simulation_engine):
         g4.G4VUserActionInitialization.__init__(self)
         EngineBase.__init__(self, simulation_engine)
 
-        # The py source engine
-        # self.simulation_engine.source_engine = source
-        self.simulation_engine = simulation_engine
-
         # *** G4 references ***
         # List of G4 source managers (one per thread)
         self.g4_PrimaryGenerator = []
 
         # The main G4 source manager
         self.g4_main_PrimaryGenerator = None
 
@@ -541,14 +438,15 @@
         self.g4_EventAction = []
         self.g4_TrackingAction = []
 
     def close(self):
         if self.verbose_close:
             warning(f"Closing ActionEngine")
         self.release_g4_references()
+        super().close()
 
     def release_g4_references(self):
         self.g4_PrimaryGenerator = None
         self.g4_main_PrimaryGenerator = None
         self.g4_RunAction = None
         self.g4_EventAction = None
         self.g4_TrackingAction = None
@@ -601,23 +499,26 @@
     """
 
     def __init__(self, simulation_engine):
         super().__init__(simulation_engine)
         # self.actor_manager = simulation.actor_manager
         # we use a weakref because it is a circular dependence
         # with custom __del__
+        # FIXME: we should not need this weak ref
         self.simulation_engine_wr = weakref.ref(simulation_engine)
         self.actors = {}
 
     def close(self):
         if self.verbose_close:
             warning(f"Closing ActorEngine")
         for actor in self.actors.values():
             actor.close()
-        self.actors = None
+        self.actors = {}
+        self.simulation_engine_wr = None
+        super().close()
 
     def get_actor(self, name):
         if name not in self.actors:
             fatal(
                 f"The actor {name} is not in the current "
                 f"list of actors: {self.actors}"
             )
@@ -788,24 +689,43 @@
             volume.volume_engine = self
 
     def close(self):
         for vol in self.volume_manager.volumes.values():
             vol.close()
         for pwv in self.volume_manager.parallel_world_volumes.values():
             pwv.close()
+        super().close()
         # self.volume_manager.world_volume.close()
 
+    def initialize(self):
+        # build the materials
+        self.simulation_engine.simulation.volume_manager.material_database.initialize()
+        # initialize actors which handle dynamic volume parametrization, e.g. MotionActors
+        self.initialize_dynamic_parametrisations()
+
+    def initialize_dynamic_parametrisations(self):
+        dynamic_volumes = self.volume_manager.dynamic_volumes
+        if len(dynamic_volumes) > 0:
+            dynamic_geometry_actor = self.simulation_engine.simulation.add_actor(
+                "DynamicGeometryActor", "dynamic_geometry_actor"
+            )
+        else:  # nothing to do
+            return
+        for vol in self.volume_manager.dynamic_volumes:
+            dynamic_geometry_actor.geometry_changers.extend(vol.create_changers())
+
     def Construct(self):
         """
         G4 overloaded.
         Override the Construct method from G4VUserDetectorConstruction
         """
 
-        # build the materials
-        self.simulation_engine.simulation.volume_manager.material_database.initialize()
+        # # build the materials
+        # # FIXME: should go into initialize method
+        # self.simulation_engine.simulation.volume_manager.material_database.initialize()
 
         # Construct all volumes within the mass world along the tree hierarchy
         # The world volume is the first item
         for volume in PreOrderIter(self.volume_manager.world_volume):
             volume.construct()
 
         # return the (main) world physical volume
@@ -1017,22 +937,23 @@
             s = self.sources_by_thread[thread].keys
             fatal(
                 f'The source "{name}" does not exist. Here is the list of sources: {s}'
             )
         return self.sources_by_thread[thread][name]
 
 
-class SimulationEngine(EngineBase):
+class SimulationEngine:
     """
     Main class to execute a Simulation (optionally in a separate subProcess)
     """
 
     def __init__(self, simulation, new_process=False):
         self.simulation = simulation
-        EngineBase.__init__(self, self)
+        self.verbose_getstate = simulation.verbose_getstate
+        self.verbose_close = simulation.verbose_close
 
         # create engines passing the simulation engine (self) as argument
         self.volume_engine = VolumeEngine(self)
         self.volume_engine.create_parallel_world_engines()
         self.physics_engine = PhysicsEngine(self)
         self.source_engine = SourceEngine(self)
         self.action_engine = ActionEngine(self)
@@ -1042,14 +963,17 @@
         # current state of the engine
         self.run_timing_intervals = None
         self.is_initialized = False
 
         # do we create a subprocess or not ?
         self.new_process = new_process
 
+        # init only ?
+        self.init_only = False
+
         # LATER : option to wait the end of completion or not
 
         # UI
         self.ui_session = None
         self.g4_ui = None
 
         # random engine
@@ -1112,16 +1036,16 @@
         if self._is_closed is False:
             self.close_engines()
             self.release_engines()
             self.release_g4_references()
             self.notify_managers()
             if self.g4_RunManager:
                 self.g4_RunManager.SetVerboseLevel(0)
-            self.g4_RunManager = None
             self._is_closed = True
+        self.g4_RunManager = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.close()
 
@@ -1150,34 +1074,44 @@
         which where set to None during pickling by implementing a __setstate__ method.
         Implementing the resetting somewhere else (maybe in multiple places...) in the code will
         make it very difficult to maintain.
 
         -> removed the lines and implemented __setstate__ methods for the classes in question
         """
 
+        # prepare the output
+        output = SimulationOutput()
+
         # initialization
         self.initialize()
 
         # things to do after init and before run
         self.apply_all_g4_commands_after_init()
         if self.user_hook_after_init:
             log.info("Simulation: initialize user fct")
             self.user_hook_after_init(self)
 
+        # if init only, we stop
+        if self.init_only:
+            output.store_actors(self)
+            output.store_sources(self)
+            output.store_hook_log(self)
+            output.current_random_seed = self.current_random_seed
+            return output
+
         # go
         self.start_and_stop()
 
         # start visualization if vrml or gdml
         self.visu_engine.start_visualisation()
         if self.user_hook_after_run:
             log.info("Simulation: User hook after run")
             self.user_hook_after_run(self)
 
         # prepare the output
-        output = SimulationOutput()
         output.store_actors(self)
         output.store_sources(self)
         output.store_hook_log(self)
         output.current_random_seed = self.current_random_seed
 
         return output
 
@@ -1262,32 +1196,41 @@
         """
         Build the main geant4 objects and initialize them.
         """
 
         # g4 verbose
         self.initialize_g4_verbose()
 
+        # visualisation ?
+        # self.pre_init_visu()
+
         # init random engine (before the MTRunManager creation)
         self.initialize_random_engine()
 
+        # Some sources (e.. PHID) need to perform computation once everything is defined in user_info but *before* the
+        # initialization of the G4 engine starts. This can be done via this function.
+        self.simulation.initialize_source_before_g4_engine()
+
         # create the run manager (assigned to self.g4_RunManager)
         self.create_run_manager()
 
         # create the handler for the exception
         self.g4_exception_handler = ExceptionHandler()
 
         # check run timing
         self.run_timing_intervals = self.simulation.run_timing_intervals.copy()
+        # FIXME: put this assertion in a setter hook
         assert_run_timing(self.run_timing_intervals)
 
         # Geometry initialization
         log.info("Simulation: initialize Geometry")
 
         # Set the userDetector pointer of the Geant4 run manager
         # to VolumeEngine object defined here in open-gate
+        self.volume_engine.initialize()
         self.g4_RunManager.SetUserInitialization(self.volume_engine)
         # Important: The volumes are constructed
         # when the G4RunManager calls the Construct method of the VolumeEngine,
         # which happens in the InitializeGeometry method of the
         # G4RunManager (Geant4 code)
 
         # Physics initialization
@@ -1388,21 +1331,21 @@
         # this creates a finalizer for the run manager which assures that
         # the close() method is called before the run manager is garbage collected,
         # i.e. G4RunManager destructor is called
         self.run_manager_finalizer = weakref.finalize(self.g4_RunManager, self.close)
 
     def apply_all_g4_commands_after_init(self):
         for command in self.simulation.g4_commands_after_init:
-            self.apply_g4_command(command)
+            self.add_g4_command_after_init(command)
 
     def apply_all_g4_commands_before_init(self):
         for command in self.simulation.g4_commands_before_init:
-            self.apply_g4_command(command)
+            self.add_g4_command_after_init(command)
 
-    def apply_g4_command(self, command):
+    def add_g4_command_after_init(self, command):
         if self.g4_ui is None:
             self.g4_ui = g4.G4UImanager.GetUIpointer()
         log.info(f"Simulation: apply G4 command '{command}'")
         code = self.g4_ui.ApplyCommand(command)
         if code == 0:
             return
         err_codes = {
```

### Comparing `opengate-10.0b7/opengate/exception.py` & `opengate-10.0b8/opengate/exception.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/geometry/materials.py` & `opengate-10.0b8/opengate/geometry/materials.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import numpy as np
 import re
 from box import Box
+import itk
 
 import opengate_core as g4
 from ..utility import fatal, g4_units, g4_best_unit
 from ..definitions import elements_name_symbol
 
 
 def read_voxel_materials(filename, def_mat="G4_AIR"):
@@ -284,14 +285,114 @@
         return None
     w = w[1].split()
     value = float(w[0])
     u = g4_units[w[1].strip()]
     return value * u
 
 
+def create_density_img(img_volume, material_database):
+    """
+
+
+    Parameters
+    ----------
+    img_volume : ImageVolume
+        opengate ImageVolume class instance
+    material_database : dict
+        dictionary with keys: material name, values: G4 material obj
+
+    Returns
+    -------
+    rho : itk.Image
+        image of the same size and resolution of the ct. The voxel value is the density of the voxel.
+        Density is returned in G4 1/kg.
+
+    """
+    voxel_materials = img_volume.user_info.voxel_materials
+    ct_itk = img_volume.itk_image
+    act = itk.GetArrayFromImage(ct_itk)
+    arho = np.zeros(act.shape, dtype=np.float32)
+
+    for material in voxel_materials:
+        *hu_interval, mat_name = material
+        hu0, hu1 = hu_interval
+        m = (act >= hu0) * (act < hu1)
+        density = material_database[mat_name].GetDensity()
+        arho[m] = density
+
+    rho = itk.GetImageFromArray(arho)
+    rho.CopyInformation(ct_itk)
+
+    return rho
+
+
+def create_mass_img(ct_itk, hu_density_file, overrides=dict()):
+    """
+
+
+    Parameters
+    ----------
+    ct_itk :itk.Image
+        ct image
+    hu_density_file : str
+        filepath of the HU to density table
+    overrides : dict, optional
+        Dict where keys are HU to be overwritten and values
+        are density values. The default is dict().
+
+    Returns
+    -------
+    mass : itk.Image
+        image of the same size and resolution of the ct. The voxel value is the mass of the voxel.
+        Mass is returned in grams.
+
+    """
+    hlut = HU_read_density_table(hu_density_file)
+    act = itk.GetArrayFromImage(ct_itk)
+    amass = np.zeros(act.shape, dtype=np.float32)
+    done = np.zeros(act.shape, dtype=bool)
+
+    m = act < hlut[0]["HU"]
+    amass[m] = hlut[0]["density"]
+    done |= m
+    m = act >= hlut[-1]["HU"]
+    amass[m] = hlut[-1]["density"]
+    done |= m
+
+    # interpolate for intermediate values
+    for hlut0, hlut1 in zip(hlut[:-1], hlut[1:]):
+        hu0, rho0 = hlut0["HU"], hlut0["density"]
+        hu1, rho1 = hlut1["HU"], hlut1["density"]
+        m = (act >= hu0) * (act < hu1)
+        assert not (m * done).any(), "programming error"
+        amass[m] = rho0
+        amass[m] += (act[m] - hu0) * (rho1 - rho0) / (hu1 - hu0)
+        done |= m
+    assert done.all(), "programming error"
+
+    #  override density for specific HU values
+    for hu, rho in overrides.items():
+        assert hu == int(hu), "overrides must be given for integer HU values"
+        assert rho >= 0, "override density values must be non-negative"
+        m = act == hu
+        amass[m] = rho
+        done |= m
+
+    spacing = ct_itk.GetSpacing()
+    voxel_vol = (
+        spacing[0] * spacing[1] * spacing[2] * 1e-3
+    )  # density in g/cm3 -> spacing in mm
+    amass *= voxel_vol  # mass in g
+
+    mass = itk.GetImageFromArray(amass)
+    mass.CopyInformation(ct_itk)
+
+    return mass
+
+
 class ElementBuilder:
     """
     A description of a G4Element that can be build.
     """
 
     def __init__(self, material_database):
         self.type = "element"
@@ -529,14 +630,30 @@
         self.current_section = None
         self.current_filename = None
         # specific to NIST materials
         self.g4_NistManager = None
         self.nist_material_names = None
         self.nist_element_names = None
 
+    def __getstate__(self):
+        return_dict = self.__dict__
+        # remove items that cannot be pickled, e.g. G4 objects
+        return_dict["g4_materials"] = {}
+        return_dict["g4_elements"] = {}
+        return_dict["g4_NistManager"] = None
+        return_dict["nist_material_names"] = None
+        return_dict["nist_element_names"] = None
+        return_dict["material_builders_by_filename"].pop("NIST", None)
+        return_dict["element_builders_by_filename"].pop("NIST", None)
+        return return_dict
+
+    def __setstate__(self, state):
+        self.__dict__ = state
+        self.initialize()
+
     def read_from_file(self, filename):
         self.filenames.append(filename)
         self.current_filename = filename
         self.element_builders_by_filename[self.current_filename] = {}
         self.material_builders_by_filename[self.current_filename] = {}
         f = open(filename, "r")
         line = f.readline()
```

### Comparing `opengate-10.0b7/opengate/geometry/solids.py` & `opengate-10.0b8/opengate/geometry/solids.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 from box import Box
 from scipy.spatial.transform import Rotation
 import sys
+import stl
+import logging
 
 from ..base import GateObject, process_cls, create_gate_object_from_dict
 from ..utility import g4_units
 from ..exception import fatal, warning
 import opengate_core as g4
 from ..decorators import requires_fatal
 
 from .utility import (
     ensure_is_g4_rotation,
     ensure_is_g4_translation,
+    vec_np_as_g4,
+    vec_g4_as_np,
 )
 
 
+logger = logging.getLogger(__name__)
+
+
 class SolidBase(GateObject):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.g4_solid = None
 
     def close(self):
         self.release_g4_references()
+        super().close()
 
     def release_g4_references(self):
         self.g4_solid = None
 
+    def __getstate__(self):
+        return_dict = super().__getstate__()
+        return_dict["g4_solid"] = None
+        return return_dict
+
     @property
     def solid_info(self):
         """Computes the properties of the solid associated with this volume."""
         # Note: This method only works in derived classes which implement the build_solid method.
         solid = self.build_solid()
         if solid is None:
             fatal(
@@ -437,14 +450,84 @@
         "dphi": (360 * g4_units.deg, {"doc": "Angle segment"}),
     }
 
     def build_solid(self):
         return g4.G4Tubs(self.name, self.rmin, self.rmax, self.dz, self.sphi, self.dphi)
 
 
+class TesselatedSolid(SolidBase):
+    """
+    https://geant4-userdoc.web.cern.ch/UsersGuides/ForApplicationDeveloper/html/Detector/Geometry/geomSolids.html?highlight=tesselated#tessellated-solids
+    """
+
+    user_info_defaults = {
+        "file_name": ("", {"doc": "Path and file name of the STL file."}),
+    }
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.g4_solid = None
+        self.facetArray = None
+        self.tessellated_solid = None
+
+    def read_file(self):
+        try:
+            box_mesh = stl.mesh.Mesh.from_file(self.file_name)
+        except Exception as e:
+            print(
+                "Error in TesselatedVolume. Could not read the file ",
+                self.file_name,
+                " Aborting.",
+            )
+            print("The error encountered was: ", e)
+            exit()
+        return box_mesh
+
+    def translate_mesh_to_center(self, mesh_to_translate):
+        # translate the mesh to the center of gravity
+        cog = mesh_to_translate.get_mass_properties()[1]
+        mesh_to_translate.translate(-cog)
+        return mesh_to_translate
+
+    def build_solid(self):
+        mm = g4_units.mm
+        box_mesh = self.read_file()
+        # translate the mesh to the center of gravity
+        box_mesh = self.translate_mesh_to_center(box_mesh)
+        # generate the tessellated solid
+        self.tessellated_solid = g4.G4TessellatedSolid(self.name)
+        # create an array of facets
+        self.facetArray = []
+        for vertex in box_mesh.vectors:
+            # Create the new facet
+            # ABSOLUTE =0
+            # RELATIVE =1
+            g4Facet = g4.G4TriangularFacet(
+                vec_np_as_g4(vertex[0]),
+                vec_np_as_g4(vertex[1]),
+                vec_np_as_g4(vertex[2]),
+                g4.G4FacetVertexType.ABSOLUTE,
+            )
+            self.facetArray.append(g4Facet)
+
+        # loop through facetArray and add the facets to the tessellated solid
+        for facet in self.facetArray:
+            self.tessellated_solid.AddFacet(facet)
+        # set the solid closed
+        self.tessellated_solid.SetSolidClosed(True)
+        logger.debug(
+            "Created Tesselated volume: {} with a volume of: {} [mm³]".format(
+                self.name, self.tessellated_solid.GetCubicVolume() * mm
+            )
+        )
+
+        return self.tessellated_solid
+
+
 class ImageSolid(SolidBase):
     """Utility to handle the solids of an ImageVolume.
     It is not intended to be used stand-alone, but only as a base class of ImageVolume.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -453,14 +536,21 @@
         self.half_size_mm = None
         self.half_spacing = None
 
         self.g4_solid_x = None
         self.g4_solid_y = None
         self.g4_solid_z = None
 
+    def __getstate__(self):
+        return_dict = super().__getstate__()
+        return_dict["g4_solid_x"] = None
+        return_dict["g4_solid_y"] = None
+        return_dict["g4_solid_z"] = None
+        return return_dict
+
     def close(self):
         self.release_g4_references()
         super().close()
 
     def release_g4_references(self):
         self.g4_solid_x = None
         self.g4_solid_y = None
@@ -499,7 +589,8 @@
 process_cls(ConsSolid)
 process_cls(PolyhedraSolid)
 process_cls(SphereSolid)
 process_cls(TrapSolid)
 process_cls(TrdSolid)
 process_cls(TubsSolid)
 process_cls(ImageSolid)
+process_cls(TesselatedSolid)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opengate-10.0b7/opengate/geometry/utility.py` & `opengate-10.0b8/opengate/geometry/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from anytree import RenderTree
 import numpy as np
 from scipy.spatial.transform import Rotation
 from box import Box
 
 import opengate_core as g4
-from ..definitions import __world_name__
+from ..definitions import __world_name__, __gate_list_objects__
 from ..exception import fatal
 
 """
 http://geant4-userdoc.web.cern.ch/geant4-userdoc/UsersGuides/ForApplicationDeveloper/html/Detector/Geometry/geomSolids.html#constructed-solid-geometry-csg-solids
 """
 
 
@@ -71,15 +71,15 @@
 def is_rotation_matrix(R):
     """
     https://stackoverflow.com/questions/53808503/how-to-test-if-a-matrix-is-a-rotation-matrix
     """
     # square matrix test
     if R.ndim != 2 or R.shape[0] != R.shape[1]:
         return False
-    should_be_identity = np.allclose(R.dot(R.T), np.identity(R.shape[0], np.float_))
+    should_be_identity = np.allclose(R.dot(R.T), np.identity(R.shape[0], np.float64))
     should_be_one = np.allclose(np.linalg.det(R), 1)
     return should_be_identity and should_be_one
 
 
 def vec_np_as_g4(v):
     return g4.G4ThreeVector(v[0], v[1], v[2])
 
@@ -143,33 +143,41 @@
     if isinstance(rotation, g4.G4RotationMatrix):
         return rotation
     else:
         return rot_np_as_g4(rotation)
 
 
 def ensure_is_g4_transform(
-    translation=[0, 0, 0], rotation=Rotation.identity().as_matrix()
+    translation=(0, 0, 0), rotation=Rotation.identity().as_matrix()
 ):
     return g4.G4Transform3D(
         ensure_is_g4_rotation(rotation), ensure_is_g4_translation(translation)
     )
 
 
 def get_translation_from_rotation_with_center(rot, center):
     center = np.array(center)
     t = rot.apply(-center) + center
     # note: apply is the same than rot.as_matrix().dot()
     return t
 
 
-def get_transform_orbiting(position, axis, angle_deg):
-    p = np.array(position)
-    rot = Rotation.from_euler(axis, angle_deg, degrees=True)
-    t = rot.apply(p)
-    return t, rot.as_matrix()
+def get_transform_orbiting(initial_position, axis, angle_deg):
+    angle_deg = list([angle_deg])
+    translations = []
+    rotations = []
+    for ang in angle_deg:
+        rot = Rotation.from_euler(axis, ang, degrees=True)
+        t = rot.apply(np.array(initial_position))
+        translations.append(t)
+        rotations.append(rot.as_matrix())
+    if len(translations) > 1:
+        return translations, rotations
+    else:
+        return translations[0], rotations[0]
 
 
 def get_transform_world_to_local(volume):
     """Calculate the rotation and translation needed
     to transform from the world reference frame
     into the local reference frame of this volume.
```

### Comparing `opengate-10.0b7/opengate/geometry/volumes.py` & `opengate-10.0b8/opengate/geometry/volumes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import re
-
+import os
 import numpy as np
 import itk
-from box import BoxList
 import json
 from anytree import NodeMixin
 from scipy.spatial.transform import Rotation
 
 import opengate_core as g4
 
-from ..base import GateObject, process_cls
+from ..base import DynamicGateObject, process_cls
 from . import solids
 from ..utility import ensure_filename_is_str
 from ..exception import fatal, warning
+from ..image import update_image_py_to_cpp, write_itk_image
 from ..image import create_3d_image, update_image_py_to_cpp
 from .utility import (
     vec_np_as_g4,
     rot_np_as_g4,
     ensure_is_g4_transform,
 )
-from ..decorators import requires_warning, requires_fatal, requires_attribute_fatal
+from ..decorators import requires_fatal, requires_attribute_fatal
 from ..definitions import __world_name__, __gate_list_objects__
-from ..logger import DEBUG
+from ..actors.dynamicactors import (
+    VolumeImageChanger,
+    VolumeTranslationChanger,
+    VolumeRotationChanger,
+)
 
 
 def _setter_hook_user_info_rotation(self, rotation_user):
     """Internal function associated with user_info rotation to check its validity."""
     if rotation_user is None:
         rotation = [Rotation.identity().as_matrix()]
     elif isinstance(rotation_user, (np.matrix, np.ndarray)) and rotation_user.shape == (
@@ -116,15 +120,15 @@
 
 
 def _setter_hook_ensure_array(self, input):
     return np.asarray(input)  # becomes dtype='<U32'
 
 
 # inherit from NodeMixin to turn the class into a tree node
-class VolumeBase(GateObject, NodeMixin):
+class VolumeBase(DynamicGateObject, NodeMixin):
     """
     Store information about a geometry volume:
     - G4 objects: Solid, LogicalVolume, PhysicalVolume
     - user parameters: user_info
     - additional data such as: mother, material etc
     """
 
@@ -141,14 +145,15 @@
             [[0, 0, 0]],
             {
                 "doc": "3-component vector or list of such vectors defining the translation "
                 "w.r.t. the mother. If translation is a list of vectors, "
                 "the volume will be repeeted once for each translation vector.",
                 "setter_hook": _setter_hook_user_info_translation,
                 "getter_hook": _getter_hook_user_info_translation,
+                "dynamic": True,
             },
         ),
         "color": (
             [1, 1, 1, 1],
             {
                 "doc": (
                     "4 component vector defining the volume's color in visual rendering. "
@@ -161,14 +166,15 @@
             {
                 "doc": "3x3 rotation matrix or list of such matrices. "
                 "The matrix (matrices) should be np.array or np.matrix."
                 "If a list of matrices is provided, the volume will be repeated, "
                 "once for each rotation vector.",
                 "setter_hook": _setter_hook_user_info_rotation,
                 "getter_hook": _getter_hook_user_info_rotation,
+                "dynamic": True,
             },
         ),
         "build_physical_volume": (
             True,
             {
                 "doc": "Boolean flag (True/False) whether G4 should build a physical volume.",
                 "type": bool,
@@ -188,15 +194,15 @@
         # GateObject base class digests all user info provided as kwargs
         super().__init__(*args, **kwargs)
 
         # if a template volume is provided, clone all user info items from it
         # except for the name of course
         if "template" in kwargs:
             # FIXME: use from_dictionary()
-            self.clone_user_info(kwargs["template"])
+            self.copy_user_info(kwargs["template"])
             # put back user infos which were explicitly passed as keyword argument
             for k in self.user_info.keys():
                 if k != "name":
                     try:
                         setattr(self, k, kwargs[k])
                     except KeyError:
                         pass
@@ -214,21 +220,33 @@
         self.g4_vis_attributes = None
         # this list contains all physical volumes (in case of repeated volume)
         self.g4_physical_volumes = []
         self.g4_material = None
 
     def close(self):
         self.release_g4_references()
+        super().close()
 
     def release_g4_references(self):
         self.g4_logical_volume = None
         self.g4_vis_attributes = None
         self.g4_physical_volumes = []
         self.g4_material = None
 
+    def __getstate__(self):
+        return_dict = super().__getstate__()
+        # Reset the following references to None because they cannot be pickled
+        # They created when running a simulation
+        return_dict["g4_logical_volume"] = None
+        return_dict["g4_vis_attributes"] = None
+        return_dict["g4_physical_volumes"] = None
+        return_dict["g4_material"] = None
+        return_dict["volume_engine"] = None
+        return return_dict
+
     def _update_node(self):
         """Internal method which retrieves the volume object
         from the volume manager based on the mother's name stored as user info 'mother'
         """
         try:
             self.parent = self.volume_manager.get_volume(self.mother)
         except KeyError:
@@ -244,14 +262,20 @@
             self.volume_manager.update_volume_tree()
         except AttributeError:
             fatal(
                 f"Unable to determine the world volume to which volume named {self.name} belongs. "
                 "Probably the volume has not yet been added to the simulation. "
             )
 
+    # FIXME: maybe store reference to simulation directly, rather than reference to volume_manager?
+    @property
+    @requires_fatal("volume_manager")
+    def simulation(self):
+        return self.volume_manager.simulation
+
     @property
     def volume_type(self):
         return type(self).__name__
 
     @property
     def world_volume(self):
         self._request_volume_tree_update()
@@ -276,17 +300,31 @@
 
     @property
     def ancestor_volumes(self):
         self._request_volume_tree_update()
         return self.ancestors[1:]  # first item is volume tree root, not a real volume
 
     @property
+    def children_volumes(self):
+        self._request_volume_tree_update()
+        return self.children
+
+    @property
     def number_of_repetitions(self):
         return len(self.user_info["translation"])
 
+    def get_g4_physical_volume(self, index):
+        try:
+            return self.g4_physical_volumes[index]
+        except IndexError:
+            fatal(
+                f"No physical volume with repetition index {index} "
+                f"found in volume {self.name}. "
+            )
+
     @property
     def translation_list(self):
         """Utility property which always returns a list of translations,
         even if the volume is not repeated and has thus only one translation vector.
         """
         len_rot = len(self.user_info["rotation"])
         if len_rot > 1 and len(self.user_info["translation"]) == 1:
@@ -309,14 +347,15 @@
     def g4_region(self):
         if self.g4_logical_volume is None:
             return None
         else:
             return self.g4_logical_volume.GetRegion()
 
     # shortcut to first physical volume
+    # FIXME: remove this shortcut. confusingly similar to self.g4_physical_volumes
     @property
     def g4_physical_volume(self):
         return self.g4_physical_volumes[0]
 
     # shortcuts to G4 variants of user info items 'translation' and 'rotation'
     @property
     def g4_translation(self):
@@ -411,14 +450,43 @@
             volume_name,  # volume name
             self.mother_g4_logical_volume,  # mother volume or None if World
             False,  # no boolean operation # FIXME for BooleanVolume ?
             copy_index,  # copy number
             self.volume_manager.simulation.check_volumes_overlap,
         )  # overlaps checking
 
+    def create_changers(self):
+        changers = super().create_changers()
+        for dp in self.dynamic_params.values():
+            if dp["extra_params"]["auto_changer"] is True:
+                if "translation" in dp:
+                    new_changer = VolumeTranslationChanger(
+                        name=f"{self.name}_volume_translation_changer_{len(changers)}",
+                        translations=dp["translation"],
+                        attached_to=self,
+                        volume_manager=self.volume_manager,
+                        repetition_index=dp["extra_params"].pop("repetition_index", 0),
+                    )
+                    changers.append(new_changer)
+                if "rotation" in dp:
+                    new_changer = VolumeRotationChanger(
+                        name=f"{self.name}_volume_translation_changer_{len(changers)}",
+                        attached_to=self,
+                        volume_manager=self.volume_manager,
+                        rotations=dp["rotation"],
+                        repetition_index=dp["extra_params"].pop("repetition_index", 0),
+                    )
+                    changers.append(new_changer)
+            else:
+                warning(
+                    f"You need to manually create a changer for dynamic parametrisation {dp} "
+                    f"of volume '{self.name}'."
+                )
+        return changers
+
     # set physical properties in this (logical) volume
     # behind the scenes, this will create a region and associate this volume with it
     @requires_fatal("volume_manager")
     def set_production_cut(self, particle_name, value):
         self.volume_manager.simulation.physics_manager.set_production_cut(
             self.name, particle_name, value
         )
@@ -478,14 +546,17 @@
                         g4t,
                         copy_index=i,
                     ),
                 )
         else:
             super().construct_physical_volume()
 
+    def add_dynamic_parametrisation(self, repetition_index=0, **params):
+        super().add_dynamic_parametrisation(repetition_index=repetition_index, **params)
+
 
 class BooleanVolume(RepeatableVolume, solids.BooleanSolid):
     """Volume resulting from a boolean operation of the solids contained in two volumes."""
 
 
 # Function to handle boolean operations on volumes
 # They create a new volume object, but the actual g4_solid is only created when the volume's
@@ -583,14 +654,18 @@
     """Volume with a symmetric trapezoidal shape."""
 
 
 class TubsVolume(RepeatableVolume, solids.TubsSolid):
     """Volume with a tube or cylindrical section shape."""
 
 
+class TesselatedVolume(RepeatableVolume, solids.TesselatedSolid):
+    """Volume based on a mesh volume by reading an STL file."""
+
+
 class RepeatParametrisedVolume(VolumeBase):
     """
     Volume created from another volume via translations.
     """
 
     user_info_defaults = {
         "linear_repeat": (
@@ -696,15 +771,15 @@
             [[-np.inf, np.inf, "G4_AIR"]],
             {
                 "doc": "FIXME",
             },
         ),
         "image": (
             "",
-            {"doc": "Path to the image file", "is_input_file": True},
+            {"doc": "Path to the image file", "is_input_file": True, "dynamic": True},
         ),
         "dump_label_image": (
             None,
             {
                 "doc": "Path at which the image containing material labels should be saved. "
                 "Set to None to dump no image."
             },
@@ -725,50 +800,67 @@
         self.g4_physical_y = None
         self.g4_physical_z = None
         self.g4_logical_x = None
         self.g4_logical_y = None
         self.g4_logical_z = None
         self.g4_voxel_param = None
 
+    def __getstate__(self):
+        return_dict = super().__getstate__()
+        return_dict["g4_physical_x"] = None
+        return_dict["g4_physical_y"] = None
+        return_dict["g4_physical_z"] = None
+        return_dict["g4_logical_x"] = None
+        return_dict["g4_logical_y"] = None
+        return_dict["g4_logical_z"] = None
+        return_dict["g4_voxel_param"] = None
+        return return_dict
+
     def close(self):
         self.release_g4_references()
         super().close()
 
     def release_g4_references(self):
         self.g4_logical_x = None
         self.g4_logical_y = None
         self.g4_logical_z = None
         self.g4_physical_x = None
         self.g4_physical_y = None
         self.g4_physical_z = None
         self.g4_voxel_param = None
 
     # @requires_fatal('itk_image')
+    # FIXME: replace this property by function in opengate.image
     @property
     def size_pix(self):
         return np.array(itk.size(self.itk_image)).astype(int)
 
     # @requires_fatal('itk_image')
+    # FIXME: replace this property by function in opengate.image
     @property
     def spacing(self):
         return np.array(self.itk_image.GetSpacing())
 
     @requires_fatal("volume_engine")
     def construct(self):
-        self.process_input_image()
+        self.material_to_label_lut = self.create_material_to_label_lut()
+        # make sure the materials are created in Geant4
+        for m in self.material_to_label_lut:
+            self.volume_manager.find_or_build_material(m)
+        self.itk_image = self.read_input_image()
+        self.label_image = self.create_label_image()
         if self.dump_label_image:
             self.save_label_image()
         # set attributes of the solid
         self.half_size_mm = 0.5 * self.size_pix * self.spacing
         self.half_spacing = 0.5 * self.spacing
         self.construct_material()
         self.construct_solid()
         self.construct_logical_volume()
-        # create self.g4_voxel_param
-        self._initialize_image_parameterisation()  # requires self.g4_logical_volume to be set before
+        self.g4_voxel_param = self.create_image_parametrisation()
         self.construct_physical_volume()
 
     def construct_physical_volume(self):
         super().construct_physical_volume()
 
         self.g4_physical_y = g4.G4PVReplica(
             self.name + "_Y",
@@ -809,109 +901,175 @@
         self.g4_logical_y = g4.G4LogicalVolume(
             self.g4_solid_y, self.g4_material, self.name + "_log_Y"
         )
         self.g4_logical_z = g4.G4LogicalVolume(
             self.g4_solid_z, self.g4_material, self.name + "_log_Z"
         )
 
-    def process_input_image(self):
-        # read image
-        self.itk_image = itk.imread(ensure_filename_is_str(self.image))
-
+    def create_material_to_label_lut(self, material=None, voxel_materials=None):
+        if voxel_materials is None:
+            voxel_materials = self.voxel_materials
+        if material is None:
+            material = self.material
         # prepare a LUT from material name to label
-        self.material_to_label_lut = {}
-        self.material_to_label_lut[self.material] = 0  # initialize with label 0
+        material_to_label_lut = {}
+        material_to_label_lut[material] = 0  # initialize with label 0
 
         # sort voxel_materials according to lower bounds
-        sort_index = np.argsort([row[0] for row in self.voxel_materials])
-        voxel_materials_sorted = [self.voxel_materials[i] for i in sort_index]
+        voxel_materials_sorted = sorted(voxel_materials, key=lambda x: x[0])
+
+        lower_bounds = np.array([row[0] for row in voxel_materials_sorted])
+        upper_bounds = np.array([row[1] for row in voxel_materials_sorted])
+        if not (lower_bounds[1:] >= upper_bounds[:-1]).all():
+            fatal(f"Overlapping intervals in voxel_materials of volume {self.name}.")
 
         # fill the LUT
         i = 1
         for row in voxel_materials_sorted:
-            if row[2] not in self.material_to_label_lut:
-                self.material_to_label_lut[row[2]] = i
+            if row[2] not in material_to_label_lut:
+                material_to_label_lut[row[2]] = i
                 i += 1
 
-        # create label image with same size as input image
-        self.label_image = create_3d_image(
-            self.size_pix, self.spacing, pixel_type="unsigned short", fill_value=0
-        )
-
-        # get numpy array view of input and output itk images
-        input = itk.array_view_from_image(self.itk_image)
-        output = itk.array_view_from_image(self.label_image)
-
-        # assign labels to output image
-        # feed the material name through the LUT to get the label
-        # this also alters label_image because output is an array_view
-        for row in self.voxel_materials:
-            output[
-                (input >= float(row[0])) & (input < float(row[1]))
-            ] = self.material_to_label_lut[row[2]]
+        return material_to_label_lut
+
+    def read_input_image(self, path=None):
+        if path is None:
+            itk_image = itk.imread(ensure_filename_is_str(self.image))
+            self.itk_image = itk_image
+        else:
+            itk_image = itk.imread(ensure_filename_is_str(path))
+        return itk_image
+
+    def create_label_image(self, itk_image=None):
+        # read image
+        if itk_image is None:
+            if self.itk_image is None:
+                self.itk_image = self.read_input_image()
+            itk_image = self.itk_image
+
+        if self.material_to_label_lut is None:
+            self.material_to_label_lut = self.create_material_to_label_lut()
+
+        # sort voxel_materials according to lower bounds
+        voxel_materials_sorted = sorted(self.voxel_materials, key=lambda x: x[0])
+
+        # find gaps in the voxels materials intervals
+        # upper bounds that are not also lower bounds of the subsequent interval
+        bins = [row[0] for row in voxel_materials_sorted]
+        # additional bins are those where an upper interval boundary
+        # does not correspond to the next lower interval boundary
+        additional_bins = set([row[1] for row in voxel_materials_sorted]).difference(
+            bins
+        )
+        bins.extend(additional_bins)
+        labels = [self.material_to_label_lut[row[2]] for row in voxel_materials_sorted]
+        labels.extend(
+            len(additional_bins) * [0]
+        )  # additional bins should have label 0,
+        # i.e. the volume's standard material
+        # np.digitize function requires bins in ascending order -> sort
+        bins_sorted = []
+        labels_sorted = [0]  # label 0 for voxel values below lowest interval
+        for b, l in sorted(zip(bins, labels), key=lambda pair: pair[0]):
+            bins_sorted.append(b)
+            labels_sorted.append(l)
+
+        # get numpy array view of input itk image
+        input_image = itk.array_view_from_image(itk_image)
+
+        label_image_arr = np.array(labels_sorted, dtype=np.ushort)[
+            np.digitize(input_image, bins=bins_sorted)
+        ]
+
+        label_image = itk.image_from_array(label_image_arr)
+        label_image.CopyInformation(itk_image)
+        return label_image
+
+    def create_image_parametrisation(self, label_image=None):
+        if label_image is None:
+            if self.label_image is None:
+                self.label_image = self.create_label_image()
+            label_image = self.label_image
+        # initialize parametrisation
+        g4_voxel_param = g4.GateImageNestedParameterisation()
+
+        # send image to cpp size
+        update_image_py_to_cpp(label_image, g4_voxel_param.cpp_edep_image, True)
+        g4_voxel_param.initialize_image()
+        g4_voxel_param.initialize_material(list(self.material_to_label_lut.keys()))
+
+        return g4_voxel_param
+
+    def update_label_image(self, label_image):
+        """Needed for dynamic image parametrisation."""
+        # send image to cpp size
+        update_image_py_to_cpp(label_image, self.g4_voxel_param.cpp_edep_image, True)
+        self.g4_voxel_param.initialize_image()
 
     def save_label_image(self, path=None):
         # dump label image ?
         if path is None:
             if self.volume_manager is None:
                 fatal(
                     f"Cannot save label image of ImageVolume {self.name}. "
                     f"Either provide a path or add the volume to the simulation. "
                 )
-            path = (
-                self.volume_manager.simulation.get_output_path()
-                / f"label_to_material_lut_{self.name}.json"
-            )
+            root, ext = os.path.splitext(self.dump_label_image)
+            # path = (
+            #    self.volume_manager.simulation.get_output_path()
+            #    / f"label_to_material_lut_{self.name}.json"
+            # )
+            path = root + ".json"
         if self.label_image is None:
-            self.process_input_image()
+            self.create_label_image()
 
         self.label_image.SetOrigin(self.itk_image.GetOrigin())  # set origin as in input
         # FIXME: should write image into output dir
-        itk.imwrite(self.label_image, str(self.dump_label_image))
+        write_itk_image(self.label_image, str(self.dump_label_image))
         with open(path, "w") as f:
             json.dump(self.material_to_label_lut, f)
 
         # re-compute image origin such that it is centered at 0
         self.label_image.SetOrigin(
             -(self.size_pix * self.spacing) / 2.0 + self.spacing / 2.0
         )
 
-    @requires_fatal("itk_image")
-    @requires_fatal("label_image")
-    @requires_fatal("volume_manager")
-    def _initialize_image_parameterisation(self):
-        """
-        From the input image, a label image is computed with each label
-        associated with a material.
-        The label image is initialized with label 0, corresponding to the first material
-        Correspondence from voxel value to material is given by a list of interval [min_value, max_value, material_name]
-        all pixels with values between min (included) and max (not included)
-        will be associated with the given material
-        """
-        if self.label_image is None:
-            self.process_input_image()
-
-        # make sure the materials are created in Geant4
-        for m in self.material_to_label_lut:
-            self.volume_manager.find_or_build_material(m)
-
-        # compute image origin such that it is centered at 0
-        self.label_image.SetOrigin(
-            -(self.size_pix * self.spacing) / 2.0 + self.spacing / 2.0
-        )
-
-        # initialize parametrisation
-        self.g4_voxel_param = g4.GateImageNestedParameterisation()
-
-        # send image to cpp size
-        update_image_py_to_cpp(
-            self.label_image, self.g4_voxel_param.cpp_edep_image, True
-        )
-        self.g4_voxel_param.initialize_image()
-        self.g4_voxel_param.initialize_material(list(self.material_to_label_lut.keys()))
+    def create_changers(self):
+        # get the changers from the mother classes and append those specific to the ImageVolume class
+        changers = super().create_changers()
+        counter = 0
+        for dp in self.dynamic_params.values():
+            if dp["extra_params"]["auto_changer"] is True:
+                if "image" in dp:
+                    # create a LUT of image parametrisations
+                    label_image = {}
+                    for path_to_image in set(dp["image"]):
+                        itk_image = self.read_input_image(path_to_image)
+                        label_image[path_to_image] = self.create_label_image(itk_image)
+                    new_changer = VolumeImageChanger(
+                        name=f"{self.name}_volume_image_changer_{len(changers)}",
+                        attached_to=self,
+                        volume_manager=self.volume_manager,
+                        images=dp["image"],
+                        label_image=label_image,
+                    )
+                    changers.append(new_changer)
+                    counter += 1
+            else:
+                warning(
+                    f"You need to manually create a changer for dynamic parametrisation {dp} "
+                    f"of volume '{self.name}'."
+                )
+        if counter > 1:
+            warning(
+                f"You have provided multiple dynamic image parametrisation (4D image) "
+                f"in the {type(self).__name__} named {self.name}. "
+                f"Consider verifying if this is intentional. "
+            )
+        return changers
 
 
 class ParallelWorldVolume(NodeMixin):
     def __init__(self, name, volume_manager):
         super().__init__()
         self.name = name
         self.volume_manager = volume_manager
@@ -927,14 +1085,21 @@
     def release_g4_references(self):
         self.g4_world_phys_vol = None
         self.g4_world_log_vol = None
 
     def close(self):
         self.release_g4_references()
 
+    def __getstate__(self):
+        return_dict = self.__dict__
+        return_dict["g4_world_phys_vol"] = None
+        return_dict["g4_world_log_vol"] = None
+        return_dict["parallel_world_engine"] = None
+        return return_dict
+
     @requires_fatal("parallel_world_engine")
     def construct(self):
         # get the physical volume through the parallel world engine
         # do not construct it
         self.g4_world_phys_vol = self.parallel_world_engine.GetWorld()
         self.g4_world_log_vol = self.g4_world_phys_vol.GetLogicalVolume()
 
@@ -946,19 +1111,25 @@
 # inherit from NodeMixin turn the class into a tree node
 class VolumeTreeRoot(NodeMixin):
     """Small class to provide a root for the volume tree."""
 
     def __init__(self, volume_manager) -> None:
         super().__init__()
         self.volume_manager = volume_manager
+        self.volume_engine = None
         self.name = "volume_tree_root"
         self.parent = None  # None means this is a tree root
 
+    def __getstate__(self):
+        return_dict = self.__dict__
+        return_dict["volume_engine"] = None
+        return return_dict
+
     def close(self):
-        pass
+        self.volume_engine = None
 
 
 # The following lines make sure that all classes which
 # inherit from the GateObject base class are processed upon importing opengate.
 # In this way, all properties corresponding to the class's user_info dictionary
 # will be created.
 # This ensures, e.g., that auto-completion in interactive python consoles
@@ -972,7 +1143,8 @@
 process_cls(PolyhedraVolume)
 process_cls(SphereVolume)
 process_cls(TrapVolume)
 process_cls(TrdVolume)
 process_cls(TubsVolume)
 process_cls(RepeatParametrisedVolume)
 process_cls(ImageVolume)
+process_cls(TesselatedVolume)
```

### Comparing `opengate-10.0b7/opengate/image.py` & `opengate-10.0b8/opengate/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,14 +329,18 @@
 
 
 def divide_itk_images(
     img1_numerator, img2_denominator, filterVal=0, replaceFilteredVal=0
 ):
     imgarr1 = itk.array_view_from_image(img1_numerator)
     imgarr2 = itk.array_view_from_image(img2_denominator)
+    if imgarr1.shape != imgarr2.shape:
+        fatal(
+            f"Cannot divide images of different shape. Found {imgarr1.shape} vs. {imgarr2.shape}."
+        )
     imgarrOut = imgarr1.copy()
     L_filterInv = imgarr2 != filterVal
     imgarrOut[L_filterInv] = np.divide(imgarr1[L_filterInv], imgarr2[L_filterInv])
 
     imgarrOut[np.invert(L_filterInv)] = replaceFilteredVal
     imgarrOut = itk.image_from_array(imgarrOut)
     imgarrOut.CopyInformation(img1_numerator)
@@ -408,7 +412,14 @@
     return np.array_equal(arr1, arr2)
 
 
 def compare_itk_image(filename1, filename2):
     im1 = itk.imread(filename1)
     im2 = itk.imread(filename2)
     return compare_itk_image_info(im1, im2) and compare_itk_image_content(im1, im2)
+
+
+def write_itk_image(img, file_path):
+    # TODO: check if filepath exists
+    # TODO: add metadata to file header
+    file_path = str(file_path)
+    itk.imwrite(img, file_path)
```

### Comparing `opengate-10.0b7/opengate/logger.py` & `opengate-10.0b8/opengate/logger.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/mac/default_visu_commands.mac` & `opengate-10.0b8/opengate/mac/default_visu_commands.mac`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/managers.py` & `opengate-10.0b8/opengate/managers.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,47 +23,59 @@
 from .geometry.materials import MaterialDatabase
 from .image import (
     create_image_with_volume_extent,
     create_image_with_extent,
     voxelize_volume,
     update_image_py_to_cpp,
     get_cpp_image,
+    write_itk_image,
 )
 from .utility import (
     assert_unique_element_name,
     g4_units,
     indent,
     read_mac_file_to_commands,
     ensure_directory_exists,
     ensure_filename_is_str,
+    insert_suffix_before_extension,
 )
 from .logger import INFO, log
-from .physics import Region, cut_particle_names
+from .physics import Region, OpticalSurface, cut_particle_names
 from .userinfo import UserInfo
 from .serialization import dump_json, dumps_json, loads_json, load_json
 from .processing import dispatch_to_subprocess
 
 from .geometry.volumes import (
     VolumeBase,
     BoxVolume,
     SphereVolume,
     TrapVolume,
     ImageVolume,
     TubsVolume,
     PolyhedraVolume,
     HexagonVolume,
+    TesselatedVolume,
     ConsVolume,
     TrdVolume,
     BooleanVolume,
     RepeatParametrisedVolume,
     ParallelWorldVolume,
     VolumeTreeRoot,
 )
 
 
+particle_names_Gate_to_G4 = {
+    "gamma": "gamma",
+    "electron": "e-",
+    "positron": "e+",
+    "proton": "proton",
+    "neutron": "neutron",
+}
+
+
 def retrieve_g4_physics_constructor_class(g4_physics_constructor_class_name):
     """
     Dynamically create a class with the given PhysicList
     Only possible if the class exist in g4
     """
     # Retrieve the G4VPhysicsConstructor class
     try:
@@ -246,14 +258,19 @@
         # init the user info
         s = UserInfo("Source", source_type, name)
         # append to the list
         self.user_info_sources[name] = s
         # return the info
         return s
 
+    def initialize_before_g4_engine(self):
+        for source in self.user_info_sources.values():
+            if source.initialize_source_before_g4_engine:
+                source.initialize_source_before_g4_engine(source)
+
 
 class ActorManager:
     """
     Manage all the actors in the simulation
     """
 
     def __init__(self, simulation):
@@ -323,48 +340,53 @@
         "G4EmStandardPhysicsGS",
         "G4EmLowEPPhysics",
         "G4EmLivermorePhysics",
         "G4EmLivermorePolarizedPhysics",
         "G4EmPenelopePhysics",
         "G4EmDNAPhysics",
         "G4OpticalPhysics",
+        "G4GenericBiasingPhysics",
     ]
 
     special_physics_constructor_classes = {}
     special_physics_constructor_classes["G4DecayPhysics"] = g4.G4DecayPhysics
-    special_physics_constructor_classes[
-        "G4RadioactiveDecayPhysics"
-    ] = g4.G4RadioactiveDecayPhysics
+    special_physics_constructor_classes["G4RadioactiveDecayPhysics"] = (
+        g4.G4RadioactiveDecayPhysics
+    )
     special_physics_constructor_classes["G4OpticalPhysics"] = g4.G4OpticalPhysics
     special_physics_constructor_classes["G4EmDNAPhysics"] = g4.G4EmDNAPhysics
+    special_physics_constructor_classes["G4GenericBiasingPhysics"] = (
+        g4.G4GenericBiasingPhysics
+    )
 
     def __init__(self, physics_manager, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.physics_manager = physics_manager
         # declare the attribute here as None;
         # set to dict in create_physics_list_classes()
         self.created_physics_list_classes = None
         self.create_physics_list_classes()
+        self.particle_with_biased_process_dictionary = {}
 
     def __getstate__(self):
         # This is needed because cannot be pickled.
-        dict_to_return = dict([(k, v) for k, v in self.__dict__.items()])
+        dict_to_return = super().__getstate__()
         dict_to_return["created_physics_list_classes"] = None
         return dict_to_return
 
     def __setstate__(self, d):
         self.__dict__ = d
         self.create_physics_list_classes()
 
     def create_physics_list_classes(self):
         self.created_physics_list_classes = {}
         for g4pc_name in self.available_g4_physics_constructors:
-            self.created_physics_list_classes[
-                g4pc_name
-            ] = create_modular_physics_list_class(g4pc_name)
+            self.created_physics_list_classes[g4pc_name] = (
+                create_modular_physics_list_class(g4pc_name)
+            )
 
     def get_physics_list(self, physics_list_name):
         if physics_list_name in self.created_physics_list_classes:
             physics_list = self.created_physics_list_classes[physics_list_name](
                 self.physics_manager.simulation.g4_verbose_level
             )
         else:
@@ -382,19 +404,25 @@
         # add special physics constructors
         for (
             spc,
             switch,
         ) in self.physics_manager.special_physics_constructors.items():
             if switch is True:
                 try:
-                    physics_list.ReplacePhysics(
-                        self.special_physics_constructor_classes[spc](
-                            self.physics_manager.simulation.g4_verbose_level
+                    if spc == "G4GenericBiasingPhysics":
+                        Bias = self.physics_manager.add_physics_bias()
+                        physics_list.RegisterPhysics(Bias)
+
+                    else:
+                        physics_list.ReplacePhysics(
+                            self.special_physics_constructor_classes[spc](
+                                self.physics_manager.simulation.g4_verbose_level
+                            )
                         )
-                    )
+
                 except KeyError:
                     fatal(
                         f"Special physics constructor named '{spc}' not found. Available constructors are: {self.special_physics_constructor_classes.keys()}."
                     )
         return physics_list
 
     def dump_info_physics_lists(self):
@@ -444,15 +472,25 @@
                 "doc": "Maximum energy for secondary particle production. If None, physics list default is used."
             },
         ),
         "optical_properties_file": (
             Path(os.path.dirname(__file__)) / "data" / "OpticalProperties.xml",
             {
                 "doc": "Path to the xml file containing the optical material properties to be used by G4OpticalPhysics. "
-                "Default: file shipped with Gate.",
+                "Default: file shipped with GATE.",
+                "is_input_file": True,
+            },
+        ),
+        "surface_properties_file": (
+            Path(os.path.dirname(__file__)) / "data" / "SurfaceProperties.xml",
+            {
+                "doc": "Path to the xml file containing the surface material properties to be used by "
+                "optical surface, i.e. G4LogicalBorderSurface."
+                f"The default file shipped with GATE located is in "
+                f"{Path(os.path.dirname(__file__)) / 'data' / 'SurfaceProperties.xml'}",
                 "is_input_file": True,
             },
         ),
         "user_limits_particles": (
             Box(
                 [
                     ("all", False),
@@ -493,14 +531,29 @@
                     for spc in PhysicsListManager.special_physics_constructor_classes
                 ]
             ),
             {
                 "doc": "Special physics constructors to be added to the physics list, e.g. G4Decay, G4OpticalPhysics. "
             },
         ),
+        "processes_to_bias": (
+            Box(
+                [
+                    ("all", None),
+                    ("all_charged", None),
+                    ("gamma", None),
+                    ("electron", None),
+                    ("positron", None),
+                    ("proton", None),
+                ]
+            ),
+            {
+                "doc": "Define the process to bias (if wanted) on the different particle types."
+            },
+        ),
     }
 
     def __init__(self, simulation, *args, **kwargs):
         super().__init__(name="physics_manager", *args, **kwargs)
 
         # Keep a pointer to the current simulation
         self.simulation = simulation
@@ -512,28 +565,41 @@
         # Dictionary to quickly find the region to which a volume is associated.
         # This dictionary is updated by the region's associate_volume method.
         # Do not update manually!
         # key=volume_name, value=region=object
         # NB: It is well-defined because each volume has only one region.
         self.volumes_regions_lut = {}
 
+        # dictionary containing all the optical surface objects
+        self.optical_surfaces = {}
+
     def reset(self):
         self.__init__(self.simulation)
 
     def to_dictionary(self):
         d = super().to_dictionary()
         d["regions"] = dict([(k, v.to_dictionary()) for k, v in self.regions.items()])
+        d["optical_surfaces"] = dict(
+            [(k, v.to_dictionary()) for k, v in self.optical_surfaces.items()]
+        )
         return d
 
     def from_dictionary(self, d):
         self.reset()
         super().from_dictionary(d)
         for r in d["regions"].values():
             region = self.add_region(r["user_info"]["name"])
             region.from_dictionary(r)
+        for s in d["optical_surfaces"].values():
+            optical_surface = self.add_optical_surface(
+                s["user_info"]["volume_from"],
+                s["user_info"]["volume_to"],
+                s["user_info"]["g4_surface_name"],
+            )
+            optical_surface.from_dictionary(s)
 
     def __str__(self):
         s = ""
         for k, v in self.user_info.items():
             s += f"{k}: {v}\n"
         return s
 
@@ -573,14 +639,25 @@
             for region in self.regions.values():
                 s += f"In region {region.name}:\n"
                 s += region.dump_production_cuts()
         else:
             s += "*** No cuts per region defined. ***\n"
         return s
 
+    def dump_optical_surfaces(self):
+        """
+        Prints each volume's name and its associated surfaces' details (surface name and connected volumes)
+        from the `volume_surfaces` dictionary in a readable format.
+        """
+        s = "The PhysicsManager is storing the following optical surfaces:\n\n"
+        for surf in self.optical_surfaces.values():
+            s += str(surf)
+            s += "\n"
+        return s
+
     @property
     def enable_decay(self):
         """Properties to quickly enable decay.
 
         Note that setting enable_decay to False means that the physics list
         default is used, i.e. it does not forcefully remove
         G4DecayPhysics from the physics list.
@@ -598,14 +675,41 @@
             )
 
     @enable_decay.setter
     def enable_decay(self, value):
         self.special_physics_constructors["G4DecayPhysics"] = value
         self.special_physics_constructors["G4RadioactiveDecayPhysics"] = value
 
+    def add_optical_surface(self, volume_from, volume_to, g4_surface_name):
+        """
+        Creates an object of class OpticalSurface with surface info.
+
+        :param volume_from: Name of the first volume (str)
+
+        :param volume_to: Name of the second volume (str)
+
+        :param g4_surface_name: Name of the surface between volumes (str)
+        """
+
+        name = "optical_surface_" + volume_from + "_" + volume_to
+
+        # Throw an error if the optical surface already exists
+        if name in self.optical_surfaces.keys():
+            fatal("An optical surface between these volumes already exists")
+
+        self.optical_surfaces[name] = OpticalSurface(
+            name=name,
+            physics_manager=self,
+            volume_from=volume_from,
+            volume_to=volume_to,
+            g4_surface_name=g4_surface_name,
+        )
+
+        return self.optical_surfaces[name]
+
     def add_region(self, name):
         if name in self.regions.keys():
             fatal("A region with this name already exists.")
         self.regions[name] = Region(name=name, physics_manager=self)
         return self.regions[name]
 
     def find_or_create_region(self, volume_name):
@@ -620,14 +724,57 @@
     def set_production_cut(self, volume_name, particle_name, value):
         if volume_name == self.simulation.world.name:
             self.global_production_cuts[particle_name] = value
         else:
             region = self.find_or_create_region(volume_name)
             region.production_cuts[particle_name] = value
 
+    def add_physics_bias(self):
+        self.processes_to_bias = self.user_info["processes_to_bias"]
+        BiasToApply = self.physics_list_manager.special_physics_constructor_classes[
+            "G4GenericBiasingPhysics"
+        ]()
+        list_of_particles = self.processes_to_bias.keys()
+        try:
+            if self.processes_to_bias["all"] != None:
+                for particle in list_of_particles:
+                    if particle != "all" and particle != "all_charged":
+                        BiasToApply.PhysicsBias(
+                            particle_names_Gate_to_G4[particle],
+                            self.processes_to_bias["all"],
+                        )
+            elif self.processes_to_bias["all_charged"] != None:
+                for particle in list_of_particles:
+                    if (
+                        particle != "all"
+                        and particle != "all_charged"
+                        and particle != "gamma"
+                        and particle != "neutron"
+                    ):
+                        BiasToApply.PhysicsBias(
+                            particle_names_Gate_to_G4[particle],
+                            self.processes_to_bias["all_charged"],
+                        )
+            else:
+                for particle in list_of_particles:
+                    list_of_process = self.processes_to_bias[particle]
+                    if list_of_process != None:
+                        BiasToApply.PhysicsBias(
+                            particle_names_Gate_to_G4[particle], list_of_process
+                        )
+        except KeyError:
+            fatal(
+                f"Found unknown particle name '{particle}' in processes_to_bias()."
+                f" Eligible names are "
+                + ", ".join(self.user_info_defaults["processes_to_bias"][0].keys())
+                + "."
+            )
+
+        return BiasToApply
+
     # set methods for the user_info parameters
     # logic: every volume with user_infos must be associated
     # with a region. If it does not yet have one, created it.
     # Outlook: These setter methods might be linked to properties
     # implemented in a future version of the Volume class
     def set_max_step_size(self, volume_name, max_step_size):
         region = self.find_or_create_region(volume_name)
@@ -674,19 +821,21 @@
     volume_types = {
         "BoxVolume": BoxVolume,
         "SphereVolume": SphereVolume,
         "TrapVolume": TrapVolume,
         "ImageVolume": ImageVolume,
         "TubsVolume": TubsVolume,
         "PolyhedraVolume": PolyhedraVolume,
+        "TextTesselatedVolume": TesselatedVolume,
         "HexagonVolume": HexagonVolume,
         "ConsVolume": ConsVolume,
         "TrdVolume": TrdVolume,
         "BooleanVolume": BooleanVolume,
         "RepeatParametrisedVolume": RepeatParametrisedVolume,
+        "TesselatedVolume": TesselatedVolume,
     }
 
     def __init__(self, simulation, *args, **kwargs):
         """
         Class that store geometry description.
         """
         self.simulation = simulation
@@ -769,14 +918,18 @@
     def parallel_world_names(self):
         return list(self.parallel_world_volumes.keys())
 
     @property
     def all_volume_names(self):
         return self.volume_names + self.parallel_world_names
 
+    @property
+    def dynamic_volumes(self):
+        return [vol for vol in self.volumes.values() if vol.is_dynamic]
+
     def get_volume(self, volume_name):
         try:
             return self.volumes[volume_name]
         except KeyError:
             try:
                 return self.parallel_world_volumes[volume_name]
             except KeyError:
@@ -926,15 +1079,15 @@
         "visu": (
             False,
             {
                 "doc": "Activate visualization? Note: Use low number of primaries if you activate visualization. Default: False"
             },
         ),
         "visu_type": (
-            "qt",
+            "vrml",
             {
                 "doc": "The type of visualization to be used.",
                 "available_values": (
                     "qt",
                     "vrml",
                     "gdml",
                     "vrml_file_only",
@@ -1019,14 +1172,21 @@
         "output_dir": (
             ".",
             {
                 "doc": "Directory to which any output is written, "
                 "unless an absolute path is provided for a specific output."
             },
         ),
+        "output_path_insert_suffix": (
+            True,
+            {
+                "doc": "Manipulates and inserts the name of the scored quantity into the filename. If False, the user defined output name is not changed."
+                "Default: True"
+            },
+        ),
         "store_json_archive": (
             False,
             {
                 "doc": "Automatically store a json file containing all parameters of the simulation after the run? "
                 "Default: False"
             },
         ),
@@ -1052,14 +1212,20 @@
         "g4_commands_after_init": (
             [],
             {
                 "doc": "Geant4 commands which will be called after the G4 runmanager has initialized the simulation.",
                 "required_type": str,
             },
         ),
+        "init_only": (
+            False,
+            {
+                "doc": "Start G4 engine initialisation but do not start the simulation.",
+            },
+        ),
     }
 
     def __init__(self, name="simulation"):
         """
         Main members are:
         - managers of volumes, physics, sources, actors and filters
         - the Geant4 objects will be only built during initialisation in SimulationEngine
@@ -1173,28 +1339,31 @@
         for f in input_files:
             # check for image header files (mhd) and add the corresponding raw files to the list
             if f.suffix == ".mhd":
                 input_files.append(f.parent.absolute() / Path(f.stem + ".raw"))
         for f in input_files:
             shutil.copy2(f, directory)
 
-    def get_output_path(self, path=None, is_file_or_directory="file"):
+    def get_output_path(self, path=None, is_file_or_directory="file", suffix=""):
         if path is None:
             # no input -> return global output directory
             p_out = Path(self.output_dir)
         else:
             # make sure type is Path
             p = Path(path)
             if not p.is_absolute():
                 # prepend the global output dir if p is relative
                 p_out = self.output_dir / p
             else:
                 # or just keep it
                 p_out = p
 
+        if self.output_path_insert_suffix:
+            p_out = insert_suffix_before_extension(p_out, suffix)
+
         # Make sure the directory exists
         if is_file_or_directory in ["file", "File", "f"]:
             n = len(p_out.parts) - 1  # last item is the filename
         elif is_file_or_directory in ["dir", "Dir", "directory", "d"]:
             n = len(p_out.parts)  # all items are part of the directory
         if len(p_out.parts) > 0 and n > 0:
             directory = Path(p_out.parts[0])
@@ -1223,14 +1392,18 @@
     def get_actor_user_info(self, name):
         s = self.actor_manager.get_actor_user_info(name)
         return s
 
     def add_volume(self, volume, name=None):
         return self.volume_manager.add_volume(volume, name)
 
+    # call this add optical surface, from_volume, to_volume,
+    def add_surface(self, volume_1, volume_2, surface_name):
+        return self.physics_manager.add_surface(volume_1, volume_2, surface_name)
+
     def add_parallel_world(self, name):
         self.volume_manager.add_parallel_world(name)
 
     def add_source(self, source_type, name):
         return self.source_manager.add_source(source_type, name)
 
     def add_actor(self, actor_type, name):
@@ -1258,14 +1431,15 @@
                 so it knows if it is running in a subprocess.
 
         Returns:
             :obj:SimulationOutput : The output of the simulation run.
         """
         with SimulationEngine(self) as se:
             se.new_process = start_new_process
+            se.init_only = self.init_only
             output = se.run_engine()
         return output
 
     def run(self, start_new_process=False):
         # if windows and MT -> fail
         if os.name == "nt" and self.multithreaded:
             fatal(
@@ -1277,14 +1451,15 @@
         if start_new_process is True:
             """Important: put the
             if __name__ == '__main__':
             at the beginning of the script
             https://britishgeologicalsurvey.github.io/science/python-forking-vs-spawn/
             """
 
+            log.info("Dispatching simulation to subprocess ...")
             self.output = dispatch_to_subprocess(self._run_simulation_engine, True)
         else:
             self.output = self._run_simulation_engine(False)
 
         # FIXME: should this not be done in a __setstate__ method?
         # put back the simulation object to all actors
         for actor in self.output.actors.values():
@@ -1342,23 +1517,30 @@
             outpath_mhd = outpath.parent / (outpath.stem + "_image.mhd")
 
             # write labels
             with open(outpath_json, "w") as outfile:
                 dump_json(labels, outfile, indent=4)
 
             # write image
-            itk.imwrite(image, ensure_filename_is_str(outpath_mhd))
+            write_itk_image(image, ensure_filename_is_str(outpath_mhd))
         else:
             outpath_mhd = "not_applicable"
 
         if return_path is True:
             return labels, image, outpath_mhd
         else:
             return labels, image
 
+    def initialize_source_before_g4_engine(self):
+        """
+        Some sources need to perform computation once everything is defined in user_info but *before* the
+        initialization of the G4 engine starts. This can be done via this function.
+        """
+        self.source_manager.initialize_before_g4_engine()
+
     def _get_voxelized_geometry(self, extent, spacing, margin):
         """Private method which returns a voxelized image of the simulation geometry
         given the extent, spacing and margin.
 
         The voxelization does not check which volume is voxelized.
         Every voxel will be assigned an ID corresponding to the material at this position
         in the world.
```

### Comparing `opengate-10.0b7/opengate/processing.py` & `opengate-10.0b8/opengate/processing.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/runtiming.py` & `opengate-10.0b8/opengate/runtiming.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/serialization.py` & `opengate-10.0b8/opengate/serialization.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/sources/beta_plus_spectra/F18/beta+_F18_tot.bs` & `opengate-10.0b8/opengate/sources/beta_plus_spectra/Rb82/beta+_Rb82_tot.bs`

 * *Files 26% similar despite different names*

```diff
@@ -1,333 +1,373 @@
----------------------------------------------------------------------------------------------
-
-BetaShape
-Version: 2.2 (05/2021)
-Author: X. Mougeot (xavier.mougeot@cea.fr)
-CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
-Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
-
----------------------------------------------------------------------------------------------
-
-Total beta + spectrum from the F-18 decay. See file of each transition for more details.
-
-Mean energy from the total beta + spectrum: 250.50 (21) keV
-
-E(keV)      dNtot/dE b+      unc.
-     0      0.00000e+00      0.00000e+00
-     2      3.21027e-05      5.04587e-08
-     4      1.11844e-04      1.75233e-07
-     6      1.98735e-04      3.10362e-07
-     8      2.83660e-04      4.41541e-07
-    10      3.64714e-04      5.65836e-07
-    12      4.41671e-04      6.82948e-07
-    14      5.14749e-04      7.93272e-07
-    16      5.84277e-04      8.97361e-07
-    18      6.50581e-04      9.95767e-07
-    20      7.13962e-04      1.08899e-06
-    22      7.74686e-04      1.17748e-06
-    24      8.32982e-04      1.26161e-06
-    26      8.89052e-04      1.34173e-06
-    28      9.43070e-04      1.41812e-06
-    30      9.95188e-04      1.49103e-06
-    32      1.04554e-03      1.56071e-06
-    34      1.09424e-03      1.62733e-06
-    36      1.14140e-03      1.69108e-06
-    38      1.18710e-03      1.75212e-06
-    40      1.23144e-03      1.81058e-06
-    42      1.27447e-03      1.86659e-06
-    44      1.31628e-03      1.92026e-06
-    46      1.35692e-03      1.97170e-06
-    48      1.39644e-03      2.02101e-06
-    50      1.43490e-03      2.06825e-06
-    52      1.47233e-03      2.11353e-06
-    54      1.50879e-03      2.15690e-06
-    56      1.54431e-03      2.19843e-06
-    58      1.57892e-03      2.23819e-06
-    60      1.61265e-03      2.27623e-06
-    62      1.64554e-03      2.31261e-06
-    64      1.67762e-03      2.34737e-06
-    66      1.70890e-03      2.38056e-06
-    68      1.73942e-03      2.41222e-06
-    70      1.76920e-03      2.44240e-06
-    72      1.79825e-03      2.47113e-06
-    74      1.82660e-03      2.49845e-06
-    76      1.85426e-03      2.52438e-06
-    78      1.88125e-03      2.54897e-06
-    80      1.90759e-03      2.57224e-06
-    82      1.93329e-03      2.59423e-06
-    84      1.95838e-03      2.61495e-06
-    86      1.98285e-03      2.63443e-06
-    88      2.00672e-03      2.65271e-06
-    90      2.03002e-03      2.66979e-06
-    92      2.05274e-03      2.68571e-06
-    94      2.07489e-03      2.70049e-06
-    96      2.09650e-03      2.71414e-06
-    98      2.11757e-03      2.72669e-06
-   100      2.13810e-03      2.73815e-06
-   102      2.15811e-03      2.74854e-06
-   104      2.17761e-03      2.75789e-06
-   106      2.19660e-03      2.76620e-06
-   108      2.21510e-03      2.77350e-06
-   110      2.23310e-03      2.77980e-06
-   112      2.25062e-03      2.78511e-06
-   114      2.26767e-03      2.78945e-06
-   116      2.28424e-03      2.79283e-06
-   118      2.30036e-03      2.79528e-06
-   120      2.31601e-03      2.79679e-06
-   122      2.33122e-03      2.79739e-06
-   124      2.34598e-03      2.79709e-06
-   126      2.36030e-03      2.79589e-06
-   128      2.37418e-03      2.79382e-06
-   130      2.38764e-03      2.79089e-06
-   132      2.40067e-03      2.78710e-06
-   134      2.41329e-03      2.78246e-06
-   136      2.42549e-03      2.77700e-06
-   138      2.43728e-03      2.77071e-06
-   140      2.44866e-03      2.76362e-06
-   142      2.45965e-03      2.75572e-06
-   144      2.47024e-03      2.74704e-06
-   146      2.48043e-03      2.73758e-06
-   148      2.49024e-03      2.72735e-06
-   150      2.49966e-03      2.71636e-06
-   152      2.50870e-03      2.70462e-06
-   154      2.51736e-03      2.69214e-06
-   156      2.52565e-03      2.67894e-06
-   158      2.53357e-03      2.66501e-06
-   160      2.54112e-03      2.65037e-06
-   162      2.54831e-03      2.63503e-06
-   164      2.55514e-03      2.61900e-06
-   166      2.56162e-03      2.60229e-06
-   168      2.56774e-03      2.58490e-06
-   170      2.57351e-03      2.56684e-06
-   172      2.57893e-03      2.54813e-06
-   174      2.58401e-03      2.52876e-06
-   176      2.58874e-03      2.50876e-06
-   178      2.59314e-03      2.48813e-06
-   180      2.59720e-03      2.46688e-06
-   182      2.60093e-03      2.44501e-06
-   184      2.60433e-03      2.42253e-06
-   186      2.60741e-03      2.39946e-06
-   188      2.61016e-03      2.37580e-06
-   190      2.61258e-03      2.35155e-06
-   192      2.61469e-03      2.32674e-06
-   194      2.61649e-03      2.30136e-06
-   196      2.61797e-03      2.27543e-06
-   198      2.61913e-03      2.24894e-06
-   200      2.61999e-03      2.22192e-06
-   202      2.62055e-03      2.19437e-06
-   204      2.62080e-03      2.16629e-06
-   206      2.62075e-03      2.13770e-06
-   208      2.62040e-03      2.10860e-06
-   210      2.61975e-03      2.07900e-06
-   212      2.61882e-03      2.04892e-06
-   214      2.61759e-03      2.01834e-06
-   216      2.61607e-03      1.98730e-06
-   218      2.61426e-03      1.95579e-06
-   220      2.61218e-03      1.92382e-06
-   222      2.60981e-03      1.89140e-06
-   224      2.60716e-03      1.85853e-06
-   226      2.60423e-03      1.82524e-06
-   228      2.60103e-03      1.79151e-06
-   230      2.59756e-03      1.75737e-06
-   232      2.59382e-03      1.72282e-06
-   234      2.58981e-03      1.68787e-06
-   236      2.58554e-03      1.65265e-06
-   238      2.58100e-03      1.61704e-06
-   240      2.57620e-03      1.58106e-06
-   242      2.57115e-03      1.54471e-06
-   244      2.56584e-03      1.50800e-06
-   246      2.56027e-03      1.47093e-06
-   248      2.55445e-03      1.43353e-06
-   250      2.54839e-03      1.39578e-06
-   252      2.54208e-03      1.35771e-06
-   254      2.53552e-03      1.31932e-06
-   256      2.52872e-03      1.28062e-06
-   258      2.52168e-03      1.24162e-06
-   260      2.51441e-03      1.20232e-06
-   262      2.50690e-03      1.16274e-06
-   264      2.49915e-03      1.12288e-06
-   266      2.49118e-03      1.08275e-06
-   268      2.48297e-03      1.04236e-06
-   270      2.47455e-03      1.00172e-06
-   272      2.46589e-03      9.60832e-07
-   274      2.45702e-03      9.19712e-07
-   276      2.44792e-03      8.78366e-07
-   278      2.43861e-03      8.36803e-07
-   280      2.42909e-03      7.95030e-07
-   282      2.41935e-03      7.53057e-07
-   284      2.40941e-03      7.10893e-07
-   286      2.39925e-03      6.68545e-07
-   288      2.38889e-03      6.26024e-07
-   290      2.37833e-03      5.83337e-07
-   292      2.36757e-03      5.40494e-07
-   294      2.35661e-03      4.97503e-07
-   296      2.34545e-03      4.54373e-07
-   298      2.33411e-03      4.11114e-07
-   300      2.32257e-03      3.67733e-07
-   302      2.31084e-03      3.24241e-07
-   304      2.29892e-03      2.80647e-07
-   306      2.28682e-03      2.36958e-07
-   308      2.27454e-03      1.93185e-07
-   310      2.26209e-03      1.49337e-07
-   312      2.24945e-03      1.05423e-07
-   314      2.23664e-03      6.14516e-08
-   316      2.22366e-03      1.74327e-08
-   318      2.21051e-03      3.17306e-08
-   320      2.19720e-03      7.59246e-08
-   322      2.18372e-03      1.20137e-07
-   324      2.17008e-03      1.64358e-07
-   326      2.15628e-03      2.08579e-07
-   328      2.14232e-03      2.52789e-07
-   330      2.12821e-03      2.96979e-07
-   332      2.11395e-03      3.41140e-07
-   334      2.09954e-03      3.85262e-07
-   336      2.08498e-03      4.29335e-07
-   338      2.07028e-03      4.73349e-07
-   340      2.05544e-03      5.17295e-07
-   342      2.04045e-03      5.61162e-07
-   344      2.02534e-03      6.04941e-07
-   346      2.01009e-03      6.48622e-07
-   348      1.99470e-03      6.92195e-07
-   350      1.97919e-03      7.35649e-07
-   352      1.96356e-03      7.78975e-07
-   354      1.94780e-03      8.22163e-07
-   356      1.93192e-03      8.65202e-07
-   358      1.91593e-03      9.08083e-07
-   360      1.89982e-03      9.50794e-07
-   362      1.88359e-03      9.93326e-07
-   364      1.86726e-03      1.03567e-06
-   366      1.85082e-03      1.07781e-06
-   368      1.83428e-03      1.11974e-06
-   370      1.81763e-03      1.16145e-06
-   372      1.80089e-03      1.20293e-06
-   374      1.78405e-03      1.24417e-06
-   376      1.76712e-03      1.28516e-06
-   378      1.75010e-03      1.32588e-06
-   380      1.73299e-03      1.36632e-06
-   382      1.71580e-03      1.40649e-06
-   384      1.69853e-03      1.44635e-06
-   386      1.68117e-03      1.48591e-06
-   388      1.66375e-03      1.52516e-06
-   390      1.64624e-03      1.56407e-06
-   392      1.62867e-03      1.60265e-06
-   394      1.61103e-03      1.64087e-06
-   396      1.59333e-03      1.67874e-06
-   398      1.57557e-03      1.71623e-06
-   400      1.55775e-03      1.75334e-06
-   402      1.53987e-03      1.79005e-06
-   404      1.52194e-03      1.82636e-06
-   406      1.50396e-03      1.86225e-06
-   408      1.48593e-03      1.89771e-06
-   410      1.46786e-03      1.93273e-06
-   412      1.44976e-03      1.96730e-06
-   414      1.43161e-03      2.00140e-06
-   416      1.41343e-03      2.03503e-06
-   418      1.39522e-03      2.06818e-06
-   420      1.37698e-03      2.10083e-06
-   422      1.35871e-03      2.13296e-06
-   424      1.34043e-03      2.16458e-06
-   426      1.32212e-03      2.19566e-06
-   428      1.30380e-03      2.22620e-06
-   430      1.28547e-03      2.25618e-06
-   432      1.26713e-03      2.28559e-06
-   434      1.24878e-03      2.31442e-06
-   436      1.23043e-03      2.34265e-06
-   438      1.21208e-03      2.37029e-06
-   440      1.19374e-03      2.39730e-06
-   442      1.17540e-03      2.42368e-06
-   444      1.15707e-03      2.44943e-06
-   446      1.13876e-03      2.47452e-06
-   448      1.12046e-03      2.49894e-06
-   450      1.10218e-03      2.52269e-06
-   452      1.08393e-03      2.54574e-06
-   454      1.06570e-03      2.56809e-06
-   456      1.04751e-03      2.58972e-06
-   458      1.02934e-03      2.61063e-06
-   460      1.01122e-03      2.63079e-06
-   462      9.93130e-04      2.65020e-06
-   464      9.75088e-04      2.66884e-06
-   466      9.57093e-04      2.68671e-06
-   468      9.39149e-04      2.70378e-06
-   470      9.21259e-04      2.72004e-06
-   472      9.03426e-04      2.73549e-06
-   474      8.85655e-04      2.75010e-06
-   476      8.67949e-04      2.76388e-06
-   478      8.50310e-04      2.77679e-06
-   480      8.32743e-04      2.78883e-06
-   482      8.15252e-04      2.79999e-06
-   484      7.97839e-04      2.81026e-06
-   486      7.80509e-04      2.81961e-06
-   488      7.63265e-04      2.82804e-06
-   490      7.46110e-04      2.83553e-06
-   492      7.29049e-04      2.84207e-06
-   494      7.12084e-04      2.84765e-06
-   496      6.95220e-04      2.85225e-06
-   498      6.78461e-04      2.85586e-06
-   500      6.61809e-04      2.85847e-06
-   502      6.45269e-04      2.86005e-06
-   504      6.28844e-04      2.86061e-06
-   506      6.12539e-04      2.86012e-06
-   508      5.96356e-04      2.85857e-06
-   510      5.80300e-04      2.85594e-06
-   512      5.64374e-04      2.85223e-06
-   514      5.48583e-04      2.84741e-06
-   516      5.32929e-04      2.84149e-06
-   518      5.17418e-04      2.83443e-06
-   520      5.02052e-04      2.82622e-06
-   522      4.86836e-04      2.81686e-06
-   524      4.71773e-04      2.80633e-06
-   526      4.56868e-04      2.79461e-06
-   528      4.42124e-04      2.78169e-06
-   530      4.27545e-04      2.76755e-06
-   532      4.13135e-04      2.75218e-06
-   534      3.98899e-04      2.73557e-06
-   536      3.84840e-04      2.71786e-06
-   538      3.70961e-04      2.69903e-06
-   540      3.57268e-04      2.67891e-06
-   542      3.43764e-04      2.65751e-06
-   544      3.30453e-04      2.63479e-06
-   546      3.17339e-04      2.61074e-06
-   548      3.04427e-04      2.58536e-06
-   550      2.91720e-04      2.55862e-06
-   552      2.79222e-04      2.53051e-06
-   554      2.66938e-04      2.50101e-06
-   556      2.54872e-04      2.47011e-06
-   558      2.43027e-04      2.43780e-06
-   560      2.31409e-04      2.40406e-06
-   562      2.20021e-04      2.36888e-06
-   564      2.08867e-04      2.33223e-06
-   566      1.97952e-04      2.29411e-06
-   568      1.87280e-04      2.25450e-06
-   570      1.76855e-04      2.21338e-06
-   572      1.66681e-04      2.17073e-06
-   574      1.56764e-04      2.12656e-06
-   576      1.47106e-04      2.08082e-06
-   578      1.37712e-04      2.03352e-06
-   580      1.28587e-04      1.98464e-06
-   582      1.19735e-04      1.93415e-06
-   584      1.11160e-04      1.88205e-06
-   586      1.02867e-04      1.82832e-06
-   588      9.48596e-05      1.77294e-06
-   590      8.71430e-05      1.71590e-06
-   592      7.97213e-05      1.65718e-06
-   594      7.25990e-05      1.59676e-06
-   596      6.57806e-05      1.53464e-06
-   598      5.92703e-05      1.47078e-06
-   600      5.30729e-05      1.40519e-06
-   602      4.71928e-05      1.33783e-06
-   604      4.16344e-05      1.26870e-06
-   606      3.64024e-05      1.19777e-06
-   608      3.15013e-05      1.12504e-06
-   610      2.69357e-05      1.05048e-06
-   612      2.27101e-05      9.74082e-07
-   614      1.88292e-05      8.95825e-07
-   616      1.52975e-05      8.15693e-07
-   618      1.21198e-05      7.33671e-07
-   620      9.30062e-06      6.49741e-07
-   622      6.84469e-06      5.63886e-07
-   624      4.75667e-06      4.76091e-07
-   626      3.04128e-06      3.86337e-07
-   628      1.70322e-06      2.94608e-07
-   630      7.47233e-07      2.00888e-07
-   632      1.78070e-07      1.05159e-07
- 633.9      0.00000e+00      0.00000e+00
+---------------------------------------------------------------------------------------------
+
+BetaShape
+Version: 2.2 (05/2021)
+Author: X. Mougeot (xavier.mougeot@cea.fr)
+CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
+Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
+
+---------------------------------------------------------------------------------------------
+
+Total beta + spectrum from the Rb-82 decay. See file of each transition for more details.
+
+Mean energy from the total beta + spectrum: 1473.0 (44) keV
+
+E(keV)      dNtot/dE b+      unc.
+     0      0.00000e+00      0.00000e+00
+     2      2.45580e-10      1.00034e-14
+     4      3.69889e-08      7.91242e-11
+     6      1.55129e-07      3.43312e-10
+     8      3.39884e-07      7.57271e-10
+    10      5.92074e-07      1.32099e-09
+    12      9.11450e-07      2.03448e-09
+    14      1.29802e-06      2.89773e-09
+    16      1.75173e-06      3.91075e-09
+    18      2.27030e-06      5.07283e-09
+    20      2.85477e-06      6.38440e-09
+    22      3.50471e-06      7.84545e-09
+    24      4.18416e-06      9.34821e-09
+    26      4.90816e-06      1.09638e-08
+    28      5.68249e-06      1.26944e-08
+    30      6.50671e-06      1.45399e-08
+    32      7.38076e-06      1.65004e-08
+    34      8.27548e-06      1.85103e-08
+    36      9.18513e-06      2.05402e-08
+    38      1.01268e-05      2.26422e-08
+    40      1.11007e-05      2.48163e-08
+    42      1.21009e-05      2.70604e-08
+    44      1.31307e-05      2.93757e-08
+    46      1.41608e-05      3.16753e-08
+    48      1.52113e-05      3.40193e-08
+    50      1.62783e-05      3.64064e-08
+    52      1.73640e-05      3.88374e-08
+    54      1.84684e-05      4.13124e-08
+    56      1.95833e-05      4.38069e-08
+    58      2.07018e-05      4.63079e-08
+    60      2.18323e-05      4.88363e-08
+    62      2.29748e-05      5.13920e-08
+    64      2.41291e-05      5.39750e-08
+    66      2.52935e-05      5.65846e-08
+    68      2.64581e-05      5.91891e-08
+    70      2.76305e-05      6.18107e-08
+    72      2.88105e-05      6.44495e-08
+    74      2.99969e-05      6.71049e-08
+    76      3.11904e-05      6.97773e-08
+    78      3.23878e-05      7.24572e-08
+    80      3.35876e-05      7.51401e-08
+    82      3.47914e-05      7.78334e-08
+    84      3.59998e-05      8.05373e-08
+    86      3.72126e-05      8.32517e-08
+    88      3.84300e-05      8.59767e-08
+    90      3.96469e-05      8.86990e-08
+    92      4.08665e-05      9.14278e-08
+    94      4.20891e-05      9.41631e-08
+    96      4.33145e-05      9.69048e-08
+    98      4.45422e-05      9.96528e-08
+   100      4.57712e-05      1.02403e-07
+   110      5.19344e-05      1.16195e-07
+   120      5.81180e-05      1.30031e-07
+   130      6.43096e-05      1.43886e-07
+   140      7.04999e-05      1.57737e-07
+   150      7.66819e-05      1.71570e-07
+   160      8.28505e-05      1.85372e-07
+   170      8.90019e-05      1.99136e-07
+   180      9.51334e-05      2.12854e-07
+   190      1.01243e-04      2.26522e-07
+   200      1.07328e-04      2.40134e-07
+   210      1.13388e-04      2.53689e-07
+   220      1.19421e-04      2.67183e-07
+   230      1.25427e-04      2.80614e-07
+   240      1.31404e-04      2.93980e-07
+   250      1.37352e-04      3.07278e-07
+   260      1.43271e-04      3.20509e-07
+   270      1.49159e-04      3.33670e-07
+   280      1.55015e-04      3.46758e-07
+   290      1.60841e-04      3.59775e-07
+   300      1.66634e-04      3.72715e-07
+   310      1.72394e-04      3.85580e-07
+   320      1.78122e-04      3.98368e-07
+   330      1.83816e-04      4.11079e-07
+   340      1.89475e-04      4.23708e-07
+   350      1.95099e-04      4.36256e-07
+   360      2.00687e-04      4.48720e-07
+   370      2.06239e-04      4.61099e-07
+   380      2.11754e-04      4.73393e-07
+   390      2.17233e-04      4.85601e-07
+   400      2.22674e-04      4.97718e-07
+   410      2.28076e-04      5.09746e-07
+   420      2.33439e-04      5.21683e-07
+   430      2.38763e-04      5.33526e-07
+   440      2.44046e-04      5.45273e-07
+   450      2.49289e-04      5.56925e-07
+   460      2.54491e-04      5.68479e-07
+   470      2.59650e-04      5.79934e-07
+   480      2.64768e-04      5.91290e-07
+   490      2.69843e-04      6.02544e-07
+   500      2.74874e-04      6.13694e-07
+   510      2.79861e-04      6.24739e-07
+   520      2.84804e-04      6.35678e-07
+   530      2.89701e-04      6.46508e-07
+   540      2.94553e-04      6.57233e-07
+   550      2.99359e-04      6.67844e-07
+   560      3.04118e-04      6.78344e-07
+   570      3.08830e-04      6.88732e-07
+   580      3.13494e-04      6.99006e-07
+   590      3.18110e-04      7.09164e-07
+   600      3.22678e-04      7.19206e-07
+   610      3.27197e-04      7.29129e-07
+   620      3.31665e-04      7.38931e-07
+   630      3.36085e-04      7.48616e-07
+   640      3.40453e-04      7.58177e-07
+   650      3.44771e-04      7.67616e-07
+   660      3.49037e-04      7.76930e-07
+   670      3.53252e-04      7.86120e-07
+   680      3.57415e-04      7.95183e-07
+   690      3.61525e-04      8.04119e-07
+   700      3.65583e-04      8.12928e-07
+   710      3.69588e-04      8.21607e-07
+   720      3.73539e-04      8.30155e-07
+   730      3.77436e-04      8.38571e-07
+   740      3.81279e-04      8.46856e-07
+   750      3.85067e-04      8.55007e-07
+   760      3.88800e-04      8.63026e-07
+   770      3.92478e-04      8.70908e-07
+   780      3.96100e-04      8.78655e-07
+   790      3.99667e-04      8.86266e-07
+   800      4.03178e-04      8.93740e-07
+   810      4.06632e-04      9.01076e-07
+   820      4.10030e-04      9.08273e-07
+   830      4.13371e-04      9.15331e-07
+   840      4.16654e-04      9.22248e-07
+   850      4.19881e-04      9.29025e-07
+   860      4.23050e-04      9.35661e-07
+   870      4.26162e-04      9.42156e-07
+   880      4.29215e-04      9.48508e-07
+   890      4.32211e-04      9.54716e-07
+   900      4.35150e-04      9.60783e-07
+   910      4.38030e-04      9.66706e-07
+   920      4.40849e-04      9.72484e-07
+   930      4.43610e-04      9.78118e-07
+   940      4.46311e-04      9.83608e-07
+   950      4.48951e-04      9.88952e-07
+   960      4.51531e-04      9.94151e-07
+   970      4.54050e-04      9.99205e-07
+   980      4.56510e-04      1.00411e-06
+   990      4.58909e-04      1.00888e-06
+  1000      4.61246e-04      1.01349e-06
+  1011      4.63748e-04      1.01840e-06
+  1022      4.66177e-04      1.02313e-06
+  1033      4.68531e-04      1.02769e-06
+  1044      4.70813e-04      1.03207e-06
+  1055      4.73021e-04      1.03627e-06
+  1066      4.75155e-04      1.04029e-06
+  1077      4.77216e-04      1.04414e-06
+  1088      4.79204e-04      1.04781e-06
+  1099      4.81118e-04      1.05131e-06
+  1110      4.82959e-04      1.05462e-06
+  1121      4.84727e-04      1.05777e-06
+  1132      4.86422e-04      1.06074e-06
+  1143      4.88045e-04      1.06353e-06
+  1154      4.89595e-04      1.06615e-06
+  1165      4.91072e-04      1.06860e-06
+  1176      4.92478e-04      1.07087e-06
+  1187      4.93811e-04      1.07297e-06
+  1198      4.95073e-04      1.07490e-06
+  1209      4.96263e-04      1.07666e-06
+  1220      4.97379e-04      1.07824e-06
+  1231      4.98415e-04      1.07966e-06
+  1242      4.99373e-04      1.08091e-06
+  1253      5.00253e-04      1.08199e-06
+  1264      5.01054e-04      1.08291e-06
+  1275      5.01776e-04      1.08366e-06
+  1286      5.02421e-04      1.08424e-06
+  1297      5.02987e-04      1.08467e-06
+  1308      5.03475e-04      1.08493e-06
+  1319      5.03885e-04      1.08503e-06
+  1330      5.04217e-04      1.08497e-06
+  1341      5.04471e-04      1.08475e-06
+  1352      5.04648e-04      1.08438e-06
+  1363      5.04747e-04      1.08385e-06
+  1374      5.04770e-04      1.08318e-06
+  1385      5.04715e-04      1.08235e-06
+  1396      5.04584e-04      1.08138e-06
+  1407      5.04376e-04      1.08025e-06
+  1418      5.04093e-04      1.07898e-06
+  1429      5.03734e-04      1.07757e-06
+  1440      5.03298e-04      1.07601e-06
+  1451      5.02789e-04      1.07431e-06
+  1462      5.02203e-04      1.07247e-06
+  1473      5.01543e-04      1.07049e-06
+  1484      5.00810e-04      1.06838e-06
+  1495      5.00001e-04      1.06613e-06
+  1506      4.99120e-04      1.06376e-06
+  1517      4.98165e-04      1.06125e-06
+  1528      4.97139e-04      1.05862e-06
+  1539      4.96040e-04      1.05587e-06
+  1550      4.94868e-04      1.05299e-06
+  1561      4.93626e-04      1.04999e-06
+  1572      4.92314e-04      1.04688e-06
+  1583      4.90931e-04      1.04366e-06
+  1594      4.89477e-04      1.04032e-06
+  1605      4.87955e-04      1.03687e-06
+  1616      4.86365e-04      1.03332e-06
+  1627      4.84706e-04      1.02966e-06
+  1638      4.82980e-04      1.02590e-06
+  1649      4.81187e-04      1.02205e-06
+  1660      4.79328e-04      1.01810e-06
+  1671      4.77403e-04      1.01406e-06
+  1682      4.75414e-04      1.00994e-06
+  1693      4.73359e-04      1.00572e-06
+  1704      4.71242e-04      1.00143e-06
+  1715      4.69061e-04      9.97052e-07
+  1726      4.66818e-04      9.92603e-07
+  1737      4.64514e-04      9.88080e-07
+  1748      4.62149e-04      9.83488e-07
+  1759      4.59724e-04      9.78832e-07
+  1770      4.57239e-04      9.74113e-07
+  1781      4.54697e-04      9.69336e-07
+  1792      4.52097e-04      9.64505e-07
+  1803      4.49439e-04      9.59621e-07
+  1814      4.46726e-04      9.54689e-07
+  1825      4.43958e-04      9.49713e-07
+  1836      4.41135e-04      9.44697e-07
+  1847      4.38259e-04      9.39644e-07
+  1858      4.35330e-04      9.34557e-07
+  1869      4.32350e-04      9.29442e-07
+  1880      4.29320e-04      9.24301e-07
+  1891      4.26239e-04      9.19145e-07
+  1902      4.23110e-04      9.13987e-07
+  1913      4.19933e-04      9.08810e-07
+  1924      4.16707e-04      9.03623e-07
+  1935      4.13434e-04      8.98430e-07
+  1946      4.10116e-04      8.93237e-07
+  1957      4.06752e-04      8.88046e-07
+  1968      4.03344e-04      8.82859e-07
+  1979      3.99893e-04      8.77684e-07
+  1990      3.96400e-04      8.72521e-07
+  2001      3.92867e-04      8.67377e-07
+  2012      3.89293e-04      8.62254e-07
+  2023      3.85681e-04      8.57157e-07
+  2034      3.82031e-04      8.52087e-07
+  2045      3.78345e-04      8.47050e-07
+  2056      3.74623e-04      8.42049e-07
+  2067      3.70867e-04      8.37087e-07
+  2078      3.67077e-04      8.32167e-07
+  2089      3.63255e-04      8.27293e-07
+  2100      3.59404e-04      8.22471e-07
+  2111      3.55522e-04      8.17697e-07
+  2122      3.51612e-04      8.12982e-07
+  2133      3.47675e-04      8.08324e-07
+  2144      3.43713e-04      8.03728e-07
+  2155      3.39726e-04      7.99195e-07
+  2166      3.35715e-04      7.94728e-07
+  2177      3.31682e-04      7.90329e-07
+  2188      3.27629e-04      7.86001e-07
+  2199      3.23557e-04      7.81748e-07
+  2210      3.19466e-04      7.77568e-07
+  2221      3.15359e-04      7.73465e-07
+  2232      3.11237e-04      7.69439e-07
+  2243      3.07100e-04      7.65493e-07
+  2254      3.02951e-04      7.61627e-07
+  2265      2.98791e-04      7.57841e-07
+  2276      2.94621e-04      7.54138e-07
+  2287      2.90444e-04      7.50518e-07
+  2298      2.86259e-04      7.46979e-07
+  2309      2.82068e-04      7.43521e-07
+  2320      2.77875e-04      7.40147e-07
+  2331      2.73678e-04      7.36853e-07
+  2342      2.69482e-04      7.33640e-07
+  2353      2.65285e-04      7.30506e-07
+  2364      2.61091e-04      7.27450e-07
+  2375      2.56901e-04      7.24470e-07
+  2386      2.52716e-04      7.21565e-07
+  2397      2.48538e-04      7.18732e-07
+  2408      2.44368e-04      7.15969e-07
+  2419      2.40209e-04      7.13272e-07
+  2430      2.36061e-04      7.10641e-07
+  2441      2.31927e-04      7.08070e-07
+  2452      2.27808e-04      7.05557e-07
+  2463      2.23705e-04      7.03098e-07
+  2474      2.19621e-04      7.00689e-07
+  2485      2.15556e-04      6.98325e-07
+  2496      2.11514e-04      6.96003e-07
+  2507      2.07495e-04      6.93718e-07
+  2518      2.03502e-04      6.91465e-07
+  2529      1.99534e-04      6.89238e-07
+  2540      1.95597e-04      6.87033e-07
+  2551      1.91688e-04      6.84843e-07
+  2562      1.87813e-04      6.82665e-07
+  2573      1.83971e-04      6.80492e-07
+  2584      1.80165e-04      6.78316e-07
+  2595      1.76396e-04      6.76134e-07
+  2606      1.72666e-04      6.73937e-07
+  2617      1.68954e-04      6.71719e-07
+  2628      1.65249e-04      6.69471e-07
+  2639      1.61552e-04      6.67187e-07
+  2650      1.57863e-04      6.64858e-07
+  2661      1.54185e-04      6.62479e-07
+  2672      1.50518e-04      6.60042e-07
+  2683      1.46864e-04      6.57540e-07
+  2694      1.43223e-04      6.54964e-07
+  2705      1.39598e-04      6.52307e-07
+  2716      1.35988e-04      6.49561e-07
+  2727      1.32396e-04      6.46718e-07
+  2738      1.28822e-04      6.43770e-07
+  2749      1.25268e-04      6.40710e-07
+  2760      1.21735e-04      6.37529e-07
+  2771      1.18225e-04      6.34218e-07
+  2782      1.14738e-04      6.30770e-07
+  2793      1.11276e-04      6.27178e-07
+  2804      1.07840e-04      6.23430e-07
+  2815      1.04431e-04      6.19520e-07
+  2826      1.01052e-04      6.15439e-07
+  2837      9.77021e-05      6.11179e-07
+  2848      9.43837e-05      6.06732e-07
+  2859      9.10981e-05      6.02087e-07
+  2870      8.78464e-05      5.97239e-07
+  2881      8.46302e-05      5.92177e-07
+  2892      8.14506e-05      5.86892e-07
+  2903      7.83093e-05      5.81377e-07
+  2914      7.52073e-05      5.75624e-07
+  2925      7.21462e-05      5.69680e-07
+  2936      6.91274e-05      5.63515e-07
+  2947      6.61523e-05      5.57089e-07
+  2958      6.32221e-05      5.50393e-07
+  2969      6.03385e-05      5.43417e-07
+  2980      5.75029e-05      5.36154e-07
+  2991      5.47165e-05      5.28595e-07
+  3002      5.19810e-05      5.20731e-07
+  3013      4.92976e-05      5.12553e-07
+  3024      4.66681e-05      5.04054e-07
+  3035      4.40937e-05      4.95225e-07
+  3046      4.15759e-05      4.86057e-07
+  3057      3.91163e-05      4.76542e-07
+  3068      3.67163e-05      4.66672e-07
+  3079      3.43775e-05      4.56437e-07
+  3090      3.21013e-05      4.45829e-07
+  3101      2.98892e-05      4.34841e-07
+  3112      2.77428e-05      4.23464e-07
+  3123      2.56638e-05      4.11689e-07
+  3134      2.36534e-05      3.99509e-07
+  3145      2.17134e-05      3.86914e-07
+  3156      1.98452e-05      3.73897e-07
+  3167      1.80505e-05      3.60450e-07
+  3178      1.63307e-05      3.46564e-07
+  3189      1.46876e-05      3.32232e-07
+  3200      1.31225e-05      3.17446e-07
+  3211      1.16372e-05      3.02197e-07
+  3222      1.02333e-05      2.86478e-07
+  3233      8.91221e-06      2.70282e-07
+  3244      7.67569e-06      2.53600e-07
+  3255      6.52529e-06      2.36427e-07
+  3266      5.46261e-06      2.18754e-07
+  3277      4.48927e-06      2.00576e-07
+  3288      3.60687e-06      1.81884e-07
+  3299      2.81700e-06      1.62675e-07
+  3310      2.12128e-06      1.42943e-07
+  3321      1.52127e-06      1.22684e-07
+  3332      1.01856e-06      1.01894e-07
+  3343      6.14692e-07      8.05752e-08
+  3354      3.11165e-07      5.87324e-08
+  3365      1.09408e-07      3.63814e-08
+  3376      1.06554e-08      1.35753e-08
+  3381      0.00000e+00      0.00000e+00
```

### Comparing `opengate-10.0b7/opengate/sources/beta_plus_spectra/Ga68/beta+_Ga68_tot.bs` & `opengate-10.0b8/opengate/sources/beta_plus_spectra/O15/beta+_O15_tot.bs`

 * *Files 25% similar despite different names*

```diff
@@ -1,419 +1,363 @@
----------------------------------------------------------------------------------------------
-
-BetaShape
-Version: 2.2 (05/2021)
-Author: X. Mougeot (xavier.mougeot@cea.fr)
-CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
-Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
-
----------------------------------------------------------------------------------------------
-
-Total beta + spectrum from the Ga-68 decay. See file of each transition for more details.
-
-Mean energy from the total beta + spectrum: 828.4 (35) keV
-
-E(keV)      dNtot/dE b+      unc.
-    0.0     0.00000e+00      0.00000e+00
-    0.8     5.69351e-10      2.27043e-13
-    1.6     4.69159e-09      1.87897e-12
-    2.4     1.23698e-08      4.95578e-12
-    3.2     2.36060e-08      9.45747e-12
-    4.0     3.84019e-08      1.53840e-11
-    4.8     5.88157e-08      2.35624e-11
-    5.6     1.78367e-07      4.08053e-10
-    6.4     3.58515e-07      1.05366e-09
-    7.2     5.78006e-07      1.84663e-09
-    8.0     8.36680e-07      2.78666e-09
-    8.8     1.13426e-06      3.87371e-09
-    9.6     1.47086e-06      5.10777e-09
-    10      1.65380e-06      5.77992e-09
-    11      2.15291e-06      7.62107e-09
-    12      2.71240e-06      9.69190e-09
-    13      3.41881e-06      1.23690e-08
-    14      4.20989e-06      1.53834e-08
-    15      5.08452e-06      1.87351e-08
-    16      6.04308e-06      2.24241e-08
-    17      7.08448e-06      2.64504e-08
-    18      8.20909e-06      3.08139e-08
-    19      9.35861e-06      3.52672e-08
-    20      1.05743e-05      3.99871e-08
-    21      1.18553e-05      4.49736e-08
-    22      1.32019e-05      5.02266e-08
-    23      1.46133e-05      5.57462e-08
-    24      1.60897e-05      6.15323e-08
-    25      1.75639e-05      6.72978e-08
-    26      1.90837e-05      7.32477e-08
-    27      2.06484e-05      7.93820e-08
-    28      2.22584e-05      8.57009e-08
-    29      2.39129e-05      9.22042e-08
-    30      2.56123e-05      9.88920e-08
-    31      2.73067e-05      1.05552e-07
-    32      2.90315e-05      1.12335e-07
-    33      3.07864e-05      1.19242e-07
-    34      3.25714e-05      1.26273e-07
-    35      3.43862e-05      1.33428e-07
-    36      3.62309e-05      1.40706e-07
-    37      3.80714e-05      1.47962e-07
-    38      3.99321e-05      1.55301e-07
-    39      4.18125e-05      1.62722e-07
-    40      4.37127e-05      1.70224e-07
-    41      4.56327e-05      1.77809e-07
-    42      4.75723e-05      1.85477e-07
-    43      4.95086e-05      1.93127e-07
-    44      5.14579e-05      2.00832e-07
-    45      5.34201e-05      2.08590e-07
-    46      5.53952e-05      2.16403e-07
-    47      5.73831e-05      2.24269e-07
-    48      5.93837e-05      2.32189e-07
-    49      6.13814e-05      2.40096e-07
-    50      6.33873e-05      2.48037e-07
-    51      6.54013e-05      2.56014e-07
-    52      6.74235e-05      2.64024e-07
-    53      6.94538e-05      2.72070e-07
-    54      7.14921e-05      2.80150e-07
-    55      7.35276e-05      2.88218e-07
-    56      7.55679e-05      2.96307e-07
-    57      7.76131e-05      3.04418e-07
-    58      7.96632e-05      3.12550e-07
-    59      8.17180e-05      3.20703e-07
-    60      8.37777e-05      3.28877e-07
-    61      8.58345e-05      3.37040e-07
-    62      8.78938e-05      3.45215e-07
-    63      8.99557e-05      3.53402e-07
-    64      9.20201e-05      3.61601e-07
-    65      9.40870e-05      3.69812e-07
-    66      9.61563e-05      3.78034e-07
-    67      9.82228e-05      3.86245e-07
-    68      1.00290e-04      3.94462e-07
-    69      1.02358e-04      4.02683e-07
-    70      1.04427e-04      4.10910e-07
-    71      1.06497e-04      4.19142e-07
-    72      1.08568e-04      4.27380e-07
-    73      1.10636e-04      4.35605e-07
-    74      1.12703e-04      4.43831e-07
-    75      1.14770e-04      4.52058e-07
-    76      1.16837e-04      4.60285e-07
-    77      1.18904e-04      4.68512e-07
-    78      1.20970e-04      4.76740e-07
-    79      1.23033e-04      4.84956e-07
-    80      1.25095e-04      4.93169e-07
-    81      1.27156e-04      5.01380e-07
-    82      1.29215e-04      5.09587e-07
-    83      1.31274e-04      5.17792e-07
-    84      1.33331e-04      5.25993e-07
-    85      1.35386e-04      5.34183e-07
-    86      1.37438e-04      5.42367e-07
-    87      1.39489e-04      5.50545e-07
-    88      1.41538e-04      5.58718e-07
-    89      1.43585e-04      5.66886e-07
-    90      1.45630e-04      5.75048e-07
-    91      1.47672e-04      5.83197e-07
-    92      1.49712e-04      5.91339e-07
-    93      1.51749e-04      5.99473e-07
-    94      1.53784e-04      6.07600e-07
-    95      1.55817e-04      6.15719e-07
-    96      1.57848e-04      6.23831e-07
-    97      1.59875e-04      6.31931e-07
-    98      1.61899e-04      6.40021e-07
-    99      1.63922e-04      6.48103e-07
-   100      1.65941e-04      6.56176e-07
-   106      1.78000e-04      7.04412e-07
-   112      1.89954e-04      7.52275e-07
-   118      2.01796e-04      7.99742e-07
-   124      2.13524e-04      8.46803e-07
-   130      2.25134e-04      8.93440e-07
-   136      2.36624e-04      9.39646e-07
-   142      2.47995e-04      9.85419e-07
-   148      2.59243e-04      1.03075e-06
-   154      2.70370e-04      1.07564e-06
-   160      2.81375e-04      1.12009e-06
-   166      2.92259e-04      1.16410e-06
-   172      3.03021e-04      1.20766e-06
-   178      3.13661e-04      1.25078e-06
-   184      3.24180e-04      1.29345e-06
-   190      3.34578e-04      1.33568e-06
-   196      3.44856e-04      1.37748e-06
-   202      3.55015e-04      1.41883e-06
-   208      3.65053e-04      1.45974e-06
-   214      3.74973e-04      1.50022e-06
-   220      3.84773e-04      1.54025e-06
-   226      3.94455e-04      1.57985e-06
-   232      4.04019e-04      1.61902e-06
-   238      4.13466e-04      1.65774e-06
-   244      4.22795e-04      1.69604e-06
-   250      4.32008e-04      1.73389e-06
-   256      4.41103e-04      1.77132e-06
-   262      4.50081e-04      1.80830e-06
-   268      4.58942e-04      1.84486e-06
-   274      4.67688e-04      1.88098e-06
-   280      4.76317e-04      1.91666e-06
-   286      4.84830e-04      1.95191e-06
-   292      4.93228e-04      1.98673e-06
-   298      5.01509e-04      2.02111e-06
-   304      5.09675e-04      2.05505e-06
-   310      5.17726e-04      2.08856e-06
-   316      5.25661e-04      2.12163e-06
-   322      5.33480e-04      2.15427e-06
-   328      5.41185e-04      2.18647e-06
-   334      5.48774e-04      2.21823e-06
-   340      5.56249e-04      2.24955e-06
-   346      5.63608e-04      2.28044e-06
-   352      5.70853e-04      2.31088e-06
-   358      5.77983e-04      2.34089e-06
-   364      5.84998e-04      2.37045e-06
-   370      5.91899e-04      2.39957e-06
-   376      5.98685e-04      2.42825e-06
-   382      6.05356e-04      2.45648e-06
-   388      6.11914e-04      2.48428e-06
-   394      6.18357e-04      2.51163e-06
-   400      6.24685e-04      2.53853e-06
-   406      6.30900e-04      2.56499e-06
-   412      6.37000e-04      2.59100e-06
-   418      6.42987e-04      2.61656e-06
-   424      6.48860e-04      2.64168e-06
-   430      6.54619e-04      2.66635e-06
-   436      6.60264e-04      2.69057e-06
-   442      6.65797e-04      2.71434e-06
-   448      6.71215e-04      2.73766e-06
-   454      6.76521e-04      2.76053e-06
-   460      6.81714e-04      2.78294e-06
-   466      6.86794e-04      2.80491e-06
-   472      6.91762e-04      2.82643e-06
-   478      6.96617e-04      2.84749e-06
-   484      7.01360e-04      2.86810e-06
-   490      7.05992e-04      2.88825e-06
-   496      7.10511e-04      2.90796e-06
-   502      7.14919e-04      2.92720e-06
-   508      7.19216e-04      2.94600e-06
-   514      7.23403e-04      2.96434e-06
-   520      7.27478e-04      2.98223e-06
-   526      7.31444e-04      2.99966e-06
-   532      7.35300e-04      3.01664e-06
-   538      7.39045e-04      3.03316e-06
-   544      7.42682e-04      3.04923e-06
-   550      7.46209e-04      3.06484e-06
-   556      7.49629e-04      3.08000e-06
-   562      7.52940e-04      3.09471e-06
-   568      7.56143e-04      3.10896e-06
-   574      7.59240e-04      3.12276e-06
-   580      7.62229e-04      3.13610e-06
-   586      7.65112e-04      3.14899e-06
-   592      7.67889e-04      3.16143e-06
-   598      7.70561e-04      3.17342e-06
-   604      7.73128e-04      3.18495e-06
-   610      7.75591e-04      3.19604e-06
-   616      7.77949e-04      3.20667e-06
-   622      7.80205e-04      3.21685e-06
-   628      7.82358e-04      3.22659e-06
-   634      7.84409e-04      3.23587e-06
-   640      7.86358e-04      3.24471e-06
-   646      7.88206e-04      3.25310e-06
-   652      7.89954e-04      3.26104e-06
-   658      7.91602e-04      3.26854e-06
-   664      7.93152e-04      3.27560e-06
-   670      7.94603e-04      3.28221e-06
-   676      7.95957e-04      3.28838e-06
-   682      7.97214e-04      3.29411e-06
-   688      7.98375e-04      3.29940e-06
-   694      7.99441e-04      3.30425e-06
-   700      8.00412e-04      3.30867e-06
-   706      8.01289e-04      3.31265e-06
-   712      8.02074e-04      3.31619e-06
-   718      8.02766e-04      3.31931e-06
-   724      8.03368e-04      3.32199e-06
-   730      8.03879e-04      3.32425e-06
-   736      8.04300e-04      3.32607e-06
-   742      8.04633e-04      3.32748e-06
-   748      8.04879e-04      3.32846e-06
-   754      8.05037e-04      3.32902e-06
-   760      8.05110e-04      3.32916e-06
-   766      8.05099e-04      3.32888e-06
-   772      8.05003e-04      3.32818e-06
-   778      8.04824e-04      3.32708e-06
-   784      8.04564e-04      3.32556e-06
-   790      8.04223e-04      3.32363e-06
-   796      8.03802e-04      3.32129e-06
-   802      8.03303e-04      3.31855e-06
-   808      8.02726e-04      3.31540e-06
-   814      8.02073e-04      3.31186e-06
-   820      8.01344e-04      3.30792e-06
-   826      8.00535e-04      3.30358e-06
-   832      7.99629e-04      3.29885e-06
-   838      7.98625e-04      3.29373e-06
-   844      7.97522e-04      3.28823e-06
-   850      7.96323e-04      3.28234e-06
-   856      7.95027e-04      3.27607e-06
-   862      7.93635e-04      3.26942e-06
-   868      7.92147e-04      3.26239e-06
-   874      7.90564e-04      3.25500e-06
-   880      7.88887e-04      3.24723e-06
-   886      7.87115e-04      3.23910e-06
-   892      7.85250e-04      3.23061e-06
-   898      7.83291e-04      3.22175e-06
-   904      7.81240e-04      3.21255e-06
-   910      7.79097e-04      3.20298e-06
-   916      7.76863e-04      3.19307e-06
-   922      7.74538e-04      3.18282e-06
-   928      7.72123e-04      3.17222e-06
-   934      7.69619e-04      3.16128e-06
-   940      7.67025e-04      3.15001e-06
-   946      7.64343e-04      3.13841e-06
-   952      7.61574e-04      3.12648e-06
-   958      7.58718e-04      3.11423e-06
-   964      7.55776e-04      3.10166e-06
-   970      7.52748e-04      3.08878e-06
-   976      7.49635e-04      3.07558e-06
-   982      7.46439e-04      3.06208e-06
-   988      7.43159e-04      3.04827e-06
-   994      7.39796e-04      3.03417e-06
-  1000      7.36352e-04      3.01977e-06
-  1006      7.32827e-04      3.00508e-06
-  1012      7.29221e-04      2.99011e-06
-  1018      7.25536e-04      2.97485e-06
-  1024      7.21772e-04      2.95932e-06
-  1030      7.17931e-04      2.94352e-06
-  1036      7.14012e-04      2.92746e-06
-  1042      7.10017e-04      2.91113e-06
-  1048      7.05947e-04      2.89455e-06
-  1054      7.01803e-04      2.87772e-06
-  1060      6.97585e-04      2.86063e-06
-  1066      6.93294e-04      2.84331e-06
-  1072      6.88932e-04      2.82575e-06
-  1078      6.84499e-04      2.80795e-06
-  1084      6.79995e-04      2.78993e-06
-  1090      6.75424e-04      2.77169e-06
-  1096      6.70784e-04      2.75323e-06
-  1102      6.66077e-04      2.73455e-06
-  1108      6.61304e-04      2.71567e-06
-  1114      6.56467e-04      2.69660e-06
-  1120      6.51565e-04      2.67732e-06
-  1126      6.46600e-04      2.65785e-06
-  1132      6.41573e-04      2.63820e-06
-  1138      6.36485e-04      2.61837e-06
-  1144      6.31338e-04      2.59837e-06
-  1150      6.26132e-04      2.57820e-06
-  1156      6.20868e-04      2.55787e-06
-  1162      6.15548e-04      2.53739e-06
-  1168      6.10172e-04      2.51675e-06
-  1174      6.04742e-04      2.49597e-06
-  1180      5.99259e-04      2.47504e-06
-  1186      5.93723e-04      2.45399e-06
-  1192      5.88136e-04      2.43281e-06
-  1198      5.82500e-04      2.41151e-06
-  1204      5.76815e-04      2.39009e-06
-  1210      5.71083e-04      2.36857e-06
-  1216      5.65305e-04      2.34694e-06
-  1222      5.59482e-04      2.32522e-06
-  1228      5.53615e-04      2.30340e-06
-  1234      5.47706e-04      2.28151e-06
-  1240      5.41755e-04      2.25953e-06
-  1246      5.35764e-04      2.23748e-06
-  1252      5.29735e-04      2.21537e-06
-  1258      5.23668e-04      2.19320e-06
-  1264      5.17566e-04      2.17098e-06
-  1270      5.11429e-04      2.14871e-06
-  1276      5.05258e-04      2.12640e-06
-  1282      4.99055e-04      2.10406e-06
-  1288      4.92822e-04      2.08169e-06
-  1294      4.86559e-04      2.05929e-06
-  1300      4.80268e-04      2.03689e-06
-  1306      4.73951e-04      2.01447e-06
-  1312      4.67608e-04      1.99205e-06
-  1318      4.61241e-04      1.96964e-06
-  1324      4.54853e-04      1.94724e-06
-  1330      4.48443e-04      1.92485e-06
-  1336      4.42014e-04      1.90248e-06
-  1342      4.35567e-04      1.88015e-06
-  1348      4.29104e-04      1.85785e-06
-  1354      4.22626e-04      1.83559e-06
-  1360      4.16133e-04      1.81337e-06
-  1366      4.09629e-04      1.79121e-06
-  1372      4.03115e-04      1.76910e-06
-  1378      3.96591e-04      1.74706e-06
-  1384      3.90060e-04      1.72509e-06
-  1390      3.83524e-04      1.70319e-06
-  1396      3.76983e-04      1.68138e-06
-  1402      3.70439e-04      1.65965e-06
-  1408      3.63894e-04      1.63800e-06
-  1414      3.57350e-04      1.61646e-06
-  1420      3.50808e-04      1.59501e-06
-  1426      3.44270e-04      1.57367e-06
-  1432      3.37737e-04      1.55244e-06
-  1438      3.31211e-04      1.53132e-06
-  1444      3.24694e-04      1.51032e-06
-  1450      3.18188e-04      1.48944e-06
-  1456      3.11694e-04      1.46869e-06
-  1462      3.05213e-04      1.44806e-06
-  1468      2.98748e-04      1.42757e-06
-  1474      2.92301e-04      1.40721e-06
-  1480      2.85873e-04      1.38698e-06
-  1486      2.79464e-04      1.36690e-06
-  1492      2.73079e-04      1.34695e-06
-  1498      2.66719e-04      1.32715e-06
-  1504      2.60384e-04      1.30750e-06
-  1510      2.54077e-04      1.28798e-06
-  1516      2.47800e-04      1.26861e-06
-  1522      2.41554e-04      1.24939e-06
-  1528      2.35342e-04      1.23031e-06
-  1534      2.29165e-04      1.21138e-06
-  1540      2.23025e-04      1.19259e-06
-  1546      2.16925e-04      1.17394e-06
-  1552      2.10865e-04      1.15544e-06
-  1558      2.04847e-04      1.13706e-06
-  1564      1.98875e-04      1.11883e-06
-  1570      1.92949e-04      1.10072e-06
-  1576      1.87072e-04      1.08274e-06
-  1582      1.81245e-04      1.06488e-06
-  1588      1.75470e-04      1.04714e-06
-  1594      1.69750e-04      1.02951e-06
-  1600      1.64087e-04      1.01199e-06
-  1606      1.58482e-04      9.94561e-07
-  1612      1.52936e-04      9.77227e-07
-  1618      1.47454e-04      9.59978e-07
-  1624      1.42036e-04      9.42803e-07
-  1630      1.36685e-04      9.25695e-07
-  1636      1.31402e-04      9.08676e-07
-  1642      1.26189e-04      8.91743e-07
-  1648      1.21049e-04      8.74850e-07
-  1654      1.15984e-04      8.57985e-07
-  1660      1.10995e-04      8.41137e-07
-  1666      1.06086e-04      8.24296e-07
-  1672      1.01258e-04      8.07445e-07
-  1678      9.65128e-05      7.90574e-07
-  1684      9.18531e-05      7.73670e-07
-  1690      8.72809e-05      7.56717e-07
-  1696      8.27984e-05      7.39702e-07
-  1702      7.84077e-05      7.22608e-07
-  1708      7.41111e-05      7.05422e-07
-  1714      6.99106e-05      6.88126e-07
-  1720      6.58087e-05      6.70705e-07
-  1726      6.18074e-05      6.53143e-07
-  1732      5.79091e-05      6.35421e-07
-  1738      5.41160e-05      6.17523e-07
-  1744      5.04304e-05      5.99431e-07
-  1750      4.68544e-05      5.81128e-07
-  1756      4.33904e-05      5.62594e-07
-  1762      4.00408e-05      5.43812e-07
-  1768      3.68077e-05      5.24762e-07
-  1774      3.36936e-05      5.05426e-07
-  1780      3.07007e-05      4.85786e-07
-  1786      2.78315e-05      4.65820e-07
-  1792      2.50882e-05      4.45511e-07
-  1798      2.24732e-05      4.24839e-07
-  1804      1.99889e-05      4.03782e-07
-  1810      1.76378e-05      3.82324e-07
-  1816      1.54221e-05      3.60442e-07
-  1822      1.33443e-05      3.38117e-07
-  1828      1.14070e-05      3.15330e-07
-  1834      9.61228e-06      2.92059e-07
-  1840      7.96282e-06      2.68286e-07
-  1846      6.46106e-06      2.43990e-07
-  1852      5.10944e-06      2.19151e-07
-  1858      3.91045e-06      1.93748e-07
-  1864      2.86660e-06      1.67763e-07
-  1870      1.98036e-06      1.41174e-07
-  1876      1.25427e-06      1.13962e-07
-  1882      6.90856e-07      8.61072e-08
-  1888      2.92654e-07      5.75893e-08
-  1894      6.22143e-08      2.83886e-08
- 1899.1     0.00000e+00      0.00000e+00
+---------------------------------------------------------------------------------------------
+
+BetaShape
+Version: 2.2 (05/2021)
+Author: X. Mougeot (xavier.mougeot@cea.fr)
+CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
+Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
+
+---------------------------------------------------------------------------------------------
+
+Total beta + spectrum from the O-15 decay. See file of each transition for more details.
+
+Mean energy from the total beta + spectrum: 734.8 (6) keV
+
+E(keV)      dNtot/dE b+      unc.
+     0      0.00000e+00      0.00000e+00
+     5      2.62304e-05      4.45546e-08
+    10      5.37915e-05      9.11348e-08
+    15      7.79110e-05      1.31657e-07
+    20      9.95482e-05      1.67781e-07
+    25      1.19378e-04      2.00671e-07
+    30      1.37834e-04      2.31080e-07
+    35      1.55207e-04      2.59509e-07
+    40      1.71702e-04      2.86312e-07
+    45      1.87467e-04      3.11747e-07
+    50      2.02614e-04      3.36009e-07
+    55      2.17229e-04      3.59247e-07
+    60      2.31382e-04      3.81580e-07
+    65      2.45126e-04      4.03103e-07
+    70      2.58505e-04      4.23894e-07
+    75      2.71558e-04      4.44016e-07
+    80      2.84313e-04      4.63523e-07
+    85      2.96798e-04      4.82460e-07
+    90      3.09034e-04      5.00866e-07
+    95      3.21040e-04      5.18773e-07
+   100      3.32832e-04      5.36210e-07
+   105      3.44425e-04      5.53200e-07
+   110      3.55830e-04      5.69766e-07
+   115      3.67058e-04      5.85926e-07
+   120      3.78119e-04      6.01697e-07
+   125      3.89020e-04      6.17093e-07
+   130      3.99770e-04      6.32127e-07
+   135      4.10375e-04      6.46811e-07
+   140      4.20840e-04      6.61155e-07
+   145      4.31172e-04      6.75167e-07
+   150      4.41373e-04      6.88856e-07
+   155      4.51449e-04      7.02230e-07
+   160      4.61403e-04      7.15294e-07
+   165      4.71239e-04      7.28055e-07
+   170      4.80960e-04      7.40518e-07
+   175      4.90567e-04      7.52688e-07
+   180      5.00064e-04      7.64570e-07
+   185      5.09453e-04      7.76166e-07
+   190      5.18736e-04      7.87482e-07
+   195      5.27915e-04      7.98519e-07
+   200      5.36990e-04      8.09282e-07
+   205      5.45964e-04      8.19772e-07
+   210      5.54838e-04      8.29992e-07
+   215      5.63613e-04      8.39944e-07
+   220      5.72290e-04      8.49631e-07
+   225      5.80870e-04      8.59054e-07
+   230      5.89354e-04      8.68215e-07
+   235      5.97742e-04      8.77115e-07
+   240      6.06035e-04      8.85756e-07
+   245      6.14234e-04      8.94139e-07
+   250      6.22339e-04      9.02266e-07
+   255      6.30351e-04      9.10136e-07
+   260      6.38270e-04      9.17753e-07
+   265      6.46097e-04      9.25115e-07
+   270      6.53831e-04      9.32225e-07
+   275      6.61473e-04      9.39082e-07
+   280      6.69023e-04      9.45688e-07
+   285      6.76482e-04      9.52044e-07
+   290      6.83848e-04      9.58150e-07
+   295      6.91124e-04      9.64006e-07
+   300      6.98308e-04      9.69613e-07
+   305      7.05401e-04      9.74972e-07
+   310      7.12402e-04      9.80084e-07
+   315      7.19312e-04      9.84948e-07
+   320      7.26131e-04      9.89565e-07
+   325      7.32858e-04      9.93936e-07
+   330      7.39494e-04      9.98060e-07
+   335      7.46039e-04      1.00194e-06
+   340      7.52492e-04      1.00557e-06
+   345      7.58853e-04      1.00896e-06
+   350      7.65123e-04      1.01211e-06
+   355      7.71301e-04      1.01501e-06
+   360      7.77386e-04      1.01767e-06
+   365      7.83380e-04      1.02008e-06
+   370      7.89282e-04      1.02225e-06
+   375      7.95091e-04      1.02418e-06
+   380      8.00808e-04      1.02587e-06
+   385      8.06432e-04      1.02732e-06
+   390      8.11963e-04      1.02852e-06
+   395      8.17402e-04      1.02949e-06
+   400      8.22747e-04      1.03021e-06
+   405      8.28000e-04      1.03070e-06
+   410      8.33158e-04      1.03094e-06
+   415      8.38224e-04      1.03095e-06
+   420      8.43196e-04      1.03072e-06
+   425      8.48074e-04      1.03025e-06
+   430      8.52858e-04      1.02955e-06
+   435      8.57547e-04      1.02861e-06
+   440      8.62143e-04      1.02743e-06
+   445      8.66644e-04      1.02602e-06
+   450      8.71051e-04      1.02437e-06
+   455      8.75363e-04      1.02249e-06
+   460      8.79581e-04      1.02037e-06
+   465      8.83703e-04      1.01803e-06
+   470      8.87730e-04      1.01545e-06
+   475      8.91663e-04      1.01264e-06
+   480      8.95500e-04      1.00960e-06
+   485      8.99241e-04      1.00633e-06
+   490      9.02888e-04      1.00283e-06
+   495      9.06438e-04      9.99104e-07
+   500      9.09893e-04      9.95151e-07
+   505      9.13253e-04      9.90971e-07
+   510      9.16516e-04      9.86566e-07
+   515      9.19684e-04      9.81937e-07
+   520      9.22755e-04      9.77084e-07
+   525      9.25731e-04      9.72009e-07
+   530      9.28610e-04      9.66712e-07
+   535      9.31394e-04      9.61195e-07
+   540      9.34081e-04      9.55459e-07
+   545      9.36672e-04      9.49505e-07
+   550      9.39167e-04      9.43334e-07
+   555      9.41565e-04      9.36946e-07
+   560      9.43868e-04      9.30344e-07
+   565      9.46074e-04      9.23529e-07
+   570      9.48184e-04      9.16501e-07
+   575      9.50197e-04      9.09262e-07
+   580      9.52115e-04      9.01814e-07
+   585      9.53936e-04      8.94157e-07
+   590      9.55661e-04      8.86293e-07
+   595      9.57290e-04      8.78223e-07
+   600      9.58823e-04      8.69949e-07
+   605      9.60260e-04      8.61472e-07
+   610      9.61601e-04      8.52793e-07
+   615      9.62847e-04      8.43915e-07
+   620      9.63996e-04      8.34839e-07
+   625      9.65050e-04      8.25565e-07
+   630      9.66008e-04      8.16097e-07
+   635      9.66871e-04      8.06435e-07
+   640      9.67639e-04      7.96580e-07
+   645      9.68311e-04      7.86536e-07
+   650      9.68889e-04      7.76303e-07
+   655      9.69371e-04      7.65883e-07
+   660      9.69759e-04      7.55278e-07
+   665      9.70052e-04      7.44490e-07
+   670      9.70250e-04      7.33520e-07
+   675      9.70355e-04      7.22371e-07
+   680      9.70365e-04      7.11044e-07
+   685      9.70282e-04      6.99541e-07
+   690      9.70105e-04      6.87879e-07
+   695      9.69835e-04      6.76076e-07
+   700      9.69471e-04      6.64103e-07
+   705      9.69014e-04      6.51963e-07
+   710      9.68465e-04      6.39657e-07
+   715      9.67824e-04      6.27188e-07
+   720      9.67090e-04      6.14557e-07
+   725      9.66264e-04      6.01767e-07
+   730      9.65347e-04      5.88821e-07
+   735      9.64339e-04      5.75719e-07
+   740      9.63239e-04      5.62466e-07
+   745      9.62049e-04      5.49062e-07
+   750      9.60768e-04      5.35510e-07
+   755      9.59398e-04      5.21812e-07
+   760      9.57937e-04      5.07972e-07
+   765      9.56388e-04      4.93990e-07
+   770      9.54749e-04      4.79870e-07
+   775      9.53022e-04      4.65615e-07
+   780      9.51207e-04      4.51226e-07
+   785      9.49303e-04      4.36706e-07
+   790      9.47313e-04      4.22058e-07
+   795      9.45235e-04      4.07284e-07
+   800      9.43071e-04      3.92387e-07
+   805      9.40820e-04      3.77370e-07
+   810      9.38484e-04      3.62235e-07
+   815      9.36063e-04      3.46985e-07
+   820      9.33557e-04      3.31623e-07
+   825      9.30966e-04      3.16152e-07
+   830      9.28292e-04      3.00573e-07
+   835      9.25534e-04      2.84891e-07
+   840      9.22693e-04      2.69108e-07
+   845      9.19770e-04      2.53227e-07
+   850      9.16765e-04      2.37251e-07
+   855      9.13679e-04      2.21183e-07
+   860      9.10511e-04      2.05026e-07
+   865      9.07264e-04      1.88783e-07
+   870      9.03937e-04      1.72457e-07
+   875      9.00531e-04      1.56050e-07
+   880      8.97046e-04      1.39568e-07
+   885      8.93483e-04      1.23011e-07
+   890      8.89843e-04      1.06384e-07
+   895      8.86126e-04      8.96900e-08
+   900      8.82333e-04      7.29319e-08
+   905      8.78465e-04      5.61133e-08
+   910      8.74521e-04      3.92373e-08
+   915      8.70503e-04      2.23073e-08
+   920      8.66412e-04      5.32683e-09
+   925      8.62248e-04      1.39256e-08
+   930      8.58011e-04      3.10404e-08
+   935      8.53703e-04      4.81951e-08
+   940      8.49324e-04      6.53860e-08
+   945      8.44875e-04      8.26098e-08
+   950      8.40357e-04      9.98626e-08
+   955      8.35770e-04      1.17141e-07
+   960      8.31114e-04      1.34441e-07
+   965      8.26392e-04      1.51760e-07
+   970      8.21603e-04      1.69093e-07
+   975      8.16748e-04      1.86436e-07
+   980      8.11829e-04      2.03787e-07
+   985      8.06845e-04      2.21141e-07
+   990      8.01798e-04      2.38494e-07
+   995      7.96688e-04      2.55842e-07
+  1000      7.91516e-04      2.73182e-07
+  1005      7.86284e-04      2.90510e-07
+  1010      7.80991e-04      3.07821e-07
+  1015      7.75640e-04      3.25111e-07
+  1020      7.70230e-04      3.42377e-07
+  1025      7.64762e-04      3.59615e-07
+  1030      7.59237e-04      3.76820e-07
+  1035      7.53657e-04      3.93988e-07
+  1040      7.48022e-04      4.11116e-07
+  1045      7.42333e-04      4.28198e-07
+  1050      7.36591e-04      4.45231e-07
+  1055      7.30797e-04      4.62210e-07
+  1060      7.24952e-04      4.79131e-07
+  1065      7.19056e-04      4.95991e-07
+  1070      7.13111e-04      5.12783e-07
+  1075      7.07118e-04      5.29505e-07
+  1080      7.01077e-04      5.46151e-07
+  1085      6.94990e-04      5.62718e-07
+  1090      6.88858e-04      5.79200e-07
+  1095      6.82681e-04      5.95593e-07
+  1100      6.76461e-04      6.11894e-07
+  1105      6.70198e-04      6.28096e-07
+  1110      6.63894e-04      6.44195e-07
+  1115      6.57550e-04      6.60188e-07
+  1120      6.51167e-04      6.76069e-07
+  1125      6.44745e-04      6.91833e-07
+  1130      6.38287e-04      7.07476e-07
+  1135      6.31792e-04      7.22993e-07
+  1140      6.25263e-04      7.38379e-07
+  1145      6.18699e-04      7.53629e-07
+  1150      6.12103e-04      7.68739e-07
+  1155      6.05476e-04      7.83704e-07
+  1160      5.98818e-04      7.98518e-07
+  1165      5.92130e-04      8.13177e-07
+  1170      5.85415e-04      8.27676e-07
+  1175      5.78673e-04      8.42010e-07
+  1180      5.71904e-04      8.56173e-07
+  1185      5.65112e-04      8.70161e-07
+  1190      5.58295e-04      8.83969e-07
+  1195      5.51457e-04      8.97591e-07
+  1200      5.44597e-04      9.11022e-07
+  1205      5.37718e-04      9.24257e-07
+  1210      5.30820e-04      9.37292e-07
+  1215      5.23905e-04      9.50119e-07
+  1220      5.16974e-04      9.62735e-07
+  1225      5.10028e-04      9.75134e-07
+  1230      5.03069e-04      9.87311e-07
+  1235      4.96097e-04      9.99259e-07
+  1240      4.89114e-04      1.01097e-06
+  1245      4.82122e-04      1.02245e-06
+  1250      4.75121e-04      1.03368e-06
+  1255      4.68113e-04      1.04467e-06
+  1260      4.61100e-04      1.05540e-06
+  1265      4.54082e-04      1.06586e-06
+  1270      4.47061e-04      1.07606e-06
+  1275      4.40039e-04      1.08599e-06
+  1280      4.33016e-04      1.09564e-06
+  1285      4.25995e-04      1.10501e-06
+  1290      4.18976e-04      1.11409e-06
+  1295      4.11960e-04      1.12288e-06
+  1300      4.04951e-04      1.13136e-06
+  1305      3.97948e-04      1.13954e-06
+  1310      3.90953e-04      1.14740e-06
+  1315      3.83967e-04      1.15495e-06
+  1320      3.76993e-04      1.16217e-06
+  1325      3.70031e-04      1.16907e-06
+  1330      3.63083e-04      1.17562e-06
+  1335      3.56151e-04      1.18184e-06
+  1340      3.49236e-04      1.18771e-06
+  1345      3.42339e-04      1.19322e-06
+  1350      3.35462e-04      1.19837e-06
+  1355      3.28606e-04      1.20316e-06
+  1360      3.21773e-04      1.20758e-06
+  1365      3.14965e-04      1.21161e-06
+  1370      3.08183e-04      1.21527e-06
+  1375      3.01429e-04      1.21853e-06
+  1380      2.94704e-04      1.22139e-06
+  1385      2.88010e-04      1.22386e-06
+  1390      2.81348e-04      1.22591e-06
+  1395      2.74719e-04      1.22754e-06
+  1400      2.68127e-04      1.22876e-06
+  1405      2.61572e-04      1.22954e-06
+  1410      2.55055e-04      1.22989e-06
+  1415      2.48579e-04      1.22980e-06
+  1420      2.42145e-04      1.22926e-06
+  1425      2.35755e-04      1.22826e-06
+  1430      2.29410e-04      1.22681e-06
+  1435      2.23112e-04      1.22488e-06
+  1440      2.16863e-04      1.22249e-06
+  1445      2.10664e-04      1.21961e-06
+  1450      2.04517e-04      1.21624e-06
+  1455      1.98424e-04      1.21238e-06
+  1460      1.92387e-04      1.20802e-06
+  1465      1.86407e-04      1.20315e-06
+  1470      1.80486e-04      1.19777e-06
+  1475      1.74626e-04      1.19186e-06
+  1480      1.68829e-04      1.18543e-06
+  1485      1.63095e-04      1.17855e-06
+  1490      1.57428e-04      1.17118e-06
+  1495      1.51829e-04      1.16326e-06
+  1500      1.46299e-04      1.15479e-06
+  1505      1.40840e-04      1.14576e-06
+  1510      1.35455e-04      1.13617e-06
+  1515      1.30145e-04      1.12600e-06
+  1520      1.24912e-04      1.11525e-06
+  1525      1.19758e-04      1.10391e-06
+  1530      1.14684e-04      1.09198e-06
+  1535      1.09693e-04      1.07945e-06
+  1540      1.04786e-04      1.06632e-06
+  1545      9.99649e-05      1.05256e-06
+  1550      9.52322e-05      1.03819e-06
+  1555      9.05895e-05      1.02318e-06
+  1560      8.60386e-05      1.00754e-06
+  1565      8.15816e-05      9.91255e-07
+  1570      7.72202e-05      9.74320e-07
+  1575      7.29565e-05      9.56727e-07
+  1580      6.87923e-05      9.38469e-07
+  1585      6.47296e-05      9.19539e-07
+  1590      6.07705e-05      8.99929e-07
+  1595      5.69167e-05      8.79634e-07
+  1600      5.31704e-05      8.58645e-07
+  1605      4.95334e-05      8.36955e-07
+  1610      4.60078e-05      8.14557e-07
+  1615      4.25956e-05      7.91444e-07
+  1620      3.92987e-05      7.67609e-07
+  1625      3.61193e-05      7.43045e-07
+  1630      3.30591e-05      7.17744e-07
+  1635      3.01205e-05      6.91700e-07
+  1640      2.73052e-05      6.64905e-07
+  1645      2.46154e-05      6.37352e-07
+  1650      2.20532e-05      6.09036e-07
+  1655      1.96205e-05      5.79947e-07
+  1660      1.73194e-05      5.50081e-07
+  1665      1.51521e-05      5.19430e-07
+  1670      1.31205e-05      4.87988e-07
+  1675      1.12267e-05      4.55748e-07
+  1680      9.47276e-06      4.22705e-07
+  1685      7.86081e-06      3.88852e-07
+  1690      6.39290e-06      3.54185e-07
+  1695      5.07108e-06      3.18698e-07
+  1700      3.89744e-06      2.82387e-07
+  1705      2.87402e-06      2.45250e-07
+  1710      2.00288e-06      2.07284e-07
+  1715      1.28603e-06      1.68490e-07
+  1720      7.25466e-07      1.28875e-07
+  1725      3.23125e-07      8.84504e-08
+  1730      8.08160e-08      4.72522e-08
+  1735      0.00000e+00      0.00000e+00
```

### Comparing `opengate-10.0b7/opengate/sources/beta_plus_spectra/Na22/beta+_Na22_tot.bs` & `opengate-10.0b8/opengate/sources/beta_plus_spectra/Na22/beta+_Na22_tot.bs`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,403 +1,403 @@
----------------------------------------------------------------------------------------------
-
-BetaShape
-Version: 2.2 (05/2021)
-Author: X. Mougeot (xavier.mougeot@cea.fr)
-CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
-Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
-
----------------------------------------------------------------------------------------------
-
-Total beta + spectrum from the Na-22 decay. See file of each transition for more details.
-
-Mean energy from the total beta + spectrum: 216.70 (24) keV
-
-E(keV)      dNtot/dE b+      unc.
-     0      0.00000e+00      0.00000e+00
-     1      2.23945e-06      2.53863e-09
-     2      1.91570e-05      2.17105e-08
-     3      4.98404e-05      5.64478e-08
-     4      8.85617e-05      1.00235e-07
-     5      1.31634e-04      1.48882e-07
-     6      1.76936e-04      1.99982e-07
-     7      2.23239e-04      2.52142e-07
-     8      2.69814e-04      3.04534e-07
-     9      3.16218e-04      3.56658e-07
-    10      3.62180e-04      4.08211e-07
-    11      4.07533e-04      4.59004e-07
-    12      4.52181e-04      5.08930e-07
-    13      4.96064e-04      5.57923e-07
-    14      5.39152e-04      6.05952e-07
-    15      5.81436e-04      6.53008e-07
-    16      6.22915e-04      6.99092e-07
-    17      6.63598e-04      7.44214e-07
-    18      7.03499e-04      7.88392e-07
-    19      7.42634e-04      8.31648e-07
-    20      7.81022e-04      8.74002e-07
-    21      8.18683e-04      9.15478e-07
-    22      8.55637e-04      9.56102e-07
-    23      8.91904e-04      9.95897e-07
-    24      9.27504e-04      1.03489e-06
-    25      9.62457e-04      1.07309e-06
-    26      9.96781e-04      1.11054e-06
-    27      1.03050e-03      1.14725e-06
-    28      1.06362e-03      1.18324e-06
-    29      1.09616e-03      1.21854e-06
-    30      1.12816e-03      1.25316e-06
-    31      1.15960e-03      1.28712e-06
-    32      1.19051e-03      1.32043e-06
-    33      1.22091e-03      1.35313e-06
-    34      1.25081e-03      1.38521e-06
-    35      1.28022e-03      1.41671e-06
-    36      1.30917e-03      1.44762e-06
-    37      1.33764e-03      1.47797e-06
-    38      1.36566e-03      1.50777e-06
-    39      1.39323e-03      1.53703e-06
-    40      1.42038e-03      1.56577e-06
-    41      1.44710e-03      1.59399e-06
-    42      1.47343e-03      1.62172e-06
-    43      1.49934e-03      1.64895e-06
-    44      1.52486e-03      1.67570e-06
-    45      1.54999e-03      1.70198e-06
-    46      1.57474e-03      1.72779e-06
-    47      1.59912e-03      1.75316e-06
-    48      1.62315e-03      1.77808e-06
-    49      1.64682e-03      1.80257e-06
-    50      1.67013e-03      1.82663e-06
-    51      1.69311e-03      1.85028e-06
-    52      1.71574e-03      1.87351e-06
-    53      1.73805e-03      1.89634e-06
-    54      1.76005e-03      1.91878e-06
-    55      1.78171e-03      1.94082e-06
-    56      1.80306e-03      1.96248e-06
-    57      1.82410e-03      1.98376e-06
-    58      1.84484e-03      2.00467e-06
-    59      1.86529e-03      2.02523e-06
-    60      1.88543e-03      2.04541e-06
-    61      1.90530e-03      2.06525e-06
-    62      1.92488e-03      2.08474e-06
-    63      1.94417e-03      2.10389e-06
-    64      1.96319e-03      2.12269e-06
-    65      1.98193e-03      2.14117e-06
-    66      2.00041e-03      2.15931e-06
-    67      2.01862e-03      2.17714e-06
-    68      2.03658e-03      2.19464e-06
-    69      2.05427e-03      2.21183e-06
-    70      2.07171e-03      2.22871e-06
-    71      2.08890e-03      2.24529e-06
-    72      2.10584e-03      2.26156e-06
-    73      2.12253e-03      2.27753e-06
-    74      2.13898e-03      2.29321e-06
-    75      2.15521e-03      2.30861e-06
-    76      2.17118e-03      2.32370e-06
-    77      2.18693e-03      2.33852e-06
-    78      2.20244e-03      2.35306e-06
-    79      2.21772e-03      2.36732e-06
-    80      2.23278e-03      2.38131e-06
-    81      2.24762e-03      2.39503e-06
-    82      2.26223e-03      2.40847e-06
-    83      2.27664e-03      2.42166e-06
-    84      2.29082e-03      2.43458e-06
-    85      2.30479e-03      2.44725e-06
-    86      2.31854e-03      2.45966e-06
-    87      2.33208e-03      2.47181e-06
-    88      2.34542e-03      2.48372e-06
-    89      2.35855e-03      2.49538e-06
-    90      2.37148e-03      2.50679e-06
-    91      2.38421e-03      2.51797e-06
-    92      2.39675e-03      2.52890e-06
-    93      2.40907e-03      2.53959e-06
-    94      2.42121e-03      2.55006e-06
-    95      2.43315e-03      2.56029e-06
-    96      2.44489e-03      2.57028e-06
-    97      2.45645e-03      2.58005e-06
-    98      2.46781e-03      2.58959e-06
-    99      2.47899e-03      2.59892e-06
-   100      2.48998e-03      2.60802e-06
-   106      2.55212e-03      2.65809e-06
-   112      2.60793e-03      2.70072e-06
-   118      2.65767e-03      2.73629e-06
-   124      2.70162e-03      2.76517e-06
-   130      2.73999e-03      2.78772e-06
-   136      2.77300e-03      2.80426e-06
-   142      2.80085e-03      2.81509e-06
-   148      2.82370e-03      2.82051e-06
-   154      2.84175e-03      2.82082e-06
-   160      2.85514e-03      2.81629e-06
-   166      2.86403e-03      2.80717e-06
-   172      2.86855e-03      2.79375e-06
-   178      2.86887e-03      2.77629e-06
-   184      2.86509e-03      2.75504e-06
-   190      2.85738e-03      2.73028e-06
-   196      2.84583e-03      2.70227e-06
-   202      2.83059e-03      2.67126e-06
-   208      2.81177e-03      2.63751e-06
-   214      2.78949e-03      2.60127e-06
-   220      2.76389e-03      2.56282e-06
-   226      2.73507e-03      2.52242e-06
-   232      2.70315e-03      2.48035e-06
-   238      2.66825e-03      2.43688e-06
-   244      2.63049e-03      2.39229e-06
-   250      2.58999e-03      2.34686e-06
-   256      2.54685e-03      2.30086e-06
-   262      2.50122e-03      2.25460e-06
-   268      2.45318e-03      2.20834e-06
-   274      2.40288e-03      2.16239e-06
-   280      2.35043e-03      2.11704e-06
-   286      2.29595e-03      2.07255e-06
-   292      2.23956e-03      2.02917e-06
-   298      2.18139e-03      1.98714e-06
-   304      2.12156e-03      1.94671e-06
-   310      2.06019e-03      1.90808e-06
-   316      1.99742e-03      1.87144e-06
-   322      1.93337e-03      1.83693e-06
-   328      1.86817e-03      1.80469e-06
-   334      1.80197e-03      1.77478e-06
-   340      1.73487e-03      1.74722e-06
-   346      1.66702e-03      1.72201e-06
-   352      1.59857e-03      1.69908e-06
-   358      1.52965e-03      1.67830e-06
-   364      1.46039e-03      1.65950e-06
-   370      1.39093e-03      1.64246e-06
-   376      1.32143e-03      1.62691e-06
-   382      1.25204e-03      1.61253e-06
-   388      1.18289e-03      1.59898e-06
-   394      1.11413e-03      1.58586e-06
-   400      1.04591e-03      1.57276e-06
-   406      9.78403e-04      1.55925e-06
-   412      9.11743e-04      1.54487e-06
-   418      8.46096e-04      1.52915e-06
-   424      7.81619e-04      1.51163e-06
-   430      7.18472e-04      1.49182e-06
-   436      6.56821e-04      1.46923e-06
-   442      5.96828e-04      1.44340e-06
-   448      5.38662e-04      1.41385e-06
-   454      4.82492e-04      1.38008e-06
-   460      4.28488e-04      1.34165e-06
-   466      3.76824e-04      1.29824e-06
-   472      3.27677e-04      1.24933e-06
-   478      2.81222e-04      1.19440e-06
-   484      2.37640e-04      1.13299e-06
-   490      1.97112e-04      1.06465e-06
-   496      1.59822e-04      9.88963e-07
-   502      1.25955e-04      9.05484e-07
-   508      9.57020e-05      8.13781e-07
-   514      6.92504e-05      7.13432e-07
-   520      4.67934e-05      6.04009e-07
-   526      2.85254e-05      4.85093e-07
-   532      1.46431e-05      3.56264e-07
-   538      5.34511e-06      2.17106e-07
-   544      8.32526e-07      6.71990e-08
-   550      4.13539e-07      5.78955e-11
-   556      4.15022e-07      5.81031e-11
-   562      4.16470e-07      5.83059e-11
-   568      4.17883e-07      5.85037e-11
-   574      4.19263e-07      5.86968e-11
-   580      4.20608e-07      5.88851e-11
-   586      4.21918e-07      5.90685e-11
-   592      4.23194e-07      5.92471e-11
-   598      4.24435e-07      5.94210e-11
-   604      4.25643e-07      5.95901e-11
-   610      4.26817e-07      5.97544e-11
-   616      4.27957e-07      5.99140e-11
-   622      4.29063e-07      6.00688e-11
-   628      4.30135e-07      6.02189e-11
-   634      4.31173e-07      6.03643e-11
-   640      4.32178e-07      6.05050e-11
-   646      4.33150e-07      6.06410e-11
-   652      4.34087e-07      6.07722e-11
-   658      4.34991e-07      6.08987e-11
-   664      4.35862e-07      6.10207e-11
-   670      4.36699e-07      6.11379e-11
-   676      4.37503e-07      6.12505e-11
-   682      4.38274e-07      6.13584e-11
-   688      4.39012e-07      6.14617e-11
-   694      4.39716e-07      6.15602e-11
-   700      4.40387e-07      6.16541e-11
-   706      4.41025e-07      6.17435e-11
-   712      4.41629e-07      6.18281e-11
-   718      4.42201e-07      6.19081e-11
-   724      4.42740e-07      6.19836e-11
-   730      4.43245e-07      6.20543e-11
-   736      4.43718e-07      6.21205e-11
-   742      4.44158e-07      6.21821e-11
-   748      4.44565e-07      6.22391e-11
-   754      4.44938e-07      6.22913e-11
-   760      4.45279e-07      6.23391e-11
-   766      4.45588e-07      6.23823e-11
-   772      4.45863e-07      6.24208e-11
-   778      4.46105e-07      6.24547e-11
-   784      4.46315e-07      6.24842e-11
-   790      4.46492e-07      6.25089e-11
-   796      4.46637e-07      6.25292e-11
-   802      4.46749e-07      6.25449e-11
-   808      4.46828e-07      6.25559e-11
-   814      4.46875e-07      6.25624e-11
-   820      4.46889e-07      6.25644e-11
-   826      4.46870e-07      6.25618e-11
-   832      4.46818e-07      6.25546e-11
-   838      4.46734e-07      6.25428e-11
-   844      4.46617e-07      6.25264e-11
-   850      4.46468e-07      6.25055e-11
-   856      4.46287e-07      6.24801e-11
-   862      4.46072e-07      6.24501e-11
-   868      4.45825e-07      6.24154e-11
-   874      4.45545e-07      6.23763e-11
-   880      4.45233e-07      6.23327e-11
-   886      4.44888e-07      6.22844e-11
-   892      4.44510e-07      6.22315e-11
-   898      4.44100e-07      6.21740e-11
-   904      4.43657e-07      6.21120e-11
-   910      4.43181e-07      6.20453e-11
-   916      4.42673e-07      6.19742e-11
-   922      4.42131e-07      6.18984e-11
-   928      4.41557e-07      6.18179e-11
-   934      4.40950e-07      6.17330e-11
-   940      4.40309e-07      6.16433e-11
-   946      4.39636e-07      6.15490e-11
-   952      4.38929e-07      6.14501e-11
-   958      4.38190e-07      6.13465e-11
-   964      4.37417e-07      6.12384e-11
-   970      4.36610e-07      6.11255e-11
-   976      4.35770e-07      6.10078e-11
-   982      4.34897e-07      6.08856e-11
-   988      4.33990e-07      6.07586e-11
-   994      4.33049e-07      6.06269e-11
-  1000      4.32074e-07      6.04904e-11
-  1006      4.31066e-07      6.03492e-11
-  1012      4.30023e-07      6.02032e-11
-  1018      4.28945e-07      6.00523e-11
-  1024      4.27834e-07      5.98967e-11
-  1030      4.26687e-07      5.97362e-11
-  1036      4.25506e-07      5.95708e-11
-  1042      4.24289e-07      5.94005e-11
-  1048      4.23038e-07      5.92253e-11
-  1054      4.21752e-07      5.90452e-11
-  1060      4.20429e-07      5.88601e-11
-  1066      4.19071e-07      5.86699e-11
-  1072      4.17677e-07      5.84747e-11
-  1078      4.16247e-07      5.82745e-11
-  1084      4.14780e-07      5.80692e-11
-  1090      4.13276e-07      5.78587e-11
-  1096      4.11736e-07      5.76431e-11
-  1102      4.10159e-07      5.74223e-11
-  1108      4.08544e-07      5.71961e-11
-  1114      4.06891e-07      5.69648e-11
-  1120      4.05201e-07      5.67281e-11
-  1126      4.03472e-07      5.64861e-11
-  1132      4.01704e-07      5.62386e-11
-  1138      3.99898e-07      5.59857e-11
-  1144      3.98052e-07      5.57273e-11
-  1150      3.96167e-07      5.54634e-11
-  1156      3.94242e-07      5.51939e-11
-  1162      3.92277e-07      5.49187e-11
-  1168      3.90271e-07      5.46379e-11
-  1174      3.88224e-07      5.43514e-11
-  1180      3.86137e-07      5.40592e-11
-  1186      3.84007e-07      5.37610e-11
-  1192      3.81836e-07      5.34570e-11
-  1198      3.79623e-07      5.31472e-11
-  1204      3.77367e-07      5.28314e-11
-  1210      3.75068e-07      5.25095e-11
-  1216      3.72726e-07      5.21816e-11
-  1222      3.70339e-07      5.18475e-11
-  1228      3.67909e-07      5.15073e-11
-  1234      3.65435e-07      5.11609e-11
-  1240      3.62916e-07      5.08082e-11
-  1246      3.60351e-07      5.04492e-11
-  1252      3.57741e-07      5.00837e-11
-  1258      3.55085e-07      4.97120e-11
-  1264      3.52383e-07      4.93337e-11
-  1270      3.49634e-07      4.89488e-11
-  1276      3.46839e-07      4.85575e-11
-  1282      3.43997e-07      4.81596e-11
-  1288      3.41107e-07      4.77550e-11
-  1294      3.38169e-07      4.73437e-11
-  1300      3.35182e-07      4.69255e-11
-  1306      3.32147e-07      4.65006e-11
-  1312      3.29064e-07      4.60690e-11
-  1318      3.25932e-07      4.56305e-11
-  1324      3.22750e-07      4.51851e-11
-  1330      3.19520e-07      4.47328e-11
-  1336      3.16240e-07      4.42735e-11
-  1342      3.12909e-07      4.38073e-11
-  1348      3.09529e-07      4.33341e-11
-  1354      3.06100e-07      4.28540e-11
-  1360      3.02619e-07      4.23667e-11
-  1366      2.99089e-07      4.18725e-11
-  1372      2.95509e-07      4.13712e-11
-  1378      2.91878e-07      4.08629e-11
-  1384      2.88197e-07      4.03476e-11
-  1390      2.84466e-07      3.98253e-11
-  1396      2.80685e-07      3.92959e-11
-  1402      2.76854e-07      3.87595e-11
-  1408      2.72974e-07      3.82163e-11
-  1414      2.69044e-07      3.76662e-11
-  1420      2.65065e-07      3.71091e-11
-  1426      2.61037e-07      3.65452e-11
-  1432      2.56961e-07      3.59746e-11
-  1438      2.52838e-07      3.53973e-11
-  1444      2.48667e-07      3.48134e-11
-  1450      2.44449e-07      3.42229e-11
-  1456      2.40186e-07      3.36261e-11
-  1462      2.35877e-07      3.30229e-11
-  1468      2.31524e-07      3.24135e-11
-  1474      2.27128e-07      3.17980e-11
-  1480      2.22689e-07      3.11765e-11
-  1486      2.18209e-07      3.05493e-11
-  1492      2.13688e-07      2.99163e-11
-  1498      2.09128e-07      2.92780e-11
-  1504      2.04531e-07      2.86344e-11
-  1510      1.99897e-07      2.79857e-11
-  1516      1.95229e-07      2.73321e-11
-  1522      1.90527e-07      2.66739e-11
-  1528      1.85795e-07      2.60114e-11
-  1534      1.81034e-07      2.53448e-11
-  1540      1.76244e-07      2.46743e-11
-  1546      1.71431e-07      2.40004e-11
-  1552      1.66594e-07      2.33233e-11
-  1558      1.61737e-07      2.26432e-11
-  1564      1.56861e-07      2.19607e-11
-  1570      1.51972e-07      2.12762e-11
-  1576      1.47070e-07      2.05899e-11
-  1582      1.42158e-07      1.99023e-11
-  1588      1.37241e-07      1.92139e-11
-  1594      1.32321e-07      1.85251e-11
-  1600      1.27403e-07      1.78365e-11
-  1606      1.22489e-07      1.71486e-11
-  1612      1.17583e-07      1.64619e-11
-  1618      1.12691e-07      1.57770e-11
-  1624      1.07816e-07      1.50944e-11
-  1630      1.02962e-07      1.44149e-11
-  1636      9.81351e-08      1.37391e-11
-  1642      9.33389e-08      1.30677e-11
-  1648      8.85798e-08      1.24014e-11
-  1654      8.38626e-08      1.17410e-11
-  1660      7.91930e-08      1.10873e-11
-  1666      7.45772e-08      1.04411e-11
-  1672      7.00212e-08      9.80327e-12
-  1678      6.55316e-08      9.17473e-12
-  1684      6.11150e-08      8.55642e-12
-  1690      5.67785e-08      7.94933e-12
-  1696      5.25294e-08      7.35447e-12
-  1702      4.83752e-08      6.77289e-12
-  1708      4.43239e-08      6.20574e-12
-  1714      4.03838e-08      5.65415e-12
-  1720      3.65635e-08      5.11931e-12
-  1726      3.28718e-08      4.60250e-12
-  1732      2.93179e-08      4.10497e-12
-  1738      2.59114e-08      3.62809e-12
-  1744      2.26623e-08      3.17324e-12
-  1750      1.95810e-08      2.74188e-12
-  1756      1.66782e-08      2.33551e-12
-  1762      1.39649e-08      1.95567e-12
-  1768      1.14527e-08      1.60400e-12
-  1774      9.15351e-09      1.28213e-12
-  1780      7.07968e-09      9.91827e-13
-  1786      5.24402e-09      7.34864e-13
-  1792      3.65975e-09      5.13098e-13
-  1798      2.34057e-09      3.28446e-13
-  1804      1.30066e-09      1.82894e-13
-  1810      5.54672e-10      7.84916e-14
-  1816      1.17740e-10      1.73528e-14
- 1821.02    0.00000e+00      0.00000e+00
+---------------------------------------------------------------------------------------------
+
+BetaShape
+Version: 2.2 (05/2021)
+Author: X. Mougeot (xavier.mougeot@cea.fr)
+CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
+Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
+
+---------------------------------------------------------------------------------------------
+
+Total beta + spectrum from the Na-22 decay. See file of each transition for more details.
+
+Mean energy from the total beta + spectrum: 216.70 (24) keV
+
+E(keV)      dNtot/dE b+      unc.
+     0      0.00000e+00      0.00000e+00
+     1      2.23945e-06      2.53863e-09
+     2      1.91570e-05      2.17105e-08
+     3      4.98404e-05      5.64478e-08
+     4      8.85617e-05      1.00235e-07
+     5      1.31634e-04      1.48882e-07
+     6      1.76936e-04      1.99982e-07
+     7      2.23239e-04      2.52142e-07
+     8      2.69814e-04      3.04534e-07
+     9      3.16218e-04      3.56658e-07
+    10      3.62180e-04      4.08211e-07
+    11      4.07533e-04      4.59004e-07
+    12      4.52181e-04      5.08930e-07
+    13      4.96064e-04      5.57923e-07
+    14      5.39152e-04      6.05952e-07
+    15      5.81436e-04      6.53008e-07
+    16      6.22915e-04      6.99092e-07
+    17      6.63598e-04      7.44214e-07
+    18      7.03499e-04      7.88392e-07
+    19      7.42634e-04      8.31648e-07
+    20      7.81022e-04      8.74002e-07
+    21      8.18683e-04      9.15478e-07
+    22      8.55637e-04      9.56102e-07
+    23      8.91904e-04      9.95897e-07
+    24      9.27504e-04      1.03489e-06
+    25      9.62457e-04      1.07309e-06
+    26      9.96781e-04      1.11054e-06
+    27      1.03050e-03      1.14725e-06
+    28      1.06362e-03      1.18324e-06
+    29      1.09616e-03      1.21854e-06
+    30      1.12816e-03      1.25316e-06
+    31      1.15960e-03      1.28712e-06
+    32      1.19051e-03      1.32043e-06
+    33      1.22091e-03      1.35313e-06
+    34      1.25081e-03      1.38521e-06
+    35      1.28022e-03      1.41671e-06
+    36      1.30917e-03      1.44762e-06
+    37      1.33764e-03      1.47797e-06
+    38      1.36566e-03      1.50777e-06
+    39      1.39323e-03      1.53703e-06
+    40      1.42038e-03      1.56577e-06
+    41      1.44710e-03      1.59399e-06
+    42      1.47343e-03      1.62172e-06
+    43      1.49934e-03      1.64895e-06
+    44      1.52486e-03      1.67570e-06
+    45      1.54999e-03      1.70198e-06
+    46      1.57474e-03      1.72779e-06
+    47      1.59912e-03      1.75316e-06
+    48      1.62315e-03      1.77808e-06
+    49      1.64682e-03      1.80257e-06
+    50      1.67013e-03      1.82663e-06
+    51      1.69311e-03      1.85028e-06
+    52      1.71574e-03      1.87351e-06
+    53      1.73805e-03      1.89634e-06
+    54      1.76005e-03      1.91878e-06
+    55      1.78171e-03      1.94082e-06
+    56      1.80306e-03      1.96248e-06
+    57      1.82410e-03      1.98376e-06
+    58      1.84484e-03      2.00467e-06
+    59      1.86529e-03      2.02523e-06
+    60      1.88543e-03      2.04541e-06
+    61      1.90530e-03      2.06525e-06
+    62      1.92488e-03      2.08474e-06
+    63      1.94417e-03      2.10389e-06
+    64      1.96319e-03      2.12269e-06
+    65      1.98193e-03      2.14117e-06
+    66      2.00041e-03      2.15931e-06
+    67      2.01862e-03      2.17714e-06
+    68      2.03658e-03      2.19464e-06
+    69      2.05427e-03      2.21183e-06
+    70      2.07171e-03      2.22871e-06
+    71      2.08890e-03      2.24529e-06
+    72      2.10584e-03      2.26156e-06
+    73      2.12253e-03      2.27753e-06
+    74      2.13898e-03      2.29321e-06
+    75      2.15521e-03      2.30861e-06
+    76      2.17118e-03      2.32370e-06
+    77      2.18693e-03      2.33852e-06
+    78      2.20244e-03      2.35306e-06
+    79      2.21772e-03      2.36732e-06
+    80      2.23278e-03      2.38131e-06
+    81      2.24762e-03      2.39503e-06
+    82      2.26223e-03      2.40847e-06
+    83      2.27664e-03      2.42166e-06
+    84      2.29082e-03      2.43458e-06
+    85      2.30479e-03      2.44725e-06
+    86      2.31854e-03      2.45966e-06
+    87      2.33208e-03      2.47181e-06
+    88      2.34542e-03      2.48372e-06
+    89      2.35855e-03      2.49538e-06
+    90      2.37148e-03      2.50679e-06
+    91      2.38421e-03      2.51797e-06
+    92      2.39675e-03      2.52890e-06
+    93      2.40907e-03      2.53959e-06
+    94      2.42121e-03      2.55006e-06
+    95      2.43315e-03      2.56029e-06
+    96      2.44489e-03      2.57028e-06
+    97      2.45645e-03      2.58005e-06
+    98      2.46781e-03      2.58959e-06
+    99      2.47899e-03      2.59892e-06
+   100      2.48998e-03      2.60802e-06
+   106      2.55212e-03      2.65809e-06
+   112      2.60793e-03      2.70072e-06
+   118      2.65767e-03      2.73629e-06
+   124      2.70162e-03      2.76517e-06
+   130      2.73999e-03      2.78772e-06
+   136      2.77300e-03      2.80426e-06
+   142      2.80085e-03      2.81509e-06
+   148      2.82370e-03      2.82051e-06
+   154      2.84175e-03      2.82082e-06
+   160      2.85514e-03      2.81629e-06
+   166      2.86403e-03      2.80717e-06
+   172      2.86855e-03      2.79375e-06
+   178      2.86887e-03      2.77629e-06
+   184      2.86509e-03      2.75504e-06
+   190      2.85738e-03      2.73028e-06
+   196      2.84583e-03      2.70227e-06
+   202      2.83059e-03      2.67126e-06
+   208      2.81177e-03      2.63751e-06
+   214      2.78949e-03      2.60127e-06
+   220      2.76389e-03      2.56282e-06
+   226      2.73507e-03      2.52242e-06
+   232      2.70315e-03      2.48035e-06
+   238      2.66825e-03      2.43688e-06
+   244      2.63049e-03      2.39229e-06
+   250      2.58999e-03      2.34686e-06
+   256      2.54685e-03      2.30086e-06
+   262      2.50122e-03      2.25460e-06
+   268      2.45318e-03      2.20834e-06
+   274      2.40288e-03      2.16239e-06
+   280      2.35043e-03      2.11704e-06
+   286      2.29595e-03      2.07255e-06
+   292      2.23956e-03      2.02917e-06
+   298      2.18139e-03      1.98714e-06
+   304      2.12156e-03      1.94671e-06
+   310      2.06019e-03      1.90808e-06
+   316      1.99742e-03      1.87144e-06
+   322      1.93337e-03      1.83693e-06
+   328      1.86817e-03      1.80469e-06
+   334      1.80197e-03      1.77478e-06
+   340      1.73487e-03      1.74722e-06
+   346      1.66702e-03      1.72201e-06
+   352      1.59857e-03      1.69908e-06
+   358      1.52965e-03      1.67830e-06
+   364      1.46039e-03      1.65950e-06
+   370      1.39093e-03      1.64246e-06
+   376      1.32143e-03      1.62691e-06
+   382      1.25204e-03      1.61253e-06
+   388      1.18289e-03      1.59898e-06
+   394      1.11413e-03      1.58586e-06
+   400      1.04591e-03      1.57276e-06
+   406      9.78403e-04      1.55925e-06
+   412      9.11743e-04      1.54487e-06
+   418      8.46096e-04      1.52915e-06
+   424      7.81619e-04      1.51163e-06
+   430      7.18472e-04      1.49182e-06
+   436      6.56821e-04      1.46923e-06
+   442      5.96828e-04      1.44340e-06
+   448      5.38662e-04      1.41385e-06
+   454      4.82492e-04      1.38008e-06
+   460      4.28488e-04      1.34165e-06
+   466      3.76824e-04      1.29824e-06
+   472      3.27677e-04      1.24933e-06
+   478      2.81222e-04      1.19440e-06
+   484      2.37640e-04      1.13299e-06
+   490      1.97112e-04      1.06465e-06
+   496      1.59822e-04      9.88963e-07
+   502      1.25955e-04      9.05484e-07
+   508      9.57020e-05      8.13781e-07
+   514      6.92504e-05      7.13432e-07
+   520      4.67934e-05      6.04009e-07
+   526      2.85254e-05      4.85093e-07
+   532      1.46431e-05      3.56264e-07
+   538      5.34511e-06      2.17106e-07
+   544      8.32526e-07      6.71990e-08
+   550      4.13539e-07      5.78955e-11
+   556      4.15022e-07      5.81031e-11
+   562      4.16470e-07      5.83059e-11
+   568      4.17883e-07      5.85037e-11
+   574      4.19263e-07      5.86968e-11
+   580      4.20608e-07      5.88851e-11
+   586      4.21918e-07      5.90685e-11
+   592      4.23194e-07      5.92471e-11
+   598      4.24435e-07      5.94210e-11
+   604      4.25643e-07      5.95901e-11
+   610      4.26817e-07      5.97544e-11
+   616      4.27957e-07      5.99140e-11
+   622      4.29063e-07      6.00688e-11
+   628      4.30135e-07      6.02189e-11
+   634      4.31173e-07      6.03643e-11
+   640      4.32178e-07      6.05050e-11
+   646      4.33150e-07      6.06410e-11
+   652      4.34087e-07      6.07722e-11
+   658      4.34991e-07      6.08987e-11
+   664      4.35862e-07      6.10207e-11
+   670      4.36699e-07      6.11379e-11
+   676      4.37503e-07      6.12505e-11
+   682      4.38274e-07      6.13584e-11
+   688      4.39012e-07      6.14617e-11
+   694      4.39716e-07      6.15602e-11
+   700      4.40387e-07      6.16541e-11
+   706      4.41025e-07      6.17435e-11
+   712      4.41629e-07      6.18281e-11
+   718      4.42201e-07      6.19081e-11
+   724      4.42740e-07      6.19836e-11
+   730      4.43245e-07      6.20543e-11
+   736      4.43718e-07      6.21205e-11
+   742      4.44158e-07      6.21821e-11
+   748      4.44565e-07      6.22391e-11
+   754      4.44938e-07      6.22913e-11
+   760      4.45279e-07      6.23391e-11
+   766      4.45588e-07      6.23823e-11
+   772      4.45863e-07      6.24208e-11
+   778      4.46105e-07      6.24547e-11
+   784      4.46315e-07      6.24842e-11
+   790      4.46492e-07      6.25089e-11
+   796      4.46637e-07      6.25292e-11
+   802      4.46749e-07      6.25449e-11
+   808      4.46828e-07      6.25559e-11
+   814      4.46875e-07      6.25624e-11
+   820      4.46889e-07      6.25644e-11
+   826      4.46870e-07      6.25618e-11
+   832      4.46818e-07      6.25546e-11
+   838      4.46734e-07      6.25428e-11
+   844      4.46617e-07      6.25264e-11
+   850      4.46468e-07      6.25055e-11
+   856      4.46287e-07      6.24801e-11
+   862      4.46072e-07      6.24501e-11
+   868      4.45825e-07      6.24154e-11
+   874      4.45545e-07      6.23763e-11
+   880      4.45233e-07      6.23327e-11
+   886      4.44888e-07      6.22844e-11
+   892      4.44510e-07      6.22315e-11
+   898      4.44100e-07      6.21740e-11
+   904      4.43657e-07      6.21120e-11
+   910      4.43181e-07      6.20453e-11
+   916      4.42673e-07      6.19742e-11
+   922      4.42131e-07      6.18984e-11
+   928      4.41557e-07      6.18179e-11
+   934      4.40950e-07      6.17330e-11
+   940      4.40309e-07      6.16433e-11
+   946      4.39636e-07      6.15490e-11
+   952      4.38929e-07      6.14501e-11
+   958      4.38190e-07      6.13465e-11
+   964      4.37417e-07      6.12384e-11
+   970      4.36610e-07      6.11255e-11
+   976      4.35770e-07      6.10078e-11
+   982      4.34897e-07      6.08856e-11
+   988      4.33990e-07      6.07586e-11
+   994      4.33049e-07      6.06269e-11
+  1000      4.32074e-07      6.04904e-11
+  1006      4.31066e-07      6.03492e-11
+  1012      4.30023e-07      6.02032e-11
+  1018      4.28945e-07      6.00523e-11
+  1024      4.27834e-07      5.98967e-11
+  1030      4.26687e-07      5.97362e-11
+  1036      4.25506e-07      5.95708e-11
+  1042      4.24289e-07      5.94005e-11
+  1048      4.23038e-07      5.92253e-11
+  1054      4.21752e-07      5.90452e-11
+  1060      4.20429e-07      5.88601e-11
+  1066      4.19071e-07      5.86699e-11
+  1072      4.17677e-07      5.84747e-11
+  1078      4.16247e-07      5.82745e-11
+  1084      4.14780e-07      5.80692e-11
+  1090      4.13276e-07      5.78587e-11
+  1096      4.11736e-07      5.76431e-11
+  1102      4.10159e-07      5.74223e-11
+  1108      4.08544e-07      5.71961e-11
+  1114      4.06891e-07      5.69648e-11
+  1120      4.05201e-07      5.67281e-11
+  1126      4.03472e-07      5.64861e-11
+  1132      4.01704e-07      5.62386e-11
+  1138      3.99898e-07      5.59857e-11
+  1144      3.98052e-07      5.57273e-11
+  1150      3.96167e-07      5.54634e-11
+  1156      3.94242e-07      5.51939e-11
+  1162      3.92277e-07      5.49187e-11
+  1168      3.90271e-07      5.46379e-11
+  1174      3.88224e-07      5.43514e-11
+  1180      3.86137e-07      5.40592e-11
+  1186      3.84007e-07      5.37610e-11
+  1192      3.81836e-07      5.34570e-11
+  1198      3.79623e-07      5.31472e-11
+  1204      3.77367e-07      5.28314e-11
+  1210      3.75068e-07      5.25095e-11
+  1216      3.72726e-07      5.21816e-11
+  1222      3.70339e-07      5.18475e-11
+  1228      3.67909e-07      5.15073e-11
+  1234      3.65435e-07      5.11609e-11
+  1240      3.62916e-07      5.08082e-11
+  1246      3.60351e-07      5.04492e-11
+  1252      3.57741e-07      5.00837e-11
+  1258      3.55085e-07      4.97120e-11
+  1264      3.52383e-07      4.93337e-11
+  1270      3.49634e-07      4.89488e-11
+  1276      3.46839e-07      4.85575e-11
+  1282      3.43997e-07      4.81596e-11
+  1288      3.41107e-07      4.77550e-11
+  1294      3.38169e-07      4.73437e-11
+  1300      3.35182e-07      4.69255e-11
+  1306      3.32147e-07      4.65006e-11
+  1312      3.29064e-07      4.60690e-11
+  1318      3.25932e-07      4.56305e-11
+  1324      3.22750e-07      4.51851e-11
+  1330      3.19520e-07      4.47328e-11
+  1336      3.16240e-07      4.42735e-11
+  1342      3.12909e-07      4.38073e-11
+  1348      3.09529e-07      4.33341e-11
+  1354      3.06100e-07      4.28540e-11
+  1360      3.02619e-07      4.23667e-11
+  1366      2.99089e-07      4.18725e-11
+  1372      2.95509e-07      4.13712e-11
+  1378      2.91878e-07      4.08629e-11
+  1384      2.88197e-07      4.03476e-11
+  1390      2.84466e-07      3.98253e-11
+  1396      2.80685e-07      3.92959e-11
+  1402      2.76854e-07      3.87595e-11
+  1408      2.72974e-07      3.82163e-11
+  1414      2.69044e-07      3.76662e-11
+  1420      2.65065e-07      3.71091e-11
+  1426      2.61037e-07      3.65452e-11
+  1432      2.56961e-07      3.59746e-11
+  1438      2.52838e-07      3.53973e-11
+  1444      2.48667e-07      3.48134e-11
+  1450      2.44449e-07      3.42229e-11
+  1456      2.40186e-07      3.36261e-11
+  1462      2.35877e-07      3.30229e-11
+  1468      2.31524e-07      3.24135e-11
+  1474      2.27128e-07      3.17980e-11
+  1480      2.22689e-07      3.11765e-11
+  1486      2.18209e-07      3.05493e-11
+  1492      2.13688e-07      2.99163e-11
+  1498      2.09128e-07      2.92780e-11
+  1504      2.04531e-07      2.86344e-11
+  1510      1.99897e-07      2.79857e-11
+  1516      1.95229e-07      2.73321e-11
+  1522      1.90527e-07      2.66739e-11
+  1528      1.85795e-07      2.60114e-11
+  1534      1.81034e-07      2.53448e-11
+  1540      1.76244e-07      2.46743e-11
+  1546      1.71431e-07      2.40004e-11
+  1552      1.66594e-07      2.33233e-11
+  1558      1.61737e-07      2.26432e-11
+  1564      1.56861e-07      2.19607e-11
+  1570      1.51972e-07      2.12762e-11
+  1576      1.47070e-07      2.05899e-11
+  1582      1.42158e-07      1.99023e-11
+  1588      1.37241e-07      1.92139e-11
+  1594      1.32321e-07      1.85251e-11
+  1600      1.27403e-07      1.78365e-11
+  1606      1.22489e-07      1.71486e-11
+  1612      1.17583e-07      1.64619e-11
+  1618      1.12691e-07      1.57770e-11
+  1624      1.07816e-07      1.50944e-11
+  1630      1.02962e-07      1.44149e-11
+  1636      9.81351e-08      1.37391e-11
+  1642      9.33389e-08      1.30677e-11
+  1648      8.85798e-08      1.24014e-11
+  1654      8.38626e-08      1.17410e-11
+  1660      7.91930e-08      1.10873e-11
+  1666      7.45772e-08      1.04411e-11
+  1672      7.00212e-08      9.80327e-12
+  1678      6.55316e-08      9.17473e-12
+  1684      6.11150e-08      8.55642e-12
+  1690      5.67785e-08      7.94933e-12
+  1696      5.25294e-08      7.35447e-12
+  1702      4.83752e-08      6.77289e-12
+  1708      4.43239e-08      6.20574e-12
+  1714      4.03838e-08      5.65415e-12
+  1720      3.65635e-08      5.11931e-12
+  1726      3.28718e-08      4.60250e-12
+  1732      2.93179e-08      4.10497e-12
+  1738      2.59114e-08      3.62809e-12
+  1744      2.26623e-08      3.17324e-12
+  1750      1.95810e-08      2.74188e-12
+  1756      1.66782e-08      2.33551e-12
+  1762      1.39649e-08      1.95567e-12
+  1768      1.14527e-08      1.60400e-12
+  1774      9.15351e-09      1.28213e-12
+  1780      7.07968e-09      9.91827e-13
+  1786      5.24402e-09      7.34864e-13
+  1792      3.65975e-09      5.13098e-13
+  1798      2.34057e-09      3.28446e-13
+  1804      1.30066e-09      1.82894e-13
+  1810      5.54672e-10      7.84916e-14
+  1816      1.17740e-10      1.73528e-14
+ 1821.02    0.00000e+00      0.00000e+00
```

### Comparing `opengate-10.0b7/opengate/sources/beta_plus_spectra/O15/beta+_O15_tot.bs` & `opengate-10.0b8/opengate/sources/beta_plus_spectra/F18/beta+_F18_tot.bs`

 * *Files 26% similar despite different names*

```diff
@@ -1,363 +1,333 @@
----------------------------------------------------------------------------------------------
-
-BetaShape
-Version: 2.2 (05/2021)
-Author: X. Mougeot (xavier.mougeot@cea.fr)
-CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
-Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
-
----------------------------------------------------------------------------------------------
-
-Total beta + spectrum from the O-15 decay. See file of each transition for more details.
-
-Mean energy from the total beta + spectrum: 734.8 (6) keV
-
-E(keV)      dNtot/dE b+      unc.
-     0      0.00000e+00      0.00000e+00
-     5      2.62304e-05      4.45546e-08
-    10      5.37915e-05      9.11348e-08
-    15      7.79110e-05      1.31657e-07
-    20      9.95482e-05      1.67781e-07
-    25      1.19378e-04      2.00671e-07
-    30      1.37834e-04      2.31080e-07
-    35      1.55207e-04      2.59509e-07
-    40      1.71702e-04      2.86312e-07
-    45      1.87467e-04      3.11747e-07
-    50      2.02614e-04      3.36009e-07
-    55      2.17229e-04      3.59247e-07
-    60      2.31382e-04      3.81580e-07
-    65      2.45126e-04      4.03103e-07
-    70      2.58505e-04      4.23894e-07
-    75      2.71558e-04      4.44016e-07
-    80      2.84313e-04      4.63523e-07
-    85      2.96798e-04      4.82460e-07
-    90      3.09034e-04      5.00866e-07
-    95      3.21040e-04      5.18773e-07
-   100      3.32832e-04      5.36210e-07
-   105      3.44425e-04      5.53200e-07
-   110      3.55830e-04      5.69766e-07
-   115      3.67058e-04      5.85926e-07
-   120      3.78119e-04      6.01697e-07
-   125      3.89020e-04      6.17093e-07
-   130      3.99770e-04      6.32127e-07
-   135      4.10375e-04      6.46811e-07
-   140      4.20840e-04      6.61155e-07
-   145      4.31172e-04      6.75167e-07
-   150      4.41373e-04      6.88856e-07
-   155      4.51449e-04      7.02230e-07
-   160      4.61403e-04      7.15294e-07
-   165      4.71239e-04      7.28055e-07
-   170      4.80960e-04      7.40518e-07
-   175      4.90567e-04      7.52688e-07
-   180      5.00064e-04      7.64570e-07
-   185      5.09453e-04      7.76166e-07
-   190      5.18736e-04      7.87482e-07
-   195      5.27915e-04      7.98519e-07
-   200      5.36990e-04      8.09282e-07
-   205      5.45964e-04      8.19772e-07
-   210      5.54838e-04      8.29992e-07
-   215      5.63613e-04      8.39944e-07
-   220      5.72290e-04      8.49631e-07
-   225      5.80870e-04      8.59054e-07
-   230      5.89354e-04      8.68215e-07
-   235      5.97742e-04      8.77115e-07
-   240      6.06035e-04      8.85756e-07
-   245      6.14234e-04      8.94139e-07
-   250      6.22339e-04      9.02266e-07
-   255      6.30351e-04      9.10136e-07
-   260      6.38270e-04      9.17753e-07
-   265      6.46097e-04      9.25115e-07
-   270      6.53831e-04      9.32225e-07
-   275      6.61473e-04      9.39082e-07
-   280      6.69023e-04      9.45688e-07
-   285      6.76482e-04      9.52044e-07
-   290      6.83848e-04      9.58150e-07
-   295      6.91124e-04      9.64006e-07
-   300      6.98308e-04      9.69613e-07
-   305      7.05401e-04      9.74972e-07
-   310      7.12402e-04      9.80084e-07
-   315      7.19312e-04      9.84948e-07
-   320      7.26131e-04      9.89565e-07
-   325      7.32858e-04      9.93936e-07
-   330      7.39494e-04      9.98060e-07
-   335      7.46039e-04      1.00194e-06
-   340      7.52492e-04      1.00557e-06
-   345      7.58853e-04      1.00896e-06
-   350      7.65123e-04      1.01211e-06
-   355      7.71301e-04      1.01501e-06
-   360      7.77386e-04      1.01767e-06
-   365      7.83380e-04      1.02008e-06
-   370      7.89282e-04      1.02225e-06
-   375      7.95091e-04      1.02418e-06
-   380      8.00808e-04      1.02587e-06
-   385      8.06432e-04      1.02732e-06
-   390      8.11963e-04      1.02852e-06
-   395      8.17402e-04      1.02949e-06
-   400      8.22747e-04      1.03021e-06
-   405      8.28000e-04      1.03070e-06
-   410      8.33158e-04      1.03094e-06
-   415      8.38224e-04      1.03095e-06
-   420      8.43196e-04      1.03072e-06
-   425      8.48074e-04      1.03025e-06
-   430      8.52858e-04      1.02955e-06
-   435      8.57547e-04      1.02861e-06
-   440      8.62143e-04      1.02743e-06
-   445      8.66644e-04      1.02602e-06
-   450      8.71051e-04      1.02437e-06
-   455      8.75363e-04      1.02249e-06
-   460      8.79581e-04      1.02037e-06
-   465      8.83703e-04      1.01803e-06
-   470      8.87730e-04      1.01545e-06
-   475      8.91663e-04      1.01264e-06
-   480      8.95500e-04      1.00960e-06
-   485      8.99241e-04      1.00633e-06
-   490      9.02888e-04      1.00283e-06
-   495      9.06438e-04      9.99104e-07
-   500      9.09893e-04      9.95151e-07
-   505      9.13253e-04      9.90971e-07
-   510      9.16516e-04      9.86566e-07
-   515      9.19684e-04      9.81937e-07
-   520      9.22755e-04      9.77084e-07
-   525      9.25731e-04      9.72009e-07
-   530      9.28610e-04      9.66712e-07
-   535      9.31394e-04      9.61195e-07
-   540      9.34081e-04      9.55459e-07
-   545      9.36672e-04      9.49505e-07
-   550      9.39167e-04      9.43334e-07
-   555      9.41565e-04      9.36946e-07
-   560      9.43868e-04      9.30344e-07
-   565      9.46074e-04      9.23529e-07
-   570      9.48184e-04      9.16501e-07
-   575      9.50197e-04      9.09262e-07
-   580      9.52115e-04      9.01814e-07
-   585      9.53936e-04      8.94157e-07
-   590      9.55661e-04      8.86293e-07
-   595      9.57290e-04      8.78223e-07
-   600      9.58823e-04      8.69949e-07
-   605      9.60260e-04      8.61472e-07
-   610      9.61601e-04      8.52793e-07
-   615      9.62847e-04      8.43915e-07
-   620      9.63996e-04      8.34839e-07
-   625      9.65050e-04      8.25565e-07
-   630      9.66008e-04      8.16097e-07
-   635      9.66871e-04      8.06435e-07
-   640      9.67639e-04      7.96580e-07
-   645      9.68311e-04      7.86536e-07
-   650      9.68889e-04      7.76303e-07
-   655      9.69371e-04      7.65883e-07
-   660      9.69759e-04      7.55278e-07
-   665      9.70052e-04      7.44490e-07
-   670      9.70250e-04      7.33520e-07
-   675      9.70355e-04      7.22371e-07
-   680      9.70365e-04      7.11044e-07
-   685      9.70282e-04      6.99541e-07
-   690      9.70105e-04      6.87879e-07
-   695      9.69835e-04      6.76076e-07
-   700      9.69471e-04      6.64103e-07
-   705      9.69014e-04      6.51963e-07
-   710      9.68465e-04      6.39657e-07
-   715      9.67824e-04      6.27188e-07
-   720      9.67090e-04      6.14557e-07
-   725      9.66264e-04      6.01767e-07
-   730      9.65347e-04      5.88821e-07
-   735      9.64339e-04      5.75719e-07
-   740      9.63239e-04      5.62466e-07
-   745      9.62049e-04      5.49062e-07
-   750      9.60768e-04      5.35510e-07
-   755      9.59398e-04      5.21812e-07
-   760      9.57937e-04      5.07972e-07
-   765      9.56388e-04      4.93990e-07
-   770      9.54749e-04      4.79870e-07
-   775      9.53022e-04      4.65615e-07
-   780      9.51207e-04      4.51226e-07
-   785      9.49303e-04      4.36706e-07
-   790      9.47313e-04      4.22058e-07
-   795      9.45235e-04      4.07284e-07
-   800      9.43071e-04      3.92387e-07
-   805      9.40820e-04      3.77370e-07
-   810      9.38484e-04      3.62235e-07
-   815      9.36063e-04      3.46985e-07
-   820      9.33557e-04      3.31623e-07
-   825      9.30966e-04      3.16152e-07
-   830      9.28292e-04      3.00573e-07
-   835      9.25534e-04      2.84891e-07
-   840      9.22693e-04      2.69108e-07
-   845      9.19770e-04      2.53227e-07
-   850      9.16765e-04      2.37251e-07
-   855      9.13679e-04      2.21183e-07
-   860      9.10511e-04      2.05026e-07
-   865      9.07264e-04      1.88783e-07
-   870      9.03937e-04      1.72457e-07
-   875      9.00531e-04      1.56050e-07
-   880      8.97046e-04      1.39568e-07
-   885      8.93483e-04      1.23011e-07
-   890      8.89843e-04      1.06384e-07
-   895      8.86126e-04      8.96900e-08
-   900      8.82333e-04      7.29319e-08
-   905      8.78465e-04      5.61133e-08
-   910      8.74521e-04      3.92373e-08
-   915      8.70503e-04      2.23073e-08
-   920      8.66412e-04      5.32683e-09
-   925      8.62248e-04      1.39256e-08
-   930      8.58011e-04      3.10404e-08
-   935      8.53703e-04      4.81951e-08
-   940      8.49324e-04      6.53860e-08
-   945      8.44875e-04      8.26098e-08
-   950      8.40357e-04      9.98626e-08
-   955      8.35770e-04      1.17141e-07
-   960      8.31114e-04      1.34441e-07
-   965      8.26392e-04      1.51760e-07
-   970      8.21603e-04      1.69093e-07
-   975      8.16748e-04      1.86436e-07
-   980      8.11829e-04      2.03787e-07
-   985      8.06845e-04      2.21141e-07
-   990      8.01798e-04      2.38494e-07
-   995      7.96688e-04      2.55842e-07
-  1000      7.91516e-04      2.73182e-07
-  1005      7.86284e-04      2.90510e-07
-  1010      7.80991e-04      3.07821e-07
-  1015      7.75640e-04      3.25111e-07
-  1020      7.70230e-04      3.42377e-07
-  1025      7.64762e-04      3.59615e-07
-  1030      7.59237e-04      3.76820e-07
-  1035      7.53657e-04      3.93988e-07
-  1040      7.48022e-04      4.11116e-07
-  1045      7.42333e-04      4.28198e-07
-  1050      7.36591e-04      4.45231e-07
-  1055      7.30797e-04      4.62210e-07
-  1060      7.24952e-04      4.79131e-07
-  1065      7.19056e-04      4.95991e-07
-  1070      7.13111e-04      5.12783e-07
-  1075      7.07118e-04      5.29505e-07
-  1080      7.01077e-04      5.46151e-07
-  1085      6.94990e-04      5.62718e-07
-  1090      6.88858e-04      5.79200e-07
-  1095      6.82681e-04      5.95593e-07
-  1100      6.76461e-04      6.11894e-07
-  1105      6.70198e-04      6.28096e-07
-  1110      6.63894e-04      6.44195e-07
-  1115      6.57550e-04      6.60188e-07
-  1120      6.51167e-04      6.76069e-07
-  1125      6.44745e-04      6.91833e-07
-  1130      6.38287e-04      7.07476e-07
-  1135      6.31792e-04      7.22993e-07
-  1140      6.25263e-04      7.38379e-07
-  1145      6.18699e-04      7.53629e-07
-  1150      6.12103e-04      7.68739e-07
-  1155      6.05476e-04      7.83704e-07
-  1160      5.98818e-04      7.98518e-07
-  1165      5.92130e-04      8.13177e-07
-  1170      5.85415e-04      8.27676e-07
-  1175      5.78673e-04      8.42010e-07
-  1180      5.71904e-04      8.56173e-07
-  1185      5.65112e-04      8.70161e-07
-  1190      5.58295e-04      8.83969e-07
-  1195      5.51457e-04      8.97591e-07
-  1200      5.44597e-04      9.11022e-07
-  1205      5.37718e-04      9.24257e-07
-  1210      5.30820e-04      9.37292e-07
-  1215      5.23905e-04      9.50119e-07
-  1220      5.16974e-04      9.62735e-07
-  1225      5.10028e-04      9.75134e-07
-  1230      5.03069e-04      9.87311e-07
-  1235      4.96097e-04      9.99259e-07
-  1240      4.89114e-04      1.01097e-06
-  1245      4.82122e-04      1.02245e-06
-  1250      4.75121e-04      1.03368e-06
-  1255      4.68113e-04      1.04467e-06
-  1260      4.61100e-04      1.05540e-06
-  1265      4.54082e-04      1.06586e-06
-  1270      4.47061e-04      1.07606e-06
-  1275      4.40039e-04      1.08599e-06
-  1280      4.33016e-04      1.09564e-06
-  1285      4.25995e-04      1.10501e-06
-  1290      4.18976e-04      1.11409e-06
-  1295      4.11960e-04      1.12288e-06
-  1300      4.04951e-04      1.13136e-06
-  1305      3.97948e-04      1.13954e-06
-  1310      3.90953e-04      1.14740e-06
-  1315      3.83967e-04      1.15495e-06
-  1320      3.76993e-04      1.16217e-06
-  1325      3.70031e-04      1.16907e-06
-  1330      3.63083e-04      1.17562e-06
-  1335      3.56151e-04      1.18184e-06
-  1340      3.49236e-04      1.18771e-06
-  1345      3.42339e-04      1.19322e-06
-  1350      3.35462e-04      1.19837e-06
-  1355      3.28606e-04      1.20316e-06
-  1360      3.21773e-04      1.20758e-06
-  1365      3.14965e-04      1.21161e-06
-  1370      3.08183e-04      1.21527e-06
-  1375      3.01429e-04      1.21853e-06
-  1380      2.94704e-04      1.22139e-06
-  1385      2.88010e-04      1.22386e-06
-  1390      2.81348e-04      1.22591e-06
-  1395      2.74719e-04      1.22754e-06
-  1400      2.68127e-04      1.22876e-06
-  1405      2.61572e-04      1.22954e-06
-  1410      2.55055e-04      1.22989e-06
-  1415      2.48579e-04      1.22980e-06
-  1420      2.42145e-04      1.22926e-06
-  1425      2.35755e-04      1.22826e-06
-  1430      2.29410e-04      1.22681e-06
-  1435      2.23112e-04      1.22488e-06
-  1440      2.16863e-04      1.22249e-06
-  1445      2.10664e-04      1.21961e-06
-  1450      2.04517e-04      1.21624e-06
-  1455      1.98424e-04      1.21238e-06
-  1460      1.92387e-04      1.20802e-06
-  1465      1.86407e-04      1.20315e-06
-  1470      1.80486e-04      1.19777e-06
-  1475      1.74626e-04      1.19186e-06
-  1480      1.68829e-04      1.18543e-06
-  1485      1.63095e-04      1.17855e-06
-  1490      1.57428e-04      1.17118e-06
-  1495      1.51829e-04      1.16326e-06
-  1500      1.46299e-04      1.15479e-06
-  1505      1.40840e-04      1.14576e-06
-  1510      1.35455e-04      1.13617e-06
-  1515      1.30145e-04      1.12600e-06
-  1520      1.24912e-04      1.11525e-06
-  1525      1.19758e-04      1.10391e-06
-  1530      1.14684e-04      1.09198e-06
-  1535      1.09693e-04      1.07945e-06
-  1540      1.04786e-04      1.06632e-06
-  1545      9.99649e-05      1.05256e-06
-  1550      9.52322e-05      1.03819e-06
-  1555      9.05895e-05      1.02318e-06
-  1560      8.60386e-05      1.00754e-06
-  1565      8.15816e-05      9.91255e-07
-  1570      7.72202e-05      9.74320e-07
-  1575      7.29565e-05      9.56727e-07
-  1580      6.87923e-05      9.38469e-07
-  1585      6.47296e-05      9.19539e-07
-  1590      6.07705e-05      8.99929e-07
-  1595      5.69167e-05      8.79634e-07
-  1600      5.31704e-05      8.58645e-07
-  1605      4.95334e-05      8.36955e-07
-  1610      4.60078e-05      8.14557e-07
-  1615      4.25956e-05      7.91444e-07
-  1620      3.92987e-05      7.67609e-07
-  1625      3.61193e-05      7.43045e-07
-  1630      3.30591e-05      7.17744e-07
-  1635      3.01205e-05      6.91700e-07
-  1640      2.73052e-05      6.64905e-07
-  1645      2.46154e-05      6.37352e-07
-  1650      2.20532e-05      6.09036e-07
-  1655      1.96205e-05      5.79947e-07
-  1660      1.73194e-05      5.50081e-07
-  1665      1.51521e-05      5.19430e-07
-  1670      1.31205e-05      4.87988e-07
-  1675      1.12267e-05      4.55748e-07
-  1680      9.47276e-06      4.22705e-07
-  1685      7.86081e-06      3.88852e-07
-  1690      6.39290e-06      3.54185e-07
-  1695      5.07108e-06      3.18698e-07
-  1700      3.89744e-06      2.82387e-07
-  1705      2.87402e-06      2.45250e-07
-  1710      2.00288e-06      2.07284e-07
-  1715      1.28603e-06      1.68490e-07
-  1720      7.25466e-07      1.28875e-07
-  1725      3.23125e-07      8.84504e-08
-  1730      8.08160e-08      4.72522e-08
-  1735      0.00000e+00      0.00000e+00
+---------------------------------------------------------------------------------------------
+
+BetaShape
+Version: 2.2 (05/2021)
+Author: X. Mougeot (xavier.mougeot@cea.fr)
+CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
+Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
+
+---------------------------------------------------------------------------------------------
+
+Total beta + spectrum from the F-18 decay. See file of each transition for more details.
+
+Mean energy from the total beta + spectrum: 250.50 (21) keV
+
+E(keV)      dNtot/dE b+      unc.
+     0      0.00000e+00      0.00000e+00
+     2      3.21027e-05      5.04587e-08
+     4      1.11844e-04      1.75233e-07
+     6      1.98735e-04      3.10362e-07
+     8      2.83660e-04      4.41541e-07
+    10      3.64714e-04      5.65836e-07
+    12      4.41671e-04      6.82948e-07
+    14      5.14749e-04      7.93272e-07
+    16      5.84277e-04      8.97361e-07
+    18      6.50581e-04      9.95767e-07
+    20      7.13962e-04      1.08899e-06
+    22      7.74686e-04      1.17748e-06
+    24      8.32982e-04      1.26161e-06
+    26      8.89052e-04      1.34173e-06
+    28      9.43070e-04      1.41812e-06
+    30      9.95188e-04      1.49103e-06
+    32      1.04554e-03      1.56071e-06
+    34      1.09424e-03      1.62733e-06
+    36      1.14140e-03      1.69108e-06
+    38      1.18710e-03      1.75212e-06
+    40      1.23144e-03      1.81058e-06
+    42      1.27447e-03      1.86659e-06
+    44      1.31628e-03      1.92026e-06
+    46      1.35692e-03      1.97170e-06
+    48      1.39644e-03      2.02101e-06
+    50      1.43490e-03      2.06825e-06
+    52      1.47233e-03      2.11353e-06
+    54      1.50879e-03      2.15690e-06
+    56      1.54431e-03      2.19843e-06
+    58      1.57892e-03      2.23819e-06
+    60      1.61265e-03      2.27623e-06
+    62      1.64554e-03      2.31261e-06
+    64      1.67762e-03      2.34737e-06
+    66      1.70890e-03      2.38056e-06
+    68      1.73942e-03      2.41222e-06
+    70      1.76920e-03      2.44240e-06
+    72      1.79825e-03      2.47113e-06
+    74      1.82660e-03      2.49845e-06
+    76      1.85426e-03      2.52438e-06
+    78      1.88125e-03      2.54897e-06
+    80      1.90759e-03      2.57224e-06
+    82      1.93329e-03      2.59423e-06
+    84      1.95838e-03      2.61495e-06
+    86      1.98285e-03      2.63443e-06
+    88      2.00672e-03      2.65271e-06
+    90      2.03002e-03      2.66979e-06
+    92      2.05274e-03      2.68571e-06
+    94      2.07489e-03      2.70049e-06
+    96      2.09650e-03      2.71414e-06
+    98      2.11757e-03      2.72669e-06
+   100      2.13810e-03      2.73815e-06
+   102      2.15811e-03      2.74854e-06
+   104      2.17761e-03      2.75789e-06
+   106      2.19660e-03      2.76620e-06
+   108      2.21510e-03      2.77350e-06
+   110      2.23310e-03      2.77980e-06
+   112      2.25062e-03      2.78511e-06
+   114      2.26767e-03      2.78945e-06
+   116      2.28424e-03      2.79283e-06
+   118      2.30036e-03      2.79528e-06
+   120      2.31601e-03      2.79679e-06
+   122      2.33122e-03      2.79739e-06
+   124      2.34598e-03      2.79709e-06
+   126      2.36030e-03      2.79589e-06
+   128      2.37418e-03      2.79382e-06
+   130      2.38764e-03      2.79089e-06
+   132      2.40067e-03      2.78710e-06
+   134      2.41329e-03      2.78246e-06
+   136      2.42549e-03      2.77700e-06
+   138      2.43728e-03      2.77071e-06
+   140      2.44866e-03      2.76362e-06
+   142      2.45965e-03      2.75572e-06
+   144      2.47024e-03      2.74704e-06
+   146      2.48043e-03      2.73758e-06
+   148      2.49024e-03      2.72735e-06
+   150      2.49966e-03      2.71636e-06
+   152      2.50870e-03      2.70462e-06
+   154      2.51736e-03      2.69214e-06
+   156      2.52565e-03      2.67894e-06
+   158      2.53357e-03      2.66501e-06
+   160      2.54112e-03      2.65037e-06
+   162      2.54831e-03      2.63503e-06
+   164      2.55514e-03      2.61900e-06
+   166      2.56162e-03      2.60229e-06
+   168      2.56774e-03      2.58490e-06
+   170      2.57351e-03      2.56684e-06
+   172      2.57893e-03      2.54813e-06
+   174      2.58401e-03      2.52876e-06
+   176      2.58874e-03      2.50876e-06
+   178      2.59314e-03      2.48813e-06
+   180      2.59720e-03      2.46688e-06
+   182      2.60093e-03      2.44501e-06
+   184      2.60433e-03      2.42253e-06
+   186      2.60741e-03      2.39946e-06
+   188      2.61016e-03      2.37580e-06
+   190      2.61258e-03      2.35155e-06
+   192      2.61469e-03      2.32674e-06
+   194      2.61649e-03      2.30136e-06
+   196      2.61797e-03      2.27543e-06
+   198      2.61913e-03      2.24894e-06
+   200      2.61999e-03      2.22192e-06
+   202      2.62055e-03      2.19437e-06
+   204      2.62080e-03      2.16629e-06
+   206      2.62075e-03      2.13770e-06
+   208      2.62040e-03      2.10860e-06
+   210      2.61975e-03      2.07900e-06
+   212      2.61882e-03      2.04892e-06
+   214      2.61759e-03      2.01834e-06
+   216      2.61607e-03      1.98730e-06
+   218      2.61426e-03      1.95579e-06
+   220      2.61218e-03      1.92382e-06
+   222      2.60981e-03      1.89140e-06
+   224      2.60716e-03      1.85853e-06
+   226      2.60423e-03      1.82524e-06
+   228      2.60103e-03      1.79151e-06
+   230      2.59756e-03      1.75737e-06
+   232      2.59382e-03      1.72282e-06
+   234      2.58981e-03      1.68787e-06
+   236      2.58554e-03      1.65265e-06
+   238      2.58100e-03      1.61704e-06
+   240      2.57620e-03      1.58106e-06
+   242      2.57115e-03      1.54471e-06
+   244      2.56584e-03      1.50800e-06
+   246      2.56027e-03      1.47093e-06
+   248      2.55445e-03      1.43353e-06
+   250      2.54839e-03      1.39578e-06
+   252      2.54208e-03      1.35771e-06
+   254      2.53552e-03      1.31932e-06
+   256      2.52872e-03      1.28062e-06
+   258      2.52168e-03      1.24162e-06
+   260      2.51441e-03      1.20232e-06
+   262      2.50690e-03      1.16274e-06
+   264      2.49915e-03      1.12288e-06
+   266      2.49118e-03      1.08275e-06
+   268      2.48297e-03      1.04236e-06
+   270      2.47455e-03      1.00172e-06
+   272      2.46589e-03      9.60832e-07
+   274      2.45702e-03      9.19712e-07
+   276      2.44792e-03      8.78366e-07
+   278      2.43861e-03      8.36803e-07
+   280      2.42909e-03      7.95030e-07
+   282      2.41935e-03      7.53057e-07
+   284      2.40941e-03      7.10893e-07
+   286      2.39925e-03      6.68545e-07
+   288      2.38889e-03      6.26024e-07
+   290      2.37833e-03      5.83337e-07
+   292      2.36757e-03      5.40494e-07
+   294      2.35661e-03      4.97503e-07
+   296      2.34545e-03      4.54373e-07
+   298      2.33411e-03      4.11114e-07
+   300      2.32257e-03      3.67733e-07
+   302      2.31084e-03      3.24241e-07
+   304      2.29892e-03      2.80647e-07
+   306      2.28682e-03      2.36958e-07
+   308      2.27454e-03      1.93185e-07
+   310      2.26209e-03      1.49337e-07
+   312      2.24945e-03      1.05423e-07
+   314      2.23664e-03      6.14516e-08
+   316      2.22366e-03      1.74327e-08
+   318      2.21051e-03      3.17306e-08
+   320      2.19720e-03      7.59246e-08
+   322      2.18372e-03      1.20137e-07
+   324      2.17008e-03      1.64358e-07
+   326      2.15628e-03      2.08579e-07
+   328      2.14232e-03      2.52789e-07
+   330      2.12821e-03      2.96979e-07
+   332      2.11395e-03      3.41140e-07
+   334      2.09954e-03      3.85262e-07
+   336      2.08498e-03      4.29335e-07
+   338      2.07028e-03      4.73349e-07
+   340      2.05544e-03      5.17295e-07
+   342      2.04045e-03      5.61162e-07
+   344      2.02534e-03      6.04941e-07
+   346      2.01009e-03      6.48622e-07
+   348      1.99470e-03      6.92195e-07
+   350      1.97919e-03      7.35649e-07
+   352      1.96356e-03      7.78975e-07
+   354      1.94780e-03      8.22163e-07
+   356      1.93192e-03      8.65202e-07
+   358      1.91593e-03      9.08083e-07
+   360      1.89982e-03      9.50794e-07
+   362      1.88359e-03      9.93326e-07
+   364      1.86726e-03      1.03567e-06
+   366      1.85082e-03      1.07781e-06
+   368      1.83428e-03      1.11974e-06
+   370      1.81763e-03      1.16145e-06
+   372      1.80089e-03      1.20293e-06
+   374      1.78405e-03      1.24417e-06
+   376      1.76712e-03      1.28516e-06
+   378      1.75010e-03      1.32588e-06
+   380      1.73299e-03      1.36632e-06
+   382      1.71580e-03      1.40649e-06
+   384      1.69853e-03      1.44635e-06
+   386      1.68117e-03      1.48591e-06
+   388      1.66375e-03      1.52516e-06
+   390      1.64624e-03      1.56407e-06
+   392      1.62867e-03      1.60265e-06
+   394      1.61103e-03      1.64087e-06
+   396      1.59333e-03      1.67874e-06
+   398      1.57557e-03      1.71623e-06
+   400      1.55775e-03      1.75334e-06
+   402      1.53987e-03      1.79005e-06
+   404      1.52194e-03      1.82636e-06
+   406      1.50396e-03      1.86225e-06
+   408      1.48593e-03      1.89771e-06
+   410      1.46786e-03      1.93273e-06
+   412      1.44976e-03      1.96730e-06
+   414      1.43161e-03      2.00140e-06
+   416      1.41343e-03      2.03503e-06
+   418      1.39522e-03      2.06818e-06
+   420      1.37698e-03      2.10083e-06
+   422      1.35871e-03      2.13296e-06
+   424      1.34043e-03      2.16458e-06
+   426      1.32212e-03      2.19566e-06
+   428      1.30380e-03      2.22620e-06
+   430      1.28547e-03      2.25618e-06
+   432      1.26713e-03      2.28559e-06
+   434      1.24878e-03      2.31442e-06
+   436      1.23043e-03      2.34265e-06
+   438      1.21208e-03      2.37029e-06
+   440      1.19374e-03      2.39730e-06
+   442      1.17540e-03      2.42368e-06
+   444      1.15707e-03      2.44943e-06
+   446      1.13876e-03      2.47452e-06
+   448      1.12046e-03      2.49894e-06
+   450      1.10218e-03      2.52269e-06
+   452      1.08393e-03      2.54574e-06
+   454      1.06570e-03      2.56809e-06
+   456      1.04751e-03      2.58972e-06
+   458      1.02934e-03      2.61063e-06
+   460      1.01122e-03      2.63079e-06
+   462      9.93130e-04      2.65020e-06
+   464      9.75088e-04      2.66884e-06
+   466      9.57093e-04      2.68671e-06
+   468      9.39149e-04      2.70378e-06
+   470      9.21259e-04      2.72004e-06
+   472      9.03426e-04      2.73549e-06
+   474      8.85655e-04      2.75010e-06
+   476      8.67949e-04      2.76388e-06
+   478      8.50310e-04      2.77679e-06
+   480      8.32743e-04      2.78883e-06
+   482      8.15252e-04      2.79999e-06
+   484      7.97839e-04      2.81026e-06
+   486      7.80509e-04      2.81961e-06
+   488      7.63265e-04      2.82804e-06
+   490      7.46110e-04      2.83553e-06
+   492      7.29049e-04      2.84207e-06
+   494      7.12084e-04      2.84765e-06
+   496      6.95220e-04      2.85225e-06
+   498      6.78461e-04      2.85586e-06
+   500      6.61809e-04      2.85847e-06
+   502      6.45269e-04      2.86005e-06
+   504      6.28844e-04      2.86061e-06
+   506      6.12539e-04      2.86012e-06
+   508      5.96356e-04      2.85857e-06
+   510      5.80300e-04      2.85594e-06
+   512      5.64374e-04      2.85223e-06
+   514      5.48583e-04      2.84741e-06
+   516      5.32929e-04      2.84149e-06
+   518      5.17418e-04      2.83443e-06
+   520      5.02052e-04      2.82622e-06
+   522      4.86836e-04      2.81686e-06
+   524      4.71773e-04      2.80633e-06
+   526      4.56868e-04      2.79461e-06
+   528      4.42124e-04      2.78169e-06
+   530      4.27545e-04      2.76755e-06
+   532      4.13135e-04      2.75218e-06
+   534      3.98899e-04      2.73557e-06
+   536      3.84840e-04      2.71786e-06
+   538      3.70961e-04      2.69903e-06
+   540      3.57268e-04      2.67891e-06
+   542      3.43764e-04      2.65751e-06
+   544      3.30453e-04      2.63479e-06
+   546      3.17339e-04      2.61074e-06
+   548      3.04427e-04      2.58536e-06
+   550      2.91720e-04      2.55862e-06
+   552      2.79222e-04      2.53051e-06
+   554      2.66938e-04      2.50101e-06
+   556      2.54872e-04      2.47011e-06
+   558      2.43027e-04      2.43780e-06
+   560      2.31409e-04      2.40406e-06
+   562      2.20021e-04      2.36888e-06
+   564      2.08867e-04      2.33223e-06
+   566      1.97952e-04      2.29411e-06
+   568      1.87280e-04      2.25450e-06
+   570      1.76855e-04      2.21338e-06
+   572      1.66681e-04      2.17073e-06
+   574      1.56764e-04      2.12656e-06
+   576      1.47106e-04      2.08082e-06
+   578      1.37712e-04      2.03352e-06
+   580      1.28587e-04      1.98464e-06
+   582      1.19735e-04      1.93415e-06
+   584      1.11160e-04      1.88205e-06
+   586      1.02867e-04      1.82832e-06
+   588      9.48596e-05      1.77294e-06
+   590      8.71430e-05      1.71590e-06
+   592      7.97213e-05      1.65718e-06
+   594      7.25990e-05      1.59676e-06
+   596      6.57806e-05      1.53464e-06
+   598      5.92703e-05      1.47078e-06
+   600      5.30729e-05      1.40519e-06
+   602      4.71928e-05      1.33783e-06
+   604      4.16344e-05      1.26870e-06
+   606      3.64024e-05      1.19777e-06
+   608      3.15013e-05      1.12504e-06
+   610      2.69357e-05      1.05048e-06
+   612      2.27101e-05      9.74082e-07
+   614      1.88292e-05      8.95825e-07
+   616      1.52975e-05      8.15693e-07
+   618      1.21198e-05      7.33671e-07
+   620      9.30062e-06      6.49741e-07
+   622      6.84469e-06      5.63886e-07
+   624      4.75667e-06      4.76091e-07
+   626      3.04128e-06      3.86337e-07
+   628      1.70322e-06      2.94608e-07
+   630      7.47233e-07      2.00888e-07
+   632      1.78070e-07      1.05159e-07
+ 633.9      0.00000e+00      0.00000e+00
```

### Comparing `opengate-10.0b7/opengate/sources/beta_plus_spectra/Rb82/beta+_Rb82_tot.bs` & `opengate-10.0b8/opengate/sources/beta_plus_spectra/Ga68/beta+_Ga68_tot.bs`

 * *Files 20% similar despite different names*

```diff
@@ -1,373 +1,419 @@
----------------------------------------------------------------------------------------------
-
-BetaShape
-Version: 2.2 (05/2021)
-Author: X. Mougeot (xavier.mougeot@cea.fr)
-CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
-Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
-
----------------------------------------------------------------------------------------------
-
-Total beta + spectrum from the Rb-82 decay. See file of each transition for more details.
-
-Mean energy from the total beta + spectrum: 1473.0 (44) keV
-
-E(keV)      dNtot/dE b+      unc.
-     0      0.00000e+00      0.00000e+00
-     2      2.45580e-10      1.00034e-14
-     4      3.69889e-08      7.91242e-11
-     6      1.55129e-07      3.43312e-10
-     8      3.39884e-07      7.57271e-10
-    10      5.92074e-07      1.32099e-09
-    12      9.11450e-07      2.03448e-09
-    14      1.29802e-06      2.89773e-09
-    16      1.75173e-06      3.91075e-09
-    18      2.27030e-06      5.07283e-09
-    20      2.85477e-06      6.38440e-09
-    22      3.50471e-06      7.84545e-09
-    24      4.18416e-06      9.34821e-09
-    26      4.90816e-06      1.09638e-08
-    28      5.68249e-06      1.26944e-08
-    30      6.50671e-06      1.45399e-08
-    32      7.38076e-06      1.65004e-08
-    34      8.27548e-06      1.85103e-08
-    36      9.18513e-06      2.05402e-08
-    38      1.01268e-05      2.26422e-08
-    40      1.11007e-05      2.48163e-08
-    42      1.21009e-05      2.70604e-08
-    44      1.31307e-05      2.93757e-08
-    46      1.41608e-05      3.16753e-08
-    48      1.52113e-05      3.40193e-08
-    50      1.62783e-05      3.64064e-08
-    52      1.73640e-05      3.88374e-08
-    54      1.84684e-05      4.13124e-08
-    56      1.95833e-05      4.38069e-08
-    58      2.07018e-05      4.63079e-08
-    60      2.18323e-05      4.88363e-08
-    62      2.29748e-05      5.13920e-08
-    64      2.41291e-05      5.39750e-08
-    66      2.52935e-05      5.65846e-08
-    68      2.64581e-05      5.91891e-08
-    70      2.76305e-05      6.18107e-08
-    72      2.88105e-05      6.44495e-08
-    74      2.99969e-05      6.71049e-08
-    76      3.11904e-05      6.97773e-08
-    78      3.23878e-05      7.24572e-08
-    80      3.35876e-05      7.51401e-08
-    82      3.47914e-05      7.78334e-08
-    84      3.59998e-05      8.05373e-08
-    86      3.72126e-05      8.32517e-08
-    88      3.84300e-05      8.59767e-08
-    90      3.96469e-05      8.86990e-08
-    92      4.08665e-05      9.14278e-08
-    94      4.20891e-05      9.41631e-08
-    96      4.33145e-05      9.69048e-08
-    98      4.45422e-05      9.96528e-08
-   100      4.57712e-05      1.02403e-07
-   110      5.19344e-05      1.16195e-07
-   120      5.81180e-05      1.30031e-07
-   130      6.43096e-05      1.43886e-07
-   140      7.04999e-05      1.57737e-07
-   150      7.66819e-05      1.71570e-07
-   160      8.28505e-05      1.85372e-07
-   170      8.90019e-05      1.99136e-07
-   180      9.51334e-05      2.12854e-07
-   190      1.01243e-04      2.26522e-07
-   200      1.07328e-04      2.40134e-07
-   210      1.13388e-04      2.53689e-07
-   220      1.19421e-04      2.67183e-07
-   230      1.25427e-04      2.80614e-07
-   240      1.31404e-04      2.93980e-07
-   250      1.37352e-04      3.07278e-07
-   260      1.43271e-04      3.20509e-07
-   270      1.49159e-04      3.33670e-07
-   280      1.55015e-04      3.46758e-07
-   290      1.60841e-04      3.59775e-07
-   300      1.66634e-04      3.72715e-07
-   310      1.72394e-04      3.85580e-07
-   320      1.78122e-04      3.98368e-07
-   330      1.83816e-04      4.11079e-07
-   340      1.89475e-04      4.23708e-07
-   350      1.95099e-04      4.36256e-07
-   360      2.00687e-04      4.48720e-07
-   370      2.06239e-04      4.61099e-07
-   380      2.11754e-04      4.73393e-07
-   390      2.17233e-04      4.85601e-07
-   400      2.22674e-04      4.97718e-07
-   410      2.28076e-04      5.09746e-07
-   420      2.33439e-04      5.21683e-07
-   430      2.38763e-04      5.33526e-07
-   440      2.44046e-04      5.45273e-07
-   450      2.49289e-04      5.56925e-07
-   460      2.54491e-04      5.68479e-07
-   470      2.59650e-04      5.79934e-07
-   480      2.64768e-04      5.91290e-07
-   490      2.69843e-04      6.02544e-07
-   500      2.74874e-04      6.13694e-07
-   510      2.79861e-04      6.24739e-07
-   520      2.84804e-04      6.35678e-07
-   530      2.89701e-04      6.46508e-07
-   540      2.94553e-04      6.57233e-07
-   550      2.99359e-04      6.67844e-07
-   560      3.04118e-04      6.78344e-07
-   570      3.08830e-04      6.88732e-07
-   580      3.13494e-04      6.99006e-07
-   590      3.18110e-04      7.09164e-07
-   600      3.22678e-04      7.19206e-07
-   610      3.27197e-04      7.29129e-07
-   620      3.31665e-04      7.38931e-07
-   630      3.36085e-04      7.48616e-07
-   640      3.40453e-04      7.58177e-07
-   650      3.44771e-04      7.67616e-07
-   660      3.49037e-04      7.76930e-07
-   670      3.53252e-04      7.86120e-07
-   680      3.57415e-04      7.95183e-07
-   690      3.61525e-04      8.04119e-07
-   700      3.65583e-04      8.12928e-07
-   710      3.69588e-04      8.21607e-07
-   720      3.73539e-04      8.30155e-07
-   730      3.77436e-04      8.38571e-07
-   740      3.81279e-04      8.46856e-07
-   750      3.85067e-04      8.55007e-07
-   760      3.88800e-04      8.63026e-07
-   770      3.92478e-04      8.70908e-07
-   780      3.96100e-04      8.78655e-07
-   790      3.99667e-04      8.86266e-07
-   800      4.03178e-04      8.93740e-07
-   810      4.06632e-04      9.01076e-07
-   820      4.10030e-04      9.08273e-07
-   830      4.13371e-04      9.15331e-07
-   840      4.16654e-04      9.22248e-07
-   850      4.19881e-04      9.29025e-07
-   860      4.23050e-04      9.35661e-07
-   870      4.26162e-04      9.42156e-07
-   880      4.29215e-04      9.48508e-07
-   890      4.32211e-04      9.54716e-07
-   900      4.35150e-04      9.60783e-07
-   910      4.38030e-04      9.66706e-07
-   920      4.40849e-04      9.72484e-07
-   930      4.43610e-04      9.78118e-07
-   940      4.46311e-04      9.83608e-07
-   950      4.48951e-04      9.88952e-07
-   960      4.51531e-04      9.94151e-07
-   970      4.54050e-04      9.99205e-07
-   980      4.56510e-04      1.00411e-06
-   990      4.58909e-04      1.00888e-06
-  1000      4.61246e-04      1.01349e-06
-  1011      4.63748e-04      1.01840e-06
-  1022      4.66177e-04      1.02313e-06
-  1033      4.68531e-04      1.02769e-06
-  1044      4.70813e-04      1.03207e-06
-  1055      4.73021e-04      1.03627e-06
-  1066      4.75155e-04      1.04029e-06
-  1077      4.77216e-04      1.04414e-06
-  1088      4.79204e-04      1.04781e-06
-  1099      4.81118e-04      1.05131e-06
-  1110      4.82959e-04      1.05462e-06
-  1121      4.84727e-04      1.05777e-06
-  1132      4.86422e-04      1.06074e-06
-  1143      4.88045e-04      1.06353e-06
-  1154      4.89595e-04      1.06615e-06
-  1165      4.91072e-04      1.06860e-06
-  1176      4.92478e-04      1.07087e-06
-  1187      4.93811e-04      1.07297e-06
-  1198      4.95073e-04      1.07490e-06
-  1209      4.96263e-04      1.07666e-06
-  1220      4.97379e-04      1.07824e-06
-  1231      4.98415e-04      1.07966e-06
-  1242      4.99373e-04      1.08091e-06
-  1253      5.00253e-04      1.08199e-06
-  1264      5.01054e-04      1.08291e-06
-  1275      5.01776e-04      1.08366e-06
-  1286      5.02421e-04      1.08424e-06
-  1297      5.02987e-04      1.08467e-06
-  1308      5.03475e-04      1.08493e-06
-  1319      5.03885e-04      1.08503e-06
-  1330      5.04217e-04      1.08497e-06
-  1341      5.04471e-04      1.08475e-06
-  1352      5.04648e-04      1.08438e-06
-  1363      5.04747e-04      1.08385e-06
-  1374      5.04770e-04      1.08318e-06
-  1385      5.04715e-04      1.08235e-06
-  1396      5.04584e-04      1.08138e-06
-  1407      5.04376e-04      1.08025e-06
-  1418      5.04093e-04      1.07898e-06
-  1429      5.03734e-04      1.07757e-06
-  1440      5.03298e-04      1.07601e-06
-  1451      5.02789e-04      1.07431e-06
-  1462      5.02203e-04      1.07247e-06
-  1473      5.01543e-04      1.07049e-06
-  1484      5.00810e-04      1.06838e-06
-  1495      5.00001e-04      1.06613e-06
-  1506      4.99120e-04      1.06376e-06
-  1517      4.98165e-04      1.06125e-06
-  1528      4.97139e-04      1.05862e-06
-  1539      4.96040e-04      1.05587e-06
-  1550      4.94868e-04      1.05299e-06
-  1561      4.93626e-04      1.04999e-06
-  1572      4.92314e-04      1.04688e-06
-  1583      4.90931e-04      1.04366e-06
-  1594      4.89477e-04      1.04032e-06
-  1605      4.87955e-04      1.03687e-06
-  1616      4.86365e-04      1.03332e-06
-  1627      4.84706e-04      1.02966e-06
-  1638      4.82980e-04      1.02590e-06
-  1649      4.81187e-04      1.02205e-06
-  1660      4.79328e-04      1.01810e-06
-  1671      4.77403e-04      1.01406e-06
-  1682      4.75414e-04      1.00994e-06
-  1693      4.73359e-04      1.00572e-06
-  1704      4.71242e-04      1.00143e-06
-  1715      4.69061e-04      9.97052e-07
-  1726      4.66818e-04      9.92603e-07
-  1737      4.64514e-04      9.88080e-07
-  1748      4.62149e-04      9.83488e-07
-  1759      4.59724e-04      9.78832e-07
-  1770      4.57239e-04      9.74113e-07
-  1781      4.54697e-04      9.69336e-07
-  1792      4.52097e-04      9.64505e-07
-  1803      4.49439e-04      9.59621e-07
-  1814      4.46726e-04      9.54689e-07
-  1825      4.43958e-04      9.49713e-07
-  1836      4.41135e-04      9.44697e-07
-  1847      4.38259e-04      9.39644e-07
-  1858      4.35330e-04      9.34557e-07
-  1869      4.32350e-04      9.29442e-07
-  1880      4.29320e-04      9.24301e-07
-  1891      4.26239e-04      9.19145e-07
-  1902      4.23110e-04      9.13987e-07
-  1913      4.19933e-04      9.08810e-07
-  1924      4.16707e-04      9.03623e-07
-  1935      4.13434e-04      8.98430e-07
-  1946      4.10116e-04      8.93237e-07
-  1957      4.06752e-04      8.88046e-07
-  1968      4.03344e-04      8.82859e-07
-  1979      3.99893e-04      8.77684e-07
-  1990      3.96400e-04      8.72521e-07
-  2001      3.92867e-04      8.67377e-07
-  2012      3.89293e-04      8.62254e-07
-  2023      3.85681e-04      8.57157e-07
-  2034      3.82031e-04      8.52087e-07
-  2045      3.78345e-04      8.47050e-07
-  2056      3.74623e-04      8.42049e-07
-  2067      3.70867e-04      8.37087e-07
-  2078      3.67077e-04      8.32167e-07
-  2089      3.63255e-04      8.27293e-07
-  2100      3.59404e-04      8.22471e-07
-  2111      3.55522e-04      8.17697e-07
-  2122      3.51612e-04      8.12982e-07
-  2133      3.47675e-04      8.08324e-07
-  2144      3.43713e-04      8.03728e-07
-  2155      3.39726e-04      7.99195e-07
-  2166      3.35715e-04      7.94728e-07
-  2177      3.31682e-04      7.90329e-07
-  2188      3.27629e-04      7.86001e-07
-  2199      3.23557e-04      7.81748e-07
-  2210      3.19466e-04      7.77568e-07
-  2221      3.15359e-04      7.73465e-07
-  2232      3.11237e-04      7.69439e-07
-  2243      3.07100e-04      7.65493e-07
-  2254      3.02951e-04      7.61627e-07
-  2265      2.98791e-04      7.57841e-07
-  2276      2.94621e-04      7.54138e-07
-  2287      2.90444e-04      7.50518e-07
-  2298      2.86259e-04      7.46979e-07
-  2309      2.82068e-04      7.43521e-07
-  2320      2.77875e-04      7.40147e-07
-  2331      2.73678e-04      7.36853e-07
-  2342      2.69482e-04      7.33640e-07
-  2353      2.65285e-04      7.30506e-07
-  2364      2.61091e-04      7.27450e-07
-  2375      2.56901e-04      7.24470e-07
-  2386      2.52716e-04      7.21565e-07
-  2397      2.48538e-04      7.18732e-07
-  2408      2.44368e-04      7.15969e-07
-  2419      2.40209e-04      7.13272e-07
-  2430      2.36061e-04      7.10641e-07
-  2441      2.31927e-04      7.08070e-07
-  2452      2.27808e-04      7.05557e-07
-  2463      2.23705e-04      7.03098e-07
-  2474      2.19621e-04      7.00689e-07
-  2485      2.15556e-04      6.98325e-07
-  2496      2.11514e-04      6.96003e-07
-  2507      2.07495e-04      6.93718e-07
-  2518      2.03502e-04      6.91465e-07
-  2529      1.99534e-04      6.89238e-07
-  2540      1.95597e-04      6.87033e-07
-  2551      1.91688e-04      6.84843e-07
-  2562      1.87813e-04      6.82665e-07
-  2573      1.83971e-04      6.80492e-07
-  2584      1.80165e-04      6.78316e-07
-  2595      1.76396e-04      6.76134e-07
-  2606      1.72666e-04      6.73937e-07
-  2617      1.68954e-04      6.71719e-07
-  2628      1.65249e-04      6.69471e-07
-  2639      1.61552e-04      6.67187e-07
-  2650      1.57863e-04      6.64858e-07
-  2661      1.54185e-04      6.62479e-07
-  2672      1.50518e-04      6.60042e-07
-  2683      1.46864e-04      6.57540e-07
-  2694      1.43223e-04      6.54964e-07
-  2705      1.39598e-04      6.52307e-07
-  2716      1.35988e-04      6.49561e-07
-  2727      1.32396e-04      6.46718e-07
-  2738      1.28822e-04      6.43770e-07
-  2749      1.25268e-04      6.40710e-07
-  2760      1.21735e-04      6.37529e-07
-  2771      1.18225e-04      6.34218e-07
-  2782      1.14738e-04      6.30770e-07
-  2793      1.11276e-04      6.27178e-07
-  2804      1.07840e-04      6.23430e-07
-  2815      1.04431e-04      6.19520e-07
-  2826      1.01052e-04      6.15439e-07
-  2837      9.77021e-05      6.11179e-07
-  2848      9.43837e-05      6.06732e-07
-  2859      9.10981e-05      6.02087e-07
-  2870      8.78464e-05      5.97239e-07
-  2881      8.46302e-05      5.92177e-07
-  2892      8.14506e-05      5.86892e-07
-  2903      7.83093e-05      5.81377e-07
-  2914      7.52073e-05      5.75624e-07
-  2925      7.21462e-05      5.69680e-07
-  2936      6.91274e-05      5.63515e-07
-  2947      6.61523e-05      5.57089e-07
-  2958      6.32221e-05      5.50393e-07
-  2969      6.03385e-05      5.43417e-07
-  2980      5.75029e-05      5.36154e-07
-  2991      5.47165e-05      5.28595e-07
-  3002      5.19810e-05      5.20731e-07
-  3013      4.92976e-05      5.12553e-07
-  3024      4.66681e-05      5.04054e-07
-  3035      4.40937e-05      4.95225e-07
-  3046      4.15759e-05      4.86057e-07
-  3057      3.91163e-05      4.76542e-07
-  3068      3.67163e-05      4.66672e-07
-  3079      3.43775e-05      4.56437e-07
-  3090      3.21013e-05      4.45829e-07
-  3101      2.98892e-05      4.34841e-07
-  3112      2.77428e-05      4.23464e-07
-  3123      2.56638e-05      4.11689e-07
-  3134      2.36534e-05      3.99509e-07
-  3145      2.17134e-05      3.86914e-07
-  3156      1.98452e-05      3.73897e-07
-  3167      1.80505e-05      3.60450e-07
-  3178      1.63307e-05      3.46564e-07
-  3189      1.46876e-05      3.32232e-07
-  3200      1.31225e-05      3.17446e-07
-  3211      1.16372e-05      3.02197e-07
-  3222      1.02333e-05      2.86478e-07
-  3233      8.91221e-06      2.70282e-07
-  3244      7.67569e-06      2.53600e-07
-  3255      6.52529e-06      2.36427e-07
-  3266      5.46261e-06      2.18754e-07
-  3277      4.48927e-06      2.00576e-07
-  3288      3.60687e-06      1.81884e-07
-  3299      2.81700e-06      1.62675e-07
-  3310      2.12128e-06      1.42943e-07
-  3321      1.52127e-06      1.22684e-07
-  3332      1.01856e-06      1.01894e-07
-  3343      6.14692e-07      8.05752e-08
-  3354      3.11165e-07      5.87324e-08
-  3365      1.09408e-07      3.63814e-08
-  3376      1.06554e-08      1.35753e-08
-  3381      0.00000e+00      0.00000e+00
+---------------------------------------------------------------------------------------------
+
+BetaShape
+Version: 2.2 (05/2021)
+Author: X. Mougeot (xavier.mougeot@cea.fr)
+CEA, LIST, Laboratoire National Henri Becquerel (LNHB), Gif-sur-Yvette F-91191, France
+Please cite: X. Mougeot, Physical Review C 91, 055504; Erratum Phys. Rev. C 92, 059902 (2015)
+
+---------------------------------------------------------------------------------------------
+
+Total beta + spectrum from the Ga-68 decay. See file of each transition for more details.
+
+Mean energy from the total beta + spectrum: 828.4 (35) keV
+
+E(keV)      dNtot/dE b+      unc.
+    0.0     0.00000e+00      0.00000e+00
+    0.8     5.69351e-10      2.27043e-13
+    1.6     4.69159e-09      1.87897e-12
+    2.4     1.23698e-08      4.95578e-12
+    3.2     2.36060e-08      9.45747e-12
+    4.0     3.84019e-08      1.53840e-11
+    4.8     5.88157e-08      2.35624e-11
+    5.6     1.78367e-07      4.08053e-10
+    6.4     3.58515e-07      1.05366e-09
+    7.2     5.78006e-07      1.84663e-09
+    8.0     8.36680e-07      2.78666e-09
+    8.8     1.13426e-06      3.87371e-09
+    9.6     1.47086e-06      5.10777e-09
+    10      1.65380e-06      5.77992e-09
+    11      2.15291e-06      7.62107e-09
+    12      2.71240e-06      9.69190e-09
+    13      3.41881e-06      1.23690e-08
+    14      4.20989e-06      1.53834e-08
+    15      5.08452e-06      1.87351e-08
+    16      6.04308e-06      2.24241e-08
+    17      7.08448e-06      2.64504e-08
+    18      8.20909e-06      3.08139e-08
+    19      9.35861e-06      3.52672e-08
+    20      1.05743e-05      3.99871e-08
+    21      1.18553e-05      4.49736e-08
+    22      1.32019e-05      5.02266e-08
+    23      1.46133e-05      5.57462e-08
+    24      1.60897e-05      6.15323e-08
+    25      1.75639e-05      6.72978e-08
+    26      1.90837e-05      7.32477e-08
+    27      2.06484e-05      7.93820e-08
+    28      2.22584e-05      8.57009e-08
+    29      2.39129e-05      9.22042e-08
+    30      2.56123e-05      9.88920e-08
+    31      2.73067e-05      1.05552e-07
+    32      2.90315e-05      1.12335e-07
+    33      3.07864e-05      1.19242e-07
+    34      3.25714e-05      1.26273e-07
+    35      3.43862e-05      1.33428e-07
+    36      3.62309e-05      1.40706e-07
+    37      3.80714e-05      1.47962e-07
+    38      3.99321e-05      1.55301e-07
+    39      4.18125e-05      1.62722e-07
+    40      4.37127e-05      1.70224e-07
+    41      4.56327e-05      1.77809e-07
+    42      4.75723e-05      1.85477e-07
+    43      4.95086e-05      1.93127e-07
+    44      5.14579e-05      2.00832e-07
+    45      5.34201e-05      2.08590e-07
+    46      5.53952e-05      2.16403e-07
+    47      5.73831e-05      2.24269e-07
+    48      5.93837e-05      2.32189e-07
+    49      6.13814e-05      2.40096e-07
+    50      6.33873e-05      2.48037e-07
+    51      6.54013e-05      2.56014e-07
+    52      6.74235e-05      2.64024e-07
+    53      6.94538e-05      2.72070e-07
+    54      7.14921e-05      2.80150e-07
+    55      7.35276e-05      2.88218e-07
+    56      7.55679e-05      2.96307e-07
+    57      7.76131e-05      3.04418e-07
+    58      7.96632e-05      3.12550e-07
+    59      8.17180e-05      3.20703e-07
+    60      8.37777e-05      3.28877e-07
+    61      8.58345e-05      3.37040e-07
+    62      8.78938e-05      3.45215e-07
+    63      8.99557e-05      3.53402e-07
+    64      9.20201e-05      3.61601e-07
+    65      9.40870e-05      3.69812e-07
+    66      9.61563e-05      3.78034e-07
+    67      9.82228e-05      3.86245e-07
+    68      1.00290e-04      3.94462e-07
+    69      1.02358e-04      4.02683e-07
+    70      1.04427e-04      4.10910e-07
+    71      1.06497e-04      4.19142e-07
+    72      1.08568e-04      4.27380e-07
+    73      1.10636e-04      4.35605e-07
+    74      1.12703e-04      4.43831e-07
+    75      1.14770e-04      4.52058e-07
+    76      1.16837e-04      4.60285e-07
+    77      1.18904e-04      4.68512e-07
+    78      1.20970e-04      4.76740e-07
+    79      1.23033e-04      4.84956e-07
+    80      1.25095e-04      4.93169e-07
+    81      1.27156e-04      5.01380e-07
+    82      1.29215e-04      5.09587e-07
+    83      1.31274e-04      5.17792e-07
+    84      1.33331e-04      5.25993e-07
+    85      1.35386e-04      5.34183e-07
+    86      1.37438e-04      5.42367e-07
+    87      1.39489e-04      5.50545e-07
+    88      1.41538e-04      5.58718e-07
+    89      1.43585e-04      5.66886e-07
+    90      1.45630e-04      5.75048e-07
+    91      1.47672e-04      5.83197e-07
+    92      1.49712e-04      5.91339e-07
+    93      1.51749e-04      5.99473e-07
+    94      1.53784e-04      6.07600e-07
+    95      1.55817e-04      6.15719e-07
+    96      1.57848e-04      6.23831e-07
+    97      1.59875e-04      6.31931e-07
+    98      1.61899e-04      6.40021e-07
+    99      1.63922e-04      6.48103e-07
+   100      1.65941e-04      6.56176e-07
+   106      1.78000e-04      7.04412e-07
+   112      1.89954e-04      7.52275e-07
+   118      2.01796e-04      7.99742e-07
+   124      2.13524e-04      8.46803e-07
+   130      2.25134e-04      8.93440e-07
+   136      2.36624e-04      9.39646e-07
+   142      2.47995e-04      9.85419e-07
+   148      2.59243e-04      1.03075e-06
+   154      2.70370e-04      1.07564e-06
+   160      2.81375e-04      1.12009e-06
+   166      2.92259e-04      1.16410e-06
+   172      3.03021e-04      1.20766e-06
+   178      3.13661e-04      1.25078e-06
+   184      3.24180e-04      1.29345e-06
+   190      3.34578e-04      1.33568e-06
+   196      3.44856e-04      1.37748e-06
+   202      3.55015e-04      1.41883e-06
+   208      3.65053e-04      1.45974e-06
+   214      3.74973e-04      1.50022e-06
+   220      3.84773e-04      1.54025e-06
+   226      3.94455e-04      1.57985e-06
+   232      4.04019e-04      1.61902e-06
+   238      4.13466e-04      1.65774e-06
+   244      4.22795e-04      1.69604e-06
+   250      4.32008e-04      1.73389e-06
+   256      4.41103e-04      1.77132e-06
+   262      4.50081e-04      1.80830e-06
+   268      4.58942e-04      1.84486e-06
+   274      4.67688e-04      1.88098e-06
+   280      4.76317e-04      1.91666e-06
+   286      4.84830e-04      1.95191e-06
+   292      4.93228e-04      1.98673e-06
+   298      5.01509e-04      2.02111e-06
+   304      5.09675e-04      2.05505e-06
+   310      5.17726e-04      2.08856e-06
+   316      5.25661e-04      2.12163e-06
+   322      5.33480e-04      2.15427e-06
+   328      5.41185e-04      2.18647e-06
+   334      5.48774e-04      2.21823e-06
+   340      5.56249e-04      2.24955e-06
+   346      5.63608e-04      2.28044e-06
+   352      5.70853e-04      2.31088e-06
+   358      5.77983e-04      2.34089e-06
+   364      5.84998e-04      2.37045e-06
+   370      5.91899e-04      2.39957e-06
+   376      5.98685e-04      2.42825e-06
+   382      6.05356e-04      2.45648e-06
+   388      6.11914e-04      2.48428e-06
+   394      6.18357e-04      2.51163e-06
+   400      6.24685e-04      2.53853e-06
+   406      6.30900e-04      2.56499e-06
+   412      6.37000e-04      2.59100e-06
+   418      6.42987e-04      2.61656e-06
+   424      6.48860e-04      2.64168e-06
+   430      6.54619e-04      2.66635e-06
+   436      6.60264e-04      2.69057e-06
+   442      6.65797e-04      2.71434e-06
+   448      6.71215e-04      2.73766e-06
+   454      6.76521e-04      2.76053e-06
+   460      6.81714e-04      2.78294e-06
+   466      6.86794e-04      2.80491e-06
+   472      6.91762e-04      2.82643e-06
+   478      6.96617e-04      2.84749e-06
+   484      7.01360e-04      2.86810e-06
+   490      7.05992e-04      2.88825e-06
+   496      7.10511e-04      2.90796e-06
+   502      7.14919e-04      2.92720e-06
+   508      7.19216e-04      2.94600e-06
+   514      7.23403e-04      2.96434e-06
+   520      7.27478e-04      2.98223e-06
+   526      7.31444e-04      2.99966e-06
+   532      7.35300e-04      3.01664e-06
+   538      7.39045e-04      3.03316e-06
+   544      7.42682e-04      3.04923e-06
+   550      7.46209e-04      3.06484e-06
+   556      7.49629e-04      3.08000e-06
+   562      7.52940e-04      3.09471e-06
+   568      7.56143e-04      3.10896e-06
+   574      7.59240e-04      3.12276e-06
+   580      7.62229e-04      3.13610e-06
+   586      7.65112e-04      3.14899e-06
+   592      7.67889e-04      3.16143e-06
+   598      7.70561e-04      3.17342e-06
+   604      7.73128e-04      3.18495e-06
+   610      7.75591e-04      3.19604e-06
+   616      7.77949e-04      3.20667e-06
+   622      7.80205e-04      3.21685e-06
+   628      7.82358e-04      3.22659e-06
+   634      7.84409e-04      3.23587e-06
+   640      7.86358e-04      3.24471e-06
+   646      7.88206e-04      3.25310e-06
+   652      7.89954e-04      3.26104e-06
+   658      7.91602e-04      3.26854e-06
+   664      7.93152e-04      3.27560e-06
+   670      7.94603e-04      3.28221e-06
+   676      7.95957e-04      3.28838e-06
+   682      7.97214e-04      3.29411e-06
+   688      7.98375e-04      3.29940e-06
+   694      7.99441e-04      3.30425e-06
+   700      8.00412e-04      3.30867e-06
+   706      8.01289e-04      3.31265e-06
+   712      8.02074e-04      3.31619e-06
+   718      8.02766e-04      3.31931e-06
+   724      8.03368e-04      3.32199e-06
+   730      8.03879e-04      3.32425e-06
+   736      8.04300e-04      3.32607e-06
+   742      8.04633e-04      3.32748e-06
+   748      8.04879e-04      3.32846e-06
+   754      8.05037e-04      3.32902e-06
+   760      8.05110e-04      3.32916e-06
+   766      8.05099e-04      3.32888e-06
+   772      8.05003e-04      3.32818e-06
+   778      8.04824e-04      3.32708e-06
+   784      8.04564e-04      3.32556e-06
+   790      8.04223e-04      3.32363e-06
+   796      8.03802e-04      3.32129e-06
+   802      8.03303e-04      3.31855e-06
+   808      8.02726e-04      3.31540e-06
+   814      8.02073e-04      3.31186e-06
+   820      8.01344e-04      3.30792e-06
+   826      8.00535e-04      3.30358e-06
+   832      7.99629e-04      3.29885e-06
+   838      7.98625e-04      3.29373e-06
+   844      7.97522e-04      3.28823e-06
+   850      7.96323e-04      3.28234e-06
+   856      7.95027e-04      3.27607e-06
+   862      7.93635e-04      3.26942e-06
+   868      7.92147e-04      3.26239e-06
+   874      7.90564e-04      3.25500e-06
+   880      7.88887e-04      3.24723e-06
+   886      7.87115e-04      3.23910e-06
+   892      7.85250e-04      3.23061e-06
+   898      7.83291e-04      3.22175e-06
+   904      7.81240e-04      3.21255e-06
+   910      7.79097e-04      3.20298e-06
+   916      7.76863e-04      3.19307e-06
+   922      7.74538e-04      3.18282e-06
+   928      7.72123e-04      3.17222e-06
+   934      7.69619e-04      3.16128e-06
+   940      7.67025e-04      3.15001e-06
+   946      7.64343e-04      3.13841e-06
+   952      7.61574e-04      3.12648e-06
+   958      7.58718e-04      3.11423e-06
+   964      7.55776e-04      3.10166e-06
+   970      7.52748e-04      3.08878e-06
+   976      7.49635e-04      3.07558e-06
+   982      7.46439e-04      3.06208e-06
+   988      7.43159e-04      3.04827e-06
+   994      7.39796e-04      3.03417e-06
+  1000      7.36352e-04      3.01977e-06
+  1006      7.32827e-04      3.00508e-06
+  1012      7.29221e-04      2.99011e-06
+  1018      7.25536e-04      2.97485e-06
+  1024      7.21772e-04      2.95932e-06
+  1030      7.17931e-04      2.94352e-06
+  1036      7.14012e-04      2.92746e-06
+  1042      7.10017e-04      2.91113e-06
+  1048      7.05947e-04      2.89455e-06
+  1054      7.01803e-04      2.87772e-06
+  1060      6.97585e-04      2.86063e-06
+  1066      6.93294e-04      2.84331e-06
+  1072      6.88932e-04      2.82575e-06
+  1078      6.84499e-04      2.80795e-06
+  1084      6.79995e-04      2.78993e-06
+  1090      6.75424e-04      2.77169e-06
+  1096      6.70784e-04      2.75323e-06
+  1102      6.66077e-04      2.73455e-06
+  1108      6.61304e-04      2.71567e-06
+  1114      6.56467e-04      2.69660e-06
+  1120      6.51565e-04      2.67732e-06
+  1126      6.46600e-04      2.65785e-06
+  1132      6.41573e-04      2.63820e-06
+  1138      6.36485e-04      2.61837e-06
+  1144      6.31338e-04      2.59837e-06
+  1150      6.26132e-04      2.57820e-06
+  1156      6.20868e-04      2.55787e-06
+  1162      6.15548e-04      2.53739e-06
+  1168      6.10172e-04      2.51675e-06
+  1174      6.04742e-04      2.49597e-06
+  1180      5.99259e-04      2.47504e-06
+  1186      5.93723e-04      2.45399e-06
+  1192      5.88136e-04      2.43281e-06
+  1198      5.82500e-04      2.41151e-06
+  1204      5.76815e-04      2.39009e-06
+  1210      5.71083e-04      2.36857e-06
+  1216      5.65305e-04      2.34694e-06
+  1222      5.59482e-04      2.32522e-06
+  1228      5.53615e-04      2.30340e-06
+  1234      5.47706e-04      2.28151e-06
+  1240      5.41755e-04      2.25953e-06
+  1246      5.35764e-04      2.23748e-06
+  1252      5.29735e-04      2.21537e-06
+  1258      5.23668e-04      2.19320e-06
+  1264      5.17566e-04      2.17098e-06
+  1270      5.11429e-04      2.14871e-06
+  1276      5.05258e-04      2.12640e-06
+  1282      4.99055e-04      2.10406e-06
+  1288      4.92822e-04      2.08169e-06
+  1294      4.86559e-04      2.05929e-06
+  1300      4.80268e-04      2.03689e-06
+  1306      4.73951e-04      2.01447e-06
+  1312      4.67608e-04      1.99205e-06
+  1318      4.61241e-04      1.96964e-06
+  1324      4.54853e-04      1.94724e-06
+  1330      4.48443e-04      1.92485e-06
+  1336      4.42014e-04      1.90248e-06
+  1342      4.35567e-04      1.88015e-06
+  1348      4.29104e-04      1.85785e-06
+  1354      4.22626e-04      1.83559e-06
+  1360      4.16133e-04      1.81337e-06
+  1366      4.09629e-04      1.79121e-06
+  1372      4.03115e-04      1.76910e-06
+  1378      3.96591e-04      1.74706e-06
+  1384      3.90060e-04      1.72509e-06
+  1390      3.83524e-04      1.70319e-06
+  1396      3.76983e-04      1.68138e-06
+  1402      3.70439e-04      1.65965e-06
+  1408      3.63894e-04      1.63800e-06
+  1414      3.57350e-04      1.61646e-06
+  1420      3.50808e-04      1.59501e-06
+  1426      3.44270e-04      1.57367e-06
+  1432      3.37737e-04      1.55244e-06
+  1438      3.31211e-04      1.53132e-06
+  1444      3.24694e-04      1.51032e-06
+  1450      3.18188e-04      1.48944e-06
+  1456      3.11694e-04      1.46869e-06
+  1462      3.05213e-04      1.44806e-06
+  1468      2.98748e-04      1.42757e-06
+  1474      2.92301e-04      1.40721e-06
+  1480      2.85873e-04      1.38698e-06
+  1486      2.79464e-04      1.36690e-06
+  1492      2.73079e-04      1.34695e-06
+  1498      2.66719e-04      1.32715e-06
+  1504      2.60384e-04      1.30750e-06
+  1510      2.54077e-04      1.28798e-06
+  1516      2.47800e-04      1.26861e-06
+  1522      2.41554e-04      1.24939e-06
+  1528      2.35342e-04      1.23031e-06
+  1534      2.29165e-04      1.21138e-06
+  1540      2.23025e-04      1.19259e-06
+  1546      2.16925e-04      1.17394e-06
+  1552      2.10865e-04      1.15544e-06
+  1558      2.04847e-04      1.13706e-06
+  1564      1.98875e-04      1.11883e-06
+  1570      1.92949e-04      1.10072e-06
+  1576      1.87072e-04      1.08274e-06
+  1582      1.81245e-04      1.06488e-06
+  1588      1.75470e-04      1.04714e-06
+  1594      1.69750e-04      1.02951e-06
+  1600      1.64087e-04      1.01199e-06
+  1606      1.58482e-04      9.94561e-07
+  1612      1.52936e-04      9.77227e-07
+  1618      1.47454e-04      9.59978e-07
+  1624      1.42036e-04      9.42803e-07
+  1630      1.36685e-04      9.25695e-07
+  1636      1.31402e-04      9.08676e-07
+  1642      1.26189e-04      8.91743e-07
+  1648      1.21049e-04      8.74850e-07
+  1654      1.15984e-04      8.57985e-07
+  1660      1.10995e-04      8.41137e-07
+  1666      1.06086e-04      8.24296e-07
+  1672      1.01258e-04      8.07445e-07
+  1678      9.65128e-05      7.90574e-07
+  1684      9.18531e-05      7.73670e-07
+  1690      8.72809e-05      7.56717e-07
+  1696      8.27984e-05      7.39702e-07
+  1702      7.84077e-05      7.22608e-07
+  1708      7.41111e-05      7.05422e-07
+  1714      6.99106e-05      6.88126e-07
+  1720      6.58087e-05      6.70705e-07
+  1726      6.18074e-05      6.53143e-07
+  1732      5.79091e-05      6.35421e-07
+  1738      5.41160e-05      6.17523e-07
+  1744      5.04304e-05      5.99431e-07
+  1750      4.68544e-05      5.81128e-07
+  1756      4.33904e-05      5.62594e-07
+  1762      4.00408e-05      5.43812e-07
+  1768      3.68077e-05      5.24762e-07
+  1774      3.36936e-05      5.05426e-07
+  1780      3.07007e-05      4.85786e-07
+  1786      2.78315e-05      4.65820e-07
+  1792      2.50882e-05      4.45511e-07
+  1798      2.24732e-05      4.24839e-07
+  1804      1.99889e-05      4.03782e-07
+  1810      1.76378e-05      3.82324e-07
+  1816      1.54221e-05      3.60442e-07
+  1822      1.33443e-05      3.38117e-07
+  1828      1.14070e-05      3.15330e-07
+  1834      9.61228e-06      2.92059e-07
+  1840      7.96282e-06      2.68286e-07
+  1846      6.46106e-06      2.43990e-07
+  1852      5.10944e-06      2.19151e-07
+  1858      3.91045e-06      1.93748e-07
+  1864      2.86660e-06      1.67763e-07
+  1870      1.98036e-06      1.41174e-07
+  1876      1.25427e-06      1.13962e-07
+  1882      6.90856e-07      8.61072e-08
+  1888      2.92654e-07      5.75893e-08
+  1894      6.22143e-08      2.83886e-08
+ 1899.1     0.00000e+00      0.00000e+00
```

### Comparing `opengate-10.0b7/opengate/sources/gansources.py` & `opengate-10.0b8/opengate/sources/gansources.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/sources/generic.py` & `opengate-10.0b8/opengate/sources/generic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from box import Box
 from scipy.spatial.transform import Rotation
 import pathlib
 import numpy as np
 
-
 import opengate_core
 from ..utility import g4_units
 from ..exception import fatal, warning
 from ..definitions import __world_name__
 from ..userelement import UserElement
 
-
 gate_source_path = pathlib.Path(__file__).parent.resolve()
 
 # http://www.lnhb.fr/nuclear-data/module-lara/
 all_beta_plus_radionuclides = [
     "F18",
     "Ga68",
     "Zr89",
@@ -104,33 +102,34 @@
     return v
 
 
 def get_rad_gamma_energy_spectrum(rad):
     weights = {}
     energies = {}
     MeV = g4_units.MeV
+    rad = rad.lower()
     # Tc99m
-    weights["Tc99m"] = [0.885]
-    energies["Tc99m"] = [0.140511 * MeV]
+    weights["tc99m"] = [0.885]
+    energies["tc99m"] = [0.140511 * MeV]
     # Lu177
-    weights["Lu177"] = [0.001726, 0.0620, 0.000470, 0.1038, 0.002012, 0.00216]
-    energies["Lu177"] = [
+    weights["lu177"] = [0.001726, 0.0620, 0.000470, 0.1038, 0.002012, 0.00216]
+    energies["lu177"] = [
         0.0716418 * MeV,
         0.1129498 * MeV,
         0.1367245 * MeV,
         0.2083662 * MeV,
         0.2496742 * MeV,
         0.3213159 * MeV,
     ]
 
     # In111
-    weights["In111"] = [0.000015, 0.9061, 0.9412]
-    energies["In111"] = [0.15081 * MeV, 0.17128 * MeV, 0.24535 * MeV]
+    weights["in111"] = [0.000015, 0.9061, 0.9412]
+    energies["in111"] = [0.15081 * MeV, 0.17128 * MeV, 0.24535 * MeV]
     # I131
-    weights["I131"] = [
+    weights["i131"] = [
         0.02607,
         0.000051,
         0.000211,
         0.00277,
         0.000023,
         0.000581,
         0.0614,
@@ -143,15 +142,15 @@
         0.812,
         0.000552,
         0.003540,
         0.0712,
         0.002183,
         0.01786,
     ]
-    energies["I131"] = [
+    energies["i131"] = [
         0.080185 * MeV,
         0.0859 * MeV,
         0.163930 * MeV,
         0.177214 * MeV,
         0.23218 * MeV,
         0.272498 * MeV,
         0.284305 * MeV,
@@ -261,26 +260,35 @@
             f"End time           : {end}"
         )
         return s
 
     def create_g4_source(self):
         fatal('The function "create_g4_source" *must* be overridden')
 
-    def initialize(self, run_timing_intervals):
+    def initialize_source_before_g4_engine(self, source):
+        pass
+
+    def initialize_start_end_time(self, run_timing_intervals):
         self.run_timing_intervals = run_timing_intervals
         # by default consider the source time start and end like the whole simulation
         # Start: start time of the first run
         # End: end time of the last run
         if not self.user_info.start_time:
             self.user_info.start_time = run_timing_intervals[0][0]
         if not self.user_info.end_time:
             self.user_info.end_time = run_timing_intervals[-1][1]
+
+    def initialize(self, run_timing_intervals):
+        self.initialize_start_end_time(run_timing_intervals)
         # this will initialize and set user_info to the cpp side
         self.g4_source.InitializeUserInfo(self.user_info.__dict__)
 
+    def add_to_source_manager(self, source_manager):
+        source_manager.AddSource(self.g4_source)
+
     def prepare_output(self):
         pass
 
     def get_estimated_number_of_events(self, run_timing_interval):
         """# by default, all event have the same time, so we check that
         # this time is included into the given time interval
         if (
@@ -301,63 +309,74 @@
     """
 
     type_name = "GenericSource"
 
     @staticmethod
     def set_default_user_info(user_info):
         SourceBase.set_default_user_info(user_info)
+
         # initial user info
         user_info.particle = "gamma"
         user_info.ion = Box()
         user_info.weight = -1
         user_info.weight_sigma = -1
         user_info.user_particle_life_time = -1  # negative means : by default
         user_info.tac_times = None
         user_info.tac_activities = None
         user_info.force_rotation = False
+
         # ion
         user_info.ion = Box()
         user_info.ion.Z = 0  # Z: Atomic Number
         user_info.ion.A = 0  # A: Atomic Mass (nn + np +nlambda)
         user_info.ion.E = 0  # E: Excitation energy (i.e. for metastable)
+
         # position
         user_info.position = Box()
         user_info.position.type = "point"
         user_info.position.radius = 0
         user_info.position.sigma_x = 0
         user_info.position.sigma_y = 0
         user_info.position.size = [0, 0, 0]
         user_info.position.translation = [0, 0, 0]
         user_info.position.rotation = Rotation.identity().as_matrix()
         user_info.position.confine = None
+
         # angle (direction)
         deg = g4_units.deg
-
         user_info.direction = Box()
         user_info.direction.type = "iso"
         user_info.direction.theta = [0, 180 * deg]
         user_info.direction.phi = [0, 360 * deg]
         user_info.direction.momentum = [0, 0, 1]
         user_info.direction.focus_point = [0, 0, 0]
         user_info.direction.sigma = [0, 0]
         user_info.direction.acceptance_angle = Box()
         user_info.direction.acceptance_angle.skip_policy = "SkipEvents"  # or ZeroEnergy
         user_info.direction.acceptance_angle.volumes = []
         user_info.direction.acceptance_angle.intersection_flag = False
         user_info.direction.acceptance_angle.normal_flag = False
         user_info.direction.acceptance_angle.normal_vector = [0, 0, 1]
         user_info.direction.acceptance_angle.normal_tolerance = 3 * deg
+        user_info.direction.accolinearity_flag = False  # only for back_to_back source
+        user_info.direction.histogram_theta_weight = []
+        user_info.direction.histogram_theta_angle = []
+        user_info.direction.histogram_phi_weight = []
+        user_info.direction.histogram_phi_angle = []
+
         # energy
         user_info.energy = Box()
         user_info.energy.type = "mono"
         user_info.energy.mono = 0
         user_info.energy.sigma_gauss = 0
         user_info.energy.is_cdf = False
         user_info.energy.min_energy = None
         user_info.energy.max_energy = None
+        user_info.energy.histogram_weight = None
+        user_info.energy.histogram_energy = None
 
     def create_g4_source(self):
         return opengate_core.GateGenericSource()
 
     def __init__(self, user_info):
         super().__init__(user_info)
         if not self.user_info.particle.startswith("ion"):
@@ -397,14 +416,19 @@
                 f"Generic Source: user_info.direction must be a Box, but is: {self.user_info.direction}"
             )
         if not isinstance(self.user_info.energy, Box):
             fatal(
                 f"Generic Source: user_info.energy must be a Box, but is: {self.user_info.energy}"
             )
 
+        if self.user_info.particle == "back_to_back":
+            # force the energy to 511 keV
+            self.user_info.energy.type = "mono"
+            self.user_info.energy.mono = 511 * g4_units.keV
+
         # check energy type
         l = [
             "mono",
             "gauss",
             "F18_analytic",
             "O15_analytic",
             "C11_analytic",
@@ -431,14 +455,31 @@
                 # self.user_info.activity *= total
                 self.user_info.energy.is_cdf = True
                 self.g4_source.SetEnergyCDF(ene)
                 self.g4_source.SetProbabilityCDF(cdf)
 
         self.update_tac_activity()
 
+        # histogram parameters: histogram_weight, histogram_energy"
+        ene = self.user_info.energy
+        if ene.type == "histogram":
+            if len(ene.histogram_weight) != len(ene.histogram_energy):
+                fatal(
+                    f"For the source {self.user_info.name} energy, "
+                    f'"histogram_energy" and "histogram_weight" must have the same length'
+                )
+
+        # check direction type
+        l = ["iso", "histogram", "momentum", "focused", "beam2d"]
+        if not self.user_info.direction.type in l:
+            fatal(
+                f"Cannot find the direction type {self.user_info.direction.type} for the source {self.user_info.name}.\n"
+                f"Available types are {l}"
+            )
+
         # logic for half life and user_particle_life_time
         ui = self.user_info
         if ui.half_life > 0:
             # if the user set the half life and not the user_particle_life_time
             # we force the latter to zero
             if ui.user_particle_life_time < 0:
                 ui.user_particle_life_time = 0
@@ -459,14 +500,32 @@
         if self.user_info.position.confine:
             if self.user_info.position.type == "point":
                 warning(
                     f"In source {self.user_info.name}, "
                     f"confine is used, while position.type is point ... really ?"
                 )
 
+    def check_ui_activity(self, ui):
+        if ui.n > 0 and ui.activity > 0:
+            fatal(f"Cannot use both n and activity, choose one: {self.user_info}")
+        if ui.n == 0 and ui.activity == 0:
+            fatal(f"Choose either n or activity : {self.user_info}")
+        if ui.activity > 0:
+            ui.n = 0
+        if ui.n > 0:
+            ui.activity = 0
+
+    def check_confine(self, ui):
+        if ui.position.confine:
+            if ui.position.type == "point":
+                warning(
+                    f"In source {ui.name}, "
+                    f"confine is used, while position.type is point ... really ?"
+                )
+
     def prepare_output(self):
         SourceBase.prepare_output(self)
         # store the output from G4 object
         self.fTotalZeroEvents = self.g4_source.fTotalZeroEvents
         self.fTotalSkippedEvents = self.g4_source.fTotalSkippedEvents
 
     def update_tac_activity(self):
```

### Comparing `opengate-10.0b7/opengate/sources/phspsources.py` & `opengate-10.0b8/opengate/sources/phspsources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import threading
 import uproot
 import numpy as np
 import numbers
 from scipy.spatial.transform import Rotation
 from box import Box
 
 import opengate_core
@@ -24,14 +23,15 @@
         self.cycle_count = 0
         # used during generation
         self.batch = None
         self.points = None
         self.w = None
 
     def __getstate__(self):
+        ## FIXME
         self.lock = None
         return self.__dict__
 
     def initialize(self, user_info):
         self.user_info = user_info
         self.read_phsp_and_keys()
 
@@ -192,15 +192,15 @@
             source.SetDirectionYBatch(batch[ui.direction_key_y])
             source.SetDirectionZBatch(batch[ui.direction_key_z])
 
         # set energy
         source.SetEnergyBatch(batch[ui.energy_key])
 
         # set weight
-        if ui.weight_key != "" or ui.weight_key is not None:
+        if ui.weight_key != "" and ui.weight_key is not None:
             if ui.weight_key in batch:
                 source.SetWeightBatch(batch[ui.weight_key])
             else:
                 fatal(
                     f"PhaseSpaceSource: no Weight key ({ui.weight_key}) in the phsp file."
                 )
         else:
```

### Comparing `opengate-10.0b7/opengate/sources/voxelsources.py` & `opengate-10.0b8/opengate/sources/voxelsources.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         user_info.position.rotation = Rotation.identity().as_matrix()
         # default values
         user_info.direction.type = "iso"
         user_info.energy.type = "mono"
         user_info.energy.mono = 0
 
     def __init__(self, user_info):
+        ## FIXME
         super().__init__(user_info)
         self.image = None
 
     def __getstate__(self):
         super().__getstate__()
         self.image = None
         return self.__dict__
```

### Comparing `opengate-10.0b7/opengate/tests/src/test001_g4threevector.py` & `opengate-10.0b8/opengate/tests/src/test001_g4threevector.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test003_g4material.py` & `opengate-10.0b8/opengate/tests/src/test003_g4material.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test004_simple.py` & `opengate-10.0b8/opengate/tests/src/test004_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     stats.track_types_flag = True
 
     """
     Start the simulation ! You can relax and drink coffee.
     (The commented line indicates how to indicate to Geant4 to verbose during the simulation,
     if the flag sim.g4_verbose is True).
     """
-    # sim.apply_g4_command("/run/verbose 1")
+    # sim.add_g4_command_after_init("/run/verbose 1")
     sim.user_hook_after_init = check_production_cuts
     sim.run()
 
     """
     Now the simulation is terminated. The results are retrieved and can be displayed.
     """
     stats = sim.output.get_actor("Stats")
```

### Comparing `opengate-10.0b7/opengate/tests/src/test004_simple_mt.py` & `opengate-10.0b8/opengate/tests/src/test004_simple_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test004_simple_subprocess.py` & `opengate-10.0b8/opengate/tests/src/test004_simple_subprocess.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test004_simple_visu_gdml.py` & `opengate-10.0b8/opengate/tests/src/test004_simple_visu_gdml.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test004_simple_visu_geometry.py` & `opengate-10.0b8/opengate/tests/src/test004_simple_visu_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,11 +108,11 @@
     stats = sim.add_actor("SimulationStatisticsActor", "Stats")
     stats.track_types_flag = True
 
     """
     Start the simulation ! You can relax and drink coffee.
     (The commented line indicates how to indicate to Geant4 to verbose during the simulation).
     """
-    # sim.apply_g4_command("/run/verbose 1")
+    # sim.add_g4_command_after_init("/run/verbose 1")
     sim.user_hook_after_init = check_production_cuts
 
     sim.visualize_geometry()
```

### Comparing `opengate-10.0b7/opengate/tests/src/test004_simple_visu_qt.py` & `opengate-10.0b8/opengate/tests/src/test004_simple_visu_qt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test004_simple_visu_vrml.py` & `opengate-10.0b8/opengate/tests/src/test004_simple_visu_vrml.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test004_simple_visu_vrml_file.py` & `opengate-10.0b8/opengate/tests/src/test004_simple_visu_vrml_file.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test004_simulation_stats_actor.py` & `opengate-10.0b8/opengate/tests/src/test004_simulation_stats_actor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test005_proton.py` & `opengate-10.0b8/opengate/tests/src/test005_proton.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,10 +55,10 @@
     print("Simulation seed:", sim.output.current_random_seed)
     print(stats)
 
     # gate_test5_proton
     # Gate mac/main.mac
     print("-" * 80)
     stats_ref = utility.read_stat_file(paths.gate_output / "stat.txt")
-    is_ok = utility.assert_stats(stats, stats_ref, tolerance=0.15)
+    is_ok = utility.assert_stats(stats, stats_ref, tolerance=0.155)
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test006_runs.py` & `opengate-10.0b8/opengate/tests/src/test006_runs.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test007_volumes.py` & `opengate-10.0b8/opengate/tests/src/test007_volumes.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,100 @@
     print("global_translation_old, global_rotation_old: ")
     print(global_translation_old, global_rotation_old)
     print("global_translation_new, global_rotation_new: ")
     print(global_translation_new, global_rotation_new)
     print("***********************************************************")
 
 
+def check_mat(se):
+    pathFile = pathlib.Path(__file__).parent.resolve()
+
+    # explicit check overlap (already performed during initialize)
+    print("check overlap with verbose")
+    se.check_volumes_overlap(verbose=True)
+    sim = se.simulation
+
+    # print info material db
+    dbn = sim.volume_manager.dump_material_database_names()
+    mnist = se.volume_engine.get_database_material_names("NIST")
+    mdb = se.volume_engine.get_database_material_names(
+        pathFile / ".." / "data" / "GateMaterials.db"
+    )
+    dm = se.volume_engine.dump_build_materials()
+    print("Material info:")
+    print("\t databases    :", dbn)
+    print("\t mat in NIST  :", len(mnist), mnist)
+    print("\t mat in db    :", mdb)
+    print("\t defined mat  :", dm)
+
+    print("dbn", dbn)
+    assert dbn == [pathFile / ".." / "data" / "GateMaterials.db"]
+    # assert len(mnist) == 308  # Geant4 11.02
+    assert len(mnist) == 309  # Geant4 11.1
+    assert mdb == [
+        "Vacuum",
+        "Aluminium",
+        "Uranium",
+        "Silicon",
+        "Germanium",
+        "Yttrium",
+        "Gadolinium",
+        "Lutetium",
+        "Tungsten",
+        "Lead",
+        "Bismuth",
+        "NaI",
+        "NaITl",
+        "PWO",
+        "BGO",
+        "LSO",
+        "Plexiglass",
+        "GSO",
+        "LuAP",
+        "YAP",
+        "Water",
+        "Quartz",
+        "Breast",
+        "Air",
+        "Glass",
+        "Scinti-C9H10",
+        "LuYAP-70",
+        "LuYAP-80",
+        "Plastic",
+        "CZT",
+        "Lung",
+        "Polyethylene",
+        "PVC",
+        "SS304",
+        "PTFE",
+        "LYSO",
+        "Body",
+        "Muscle",
+        "LungMoby",
+        "SpineBone",
+        "RibBone",
+        "Adipose",
+        "Blood",
+        "Heart",
+        "Kidney",
+        "Liver",
+        "Lymph",
+        "Pancreas",
+        "Intestine",
+        "Skull",
+        "Cartilage",
+        "Brain",
+        "Spleen",
+        "Testis",
+        "PMMA",
+    ]
+    assert dm == ["G4_AIR", "G4_WATER", "Lead", "Lung", "G4_LUCITE"]
+    assert len(se.volume_engine.dump_build_materials()) == 5
+
+
 if __name__ == "__main__":
     pathFile = pathlib.Path(__file__).parent.resolve()
     paths = utility.get_default_test_paths(__file__)
 
     # create the simulation
     sim = gate.Simulation()
     print(f"Volumes types: {sim.volume_manager.dump_volume_types()}")
@@ -106,106 +192,24 @@
     sim.run_timing_intervals = [
         [0, 0.5 * sec]
         # ,[0.5 * sec, 1.2 * sec]
     ]
 
     print(sim)
 
-    def check_mat(se):
-        # explicit check overlap (already performed during initialize)
-        print("check overlap with verbose")
-        se.check_volumes_overlap(verbose=True)
-
-        # print info material db
-        dbn = sim.volume_manager.dump_material_database_names()
-        mnist = se.volume_engine.get_database_material_names("NIST")
-        mdb = se.volume_engine.get_database_material_names(
-            pathFile / ".." / "data" / "GateMaterials.db"
-        )
-        dm = se.volume_engine.dump_build_materials()
-        print("Material info:")
-        print("\t databases    :", dbn)
-        print("\t mat in NIST  :", len(mnist), mnist)
-        print("\t mat in db    :", mdb)
-        print("\t defined mat  :", dm)
-
-        print("dbn", dbn)
-        assert dbn == [pathFile / ".." / "data" / "GateMaterials.db"]
-        # assert len(mnist) == 308  # Geant4 11.02
-        assert len(mnist) == 309  # Geant4 11.1
-        assert mdb == [
-            "Vacuum",
-            "Aluminium",
-            "Uranium",
-            "Silicon",
-            "Germanium",
-            "Yttrium",
-            "Gadolinium",
-            "Lutetium",
-            "Tungsten",
-            "Lead",
-            "Bismuth",
-            "NaI",
-            "NaITl",
-            "PWO",
-            "BGO",
-            "LSO",
-            "Plexiglass",
-            "GSO",
-            "LuAP",
-            "YAP",
-            "Water",
-            "Quartz",
-            "Breast",
-            "Air",
-            "Glass",
-            "Scinti-C9H10",
-            "LuYAP-70",
-            "LuYAP-80",
-            "Plastic",
-            "CZT",
-            "Lung",
-            "Polyethylene",
-            "PVC",
-            "SS304",
-            "PTFE",
-            "LYSO",
-            "Body",
-            "Muscle",
-            "LungMoby",
-            "SpineBone",
-            "RibBone",
-            "Adipose",
-            "Blood",
-            "Heart",
-            "Kidney",
-            "Liver",
-            "Lymph",
-            "Pancreas",
-            "Intestine",
-            "Skull",
-            "Cartilage",
-            "Brain",
-            "Spleen",
-            "Testis",
-            "PMMA",
-        ]
-        assert dm == ["G4_AIR", "G4_WATER", "Lead", "Lung", "G4_LUCITE"]
-        assert len(se.volume_engine.dump_build_materials()) == 5
-
     # verbose
     sim.add_g4_command_after_init("/tracking/verbose 0")
     # sim.g4_com("/run/verbose 2")
     # sim.g4_com("/event/verbose 2")
     # sim.g4_com("/tracking/verbose 1")
 
     # start simulation
     sim.user_hook_after_init = check_mat
     sim.user_hook_after_run = user_hook_volume
-    sim.run()
+    sim.run(start_new_process=True)
 
     # print results at the end
     stats = sim.output.get_actor("Stats")
     print(stats)
 
     # check
     stats_ref = gate.actors.miscactors.SimulationStatisticsActor()
```

### Comparing `opengate-10.0b7/opengate/tests/src/test008_dose_actor.py` & `opengate-10.0b8/opengate/tests/src/test008_dose_actor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 
 import opengate as gate
 from opengate.tests import utility
 from scipy.spatial.transform import Rotation
 import pathlib
 
 if __name__ == "__main__":
-    current_path = pathlib.Path(__file__).parent.resolve()
-    data_path = current_path / ".." / "data"
-    ref_path = (
-        current_path / ".." / "data" / "gate" / "gate_test008_dose_actor" / "output"
-    )
+    paths = utility.get_default_test_paths(__file__, "gate_test008_dose_actor")
+    output_path = paths.output
+    data_path = paths.data
+    ref_path = paths.gate_output
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
     sim.g4_verbose_level = 1
     sim.visu = False
     sim.random_seed = 12345678
-    sim.output_dir = current_path / ".." / "output"
+    sim.output_dir = output_path
 
     # shortcuts for units
     m = gate.g4_units.m
     cm = gate.g4_units.cm
 
     #  change world size
     world = sim.world
@@ -71,15 +70,15 @@
     source.position.radius = 1 * nm
     source.direction.type = "momentum"
     source.direction.momentum = [0, 0, 1]
     source.activity = 50000 * Bq
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = "test008-edep.mhd"
+    dose.output = "test008.mhd"
     dose.mother = "waterbox"
     dose.size = [99, 99, 99]
     mm = gate.g4_units.mm
     dose.spacing = [2 * mm, 2 * mm, 2 * mm]
     dose.translation = [2 * mm, 3 * mm, -2 * mm]
     dose.uncertainty = True
     dose.hit_type = "random"
@@ -102,28 +101,28 @@
     stats_ref = utility.read_stat_file(ref_path / "stat.txt")
     is_ok = utility.assert_stats(stat, stats_ref, 0.11)
 
     print("\nDifference for EDEP")
     is_ok = (
         utility.assert_images(
             ref_path / "output-Edep.mhd",
-            sim.output_dir / "test008-edep.mhd",
+            sim.output_dir / dose.user_info.output,
             stat,
             tolerance=13,
             ignore_value=0,
             sum_tolerance=1,
         )
         and is_ok
     )
 
     print("\nDifference for uncertainty")
     is_ok = (
         utility.assert_images(
             ref_path / "output-Edep-Uncertainty.mhd",
-            sim.output_dir / "test008-edep_uncertainty.mhd",
+            sim.output_dir / dose.user_info.output_uncertainty,
             stat,
             tolerance=30,
             ignore_value=1,
             sum_tolerance=1,
         )
         and is_ok
     )
```

### Comparing `opengate-10.0b7/opengate/tests/src/test008_geometry_dose_grid.py` & `opengate-10.0b8/opengate/tests/src/test008_geometry_dose_grid.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test009_voxels.py` & `opengate-10.0b8/opengate/tests/src/test009_voxels.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from opengate.geometry.materials import (
     read_voxel_materials,
 )
 from opengate.tests import utility
 from scipy.spatial.transform import Rotation
 
 if __name__ == "__main__":
-    paths = utility.get_default_test_paths(__file__, "gate_test009_voxels")
+    paths = utility.get_default_test_paths(__file__, "gate_test009_voxels", "test009")
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
     sim.g4_verbose_level = 1
@@ -82,15 +82,15 @@
     patient.set_production_cut(
         particle_name="electron",
         value=3 * mm,
     )
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = paths.output / "test009-edep.mhd"
+    dose.output = paths.output / "test009.mhd"
     dose.mother = "patient"
     dose.size = [99, 99, 99]
     dose.spacing = [2 * mm, 2 * mm, 2 * mm]
     dose.img_coord_system = True
     dose.translation = [2 * mm, 3 * mm, -2 * mm]
     dose.hit_type = "random"
 
@@ -106,21 +106,21 @@
 
     # start simulation
     sim.run(start_new_process=True)
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     print(stat)
-    d = sim.output.get_actor("dose")
-    print(d)
+    dose = sim.output.get_actor("dose")
+    print(dose)
 
     # tests
     stats_ref = utility.read_stat_file(paths.gate_output / "stat.txt")
     is_ok = utility.assert_stats(stat, stats_ref, 0.15)
     is_ok = is_ok and utility.assert_images(
         paths.gate_output / "output-Edep.mhd",
-        paths.output / "test009-edep.mhd",
+        paths.output / dose.user_info.output,
         stat,
         tolerance=35,
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test009_voxels_hu.py` & `opengate-10.0b8/opengate/tests/src/test009_voxels_hu.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import opengate as gate
 from opengate.geometry.materials import MaterialDatabase, assert_same_material
 from opengate.tests import utility
 from scipy.spatial.transform import Rotation
 
 if __name__ == "__main__":
-    paths = utility.get_default_test_paths(__file__, "gate_test009_voxels")
+    paths = utility.get_default_test_paths(__file__, "gate_test009_voxels", "test009")
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
     sim.g4_verbose_level = 1
@@ -93,15 +93,15 @@
     source.position.translation = [0, 0, -14 * cm]
     source.activity = 10000 * Bq
     source.direction.type = "momentum"
     source.direction.momentum = [0, 0, 1]
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = paths.output / "test009_hu-edep.mhd"
+    dose.output = paths.output / "test009_hu.mhd"
     dose.mother = "patient"
     dose.size = [99, 99, 99]
     dose.spacing = [2 * mm, 2 * mm, 2 * mm]
     dose.img_coord_system = True
     dose.translation = [2 * mm, 3 * mm, -2 * mm]
     dose.hit_type = "random"
 
@@ -118,22 +118,22 @@
     # start simulation
     sim.run()
 
     # print results at the end
     gate.exception.warning(f"Check stats")
     stat = sim.output.get_actor("Stats")
     print(stat)
-    d = sim.output.get_actor("dose")
-    print(d)
+    dose = sim.output.get_actor("dose")
+    print(dose)
 
     # tests
     gate.exception.warning(f"Check dose")
     stats_ref = utility.read_stat_file(paths.gate_output / "stat_hu.txt")
     is_ok = utility.assert_stats(stat, stats_ref, 0.15)
     is_ok = is_ok and utility.assert_images(
         paths.gate_output / "output_hu-Edep.mhd",
-        paths.output / "test009_hu-edep.mhd",
+        paths.output / dose.user_info.output,
         stat,
         tolerance=35,
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test010_generic_source.py` & `opengate-10.0b8/opengate/tests/src/test010_generic_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     # actors
     stats_actor = sim.add_actor("SimulationStatisticsActor", "Stats")
 
     # src_info = sim.add_actor('SourceInfoActor', 'src_info')
     # src_info.filename = 'output/sources.root'
 
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = paths.output / "test010-edep.mhd"
+    dose.output = paths.output / "test010.mhd"
     dose.mother = "waterbox"
     dose.size = [50, 50, 50]
     dose.spacing = [4 * mm, 4 * mm, 4 * mm]
 
     # verbose
     sim.add_g4_command_after_init("/tracking/verbose 0")
     # sim.add_g4_command_after_init("/run/verbose 2")
@@ -122,13 +122,13 @@
     # Gate mac/main.mac
     # Current version is two times slower :(
     stats_ref = utility.read_stat_file(paths.gate_output / "stat.txt")
     print("-" * 80)
     is_ok = utility.assert_stats(stats, stats_ref, tolerance=0.05)
     is_ok = is_ok and utility.assert_images(
         paths.gate_output / "output-Edep.mhd",
-        paths.output / "test010-edep.mhd",
+        paths.output / dose.user_info.output,
         stats,
         tolerance=30,
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test010_generic_source_confine.py` & `opengate-10.0b8/opengate/tests/src/test010_generic_source_confine.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,35 +99,36 @@
     source.energy.type = "mono"
     source.energy.mono = 1 * MeV
 
     # actors
     sim.add_actor("SimulationStatisticsActor", "Stats")
 
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = paths.output / "test010-2-edep.mhd"
+    dose.output = paths.output / "test010-2.mhd"
     # dose.output = paths.output_ref / 'test010-2-edep.mhd'
     dose.mother = "waterbox"
     dose.size = [100, 100, 100]
     dose.spacing = [2 * mm, 1 * mm, 1 * mm]
 
     # start simulation
     sim.run()
 
     # print
     print("Simulation seed:", sim.output.current_random_seed)
 
     # get results
     stats = sim.output.get_actor("Stats")
+    dose = sim.output.get_actor("dose")
     print(stats)
     # stats.write(paths.output_ref / 'test010_confine_stats.txt')
 
     # tests
     stats_ref = utility.read_stat_file(paths.output_ref / "test010_confine_stats.txt")
     is_ok = utility.assert_stats(stats, stats_ref, 0.10)
     is_ok = is_ok and utility.assert_images(
         paths.output_ref / "test010-2-edep.mhd",
-        paths.output / "test010-2-edep.mhd",
+        paths.output / dose.user_info.output,
         stats,
         tolerance=59,
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test010_generic_source_thetaphi.py` & `opengate-10.0b8/opengate/tests/src/test010_generic_source_thetaphi.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test011_mt.py` & `opengate-10.0b8/opengate/tests/src/test011_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test012_mt_dose_actor.py` & `opengate-10.0b8/opengate/tests/src/test012_mt_dose_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import opengate as gate
 from opengate.tests import utility
 
 from scipy.spatial.transform import Rotation
 
+
 if __name__ == "__main__":
     paths = utility.get_default_test_paths(__file__, "gate_test008_dose_actor")
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
@@ -100,14 +101,14 @@
     # change the number of run to the number of threads
     stats_ref.counts.run_count = sim.number_of_threads
     is_ok = utility.assert_stats(stat, stats_ref, 0.10)
 
     is_ok = (
         utility.assert_images(
             paths.gate_output / "output-Edep.mhd",
-            paths.output / "test012-edep.mhd",
+            paths.output / dose.user_info.output,
             stat,
             tolerance=45,
         )
         and is_ok
     )
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test013_half_life.py` & `opengate-10.0b8/opengate/tests/src/test013_half_life.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     wb2 = sim.add_volume("Box", "waterbox2")
     wb2.size = [20 * cm, 20 * cm, 20 * cm]
     wb2.translation = [20 * cm, 0, 0]
 
     # physics
     sim.physics_manager.physics_list_name = "G4EmStandardPhysics_option4"
     sim.physics_manager.enable_decay = True
-    sim.physics_manager.set_production_cut("world", "all", 0.1 * mm)
+    sim.physics_manager.global_production_cuts.all = 0.1 * mm
     # p.energy_range_min = 250 * eV
     # p.energy_range_max = 15 * MeV
 
     # sources info
     activity = 10 * Bq
     hl = 6586.26 * sec  # 109.771 minutes
```

### Comparing `opengate-10.0b7/opengate/tests/src/test013_phys_lists_1.py` & `opengate-10.0b8/opengate/tests/src/test013_phys_lists_1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test013_phys_lists_2_wip.py` & `opengate-10.0b8/opengate/tests/src/test013_phys_lists_2_wip.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test013_phys_lists_3_wip.py` & `opengate-10.0b8/opengate/tests/src/test013_phys_lists_3_wip.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     print("Phys list cuts:")
     print(sim.physics_manager.dump_production_cuts())
     print("Volume tree:")
     print(sim.volume_manager.dump_volume_tree())
 
     # start simulation
     sim.g4_verbose = False
-    # sim.apply_g4_command("/tracking/verbose 1")
+    # sim.add_g4_command_after_init("/tracking/verbose 1")
     sim.user_hook_after_init = check_production_cuts
     sim.run()
 
     # Gate mac/main_3.mac
     stats = sim.output.get_actor("Stats")
     stats_ref = utility.read_stat_file(paths.gate_output / "stat_3.txt")
     is_ok = utility.assert_stats(stats, stats_ref, tolerance=0.1)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test013_phys_lists_4.py` & `opengate-10.0b8/opengate/tests/src/test013_phys_lists_4.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test013_phys_lists_5_wip.py` & `opengate-10.0b8/opengate/tests/src/test013_phys_lists_5_wip.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test013_phys_lists_6.py` & `opengate-10.0b8/opengate/tests/src/test013_phys_lists_6.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test013_phys_lists_helpers.py` & `opengate-10.0b8/opengate/tests/src/test013_phys_lists_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test014_engine_2.py` & `opengate-10.0b8/opengate/tests/src/test014_engine_2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test014_engine_helpers.py` & `opengate-10.0b8/opengate/tests/src/test014_engine_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test015_iec_phantom_1.py` & `opengate-10.0b8/opengate/tests/src/test015_iec_phantom_1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test015_iec_phantom_2.py` & `opengate-10.0b8/opengate/tests/src/test015_iec_phantom_2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test015_iec_phantom_3.py` & `opengate-10.0b8/opengate/tests/src/test015_iec_phantom_3.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,18 +66,19 @@
 
     # compare stats
     stats = sim.output.get_actor("stats")
     stats_ref = utility.read_stat_file(paths.output_ref / "test015_iec_3_stats.txt")
     is_ok = utility.assert_stats(stats, stats_ref, tolerance=0.02)
 
     # compare images
+    dose = sim.output.get_actor("dose")
     f = paths.output / "test015_iec_3.mhd"
     im_ok = utility.assert_images(
         paths.output_ref / "test015_iec_3.mhd",
-        dose.output,
+        paths.output / dose.user_info.output,
         stats,
         axis="y",
         tolerance=86,
         ignore_value=0,
         sum_tolerance=2,
     )
```

### Comparing `opengate-10.0b7/opengate/tests/src/test015_iec_phantom_4_wip.py` & `opengate-10.0b8/opengate/tests/src/test015_iec_phantom_4_wip.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     # ui.visu = True
     # ui.visu_type = "qt"
     ui.check_volumes_overlap = True
     ui.random_seed = 123654987
 
     # physics
     p = sim.get_physics_user_info()
-    p.physics_list_name = "G4EmStandardPhysics_option3"
+    sim.physics_manager.physics_list_name = "G4EmStandardPhysics_option3"
     sim.physics_manager.set_production_cut("world", "all", 10 * mm)
 
     # world size
     world = sim.world
     world.size = [0.5 * m, 0.5 * m, 0.5 * m]
 
     # add an iec phantom
```

### Comparing `opengate-10.0b7/opengate/tests/src/test016_bool_volumes.py` & `opengate-10.0b8/opengate/tests/src/test016_bool_volumes.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test017_repeater.py` & `opengate-10.0b8/opengate/tests/src/test017_repeater.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
 
     # dose actor
     d = sim.add_actor("DoseActor", "dose")
-    d.output = paths.output / "test017-edep.mhd"
+    d.output = paths.output / "test017.mhd"
     # d.output = ref_path / 'test017-edep-ref.mhd'
     d.mother = "crystal"
     d.size = [150, 150, 150]
     d.spacing = [1 * mm, 1 * mm, 1 * mm]
     d.translation = [5 * mm, 0 * mm, 0 * mm]
     d.physical_volume_index = 0
     print(
@@ -94,22 +94,22 @@
 
     # start simulation
     sim.run()
 
     # print results
     stats = sim.output.get_actor("Stats")
     # stats.write(ref_path / 'test017-stats-ref.txt')
-
+    dose = sim.output.get_actor("dose")
     # tests
     stats_ref = utility.read_stat_file(paths.output_ref / "test017-stats-ref.txt")
     is_ok = utility.assert_stats(stats, stats_ref, 0.04)
     is_ok = (
         utility.assert_images(
             paths.output_ref / "test017-edep-ref.mhd",
-            paths.output / "test017-edep.mhd",
+            paths.output / dose.user_info.output,
             stats,
             sum_tolerance=6,
             tolerance=70,
         )
         and is_ok
     )
```

### Comparing `opengate-10.0b7/opengate/tests/src/test018_pet_wip.py` & `opengate-10.0b8/opengate/tests/src/test018_pet_wip.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test019_linac_phsp_helpers.py` & `opengate-10.0b8/opengate/tests/src/test019_linac_phsp_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,55 +15,56 @@
 
 def init_test019(nt):
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
-    sim.visu = False
+    # sim.visu = True
+    sim.visu_type = "vrml"
     sim.check_volumes_overlap = False
     sim.number_of_threads = nt
     sim.random_seed = 123456789
     print(sim)
 
     # units
     m = gate.g4_units.m
     mm = gate.g4_units.mm
     nm = gate.g4_units.nm
     Bq = gate.g4_units.Bq
     MeV = gate.g4_units.MeV
 
     #  adapt world size
     world = sim.world
-    world.size = [1 * m, 1 * m, 1 * m]
+    world.size = [1 * m, 1 * m, 1.3 * m]
 
     # add a linac
     linac = gate_linac.add_linac(sim, "linac")
     linac.translation = [0, 0, 0 * m]
 
     # virtual plane for phase space
     plane = sim.add_volume("Tubs", "phase_space_plane")
-    plane.mother = world.name
+    plane.mother = linac.name
     plane.material = "G4_AIR"
     plane.rmin = 0
     plane.rmax = 70 * mm
     plane.dz = 1 * nm  # half height
-    plane.translation = [0, 0, -300.0001 * mm]
+    plane.translation = [0, 0, linac.size[2] / 2 - 300 * mm]
     plane.color = [1, 0, 0, 1]  # red
 
     # e- source
     source = sim.add_source("GenericSource", "Default")
     source.particle = "e-"
     source.mother = f"{linac.name}_target"
     source.energy.type = "gauss"
     source.energy.mono = 6.7 * MeV
     source.energy.sigma_gauss = 0.077 * MeV
     source.position.type = "disc"
     source.position.radius = 2 * mm  # FIXME not really similar to GATE need sigma etc
-    source.position.translation = [0, 0, 0.6 * mm]
+    source.position.translation = [0, 0, 0.5 * mm - 1 * nm]
     source.direction.type = "momentum"
     source.direction.momentum = [0, 0, -1]
     source.activity = 5000 * Bq / sim.number_of_threads
 
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
@@ -141,20 +142,22 @@
     fn2 = paths.output / "test019_hits.root"
     print("Reference gate tree : ", fn1)
     print("Checked Tree : ", fn2)
     data_ref, keys_ref, m_ref = phsp.load(fn1)
     data, keys, m = phsp.load(fn2)
     # find the good key's names
     keys1, keys2, scalings, tols = utility.get_keys_correspondence(keys_ref)
+    keys1.remove("Z")
+    keys2.remove("PrePosition_Z")
     # Do not check some keys
     tols[keys1.index("Weight")] = 0.001
     tols[keys1.index("Ekine")] = 0.1
     tols[keys1.index("Y")] = 2.0
-    tols[keys1.index("X")] = 2.0
-    tols[keys1.index("Z")] = 0.2
+    tols[keys1.index("X")] = 3.0
+    # tols[keys1.index("Z")] = 0.2
     # perform the test
     is_ok = (
         utility.compare_trees(
             data_ref, keys_ref, data, keys, keys1, keys2, tols, scalings, scalings, True
         )
         and is_ok
     )
@@ -174,15 +177,15 @@
     # main options
     sim.g4_verbose = False
     # sim.visu = True
     sim.visu_type = "vrml"
     sim.check_volumes_overlap = False
     # sim.running_verbose_level = gate.logger.EVENT
     sim.number_of_threads = 1
-    sim.random_seed = "auto"
+    sim.random_seed = 987654321
 
     # units
     m = gate.g4_units.m
     mm = gate.g4_units.mm
     nm = gate.g4_units.nm
 
     #  adapt world size
```

### Comparing `opengate-10.0b7/opengate/tests/src/test019_linac_phsp_pdgcode.py` & `opengate-10.0b8/opengate/tests/src/test019_linac_phsp_pdgcode.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test019_linac_phsp_source_mt.py` & `opengate-10.0b8/opengate/tests/src/test019_linac_phsp_source_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test019_phsp_actor.py` & `opengate-10.0b8/opengate/tests/src/test019_phsp_actor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test020_profiling.py` & `opengate-10.0b8/opengate/tests/src/test020_profiling.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import opengate as gate
 from opengate.tests import utility
 from scipy.spatial.transform import Rotation
 
 if __name__ == "__main__":
-    paths = utility.get_default_test_paths(__file__, "gate_test009_voxels")
+    paths = utility.get_default_test_paths(__file__, "gate_test009_voxels", "test020")
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
     sim.g4_verbose_level = 1
@@ -91,21 +91,21 @@
 
     # start simulations
     sim.run()
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     print(stat)
-    d = sim.output.get_actor("dose")
-    print(d)
+    dose = sim.output.get_actor("dose")
+    print(dose)
 
     # tests
     stats_ref = utility.read_stat_file(paths.gate / "output" / "stat_profiling.txt")
     stats_ref.counts.run_count = sim.number_of_threads
     is_ok = utility.assert_stats(stat, stats_ref, 0.1)
     is_ok = is_ok and utility.assert_images(
         paths.gate / "output" / "output_profiling-Edep.mhd",
-        paths.output / "test20-edep.mhd",
+        paths.output / dose.user_info.output,
         stat,
         tolerance=79,
     )
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test021_voxel_source1.py` & `opengate-10.0b8/opengate/tests/src/test021_voxel_source1.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         src_info.origin,
         src_info.size,
         src_info.spacing,
     )
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = paths.output / "test021-edep_1.mhd"
+    dose.output = paths.output / "test021-1.mhd"
     dose.mother = ct.name
     img_info = gate.image.read_image_info(ct.image)
     dose.size = img_info.size
     dose.spacing = img_info.spacing
     dose.img_coord_system = True
 
     # cuts
@@ -99,18 +99,18 @@
 
     # start simulation
     sim.run()
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     # stat.write(paths.output_ref / "stat021_ref_1.txt")
-
+    dose = sim.output.get_actor("dose")
     # test pixels in dose #1
     # test pixels in dose #1
-    d_even = itk.imread(str(dose.output))
+    d_even = itk.imread(paths.output / dose.user_info.output)
     s = itk.array_view_from_image(d_even).sum()
     v0 = d_even.GetPixel([5, 5, 5])
     v1 = d_even.GetPixel([1, 5, 5])
     v2 = d_even.GetPixel([1, 2, 5])
     v3 = d_even.GetPixel([5, 2, 5])
     v4 = d_even.GetPixel([6, 2, 5])
     tol = 0.15
```

### Comparing `opengate-10.0b7/opengate/tests/src/test021_voxel_source2.py` & `opengate-10.0b8/opengate/tests/src/test021_voxel_source2.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         src_info.origin,
         src_info.size,
         src_info.spacing,
     )
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = str(paths.output / "test021-edep_2.mhd")
+    dose.output = str(paths.output / "test021-2.mhd")
     dose.mother = ct.name
     img_info = gate.image.read_image_info(ct.image)
 
     """
     # test same size/spacing than source : OK
     dose.size = src_info.size
     dose.spacing = src_info.spacing
@@ -117,15 +117,16 @@
     sim.run()
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     # stat.write(paths.output_ref / "stat021_ref_2.txt")
 
     # test pixels in dose #1
-    final_dose = itk.imread(dose.output)
+    dose = sim.output.get_actor("dose")
+    final_dose = itk.imread(paths.output / dose.user_info.output)
     s = itk.array_view_from_image(final_dose).sum()
 
     # loo for all source pixels (should be five)
     src = itk.imread(source.image)
     p = []
     arr = itk.array_view_from_image(src)
     for [i, j, k], flow in np.ndenumerate(src):
@@ -148,15 +149,15 @@
     stats_ref = utility.read_stat_file(paths.output_ref / "stat021_ref_2.txt")
     stats_ref.counts.run_count = sim.number_of_threads
     is_ok = utility.assert_stats(stat, stats_ref, 0.1) and is_ok
 
     is_ok = (
         utility.assert_images(
             paths.output_ref / "test021-edep_2.mhd",
-            dose.output,
+            paths.output / dose.user_info.output,
             stat,
             tolerance=11,
             ignore_value=0,
             axis="y",
         )
         and is_ok
     )
```

### Comparing `opengate-10.0b7/opengate/tests/src/test021_voxel_source_old_wip.py` & `opengate-10.0b8/opengate/tests/src/test021_voxel_source_old_wip.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,25 +133,27 @@
     sim.run()
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     # stat.write('output_ref/stat021_ref.txt')
 
     # test pixels in dose #1
-    d_odd = itk.imread(str(dose1.output))
+    dose1 = sim.output.get_actor("dose1")
+    dose2 = sim.output.get_actor("dose2")
+    d_odd = itk.imread(paths.output / dose1.user_info.output)
     s = itk.array_view_from_image(d_odd).sum()
     v = d_odd.GetPixel([5, 5, 5])
     diff = (s - v) / s
     tol = 0.01
     is_ok = diff < tol
     diff *= 100
     utility.print_test(is_ok, f"Image #1 (odd): {v:.2f} {s:.2f} -> {diff:.2f}%")
 
     # test pixels in dose #1
-    d_even = itk.imread(str(dose2.output))
+    d_even = itk.imread(paths.output / dose2.user_info.output)
     s = itk.array_view_from_image(d_even).sum()
     v0 = d_even.GetPixel([5, 5, 5])
     v1 = d_even.GetPixel([1, 5, 5])
     v2 = d_even.GetPixel([1, 2, 5])
     v3 = d_even.GetPixel([5, 2, 5])
     v4 = d_even.GetPixel([6, 2, 5])
     tol = 0.15
```

### Comparing `opengate-10.0b7/opengate/tests/src/test022_half_life.py` & `opengate-10.0b8/opengate/tests/src/test022_half_life.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test022_half_life_helpers.py` & `opengate-10.0b8/opengate/tests/src/test022_half_life_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test022_half_life_ion.py` & `opengate-10.0b8/opengate/tests/src/test022_half_life_ion.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,29 +66,29 @@
     sim.physics_manager.physics_list_name = "QGSP_BERT_EMZ"
     sim.physics_manager.enable_decay = True
     sim.physics_manager.global_production_cuts.all = (
         1 * mm
     )  # all means: proton, electron, positron, gamma
 
     # activity
-    activity_Bq = 4000
-    half_life = 5.0 * sec
+    activity_Bq = 4000 * Bq
+    half_life = 5 * sec
     lifetime = half_life / math.log(2.0)
 
     # "hole" in the timeline to check if no particle are emitted at this moment
     sim.run_timing_intervals = [[0 * sec, 12 * sec], [13 * sec, 20 * sec]]
 
     # source #1
     source1 = sim.add_source("GenericSource", "source1")
     source1.mother = "waterbox1"
     source1.particle = "ion 49 111"  # In111 171 keV and 245 keV
     source1.position.type = "sphere"
     source1.position.radius = 1 * mm
     source1.direction.type = "iso"
-    source1.activity = activity_Bq * Bq / sim.number_of_threads
+    source1.activity = activity_Bq / sim.number_of_threads
     source1.half_life = half_life
     # this is needed, but automatically done in GenericSource.py
     source1.user_particle_life_time = 0
     print()
     print(f"Source1 ac = {source1.activity / Bq} Bq")
     print(f"Source1 HL = {half_life / sec} sec")
 
@@ -97,15 +97,15 @@
     source2.mother = "waterbox2"
     source2.particle = "ion 49 111"  # In111 171 keV and 245 keV
     source2.position.type = "sphere"
     source2.position.radius = 1 * mm
     source2.position.translation = [0, 0, -3 * cm]
     source2.direction.type = "iso"
     source2.user_particle_life_time = lifetime
-    source2.n = activity_Bq / sim.number_of_threads * lifetime / sec
+    source2.n = activity_Bq / Bq / sim.number_of_threads * lifetime / sec
     print()
     print("Source2 n = ", source2.n)
     print(f"Source2 HL = {half_life / sec} sec")
     print(f"Source2 LT = {lifetime / sec} sec")
     print()
 
     # add stat actor
```

### Comparing `opengate-10.0b7/opengate/tests/src/test023_filters.py` & `opengate-10.0b8/opengate/tests/src/test023_filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,27 +44,29 @@
 
     # filter : keep e- only
     fp = sim.add_filter("ParticleFilter", "fp")
     fp.particle = "e-"
 
     # add dose actor
     dose1 = sim.add_actor("DoseActor", "dose1")
-    dose1.output = paths.output / "test023-edep.mhd"
+    dose1.output = paths.output / "test023.mhd"
     # dose1.output = paths.output_ref / 'test023-edep.mhd'
     dose1.mother = "waterbox"
     dose1.size = [100, 100, 100]
     dose1.spacing = [2 * mm, 2 * mm, 2 * mm]
     dose1.filters.append(fp)
 
     # add dose actor, without e- (to check)
     fe = sim.add_filter("ParticleFilter", "f")
     fe.particle = "e-"
     fe.policy = "discard"
+    print(dir(fe))
+
     dose2 = sim.add_actor("DoseActor", "dose2")
-    dose2.output = paths.output / "test023-noe-edep.mhd"
+    dose2.output = paths.output / "test023-noe.mhd"
     # dose2.output = paths.output_ref / "test023-noe-edep.mhd"
     dose2.mother = "waterbox"
     dose2.size = [100, 100, 100]
     dose2.spacing = [2 * mm, 2 * mm, 2 * mm]
     dose2.filters.append(fe)
 
     """fe = sim.add_filter("ParticleFilter", "f")
@@ -92,32 +94,34 @@
 
     # start simulation
     sim.run()
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     print(stat)
+    dose1 = sim.output.get_actor("dose1")
+    dose2 = sim.output.get_actor("dose2")
     # stat.write(paths.output_ref / 'test023_stats.txt')
 
     # tests
     stats_ref = utility.read_stat_file(paths.output_ref / "test023_stats.txt")
     is_ok = utility.assert_stats(stat, stats_ref, 0.8)
 
     print()
     is_ok = is_ok and utility.assert_images(
         paths.output_ref / "test023-edep.mhd",
-        dose1.output,
+        paths.output / dose1.user_info.output,
         stat,
         tolerance=50,
         sum_tolerance=4,
     )
 
     print()
     is_ok = is_ok and utility.assert_images(
         paths.output_ref / "test023-noe-edep.mhd",
-        dose2.output,
+        paths.output / dose2.user_info.output,
         stat,
         tolerance=40,
         sum_tolerance=2,
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test023_filters_attribute.py` & `opengate-10.0b8/opengate/tests/src/test023_filters_attribute.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test023_filters_attribute_bool.py` & `opengate-10.0b8/opengate/tests/src/test023_filters_attribute_bool.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test023_filters_iec_phantom.py` & `opengate-10.0b8/opengate/tests/src/test023_filters_iec_phantom.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,22 +76,23 @@
     sim.user_hook_after_init = check_production_cuts
 
     # start simulation
     sim.run(start_new_process=True)
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
+    dose = sim.output.get_actor("dose")
     # stat.write(paths.output_ref / 'test023_stats_iec_phantom.txt')
 
     # tests
     f = paths.output_ref / "test023_stats_iec_phantom.txt"
     stats_ref = utility.read_stat_file(f)
     is_ok = utility.assert_stats(stat, stats_ref, 0.12)
     is_ok = is_ok and utility.assert_images(
         paths.output_ref / "test023_iec_phantom.mhd",
-        paths.output / "test023_iec_phantom.mhd",
+        paths.output / dose.user_info.output,
         stat,
         sum_tolerance=28,
         tolerance=102,
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test023_filters_material.py` & `opengate-10.0b8/opengate/tests/src/test023_filters_material.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     f = sim.add_filter("ParticleFilter", "f")
     f.particle = "gamma"
     fp = sim.add_filter("ParticleFilter", "fp")
     fp.particle = "e-"
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = paths.output / "test023-edep.mhd"
+    dose.output = paths.output / "test023.mhd"
     # dose.output = paths.output_ref / "test023-edep.mhd"
     dose.mother = "waterbox"
     dose.size = [100, 100, 100]
     dose.spacing = [2 * mm, 2 * mm, 2 * mm]
     dose.filters.append(fp)
 
     # add stat actor
@@ -81,14 +81,16 @@
 
     # start simulation
     sim.run(start_new_process=True)
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     # print(stat)
+
+    dose = sim.output.get_actor("dose")
     f = paths.output_ref / "test023_stats_iec_mat.txt"
     # stat.write(f)
 
     stat2 = sim.output.get_actor("Stats2")
     # print(stat2)
     f2 = paths.output_ref / "test023_stats_iec_mat_e.txt"
     # stat2.write(f2)
@@ -101,14 +103,14 @@
     print()
     gate.exception.warning(f"Stats filter 2")
     stats_ref = utility.read_stat_file(f2)
     is_ok = utility.assert_stats(stat2, stats_ref, 0.07) and is_ok
 
     is_ok = is_ok and utility.assert_images(
         paths.output_ref / "test023-edep.mhd",
-        paths.output / "test023-edep.mhd",
+        paths.output / dose.user_info.output,
         stat,
         sum_tolerance=3,
         tolerance=50,
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test024_py_actor_wip.py` & `opengate-10.0b8/opengate/tests/src/test024_py_actor_wip.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test025_hits_collection_helpers.py` & `opengate-10.0b8/opengate/tests/src/test025_hits_collection_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test026_simple_signal.py` & `opengate-10.0b8/opengate/tests/src/test026_simple_signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
     sim.g4_verbose_level = 1
     sim.visu = False
     sim.random_engine = "MersenneTwister"
-    sim.random_seed = "auto"
+    sim.random_seed = 987654321
 
     print(sim)
 
     m = gate.g4_units.m
     cm = gate.g4_units.cm
     keV = gate.g4_units.keV
     mm = gate.g4_units.mm
```

### Comparing `opengate-10.0b7/opengate/tests/src/test027_fake_spect_mt.py` & `opengate-10.0b8/opengate/tests/src/test027_fake_spect_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_1_colli.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_1_colli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 from opengate.tests import utility
 
 if __name__ == "__main__":
     paths = utility.get_default_test_paths(__file__, "gate_test028_ge_nm670_spect")
 
     # create the simulation
     sim = gate.Simulation()
@@ -26,15 +26,15 @@
     kBq = 1000 * Bq
 
     # world size
     sim.world.size = [1 * m, 1 * m, 1 * m]
     sim.world.material = "G4_AIR"
 
     # spect head (debug mode = very small collimator)
-    spect, crystal = gate_spect.add_ge_nm67_spect_head(sim, "spect", debug=False)
+    spect, colli, crystal = gate_spect.add_spect_head(sim, "spect", debug=False)
     psd = 6.11 * cm
     spect.translation = [0, 0, -(20 * cm + psd)]
 
     # waterbox
     waterbox = sim.add_volume("Box", "waterbox")
     waterbox.size = [15 * cm, 15 * cm, 15 * cm]
     waterbox.material = "G4_WATER"
```

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_1_colli_visu.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_1_colli_visu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 from opengate.tests import utility
 
 if __name__ == "__main__":
     paths = utility.get_default_test_paths(__file__, "gate_test028_ge_nm670_spect")
 
     # create the simulation
     sim = gate.Simulation()
@@ -28,15 +28,15 @@
     kBq = 1000 * Bq
 
     # world size
     sim.world.size = [1 * m, 1 * m, 1 * m]
     sim.world.material = "G4_AIR"
 
     # spect head (debug mode = very small collimator)
-    spect, crystal = gate_spect.add_ge_nm67_spect_head(sim, "spect", debug=True)
+    spect, crystal = gate_spect.add_spect_head(sim, "spect", debug=True)
     psd = 6.11 * cm
     spect.translation = [0, 0, -(20 * cm + psd)]
 
     # waterbox
     waterbox = sim.add_volume("Box", "waterbox")
     waterbox.size = [15 * cm, 15 * cm, 15 * cm]
     waterbox.material = "G4_WATER"
```

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_2_helpers.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_2_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import itk
 import numpy as np
 
 import opengate as gate
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 from opengate.userhooks import check_production_cuts
 from opengate.tests import utility
 
 
 def create_spect_simu(sim, paths, number_of_threads=1):
     # main options
     sim.g4_verbose = False
@@ -26,15 +26,15 @@
     kBq = 1000 * Bq
 
     # world size
     sim.world.size = [1 * m, 1 * m, 1 * m]
     sim.world.material = "G4_AIR"
 
     # spect head (debug mode = very small collimator)
-    spect, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect, colli, crystal = gate_spect.add_spect_head(
         sim, "spect", collimator_type=False, debug=False
     )
     psd = 6.11 * cm
     spect.translation = [0, 0, -(20 * cm + psd)]
 
     # waterbox
     waterbox = sim.add_volume("Box", "waterbox")
```

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_2_hits.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_2_hits.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_2_hits_mt.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_2_hits_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_3_proj.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_3_proj.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_3_proj_blur.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_3_proj_blur.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_3_proj_mt.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_3_proj_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     )
 
     # go
     sim.run()
 
     # check
     is_ok = test028.compare_result(
-        sim.output, proj, "test028_aa_skip_events.png", sum_tolerance=17
+        sim.output, proj, "test028_aa_skip_events.png", sum_tolerance=17.5
     )
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se_mt.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_ze.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_ze.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_helpers.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
 from opengate.tests import utility
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import itk
 import numpy as np
 
 paths = utility.get_default_test_paths(__file__, "gate_test028_ge_nm670_spect")
 
 
 def create_spect_simu(
@@ -35,15 +35,15 @@
     kBq = 1000 * Bq
 
     # world size
     sim.world.size = [1 * m, 1 * m, 1 * m]
     sim.world.material = "G4_AIR"
 
     # spect head (debug mode = very small collimator)
-    spect, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect, colli, crystal = gate_spect.add_spect_head(
         sim, "spect", collimator_type="lehr", debug=False
     )
 
     # waterbox
     waterbox = sim.add_volume("Box", "waterbox")
     waterbox.size = [15 * cm, 15 * cm, 15 * cm]
     waterbox.material = "G4_WATER"
```

### Comparing `opengate-10.0b7/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_noaa.py` & `opengate-10.0b8/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_noaa.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test029_volume_time_rotation_1.py` & `opengate-10.0b8/opengate/tests/src/test029_volume_time_rotation_1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test029_volume_time_rotation_1_process.py` & `opengate-10.0b8/opengate/tests/src/test029_volume_time_rotation_1_process.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test029_volume_time_rotation_2.py` & `opengate-10.0b8/opengate/tests/src/test029_volume_time_rotation_2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test029_volume_time_rotation_helpers.py` & `opengate-10.0b8/opengate/tests/src/test029_volume_time_rotation_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import opengate.contrib.phantoms.nemaiec as gate_iec
 from scipy.spatial.transform import Rotation
 from opengate.tests import utility
 
 paths = utility.get_default_test_paths(
     __file__, "gate_test029_volume_time_rotation", "test029"
 )
@@ -33,15 +33,15 @@
     sim.user_hook_after_init = gate.userhooks.check_production_cuts
 
     # world size
     sim.world.size = [2 * m, 2 * m, 2 * m]
     sim.world.material = "G4_AIR"
 
     # spect head (no collimator)
-    spect, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect, colli, crystal = gate_spect.add_spect_head(
         sim, "spect", collimator_type=False, debug=False
     )
     # will be overriden by MotionActor
     """initial_rot = Rotation.from_euler("X", 90, degrees=True)
     t, rot = gate.geometry.utility.get_transform_orbiting([0, 25 * cm, 0], "Z", 0)
     rot = Rotation.from_matrix(rot)
     spect.translation = t
```

### Comparing `opengate-10.0b7/opengate/tests/src/test030_dose_motion.py` & `opengate-10.0b8/opengate/tests/src/test030_dose_motion.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     source.position.radius = 5 * mm
     source.direction.type = "momentum"
     source.direction.momentum = [0, 0, 1]
     source.activity = 30000 * Bq
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = paths.output / "test030-edep.mhd"
+    dose.output = paths.output / "test030.mhd"
     dose.mother = "waterbox"
     dose.size = [99, 99, 99]
     mm = gate.g4_units.mm
     dose.spacing = [2 * mm, 2 * mm, 2 * mm]
     dose.translation = [2 * mm, 3 * mm, -2 * mm]
     dose.uncertainty = True
 
@@ -109,32 +109,32 @@
     print(dose)
 
     # tests
     stats_ref = utility.read_stat_file(paths.output_ref / "stats030.txt")
     is_ok = utility.assert_stats(stat, stats_ref, 0.11)
 
     print()
+
     gate.exception.warning("Difference for EDEP")
     is_ok = (
         utility.assert_images(
             paths.output_ref / "test030-edep.mhd",
-            paths.output / "test030-edep.mhd",
+            dose.user_info.output,
             stat,
             tolerance=30,
             ignore_value=0,
         )
         and is_ok
     )
 
     print("\nDifference for uncertainty")
     is_ok = (
         utility.assert_images(
             paths.output_ref / "test030-edep_uncertainty.mhd",
-            paths.output / "test030-edep_uncertainty.mhd",
+            dose.user_info.output_uncertainty,
             stat,
             tolerance=15,
             ignore_value=1,
         )
-        and is_ok
-    )
+    ) and is_ok
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test031_beta_plus_spectrum.py` & `opengate-10.0b8/opengate/tests/src/test031_beta_plus_spectrum.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test032_create_voxelized_volume.py` & `opengate-10.0b8/opengate/tests/src/test032_create_voxelized_volume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test032_voxel_vs_volume.py` & `opengate-10.0b8/opengate/tests/src/test032_voxel_vs_volume.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     # add stat actor
     stats = sim.add_actor("SimulationStatisticsActor", "stats")
     stats.track_types_flag = True
 
     # add dose actor
     for i in range(1, 3):
         dose = sim.add_actor("DoseActor", f"dose{i}")
-        dose.output = paths.output / f"test032_iec{i}_edep.mhd"
+        dose.output = paths.output / f"test032_iec{i}.mhd"
         dose.mother = f"iec{i}"
         dose.size = [100, 100, 100]
         dose.spacing = [2 * mm, 2 * mm, 2 * mm]
         # translate the iec1 to have the exact same dose origin
         # (only needed to perform the assert_image test)
         if i == 1:
             dose.translation = [0 * mm, 35 * mm, 0 * mm]
@@ -132,18 +132,20 @@
 
     # initialize & start
     sim.run()
 
     # stats
     stats = sim.output.get_actor("stats")
     print(stats)
-
+    dose1 = sim.output.get_actor("dose1")
+    dose2 = sim.output.get_actor("dose2")
     # compare edep map
+
     is_ok = utility.assert_images(
-        paths.output / "test032_iec1_edep.mhd",
-        paths.output / "test032_iec2_edep.mhd",
+        dose1.user_info.output,
+        dose2.user_info.output,
         stats,
         tolerance=87,
         axis="x",
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test032_voxelized_volume_source.py` & `opengate-10.0b8/opengate/tests/src/test032_voxelized_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     is_ok = True
 
     # test 1 = 10mm and with shell
     f1 = paths.output / "iec_10mm.mhd"
     f2 = paths.output / "iec_source_10mm.mhd"
     path_voxelize_script = os.path.join(
-        os.path.dirname(__file__), "..", "..", "bin", "voxelize_iec_phantom"
+        os.path.dirname(__file__), "..", "..", "bin", "voxelize_iec_phantom.py"
     )
     cmd = (
         f"python {path_voxelize_script} -o {f1} "
         f"-s 10 "
         f"--output_source {f2} "
         f"-a 666 555 444 333 222 111 "
     )
```

### Comparing `opengate-10.0b7/opengate/tests/src/test033_rotation_spect_aa_helpers.py` & `opengate-10.0b8/opengate/tests/src/test033_rotation_spect_aa_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 from opengate.tests import utility
 from opengate.element import copy_user_info
 
 paths = utility.get_default_test_paths(__file__, "", "test033")
 
 
 def create_test(sim, nb_thread=1):
@@ -40,23 +40,23 @@
 
     # world size
     world = sim.world
     world.size = [1.5 * m, 1.5 * m, 1.5 * m]
     world.material = "G4_AIR"
 
     # spect head (debug mode = very small collimator)
-    spect1, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect1, colli, crystal = gate_spect.add_spect_head(
         sim, "spect1", collimator_type="lehr", debug=sim.visu
     )
     spect1.translation, spect1.rotation = gate.geometry.utility.get_transform_orbiting(
         p, "x", 180
     )
 
     # spect head (debug mode = very small collimator)
-    spect2, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect2, colli, crystal = gate_spect.add_spect_head(
         sim, "spect2", collimator_type="lehr", debug=sim.visu
     )
     spect2.translation, spect2.rotation = gate.geometry.utility.get_transform_orbiting(
         p, "x", 0
     )
 
     # physic list
@@ -93,19 +93,19 @@
     sources.append(source2)
 
     # add stat actor
     stat = sim.add_actor("SimulationStatisticsActor", "Stats")
     stat.output = paths.output / "test033_stats.txt"
 
     # add default digitizer (it is easy to change parameters if needed)
-    proj = gate_spect.add_simplified_digitizer_Tc99m(
+    proj = gate_spect.add_simplified_digitizer_tc99m(
         sim, "spect1_crystal", paths.output / "test033_proj_1.mhd"
     )
     proj.origin_as_image_center = False
-    proj = gate_spect.add_simplified_digitizer_Tc99m(
+    proj = gate_spect.add_simplified_digitizer_tc99m(
         sim, "spect2_crystal", paths.output / "test033_proj_2.mhd"
     )
     proj.origin_as_image_center = False
 
     # motion of the spect, create also the run time interval
     heads = [spect1, spect2]
```

### Comparing `opengate-10.0b7/opengate/tests/src/test033_rotation_spect_aa_se.py` & `opengate-10.0b8/opengate/tests/src/test033_rotation_spect_aa_se.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test033_rotation_spect_aa_se_mt.py` & `opengate-10.0b8/opengate/tests/src/test033_rotation_spect_aa_se_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test033_rotation_spect_aa_ze.py` & `opengate-10.0b8/opengate/tests/src/test033_rotation_spect_aa_ze.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test033_rotation_spect_noaa.py` & `opengate-10.0b8/opengate/tests/src/test033_rotation_spect_noaa.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test033_rotation_spect_noaa_mt.py` & `opengate-10.0b8/opengate/tests/src/test033_rotation_spect_noaa_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test034_gan_phsp_linac.py` & `opengate-10.0b8/opengate/tests/src/test034_gan_phsp_linac.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     s.track_types_flag = True
 
     # PhaseSpace Actor
     dose = sim.add_actor("DoseActor", "dose")
     dose.mother = waterbox.name
     dose.spacing = [4 * mm, 4 * mm, 4 * mm]
     dose.size = [75, 75, 75]
-    dose.output = paths.output / "test034_edep.mhd"
+    dose.output = paths.output / "test034.mhd"
     dose.uncertainty = True
 
     """
     Dont know why similar to hit_type == post while in Gate
     this is hit_type = random ?
     """
     dose.hit_type = "post"
@@ -111,20 +111,21 @@
     gate.exception.warning(f"Check stats")
     stats = sim.output.get_actor("Stats")
     print(stats)
     stats_ref = utility.read_stat_file(paths.gate / "stats.txt")
     is_ok = utility.assert_stats(stats, stats_ref, 0.10)
 
     gate.exception.warning(f"Check dose")
-    h = sim.output.get_actor("dose")
-    print(h)
+    dose = sim.output.get_actor("dose")
+    print(dose)
+
     is_ok = (
         utility.assert_images(
             paths.gate / "dose-Edep.mhd",
-            dose.output,
+            paths.output / dose.user_info.output,
             stats,
             tolerance=58,
             ignore_value=0,
         )
         and is_ok
     )
```

### Comparing `opengate-10.0b7/opengate/tests/src/test035_dose_rate.py` & `opengate-10.0b8/opengate/tests/src/test035_dose_rate.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test036_adder_depth_helpers.py` & `opengate-10.0b8/opengate/tests/src/test036_adder_depth_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test037_digi_attributes_list.py` & `opengate-10.0b8/opengate/tests/src/test037_digi_attributes_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,13 +16,13 @@
     print(
         f"Types are: 3 (ThreeVector), D (double), S (string), I (int), U (unique volume ID)"
     )
     for a in nlist:
         att = am.GetDigiAttributeByName(a)
         print(att.GetDigiAttributeName(), att.GetDigiAttributeType())
 
-    n = 44
+    n = 47
     is_ok = len(nlist) == n
 
     utility.print_test(is_ok, f"Done for {n} attributes.")
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test037_pet_hits_singles_1.py` & `opengate-10.0b8/opengate/tests/src/test037_pet_hits_singles_1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test037_pet_hits_singles_1_visu.py` & `opengate-10.0b8/opengate/tests/src/test037_pet_hits_singles_1_visu.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test037_pet_hits_singles_2.py` & `opengate-10.0b8/opengate/tests/src/test037_pet_hits_singles_2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test037_pet_hits_singles_helpers.py` & `opengate-10.0b8/opengate/tests/src/test037_pet_hits_singles_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     world.material = "G4_AIR"
 
     # add a PET VEREOS
     sim.volume_manager.add_material_database(paths.gate_data / "GateMaterials_pet.db")
     if not debug:
         pet = pet_vereos.add_pet(sim, "pet", create_housing=True, create_mat=create_mat)
     else:
-        pet = pet_vereos.add_pet_debug(
-            sim, "pet", create_housing=True, create_mat=create_mat
+        pet = pet_vereos.add_pet(
+            sim, "pet", create_housing=True, create_mat=create_mat, debug=True
         )
 
     # add table
     bed = pet_vereos.add_table(sim, "pet")
 
     # add NECR phantom
     phantom = phantom_necr.add_necr_phantom(sim, "phantom")
```

### Comparing `opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_aa.py` & `opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_aa.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_helpers.py` & `opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import uproot
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 import opengate as gate
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import opengate.contrib.phantoms.nemaiec as gate_iec
 import gatetools.phsp as phsp
 from opengate.tests import utility
 
 
 class GANTest:
     def __init__(self, spheres_activity_ratio, spheres_centers, spheres_radius, rs):
@@ -78,15 +78,15 @@
     phase_space_sphere.color = [1, 1, 1, 1]
     phase_space_sphere.material = "G4_AIR"
 
     # spect head
     distance = 30 * cm
     psd = 6.11 * cm
     p = [0, 0, -(distance + psd)]
-    spect1, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect1, colli, crystal = gate_spect.add_spect_head(
         sim, "spect1", collimator_type=colli, debug=sim.visu
     )
     spect1.translation, spect1.rotation = gate.geometry.utility.get_transform_orbiting(
         p, "x", 180
     )
 
     # physic list
@@ -165,15 +165,15 @@
     # gsource.direction.acceptance_angle.intersection_flag = True
 
     # add stat actor
     stat = sim.add_actor("SimulationStatisticsActor", "Stats")
     stat.output = paths.output / "test038_gan_stats.txt"
 
     # add default digitizer (it is easy to change parameters if needed)
-    gate_spect.add_simplified_digitizer_Tc99m(
+    gate_spect.add_simplified_digitizer_tc99m(
         sim, "spect1_crystal", paths.output / "test038_gan_proj.mhd"
     )
     # gate_spect.add_ge_nm670_spect_simplified_digitizer(sim, 'spect2_crystal', paths.output / 'test033_proj_2.mhd')
     singles_actor = sim.get_actor_user_info(f"Singles_spect1_crystal")
     singles_actor.output = paths.output / "test038_gan_singles.root"
 
     # motion of the spect, create also the run time interval
```

### Comparing `opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_mt.py` & `opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_se.py` & `opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_se.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_gan_ze.py` & `opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_gan_ze.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test038_gan_phsp_spect_training_dataset.py` & `opengate-10.0b8/opengate/tests/src/test038_gan_phsp_spect_training_dataset.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test039_hits_memory_check_helpers.py` & `opengate-10.0b8/opengate/tests/src/test039_hits_memory_check_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
     sim.visu = False
     sim.number_of_threads = nb_threads
-    sim.random_seed = "auto"  # 123456
+    sim.random_seed = 987654321  # 123456
     sim.check_volumes_overlap = False
 
     # units
     m = gate.g4_units.m
     cm = gate.g4_units.cm
     keV = gate.g4_units.keV
     mm = gate.g4_units.mm
```

### Comparing `opengate-10.0b7/opengate/tests/src/test040_gan_phsp_pet_aref.py` & `opengate-10.0b8/opengate/tests/src/test040_gan_phsp_pet_aref.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,14 @@
     gate.exception.warning(f"Check stats")
     stats = sim.output.get_actor("Stats")
     print(stats)
     stats_ref = utility.read_stat_file(paths.output_ref / "test040_ref_stats.txt")
     is_ok = utility.assert_stats(stats, stats_ref, 0.01)
 
     # 426760*2*0.8883814158496728 = 758251.3
-
     phsp = sim.output.get_actor("phsp")
     ref = 9523
     ae = phsp.fNumberOfAbsorbedEvents
     err = abs(ae - ref) / ref
     tol = 0.055
     is_ok = err < tol and is_ok
     utility.print_test(
```

### Comparing `opengate-10.0b7/opengate/tests/src/test040_gan_phsp_pet_gan.py` & `opengate-10.0b8/opengate/tests/src/test040_gan_phsp_pet_gan.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test040_gan_phsp_pet_training_dataset.py` & `opengate-10.0b8/opengate/tests/src/test040_gan_phsp_pet_training_dataset.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test041_dose_actor.py` & `opengate-10.0b8/opengate/tests/src/test054_parallel_geometry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,135 +1,133 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+from scipy.spatial.transform import Rotation
 import opengate as gate
 from opengate.tests import utility
 
 if __name__ == "__main__":
-    paths = utility.get_default_test_paths(__file__, "gate_test008_dose_actor")
+    paths = utility.get_default_test_paths(__file__, None, "test054")
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
-    sim.g4_verbose = False
-    sim.g4_verbose_level = 1
+    # sim.visu_type = "vrml"
     sim.visu = False
-    sim.random_seed = 123456
+    sim.check_volumes_overlap = True
+    sim.number_of_threads = 1
+    sim.random_seed = 654923
+
+    sim.physics_manager.physics_list_name = "G4EmStandardPhysics_option4"
+
+    # add a material database
+    sim.volume_manager.add_material_database(paths.data / "GateMaterials.db")
 
     # units
     m = gate.g4_units.m
     cm = gate.g4_units.cm
-    mm = gate.g4_units.mm
     MeV = gate.g4_units.MeV
     Bq = gate.g4_units.Bq
+    mm = gate.g4_units.mm
 
     #  change world size
     world = sim.world
-    world.size = [0.5 * m, 0.5 * m, 0.5 * m]
+    world.size = [1 * m, 1 * m, 1 * m]
+    world.material = "G4_AIR"
 
-    # waterbox
-    waterbox = sim.add_volume("Box", "waterbox")
-    waterbox.size = [10 * cm, 10 * cm, 10 * cm]
-    waterbox.material = "G4_WATER"
-    waterbox.color = [0, 0, 1, 1]
-
-    # lungbox
-    lungbox = sim.add_volume("Box", "lungbox")
-    lungbox.mother = waterbox.name
-    lungbox.size = [10 * cm, 10 * cm, 4 * cm]
-    lungbox.translation = [0 * cm, 0 * cm, 2.5 * cm]
-    lungbox.material = "G4_LUNG_ICRP"
-    lungbox.color = [0, 1, 1, 1]
-
-    # bonebox
-    bonebox = sim.add_volume("Box", "bonebox")
-    bonebox.mother = waterbox.name
-    bonebox.size = [10 * cm, 10 * cm, 4 * cm]
-    bonebox.translation = [0 * cm, 0 * cm, -2.5 * cm]
-    bonebox.material = "G4_BONE_CORTICAL_ICRP"
-    bonebox.color = [1, 0, 0, 1]
-
-    # physics
-    sim.physics_manager.physics_list_name = "QGSP_BERT_EMV"
-    sim.physics_manager.global_production_cuts.all = 1 * mm
-
-    # default source for tests
-    source = sim.add_source("GenericSource", "mysource")
-    source.energy.mono = 115 * MeV
-    source.particle = "proton"
-    source.position.type = "disc"
-    source.position.radius = 1 * cm
-    source.position.translation = [0, 0, -80 * mm]
+    fake = sim.add_volume("Box", "fake")
+    fake.size = [40 * cm, 40 * cm, 40 * cm]
+    fake.material = "G4_AIR"
+    fake.color = [1, 0, 1, 1]
+
+    # image
+    patient = sim.add_volume("Image", "patient")
+    patient.mother = fake.name
+    patient.image = paths.data / "patient-40mm.mhd"
+    patient.material = "G4_AIR"  # material used by default
+    patient.voxel_materials = [
+        [-2000, -900, "G4_AIR"],
+        [-900, -100, "Lung"],
+        [-100, 0, "G4_ADIPOSE_TISSUE_ICRP"],
+        [0, 300, "G4_TISSUE_SOFT_ICRP"],
+        [300, 800, "G4_B-100_BONE"],
+        [800, 6000, "G4_BONE_COMPACT_ICRU"],
+    ]
+
+    # create two other parallel worlds
+    sim.add_parallel_world("world2")
+    sim.add_parallel_world("world3")
+
+    # detector in w2 (on top of world)
+    det = sim.add_volume("Box", "detector")
+    det.mother = "world2"
+    det.material = "G4_GLASS_LEAD"
+    det.size = [400 * mm, 400 * mm, 2 * mm]
+    det.translation = [0, 0, 200 * mm]
+    det.rotation = Rotation.from_euler("x", 40, degrees=True).as_matrix()
+    det.color = [1, 0, 0, 1]
+
+    # detector in w3 (on top of w2)
+    det2 = sim.add_volume("Box", "detector2")
+    det2.mother = "world3"
+    det2.material = "G4_GLASS_LEAD"  # set 'None' if this volume should be transparent
+    det2.size = [400 * mm, 400 * mm, 2 * mm]
+    det2.translation = [0, 0, 200 * mm]
+    det2.rotation = Rotation.from_euler("x", -40, degrees=True).as_matrix()
+    det2.color = [1, 0, 0, 1]
+
+    # source
+    source = sim.add_source("GenericSource", "source")
+    source.energy.mono = 0.1 * MeV
+    source.particle = "gamma"
+    source.position.type = "box"
+    source.position.size = [1 * mm, 200 * mm, 1 * mm]
+    source.position.translation = [0, 0, 0 * cm]
+    source.activity = 10000 * Bq / sim.number_of_threads
     source.direction.type = "momentum"
     source.direction.momentum = [0, 0, 1]
-    source.activity = 5000 * Bq
 
-    # add dose actor
-    dose = sim.add_actor("DoseActor", "dose")
-    dose.output = paths.output / "test041-edep.mhd"
-    dose.mother = "waterbox"
-    dose.size = [10, 10, 50]
-    mm = gate.g4_units.mm
-    ts = [200 * mm, 200 * mm, 200 * mm]
-    dose.spacing = [x / y for x, y in zip(ts, dose.size)]
-    print(dose.spacing)
-    dose.uncertainty = True
-    dose.gray = True
-    dose.hit_type = "random"
+    # add phsp actor detector 1 (overlap!)
+    phsp = sim.add_actor("PhaseSpaceActor", "phsp")
+    phsp.output = paths.output / "test054.root"
+    phsp.mother = det.name
+    phsp.attributes = [
+        "KineticEnergy",
+        "PrePosition",
+    ]
 
     # add stat actor
-    s = sim.add_actor("SimulationStatisticsActor", "Stats")
-    s.track_types_flag = True
+    stats = sim.add_actor("SimulationStatisticsActor", "Stats")
+    stats.track_types_flag = True
+
+    # print
+    print("Geometry trees: ")
+    print(sim.volume_manager.dump_volume_tree())
 
     # start simulation
-    sim.run(start_new_process=True)
+    sim.run(True)
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     print(stat)
+    d = sim.output.get_actor("phsp")
+    print(d)
 
-    dose = sim.output.get_actor("dose")
-    print(dose)
-
-    # tests
-    gate.exception.warning("Tests stats file")
-    stats_ref = utility.read_stat_file(paths.gate_output / "stat2.txt")
-    is_ok = utility.assert_stats(stat, stats_ref, 0.10)
-
-    gate.exception.warning("\nDifference for EDEP")
-    is_ok = (
-        utility.assert_images(
-            paths.gate_output / "output2-Edep.mhd",
-            paths.output / "test041-edep.mhd",
-            stat,
-            tolerance=10,
-            ignore_value=0,
-        )
-        and is_ok
-    )
-
-    gate.exception.warning("\nDifference for uncertainty")
-    is_ok = (
-        utility.assert_images(
-            paths.gate_output / "output2-Edep-Uncertainty.mhd",
-            paths.output / "test041-edep_uncertainty.mhd",
-            stat,
-            tolerance=30,
-            ignore_value=1,
-        )
-        and is_ok
+    keys = ["KineticEnergy", "PrePosition_X", "PrePosition_Y", "PrePosition_Z"]
+    tols = [0.01, 2.6, 1.8, 1.7]
+    ref = paths.output_ref / "test054_ref.root"
+    f = paths.output / "test054.png"
+    is_ok = utility.compare_root3(
+        ref,
+        phsp.output,
+        "phsp",
+        "phsp",
+        keys,
+        keys,
+        tols,
+        None,
+        None,
+        f,
+        hits_tol=6.1,
     )
-
-    gate.exception.warning("\nDifference for dose in Gray")
-    is_ok = (
-        utility.assert_images(
-            paths.gate_output / "output2-Dose.mhd",
-            paths.output / "test041-edep_dose.mhd",
-            stat,
-            tolerance=10,
-            ignore_value=0,
-        )
-        and is_ok
-    )
-
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test042_gauss_gps.py` & `opengate-10.0b8/opengate/tests/src/test042_gauss_gps.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,42 +120,42 @@
     is_ok = utility.assert_stats(stat, stats_ref, 0.14)
 
     print()
     gate.exception.warning("Difference for EDEP XZ")
     is_ok = (
         utility.assert_images(
             paths.gate_output / "lateral_xz_Protons_40MeV_sourceShapeGaussian-Edep.mhd",
-            sim.output.get_actor("doseInXZ").user_info.output,
+            paths.output / sim.output.get_actor("doseInXZ").user_info.output,
             stat,
             tolerance=10,
             ignore_value=0,
         )
         and is_ok
     )
 
     print()
     gate.exception.warning("Difference for EDEP XY")
     is_ok = (
         utility.assert_images(
             paths.gate_output / "lateral_xy_Protons_40MeV_sourceShapeGaussian-Edep.mhd",
-            sim.output.get_actor("doseInXY").user_info.output,
+            paths.output / sim.output.get_actor("doseInXY").user_info.output,
             stat,
             tolerance=10,
             ignore_value=0,
             axis="y",
         )
         and is_ok
     )
 
     print()
     gate.exception.warning("Difference for EDEP YZ")
     is_ok = (
         utility.assert_images(
             paths.gate_output / "lateral_yz_Protons_40MeV_sourceShapeGaussian-Edep.mhd",
-            sim.output.get_actor("doseInYZ").user_info.output,
+            paths.output / sim.output.get_actor("doseInYZ").user_info.output,
             stat,
             tolerance=30,
             ignore_value=0,
             axis="y",
         )
         and is_ok
     )
```

### Comparing `opengate-10.0b7/opengate/tests/src/test043_distances.py` & `opengate-10.0b8/opengate/tests/src/test043_distances.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import math
 import opengate as gate
 import test043_garf_helpers as test43
 from opengate.tests import utility
 
 
 if __name__ == "__main__":
@@ -30,30 +30,30 @@
     test43.sim_set_world(sim)
 
     # distance
     spect_translation = 50 * cm
     debug = True
 
     # spect head n°1
-    spect1, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect1, colli, crystal = gate_spect.add_spect_head(
         sim, "spect_lehr", "lehr", debug=debug
     )
     spect1.translation = [0, 0, -spect_translation]
 
     # spect head n°2
-    spect2, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect2, colli, crystal = gate_spect.add_spect_head(
         sim, "spect_megp", "megp", debug=debug
     )
     p = [0, 0, -spect_translation]
     itr, irot = gate.geometry.utility.get_transform_orbiting(p, "x", 180)
     spect2.translation = itr
     spect2.rotation = irot
 
     # spect head n°3
-    spect3, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect3, colli, crystal = gate_spect.add_spect_head(
         sim, "spect_hegp", "hegp", debug=debug
     )
     p = [0, 0, -spect_translation]
     itr, irot = gate.geometry.utility.get_transform_orbiting(p, "x", 90)
     spect3.translation = itr
     spect3.rotation = irot
```

### Comparing `opengate-10.0b7/opengate/tests/src/test043_garf.py` & `opengate-10.0b8/opengate/tests/src/test043_garf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import itk
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import opengate as gate
 import test043_garf_helpers as test43
 from opengate.tests import utility
 
 if __name__ == "__main__":
     # create the simulation
     sim = gate.Simulation()
@@ -36,15 +36,15 @@
         test43.paths.gate_data / "GateMaterials.db"
     )
 
     # init world
     test43.sim_set_world(sim)
 
     # fake spect head
-    head = gate_spect.add_ge_nm67_fake_spect_head(sim, "spect")
+    head = gate_spect.add_fake_spect_head(sim, "spect")
     head.translation = [0, 0, -15 * cm]
 
     # detector input plane (+ 1nm to avoid overlap)
     pos, crystal_dist, psd = gate_spect.get_plane_position_and_distance_to_crystal(
         "lehr"
     )
     pos += 1 * nm
```

### Comparing `opengate-10.0b7/opengate/tests/src/test043_garf_analog.py` & `opengate-10.0b8/opengate/tests/src/test043_garf_analog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import itk
 import numpy as np
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import opengate as gate
 import test043_garf_helpers as test43
 from opengate.tests import utility
 
 
 if __name__ == "__main__":
     # create the simulation
@@ -29,15 +29,15 @@
 
     activity = 1e6 * Bq / sim.number_of_threads
 
     # world
     test43.sim_set_world(sim)
 
     # spect head
-    spect, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect, colli, crystal = gate_spect.add_spect_head(
         sim, "spect", collimator_type=colli, debug=sim.visu
     )
     spect.translation = [0, 0, -15 * cm]
     crystal_name = f"{spect.name}_crystal"
 
     # physics
     test43.sim_phys(sim)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test043_garf_helpers.py` & `opengate-10.0b8/opengate/tests/src/test043_garf_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 from opengate.tests import utility
 
 paths = utility.get_default_test_paths(__file__, "gate_test043_garf")
 
 m = gate.g4_units.m
 cm = gate.g4_units.cm
 mm = gate.g4_units.mm
@@ -102,15 +102,15 @@
     # add a material database
     sim.volume_manager.add_material_database(paths.gate_data / "GateMaterials.db")
 
     # init world
     sim_set_world(sim)
 
     # fake spect head
-    head = gate_spect.add_ge_nm67_fake_spect_head(sim, "spect")
+    head = gate_spect.add_fake_spect_head(sim, "spect")
     head.translation = [0, 0, -15 * cm]
 
     # detector input plane (+ 1nm to avoid overlap)
     pos, crystal_dist, psd = gate_spect.get_plane_position_and_distance_to_crystal(
         "lehr"
     )
     pos += 1 * nm
```

### Comparing `opengate-10.0b7/opengate/tests/src/test043_garf_mt.py` & `opengate-10.0b8/opengate/tests/src/test043_garf_mt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import itk
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import opengate as gate
 import test043_garf_helpers as test43
 from opengate.tests import utility
 
 if __name__ == "__main__":
     # create the simulation
     sim = gate.Simulation()
@@ -33,15 +33,15 @@
         test43.paths.gate_data / "GateMaterials.db"
     )
 
     # init world
     test43.sim_set_world(sim)
 
     # fake spect head
-    head = gate_spect.add_ge_nm67_fake_spect_head(sim, "spect")
+    head = gate_spect.add_fake_spect_head(sim, "spect")
     head.translation = [0, 0, -15 * cm]
 
     # detector input plane (+ 1nm to avoid overlap)
     pos, crystal_dist, psd = gate_spect.get_plane_position_and_distance_to_crystal(
         "lehr"
     )
     pos += 1 * nm
```

### Comparing `opengate-10.0b7/opengate/tests/src/test043_garf_training_dataset.py` & `opengate-10.0b8/opengate/tests/src/test043_garf_training_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import opengate as gate
 import test043_garf_helpers as test43
 from opengate.tests import utility
 
 if __name__ == "__main__":
     paths = utility.get_default_test_paths(__file__, "gate_test043_garf")
 
@@ -30,15 +30,15 @@
     # activity
     activity = 1e6 * Bq / sim.number_of_threads
 
     # world size
     test43.sim_set_world(sim)
 
     # spect head
-    spect, cystal = gate_spect.add_ge_nm67_spect_head(
+    spect, colli, cystal = gate_spect.add_spect_head(
         sim, "spect", collimator_type="lehr", debug=sim.visu
     )
     crystal_name = f"{spect.name}_crystal"
 
     # detector input plane
     pos, crystal_dist, psd = gate_spect.get_plane_position_and_distance_to_crystal(
         "lehr"
```

### Comparing `opengate-10.0b7/opengate/tests/src/test043_garf_training_dataset_full_wip.py` & `opengate-10.0b8/opengate/tests/src/test043_garf_training_dataset_full_wip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import opengate as gate
 import test043_garf_helpers as test43
 from opengate.tests import utility
 
 if __name__ == "__main__":
     paths = utility.get_default_test_paths(__file__, "gate_test043_garf_full")
 
@@ -30,15 +30,15 @@
     # activity
     activity = 1e9 * Bq / sim.number_of_threads
 
     # world size
     test43.sim_set_world(sim)
 
     # spect head
-    spect, cystal = gate_spect.add_ge_nm67_spect_head(
+    spect, cystal = gate_spect.add_spect_head(
         sim, "spect", collimator_type="lehr", debug=sim.visu
     )
     crystal_name = f"{spect.name}_crystal"
 
     # detector input plane
     pos, crystal_dist, psd = gate_spect.get_plane_position_and_distance_to_crystal(
         "lehr"
```

### Comparing `opengate-10.0b7/opengate/tests/src/test044_pbs.py` & `opengate-10.0b8/opengate/tests/src/test044_pbs_rot_transl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import os
 from scipy.spatial.transform import Rotation
+import os
 import opengate as gate
 from opengate.tests import utility
 
+
 if __name__ == "__main__":
-    paths = utility.get_default_test_paths(__file__, "gate_test044_pbs")
+    paths = utility.get_default_test_paths(__file__, "gate_test044_pbs_rot_transl")
 
     particle = "Carbon_"
     energy = "1440MeV_"
     beam_shape = "sourceShapePBS"
     folder = particle + energy + beam_shape
 
-    output_path = paths.output / "output_test044"
+    output_path = paths.output / "output_test044_rot_transl"
     ref_path = paths.gate_output
 
-    # for the for loop
+    # for for loop
     start = -500
     spacing = 100
     end = -start + spacing
     planePositionsV = range(start, end, spacing)
 
     # create the simulation
     sim = gate.Simulation()
@@ -51,15 +52,16 @@
     world = sim.world
     world.size = [600 * cm, 500 * cm, 500 * cm]
 
     # waterbox
     # translation and rotation like in the Gate macro
     waterbox = sim.add_volume("Box", "waterbox")
     waterbox.size = [10 * cm, 10 * cm, 100.2 * cm]
-    waterbox.translation = [0 * cm, 0 * cm, 50.1 * cm]
+    waterbox.rotation = Rotation.from_euler("y", 90, degrees=True).as_matrix()
+    waterbox.translation = [-50.1 * cm, 0 * cm, 0 * cm]
     waterbox.material = "Vacuum"
     waterbox.color = [0, 0, 1, 1]
 
     # Planes
     m = Rotation.identity().as_matrix()
 
     for i in planePositionsV:
@@ -74,20 +76,22 @@
     # physics
     sim.physics_manager.physics_list_name = "FTFP_INCLXX_EMZ"
     sim.physics_manager.global_production_cuts.all = 1000 * km
 
     # default source for tests (from test42)
     source = sim.add_source("IonPencilBeamSource", "mysource")
     source.energy.mono = 1440 * MeV
+    # source.energy.type = 'gauss'
     source.particle = "ion 6 12"  # carbon
     source.position.type = "disc"  # pos = Beam, shape = circle + sigma
-    source.position.translation = [0 * mm, 0 * mm, 0 * cm]
     # rotate the disc, equiv to : rot1 0 1 0 and rot2 0 0 1
+    source.position.rotation = Rotation.from_euler("y", -90, degrees=True).as_matrix()
+    source.position.translation = [-100 * mm, 20 * mm, 30 * mm]
     source.direction.type = "momentum"
-    source.direction.momentum = [0, 0, 1]
+    source.direction.momentum = [-1, 0, 0]
     source.n = 20000
     source.direction.partPhSp_x = [
         2.3335754 * mm,
         2.3335754 * mrad,
         0.00078728 * mm * mrad,
         0,
     ]
@@ -110,82 +114,103 @@
         dose.hit_type = "random"
         count += 1
 
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
 
+    print(sim.source_manager.dump_sources())
+
     # create output dir, if it doesn't exist
     if not os.path.isdir(output_path):
         os.mkdir(output_path)
 
     # start simulation
     sim.run()
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     print(stat)
 
     print("Start to analyze data")
-    override = False
-    if (not os.path.exists(ref_path / "sigma_values.txt")) or override:
-        sigmasRef, musRef = utility.write_gauss_param_to_file(
-            ref_path,
-            planePositionsV,
-            saveFig=False,
-            fNamePrefix="plane",
-            fNameSuffix="a_Carbon_1440MeV_sourceShapePBS-Edep.mhd",
-        )
-    override = False
+    # override = False
+    # if (not os.path.exists(ref_path / "sigma_values.txt")) or override:
+    #     sigmasRef, musRef = utility.write_gauss_param_to_file(
+    #         ref_path,
+    #         planePositionsV,
+    #         saveFig=False,
+    #         fNamePrefix="plane",
+    #         fNameSuffix="a_Carbon_1440MeV_sourceShapePBS-Edep.mhd",
+    # )
+    override = True
+    output_pathV = [
+        sim.output.get_actor("doseInYZ" + str(i)).user_info.output
+        for i in planePositionsV
+    ]
     if (not os.path.exists(output_path / "sigma_values.txt")) or override:
         sigmasGam, musGam = utility.write_gauss_param_to_file(
-            output_path,
-            planePositionsV,
-            saveFig=False,
-            fNamePrefix="plane",
-            fNameSuffix="a.mhd",
+            output_pathV, planePositionsV, saveFig=False
         )
     else:
         print("Some data are already available for analysis")
 
     # ----------------------------------------------------------------------------------------------------------------
     # tests
 
     # statistics
     stat_file = "SimulationStatistic_" + folder + ".txt"
     stats_ref = utility.read_stat_file(ref_path / stat_file)
-    is_ok = utility.assert_stats(stat, stats_ref, 0.10)
+    is_ok = utility.assert_stats(stat, stats_ref, 0.15)
 
     # energy deposition
     for i in planePositionsV:
         print("\nDifference for EDEP plane " + str(i))
-        mhd_gate = "plane" + str(i) + "a.mhd"
+        # mhd_gate = "plane" + str(i) + "a.mhd"
+        mhd_gate = sim.output.get_actor("doseInYZ" + str(i)).user_info.output
         mhd_ref = "plane" + str(i) + "a_" + folder + "-Edep.mhd"
         is_ok = (
             utility.assert_images(
                 ref_path / mhd_ref,
                 output_path / mhd_gate,
                 stat,
+                axis="x",
                 tolerance=50,
                 ignore_value=0,
             )
             and is_ok
         )
-        """EdepColorMap = utility.create_2D_Edep_colorMap(output_path / mhd_gate)
+
+        """
+        EdepColorMap = utility.create_2D_Edep_colorMap(output_path / mhd_gate)
         img_name = 'Plane_'+str(i)+'ColorMap.png'
         EdepColorMap.savefig(output_path / img_name)
-        plt.close(EdepColorMap)"""
+        plt.close(EdepColorMap)
+        """
 
     # beam shape
+    print("Comparing sigma values")
     sigma_file = "sigma_values.txt"
     is_ok = (
         utility.compareGaussParamFromFile(
             output_path / sigma_file,
             ref_path / sigma_file,
             rel_tol=2,
             abs_tol=0.5,
             verb=True,
+        )
+        and is_ok
+    )
+
+    print("Comparing mu values")
+    sigma_file = "mu_values.txt"
+    is_ok = (
+        utility.compareGaussParamFromFile(
+            output_path / sigma_file,
+            ref_path / sigma_file,
+            rel_tol=2,
+            abs_tol=0.5,
+            verb=True,
         )
         and is_ok
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test044_pbs_rot_transl.py` & `opengate-10.0b8/opengate/tests/src/test044_pbs_unfocused.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from scipy.spatial.transform import Rotation
-import os
+import os, sys
 import opengate as gate
 from opengate.tests import utility
 
-
 if __name__ == "__main__":
-    paths = utility.get_default_test_paths(__file__, "gate_test044_pbs_rot_transl")
+    sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+    # import ../db.py
+
+    # from sim_output_analysis import compareGaussParam, plot_edep
+
+    paths = utility.get_default_test_paths(__file__, "gate_test044_pbs_unFocused")
 
     particle = "Carbon_"
     energy = "1440MeV_"
     beam_shape = "sourceShapePBS"
     folder = particle + energy + beam_shape
 
-    output_path = paths.output / "output_test044_rot_transl"
+    output_path = paths.output
     ref_path = paths.gate_output
 
     # for for loop
     start = -500
     spacing = 100
     end = -start + spacing
     planePositionsV = range(start, end, spacing)
@@ -76,35 +80,34 @@
     # physics
     sim.physics_manager.physics_list_name = "FTFP_INCLXX_EMZ"
     sim.physics_manager.global_production_cuts.all = 1000 * km
 
     # default source for tests (from test42)
     source = sim.add_source("IonPencilBeamSource", "mysource")
     source.energy.mono = 1440 * MeV
-    # source.energy.type = 'gauss'
     source.particle = "ion 6 12"  # carbon
     source.position.type = "disc"  # pos = Beam, shape = circle + sigma
-    # rotate the disc, equiv to : rot1 0 1 0 and rot2 0 0 1
+    source.position.translation = [0 * mm, 0 * mm, 0 * cm]
     source.position.rotation = Rotation.from_euler("y", -90, degrees=True).as_matrix()
-    source.position.translation = [-100 * mm, 20 * mm, 30 * mm]
+    # rotate the disc, equiv to : rot1 0 1 0 and rot2 0 0 1
     source.direction.type = "momentum"
     source.direction.momentum = [-1, 0, 0]
     source.n = 20000
     source.direction.partPhSp_x = [
         2.3335754 * mm,
         2.3335754 * mrad,
         0.00078728 * mm * mrad,
         0,
-    ]
+    ]  # negative
     source.direction.partPhSp_y = [
         1.96433431 * mm,
-        0.00079118 * mrad,
+        1.79118 * mrad,
         0.00249161 * mm * mrad,
-        0,
-    ]
+        1,
+    ]  # positive
 
     count = 0
     # add dose actors
     for i in planePositionsV:
         dose = sim.add_actor("DoseActor", "doseInYZ" + str(i))
         filename = "plane" + str(i) + "a.mhd"
         dose.output = output_path / filename
@@ -129,30 +132,30 @@
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     print(stat)
 
     print("Start to analyze data")
     override = False
-    if (not os.path.exists(ref_path / "sigma_values.txt")) or override:
-        sigmasRef, musRef = utility.write_gauss_param_to_file(
-            ref_path,
-            planePositionsV,
-            saveFig=False,
-            fNamePrefix="plane",
-            fNameSuffix="a_Carbon_1440MeV_sourceShapePBS-Edep.mhd",
-        )
-    override = False
+    # if (not os.path.exists(ref_path / "sigma_values.txt")) or override:
+    #     sigmasRef, musRef = utility.write_gauss_param_to_file(
+    #         ref_path,
+    #         planePositionsV,
+    #         saveFig=False,
+    #         fNamePrefix="plane",
+    #         fNameSuffix="a_Carbon_1440MeV_sourceShapePBS-Edep.mhd",
+    #     )
+    override = True
+    output_pathV = [
+        sim.output.get_actor("doseInYZ" + str(i)).user_info.output
+        for i in planePositionsV
+    ]
     if (not os.path.exists(output_path / "sigma_values.txt")) or override:
         sigmasGam, musGam = utility.write_gauss_param_to_file(
-            output_path,
-            planePositionsV,
-            saveFig=False,
-            fNamePrefix="plane",
-            fNameSuffix="a.mhd",
+            output_pathV, planePositionsV, saveFig=False
         )
     else:
         print("Some data are already available for analysis")
 
     # ----------------------------------------------------------------------------------------------------------------
     # tests
 
@@ -160,33 +163,31 @@
     stat_file = "SimulationStatistic_" + folder + ".txt"
     stats_ref = utility.read_stat_file(ref_path / stat_file)
     is_ok = utility.assert_stats(stat, stats_ref, 0.15)
 
     # energy deposition
     for i in planePositionsV:
         print("\nDifference for EDEP plane " + str(i))
-        mhd_gate = "plane" + str(i) + "a.mhd"
+        # mhd_gate = "plane" + str(i) + "a.mhd"
+        mhd_gate = sim.output.get_actor("doseInYZ" + str(i)).user_info.output
         mhd_ref = "plane" + str(i) + "a_" + folder + "-Edep.mhd"
         is_ok = (
             utility.assert_images(
                 ref_path / mhd_ref,
                 output_path / mhd_gate,
                 stat,
-                axis="x",
                 tolerance=50,
                 ignore_value=0,
             )
             and is_ok
         )
-        """
-        EdepColorMap = utility.create_2D_Edep_colorMap(output_path / mhd_gate)
+        """EdepColorMap = utlity.create_2D_Edep_colorMap(output_path / mhd_gate)
         img_name = 'Plane_'+str(i)+'ColorMap.png'
         EdepColorMap.savefig(output_path / img_name)
-        plt.close(EdepColorMap)
-        """
+        plt.close(EdepColorMap)"""
 
     # beam shape
     print("Comparing sigma values")
     sigma_file = "sigma_values.txt"
     is_ok = (
         utility.compareGaussParamFromFile(
             output_path / sigma_file,
```

### Comparing `opengate-10.0b7/opengate/tests/src/test044_pbs_source_to_volume.py` & `opengate-10.0b8/opengate/tests/src/test044_pbs_source_to_volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,31 +126,31 @@
     sim.run()
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     print(stat)
 
     print("Start to analyze data")
-    override = False
-    if (not os.path.exists(ref_path / "sigma_values.txt")) or override:
-        sigmasRef, musRef = utility.write_gauss_param_to_file(
-            ref_path,
-            planePositionsV,
-            saveFig=False,
-            fNamePrefix="plane",
-            fNameSuffix="a_Carbon_1440MeV_sourceShapePBS-Edep.mhd",
-        )
-    override = False
+    # override = False
+    # if (not os.path.exists(ref_path / "sigma_values.txt")) or override:
+    #     sigmasRef, musRef = utility.write_gauss_param_to_file(
+    #         ref_path,
+    #         planePositionsV,
+    #         saveFig=False,
+    #         fNamePrefix="plane",
+    #         fNameSuffix="a_Carbon_1440MeV_sourceShapePBS-Edep.mhd",
+    #     )
+    override = True
+    output_file_paths = [
+        sim.output.get_actor("doseInYZ" + str(i)).user_info.output
+        for i in planePositionsV
+    ]
     if (not os.path.exists(output_path / "sigma_values.txt")) or override:
         sigmasGam, musGam = utility.write_gauss_param_to_file(
-            output_path,
-            planePositionsV,
-            saveFig=False,
-            fNamePrefix="plane",
-            fNameSuffix="a.mhd",
+            output_file_paths, planePositionsV, saveFig=False
         )
     else:
         print("Some data are already available for analysis")
 
     # ----------------------------------------------------------------------------------------------------------------
     # tests
 
@@ -158,15 +158,15 @@
     stat_file = "SimulationStatistic_" + folder + ".txt"
     stats_ref = utility.read_stat_file(ref_path / stat_file)
     is_ok = utility.assert_stats(stat, stats_ref, 0.10)
 
     # energy deposition
     for i in planePositionsV:
         print("\nDifference for EDEP plane " + str(i))
-        mhd_gate = "plane" + str(i) + "a.mhd"
+        mhd_gate = sim.output.get_actor("doseInYZ" + str(i)).user_info.output
         mhd_ref = "plane" + str(i) + "a_" + folder + "-Edep.mhd"
         is_ok = (
             utility.assert_images(
                 ref_path / mhd_ref,
                 output_path / mhd_gate,
                 stat,
                 tolerance=50,
```

### Comparing `opengate-10.0b7/opengate/tests/src/test044_pbs_unfocused.py` & `opengate-10.0b8/opengate/tests/src/test044_pbs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import os
 from scipy.spatial.transform import Rotation
-import os, sys
 import opengate as gate
 from opengate.tests import utility
 
 if __name__ == "__main__":
-    sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-
-    # from sim_output_analysis import compareGaussParam, plot_edep
-    paths = utility.get_default_test_paths(__file__, "gate_test044_pbs_unFocused")
+    paths = utility.get_default_test_paths(__file__, "gate_test044_pbs")
 
     particle = "Carbon_"
     energy = "1440MeV_"
     beam_shape = "sourceShapePBS"
     folder = particle + energy + beam_shape
 
-    output_path = paths.output / "output_test044_unFocused"
+    output_path = paths.output / "output_test044"
     ref_path = paths.gate_output
+    print(f"{ref_path =}")
 
-    # for for loop
+    # for the for loop
     start = -500
     spacing = 100
     end = -start + spacing
     planePositionsV = range(start, end, spacing)
 
     # create the simulation
     sim = gate.Simulation()
@@ -54,16 +52,15 @@
     world = sim.world
     world.size = [600 * cm, 500 * cm, 500 * cm]
 
     # waterbox
     # translation and rotation like in the Gate macro
     waterbox = sim.add_volume("Box", "waterbox")
     waterbox.size = [10 * cm, 10 * cm, 100.2 * cm]
-    waterbox.rotation = Rotation.from_euler("y", 90, degrees=True).as_matrix()
-    waterbox.translation = [-50.1 * cm, 0 * cm, 0 * cm]
+    waterbox.translation = [0 * cm, 0 * cm, 50.1 * cm]
     waterbox.material = "Vacuum"
     waterbox.color = [0, 0, 1, 1]
 
     # Planes
     m = Rotation.identity().as_matrix()
 
     for i in planePositionsV:
@@ -81,31 +78,30 @@
 
     # default source for tests (from test42)
     source = sim.add_source("IonPencilBeamSource", "mysource")
     source.energy.mono = 1440 * MeV
     source.particle = "ion 6 12"  # carbon
     source.position.type = "disc"  # pos = Beam, shape = circle + sigma
     source.position.translation = [0 * mm, 0 * mm, 0 * cm]
-    source.position.rotation = Rotation.from_euler("y", -90, degrees=True).as_matrix()
     # rotate the disc, equiv to : rot1 0 1 0 and rot2 0 0 1
     source.direction.type = "momentum"
-    source.direction.momentum = [-1, 0, 0]
+    source.direction.momentum = [0, 0, 1]
     source.n = 20000
     source.direction.partPhSp_x = [
         2.3335754 * mm,
         2.3335754 * mrad,
         0.00078728 * mm * mrad,
         0,
-    ]  # negative
+    ]
     source.direction.partPhSp_y = [
         1.96433431 * mm,
-        1.79118 * mrad,
+        0.00079118 * mrad,
         0.00249161 * mm * mrad,
-        1,
-    ]  # positive
+        0,
+    ]
 
     count = 0
     # add dose actors
     for i in planePositionsV:
         dose = sim.add_actor("DoseActor", "doseInYZ" + str(i))
         filename = "plane" + str(i) + "a.mhd"
         dose.output = output_path / filename
@@ -115,98 +111,83 @@
         dose.hit_type = "random"
         count += 1
 
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
 
-    print(sim.source_manager.dump_sources())
-
     # create output dir, if it doesn't exist
     if not os.path.isdir(output_path):
         os.mkdir(output_path)
 
     # start simulation
     sim.run()
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
     print(stat)
 
     print("Start to analyze data")
     override = False
-    if (not os.path.exists(ref_path / "sigma_values.txt")) or override:
-        sigmasRef, musRef = utility.write_gauss_param_to_file(
-            ref_path,
-            planePositionsV,
-            saveFig=False,
-            fNamePrefix="plane",
-            fNameSuffix="a_Carbon_1440MeV_sourceShapePBS-Edep.mhd",
-        )
-    override = False
+    # if (not os.path.exists(ref_path / "sigma_values.txt")) or override:
+    #     sigmasRef, musRef = utility.write_gauss_param_to_file(
+    #         ref_path,
+    #         planePositionsV,
+    #         saveFig=False,
+    #         fNamePrefix="plane",
+    #         fNameSuffix="a_Carbon_1440MeV_sourceShapePBS-Edep.mhd",
+    #     )
+    override = True
+    output_pathV = [
+        sim.output.get_actor("doseInYZ" + str(i)).user_info.output
+        for i in planePositionsV
+    ]
     if (not os.path.exists(output_path / "sigma_values.txt")) or override:
         sigmasGam, musGam = utility.write_gauss_param_to_file(
-            output_path,
-            planePositionsV,
-            saveFig=False,
-            fNamePrefix="plane",
-            fNameSuffix="a.mhd",
+            output_pathV, planePositionsV, saveFig=False
         )
     else:
         print("Some data are already available for analysis")
 
     # ----------------------------------------------------------------------------------------------------------------
     # tests
 
     # statistics
     stat_file = "SimulationStatistic_" + folder + ".txt"
     stats_ref = utility.read_stat_file(ref_path / stat_file)
-    is_ok = utility.assert_stats(stat, stats_ref, 0.15)
+    is_ok = utility.assert_stats(stat, stats_ref, 0.10)
 
     # energy deposition
     for i in planePositionsV:
         print("\nDifference for EDEP plane " + str(i))
-        mhd_gate = "plane" + str(i) + "a.mhd"
+        # mhd_gate = "plane" + str(i) + "a.mhd"
+        mhd_gate = sim.output.get_actor("doseInYZ" + str(i)).user_info.output
         mhd_ref = "plane" + str(i) + "a_" + folder + "-Edep.mhd"
         is_ok = (
             utility.assert_images(
                 ref_path / mhd_ref,
                 output_path / mhd_gate,
                 stat,
                 tolerance=50,
                 ignore_value=0,
             )
             and is_ok
         )
-        """EdepColorMap = utlity.create_2D_Edep_colorMap(output_path / mhd_gate)
+        """EdepColorMap = utility.create_2D_Edep_colorMap(output_path / mhd_gate)
         img_name = 'Plane_'+str(i)+'ColorMap.png'
         EdepColorMap.savefig(output_path / img_name)
         plt.close(EdepColorMap)"""
 
     # beam shape
-    print("Comparing sigma values")
     sigma_file = "sigma_values.txt"
     is_ok = (
         utility.compareGaussParamFromFile(
             output_path / sigma_file,
             ref_path / sigma_file,
             rel_tol=2,
             abs_tol=0.5,
             verb=True,
-        )
-        and is_ok
-    )
-
-    print("Comparing mu values")
-    sigma_file = "mu_values.txt"
-    is_ok = (
-        utility.compareGaussParamFromFile(
-            output_path / sigma_file,
-            ref_path / sigma_file,
-            rel_tol=2,
-            abs_tol=0.5,
-            verb=True,
         )
         and is_ok
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test044_pbs_weight.py` & `opengate-10.0b8/opengate/tests/src/test044_pbs_weight.py`

 * *Files 9% similar despite different names*

```diff
@@ -161,25 +161,26 @@
         os.mkdir(output_path)
 
     # start simulation
     sim.run()
 
     # print results at the end
     stat = sim.output.get_actor("Stats")
+
     print(stat)
 
     # ----------------------------------------------------------------------------------------------------------------
     # tests
 
     # energy deposition: we expect the edep from source two
     # to be double the one of source one
 
     print("\nDifference for EDEP")
-    mhd_1 = "phantom_a_1.mhd"
-    mhd_2 = "phantom_a_2.mhd"
+    mhd_1 = sim.output.get_actor("doseInYZ_1").user_info.output
+    mhd_2 = sim.output.get_actor("doseInYZ_2").user_info.output
     test = True
     # test = utility.assert_images(
     #     output_path / mhd_1,
     #     output_path / mhd_2,
     #     stat,
     #     axis="x",
     #     tolerance=50,
```

### Comparing `opengate-10.0b7/opengate/tests/src/test045_gan_phsp_pet_gan_helpers.py` & `opengate-10.0b8/opengate/tests/src/test045_gan_phsp_pet_gan_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test045_speedup.py` & `opengate-10.0b8/opengate/tests/src/test045_speedup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import click
 from box import Box
 import opengate as gate
 import test045_gan_phsp_pet_gan_helpers as t45
 from opengate.tests import utility
+from pathlib import Path
 
 paths = utility.get_default_test_paths(__file__, "", "test045")
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
@@ -20,15 +21,15 @@
 @click.option("--pet", default=False, is_flag=True, help="W/wo PET output")
 @click.option("--activity_bqml", "-a", default="10", help="Activity in BqmL")
 @click.option("--threads", "-t", default=1, help="Nb of threads")
 @click.option("--visu", "-v", default=False, is_flag=True, help="visu for debug")
 @click.option(
     "--output_folder",
     "-o",
-    default=".",
+    default="AUTO",
     help="output folder (AUTO for the tests)",
 )
 @click.option("--seed", default="auto", help="random engine seed")
 def go(
     phantom, source, rad, gaga, pet, activity_bqml, visu, threads, output_folder, seed
 ):
     run_test_045_speedrun(
@@ -67,16 +68,19 @@
     p.gaga_pth = paths.data / "pth120_test9221_GP_0GP_10.0_100000.pth"
 
     gate.utility.print_dic(p)
 
     # output
     if output_folder == "AUTO":
         output_folder = paths.output
-    out = f"test045_speedup_p_{p.phantom_type}_s_{p.source_type}_pet_{p.use_pet}_gaga_{gaga}"
-    p.pet_output = f"{output_folder}/{out}.root"
+    out = (
+        output_folder
+        / f"test045_speedup_p_{p.phantom_type}_s_{p.source_type}_pet_{p.use_pet}_gaga_{gaga}"
+    )
+    p.pet_output = output_folder / f"{out}.root"
 
     # init the simulation
     sim = gate.Simulation()
 
     # visu
     sim.visu = visu
     if visu:
@@ -96,15 +100,15 @@
     sim.run()
 
     # print
     stats = sim.output.get_actor("Stats")
     print(stats)
 
     # save
-    stats.write(f"{output_folder}/{out}.txt")
+    stats.write(output_folder / f"{out}.txt")
 
     if p.use_pet:
         import uproot
 
         phsp = sim.output.get_actor("Singles").user_info
         f = phsp.output
         s = uproot.open(f)["Singles"]
```

### Comparing `opengate-10.0b7/opengate/tests/src/test045_speedup_all_wip.py` & `opengate-10.0b8/opengate/tests/src/test045_speedup_all_wip.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test046_rad.py` & `opengate-10.0b8/opengate/tests/src/test046_rad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from box import Box
 import json
 import numpy as np
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import opengate as gate
 from opengate.tests import utility
 
 if __name__ == "__main__":
     paths = utility.get_default_test_paths(__file__, "")
 
     radionuclides = ["Tc99m", "Lu177", "In111", "I131"]
```

### Comparing `opengate-10.0b7/opengate/tests/src/test047_gan_vox_source_cond.py` & `opengate-10.0b8/opengate/tests/src/test047_gan_vox_source_cond.py`

 * *Files 9% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     )  # should be "auto" but "cpu" for macOS github actions to avoid mps errors
 
     # cuts (not need precision here)
     c = sim.physics_manager.global_production_cuts.all = 100 * mm
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "dose")
-    dose.output = paths.output / "test047-edep.mhd"
+    dose.output = paths.output / "test047.mhd"
     dose.mother = "ct"
     dose.size = [70, 70, 240]
     dose.spacing = [3.5 * mm, 3.5 * mm, 3.5 * mm]
     dose.img_coord_system = True
     dose.hit_type = "random"
 
     # add stat actor
@@ -131,25 +131,26 @@
     stat = sim.output.get_actor("Stats")
     print(stat)
     ref_stat_file = paths.output_ref / "t047_stats.txt"
     # stat.write(ref_stat_file) # (for reference)
     stats_ref = utility.read_stat_file(ref_stat_file)
     is_ok = utility.assert_stats(stat, stats_ref, 0.005)
 
+    dose = sim.output.get_actor("dose")
     print()
     gate.exception.warning("Compare image to analog")
     is_ok = (
         utility.assert_images(
             paths.output_ref / "test047-edep.mhd",
-            dose.output,
+            paths.output / dose.user_info.output,
             stat,
             tolerance=19,
             ignore_value=0,
             axis="x",
         )
         and is_ok
     )
 
     print("Test with vv: ")
-    print(f"vv {source.cond_image} --fusion {dose.output}")
+    print(f"vv {source.cond_image} --fusion {dose.user_info.output}")
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test047_voxelization.py` & `opengate-10.0b8/opengate/tests/src/test047_voxelization.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test048_split_spect_projections.py` & `opengate-10.0b8/opengate/tests/src/test048_split_spect_projections.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_helpers.py` & `opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         m = np.mean(ref)
         s1, is_ok1 = rel_d(np.min(ref), np.min(val), m, tol)
         s2, is_ok2 = rel_d(m, np.mean(val), m, tol)
         s3, is_ok3 = rel_d(np.max(ref), np.max(val), m, tol)
         s = f"Min: {s1}    Mean: {s2}     Max: {s3}"
         return s, is_ok1 and is_ok2 and is_ok3
 
-    tol = 1
+    tol = 1.2
     s, b = compare_stat(times_ref, times, tol)
     print()
     utility.print_test(b, f"Hits timing ref:\n{s}, Passed? {b}")
     is_ok = b
 
     times_ref = (
         uproot.open(ref_root_file)["Singles"].arrays(library="numpy")["time"] * 1e9
```

### Comparing `opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_v1.py` & `opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_v1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_v2_mt.py` & `opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_v2_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_v3.py` & `opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_v3.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test049_pet_digit_blurring_v4.py` & `opengate-10.0b8/opengate/tests/src/test049_pet_digit_blurring_v4.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test050_let_actor_letd.py` & `opengate-10.0b8/opengate/tests/src/test050_let_actor_letd_mt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from scipy.spatial.transform import Rotation
+
 import opengate as gate
 from opengate.tests import utility
 
+
 if __name__ == "__main__":
+    do_debug = False
     paths = utility.get_default_test_paths(__file__, "test050_let_actor_letd")
 
     ref_path = paths.output_ref
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
     sim.g4_verbose_level = 1
     sim.visu = False
-    sim.random_seed = 12345678910
+    sim.random_seed = 1234567891
+    sim.number_of_threads = 2
 
-    numPartSimTest = 20000
+    numPartSimTest = 40000 / sim.number_of_threads
     numPartSimRef = 1e5
 
     # units
     m = gate.g4_units.m
     cm = gate.g4_units.cm
     mm = gate.g4_units.mm
     km = gate.g4_units.km
@@ -51,17 +55,17 @@
     phantom_off.material = test_material_name
     phantom_off.color = [0, 0, 1, 1]
 
     # physics
     sim.physics_manager.physics_list_name = "QGSP_BIC_EMZ"
     # sim.physics_manager.set_production_cut("world", "all", 1000 * km)
     # FIXME need SetMaxStepSizeInRegion ActivateStepLimiter
-    # now avialable
+    # now available
     # e.g.
-    # sim.physics_manager.set_max_step_size(volume_name='phantom.name', max_step_size=1*mm)
+    # sim.physics_manager.set_max_step_size(volume_name='phantom', max_step_size=1*mm)
 
     # default source for tests
     source = sim.add_source("GenericSource", "mysource")
     source.energy.mono = 80 * MeV
     # source.energy.type = 'gauss'
     # source.energy.sigma_gauss = 1 * MeV
     source.particle = "proton"
@@ -85,15 +89,15 @@
     doseActorName_IDD_d = "IDD_d"
     doseIDD = sim.add_actor("DoseActor", doseActorName_IDD_d)
     doseIDD.output = paths.output / ("test050-" + doseActorName_IDD_d + ".mhd")
     doseIDD.mother = phantom_off.name
     doseIDD.size = size
     doseIDD.spacing = spacing
     doseIDD.hit_type = "random"
-    doseIDD.gray = False
+    doseIDD.dose = False
 
     LETActorName_IDD_d = "LETActorOG_d"
     LETActor_IDD_d = sim.add_actor("LETActor", LETActorName_IDD_d)
     LETActor_IDD_d.output = paths.output / ("test050-" + LETActorName_IDD_d + ".mhd")
     LETActor_IDD_d.mother = phantom_off.name
     LETActor_IDD_d.size = size
     LETActor_IDD_d.spacing = spacing
@@ -122,76 +126,101 @@
     LETActor_IDD_d2w.mother = phantom_off.name
     LETActor_IDD_d2w.size = size
     LETActor_IDD_d2w.spacing = spacing
     LETActor_IDD_d2w.hit_type = "random"
     LETActor_IDD_d2w.other_material = "G4_WATER"
     setattr(LETActor_IDD_d2w, "dose_average", True)
 
+    LET_primaries = "LETprimaries"
+    LETActor_primaries = sim.add_actor("LETActor", LET_primaries)
+    LETActor_primaries.output = paths.output / ("test050-" + LET_primaries + ".mhd")
+    LETActor_primaries.mother = phantom_off.name
+    LETActor_primaries.size = size
+    LETActor_primaries.spacing = spacing
+    LETActor_primaries.hit_type = "random"
+    LETActor_primaries.dose_average = True
+
+    # # add dose actor, without e- (to check)
+    fe = sim.add_filter("ParticleFilter", "f")
+    fe.particle = "proton"
+    fe.policy = "keep"
+    LETActor_primaries.filters.append(fe)
+    print(dir(fe))
+
     fName_ref_IDD = "IDD__Proton_Energy1MeVu_RiFiout-Edep.mhd"
     print(paths)
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "stats")
     s.track_types_flag = True
     # s.filters.append(f)
 
     print("Filters: ", sim.filter_manager)
-    print(sim.filter_manager.dump())
+    # print(sim.filter_manager.dump())
 
     # start simulation
-    sim.n = 10
     sim.run()
 
     # paths.gate_output
 
     # print results at the end
     stat = sim.output.get_actor("stats")
+
     print(stat)
 
     # ----------------------------------------------------------------------------------------------------------------
     # tests
     print()
     # gate.exception.warning("Tests stats file")
     # stats_ref = utility.read_stat_file(paths.gate_output / "stats.txt")
     # is_ok = utility.assert_stats(stat, stats_ref, 0.14)
 
-    LETActorFPath_doseAveraged = sim.output.get_actor(
-        LETActorName_IDD_d
-    ).user_info.output
-    LETActorFPath_trackAveraged = sim.output.get_actor(
-        LETActorName_IDD_t
-    ).user_info.output
-
-    fNameIDD = "test050_IDD__Proton_Energy1MeVu_RiFiout-Edep.mhd"
-    """
-    is_ok = utility.assert_images(
-        ref_path / fNameIDD,
-        doseIDD.output,
-        stat,
-        tolerance=100,
-        ignore_value=0,
-        axis="x",
-        scaleImageValuesFactor=numPartSimRef / numPartSimTest,
-    )
-    """
+    LETActor_doseAveraged = sim.output.get_actor(LETActorName_IDD_d)
+    LETActor_trackAveraged = sim.output.get_actor(LETActorName_IDD_t)
+
+    LETActor_primaries = sim.output.get_actor(LET_primaries)
+
+    fNameIDD = sim.output.get_actor(doseActorName_IDD_d).user_info.output
+    if do_debug:
+        is_ok = utility.assert_images(
+            ref_path / fNameIDD,
+            doseIDD.output,
+            stat,
+            tolerance=100,
+            ignore_value=0,
+            axis="x",
+            scaleImageValuesFactor=numPartSimRef / numPartSimTest,
+        )
 
+    tests_pass = []
     is_ok = utility.assert_filtered_imagesprofile1D(
         ref_filter_filename1=ref_path / fNameIDD,
         ref_filename1=ref_path
         / "test050_LET1D_noFilter__PrimaryProton-doseAveraged.mhd",
-        filename2=LETActor_IDD_d.output,
-        tolerance=15,
-        plt_ylim=[0, 25],
+        filename2=paths.output / LETActor_doseAveraged.user_info.output,
+        tolerance=40,
+        #  plt_ylim=[0, 25],
     )
+    tests_pass.append(is_ok)
+    print(f"218 {is_ok =}")
 
-    is_ok = (
-        utility.assert_filtered_imagesprofile1D(
-            ref_filter_filename1=ref_path / fNameIDD,
-            ref_filename1=ref_path
-            / "test050_LET1D_noFilter__PrimaryProton-trackAveraged.mhd",
-            filename2=LETActor_IDD_t.output,
-            tolerance=8,
-            plt_ylim=[0, 18],
-        )
-        and is_ok
+    is_ok = utility.assert_filtered_imagesprofile1D(
+        ref_filter_filename1=ref_path / fNameIDD,
+        ref_filename1=ref_path
+        / "test050_LET1D_noFilter__PrimaryProton-trackAveraged.mhd",
+        filename2=paths.output / LETActor_trackAveraged.user_info.output,
+        tolerance=8,
+        #    plt_ylim=[0, 18],
+    )
+
+    tests_pass.append(is_ok)
+    print(f"202 {is_ok =}")
+    is_ok = utility.assert_filtered_imagesprofile1D(
+        ref_filter_filename1=ref_path / fNameIDD,
+        ref_filename1=ref_path / "test050_LET1D_Z1__PrimaryProton-doseAveraged.mhd",
+        filename2=paths.output / LETActor_primaries.user_info.output,
+        tolerance=5,
+        #    plt_ylim=[0, 18],
     )
+    print(f"222 {is_ok =}")
+    tests_pass.append(is_ok)
 
-    utility.test_ok(is_ok)
+    utility.test_ok(all(tests_pass))
```

### Comparing `opengate-10.0b7/opengate/tests/src/test051_adder_time_difference.py` & `opengate-10.0b8/opengate/tests/src/test051_adder_time_difference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import matplotlib.pyplot as plt
 import numpy as np
-import opengate.contrib.spect.genm670 as gate_spect
+import opengate.contrib.spect.ge_discovery_nm670 as gate_spect
 import opengate as gate
 from opengate.tests import utility
 
 if __name__ == "__main__":
     paths = utility.get_default_test_paths(__file__, "")
 
     """
@@ -37,15 +37,15 @@
 
     # world size
     world = sim.world
     world.size = [2.5 * m, 2.5 * m, 2.5 * m]
     world.material = "G4_AIR"
 
     # spect head without collimator
-    spect, crystal = gate_spect.add_ge_nm67_spect_head(
+    spect, colli, crystal = gate_spect.add_spect_head(
         sim, "spect", collimator_type=False, debug=False
     )
     spect.translation = [0, 0, -15 * cm]
 
     # spect digitizer
     hc = sim.add_actor("DigitizerHitsCollectionActor", f"Hits")
     hc.mother = crystal.name
```

### Comparing `opengate-10.0b7/opengate/tests/src/test052_tac_activity_source.py` & `opengate-10.0b8/opengate/tests/src/test052_tac_activity_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     keV = gate.g4_units.keV
 
     # verbose
     sim.visu = False
     sim.g4_verbose = False
     sim.g4_verbose_level = 1
     sim.number_of_threads = 1
-    sim.random_seed = "auto"
+    sim.random_seed = 987654321
 
     # world size
     world = sim.world
     world.size = [1 * m, 1 * m, 1 * m]
     world.material = "G4_AIR"
 
     # source of Ac225 ion
```

### Comparing `opengate-10.0b7/opengate/tests/src/test053_production_cuts.py` & `opengate-10.0b8/opengate/tests/src/test053_production_cuts.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test053_step_limiter_mt.py` & `opengate-10.0b8/opengate/tests/src/test053_step_limiter_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test054_parallel_geometry.py` & `opengate-10.0b8/opengate/tests/src/test072_coinc_sorter_1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,133 +1,147 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-from scipy.spatial.transform import Rotation
 import opengate as gate
 from opengate.tests import utility
 
 if __name__ == "__main__":
-    paths = utility.get_default_test_paths(__file__, None, "test054")
-
-    # create the simulation
     sim = gate.Simulation()
 
-    # main options
-    # sim.visu_type = "vrml"
-    sim.visu = False
-    sim.check_volumes_overlap = True
+    # options
+    # warning the visualisation is slow !
+    # sim.visu = True
+    sim.visu_type = "vrml"
+    sim.random_seed = 123456
     sim.number_of_threads = 1
-    sim.random_seed = 654923
-
-    sim.physics_manager.physics_list_name = "G4EmStandardPhysics_option4"
-
-    # add a material database
-    sim.volume_manager.add_material_database(paths.data / "GateMaterials.db")
 
     # units
     m = gate.g4_units.m
+    mm = gate.g4_units.mm
     cm = gate.g4_units.cm
-    MeV = gate.g4_units.MeV
+    sec = gate.g4_units.s
+    ps = gate.g4_units.ps
+    keV = gate.g4_units.keV
     Bq = gate.g4_units.Bq
-    mm = gate.g4_units.mm
+    gcm3 = gate.g4_units.g_cm3
+    deg = gate.g4_units.deg
 
-    #  change world size
+    # colors (similar to the ones of Gate)
+    red = [1, 0, 0, 1]
+    blue = [0, 0, 1, 1]
+    green = [0, 1, 0, 1]
+    yellow = [0.9, 0.9, 0.3, 1]
+    gray = [0.5, 0.5, 0.5, 1]
+    white = [1, 1, 1, 0.8]
+
+    # folders
+    paths = utility.get_default_test_paths(
+        __file__, output_folder="test072_coinc_sorter"
+    )
+
+    # world
     world = sim.world
-    world.size = [1 * m, 1 * m, 1 * m]
+    world.size = [450 * mm, 450 * mm, 70 * mm]
     world.material = "G4_AIR"
 
-    fake = sim.add_volume("Box", "fake")
-    fake.size = [40 * cm, 40 * cm, 40 * cm]
-    fake.material = "G4_AIR"
-    fake.color = [1, 0, 1, 1]
-
-    # image
-    patient = sim.add_volume("Image", "patient")
-    patient.mother = fake.name
-    patient.image = paths.data / "patient-40mm.mhd"
-    patient.material = "G4_AIR"  # material used by default
-    patient.voxel_materials = [
-        [-2000, -900, "G4_AIR"],
-        [-900, -100, "Lung"],
-        [-100, 0, "G4_ADIPOSE_TISSUE_ICRP"],
-        [0, 300, "G4_TISSUE_SOFT_ICRP"],
-        [300, 800, "G4_B-100_BONE"],
-        [800, 6000, "G4_BONE_COMPACT_ICRU"],
-    ]
+    # create the materials
+    sim.volume_manager.material_database.add_material_nb_atoms(
+        "Lead", ["Pb"], [1], 11.4 * gcm3
+    )
+    sim.volume_manager.material_database.add_material_nb_atoms(
+        "BGO", ["Bi", "Ge", "O"], [4, 3, 12], 7.13 * gcm3
+    )
 
-    # create two other parallel worlds
-    sim.add_parallel_world("world2")
-    sim.add_parallel_world("world3")
-
-    # detector in w2 (on top of world)
-    det = sim.add_volume("Box", "detector")
-    det.mother = "world2"
-    det.material = "G4_GLASS_LEAD"
-    det.size = [400 * mm, 400 * mm, 2 * mm]
-    det.translation = [0, 0, 200 * mm]
-    det.rotation = Rotation.from_euler("x", 40, degrees=True).as_matrix()
-    det.color = [1, 0, 0, 1]
-
-    # detector in w3 (on top of w2)
-    det2 = sim.add_volume("Box", "detector2")
-    det2.mother = "world3"
-    det2.material = "G4_GLASS_LEAD"  # set 'None' if this volume should be transparent
-    det2.size = [400 * mm, 400 * mm, 2 * mm]
-    det2.translation = [0, 0, 200 * mm]
-    det2.rotation = Rotation.from_euler("x", -40, degrees=True).as_matrix()
-    det2.color = [1, 0, 0, 1]
+    sim.volume_manager.material_database.add_material_nb_atoms(
+        "LSO", ["Lu", "Si", "O"], [2, 1, 5], 7.4 * gcm3
+    )
+
+    sim.volume_manager.material_database.add_material_weights(
+        "LeadSb", ["Pb", "Sb"], [0.95, 0.05], 11.16 * gcm3
+    )
+
+    sim.volume_manager.material_database.add_material_weights(
+        "LYSO",
+        ["Lu", "Y", "Si", "O"],
+        [0.31101534, 0.368765605, 0.083209699, 0.237009356],
+        5.37 * gcm3,
+    )
+
+    # ring volume
+    pet = sim.add_volume("Tubs", "pet")
+    pet.rmax = 200 * mm
+    pet.rmin = 127 * mm
+    pet.dz = 32 * mm
+    pet.color = gray
+    pet.material = "G4_AIR"
+
+    # block
+    block = sim.add_volume("Box", "block")
+    block.mother = pet.name
+    block.size = [60 * mm, 10 * mm, 10 * mm]
+    translations_ring, rotations_ring = gate.geometry.utility.get_circular_repetition(
+        80, [160 * mm, 0.0 * mm, 0], start_angle_deg=180, axis=[0, 0, 1]
+    )
+    block.translation = translations_ring
+    block.rotation = rotations_ring
+    block.material = "G4_AIR"
+    block.color = white
+
+    # Crystal
+    crystal = sim.add_volume("Box", "crystal")
+    crystal.mother = block.name
+    crystal.size = [60 * mm, 10 * mm, 10 * mm]
+    crystal.material = "LYSO"
+    crystal.color = green
 
     # source
-    source = sim.add_source("GenericSource", "source")
-    source.energy.mono = 0.1 * MeV
-    source.particle = "gamma"
-    source.position.type = "box"
-    source.position.size = [1 * mm, 200 * mm, 1 * mm]
-    source.position.translation = [0, 0, 0 * cm]
-    source.activity = 10000 * Bq / sim.number_of_threads
-    source.direction.type = "momentum"
-    source.direction.momentum = [0, 0, 1]
-
-    # add phsp actor detector 1 (overlap!)
-    phsp = sim.add_actor("PhaseSpaceActor", "phsp")
-    phsp.output = paths.output / "test054.root"
-    phsp.mother = det.name
-    phsp.attributes = [
-        "KineticEnergy",
-        "PrePosition",
+    source = sim.add_source("GenericSource", "b2b")
+    source.particle = "back_to_back"
+    source.activity = 20 * Bq
+    source.position.type = "sphere"
+    source.position.radius = 0.0000000000000005 * mm
+    source.energy.mono = 511 * keV
+    source.direction.theta = [90 * deg, 90 * deg]
+    source.direction.phi = [0, 360 * deg]
+
+    # physics
+    sim.physics_manager.physics_list_name = "G4EmStandardPhysics_option3"
+
+    # actors
+    stats_actor = sim.add_actor("SimulationStatisticsActor", "Stats")
+    stats_actor.output = paths.output / "stats.txt"
+
+    # Hits
+    hc = sim.add_actor("DigitizerHitsCollectionActor", f"Hits_{crystal.name}")
+    hc.mother = crystal.name
+    hc.output = paths.output / "test72_output_1.root"
+    hc.attributes = [
+        "EventID",
+        "PostPosition",
+        "TotalEnergyDeposit",
+        "PreStepUniqueVolumeID",
+        "GlobalTime",
     ]
 
-    # add stat actor
-    stats = sim.add_actor("SimulationStatisticsActor", "Stats")
-    stats.track_types_flag = True
-
-    # print
-    print("Geometry trees: ")
-    print(sim.volume_manager.dump_volume_tree())
-
-    # start simulation
-    sim.run(True)
-
-    # print results at the end
-    stat = sim.output.get_actor("Stats")
-    print(stat)
-    d = sim.output.get_actor("phsp")
-    print(d)
-
-    keys = ["KineticEnergy", "PrePosition_X", "PrePosition_Y", "PrePosition_Z"]
-    tols = [0.01, 2.6, 1.8, 1.7]
-    ref = paths.output_ref / "test054_ref.root"
-    f = paths.output / "test054.png"
-    is_ok = utility.compare_root3(
-        ref,
-        phsp.output,
-        "phsp",
-        "phsp",
-        keys,
-        keys,
-        tols,
-        None,
-        None,
-        f,
-        hits_tol=6.1,
-    )
+    # Singles
+    sc = sim.add_actor("DigitizerAdderActor", f"Singles_{crystal.name}")
+    sc.mother = hc.mother
+    sc.input_digi_collection = hc.name
+    sc.policy = "EnergyWinnerPosition"
+    sc.output = hc.output
+
+    # timing
+    sim.run_timing_intervals = [[0, 200 * sec]]
+
+    # go
+    sim.run()
+
+    # end
+    stats = sim.output.get_actor("Stats")
+    print(stats)
+
+    # This test produces the data for the other 072_coinc_sorter tests
+    stats_ref = paths.output_ref / "stats.txt"
+    stats_ref = utility.read_stat_file(stats_ref)
+    is_ok = utility.assert_stats(stats, stats_ref, tolerance=0.04)
+
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test056_template_source.py` & `opengate-10.0b8/opengate/tests/src/test056_template_source.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test057_digit_efficiency.py` & `opengate-10.0b8/opengate/tests/src/test057_digit_efficiency.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test058_calc_uncertainty_mt.py` & `opengate-10.0b8/opengate/tests/src/test058_calc_uncertainty_mt.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     # main options
     sim.g4_verbose = False
     sim.visu = False
     # sim.visu_type = "vrml"
     sim.check_volumes_overlap = False
     # sim.running_verbose_level = gate.EVENT
     sim.number_of_threads = 5
-    sim.random_seed = "auto"
+    sim.random_seed = 12365445
 
     # units
     m = gate.g4_units.m
     km = gate.g4_units.km
     mm = gate.g4_units.mm
     cm = gate.g4_units.cm
     nm = gate.g4_units.nm
@@ -195,21 +195,22 @@
     sim.physics_manager.global_production_cuts.positron = 1 * km
 
     sim.run()
 
     # print results
     stats = sim.output.get_actor("Stats")
     h = sim.output.get_actor("PhaseSpace")
+    dose = sim.output.get_actor("dose")
     print(stats)
 
     # Open images for comparison
 
-    img_E = itk.imread(output_path / "test058_MT.mhd")
+    img_E = itk.imread(output_path / dose.user_info.output)
     array_E = itk.GetArrayFromImage(img_E)
-    err_img_E = itk.imread(output_path / "test058_MT_uncertainty.mhd")
+    err_img_E = itk.imread(output_path / dose.user_info.output_uncertainty)
     err_array_E = itk.GetArrayFromImage(err_img_E)
 
     f_phsp = uproot.open(output_path / "test058_MT.root")
     arr_phsp = f_phsp["PhaseSpace"]
     keys_data = arr_phsp.keys(filter_typename="double")
     E = f_phsp["PhaseSpace;1/KineticEnergy"]
     Ephoton = E.array()
```

### Comparing `opengate-10.0b7/opengate/tests/src/test058_iec_six_spheres.py` & `opengate-10.0b8/opengate/tests/src/test058_iec_six_spheres.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test059_tpsource_abs_dose.py` & `opengate-10.0b8/opengate/tests/src/test059_tpsource_abs_dose.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from opengate.tests import utility
 from opengate.contrib.beamlines.ionbeamline import BeamlineModel
 from opengate.contrib.tps.ionbeamtherapy import spots_info_from_txt, TreatmentPlanSource
 
 if __name__ == "__main__":
     # ------ INITIALIZE SIMULATION ENVIRONMENT ----------
     paths = utility.get_default_test_paths(__file__, "gate_test044_pbs")
+
     output_path = paths.output / "output_test059_rtp"
     ref_path = paths.output_ref / "test059_ref"
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
@@ -37,16 +38,15 @@
     deg = gate.g4_units.deg
     rad = gate.g4_units.rad
 
     # add a material database
     sim.volume_manager.add_material_database(paths.gate_data / "HFMaterials2014.db")
 
     #  change world size
-    world = sim.world
-    world.size = [600 * cm, 500 * cm, 500 * cm]
+    sim.world.size = [600 * cm, 500 * cm, 500 * cm]
 
     # nozzle box
     box = sim.add_volume("Box", "box")
     box.size = [500 * mm, 500 * mm, 1000 * mm]
     box.translation = [1148 * mm, 0.0, 0.0]
     box.rotation = Rotation.from_euler("y", -90, degrees=True).as_matrix()
     box.material = "Vacuum"
@@ -72,28 +72,29 @@
     roos.material = "G4_WATER"
     roos.rmax = 7.8
     roos.rmin = 0
     roos.dz = 200
     roos.color = [1, 0, 1, 1]
 
     # physics
+
     sim.physics_manager.physics_list_name = (
         "FTFP_INCLXX_EMZ"  # 'QGSP_BIC_HP_EMZ' #"FTFP_INCLXX_EMZ"
     )
 
     sim.physics_manager.set_production_cut("world", "all", 1000 * km)
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "doseInXYZ")
     dose.output = output_path / "abs_dose_roos.mhd"
     dose.mother = roos.name
     dose.size = [1, 1, 800]
     dose.spacing = [15.6, 15.6, 0.5]
     dose.hit_type = "random"
-    dose.gray = True
+    dose.dose = True
 
     ## ---------- DEFINE BEAMLINE MODEL -------------##
     IR2HBL = BeamlineModel()
     IR2HBL.name = None
     IR2HBL.radiation_types = "ion 6 12"
     # Nozzle entrance to Isocenter distance
     IR2HBL.distance_nozzle_iso = 1300.00  # 1648 * mm#1300 * mm
@@ -111,26 +112,25 @@
     IR2HBL.theta_y_coeffs = [0.0007911780133478402]
     IR2HBL.epsilon_y_coeffs = [0.0024916149017600447]
 
     ## --------START PENCIL BEAM SCANNING---------- ##
     # NOTE: HBL means that the beam is coming from -x (90 degree rot around y)
 
     nSim = 50000  # 328935  # particles to simulate per beam
-
-    spots, ntot, energies, G = spots_info_from_txt(
-        ref_path / "TreatmentPlan4Gate-F5x5cm_E120MeVn.txt", "ion 6 12"
+    beam_data_dict = spots_info_from_txt(
+        ref_path / "TreatmentPlan4Gate-F5x5cm_E120MeVn.txt", "ion 6 12", beam_nr=1
     )
-    tps = TreatmentPlanSource("RT_plan", sim)
-    tps.set_beamline_model(IR2HBL)
-    tps.set_particles_to_simulate(nSim)
-    tps.set_spots(spots)
-    tps.rotation = Rotation.from_euler("z", G, degrees=True)
-    tps.initialize_tpsource()
-
-    actual_sim_particles = tps.actual_sim_particles
+    tps = sim.add_source("TreatmentPlanPBSource", "TPSource")
+    tps.n = nSim
+    tps.sorted_spot_generation = True
+    tps.beam_model = IR2HBL
+    tps.beam_data_dict = beam_data_dict
+    tps.beam_nr = 1
+    tps.particle = "ion 6 12"
+    ntot = beam_data_dict["msw_beam"]
 
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
     # start simulation
 
     # create output dir, if it doesn't exist
@@ -143,17 +143,17 @@
     ## -------------END SCANNING------------- ##
     # print results at the end
     stat = output.get_actor("Stats")
     print(stat)
 
     ## ------ TESTS -------##
     dose_path = utility.scale_dose(
-        str(dose.output).replace(".mhd", "_dose.mhd"),
-        ntot / actual_sim_particles,
-        output_path / "threeDdoseWaternew.mhd",
+        str(dose.output),
+        ntot / nSim,
+        output_path / "abs_dose_roos-Scaled.mhd",
     )
 
     # ABSOLUTE DOSE
 
     # read output and ref
     img_mhd_out = itk.imread(dose_path)
     img_mhd_ref = itk.imread(
@@ -161,32 +161,29 @@
     )
     data = itk.GetArrayViewFromImage(img_mhd_out)
     data_ref = itk.GetArrayViewFromImage(img_mhd_ref)
     shape = data.shape
     spacing = img_mhd_out.GetSpacing()
     spacing_ref = np.flip(img_mhd_ref.GetSpacing())
 
-    ok = utility.assert_img_sum(
-        img_mhd_out,
-        img_mhd_ref,
-    )
+    ok = utility.assert_img_sum(img_mhd_out, img_mhd_ref, sum_tolerance=5.5)
 
     points = 400 - np.linspace(10, 14, 9)
     ok = (
         utility.compare_dose_at_points(
             points,
             data,
             data_ref,
             shape,
             data_ref.shape,
             spacing,
             spacing_ref,
             axis1="z",
             axis2="x",
-            rel_tol=0.03,
+            rel_tol=0.065,
         )
         and ok
     )
 
     # 1D
     # fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(25, 10))
     # gate.plot_img_axis(ax, img_mhd_out, "x profile", axis="z")
```

### Comparing `opengate-10.0b7/opengate/tests/src/test059_tpsource_gantry_rot.py` & `opengate-10.0b8/opengate/tests/src/test059_tpsource_optics_vbl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import itk
 import os
+import numpy as np
+import matplotlib.pyplot as plt
 from scipy.spatial.transform import Rotation
 import opengate as gate
 from opengate.tests import utility
-import opengate.element
 from opengate.contrib.beamlines.ionbeamline import BeamlineModel
 from opengate.contrib.tps.ionbeamtherapy import spots_info_from_txt, TreatmentPlanSource
 
 if __name__ == "__main__":
     # ------ INITIALIZE SIMULATION ENVIRONMENT ----------
     paths = utility.get_default_test_paths(__file__, "gate_test044_pbs")
+
     output_path = paths.output / "output_test059_rtp"
     ref_path = paths.output_ref / "test059_ref"
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
@@ -26,182 +28,181 @@
     sim.random_seed = 12365478910
     sim.random_engine = "MersenneTwister"
 
     # units
     km = gate.g4_units.km
     cm = gate.g4_units.cm
     mm = gate.g4_units.mm
+    um = gate.g4_units.um
+    MeV = gate.g4_units.MeV
+    Bq = gate.g4_units.Bq
+    nm = gate.g4_units.nm
+    deg = gate.g4_units.deg
+    rad = gate.g4_units.rad
 
     # add a material database
     sim.volume_manager.add_material_database(paths.gate_data / "HFMaterials2014.db")
 
     #  change world size
     world = sim.world
     world.size = [600 * cm, 500 * cm, 500 * cm]
 
-    ## ---------- DEFINE BEAMLINE MODEL -------------##
-    beamline = BeamlineModel()
-    beamline.name = None
-    beamline.radiation_types = "ion 6 12"
-    # Nozzle entrance to Isocenter distance
-    beamline.distance_nozzle_iso = 1300.00  # 1648 * mm#1300 * mm
-    # SMX to Isocenter distance
-    beamline.distance_stearmag_to_isocenter_x = 6700.00
-    # SMY to Isocenter distance
-    beamline.distance_stearmag_to_isocenter_y = 7420.00
-    # polinomial coefficients
-    beamline.energy_mean_coeffs = [11.91893485094217, -9.539517997860457]
-    beamline.energy_spread_coeffs = [0.0004790681841295621, 5.253257865904452]
-    beamline.sigma_x_coeffs = [2.3335753978880014]
-    beamline.theta_x_coeffs = [0.0002944903217664001]
-    beamline.epsilon_x_coeffs = [0.0007872786903040108]
-    beamline.sigma_y_coeffs = [1.9643343053823967]
-    beamline.theta_y_coeffs = [0.0007911780133478402]
-    beamline.epsilon_y_coeffs = [0.0024916149017600447]
-
-    # NOTE: HBL means that the beam is coming from -x (90 degree rot around y)
-    nSim = 20000  # particles to simulate per beam
-    # rt_plan = ref_path / "RP1.2.752.243.1.1.20220406175810679.4500.52008_tagman.dcm"
-    # beamset = BeamsetInfo(rt_plan)
-    # G = float(beamset.beam_angles[0])
-
-    ## ----  VBL Nozzle  ---
     # nozzle box
     box = sim.add_volume("Box", "box")
     box.size = [500 * mm, 500 * mm, 1000 * mm]
     box.rotation = Rotation.from_euler("x", -90, degrees=True).as_matrix()
     box.translation = [0.0, -1148 * mm, 0.0]
-    box.material = "Vacuum"
+    box.material = "Air"
     box.color = [0, 0, 1, 1]
 
     # nozzle WET
     nozzle = sim.add_volume("Box", "nozzle")
     nozzle.mother = box.name
     nozzle.size = [500 * mm, 500 * mm, 2 * mm]
     nozzle.material = "G4_WATER"
 
-    # Rashi
-    rashi = sim.add_volume("Box", "rashi")
-    rashi.mother = box.name
-    rashi.size = [500 * mm, 500 * mm, 5 * mm]
-    rashi.translation = [0.0, 0.0, 200 * mm]
-    rashi.material = "G4_LUCITE"
-    rashi.color = [1, 0, 1, 1]
-
-    ## ----  HBL Nozzle  ---
-    # FIXME : will change after volumes are refactored
-    box_rot = sim.add_volume("Box", "box_rot")
-    gate.element.copy_user_info(box, box_rot)
-    box_rot.rotation = Rotation.from_euler("y", -90, degrees=True).as_matrix()
-    box_rot.translation = [1148.0, 0.0, 1000.0]
-
-    nozzle_rot = sim.add_volume("Box", "nozzle_rot")
-    gate.element.copy_user_info(nozzle, nozzle_rot)
-    nozzle_rot.mother = box_rot.name
-
-    rashi_rot = sim.add_volume("Box", "rashi_rot")
-    gate.element.copy_user_info(rashi, rashi_rot)
-    rashi_rot.mother = box_rot.name
-
-    # -----------------------------------
-
-    # target 1 VBL
+    # target
     phantom = sim.add_volume("Box", "phantom")
-    phantom.size = [324 * mm, 324 * mm, 324 * mm]
-    phantom.translation = [0 * mm, 0.0, 0.0]
-    phantom.material = "G4_WATER"
+    phantom.size = [300 * mm, 310 * mm, 310 * mm]
+    phantom.rotation = Rotation.from_euler("z", -90, degrees=True).as_matrix()
+    phantom.translation = [0.0, -150 * mm, 0.0]
+    phantom.material = "G4_AIR"
     phantom.color = [0, 0, 1, 1]
+    sim.physics_manager.set_max_step_size(phantom.name, 0.8)
 
-    # target 2 HBL
-    phantom_rot = sim.add_volume("Box", "phantom_rot")
-    gate.element.copy_user_info(phantom, phantom_rot)
-    phantom_rot.rotation = Rotation.from_euler("z", 90, degrees=True).as_matrix()
-    phantom_rot.translation = [0.0, 0.0, 1000.0]
+    # physics
+    sim.physics_manager.physics_list_name = "FTFP_INCLXX_EMZ"
+    sim.physics_manager.set_production_cut("world", "all", 1000 * km)
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "doseInXYZ")
-    dose.output = output_path / "testTPSgantry.mhd"
+    dose.output = output_path / "TPS_optics_vbl.mhd"
     dose.mother = phantom.name
-    dose.size = [162, 1620, 162]
-    dose.spacing = [2.0, 0.2, 2.0]
+    dose.size = [30, 620, 620]
+    dose.spacing = [10.0, 0.5, 0.5]
     dose.hit_type = "random"
-    dose.gray = True
+    dose.dose = True
 
-    dose_rot = sim.add_actor("DoseActor", "doseInXYZ_rot")
-    gate.element.copy_user_info(dose, dose_rot)
-    dose_rot.mother = phantom_rot.name
-    dose_rot.output = output_path / "testTPSganry_rot.mhd"
-
-    # physics
-    sim.physics_manager.physics_list_name = "FTFP_INCLXX_EMZ"
-    sim.physics_manager.set_production_cut("world", "all", 1000 * km)
-
-    # add TPSources
-    spots, ntot, energies, G = spots_info_from_txt(
-        ref_path / "TreatmentPlan4Gate-1D_HBL_120.txt", "ion 6 12"
-    )
-    tps = TreatmentPlanSource("VBL", sim)
-    tps.set_beamline_model(beamline)
-    tps.set_particles_to_simulate(nSim)
-    tps.set_spots(spots)
-    tps.rotation = Rotation.from_euler("z", 0, degrees=True)
-    tps.initialize_tpsource()
-
-    tps_rot = TreatmentPlanSource("HBL", sim)
-    tps_rot.set_beamline_model(beamline)
-    tps_rot.set_particles_to_simulate(nSim)
-    tps_rot.set_spots(spots)
-    tps_rot.rotation = Rotation.from_euler("z", G, degrees=True)
-    tps_rot.translation = [0.0, 0.0, 1000.0]
-    tps_rot.initialize_tpsource()
+    # ---------- DEFINE BEAMLINE MODEL -------------
+    IR2VBL = BeamlineModel()
+    IR2VBL.name = None
+    IR2VBL.radiation_types = "ion 6 12"
+    # Nozzle entrance to Isocenter distance
+    IR2VBL.distance_nozzle_iso = 1300.00  # 1648 * mm#1300 * mm
+    # SMX to Isocenter distance
+    IR2VBL.distance_stearmag_to_isocenter_x = 6700.00
+    # SMY to Isocenter distance
+    IR2VBL.distance_stearmag_to_isocenter_y = 7420.00
+    # polinomial coefficients
+    IR2VBL.energy_mean_coeffs = [11.91893485094217, -9.539517997860457]
+    IR2VBL.energy_spread_coeffs = [0.0004790681841295621, 5.253257865904452]
+    IR2VBL.sigma_x_coeffs = [-0.00011142901344618727, 2.346946879501544]
+    IR2VBL.theta_x_coeffs = [-3.6368814874049214e-07, 0.0003381328996152591]
+    IR2VBL.epsilon_x_coeffs = [3.1292233857396716e-06, 0.0004117718840152502]
+    IR2VBL.sigma_y_coeffs = [-0.0004009682717802152, 2.0124504979960225]
+    IR2VBL.theta_y_coeffs = [-8.437400716390318e-07, 0.000892426821944524]
+    IR2VBL.epsilon_y_coeffs = [-8.757558864087579e-08, 0.00250212397239695]
+
+    # --------START PENCIL BEAM SCANNING----------
+    # nSim = 328935  # particles to simulate per beam
+    nSim = 20000
+    tps = sim.add_source("TreatmentPlanPBSource", "TP source")
+    tps.beam_model = IR2VBL
+    tps.n = nSim
+    tps.particle = "ion 6 12"
+    tps.plan_path = ref_path / "TreatmentPlan4Gate-gate_test59tps_v.txt"
 
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
 
     # create output dir, if it doesn't exist
     if not os.path.isdir(output_path):
         os.mkdir(output_path)
 
     # start simulation
     sim.run()
     output = sim.output
 
+    # -------------END SCANNING-------------
     # print results at the end
     stat = output.get_actor("Stats")
     print(stat)
 
-    ## ------ TESTS -------##
-
-    # ABSOLUTE DOSE
-    # ok = utility.assert_images(
-    #     dose.output,
-    #     dose_rot.output,
-    #     stat,
-    #     tolerance=50,
-    #     ignore_value=0,
+    # ------ TESTS -------
+    # dose_path = utility.scale_dose(
+    #     str(dose.output).replace(".mhd", "_dose.mhd"),
+    #     ntot / actual_sim_particles,
     # )
-    ok = True
 
+    # SPOT POSITIONS COMPARISON
     # read output and ref
-    img_mhd_out = itk.imread(dose_rot.output)
-    img_mhd_ref = itk.imread(dose.output)
+    img_mhd_out = itk.imread(dose.output)
+    img_mhd_ref = itk.imread(
+        ref_path / "idc-PHANTOM-air_box_vbl-gate_test59tps_v-PLAN-Physical.mhd"
+    )
     data = itk.GetArrayViewFromImage(img_mhd_out)
     data_ref = itk.GetArrayViewFromImage(img_mhd_ref)
+    shape = data.shape
     spacing = img_mhd_out.GetSpacing()
 
-    # Range 80
-    ok = (
-        utility.compareRange(
-            data, data_ref, data.shape, data_ref.shape, spacing, spacing
-        )
-        and ok
-    )
+    # spot comparison (N.B x and z are inverted in np array!)
+    # spots in the plan file
+    yz = [
+        0,
+        50,
+        0,
+        0,
+        -62.507,
+        -21.669,
+        -61.951,
+        -72.23,
+        50,
+        -50,
+        50,
+        0,
+        50,
+        50,
+        -50,
+        50,
+    ]
+
+    yzM = np.array(yz).reshape(int(len(yz) / 2), 2)
+    # convert from mm (wrt image center) to voxel
+    spot_y = [int(y / dose.spacing[1]) + int(dose.size[1] / 2) for y in yzM[:, 0]]
+    spot_z = [int(z / dose.spacing[1]) + int(dose.size[1] / 2) for z in yzM[:, 1]]
+
+    thresh = 0.105
+
+    # 1D
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(25, 10))
+    utility.plot_img_axis(ax, img_mhd_out, "z profile", axis="z")
+    utility.plot_img_axis(ax, img_mhd_out, "x profile", axis="x")
+    utility.plot_img_axis(ax, img_mhd_out, "y profile", axis="y")
 
-    # 1D plots
     # fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(25, 10))
-    # gate.plot_img_axis(ax, img_mhd_out, "y profile", axis="y")
-    # gate.plot_img_axis(ax, img_mhd_ref, "y ref", axis="y")
-    # fig.savefig(output_path / "dose_profiles_water.png")
-    # plt.show()
+    utility.plot_img_axis(ax, img_mhd_ref, "z ref", axis="z")
+    utility.plot_img_axis(ax, img_mhd_ref, "x ref", axis="x")
+    utility.plot_img_axis(ax, img_mhd_ref, "y ref", axis="y")
+    fig.savefig(output_path / "dose_profiles_spots_vbl.png")
+
+    ok = True
+    for i in range(1, shape[2], shape[2] // 3):
+        # check i-th slab
+        print(f"Airslab nr. {i}")
+        # gate.plot2D(data[:, :, i], "2D Edep opengate", show=True)
+        # gate.plot2D(data_ref[:, :, i], "2D Edep gate", show=True)
+        for y, z in zip(spot_y, spot_z):
+            # i = 0
+            print(f" ({y:.2f},{z:.2f})")
+            # 'cut' the slab around the spot expected in y,z
+            w = 30  # cut window's half size
+            d_out = data[z - w : z + w, y - w : y + w, i : i + 1]
+            d_ref = data_ref[z - w : z + w, y - w : y + w, i : i + 1]
+            ok = (
+                utility.test_tps_spot_size_positions(
+                    d_out, d_ref, spacing, thresh=thresh, abs_tol=0.3
+                )
+                and ok
+            )
 
     utility.test_ok(ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test059_tpsource_optics.py` & `opengate-10.0b8/opengate/tests/src/test059_tpsource_optics.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import numpy as np
 from scipy.spatial.transform import Rotation
 import opengate as gate
 from opengate.tests import utility
 from opengate.contrib.beamlines.ionbeamline import BeamlineModel
 from opengate.contrib.tps.ionbeamtherapy import spots_info_from_txt, TreatmentPlanSource
 
-
 if __name__ == "__main__":
     # ------ INITIALIZE SIMULATION ENVIRONMENT ----------
     paths = utility.get_default_test_paths(__file__, "gate_test044_pbs")
+
     output_path = paths.output / "output_test059_rtp"
     ref_path = paths.output_ref / "test059_ref"
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
@@ -63,33 +63,30 @@
     phantom = sim.add_volume("Box", "phantom")
     phantom.size = [300 * mm, 310 * mm, 310 * mm]
     phantom.translation = [150 * mm, 0.0, 0.0]
     # phantom.rotation = Rotation.from_euler('x',-90,degrees=True).as_matrix()
     phantom.material = "G4_AIR"
     phantom.color = [0, 0, 1, 1]
     sim.physics_manager.set_max_step_size(phantom.name, 0.8)
+    sim.physics_manager.set_user_limits_particles("all")
 
     # physics
-    sim.physics_manager.physics_list_name = (
-        "FTFP_INCLXX_EMZ"  # "Shielding_EMZ"#"FTFP_INCLXX_EMZ"
-    )
-
-    # p.physics_list_name = "QGSP_BIC_EMZ"
+    sim.physics_manager.physics_list_name = "FTFP_INCLXX_EMZ"
     sim.physics_manager.set_production_cut("world", "all", 1000 * km)
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "doseInXYZ")
     dose.output = output_path / "testTPSoptics.mhd"
     dose.mother = phantom.name
     dose.size = [30, 620, 620]
     dose.spacing = [10.0, 0.5, 0.5]
     dose.hit_type = "random"
-    dose.gray = True
+    dose.dose = True
 
-    ## ---------- DEFINE BEAMLINE MODEL -------------##
+    # ---------- DEFINE BEAMLINE MODEL -------------
     IR2HBL = BeamlineModel()
     IR2HBL.name = None
     IR2HBL.radiation_types = "ion 6 12"
     # Nozzle entrance to Isocenter distance
     IR2HBL.distance_nozzle_iso = 1300.00  # 1648 * mm#1300 * mm
     # SMX to Isocenter distance
     IR2HBL.distance_stearmag_to_isocenter_x = 6700.00
@@ -101,58 +98,54 @@
     IR2HBL.sigma_x_coeffs = [-0.00011142901344618727, 2.346946879501544]
     IR2HBL.theta_x_coeffs = [-3.6368814874049214e-07, 0.0003381328996152591]
     IR2HBL.epsilon_x_coeffs = [3.1292233857396716e-06, 0.0004117718840152502]
     IR2HBL.sigma_y_coeffs = [-0.0004009682717802152, 2.0124504979960225]
     IR2HBL.theta_y_coeffs = [-8.437400716390318e-07, 0.000892426821944524]
     IR2HBL.epsilon_y_coeffs = [-8.757558864087579e-08, 0.00250212397239695]
 
-    ## --------START PENCIL BEAM SCANNING---------- ##
+    # --------START PENCIL BEAM SCANNING----------
     # NOTE: HBL means that the beam is coming from -x (90 degree rot around y)
     # nSim = 328935  # particles to simulate per beam
     nSim = 20000
-    spots, ntot, energies, G = spots_info_from_txt(
-        ref_path / "TreatmentPlan4Gate-gate_test59_TP_1_old.txt", "ion 6 12"
+    beam_data_dict = spots_info_from_txt(
+        ref_path / "TreatmentPlan4Gate-gate_test59_TP_1_old.txt", "ion 6 12", beam_nr=1
     )
-    tps = TreatmentPlanSource("RT_plan", sim)
-    tps.set_beamline_model(IR2HBL)
-    tps.set_particles_to_simulate(nSim)
-    tps.set_spots(spots)
-    tps.rotation = Rotation.from_euler("z", G, degrees=True)
-    # rt_plan = ref_path / "RP1.2.752.243.1.1.20230119115736709.2000.75541.dcm"
-    # tps.set_spots_from_rtplan(rt_plan) # no need to set rotation here
-    tps.initialize_tpsource()
-    actual_sim_particles = tps.actual_sim_particles
-
+    ntot = beam_data_dict["msw_beam"]
+    tps = sim.add_source("TreatmentPlanPBSource", "TP source")
+    tps.beam_model = IR2HBL
+    tps.n = nSim
+    tps.particle = "ion 6 12"
+    tps.beam_data_dict = beam_data_dict
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
 
     # create output dir, if it doesn't exist
     if not os.path.isdir(output_path):
         os.mkdir(output_path)
 
     # start simulation
     sim.run()
     output = sim.output
 
-    ## -------------END SCANNING------------- ##
+    # -------------END SCANNING------------- #
     # print results at the end
     stat = output.get_actor("Stats")
+    d_fPath = output_path / output.get_actor("doseInXYZ").user_info.output
     print(stat)
 
-    ## ------ TESTS -------##
-    dose_path = utility.scale_dose(
-        str(dose.output).replace(".mhd", "_dose.mhd"),
-        ntot / actual_sim_particles,
-        output_path / "threeDdoseAirSpots.mhd",
-    )
+    # ------ TESTS -------#
+    # dose_path = utility.scale_dose(
+    #     str(dose.output).replace(".mhd", "_dose.mhd"),
+    #     ntot / actual_sim_particles,
+    # )
 
     # SPOT POSITIONS COMPARISON
     # read output and ref
-    img_mhd_out = itk.imread(dose_path)
+    img_mhd_out = itk.imread(dose.output)
     img_mhd_ref = itk.imread(
         ref_path / "idc-PHANTOM-air_box-gate_test59_TP_1-PLAN-Physical.mhd"
     )
     data = itk.GetArrayViewFromImage(img_mhd_out)
     data_ref = itk.GetArrayViewFromImage(img_mhd_ref)
     shape = data.shape
     spacing = img_mhd_out.GetSpacing()
@@ -189,15 +182,15 @@
     ]
 
     yzM = np.array(yz).reshape(int(len(yz) / 2), 2)
     # convert from mm (wrt image center) to voxel
     spot_y = [int(y / dose.spacing[1]) + int(dose.size[1] / 2) for y in yzM[:, 0]]
     spot_z = [int(z / dose.spacing[1]) + int(dose.size[1] / 2) for z in yzM[:, 1]]
 
-    thresh = 0.1
+    thresh = 0.105
 
     # # 1D
     # fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(25, 10))
     # gate.plot_img_axis(ax, img_mhd_out, "z profile", axis="z")
     # #gate.plot_img_axis(ax, img_mhd_out, "x profile", axis="x")
     # gate.plot_img_axis(ax, img_mhd_out, "y profile", axis="y")
```

### Comparing `opengate-10.0b7/opengate/tests/src/test059_tpsource_optics_vbl.py` & `opengate-10.0b8/opengate/tests/src/test059_tpsource_gantry_rot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import itk
 import os
-import numpy as np
-import matplotlib.pyplot as plt
 from scipy.spatial.transform import Rotation
 import opengate as gate
 from opengate.tests import utility
+import opengate.element
 from opengate.contrib.beamlines.ionbeamline import BeamlineModel
 from opengate.contrib.tps.ionbeamtherapy import spots_info_from_txt, TreatmentPlanSource
 
 if __name__ == "__main__":
     # ------ INITIALIZE SIMULATION ENVIRONMENT ----------
     paths = utility.get_default_test_paths(__file__, "gate_test044_pbs")
+
     output_path = paths.output / "output_test059_rtp"
     ref_path = paths.output_ref / "test059_ref"
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
@@ -27,187 +27,195 @@
     sim.random_seed = 12365478910
     sim.random_engine = "MersenneTwister"
 
     # units
     km = gate.g4_units.km
     cm = gate.g4_units.cm
     mm = gate.g4_units.mm
-    um = gate.g4_units.um
-    MeV = gate.g4_units.MeV
-    Bq = gate.g4_units.Bq
-    nm = gate.g4_units.nm
-    deg = gate.g4_units.deg
-    rad = gate.g4_units.rad
+    s = gate.g4_units.s
 
     # add a material database
     sim.volume_manager.add_material_database(paths.gate_data / "HFMaterials2014.db")
 
     #  change world size
     world = sim.world
     world.size = [600 * cm, 500 * cm, 500 * cm]
 
+    ## ---------- DEFINE BEAMLINE MODEL -------------##
+    beamline = BeamlineModel()
+    beamline.name = None
+    beamline.radiation_types = "ion 6 12"
+    # Nozzle entrance to Isocenter distance
+    beamline.distance_nozzle_iso = 1300.00  # 1648 * mm#1300 * mm
+    # SMX to Isocenter distance
+    beamline.distance_stearmag_to_isocenter_x = 6700.00
+    # SMY to Isocenter distance
+    beamline.distance_stearmag_to_isocenter_y = 7420.00
+    # polinomial coefficients
+    beamline.energy_mean_coeffs = [11.91893485094217, -9.539517997860457]
+    beamline.energy_spread_coeffs = [0.0004790681841295621, 5.253257865904452]
+    beamline.sigma_x_coeffs = [2.3335753978880014]
+    beamline.theta_x_coeffs = [0.0002944903217664001]
+    beamline.epsilon_x_coeffs = [0.0007872786903040108]
+    beamline.sigma_y_coeffs = [1.9643343053823967]
+    beamline.theta_y_coeffs = [0.0007911780133478402]
+    beamline.epsilon_y_coeffs = [0.0024916149017600447]
+
+    # NOTE: HBL means that the beam is coming from -x (90 degree rot around y)
+    nSim = 20000  # particles to simulate per beam
+    # rt_plan = ref_path / "RP1.2.752.243.1.1.20220406175810679.4500.52008_tagman.dcm"
+    # beamset = BeamsetInfo(rt_plan)
+    # G = float(beamset.beam_angles[0])
+
+    ## ----  VBL Nozzle  ---
     # nozzle box
     box = sim.add_volume("Box", "box")
     box.size = [500 * mm, 500 * mm, 1000 * mm]
     box.rotation = Rotation.from_euler("x", -90, degrees=True).as_matrix()
     box.translation = [0.0, -1148 * mm, 0.0]
-    box.material = "Air"
+    box.material = "Vacuum"
     box.color = [0, 0, 1, 1]
 
     # nozzle WET
     nozzle = sim.add_volume("Box", "nozzle")
     nozzle.mother = box.name
     nozzle.size = [500 * mm, 500 * mm, 2 * mm]
     nozzle.material = "G4_WATER"
 
-    # target
+    # Rashi
+    rashi = sim.add_volume("Box", "rashi")
+    rashi.mother = box.name
+    rashi.size = [500 * mm, 500 * mm, 5 * mm]
+    rashi.translation = [0.0, 0.0, 200 * mm]
+    rashi.material = "G4_LUCITE"
+    rashi.color = [1, 0, 1, 1]
+
+    ## ----  HBL Nozzle  ---
+    # FIXME : will change after volumes are refactored
+    box_rot = sim.add_volume("Box", "box_rot")
+    box_rot.copy_user_info(box)
+    box_rot.rotation = Rotation.from_euler("y", -90, degrees=True).as_matrix()
+    box_rot.translation = [1148.0, 0.0, 1000.0]
+
+    nozzle_rot = sim.add_volume("Box", "nozzle_rot")
+    nozzle_rot.copy_user_info(nozzle)
+    nozzle_rot.mother = box_rot.name
+
+    rashi_rot = sim.add_volume("Box", "rashi_rot")
+    rashi_rot.copy_user_info(rashi)
+    rashi_rot.mother = box_rot.name
+
+    # -----------------------------------
+
+    # target 1 VBL
     phantom = sim.add_volume("Box", "phantom")
-    phantom.size = [300 * mm, 310 * mm, 310 * mm]
-    phantom.rotation = Rotation.from_euler("z", -90, degrees=True).as_matrix()
-    phantom.translation = [0.0, -150 * mm, 0.0]
-    phantom.material = "G4_AIR"
+    phantom.size = [324 * mm, 324 * mm, 324 * mm]
+    phantom.translation = [0 * mm, 0.0, 0.0]
+    phantom.material = "G4_WATER"
     phantom.color = [0, 0, 1, 1]
-    sim.physics_manager.set_max_step_size(phantom.name, 0.8)
 
-    # physics
-    sim.physics_manager.physics_list_name = "FTFP_INCLXX_EMZ"
-    sim.physics_manager.set_production_cut("world", "all", 1000 * km)
+    # target 2 HBL
+    phantom_rot = sim.add_volume("Box", "phantom_rot")
+    phantom_rot.copy_user_info(phantom)
+    phantom_rot.rotation = Rotation.from_euler("z", 90, degrees=True).as_matrix()
+    phantom_rot.translation = [0.0, 0.0, 1000.0]
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "doseInXYZ")
-    dose.output = output_path / "TPS_optics_vbl.mhd"
+    dose.output = output_path / "testTPSgantry.mhd"
     dose.mother = phantom.name
-    dose.size = [30, 620, 620]
-    dose.spacing = [10.0, 0.5, 0.5]
+    dose.size = [162, 1620, 162]
+    dose.spacing = [2.0, 0.2, 2.0]
     dose.hit_type = "random"
-    dose.gray = True
+    dose.dose = True
 
-    # ---------- DEFINE BEAMLINE MODEL -------------
-    IR2VBL = BeamlineModel()
-    IR2VBL.name = None
-    IR2VBL.radiation_types = "ion 6 12"
-    # Nozzle entrance to Isocenter distance
-    IR2VBL.distance_nozzle_iso = 1300.00  # 1648 * mm#1300 * mm
-    # SMX to Isocenter distance
-    IR2VBL.distance_stearmag_to_isocenter_x = 6700.00
-    # SMY to Isocenter distance
-    IR2VBL.distance_stearmag_to_isocenter_y = 7420.00
-    # polinomial coefficients
-    IR2VBL.energy_mean_coeffs = [11.91893485094217, -9.539517997860457]
-    IR2VBL.energy_spread_coeffs = [0.0004790681841295621, 5.253257865904452]
-    IR2VBL.sigma_x_coeffs = [-0.00011142901344618727, 2.346946879501544]
-    IR2VBL.theta_x_coeffs = [-3.6368814874049214e-07, 0.0003381328996152591]
-    IR2VBL.epsilon_x_coeffs = [3.1292233857396716e-06, 0.0004117718840152502]
-    IR2VBL.sigma_y_coeffs = [-0.0004009682717802152, 2.0124504979960225]
-    IR2VBL.theta_y_coeffs = [-8.437400716390318e-07, 0.000892426821944524]
-    IR2VBL.epsilon_y_coeffs = [-8.757558864087579e-08, 0.00250212397239695]
-
-    # --------START PENCIL BEAM SCANNING----------
-    # nSim = 328935  # particles to simulate per beam
-    nSim = 20000
-    spots, ntot, energies, G = spots_info_from_txt(
-        ref_path / "TreatmentPlan4Gate-gate_test59tps_v.txt", "ion 6 12"
+    dose_rot = sim.add_actor("DoseActor", "doseInXYZ_rot")
+    gate.element.copy_user_info(dose, dose_rot)
+    dose_rot.mother = phantom_rot.name
+    dose_rot.output = output_path / "testTPSganry_rot.mhd"
+
+    # physics
+    sim.physics_manager.physics_list_name = "FTFP_INCLXX_EMZ"
+    sim.physics_manager.set_production_cut("world", "all", 1000 * km)
+
+    # add TPSources
+    beam_data_dict = spots_info_from_txt(
+        ref_path / "TreatmentPlan4Gate-1D_HBL_120.txt", "ion 6 12", beam_nr=1
     )
-    tps = TreatmentPlanSource("RT_plan", sim)
-    tps.set_beamline_model(IR2VBL)
-    tps.set_particles_to_simulate(nSim)
-    tps.set_spots(spots)
-    tps.rotation = Rotation.from_euler("z", G, degrees=True)
-    tps.initialize_tpsource()
-    actual_sim_particles = tps.actual_sim_particles
+
+    tps_rot = sim.add_source("TreatmentPlanPBSource", "HBL")
+    tps_rot.n = nSim
+    tps_rot.end_time = 0.5 * s
+    tps_rot.beam_model = beamline
+    tps_rot.beam_data_dict = beam_data_dict
+    tps_rot.beam_nr = 1
+    tps_rot.particle = "ion 6 12"
+    tps_rot.position.translation = [0.0, 0.0, 1000.0]
+    tps_rot.sorted_spot_generation = True
+
+    beam_data_dict_vbl = beam_data_dict.copy()
+    beam_data_dict_vbl["gantry_angle"] = 0
+
+    tps = sim.add_source("TreatmentPlanPBSource", "VBL")
+    tps.n = nSim
+    tps.start_time = 0.5 * s
+    tps.beam_model = beamline
+    tps.beam_data_dict = beam_data_dict_vbl
+    tps.beam_nr = 1
+    tps.particle = "ion 6 12"
+    tps.sorted_spot_generation = True
 
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
 
     # create output dir, if it doesn't exist
     if not os.path.isdir(output_path):
         os.mkdir(output_path)
 
     # start simulation
     sim.run()
     output = sim.output
 
-    # -------------END SCANNING-------------
     # print results at the end
     stat = output.get_actor("Stats")
     print(stat)
 
-    # ------ TESTS -------
-    dose_path = utility.scale_dose(
-        str(dose.output).replace(".mhd", "_dose.mhd"),
-        ntot / actual_sim_particles,
-        output_path / "threeDdoseAirSpots_vbl.mhd",
-    )
+    ## ------ TESTS -------##
+
+    # ABSOLUTE DOSE
+    # ok = utility.assert_images(
+    #     dose.output,
+    #     dose_rot.output,
+    #     stat,
+    #     tolerance=50,
+    #     ignore_value=0,
+    # )
+    ok = True
 
-    # SPOT POSITIONS COMPARISON
     # read output and ref
-    img_mhd_out = itk.imread(dose_path)
+    img_mhd_out = itk.imread(
+        output_path / output.get_actor("doseInXYZ_rot").user_info.output
+    )
     img_mhd_ref = itk.imread(
-        ref_path / "idc-PHANTOM-air_box_vbl-gate_test59tps_v-PLAN-Physical.mhd"
+        output_path / output.get_actor("doseInXYZ").user_info.output
     )
     data = itk.GetArrayViewFromImage(img_mhd_out)
     data_ref = itk.GetArrayViewFromImage(img_mhd_ref)
-    shape = data.shape
     spacing = img_mhd_out.GetSpacing()
 
-    # spot comparison (N.B x and z are inverted in np array!)
-    # spots in the plan file
-    yz = [
-        0,
-        50,
-        0,
-        0,
-        -62.507,
-        -21.669,
-        -61.951,
-        -72.23,
-        50,
-        -50,
-        50,
-        0,
-        50,
-        50,
-        -50,
-        50,
-    ]
-
-    yzM = np.array(yz).reshape(int(len(yz) / 2), 2)
-    # convert from mm (wrt image center) to voxel
-    spot_y = [int(y / dose.spacing[1]) + int(dose.size[1] / 2) for y in yzM[:, 0]]
-    spot_z = [int(z / dose.spacing[1]) + int(dose.size[1] / 2) for z in yzM[:, 1]]
-
-    thresh = 0.1
-
-    # 1D
-    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(25, 10))
-    utility.plot_img_axis(ax, img_mhd_out, "z profile", axis="z")
-    utility.plot_img_axis(ax, img_mhd_out, "x profile", axis="x")
-    utility.plot_img_axis(ax, img_mhd_out, "y profile", axis="y")
+    # Range 80
+    ok = (
+        utility.compareRange(
+            data, data_ref, data.shape, data_ref.shape, spacing, spacing
+        )
+        and ok
+    )
 
+    # 1D plots
     # fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(25, 10))
-    utility.plot_img_axis(ax, img_mhd_ref, "z ref", axis="z")
-    utility.plot_img_axis(ax, img_mhd_ref, "x ref", axis="x")
-    utility.plot_img_axis(ax, img_mhd_ref, "y ref", axis="y")
-    fig.savefig(output_path / "dose_profiles_spots_vbl.png")
-
-    ok = True
-    for i in range(1, shape[2], shape[2] // 3):
-        # check i-th slab
-        print(f"Airslab nr. {i}")
-        # gate.plot2D(data[:, :, i], "2D Edep opengate", show=True)
-        # gate.plot2D(data_ref[:, :, i], "2D Edep gate", show=True)
-        for y, z in zip(spot_y, spot_z):
-            # i = 0
-            print(f" ({y:.2f},{z:.2f})")
-            # 'cut' the slab around the spot expected in y,z
-            w = 30  # cut window's half size
-            d_out = data[z - w : z + w, y - w : y + w, i : i + 1]
-            d_ref = data_ref[z - w : z + w, y - w : y + w, i : i + 1]
-            ok = (
-                utility.test_tps_spot_size_positions(
-                    d_out, d_ref, spacing, thresh=thresh, abs_tol=0.3
-                )
-                and ok
-            )
+    # gate.plot_img_axis(ax, img_mhd_out, "y profile", axis="y")
+    # gate.plot_img_axis(ax, img_mhd_ref, "y ref", axis="y")
+    # fig.savefig(output_path / "dose_profiles_water.png")
+    # plt.show()
 
     utility.test_ok(ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test059_tpsource_range_ref.py` & `opengate-10.0b8/opengate/tests/src/test059_tpsource_range_ref.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from opengate.tests import utility
 from opengate.contrib.beamlines.ionbeamline import BeamlineModel
 from opengate.contrib.tps.ionbeamtherapy import TreatmentPlanSource, spots_info_from_txt
 
 if __name__ == "__main__":
     # ------ INITIALIZE SIMULATION ENVIRONMENT ----------
     paths = utility.get_default_test_paths(__file__, "gate_test044_pbs")
+
     output_path = paths.output / "output_test059_rtp"
     ref_path = paths.output_ref / "test059_ref"
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
@@ -71,27 +72,25 @@
     peak_finder.material = "G4_WATER"
     peak_finder.rmax = 40.3
     peak_finder.rmin = 0
     peak_finder.dz = 200
     peak_finder.color = [1, 0, 1, 1]
 
     # physics
-    sim.physics_manager.physics_list_name = (
-        "FTFP_INCLXX_EMZ"  # 'QGSP_BIC_HP_EMZ' #"FTFP_INCLXX_EMZ"
-    )
+    sim.physics_manager.physics_list_name = "FTFP_INCLXX_EMZ"
     sim.physics_manager.set_production_cut("world", "all", 1000 * km)
 
     # add dose actor
     dose = sim.add_actor("DoseActor", "doseInXYZ")
     dose.output = output_path / "dose_peak_finder.mhd"
     dose.mother = peak_finder.name
     dose.size = [1, 1, 8000]
     dose.spacing = [80.6, 80.6, 0.05]
     dose.hit_type = "random"
-    dose.gray = True
+    dose.dose = True
 
     # ---------- DEFINE BEAMLINE MODEL -------------
     IR2HBL = BeamlineModel()
     IR2HBL.name = None
     IR2HBL.radiation_types = "ion 6 12"
     # Nozzle entrance to Isocenter distance
     IR2HBL.distance_nozzle_iso = 1300.00  # 1648 * mm#1300 * mm
@@ -107,24 +106,21 @@
     IR2HBL.epsilon_x_coeffs = [0.00078]
     IR2HBL.sigma_y_coeffs = [1.96]
     IR2HBL.theta_y_coeffs = [0.00079]
     IR2HBL.epsilon_y_coeffs = [0.0024]
 
     # --------START PENCIL BEAM SCANNING----------
     # NOTE: HBL means that the beam is coming from -x (90 degree rot around y)
-    nSim = 20000  # 328935  # particles to simulate per beam
-    spots, ntot, energies, G = spots_info_from_txt(
-        ref_path / "PlanCentralSpot_1440MeV.txt", "ion 6 12"
-    )
-    tps = TreatmentPlanSource("RT_plan", sim)
-    tps.set_beamline_model(IR2HBL)
-    tps.set_particles_to_simulate(nSim)
-    tps.set_spots(spots)
-    tps.rotation = Rotation.from_euler("z", G, degrees=True)
-    tps.initialize_tpsource()
+
+    tps = sim.add_source("TreatmentPlanPBSource", "TPSource")
+    tps.n = 20000
+    tps.beam_model = IR2HBL
+    tps.plan_path = ref_path / "PlanCentralSpot_1440MeV.txt"
+    tps.beam_nr = 1
+    tps.particle = "ion 6 12"
 
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
 
     # create output dir, if it doesn't exist
     if not os.path.isdir(output_path):
@@ -135,16 +131,16 @@
     output = sim.output
 
     # -------------END SCANNING-------------
     # print results at the end
     stat = output.get_actor("Stats")
     print(stat)
 
-    # ------ TESTS -------
-    dose_path = str(dose.output).replace(".mhd", "_dose.mhd")
+    ## ------ TESTS -------##
+    dose_path = output_path / output.get_actor("doseInXYZ").user_info.output
 
     # RANGE
 
     # read output and ref
     img_mhd_out = itk.imread(dose_path)
     data = itk.GetArrayViewFromImage(img_mhd_out)
     shape = data.shape
```

### Comparing `opengate-10.0b7/opengate/tests/src/test059_tpsource_weights.py` & `opengate-10.0b8/opengate/tests/src/test059_tpsource_weights.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     # main options
     sim.g4_verbose = False
     sim.g4_verbose_level = 1
     sim.visu = False
     sim.random_seed = 123654789
     sim.random_engine = "MersenneTwister"
+    # sim.number_of_threads = 16
 
     # units
     km = gate.g4_units.km
     cm = gate.g4_units.cm
     mm = gate.g4_units.mm
     um = gate.g4_units.um
     MeV = gate.g4_units.MeV
@@ -112,24 +113,24 @@
     beamline.theta_x_coeffs = [2.3335754e-3]
     beamline.epsilon_x_coeffs = [0.00078728e-3]
     beamline.sigma_y_coeffs = [1.96433431]
     beamline.theta_y_coeffs = [0.00079118e-3]
     beamline.epsilon_y_coeffs = [0.00249161e-3]
 
     # tps
-    nSim = 60000  # particles to simulate per beam
-    spots, ntot, energies, G = spots_info_from_txt(
-        ref_path / "TreatmentPlan2Spots.txt", "proton"
-    )
-    tps = TreatmentPlanSource("test", sim)
-    tps.set_beamline_model(beamline)
-    tps.set_particles_to_simulate(nSim)
-    tps.set_spots(spots)
-    tps.rotation = Rotation.from_euler("x", 90, degrees=True)
-    tps.initialize_tpsource()
+    nSim = 80000  # particles to simulate per beam
+
+    tps = sim.add_source("TreatmentPlanPBSource", "TPSource")
+    tps.n = nSim
+    tps.beam_model = beamline
+    tps.plan_path = ref_path / "TreatmentPlan2Spots.txt"
+    tps.beam_nr = 1
+    tps.gantry_rot_axis = "x"
+    # tps.sorted_spot_gneration = True
+    tps.particle = "proton"
 
     # add stat actor
     s = sim.add_actor("SimulationStatisticsActor", "Stats")
     s.track_types_flag = True
 
     # physics
     sim.physics_manager.physics_list_name = "FTFP_INCLXX_EMZ"
@@ -152,16 +153,16 @@
     # tests
 
     # energy deposition: we expect the edep from source two
     # to be double the one of source one
 
     print("Compare tps Edep to single pb sources")
     print(" --------------------------------------- ")
-    mhd_1 = "phantom_a_1.mhd"
-    mhd_2 = "phantom_a_2.mhd"
+    mhd_1 = output.get_actor("doseInYZ_1").user_info.output
+    mhd_2 = output.get_actor("doseInYZ_2").user_info.output
     test = True
 
     # check first spot
     test = (
         utility.assert_images(
             ref_path / mhd_1,
             output_path / mhd_1,
```

### Comparing `opengate-10.0b7/opengate/tests/src/test060_phsp_source_helpers.py` & `opengate-10.0b8/opengate/tests/src/test060_phsp_source_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,42 +2,43 @@
 # -*- coding: utf-8 -*-
 
 import os
 from scipy.spatial.transform import Rotation
 import gatetools.phsp as phsp
 import opengate as gate
 from opengate.tests import utility
+from pathlib import Path
 
 # units
 m = gate.g4_units.m
 mm = gate.g4_units.mm
 cm = gate.g4_units.cm
 nm = gate.g4_units.nm
 Bq = gate.g4_units.Bq
 MeV = gate.g4_units.MeV
 deg = gate.g4_units.deg
 
 
 def create_test_phs(
     particle="proton",
-    phs_name="output/test_proton.root",
+    phs_name=Path("output") / "test_proton.root",
     number_of_particles=1,
     translation=[0 * mm, 0 * mm, 0 * mm],
 ):
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
     # sim.visu = True
     sim.visu_type = "vrml"
     sim.check_volumes_overlap = False
     # sim.running_verbose_level = gate.EVENT
     sim.number_of_threads = 1
-    sim.random_seed = "auto"
+    sim.random_seed = 987654321
 
     # units
     m = gate.g4_units.m
     cm = gate.g4_units.cm
     nm = gate.g4_units.nm
     MeV = gate.g4_units.MeV
 
@@ -165,27 +166,27 @@
     source.energy.mono = 150 * MeV
     source.n = number_of_particles
 
     sim.run(start_new_process=True)
 
 
 def create_phs_without_source(
-    phs_name="output/test_proton.root",
+    phs_name=Path("output") / "test_proton.root",
 ):
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     sim.g4_verbose = False
     # sim.visu = True
     sim.visu_type = "vrml"
     sim.check_volumes_overlap = False
     # sim.running_verbose_level = gate.EVENT
     sim.number_of_threads = 1
-    sim.random_seed = "auto"
+    sim.random_seed = 987654321
 
     # units
     m = gate.g4_units.m
     mm = gate.g4_units.mm
     cm = gate.g4_units.cm
     nm = gate.g4_units.nm
     Bq = gate.g4_units.Bq
@@ -255,16 +256,16 @@
     # output = sim.run()
     # output = sim.start()
     # output = sim.start(start_new_process=True)
     return sim
 
 
 def test_source_name(
-    source_file_name="output/test_proton_offset.root",
-    phs_file_name_out="output/output/test_source_electron.root",
+    source_file_name=Path("output") / "test_proton_offset.root",
+    phs_file_name_out=Path("output") / "output/test_source_electron.root",
 ) -> None:
     sim = create_phs_without_source(
         phs_name=phs_file_name_out,
     )
     particle = "e-"
     number_of_particles = 1
     ##########################################################################################
@@ -282,16 +283,16 @@
     source.n = number_of_particles
     # source.position.translation = [0 * cm, 0 * cm, -35 * cm]
 
     sim.run()
 
 
 def test_source_particle_info_from_phs(
-    source_file_name="output/test_proton_offset.root",
-    phs_file_name_out="output/test_source_PDG_proton.root",
+    source_file_name=Path("output") / "test_proton_offset.root",
+    phs_file_name_out=Path("output") / "test_source_PDG_proton.root",
 ) -> None:
     sim = create_phs_without_source(
         phs_name=phs_file_name_out,
     )
     number_of_particles = 1
     ##########################################################################################
     #  Source
@@ -308,16 +309,16 @@
     source.n = number_of_particles
     # source.position.translation = [0 * cm, 0 * cm, -35 * cm]
 
     sim.run()
 
 
 def test_source_translation(
-    source_file_name="output/test_proton_offset.root",
-    phs_file_name_out="output/output/test_source_electron.root",
+    source_file_name=Path("output") / "test_proton_offset.root",
+    phs_file_name_out=Path("output") / "output/test_source_electron.root",
 ) -> None:
     sim = create_phs_without_source(
         phs_name=phs_file_name_out,
     )
     number_of_particles = 1
     ##########################################################################################
     #  Source
@@ -336,16 +337,16 @@
     source.position.translation = [3 * cm, 0 * cm, 0 * cm]
     print(source)
 
     sim.run()
 
 
 def test_source_rotation(
-    source_file_name="output/test_proton_offset.root",
-    phs_file_name_out="output/output/test_source_electron.root",
+    source_file_name=Path("output") / "test_proton_offset.root",
+    phs_file_name_out=Path("output") / "output/test_source_electron.root",
 ) -> None:
     sim = create_phs_without_source(
         phs_name=phs_file_name_out,
     )
     number_of_particles = 1
     ##########################################################################################
     #  Source
@@ -368,16 +369,16 @@
     source.position.rotation = rotation.as_matrix()
     print(source)
 
     sim.run()
 
 
 def test_source_untilPrimary(
-    source_file_name="output/test_proton_offset.root",
-    phs_file_name_out="output/output/test_source_electron.root",
+    source_file_name=Path("output") / "test_proton_offset.root",
+    phs_file_name_out=Path("output") / "output/test_source_electron.root",
 ) -> None:
     sim = create_phs_without_source(
         phs_name=phs_file_name_out,
     )
     number_of_particles = 2
     ##########################################################################################
     #  Source
@@ -398,28 +399,28 @@
     print(source)
 
     sim.run()
     output = sim.output
 
 
 def get_first_entry_of_key(
-    file_name_root="output/test_source_electron.root", key="ParticleName"
+    file_name_root=Path("output") / "test_source_electron.root", key="ParticleName"
 ) -> None:
     # read root file
     data_ref, keys_ref, m_ref = phsp.load(file_name_root)
     # print(data_ref)
     # print(keys_ref)
     index = keys_ref.index(key)
     # print(index)
     # print(data_ref[index][0])
     return data_ref[0][index]
 
 
 def check_value_from_root_file(
-    file_name_root="output/test_source_electron.root",
+    file_name_root=Path("output") / "test_source_electron.root",
     key="ParticleName",
     ref_value="e-",
 ):
     # read root file
     value = get_first_entry_of_key(file_name_root=file_name_root, key=key)
     if (type(ref_value) != str) and (type(value) != str):
         is_ok = utility.check_diff_abs(
```

### Comparing `opengate-10.0b7/opengate/tests/src/test060_phsp_source_particletype_direct.py` & `opengate-10.0b8/opengate/tests/src/test060_phsp_source_particletype_direct.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test060_phsp_source_particletype_fromphs_particlename_wip.py` & `opengate-10.0b8/opengate/tests/src/test060_phsp_source_particletype_fromphs_particlename_wip.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test060_phsp_source_particletype_fromphs_pdgcode.py` & `opengate-10.0b8/opengate/tests/src/test060_phsp_source_particletype_fromphs_pdgcode.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test060_phsp_source_rotation.py` & `opengate-10.0b8/opengate/tests/src/test060_phsp_source_rotation.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test060_phsp_source_translation.py` & `opengate-10.0b8/opengate/tests/src/test060_phsp_source_translation.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test060_phsp_source_untilNextPrimary.py` & `opengate-10.0b8/opengate/tests/src/test060_phsp_source_untilNextPrimary.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test061_TPPhsSource.py` & `opengate-10.0b8/opengate/tests/src/test061_TPPhsSource.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test061_TPPhsSource_helpers.py` & `opengate-10.0b8/opengate/tests/src/test061_TPPhsSource_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 import opengate as gate
 
-# import numpy as np
-# import matplotlib.pyplot as plot
 from scipy.spatial.transform import Rotation
 import gatetools.phsp as phsp
 import os
 from opengate.tests import utility
 from opengate.contrib.tps.treatmentPlanPhsSource import TreatmentPlanPhsSource
 from opengate.contrib.tps.ionbeamtherapy import spots_info_from_txt, TreatmentPlanSource
-
-
-# paths = gate.get_default_test_paths(
-#     __file__, "gate_test019_linac_phsp", output_folder="test019"
-# )
-# paths = {output: "output"}
+from pathlib import Path
 
 # units
 m = gate.g4_units.m
 mm = gate.g4_units.mm
 cm = gate.g4_units.cm
 nm = gate.g4_units.nm
 Bq = gate.g4_units.Bq
 MeV = gate.g4_units.MeV
 deg: float = gate.g4_units.deg
 
 
 def create_test_Phs(
     particle="proton",
-    phs_name="output/test_proton.root",
+    phs_name=Path("output") / "test_proton.root",
     number_of_particles=1,
     translation=[0 * mm, 0 * mm, 0 * mm],
 ):
     # create the simulation
     sim = gate.Simulation()
 
     # main options
@@ -112,15 +105,15 @@
     source.n = number_of_particles
 
     sim.run()
     output = sim.output
 
 
 def create_PhS_withoutSource(
-    phs_name="output/test_proton.root",
+    phs_name=Path("output") / "test_proton.root",
 ):
     # create the simulation
     sim = gate.Simulation()
 
     # main options
     ui = sim.user_info
     ui.g4_verbose = False
@@ -193,32 +186,33 @@
     # output = sim.run()
     # output = sim.start()
     # output = sim.start(start_new_process=True)
     return sim, plane
 
 
 def test_source_rotation_A(
-    plan_file_name="output/test_proton_offset.root",
+    plan_file_name=Path("output") / "test_proton_offset.root",
     phs_list_file_name="PhsList.txt",
     phs_folder_name="",
-    phs_file_name_out="output/output/test_source_electron.root",
+    phs_file_name_out=Path("output") / "output/test_source_electron.root",
 ) -> None:
     sim, plane = create_PhS_withoutSource(
         phs_name=phs_file_name_out,
     )
     number_of_particles = 1
     ##########################################################################################
     #  Source
     ##########################################################################################
     # TreatmentPlanPhsSource source
     tpPhSs = TreatmentPlanPhsSource("RT_plan", sim)
     tpPhSs.set_phaseSpaceList_file_name(phs_list_file_name)
     tpPhSs.set_phaseSpaceFolder(phs_folder_name)
-    spots, ntot, energies, G = spots_info_from_txt(plan_file_name, "")
-    # print(spots, ntot, energies, G)
+    beam_dict = spots_info_from_txt(plan_file_name, "", 1)
+    G = beam_dict["gantry_angle"]
+    spots = beam_dict["spots"]
     tpPhSs.set_spots(spots)
     tpPhSs.set_particles_to_simulate(number_of_particles)
     tpPhSs.set_distance_source_to_isocenter(100 * cm)
     tpPhSs.set_distance_stearmag_to_isocenter(5 * m, 5 * m)
     tpPhSs.rotation = Rotation.from_euler("z", G, degrees=True)
     tpPhSs.initialize_tpPhssource()
 
@@ -226,28 +220,28 @@
     plane.rotation = Rotation.from_euler("y", 90, degrees=True).as_matrix()
 
     sim.run()
     output = sim.output
 
 
 def get_first_entry_of_key(
-    file_name_root="output/test_source_electron.root", key="ParticleName"
+    file_name_root=Path("output") / "test_source_electron.root", key="ParticleName"
 ) -> None:
     # read root file
     data_ref, keys_ref, m_ref = phsp.load(file_name_root)
     # print(data_ref)
     # print(keys_ref)
     index = keys_ref.index(key)
     # print(index)
     # print(data_ref[index][0])
     return data_ref[0][index]
 
 
 def check_value_from_root_file(
-    file_name_root="output/test_source_electron.root",
+    file_name_root=Path("output") / "test_source_electron.root",
     key="ParticleName",
     ref_value="e-",
 ):
     # read root file
     value = get_first_entry_of_key(file_name_root=file_name_root, key=key)
     if (type(ref_value) != str) and (type(value) != str):
         is_ok = utility.check_diff_abs(
```

### Comparing `opengate-10.0b7/opengate/tests/src/test061_user_event_info_helpers.py` & `opengate-10.0b8/opengate/tests/src/test061_user_event_info_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         "ParentID",
         "GlobalTime",
         "ParticleName",
         "ParentParticleName",
         "TrackCreatorProcess",
         "ProcessDefinedStep",
     ]
-    phsp.debug = False
+    # phsp.debug = True
     phsp.output = paths.output / f"test061_{name}.root"
 
 
 def analyse(output):
     # end
     stats = output.get_actor("stats")
     print(stats)
@@ -82,30 +82,34 @@
     parent_particle_array = events["ParentParticleName"]
     particle_array = events["ParticleName"]
     event_id_array = events["EventID"]
     track_id_array = events["TrackID"]
     parent_id_array = events["ParentID"]
     parent_particle_array_ref = ["unknown"] * len(kinetic_energy_array)
 
-    # we test if the stored ParentParticleName is exactly the same as the one we can retrieve from
+    # we test if the stored ParentParticleName is the same as the one we can retrieve from
     # the TrackID and ParentID
 
     def set_parent_name(parent_by_track, starting_index):
         # print('set parent name', starting_index, len(parent_by_track))
         lindex = starting_index
         lis_ok = True
         while lindex < starting_index + len(parent_by_track):
             pid = parent_id_array[lindex]
             if pid in parent_by_track:
                 parent_particle_array_ref[lindex] = parent_by_track[pid]
             else:
-                # the events are not store in the phsp because they do not do a single step,
-                # for the test we force to Ac225
+                # the events are not stored in the phsp because they do not do a single step,
+                # for the test we force to Ac225 ? NO ! was ok in G4 11.1, but no more valid in G4 11.2
+                # now we check if this is an ion with [] inside the name
                 parent_particle_array_ref[lindex] = "Ac225"
-            ok = parent_particle_array_ref[lindex] == parent_particle_array[lindex]
+            ok = (
+                parent_particle_array_ref[lindex] == parent_particle_array[lindex]
+                or "[" in parent_particle_array[lindex]
+            )
             if not ok or lindex % 100 == 0:
                 utility.print_test(
                     ok,
                     f"Parent particle i={lindex} track={track_id_array[lindex]} name={particle_array[lindex]}  ptrack={pid} "
                     f"       ref = {parent_particle_array_ref[lindex]} "
                     f"vs = {parent_particle_array[lindex]}",
                 )
```

### Comparing `opengate-10.0b7/opengate/tests/src/test061_user_event_info_mt.py` & `opengate-10.0b8/opengate/tests/src/test061_user_event_info_mt.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test062_apply_g4_cmds.py` & `opengate-10.0b8/opengate/tests/src/test062_apply_g4_cmds.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test063_em_switches.py` & `opengate-10.0b8/opengate/tests/src/test063_em_switches.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test064_kill_actor_mt.py` & `opengate-10.0b8/opengate/tests/src/test064_kill_actor_mt.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # main options
     sim.g4_verbose = False
     # sim.visu = True
     sim.visu_type = "vrml"
     sim.check_volumes_overlap = False
     # sim.running_verbose_level = gate.EVENT
     sim.number_of_threads = 2
-    sim.random_seed = "auto"
+    sim.random_seed = 987654321
 
     # units
     m = gate.g4_units.m
     km = gate.g4_units.km
     mm = gate.g4_units.mm
     cm = gate.g4_units.cm
     nm = gate.g4_units.nm
```

### Comparing `opengate-10.0b7/opengate/tests/src/test065_sim_as_dict.py` & `opengate-10.0b8/opengate/tests/src/test065_sim_as_dict.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test065_sim_from_dict.py` & `opengate-10.0b8/opengate/tests/src/test065_sim_from_dict.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
 from opengate.tests import utility
 import pathlib
+import os
+import subprocess
 
 # This test is to be run after test065_sim_as_dict.py
 # It checks whether the simulation is recreated correctly from the JSON file,
 # but does not actually run any simulation.
 
 if __name__ == "__main__":
     pathFile = pathlib.Path(__file__).parent.resolve()
     paths = utility.get_default_test_paths(__file__)
 
+    # the test065_sim_as_dict.py is needed first
+    if not os.path.isfile(paths.output / "simu_test065.json"):
+        print(f"Running test065_sim_as_dict.py")
+        subprocess.call(["python", paths.current / "test065_sim_as_dict.py"])
+
     # create the simulation
     sim = gate.Simulation()
     sim.from_json_file(paths.output / "test065" / "simu_test065.json")
 
     # Assert that objects have been read back correctly
     assert "rod" in sim.volume_manager.volumes
     m = gate.g4_units.m
```

### Comparing `opengate-10.0b7/opengate/tests/src/test066_phspsource_activity.py` & `opengate-10.0b8/opengate/tests/src/test066_phspsource_activity.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_0_orientation.py` & `opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_0_orientation.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,15 @@
 
     # options
     colli_type = "lehr"
     radius = 400 * mm
     gantry_angle = -20
 
     # main elements : spect + phantom
-    head, crystal = genm670.add_ge_nm67_spect_head(
-        sim, collimator_type=colli_type, debug=True
-    )
+    head, crystal = genm670.add_spect_head(sim, collimator_type=colli_type, debug=True)
 
     # rotation by default
     genm670.set_head_orientation(head, colli_type, radius, gantry_angle)
     print(f"Head translation = {head.translation[0]=:.2f}")
 
     # add arf plane (put in parallel world to avoid overlap)
     sim.add_parallel_world("arf_world")
```

### Comparing `opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_1_reference.py` & `opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_1_reference.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_2.py` & `opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_3_standalone.py` & `opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_3_standalone.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from opengate.tests import utility
 import gaga_phsp as gaga
 import itk
 from box import Box
 from scipy.spatial.transform import Rotation
 import opengate as gate
-from opengate.contrib.spect import genm670
+from opengate.contrib.spect import ge_discovery_nm670
 import time
 
 if __name__ == "__main__":
     paths = utility.get_default_test_paths(__file__, None, "test066")
     output_path = paths.output
 
     # create the simulation
```

### Comparing `opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_4_analyse1.py` & `opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_4_analyse1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_5_analyse2.py` & `opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_5_analyse2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/tests/src/test066_spect_gaga_garf_helpers.py` & `opengate-10.0b8/opengate/tests/src/test066_spect_gaga_garf_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
 import opengate.contrib.phantoms.nemaiec as gate_iec
 import opengate.sources.gansources as gansources
 from opengate.sources.generic import get_rad_gamma_energy_spectrum
-from opengate.contrib.spect import genm670
+from opengate.contrib.spect import ge_discovery_nm670
 from scipy.spatial.transform import Rotation
 
 
 def create_world(sim):
     # world size
     m = gate.g4_units.m
     sim.world.size = [2 * m, 2 * m, 2 * m]
     sim.world.material = "G4_AIR"
 
 
 def set_phys(sim):
     m = gate.g4_units.m
-    p = sim.get_physics_user_info()
-    p.physics_list_name = "G4EmStandardPhysics_option3"
+    sim.physics_manager.physics_list = "G4EmStandardPhysics_option3"
     sim.physics_manager.set_production_cut("world", "all", 1e3 * m)
 
 
 def create_simu_with_genm670(sim, collimator_type="lehr", debug=False):
     # units
     mm = gate.g4_units.mm
 
     # world size
     create_world(sim)
 
     # spect system
-    head1, crystal1 = genm670.add_ge_nm67_spect_head(
+    head1, crystal1 = genm670.add_spect_head(
         sim, "spect1", collimator_type=collimator_type, debug=debug
     )
-    head2, crystal2 = genm670.add_ge_nm67_spect_head(
+    head2, crystal2 = genm670.add_spect_head(
         sim, "spect2", collimator_type=collimator_type, debug=debug
     )
 
     # default rotation to be in front of the IEC
     radius = 280 * mm
     genm670.set_head_orientation(head1, collimator_type, radius, 0)
     genm670.set_head_orientation(head2, collimator_type, radius, 180)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test067_cbct_fluence_actor_mt.py` & `opengate-10.0b8/opengate/tests/src/test067_cbct_fluence_actor_mt.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 from opengate.tests import utility
 
 if __name__ == "__main__":
     paths = utility.get_default_test_paths(__file__, "gate_test067", "test067")
 
     sim = gate.Simulation()
 
-    ui = sim.user_info
-    # ui.visu = True
-    ui.visu_type = "vrml"
-    ui.random_engine = "MersenneTwister"
-    ui.random_seed = "auto"
-    ui.number_of_threads = 2
+    # sim.visu = True
+    sim.visu_type = "vrml"
+    sim.random_engine = "MersenneTwister"
+    sim.random_seed = 321654
+    sim.number_of_threads = 2
 
     # units
     m = gate.g4_units.m
     cm = gate.g4_units.cm
     nm = gate.g4_units.nm
     cm3 = gate.g4_units.cm3
     keV = gate.g4_units.keV
@@ -69,35 +68,36 @@
     source.particle = "gamma"
     source.energy.mono = 60 * keV
     source.position.type = "box"
     source.position.size = [1 * nm, 2 * 8 * mm, 2 * 8 * mm]
     source.direction.type = "focused"
     # FIXME warning in world coord ! Should be in mother coord system
     source.direction.focus_point = [gantry.translation[0] - 60 * mm, 0, 0]
-    source.n = 50000 / ui.number_of_threads
+    source.n = 50000 / sim.number_of_threads
 
-    if ui.visu:
+    if sim.visu:
         source.n = 100
 
     # statistics
     stats = sim.add_actor("SimulationStatisticsActor", "stats")
     stats.track_types_flag = True
     stats.output = paths.output / "stats.txt"
 
     # run
     sim.run()
     output = sim.output
 
     # print output statistics
     stats = output.get_actor("stats")
     print(stats)
+    out_path = sim.output.get_actor("detector_actor").user_info.output
 
     # check images
     is_ok = utility.assert_images(
         paths.gate_output / "detector.mhd",
-        paths.output / "fluence.mhd",
+        out_path,
         stats,
         tolerance=44,
         axis="y",
     )
 
     utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/src/test068_rotation_source.py` & `opengate-10.0b8/opengate/tests/src/test068_rotation_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import opengate as gate
 from opengate.tests import utility
 from scipy.spatial.transform import Rotation
 import numpy as np
 import uproot
 
 
-# The test generates two differents generic sources, momentum and focused, which is attached to a plan.
+# The test generates two different generic sources, momentum and focused, which is attached to a plan.
 # The plan is randomly rotated and we verify that the generated particles have a direction which is in accordance
 # with the applied rotations and the transmissions.
 
 
 def test068(tab, nb_run, nb_part, nb_source):
     nb_event = len(tab)
     nb_event_theo = nb_run * nb_part * nb_source
@@ -27,22 +27,21 @@
     paths = utility.get_default_test_paths(__file__)
     output_path = paths.output
 
     # create the simulation
     sim = gate.Simulation()
 
     # main options
-    ui = sim.user_info
-    ui.g4_verbose = False
-    # ui.visu = True
-    ui.visu_type = "vrml"
-    ui.check_volumes_overlap = False
-    # ui.running_verbose_level = gate.logger.EVENT
-    ui.number_of_threads = 1
-    ui.random_seed = "auto"
+    sim.g4_verbose = False
+    # sim.visu = True
+    sim.visu_type = "vrml"
+    sim.check_volumes_overlap = False
+    # sim.running_verbose_level = gate.logger.EVENT
+    sim.number_of_threads = 1
+    sim.random_seed = 123654987
 
     # units
     m = gate.g4_units.m
     km = gate.g4_units.km
     mm = gate.g4_units.mm
     cm = gate.g4_units.cm
     nm = gate.g4_units.nm
@@ -75,28 +74,28 @@
     source1.position.size = [10 * cm, 10 * cm, 1 * nm]
     source1.direction.type = "momentum"
     source1.force_rotation = True
     # source1.direction.focus_point = [0*cm, 0*cm, -5 *cm]
     source1.direction.momentum = [0, 0, -1]
     source1.energy.type = "mono"
     source1.energy.mono = 1 * MeV
-    source1.activity = n * Bq / ui.number_of_threads
+    source1.activity = n * Bq / sim.number_of_threads
 
     source2 = sim.add_source("GenericSource", "photon_source_2")
     source2.particle = "gamma"
     source2.position.type = "box"
     source2.mother = plan.name
     source2.position.size = [10 * cm, 10 * cm, 1 * nm]
     source2.direction.type = "focused"
     source2.force_rotation = True
     source2.direction.focus_point = [0 * cm, 0 * cm, -5 * cm]
     # source1.direction.momentum = [0, 0, -1]
     source2.energy.type = "mono"
     source2.energy.mono = 1 * MeV
-    source2.activity = n * Bq / ui.number_of_threads
+    source2.activity = n * Bq / sim.number_of_threads
 
     # Phase Space
 
     phsp_plan = sim.add_volume("Box", "phsp_plan")
     phsp_plan.mother = world.name
     phsp_plan.material = "G4_Galactic"
     phsp_plan.size = [10 * cm, 10 * cm, 1 * nm]
```

### Comparing `opengate-10.0b7/opengate/tests/src/test069_rotation_DICOM_RT_plan.py` & `opengate-10.0b8/opengate/tests/src/test019_linac_elekta_versa_with_mlc_rt_plan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,85 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
 import opengate as gate
+import opengate.contrib.linacs.elektaversa as versa
+import opengate.contrib.linacs.dicomrtplan as rtplan
+from opengate.tests import utility
+from opengate.utility import g4_units
+from scipy.spatial.transform import Rotation
 import numpy as np
 import itk
-import test069_rotation_DICOM_RT_plan_helpers as t
-from opengate.tests import utility
-
-
-def validation_test(theoretical_calculation, MC_calculation, tol=0.08):
-    print(
-        "Area from theoretical calculation for all CP (mm2): ", theoretical_calculation
-    )
-    print("Area from MC simulations for all CP: (mm2)", MC_calculation)
-    percentage_diff = (
-        100 * (theoretical_calculation - MC_calculation) / theoretical_calculation
-    )
-    bool_percentage_diff = np.abs(percentage_diff) > tol * 100
-    if np.sum(bool_percentage_diff) == 0:
-        return True
-    else:
-        return False
 
 
-def calc_MLC_aperture(
-    x_leaf_position, y_jaws, pos_MLC=349.3, pos_jaws=470.5, SAD=1000, leaf_width=1.85
+def calc_mlc_aperture(
+    x_leaf_position, y_jaws, pos_mlc=349.3, pos_jaws=470.5, sad=1000, leaf_width=1.85
 ):
     mm = gate.g4_units.mm
     leaf_width = leaf_width * mm
-    left = x_leaf_position[:80] * pos_MLC / SAD
-    right = x_leaf_position[80:] * pos_MLC / SAD
+    left = x_leaf_position[:80] * pos_mlc / sad
+    right = x_leaf_position[80:] * pos_mlc / sad
     left[left != 0] = left[left != 0] - left[left != 0] % 0.5
     right[right != 0] = right[right != 0] + 0.5 - right[right != 0] % 0.5
 
-    pos_Y_leaf = np.arange(
+    pos_y_leaf = np.arange(
         -leaf_width * 40 + leaf_width / 2,
         leaf_width * 40 - leaf_width / 2 + 0.01,
         leaf_width,
     )
-    left[pos_Y_leaf < y_jaws[0] * pos_jaws / SAD] = 0
-    left[pos_Y_leaf > y_jaws[1] * pos_jaws / SAD] = 0
-    right[pos_Y_leaf < y_jaws[0] * pos_jaws / SAD] = 0
-    right[pos_Y_leaf > y_jaws[1] * pos_jaws / SAD] = 0
+    left[pos_y_leaf < y_jaws[0] * pos_jaws / sad] = 0
+    left[pos_y_leaf > y_jaws[1] * pos_jaws / sad] = 0
+    right[pos_y_leaf < y_jaws[0] * pos_jaws / sad] = 0
+    right[pos_y_leaf > y_jaws[1] * pos_jaws / sad] = 0
     diff = np.array(right - left)
 
     return np.sum(diff) * leaf_width
 
 
-def add_VolumeToIrradiate(sim, name, rot_volume):
-    mm = gate.g4_units.mm
-    Box = sim.add_volume("Box", "cylinder")
-    Box.material = "G4_WATER"
-    Box.mother = name
-    Box.size = [400 * mm, 400 * mm, 400 * mm]
+def add_volume_to_irradiate(sim, name):
+    mm = g4_units.mm
+    m = g4_units.m
+    plane = sim.add_volume("Box", "water_plane")
+    plane.mother = name
+    plane.material = "G4_WATER"
+    plane.size = [0.4 * m, 0.4 * m, 2 * cm]
+    plane.translation = [0 * mm, 0 * mm, 0 * mm]
+    plane.color = [1, 0, 0, 1]  # red
 
     voxel_size_x = 0.5 * mm
     voxel_size_y = 0.5 * mm
-    voxel_size_z = 400 * mm
+    voxel_size_z = 2 * cm
 
     dim_box = [
-        400 * mm / voxel_size_x,
-        400 * mm / voxel_size_y,
-        400 * mm / voxel_size_z,
+        plane.size[0] / voxel_size_x,
+        plane.size[1] / voxel_size_y,
+        1,
     ]
-    dose = sim.add_actor("DoseActor", "dose")
-    dose.output = "output/testilol.mhd"
-    dose.mother = Box.name
+    dose = sim.add_actor("DoseActor", "dose_water_slice")
+    dose.mother = plane.name
+    dose.output = paths.output / "dose_actor_versa_rt_plan.mhd"
     dose.size = [int(dim_box[0]), int(dim_box[1]), int(dim_box[2])]
     dose.spacing = [voxel_size_x, voxel_size_y, voxel_size_z]
     dose.uncertainty = False
     dose.square = False
     dose.hit_type = "random"
 
-    motion_tubs = sim.add_actor("MotionVolumeActor", "Move_Tubs")
-    motion_tubs.mother = Box.name
-    motion_tubs.rotations = []
-    motion_tubs.translations = []
-    for i in range(len(rot_volume)):
-        motion_tubs.rotations.append(rot_volume[i])
-        motion_tubs.translations.append([0, 0, 0])
+    motion_phsp = sim.add_actor("MotionVolumeActor", "Move_phsp")
+    motion_phsp.mother = plane.name
+    motion_phsp.rotations = []
+    motion_phsp.translations = []
+    rotation_angle = rt_plan_parameters["gantry angle"]
+    for n in l_cp:
+        rot = Rotation.from_euler("y", rotation_angle[n], degrees=True)
+        rot = rot.as_matrix()
+        motion_phsp.rotations.append(rot)
+        motion_phsp.translations.append(np.zeros(3))
 
 
 def add_alpha_source(sim, name, pos_Z, nb_part):
-    ui = sim.user_info
     mm = gate.g4_units.mm
     nm = gate.g4_units.nm
     plan_source = sim.add_volume("Box", "plan_alpha_source")
     plan_source.material = "G4_Galactic"
     plan_source.mother = name
     plan_size = np.array([250 * mm, 148 * mm, 1 * nm])
     plan_source.size = np.copy(plan_size)
@@ -97,106 +93,152 @@
     source.energy.type = "mono"
     source.energy.mono = 1 * MeV
     source.position.type = "box"
     source.position.size = np.copy(plan_size)
     source.direction.type = "momentum"
     source.force_rotation = True
     source.direction.momentum = [0, 0, -1]
-    source.activity = nb_part * Bq / ui.number_of_threads
+    source.activity = nb_part * Bq / sim.number_of_threads
 
 
-def launch_simulation(
-    nt, path_img, img, file, output_path, output, nb_part, src_f, vis, seg_cp, patient
+def validation_test_19_rt_plan(
+    theoretical_calculation,
+    MC_calculation,
+    cp_id,
+    rt_plan_parameters,
+    nb_part_init,
+    nb_part_sent,
+    tol=0.1,
 ):
-    visu = vis
-    km = gate.g4_units.km
-    nb_cp = t.liste_CP(file)
-    nb_aleatoire = np.random.randint(0, nb_cp - 1, 4)
-    print("Control Points ID: ", nb_aleatoire)
-    seg_cp += 1
-    l_aperture_voxel = np.zeros(len(nb_aleatoire))
-    l_aperture_calc = np.zeros(len(nb_aleatoire))
-    for i in range(len(nb_aleatoire)):
-        cp_param = t.Dataset_DICOM_MLC_jaws(
-            file, [nb_aleatoire[i], nb_aleatoire[i] + 1], 0
-        )
-        mean_leaves = (cp_param["Leaves"][0] + cp_param["Leaves"][1]) / 2
-        mean_jaws_1 = (cp_param["Y_jaws_1"][0] + cp_param["Y_jaws_1"][1]) / 2
-        mean_jaws_2 = (cp_param["Y_jaws_2"][0] + cp_param["Y_jaws_2"][1]) / 2
-        y_jaws = [mean_jaws_1, mean_jaws_2]
-        area = calc_MLC_aperture(mean_leaves, y_jaws)
-        l_aperture_calc[i] = area
-        sim = t.init_simulation(
-            nt,
-            cp_param,
-            path_img,
-            img,
-            visu,
-            src_f,
-            bool_phsp=False,
-            seg_cp=seg_cp,
-            patient=patient,
-        )
-
-        ui = sim.user_info
-        ui.running_verbose_level = gate.logger.RUN
-
-        linac = sim.volume_manager.volumes["Linac_box"]
-        world = sim.volume_manager.volumes["world"]
-        linac.material = "G4_Galactic"
-        world.material = "G4_Galactic"
-        motion_actor = sim.get_actor_user_info("Move_LINAC")
-        rotation_volume = motion_actor.rotations
-        add_alpha_source(sim, linac.name, linac.size[2], nb_part)
-        add_VolumeToIrradiate(sim, world.name, rotation_volume)
-
-        dose_actor = sim.get_actor_user_info("dose")
-        dose_actor.output = output_path / output
-
-        ui.visu = visu
-        if visu:
-            ui.visu_type = "vrml"
-        sim.physics_manager.global_production_cuts.gamma = 1 * km
-        sim.physics_manager.global_production_cuts.electron = 1 * km
-        sim.physics_manager.global_production_cuts.positron = 1 * km
-        sec = gate.g4_units.s
-        sim.run_timing_intervals = []
-        for j in range(len(rotation_volume)):
-            sim.run_timing_intervals.append([j * sec, (j + 1) * sec])
-
-        sim.run(start_new_process=True)
-        img_MC = itk.imread(output_path / output)
-        array_MC = itk.GetArrayFromImage(img_MC)
-        bool_MC = array_MC[array_MC != 0]
-        l_aperture_voxel[i] = len(bool_MC) / 4
-    is_ok = validation_test(l_aperture_calc, l_aperture_voxel)
-    utility.test_ok(is_ok)
+    print(
+        "Area from theoretical calculations for the chosen CP:",
+        theoretical_calculation,
+        "mm2",
+    )
+    print("Area from MC simulations for the chosen CP:", MC_calculation, "mm2")
+
+    print("Number of particles emitted:", nb_part_sent)
+    percentage_diff = (
+        100 * (theoretical_calculation - MC_calculation) / theoretical_calculation
+    )
+    bool_percentage_diff = np.abs(percentage_diff) > tol * 100
+    monitor_units = rt_plan_parameters["weight"][cp_id]
+    nb_part_theo = nb_part_init * monitor_units
+    print("Number of particles theoretically emitted:", int(np.round(nb_part_theo)))
+    err_nb_part = np.sqrt(nb_part_theo)
+    if (
+        (nb_part_sent >= nb_part_theo - 4 * err_nb_part)
+        and (nb_part_sent <= nb_part_theo + 4 * err_nb_part)
+        and np.sum(bool_percentage_diff) == 0
+    ):
+        return True
+    else:
+        return False
 
 
 if __name__ == "__main__":
-    paths = utility.get_default_test_paths(__file__)
-    output_path = paths.output
-    patient = False
-    nt = 1
-    ###### The three following variables are here to not modify the main program (the helpers) which need it ######
-    path_img = "useless"
-    img = "useless"
-    src_f = "alpha"
-    ###############################################################################################################
-    output = "img_test_069.mhd"
+    # paths
+    paths = utility.get_default_test_paths(__file__, output_folder="test019_linac")
+
+    # create the simulation
+    sim = gate.Simulation()
+
+    # main options
+    sim.g4_verbose = False
+    # sim.visu = True
+    sim.visu_type = "vrml"
+    sim.check_volumes_overlap = False
+    sim.number_of_threads = 1
+    sim.output_dir = paths.output  # FIXME (not yet)
+    sim.random_seed = 123456789
+    sim.check_volumes_overlap = True
+
+    # unit
+    nm = gate.g4_units.nm
+    m = gate.g4_units.m
+    mm = gate.g4_units.mm
+    cm = gate.g4_units.cm
+    MeV = gate.g4_units.MeV
+    sec = gate.g4_units.s
+    Bq = gate.g4_units.Bq
+
+    # world
+    world = sim.world
+    world.size = [3 * m, 3 * m, 3 * m]
+    world.material = "G4_Galactic"
+    a = np.array([0])
+
+    # linac
+    versa.add_linac_materials(sim)
+    sad = 1000 * mm
+    linac = versa.add_empty_linac_box(sim, "linac_box", sad)
+    linac.material = "G4_Galactic"
+
+    # jaws
+    if sim.visu:
+        jaws = versa.add_jaws_visu(sim, linac.name)
+    else:
+        jaws = versa.add_jaws(sim, linac.name)
+
+    # mlc
+    mlc = versa.add_mlc(sim, linac.name)
+
+    # add alpha source :
     nb_part = 750000
-    seg_cp = 1
-    vis = False
-    file = str(paths.data / "DICOM_RT_plan.dcm")
-    launch_simulation(
-        nt,
-        path_img,
-        img,
-        file,
-        output_path,
-        output,
+    z_linac = linac.size[2]
+    rt_plan_parameters = rtplan.read(str(paths.data / "DICOM_RT_plan.dcm"))
+    l_cp = [np.random.randint(0, len(rt_plan_parameters["jaws 1"]), 1)[0]]
+    versa.set_linac_head_motion(
+        sim, linac.name, jaws, mlc, rt_plan_parameters, sad=sad, cp_id=l_cp
+    )
+    MU = rt_plan_parameters["weight"][l_cp[0]]
+    nb_part = nb_part / MU
+
+    if sim.visu:
+        add_alpha_source(sim, linac.name, z_linac / 2 - 5.6 * mm, 10)
+    else:
+        add_alpha_source(sim, linac.name, z_linac / 2 - 5.6 * mm, nb_part)
+
+    # Linac head rotation and jaws and mlc translation according to a DICOM rt plan
+
+    # physics
+    sim.physics_manager.physics_list_name = "G4EmStandardPhysics_option3"
+    sim.physics_manager.set_production_cut("world", "all", 1000 * m)
+
+    # add stat actor
+    s = sim.add_actor("SimulationStatisticsActor", "stats")
+    s.track_types_flag = True
+
+    # add water slice with a dose actor and a motion actor
+    add_volume_to_irradiate(sim, world.name)
+
+    # start simulation
+    # The number of particles provided (sim.activity) will be adapted
+    # according to the number of MU delivered at each control points.
+    versa.set_time_intervals_from_rtplan(sim, rt_plan_parameters, cp_id=l_cp)
+    sim.run()
+
+    # print results
+    stats = sim.output.get_actor(s.name)
+    print(stats)
+
+    # test
+    leaves = rt_plan_parameters["leaves"][l_cp[0]]
+    jaws_1 = rt_plan_parameters["jaws 1"][l_cp[0]]
+    jaws_2 = rt_plan_parameters["jaws 2"][l_cp[0]]
+    jaws = [jaws_1, jaws_2]
+    theoretical_area = calc_mlc_aperture(leaves, jaws, sad=sad)
+
+    dose2 = sim.output.get_actor("dose_water_slice")
+    img_MC = itk.imread(paths.output / dose2.user_info.output)
+    array_MC = itk.GetArrayFromImage(img_MC)
+    bool_MC = array_MC[array_MC != 0]
+    simulated_area = len(bool_MC) / 4
+    is_ok = validation_test_19_rt_plan(
+        theoretical_area,
+        simulated_area,
+        l_cp[0],
+        rt_plan_parameters,
         nb_part,
-        src_f,
-        vis,
-        seg_cp,
-        patient,
+        stats.counts.event_count,
     )
+    utility.test_ok(is_ok)
```

### Comparing `opengate-10.0b7/opengate/tests/utility.py` & `opengate-10.0b8/opengate/tests/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 import string
 import colored
 from box import Box, BoxList
 import scipy
 import pathlib
 import uproot
 import sys
+from pathlib import Path
 import matplotlib.pyplot as plt
 from matplotlib.ticker import StrMethodFormatter
 import gatetools.phsp as phsp
 from matplotlib.patches import Circle
 
-from ..utility import g4_units, ensure_filename_is_str
+from ..utility import g4_units, ensure_filename_is_str, insert_suffix_before_extension
 from ..exception import fatal, color_error, color_ok
-from ..image import get_info_from_image, itk_image_view_from_array
+from ..image import get_info_from_image, itk_image_view_from_array, write_itk_image
 from ..userinfo import UserInfo
 from ..actors.miscactors import SimulationStatisticsActor
 
 
 def test_ok(is_ok=False):
     if is_ok:
         s = "Great, tests are ok."
@@ -71,14 +72,15 @@
                 stat.nb_thread = int(a)
             except:
                 stat.nb_thread = "?"
     return stat
 
 
 def print_test(b, s):
+    s += f" --> OK? {b}"
     if b:
         print(s)
     else:
         color = color_error
         print(colored.stylize(s, color))
     return b
 
@@ -109,15 +111,15 @@
     if stat2.sps != 0:
         sps_d = stat1.sps / stat2.sps * 100 - 100
     else:
         sps_d = 100
 
     b = stat1.counts.run_count == stat2.counts.run_count
     is_ok = b and is_ok
-    print_test(b, f"Runs:         {stat1.counts.run_count} {stat2.counts.run_count} ")
+    print_test(b, f"Runs:         {stat1.counts.run_count} {stat2.counts.run_count}")
 
     b = abs(event_d) <= tolerance * 100
     is_ok = b and is_ok
     st = f"(tol = {tolerance * 100:.2f} %)"
     print_test(
         b,
         f"Events:       {stat1.counts.event_count} {stat2.counts.event_count} : {event_d:+.2f} %  {st}",
@@ -337,15 +339,15 @@
     )
     ax.set_ylabel("Counts")
     ax.legend()
 
 
 def plot_profile(ax, y, y_spacing=1, label=""):
     x = np.arange(len(y)) * y_spacing
-    ax.plot(x, y, label=label)
+    ax.plot(x, y, label=label, drawstyle="steps")
     ax.legend()
 
 
 def assert_filtered_imagesprofile1D(
     ref_filter_filename1,
     ref_filename1,
     filename2,
@@ -379,58 +381,60 @@
         data1 = np.flip(data1)
         data2 = np.flip(data2)
     max_ind = np.argmax(filter_data)
     L_filter = range(max_ind)
     d1 = data1[L_filter]
     d2 = data2[L_filter]
 
-    s1 = np.sum(d1)
-    s2 = np.sum(d2)
-    print(
-        f"Evaluate only data from entry up to peak position of reference filter image"
-    )
-    print(f"Going to evaluate {d1.size} elements out of {data1.size}")
-    t = np.fabs((s1 - s2) / s1) * 100
-    b = t < sum_tolerance
-    print_test(b, f"Img sums {s1} vs {s2} : {t:.2f} %  (tol {sum_tolerance:.2f} %)")
-
-    # do not consider pixels with a value of zero (data2 is the reference)
-    # d1 = data1[data2 != ignore_value]
-    # d2 = data2[data2 != ignore_value]
-
     # normalise by event
     if stats is not None:
         d1 = d1 / stats.counts.event_count
         d2 = d2 / stats.counts.event_count
 
-    # normalize by sum of d1
-    s = np.sum(d2)
-    d1 = d1 / s
-    d2 = d2 / s
+    mean_deviation = np.mean(d2 / d1 - 1) * 100
+    max_deviation = np.amax(np.abs(d1 / d2 - 1)) * 100
+    is_ok = is_ok and mean_deviation < tolerance and max_deviation < 2 * tolerance
 
-    # sum of absolute difference (in %)
-    sad = np.fabs(d1 - d2).sum() * 100
-    is_ok = is_ok and sad < tolerance
     print_test(
         is_ok,
-        f"Image diff computed on {len(data2 != 0)}/{len(data2.ravel())} \n"
-        f"SAD (per event/total): {sad:.2f} % "
-        f" (tolerance is {tolerance :.2f} %)",
+        f"Evaluate only data from entry up to peak position of reference filter image\n"
+        f"Evaluated {d1.size} elements out of {data1.size} \n"
+        f"Mean deviation: {mean_deviation:.2f} % | (tolerance is {tolerance :.2f} %) \n"
+        f"Max unsigned deviation: {max_deviation:.2f} % | (tolerance is {2*tolerance :.2f} % \n\n"
+        f" ",
     )
-    filter_data_norm_au = filter_data / np.amax(filter_data) * np.amax(data1) * 0.7
-    # plot
-    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(25, 10))
-
-    plot_profile(ax, filter_data_norm_au, info1.spacing[0], "filter")
-    plot_profile(ax, data1, info1.spacing[0], "reference")
-    plot_profile(ax, data2, info2.spacing[0], "test")
-    ax.plot(max_ind * info1.spacing[0], filter_data_norm_au[max_ind], "o", label="p")
 
+    filter_data_norm_au = filter_data / np.amax(filter_data) * np.amax(d2) * 0.7
+    # plot
+    fig, ax = plt.subplots(ncols=1, nrows=2, figsize=(15, 15))
+    xV = np.arange(len(data1)) * info1.spacing[0]
+    x_max = np.ceil(xV[max_ind] * 1.05 + 2)
+    plot_profile(ax[0], filter_data_norm_au, info1.spacing[0], "filter")
+    plot_profile(ax[0], data1, info1.spacing[0], "reference")
+    plot_profile(ax[0], data2, info2.spacing[0], "test")
+    ax[0].plot(xV[max_ind], filter_data_norm_au[max_ind], "o", label="p")
+    ax[1].plot(xV[:max_ind], (d2 / d1 - 1) * 100, "o", label="test/ref")
+    ax[0].set_xlabel("x [mm]")
+    ax[1].set_xlabel("x [mm]")
+    ax[0].set_ylabel("LET")
+    ax[0].set_ylim(
+        [np.amin([np.amin(d2), 0]), np.ceil(np.amax([np.amax(d1), np.amax(d2)]) * 1.1)]
+    )
+    ax[0].set_xlim([np.amin([np.amin(xV), 0]), x_max])
+    ax[1].set_ylabel("Local deviation")
+    ax[1].axhline(0, color="grey")
+    ax[1].axhline(mean_deviation, linestyle="-", color="g", label="mean deviation")
+    ax[1].axhline(tolerance, linestyle="--", color="g", label="tolerance mean")
+    ax[1].axhline(-tolerance, linestyle="--", color="g")
+    ax[1].axhline(2 * tolerance, color="r", label="tolerance max")
+    ax[1].axhline(-2 * tolerance, color="r")
+    ax[1].set_xlim(ax[0].get_xlim())
+    ax[1].legend()
     if plt_ylim:
-        ax.set_ylim(plt_ylim)
+        ax[0].set_ylim(plt_ylim)
     # plt.show()
 
     if fig_name is None:
         n = filename2.replace(".mhd", "_test.png")
     else:
         n = fig_name
     print("Save image test figure :", n)
@@ -439,18 +443,14 @@
     return is_ok
 
 
 def exponential_func(x, a, b):
     return a * np.exp(-b * x)
 
 
-def Gauss(x, A, x0, sigma):
-    return A * np.exp(-((x - x0) ** 2) / (2 * sigma**2))
-
-
 def fit_exponential_decay(data, start, end):
     bin_heights, bin_borders = np.histogram(np.array(data), bins="auto", density=True)
     bin_widths = np.diff(bin_borders)
     bin_centers = bin_borders[:-1] + bin_widths / 2
 
     popt, pcov = scipy.optimize.curve_fit(exponential_func, bin_centers, bin_heights)
     xx = np.linspace(start, end, 100)
@@ -827,14 +827,19 @@
     print(f"Current tree:   {hits2.keys()}")
 
     if scalings1 is None:
         scalings1 = [1] * len(keys1)
     if scalings2 is None:
         scalings2 = [1] * len(keys2)
 
+    if keys1 is None:
+        keys1 = hits1.keys()
+    if keys2 is None:
+        keys2 = hits2.keys()
+
     # keys1, keys2, scalings, tols = get_keys_correspondence(checked_keys)
     is_ok = (
         compare_trees(
             hits1,
             list(hits1.keys()),
             hits2,
             list(hits2.keys()),
@@ -876,39 +881,30 @@
     removed = d2_keys - d1_keys
     modified = {o: (d1[o], d2[o]) for o in shared_keys if d1[o] != d2[o]}
     same = set(o for o in shared_keys if d1[o] == d2[o])
     return added, removed, modified, same
 
 
 # Edit by Andreas and Martina
-def write_gauss_param_to_file(
-    outputdir, planePositionsV, saveFig=False, fNamePrefix="plane", fNameSuffix="a.mhd"
-):
-    # create output dir, if it doesn't exist
-    if not os.path.isdir(outputdir):
-        os.mkdir(outputdir)
-
-    print("fNameSuffix", fNameSuffix)
-    print("write mu and sigma file to dir: ")
-    print(outputdir)
+def write_gauss_param_to_file(output_file_pathV, planePositionsV, saveFig=False):
 
     # Extract gauss param along the two dim of each plane
     sigma_values = []
     mu_values = []
-    for i in planePositionsV:
-        filename = fNamePrefix + str(i) + fNameSuffix
-        filepath = outputdir / filename
+    for fp, i in zip(output_file_pathV, planePositionsV):
+        filepath = Path(fp)
+        outputdir = filepath.parent
 
         # Get data from file
-        data, spacing, shape = read_mhd(filepath)
+        data, spacing, shape = read_mhd(fp)
 
         # Figure output is saved only if fig names are provided
         fig_name = None
         if saveFig:
-            fig_name = str(outputdir) + "/Plane_" + str(i) + fNameSuffix + "_profile"
+            fig_name = str(filepath) + "_profile"
 
         # Get relevant gauss param
         sigma_x, mu_x, sigma_y, mu_y = get_gauss_param_xy(
             data, spacing, shape, filepath=fig_name, saveFig=saveFig
         )
         sigma_values.append([i, sigma_x, sigma_y])
         mu_values.append([i, mu_x, mu_y])
@@ -982,26 +978,27 @@
         positionVec = np.arange(0, width, spacing) - width / 2 + spacing / 2
     else:
         positionVec = np.arange(0, width, spacing)
 
     return positionVec
 
 
-def Gauss(x, A, x0, sigma):
+def gauss_func(x, A, x0, sigma):
     return A * np.exp(-((x - x0) ** 2) / (2 * sigma**2))
 
 
 def gaussian_fit(positionVec, dose):
     # Fit data with Gaussian func
     mean = sum(positionVec * dose) / sum(dose)
     sigma = np.sqrt(sum(dose * (positionVec - mean) ** 2) / sum(dose))
+
     parameters, covariance = scipy.optimize.curve_fit(
-        Gauss, positionVec, dose, p0=[max(dose), mean, sigma]
+        gauss_func, positionVec, dose, p0=[max(dose), mean, sigma]
     )
-    fit = Gauss(positionVec, parameters[0], parameters[1], parameters[2])
+    fit = gauss_func(positionVec, parameters[0], parameters[1], parameters[2])
 
     return parameters, fit
 
 
 def read_mhd(filename):
     img = itk.imread(str(filename))
     data = itk.GetArrayViewFromImage(img)
@@ -1237,41 +1234,45 @@
 
     if (
         (abs(diffmY) > 2 * abs_tol)
         or (abs(diffmZ) > 2 * abs_tol)
         or (abs(mean_diff) > abs_tol)
     ):
         print(
-            f"\033[91m Position error above threshold. DiffX={diffmY:.2f}, diffY={diffmZ:.2f}, threshold is 0.3mm \033[0m"
+            f"\033[91m Position error above threshold. DiffX={diffmY:.2f}, diffY={diffmZ:.2f}, threshold is {abs_tol} mm \033[0m"
         )
         ok = False
 
     # check sizes
-    print("Check size of the spot")
-    print(f"   opengate: ({param_y_out[2]:.2f},{param_z_out[2]:.2f})")
-    print(f"   gate:     ({param_y_ref[2]:.2f},{param_z_ref[2]:.2f})")
 
     diffsY = (param_y_out[2] - param_y_ref[2]) / param_y_ref[2]
     diffsZ = (param_z_out[2] - param_z_ref[2]) / param_z_ref[2]
 
+    print("Check size of the spot")
+    print(f"   opengate: ({param_y_out[2]:.2f},{param_z_out[2]:.2f})")
+    print(f"   gate:     ({param_y_ref[2]:.2f},{param_z_ref[2]:.2f})")
+    print(f"Relative differences: Y: {diffsY}, Z: {diffsZ}")
+
     if (diffsY > thresh) or (diffsZ > thresh):
-        print("\033[91m Size error above threshold \033[0m")
+        print(f"\033[91m Size error above threshold ({thresh}) \033[0m")
         ok = False
 
     return ok
 
 
-def scale_dose(path, scaling, outpath):
+def scale_dose(path, scaling, outpath=""):
+    if not outpath:
+        outpath = insert_suffix_before_extension(path, "Scaled")
     img_mhd_in = itk.imread(path)
     data = itk.GetArrayViewFromImage(img_mhd_in)
     dose = data * scaling
     spacing = img_mhd_in.GetSpacing()
     img = itk_image_view_from_array(dose)
     img.SetSpacing(spacing)
-    itk.imwrite(img, outpath)
+    write_itk_image(img, outpath)
     return outpath
 
 
 def check_dose_grid_geometry(dose_mhd_path, dose_actor):
     img = itk.imread(dose_mhd_path)
     data = itk.GetArrayViewFromImage(img)
     shape = data.shape
@@ -1393,29 +1394,26 @@
     rel_tol=0.03,
 ):
     ok = True
     s1 = 0
     s2 = 0
     x1, doseV1 = get_1D_profile(dose1, shape1, spacing1, axis=axis1)
     x2, doseV2 = get_1D_profile(dose2, shape2, spacing2, axis=axis2)
-    # plt.plot(x1, doseV1)
-    # plt.plot(x2, doseV2)
-    # plt.show()
     for p in pointsV:
         # get dose at the position p [mm]
         cp1 = min(x1, key=lambda x: abs(x - p))
         d1_p = doseV1[np.where(x1 == cp1)]
 
         cp2 = min(x2, key=lambda x: abs(x - p))
         d2_p = doseV2[np.where(x2 == cp2)]
 
         s1 += d1_p
         s2 += d2_p
 
-    print(abs(s1 - s2) / s2)
+    print(f"Relative dose difference is: {abs(s1 - s2) / s2}, tolerance: {rel_tol}.")
 
     # print(f"Dose difference at {p} mm is {diff_pc}%")
     if abs(s1 - s2) / s2 > rel_tol:
         print(f"\033[91mDose difference above threshold \033[0m")
         ok = False
     return ok
 
@@ -1431,14 +1429,88 @@
     else:
         t = np.fabs((s1 - s2) / s1) * 100
     b = t < sum_tolerance
     print_test(b, f"Img sums {s1} vs {s2} : {t:.2f} %  (tol {sum_tolerance:.2f} %)")
     return b
 
 
+def assert_images_ratio(
+    expected_ratio, mhd_1, mhd_2, abs_tolerance=0.1, fn_to_apply=None
+):
+    img1 = itk.imread(str(mhd_1))
+    img2 = itk.imread(str(mhd_2))
+    data1 = itk.GetArrayViewFromImage(img1).ravel()
+    data2 = itk.GetArrayViewFromImage(img2).ravel()
+
+    if fn_to_apply is None:
+        fn_to_apply = lambda x: np.sum(x)
+    sum2 = fn_to_apply(data2)
+    sum1 = fn_to_apply(data1)
+    # if mode.lower() in [ "sum", "cumulative"]:
+    # sum1 = np.sum(data1)
+    # sum2 = np.sum(data2)
+    ratio = sum2 / sum1
+
+    print("\nSum energy dep for phantom 1: ", sum1)
+    print("MSum energy dep for phantom 2: ", sum2)
+    print("Ratio is: ", ratio)
+    print("Expected ratio is: ", expected_ratio)
+
+    is_ok = False
+    if abs(ratio - expected_ratio) < abs_tolerance:
+        is_ok = True
+        print("Test passed.")
+    else:
+        print("\033[91m Ratio not as expected \033[0m")
+
+    return is_ok
+
+
+def assert_images_ratio_per_voxel(
+    expected_ratio, mhd_1, mhd_2, abs_tolerance=0.1, mhd_is_path=True
+):
+    if mhd_is_path:
+        img1 = itk.imread(str(mhd_1))
+        img2 = itk.imread(str(mhd_2))
+    else:
+        img1 = mhd_1
+        img2 = mhd_2
+    data1 = itk.GetArrayViewFromImage(img1).ravel()
+    data2 = itk.GetArrayViewFromImage(img2).ravel()
+
+    ratio = np.divide(data1, data2, out=np.zeros_like(data1), where=data2 != 0)
+    within_tolerance_M = abs(ratio - expected_ratio) < abs_tolerance
+    N_within_tolerance = np.sum(within_tolerance_M)
+    fraction_within_tolerance = N_within_tolerance / np.array(data1).size
+    fraction_within_tolerance = N_within_tolerance / np.sum(data2 != 0)
+
+    mean = np.mean(ratio)
+    std = np.std(ratio)
+    print("Ratio is: ", ratio)
+    print("Expected ratio is: ", expected_ratio)
+    print(f"{fraction_within_tolerance =}")
+    print(f"Mean {mean} \nStd {std}")
+
+    data1_mean = np.mean(data1[:])
+    data2_mean = np.mean(data2[:])
+    print(f"{data1_mean =}")
+    print(f"{data2_mean =}")
+    is_ok = False
+    if fraction_within_tolerance > 0.999:
+        is_ok = True
+        print("Test passed.")
+    else:
+        print("\033[91m Ratio not as expected \033[0m")
+        print(f"{data1[0:4] = }")
+        print(f"{data2[0:4] = }")
+        print(f"{data1[-5:] = }")
+        print(f"{data2[-5:] = }")
+    return is_ok
+
+
 def check_diff(value1, value2, tolerance, txt):
     diff = np.fabs(value1 - value2) / value1 * 100
     t = diff < tolerance
     s = f"{txt} {value1:.2f} vs {value2:.2f} -> {diff:.2f}% (tol={tolerance}%)"
     print_test(t, s)
     return t
```

### Comparing `opengate-10.0b7/opengate/uisessions.py` & `opengate-10.0b8/opengate/uisessions.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/userelement.py` & `opengate-10.0b8/opengate/userelement.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b7/opengate/userhooks.py` & `opengate-10.0b8/opengate/userhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 import opengate.engines
 import opengate_core as g4
+
+import opengate.physics
 from opengate.utility import get_material_name_variants
 
 
+def get_ions_generated_per_spot(simulation_engine):
+    sources = [
+        s
+        for s in simulation_engine.source_engine.sources
+        if s.type_name == "TreatmentPlanPBSource"
+    ]
+    generated_primaries = {}
+    for i, s in enumerate(sources):
+        print(s.user_info.name)
+        generated_primaries[s.user_info.name + f"_{i}"] = s.get_generated_primaries()
+    print(generated_primaries)
+
+
 def check_production_cuts(simulation_engine):
     """Function to be called by opengate after initialization
     of the simulation, i.e. when G4 volumes and regions exist.
     The purpose is to check whether Geant4 has properly set
     the production cuts in the specific region.
 
     The value max_step_size is stored in the attribute hook_log
@@ -35,15 +50,15 @@
             print("Found no cuts in this region")
 
 
 def user_hook_dump_material_properties(simulation_engine):
     print("*** In user hook dump_material_properties ***")
     for vol in simulation_engine.simulation.volume_manager.volumes.values():
         material_name = vol.g4_material.GetName()
-        material_dict = opengate.engines.load_optical_properties_from_xml(
+        material_dict = opengate.physics.load_optical_properties_from_xml(
             simulation_engine.simulation.physics_manager.optical_properties_file,
             material_name,
         )
         print(f"Volume {vol.name} has material {material_name}")
         mpt = vol.g4_material.GetMaterialPropertiesTable()
         if mpt is not None and material_dict is not None:
             const_prop_names = mpt.GetMaterialConstPropertyNames()
@@ -77,20 +92,20 @@
 
 
 def user_hook_em_switches(simulation_engine):
     switches = {}
     switches["auger"] = simulation_engine.physics_engine.g4_em_parameters.Auger()
     switches["fluo"] = simulation_engine.physics_engine.g4_em_parameters.Fluo()
     switches["pixe"] = simulation_engine.physics_engine.g4_em_parameters.Pixe()
-    switches[
-        "auger_cascade"
-    ] = simulation_engine.physics_engine.g4_em_parameters.AugerCascade()
-    switches[
-        "deexcitation_ignore_cut"
-    ] = simulation_engine.physics_engine.g4_em_parameters.DeexcitationIgnoreCut()
+    switches["auger_cascade"] = (
+        simulation_engine.physics_engine.g4_em_parameters.AugerCascade()
+    )
+    switches["deexcitation_ignore_cut"] = (
+        simulation_engine.physics_engine.g4_em_parameters.DeexcitationIgnoreCut()
+    )
     simulation_engine.hook_log.append(switches)
     print("Found the following em parameters via the user hook:")
     for k, v in switches.items():
         print(f"{k}: {v}")
 
 
 def user_hook_active_regions(simulation_engine):
```

### Comparing `opengate-10.0b7/opengate/userinfo.py` & `opengate-10.0b8/opengate/userinfo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-class UserInfo:
+import opengate as gate
+import copy
+
+
+class UserInfo(object):
     """
     A simple dict that contains the list of user parameters.
     Note that the dict is a Box, allowing simpler access to the keys with a dot
     (rather than brackets)
 
     The default elements are set with set_default_user_info according to
     the class found thanks to element_type and type_name
+
+    (need to inherit from object to allow jsonpickle)
     """
 
     def __init__(self, element_type, type_name, name=None):
         # set the element and the type (it will be checked in get_element_class later)
         # element_type is Volume, Source or Actor
         # set the name
         self._name = name
@@ -26,7 +32,16 @@
         # make 'name' a property make it read_only.
         # user cannot change the name of the object once it is declared
         return self._name
 
     def __str__(self):
         s = f"{self.element_type} {self.name} : {self.__dict__}"
         return s
+
+    def copy_from(self, ui):
+        for att in ui.__dict__:
+            if att == "_name":
+                continue
+            self.__dict__[att] = copy.deepcopy(ui.__dict__[att])
+
+    def initialize_source_before_g4_engine(self, source):
+        pass
```

### Comparing `opengate-10.0b7/opengate/utility.py` & `opengate-10.0b8/opengate/utility.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import scipy as sc
 from numpy.random import MT19937
 from numpy.random import RandomState, SeedSequence
 import random
 from box import Box
 import textwrap
 import inspect
 import pkg_resources
@@ -144,14 +145,33 @@
 def ensure_filename_is_str(filename):
     # Algorithms (itk) do not support Path -> convert to str
     if isinstance(filename, Path):
         return str(filename)
     return filename
 
 
+def insert_suffix_before_extension(file_path, suffix, suffixSeparator="-"):
+    print(file_path)
+    print(suffix)
+    if suffix:
+        suffix = suffix.strip("_- *")
+        suffix = suffix.lower()
+    else:
+        return file_path
+    if not isinstance(file_path, Path):
+        path = Path(file_path)
+    else:
+        path = file_path
+
+    new_file_name = path.with_name(path.stem + suffixSeparator + suffix + path.suffix)
+    print(new_file_name)
+
+    return new_file_name
+
+
 def get_random_folder_name(size=8, create=True):
     r = "".join(random.choices(string.ascii_lowercase + string.digits, k=size))
     r = "run." + r
     if create:
         if not os.path.exists(r):
             print(f"Creating output folder {r}")
             os.mkdir(r)
@@ -208,14 +228,19 @@
             return f"{release_date}"
         else:
             return "unknown"
     else:
         return "unknown"
 
 
+def get_contrib_path():
+    module_path = os.path.dirname(__file__)
+    return Path(module_path) / "contrib"
+
+
 def print_opengate_info():
     """
     Print information about OpenGate and the environment
     """
 
     gi = g4.GateInfo
     v = gi.get_G4Version().replace("$Name: ", "")
@@ -246,7 +271,30 @@
         print(f"GATE git sha     {sha}")
         commit = git_repo.head.commit
         commit_date = commit.committed_datetime
         print(f"GATE date        {commit_date}  (last commit)")
 
     except:
         print(f"GATE date        {get_release_date(version('opengate'))} (pypi)")
+
+
+def standard_error_c4_correction(n):
+    """
+    Parameters
+    ----------
+    n : integer
+        Number of subsets (of the samples).
+
+    Returns
+    -------
+    c4 : double
+        Factor to convert the biased standard error of the mean of subsets of the sample into an unbiased
+        -  assuming a normal distribution .
+        Usage: standard_error(unbiased) = standard_deviation_of_mean(=biased) / c4
+        The reason is that the standard deviation of the mean of subsets of the sample X underestimates the true standard error. For n = 2 this underestimation is about 25%.
+
+        Values for c4: n=2: 0.7979; n= 9: 0.9693
+
+    """
+    return (
+        np.sqrt(2 / (n - 1)) * sc.special.gamma(n / 2) / sc.special.gamma((n - 1) / 2)
+    )
```

