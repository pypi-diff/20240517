# Comparing `tmp/scqubits-4.0.0.tar.gz` & `tmp/scqubits-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scqubits-4.0.0.tar", last modified: Sat Mar  2 02:45:58 2024, max compression
+gzip compressed data, was "scqubits-4.1.0.tar", last modified: Fri May 17 01:21:49 2024, max compression
```

## Comparing `scqubits-4.0.0.tar` & `scqubits-4.1.0.tar`

### file list

```diff
@@ -1,153 +1,155 @@
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.850462 scqubits-4.0.0/
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1549 2024-03-02 02:45:01.000000 scqubits-4.0.0/LICENSE
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      261 2024-03-02 02:45:01.000000 scqubits-4.0.0/MANIFEST.in
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     1892 2024-03-02 02:45:58.850462 scqubits-4.0.0/PKG-INFO
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     3853 2024-03-02 02:45:01.000000 scqubits-4.0.0/README.md
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)       82 2024-03-02 02:45:01.000000 scqubits-4.0.0/optional-requirements.txt
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      118 2024-03-02 02:45:01.000000 scqubits-4.0.0/requirements.txt
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.834462 scqubits-4.0.0/scqubits/
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     4145 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/__init__.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.838462 scqubits-4.0.0/scqubits/core/
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      482 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/__init__.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     6999 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/central_dispatch.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    53584 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/circuit.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     8543 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/circuit_input.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    29578 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/circuit_noise.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)   153686 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/circuit_routines.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    28544 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/circuit_utils.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1107 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/constants.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    55192 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/cos2phi_qubit.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     4194 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/descriptors.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    22273 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/diag.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     9106 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/discretization.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    39299 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/flux_qubit.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    19590 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/fluxonium.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     3645 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/generic_qubit.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    50361 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/hilbert_space.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    24921 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/namedslots_array.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    62438 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/noise.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     7794 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/operators.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     8956 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/oscillator.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    60305 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/param_sweep.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    45659 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_base.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.838462 scqubits-4.0.0/scqubits/core/qubit_img/
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)   159663 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/Bifluxon.jpg
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)   104902 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/Cos2PhiQubit.jpg
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)   108284 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/FluxQubit.jpg
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)   320438 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/Fluxonium.jpg
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)   125604 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/FullZeroPi.jpg
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    63343 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/KerrOscillator.jpg
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    90602 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/Oscillator.jpg
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)   154768 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/Snailmon.jpg
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    97656 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/Transmon.jpg
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)   127799 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/TunableTransmon.jpg
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)   116961 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/qubit_img/ZeroPi.jpg
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    16414 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/spec_lookup.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     9058 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/storage.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     3071 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/sweeps.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    86604 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/symbolic_circuit.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    32306 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/transmon.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     4865 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/units.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    33462 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/zeropi.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    31121 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/core/zeropi_full.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.838462 scqubits-4.0.0/scqubits/explorer/
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/explorer/__init__.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    11849 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/explorer/explorer_panels.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    12577 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/explorer/explorer_settings.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    24839 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/explorer/explorer_widget.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.842462 scqubits-4.0.0/scqubits/io_utils/
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/io_utils/__init__.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     5914 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/io_utils/fileio.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    13959 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/io_utils/fileio_backends.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     2530 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/io_utils/fileio_qutip.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    11771 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/io_utils/fileio_serializers.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     5415 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/settings.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      689 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/testing.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.842462 scqubits-4.0.0/scqubits/tests/
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/__init__.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     9776 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/conftest.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.850462 scqubits-4.0.0/scqubits/tests/data/
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)      160 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/circuit_DFC.yaml
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)       57 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/circuit_fluxonium.yaml
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)      146 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/circuit_zeropi.yaml
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    15496 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/cos2phiqubit_1.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)   214632 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/cos2phiqubit_2.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)   472471 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/cos2phiqubit_4.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    16032 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/cos2phiqubit_5.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    15048 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fluxonium_1.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    21667 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fluxonium_2.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)   367163 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fluxonium_4.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    14512 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fluxonium_5.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    14136 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fluxqubit_1.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    39269 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fluxqubit_2.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)  1205265 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fluxqubit_4.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    14960 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fluxqubit_5.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    17920 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fullzeropi_1.hdf5
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    33599 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/fullzeropi_2.hdf5
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    15824 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/snailmon_1.hdf5
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    22048 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/snailmon_2.hdf5
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)   520543 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/snailmon_4.hdf5
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    16360 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/snailmon_5.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    13624 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/transmon_1.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    18560 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/transmon_2.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)   120906 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/transmon_4.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    14416 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/transmon_5.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     9024 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/zeropi-test.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    17664 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/zeropi_1.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)   788882 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/zeropi_2.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)  1761598 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/zeropi_4.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    18200 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/zeropi_5.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     9264 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/data/zpifull-test.hdf5
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     2659 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_centraldispatch.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     8987 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_circuit.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)      918 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_circuit_plot.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1020 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_cos2phiqubit.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     2424 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_explorer.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      951 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_fluxonium.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      953 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_fluxqubit.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     2110 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_fullzeropi.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      595 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_gui.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    16747 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_hilbertspace.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1509 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_namedslotsndarray.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     4762 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_noise.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1545 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_parameters.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     4191 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_parametersweep.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    16340 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_spectrumlookup.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1172 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_transmon.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1367 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_units.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1006 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/tests/test_zeropi.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.850462 scqubits-4.0.0/scqubits/ui/
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      619 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/__init__.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    66978 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/gui.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    17280 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/gui_custom_widgets.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    11363 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/gui_defaults.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     3719 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/gui_navbar.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    15936 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/gui_setup.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    21542 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/hspace_widget.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.850462 scqubits-4.0.0/scqubits/ui/icons/
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     3660 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/icons/En.png
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     5345 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/icons/Me.png
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     9994 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/icons/MeS.png
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     6495 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/icons/T1.png
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    11754 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/icons/psi.png
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     7272 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/icons/scq-logo.png
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     3167 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/ui/qubit_widget.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.850462 scqubits-4.0.0/scqubits/utils/
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      619 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/utils/__init__.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1856 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/utils/cpu_switch.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    15759 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/utils/misc.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     6892 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/utils/plot_defaults.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     7046 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/utils/plot_utils.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    18985 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/utils/plotting.py
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    16009 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/utils/spectrum_utils.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     1293 2024-03-02 02:45:01.000000 scqubits-4.0.0/scqubits/utils/typedefs.py
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)      105 2024-03-02 02:45:58.000000 scqubits-4.0.0/scqubits/version.py
-drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-03-02 02:45:58.834462 scqubits-4.0.0/scqubits.egg-info/
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     1892 2024-03-02 02:45:58.000000 scqubits-4.0.0/scqubits.egg-info/PKG-INFO
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     4357 2024-03-02 02:45:58.000000 scqubits-4.0.0/scqubits.egg-info/SOURCES.txt
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)        1 2024-03-02 02:45:58.000000 scqubits-4.0.0/scqubits.egg-info/dependency_links.txt
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)        1 2024-03-02 02:45:58.000000 scqubits-4.0.0/scqubits.egg-info/not-zip-safe
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)      235 2024-03-02 02:45:58.000000 scqubits-4.0.0/scqubits.egg-info/requires.txt
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)      101 2024-03-02 02:45:58.000000 scqubits-4.0.0/scqubits.egg-info/top_level.txt
--rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)       38 2024-03-02 02:45:58.850462 scqubits-4.0.0/setup.cfg
--rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     4725 2024-03-02 02:45:01.000000 scqubits-4.0.0/setup.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.415420 scqubits-4.1.0/
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     1549 2024-05-08 14:04:40.000000 scqubits-4.1.0/LICENSE
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)      261 2024-05-08 14:04:40.000000 scqubits-4.1.0/MANIFEST.in
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     2476 2024-05-17 01:21:49.415420 scqubits-4.1.0/PKG-INFO
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     3853 2024-05-08 14:04:40.000000 scqubits-4.1.0/README.md
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)       81 2024-05-16 23:48:45.000000 scqubits-4.1.0/optional-requirements.txt
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)      172 2024-05-16 23:48:45.000000 scqubits-4.1.0/requirements.txt
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.399420 scqubits-4.1.0/scqubits/
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     4145 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/__init__.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.403420 scqubits-4.1.0/scqubits/core/
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)      482 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/__init__.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     6999 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/central_dispatch.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    53584 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/circuit.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     8565 2024-05-16 23:48:45.000000 scqubits-4.1.0/scqubits/core/circuit_input.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    29578 2024-05-15 03:36:58.000000 scqubits-4.1.0/scqubits/core/circuit_noise.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)   153945 2024-05-16 23:48:45.000000 scqubits-4.1.0/scqubits/core/circuit_routines.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    28544 2024-05-15 03:36:58.000000 scqubits-4.1.0/scqubits/core/circuit_utils.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     1107 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/constants.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    55192 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/cos2phi_qubit.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     4194 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/descriptors.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    23211 2024-05-16 23:48:45.000000 scqubits-4.1.0/scqubits/core/diag.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     9106 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/discretization.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    39299 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/flux_qubit.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    19590 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/fluxonium.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     3645 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/generic_qubit.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    50475 2024-05-17 00:00:58.000000 scqubits-4.1.0/scqubits/core/hilbert_space.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    24921 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/namedslots_array.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    62438 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/noise.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     7794 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/operators.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     8956 2024-05-15 03:36:58.000000 scqubits-4.1.0/scqubits/core/oscillator.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    60305 2024-05-15 03:36:58.000000 scqubits-4.1.0/scqubits/core/param_sweep.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    45659 2024-05-15 03:36:58.000000 scqubits-4.1.0/scqubits/core/qubit_base.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.407420 scqubits-4.1.0/scqubits/core/qubit_img/
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)   159663 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/Bifluxon.jpg
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)   104902 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/Cos2PhiQubit.jpg
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)   108284 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/FluxQubit.jpg
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)   320438 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/Fluxonium.jpg
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)   125604 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/FullZeroPi.jpg
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    63343 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/KerrOscillator.jpg
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    90602 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/Oscillator.jpg
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)   154768 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/Snailmon.jpg
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    97656 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/Transmon.jpg
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)   127799 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/TunableTransmon.jpg
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)   116961 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/qubit_img/ZeroPi.jpg
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    16414 2024-05-15 03:36:58.000000 scqubits-4.1.0/scqubits/core/spec_lookup.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     9058 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/storage.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     3071 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/sweeps.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    86604 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/symbolic_circuit.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    32306 2024-05-15 03:36:58.000000 scqubits-4.1.0/scqubits/core/transmon.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     4865 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/units.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    33462 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/zeropi.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    31121 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/core/zeropi_full.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.407420 scqubits-4.1.0/scqubits/explorer/
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/explorer/__init__.py
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    11849 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/explorer/explorer_panels.py
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    12577 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/explorer/explorer_settings.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    24791 2024-05-16 23:48:45.000000 scqubits-4.1.0/scqubits/explorer/explorer_widget.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.407420 scqubits-4.1.0/scqubits/io_utils/
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/io_utils/__init__.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     5914 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/io_utils/fileio.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    13959 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/io_utils/fileio_backends.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     2382 2024-05-16 23:48:45.000000 scqubits-4.1.0/scqubits/io_utils/fileio_qutip.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    11771 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/io_utils/fileio_serializers.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)       27 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/py.typed
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    25247 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/qubit_base_OLD.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     5415 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/settings.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)      689 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/testing.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.407420 scqubits-4.1.0/scqubits/tests/
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/__init__.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     9776 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/conftest.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.415420 scqubits-4.1.0/scqubits/tests/data/
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)      160 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/circuit_DFC.yaml
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)       57 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/circuit_fluxonium.yaml
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)      146 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/circuit_zeropi.yaml
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    15496 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/cos2phiqubit_1.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)   214632 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/cos2phiqubit_2.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)   472471 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/cos2phiqubit_4.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    16032 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/cos2phiqubit_5.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    15048 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fluxonium_1.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    21667 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fluxonium_2.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)   367163 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fluxonium_4.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    14512 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fluxonium_5.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    14136 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fluxqubit_1.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    39269 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fluxqubit_2.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)  1205265 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fluxqubit_4.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    14960 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fluxqubit_5.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    17920 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fullzeropi_1.hdf5
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    33599 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/fullzeropi_2.hdf5
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    15824 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/snailmon_1.hdf5
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    22048 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/snailmon_2.hdf5
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)   520543 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/snailmon_4.hdf5
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    16360 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/snailmon_5.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    13624 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/transmon_1.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    18560 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/transmon_2.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)   120906 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/transmon_4.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    14416 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/transmon_5.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     9024 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/zeropi-test.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    17664 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/zeropi_1.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)   788882 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/zeropi_2.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)  1761598 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/zeropi_4.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    18200 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/zeropi_5.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     9264 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/data/zpifull-test.hdf5
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     2659 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_centraldispatch.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)     8987 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_circuit.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)      918 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_circuit_plot.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     1020 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_cos2phiqubit.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     2424 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_explorer.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)      951 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_fluxonium.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)      953 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_fluxqubit.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     2110 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_fullzeropi.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)      595 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_gui.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    16747 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_hilbertspace.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     1509 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_namedslotsndarray.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     4762 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_noise.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     1545 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_parameters.py
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     4191 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_parametersweep.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    16340 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_spectrumlookup.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     1172 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_transmon.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     1367 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_units.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     1006 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/tests/test_zeropi.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.415420 scqubits-4.1.0/scqubits/ui/
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)      619 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/__init__.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    66931 2024-05-16 23:48:45.000000 scqubits-4.1.0/scqubits/ui/gui.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    17280 2024-05-15 03:36:58.000000 scqubits-4.1.0/scqubits/ui/gui_custom_widgets.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)    11363 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/gui_defaults.py
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     3719 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/gui_navbar.py
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    15936 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/gui_setup.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    21542 2024-05-15 03:36:58.000000 scqubits-4.1.0/scqubits/ui/hspace_widget.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.415420 scqubits-4.1.0/scqubits/ui/icons/
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     3660 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/icons/En.png
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     5345 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/icons/Me.png
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     9994 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/icons/MeS.png
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     6495 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/icons/T1.png
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)    11754 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/icons/psi.png
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     7272 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/icons/scq-logo.png
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     3167 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/ui/qubit_widget.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.415420 scqubits-4.1.0/scqubits/utils/
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)      619 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/utils/__init__.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     1856 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/utils/cpu_switch.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    15423 2024-05-16 23:48:45.000000 scqubits-4.1.0/scqubits/utils/misc.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)     6892 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/utils/plot_defaults.py
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     7046 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/utils/plot_utils.py
+-rwxr--r--   0 pgroszko  (1000) pgroszko  (1000)    18985 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/utils/plotting.py
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)    16009 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/utils/spectrum_utils.py
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     1293 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits/utils/typedefs.py
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)      105 2024-05-17 01:21:49.000000 scqubits-4.1.0/scqubits/version.py
+drwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)        0 2024-05-17 01:21:49.415420 scqubits-4.1.0/scqubits.egg-info/
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     2476 2024-05-17 01:21:49.000000 scqubits-4.1.0/scqubits.egg-info/PKG-INFO
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)     4402 2024-05-17 01:21:49.000000 scqubits-4.1.0/scqubits.egg-info/SOURCES.txt
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)        1 2024-05-17 01:21:49.000000 scqubits-4.1.0/scqubits.egg-info/dependency_links.txt
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)        1 2024-05-08 14:04:42.000000 scqubits-4.1.0/scqubits.egg-info/not-zip-safe
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)      295 2024-05-17 01:21:49.000000 scqubits-4.1.0/scqubits.egg-info/requires.txt
+-rw-r--r--   0 pgroszko  (1000) pgroszko  (1000)      101 2024-05-17 01:21:49.000000 scqubits-4.1.0/scqubits.egg-info/top_level.txt
+-rw-rw-r--   0 pgroszko  (1000) pgroszko  (1000)       38 2024-05-17 01:21:49.415420 scqubits-4.1.0/setup.cfg
+-rwxrwxr-x   0 pgroszko  (1000) pgroszko  (1000)     4725 2024-05-17 01:04:11.000000 scqubits-4.1.0/setup.py
```

### Comparing `scqubits-4.0.0/LICENSE` & `scqubits-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/README.md` & `scqubits-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/__init__.py` & `scqubits-4.1.0/scqubits/__init__.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/central_dispatch.py` & `scqubits-4.1.0/scqubits/core/central_dispatch.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/circuit.py` & `scqubits-4.1.0/scqubits/core/circuit.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/circuit_input.py` & `scqubits-4.1.0/scqubits/core/circuit_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 energy_names = ["EJ", "EC", "EL"]
 
 
 UNITS_FREQ_ENERGY = Literal("Hz") ^ Literal("J") ^ Literal("eV")
 
 UNITS = {name: Opt(PREFIX, None) for name in energy_names}
-UNITS["EJ"] += UNITS_FREQ_ENERGY ^ Literal("A")  # Ampere
+UNITS["EJ"] += UNITS_FREQ_ENERGY ^ Literal("A") ^ Literal("H")  # Ampere, Henry
 UNITS["EC"] += UNITS_FREQ_ENERGY ^ Literal("F")  # Farad
 UNITS["EL"] += UNITS_FREQ_ENERGY ^ Literal("H")  # Henry
 for name, unit in UNITS.items():
     unit.leave_whitespace()  # allow only "kHz", not "k Hz"
     unit.set_name(f"{name}_UNITS")
 
 # - Parameter specifications --------------------------------
```

### Comparing `scqubits-4.0.0/scqubits/core/circuit_noise.py` & `scqubits-4.1.0/scqubits/core/circuit_noise.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/circuit_routines.py` & `scqubits-4.1.0/scqubits/core/circuit_routines.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,14 +223,18 @@
 
         self.normal_mode_freqs = normal_mode_freqs_sq**0.5
 
         self._hamiltonian_sym_for_numerics = round_symbolic_expr(
             self._transform_hamiltonian(self.hamiltonian_symbolic, eig_vecs).expand(),
             12,
         )
+        for flux in self.external_fluxes:
+            self._hamiltonian_sym_for_numerics = (
+                self._hamiltonian_sym_for_numerics.subs(flux, flux * np.pi * 2)
+            )
         # storing the annihilation operators in the eigenbasis
         osc_lengths = (
             np.diagonal(
                 8
                 * np.linalg.inv(eig_vecs.T @ np.linalg.inv(EC) @ eig_vecs)
                 @ np.linalg.inv(eig_vecs.T @ EL @ eig_vecs)
             )
@@ -1639,15 +1643,15 @@
         """
         Returns the Identity operator for the entire Hilbert space of the circuit.
         """
         if (
             hasattr(self, "hierarchical_diagonalization")
             and self.hierarchical_diagonalization
         ):
-            return None
+            return self._identity_qobj()
         dim = self.hilbertdim()
         if self.type_of_matrices == "sparse":
             op = sparse.identity(dim, format="csc")
             return op
         elif self.type_of_matrices == "dense":
             return np.identity(dim)
 
@@ -1681,15 +1685,15 @@
                     (diagonal, [0]), shape=(phi_grid.pt_count, phi_grid.pt_count)
                 ).tocsc()
             elif "Q" in var_sym.name:
                 exp_i_theta = sp.linalg.expm(
                     _i_d_dphi_operator(phi_grid).toarray() * prefactor * 1j
                 )
         elif var_basis == "harmonic":
-            osc_length = self.osc_lengths[var_index]
+            osc_length = self.get_osc_param(var_index, which_param="length")
             if "θ" in var_sym.name:
                 exp_argument_op = op.a_plus_adag_sparse(
                     self.cutoffs_dict()[var_index],
                     prefactor=(osc_length / 2**0.5),
                 )
             elif "Q" in var_sym.name:
                 exp_argument_op = op.iadag_minus_ia_sparse(
@@ -2546,16 +2550,16 @@
 
                 if parameter_expr in time_dep_terms:
                     time_dep_terms[parameter_expr] = (
                         operator_expr * expr_dict[term] * term_expr_dict[inner_term]
                         + time_dep_terms[parameter_expr]
                     )
                 else:
-                    time_dep_terms[parameter_expr] = (
-                        operator_expr * expr_dict[term] * term_expr_dict[inner_term]
+                    time_dep_terms[parameter_expr] = round_symbolic_expr(
+                        operator_expr * expr_dict[term] * term_expr_dict[inner_term], 13
                     )
 
         for parameter_expr in time_dep_terms:
             # separating the time independent constants
             for sym in parameter_expr.free_symbols:
                 if sym not in free_var_symbols:
                     parameter_expr = parameter_expr.subs(sym, getattr(self, sym.name))
@@ -2697,15 +2701,15 @@
             equalities_in_latex = equalities_in_latex[:-4] + " $"
             display(Latex(equalities_in_latex))
 
     def __repr__(self) -> str:
         # string to describe the Circuit
         return self._id_str
 
-    def info(self):
+    def _repr_latex_(self):
         """
         Describes the Circuit instance, its parameters, and the symbolic Hamiltonian.
         """
         # string to describe the Circuit
         if not _HAS_IPYTHON:
             return self._id_str
         # Hamiltonian string
```

### Comparing `scqubits-4.0.0/scqubits/core/circuit_utils.py` & `scqubits-4.1.0/scqubits/core/circuit_utils.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/constants.py` & `scqubits-4.1.0/scqubits/core/constants.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/cos2phi_qubit.py` & `scqubits-4.1.0/scqubits/core/cos2phi_qubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/descriptors.py` & `scqubits-4.1.0/scqubits/core/descriptors.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/diag.py` & `scqubits-4.1.0/scqubits/core/diag.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from qutip import Qobj
 from scipy.sparse import csc_matrix
 from scqubits.io_utils.fileio_qutip import QutipEigenstates
 from scqubits.utils.spectrum_utils import order_eigensystem, has_degeneracy
 
 import copy
 import numpy as np
+import qutip as q
 import scipy as sp
 import scqubits.settings as settings
 import warnings
 
 
 def _dict_merge(
     d: Dict[str, Any],
@@ -63,50 +64,72 @@
     return d_new
 
 
 def _cast_matrix(
     matrix: Union[ndarray, csc_matrix, Qobj], cast_to: str, force_cast: bool = True
 ) -> Union[ndarray, csc_matrix, Qobj]:
     """
-    Casts a given matrix into a required form ('sparse' or 'dense')
-    as defined by `cast_to` parameter.
-    Note that in some cases casting may not be explicitly needed,
-    for example: the sparse matrix routines can can often accept
-    dense matrices. The parameter `force_cast` determines if the
-    casing should be always done, or only where it is necessary.
+    Casts a given operator (possibly given as a `Qobj`) into a
+    required form ('sparse' or 'dense' numpy array or scipy martrix) as
+    defined by `cast_to` parameter.
+
+    Operators of the type `Qobj` are first converted to a `ndarray` or a
+    scipy sparse matrix form (depending on the given object's underlying
+    `dtype`).
+
+    Later those are converted (or not) to a dense or spare forms depending
+    on whether `force_cast` is set.
+
+    NOTE: Currently we only ever cast to the csc format for sparse
+    matrices. Internally `Qobj` uses the csr or dia formats instead, however.
+    It could be worthwhile to also use those representations directly
+    whenever it makes sense, and avoid unnecessary conversions.
 
     Parameters
     ----------
-    matrix: Qobj, ndarray or csc_matrx
+    matrix: `Qobj`, `ndarray` or scipy's sparse matrix format
         matrix given as an ndarray, Qobj, or scipy's sparse matrix format
     cast_to: str
         string representing the format that matrix should be cast into: 'sparse' or 'dense'
     force_cast: bool
-        determines of casting should be always performed or only where necessary
+        determines if explicit casting to dense or sparse format should be always
+        performed
 
     Returns
     ----------
-        matrix in the right sparse or dense form
+        matrix in the sparse or dense form
 
     """
+    if cast_to not in ["sparse", "dense"]:
+        raise ValueError("Can only cast matrix to 'sparse' or 'dense' forms.")
+
     m = matrix
 
-    if cast_to == "sparse":
-        if isinstance(matrix, Qobj):
-            m = csc_matrix(matrix.data)
-        elif force_cast and isinstance(matrix, ndarray):
-            m = csc_matrix(matrix)
-
-    elif cast_to == "dense":
-        if isinstance(matrix, Qobj):
-            m = matrix.full()
-        elif force_cast and sp.sparse.issparse(matrix):
-            m = matrix.toarray()
-    else:
-        raise ValueError("Can only matrix to 'sparse' or 'dense' forms.")
+    # First, if we are dealing with a Qobj, we convert it to either
+    # an ndarray or a scipy sparse matrix.
+    if isinstance(matrix, Qobj):
+        if q.__version__ >= "5.0.0":
+            if matrix.dtype == q.core.data.dense.Dense:
+                m = matrix.full()
+            else:
+                # This could be costly if the data is in a "Dia"
+                # form. In the future we may want to support other
+                # formats as well.
+                m = matrix.to("CSR").as_data()
+        else:
+            # In previous versions of qutip data was always in the csr form
+            m = matrix.data
+
+    # Next, we do casting dense or sparse (CSC) representation
+    # if force_cast is True
+    if force_cast:
+        if cast_to == "dense" and not isinstance(m, ndarray):
+            m = m.toarray()
+        if cast_to == "sparse":
+            m = csc_matrix(m)
 
     return m
 
 
 def _convert_evecs_to_qobjs(evecs: ndarray, matrix_qobj, wrap: bool = False) -> ndarray:
     """
     Converts an `ndarray` containing eigenvectors (that would be typically
@@ -129,15 +152,15 @@
 
     """
     evecs_count = evecs.shape[1]
     evec_dims = [matrix_qobj.dims[0], [1] * len(matrix_qobj.dims[0])]
     evecs_qobj = np.empty((evecs_count,), dtype=object)
 
     for i in range(evecs_count):
-        v = Qobj(evecs[:, i], dims=evec_dims, type="ket")
+        v = Qobj(evecs[:, i], dims=evec_dims)
         evecs_qobj[i] = v / v.norm()
 
     # Optionally, we wrap the resulting array in QutipEigenstates as is done in HilbertSpace.
     if wrap:
         evecs_qobj = evecs_qobj.view(QutipEigenstates)
 
     return evecs_qobj
```

### Comparing `scqubits-4.0.0/scqubits/core/discretization.py` & `scqubits-4.1.0/scqubits/core/discretization.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/flux_qubit.py` & `scqubits-4.1.0/scqubits/core/flux_qubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/fluxonium.py` & `scqubits-4.1.0/scqubits/core/fluxonium.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/generic_qubit.py` & `scqubits-4.1.0/scqubits/core/generic_qubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/hilbert_space.py` & `scqubits-4.1.0/scqubits/core/hilbert_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,14 +439,15 @@
         # The following attributes are for compatibility with SpectrumLookupMixin
         self._data: Dict[str, Any] = {}
         self._parameters = Parameters({"dummy_parameter": np.array([0])})
         self._ignore_low_overlap = ignore_low_overlap
         self._current_param_indices = 0
         self._evals_count = self.dimension
         self._out_of_sync = False
+        self._out_of_sync_warning_issued = False
         # end attributes for compatibility with SpectrumLookupMixin
 
         dispatch.CENTRAL_DISPATCH.register("QUANTUMSYSTEM_UPDATE", self)
         dispatch.CENTRAL_DISPATCH.register("INTERACTIONTERM_UPDATE", self)
         dispatch.CENTRAL_DISPATCH.register("INTERACTIONLIST_UPDATE", self)
 
     @overload
@@ -825,19 +826,19 @@
             speed up computation; these are provided in dict form via <subsys>: esys
 
         Returns
         -------
             composite Hamiltonian composed of bare Hamiltonians of subsystems
             independent of the external parameter
         """
-        bare_hamiltonian = (
-            qt.Qobj(0, dims=[self.subsystem_dims] * 2)
-            if qt.__version__ >= "5.0.0"
-            else qt.Qobj(0)
+        # We create a dimension [1] system if no subsystems have been given
+        bare_hamiltonian = qt.qzero(
+            [1] if len(self.subsystem_dims) == 0 else self.subsystem_dims
         )
+
         for subsys_index, subsys in enumerate(self):
             if bare_esys is not None and subsys_index in bare_esys:
                 evals = bare_esys[subsys_index][0]
             else:
                 evals = subsys.eigenvals(evals_count=subsys.truncated_dim)
             bare_hamiltonian += self.diag_hamiltonian(subsys, evals)
         return bare_hamiltonian
@@ -856,18 +857,17 @@
             speed up computation; these are provided in dict form via <subsys>: esys
 
         Returns
         -------
             interaction Hamiltonian
         """
         if not self.interaction_list:
-            return (
-                qt.Qobj(0, dims=[self.subsystem_dims] * 2)
-                if qt.__version__ >= "5.0.0"
-                else qt.Qobj(0)
+            # We return a dimension [1] system if no subsystems have been given
+            return qt.qzero(
+                [1] if len(self.subsystem_dims) == 0 else self.subsystem_dims
             )
 
         operator_list = []
         for term in self.interaction_list:
             if isinstance(term, qt.Qobj):
                 operator_list.append(term)
             elif isinstance(term, (InteractionTerm, InteractionTermStr)):
```

### Comparing `scqubits-4.0.0/scqubits/core/namedslots_array.py` & `scqubits-4.1.0/scqubits/core/namedslots_array.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/noise.py` & `scqubits-4.1.0/scqubits/core/noise.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/operators.py` & `scqubits-4.1.0/scqubits/core/operators.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/oscillator.py` & `scqubits-4.1.0/scqubits/core/oscillator.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/param_sweep.py` & `scqubits-4.1.0/scqubits/core/param_sweep.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_base.py` & `scqubits-4.1.0/scqubits/core/qubit_base.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/Bifluxon.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/Bifluxon.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/Cos2PhiQubit.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/Cos2PhiQubit.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/FluxQubit.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/FluxQubit.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/Fluxonium.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/Fluxonium.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/FullZeroPi.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/FullZeroPi.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/KerrOscillator.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/KerrOscillator.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/Oscillator.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/Oscillator.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/Snailmon.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/Snailmon.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/Transmon.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/Transmon.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/TunableTransmon.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/TunableTransmon.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/qubit_img/ZeroPi.jpg` & `scqubits-4.1.0/scqubits/core/qubit_img/ZeroPi.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/spec_lookup.py` & `scqubits-4.1.0/scqubits/core/spec_lookup.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/storage.py` & `scqubits-4.1.0/scqubits/core/storage.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/sweeps.py` & `scqubits-4.1.0/scqubits/core/sweeps.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/symbolic_circuit.py` & `scqubits-4.1.0/scqubits/core/symbolic_circuit.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/transmon.py` & `scqubits-4.1.0/scqubits/core/transmon.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/units.py` & `scqubits-4.1.0/scqubits/core/units.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/zeropi.py` & `scqubits-4.1.0/scqubits/core/zeropi.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/core/zeropi_full.py` & `scqubits-4.1.0/scqubits/core/zeropi_full.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/explorer/explorer_panels.py` & `scqubits-4.1.0/scqubits/explorer/explorer_panels.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/explorer/explorer_settings.py` & `scqubits-4.1.0/scqubits/explorer/explorer_settings.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/explorer/explorer_widget.py` & `scqubits-4.1.0/scqubits/explorer/explorer_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,14 @@
         """Set up all widget GUI elements and class attributes."""
         self.sweep = sweep
         self.ncols = ncols  # number of columns used for axes in the figure display
 
         self.subsystems: List[QuantumSystem] = self.sweep.hilbertspace.subsystem_list
         self.subsys_names: List[str] = [subsys.id_str for subsys in self.subsystems]
 
-        utils.check_matplotlib_compatibility()
-
         # == GUI elements =========================================================
         self.ui: Dict[str, Any] = {}
         self.build_panel_switches()
         self.ui["add_plot_dialog"] = self.build_ui_add_plot_dialog()
 
         self.ui["sweep_param_dropdown"] = ui.InitializedSelect(
             class_="px-2",
```

### Comparing `scqubits-4.0.0/scqubits/io_utils/fileio.py` & `scqubits-4.1.0/scqubits/io_utils/fileio.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/io_utils/fileio_backends.py` & `scqubits-4.1.0/scqubits/io_utils/fileio_backends.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/io_utils/fileio_qutip.py` & `scqubits-4.1.0/scqubits/io_utils/fileio_qutip.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,26 +24,21 @@
 
     @classmethod
     def deserialize(cls, io_data: IOData) -> np.ndarray:  # type:ignore
         """
         Take the given IOData and return an instance of the described class, initialized
         with the data stored in io_data.
         """
-        qobj_dims = io_data.ndarrays["qobj_dims"]
+        # Qobj in Qutip>=5 wants this to be a nested list
+        qobj_dims = io_data.ndarrays["qobj_dims"].tolist()
         qobj_shape = io_data.ndarrays["qobj_shape"]
         evec_array = io_data.ndarrays["evecs"]
+
         qt_eigenstates = np.asarray(
-            [
-                (
-                    qt.Qobj(evec, type="ket")
-                    if qt.__version__ >= "5.0.0"
-                    else qt.Qobj(evec, dims=qobj_dims, shape=qobj_shape, type="ket")
-                )
-                for evec in evec_array
-            ],
+            [qt.Qobj(evec, dims=qobj_dims) for evec in evec_array],
             dtype=np.dtype("O"),
         )
         return qt_eigenstates
 
     def serialize(self) -> IOData:
         """
         Convert the content of the current class instance into IOData format.
```

### Comparing `scqubits-4.0.0/scqubits/io_utils/fileio_serializers.py` & `scqubits-4.1.0/scqubits/io_utils/fileio_serializers.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/settings.py` & `scqubits-4.1.0/scqubits/settings.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/testing.py` & `scqubits-4.1.0/scqubits/testing.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/conftest.py` & `scqubits-4.1.0/scqubits/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/cos2phiqubit_1.hdf5` & `scqubits-4.1.0/scqubits/tests/data/cos2phiqubit_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/cos2phiqubit_2.hdf5` & `scqubits-4.1.0/scqubits/tests/data/cos2phiqubit_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/cos2phiqubit_4.hdf5` & `scqubits-4.1.0/scqubits/tests/data/cos2phiqubit_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/cos2phiqubit_5.hdf5` & `scqubits-4.1.0/scqubits/tests/data/cos2phiqubit_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fluxonium_1.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fluxonium_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fluxonium_2.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fluxonium_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fluxonium_4.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fluxonium_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fluxonium_5.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fluxonium_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fluxqubit_1.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fluxqubit_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fluxqubit_2.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fluxqubit_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fluxqubit_4.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fluxqubit_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fluxqubit_5.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fluxqubit_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fullzeropi_1.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fullzeropi_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/fullzeropi_2.hdf5` & `scqubits-4.1.0/scqubits/tests/data/fullzeropi_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/snailmon_1.hdf5` & `scqubits-4.1.0/scqubits/tests/data/snailmon_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/snailmon_2.hdf5` & `scqubits-4.1.0/scqubits/tests/data/snailmon_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/snailmon_4.hdf5` & `scqubits-4.1.0/scqubits/tests/data/snailmon_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/snailmon_5.hdf5` & `scqubits-4.1.0/scqubits/tests/data/snailmon_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/transmon_1.hdf5` & `scqubits-4.1.0/scqubits/tests/data/transmon_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/transmon_2.hdf5` & `scqubits-4.1.0/scqubits/tests/data/transmon_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/transmon_4.hdf5` & `scqubits-4.1.0/scqubits/tests/data/transmon_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/transmon_5.hdf5` & `scqubits-4.1.0/scqubits/tests/data/transmon_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/zeropi-test.hdf5` & `scqubits-4.1.0/scqubits/tests/data/zeropi-test.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/zeropi_1.hdf5` & `scqubits-4.1.0/scqubits/tests/data/zeropi_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/zeropi_2.hdf5` & `scqubits-4.1.0/scqubits/tests/data/zeropi_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/zeropi_4.hdf5` & `scqubits-4.1.0/scqubits/tests/data/zeropi_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/zeropi_5.hdf5` & `scqubits-4.1.0/scqubits/tests/data/zeropi_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/data/zpifull-test.hdf5` & `scqubits-4.1.0/scqubits/tests/data/zpifull-test.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_centraldispatch.py` & `scqubits-4.1.0/scqubits/tests/test_centraldispatch.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_circuit.py` & `scqubits-4.1.0/scqubits/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_circuit_plot.py` & `scqubits-4.1.0/scqubits/tests/test_circuit_plot.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_cos2phiqubit.py` & `scqubits-4.1.0/scqubits/tests/test_cos2phiqubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_explorer.py` & `scqubits-4.1.0/scqubits/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_fluxonium.py` & `scqubits-4.1.0/scqubits/tests/test_fluxonium.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_fluxqubit.py` & `scqubits-4.1.0/scqubits/tests/test_fluxqubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_fullzeropi.py` & `scqubits-4.1.0/scqubits/tests/test_fullzeropi.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_gui.py` & `scqubits-4.1.0/scqubits/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_hilbertspace.py` & `scqubits-4.1.0/scqubits/tests/test_hilbertspace.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_namedslotsndarray.py` & `scqubits-4.1.0/scqubits/tests/test_namedslotsndarray.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_noise.py` & `scqubits-4.1.0/scqubits/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_parameters.py` & `scqubits-4.1.0/scqubits/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_parametersweep.py` & `scqubits-4.1.0/scqubits/tests/test_parametersweep.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_spectrumlookup.py` & `scqubits-4.1.0/scqubits/tests/test_spectrumlookup.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_transmon.py` & `scqubits-4.1.0/scqubits/tests/test_transmon.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_units.py` & `scqubits-4.1.0/scqubits/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/tests/test_zeropi.py` & `scqubits-4.1.0/scqubits/tests/test_zeropi.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/__init__.py` & `scqubits-4.1.0/scqubits/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/gui.py` & `scqubits-4.1.0/scqubits/ui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         "info_panel",
         "literature_params",
         "link_HTML",
     ]
 
     @utils.Required(ipyvuetify=_HAS_IPYVUETIFY, IPython=_HAS_IPYTHON)
     def __init__(self):
-        utils.check_matplotlib_compatibility()
 
         # scq.settings.PROGRESSBAR_DISABLED = False
         scq.settings.T1_DEFAULT_WARNING = False
 
         self.plot_renewal_requested = True
 
         self.active_defaults: Dict[str, Any] = {}
```

### Comparing `scqubits-4.0.0/scqubits/ui/gui_custom_widgets.py` & `scqubits-4.1.0/scqubits/ui/gui_custom_widgets.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/gui_defaults.py` & `scqubits-4.1.0/scqubits/ui/gui_defaults.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/gui_navbar.py` & `scqubits-4.1.0/scqubits/ui/gui_navbar.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/gui_setup.py` & `scqubits-4.1.0/scqubits/ui/gui_setup.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/hspace_widget.py` & `scqubits-4.1.0/scqubits/ui/hspace_widget.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/icons/En.png` & `scqubits-4.1.0/scqubits/ui/icons/En.png`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/icons/Me.png` & `scqubits-4.1.0/scqubits/ui/icons/Me.png`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/icons/MeS.png` & `scqubits-4.1.0/scqubits/ui/icons/MeS.png`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/icons/T1.png` & `scqubits-4.1.0/scqubits/ui/icons/T1.png`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/icons/psi.png` & `scqubits-4.1.0/scqubits/ui/icons/psi.png`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/icons/scq-logo.png` & `scqubits-4.1.0/scqubits/ui/icons/scq-logo.png`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/ui/qubit_widget.py` & `scqubits-4.1.0/scqubits/ui/qubit_widget.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/utils/__init__.py` & `scqubits-4.1.0/scqubits/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/utils/cpu_switch.py` & `scqubits-4.1.0/scqubits/utils/cpu_switch.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/utils/misc.py` & `scqubits-4.1.0/scqubits/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import ast
 import functools
 import platform
 import warnings
 
 import inspect
 from collections.abc import Sequence
-from distutils.version import StrictVersion
 from io import StringIO
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import matplotlib
 import numpy as np
 import qutip as qt
 import scipy as sp
@@ -480,24 +479,14 @@
     Returns
     -------
     The number of lists in the list
     """
     return sum([1 for element in list_object if type(element) == list])
 
 
-def check_matplotlib_compatibility():
-    if _HAS_WIDGET_BACKEND and StrictVersion(matplotlib.__version__) < StrictVersion(
-        "3.5.1"
-    ):
-        warnings.warn(
-            "The widget backend requires Matplotlib >=3.5.1 for proper functioning",
-            UserWarning,
-        )
-
-
 def inspect_public_API(
     module: Any,
     public_names: List[str] = [],
     private_names: List[str] = [],
 ) -> List[str]:
     """
     Find all public names in a module.
```

### Comparing `scqubits-4.0.0/scqubits/utils/plot_defaults.py` & `scqubits-4.1.0/scqubits/utils/plot_defaults.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/utils/plot_utils.py` & `scqubits-4.1.0/scqubits/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/utils/plotting.py` & `scqubits-4.1.0/scqubits/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/utils/spectrum_utils.py` & `scqubits-4.1.0/scqubits/utils/spectrum_utils.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits/utils/typedefs.py` & `scqubits-4.1.0/scqubits/utils/typedefs.py`

 * *Files identical despite different names*

### Comparing `scqubits-4.0.0/scqubits.egg-info/SOURCES.txt` & `scqubits-4.1.0/scqubits.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 optional-requirements.txt
 requirements.txt
 setup.py
 scqubits/__init__.py
+scqubits/py.typed
+scqubits/qubit_base_OLD.py
 scqubits/settings.py
 scqubits/testing.py
 scqubits/version.py
 scqubits.egg-info/PKG-INFO
 scqubits.egg-info/SOURCES.txt
 scqubits.egg-info/dependency_links.txt
 scqubits.egg-info/not-zip-safe
```

### Comparing `scqubits-4.0.0/setup.py` & `scqubits-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 """
 
 
 EXTRA_KWARGS = {}
 
 # version information about scqubits goes here
 MAJOR = 4
-MINOR = 0
+MINOR = 1
 MICRO = 0
 ISRELEASED = True
 
 VERSION = "%d.%d.%d" % (MAJOR, MINOR, MICRO)
 
 CURRENT_DIR = os.path.dirname(os.path.abspath(__file__))
 with open(os.path.join(CURRENT_DIR, "requirements.txt")) as requirements:
```

