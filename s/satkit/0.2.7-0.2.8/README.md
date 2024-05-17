# Comparing `tmp/satkit-0.2.7.tar.gz` & `tmp/satkit-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satkit-0.2.7.tar", last modified: Thu Apr 25 02:29:08 2024, max compression
+gzip compressed data, was "satkit-0.2.8.tar", last modified: Fri May 17 01:30:44 2024, max compression
```

## Comparing `satkit-0.2.7.tar` & `satkit-0.2.8.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.551812 satkit-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-25 02:24:53.000000 satkit-0.2.7/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 02:24:53.000000 satkit-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 02:24:53.000000 satkit-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-25 02:29:08.551812 satkit-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-25 02:24:53.000000 satkit-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-25 02:24:53.000000 satkit-0.2.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.531812 satkit-0.2.7/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.531812 satkit-0.2.7/python/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.535812 satkit-0.2.7/python/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-04-25 02:24:53.000000 satkit-0.2.7/python/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.535812 satkit-0.2.7/python/satkit/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.535812 satkit-0.2.7/python/satkit/astro-data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/astro-data/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/density.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/frametransform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/jplephem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/moon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    41215 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/satkit.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/satprop.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/sun.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-25 02:24:53.000000 satkit-0.2.7/python/satkit/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.551812 satkit-0.2.7/python/satkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-25 02:29:08.000000 satkit-0.2.7/python/satkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-25 02:29:08.000000 satkit-0.2.7/python/satkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:29:08.000000 satkit-0.2.7/python/satkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 02:29:08.000000 satkit-0.2.7/python/satkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 02:29:08.000000 satkit-0.2.7/python/satkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.539812 satkit-0.2.7/python/test/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-25 02:24:53.000000 satkit-0.2.7/python/test/download_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-25 02:24:53.000000 satkit-0.2.7/python/test/download_from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-25 02:24:53.000000 satkit-0.2.7/python/test/download_testvecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-25 02:24:53.000000 satkit-0.2.7/python/test/orbitprop_gps_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-25 02:24:53.000000 satkit-0.2.7/python/test/sp3file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25177 2024-04-25 02:24:53.000000 satkit-0.2.7/python/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:29:08.551812 satkit-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.539812 satkit-0.2.7/src/
--rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-04-25 02:24:53.000000 satkit-0.2.7/src/astrotime.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-25 02:24:53.000000 satkit-0.2.7/src/consts.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-25 02:24:53.000000 satkit-0.2.7/src/duration.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-25 02:24:53.000000 satkit-0.2.7/src/earth_orientation_params.rs
--rw-r--r--   0 runner    (1001) docker     (127)    22770 2024-04-25 02:24:53.000000 satkit-0.2.7/src/earthgravity.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.539812 satkit-0.2.7/src/frametransform/
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-25 02:24:53.000000 satkit-0.2.7/src/frametransform/ierstable.rs
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-04-25 02:24:53.000000 satkit-0.2.7/src/frametransform/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-25 02:24:53.000000 satkit-0.2.7/src/frametransform/qcirs2gcrs.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21772 2024-04-25 02:24:53.000000 satkit-0.2.7/src/itrfcoord.rs
--rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-04-25 02:24:53.000000 satkit-0.2.7/src/jplephem.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-25 02:24:53.000000 satkit-0.2.7/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.539812 satkit-0.2.7/src/lpephem/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 02:24:53.000000 satkit-0.2.7/src/lpephem/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-25 02:24:53.000000 satkit-0.2.7/src/lpephem/moon.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-25 02:24:53.000000 satkit-0.2.7/src/lpephem/sun.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-25 02:24:53.000000 satkit-0.2.7/src/nrlmsise.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.543812 satkit-0.2.7/src/ode/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/harmonic_oscillator.rs
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/nalgebra.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rk_adaptive.rs
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rk_adaptive_settings.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rk_explicit.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkf45.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkts54.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkv65.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkv65_table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkv87.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkv87_table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkv98.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkv98_nointerp.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkv98_nointerp_table.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/rkv98_table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-25 02:24:53.000000 satkit-0.2.7/src/ode/types.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.543812 satkit-0.2.7/src/orbitprop/
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-25 02:24:53.000000 satkit-0.2.7/src/orbitprop/drag.rs
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-25 02:24:53.000000 satkit-0.2.7/src/orbitprop/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-25 02:24:53.000000 satkit-0.2.7/src/orbitprop/point_gravity.rs
--rw-r--r--   0 runner    (1001) docker     (127)    27160 2024-04-25 02:24:53.000000 satkit-0.2.7/src/orbitprop/propagator.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-25 02:24:53.000000 satkit-0.2.7/src/orbitprop/satproperties.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-25 02:24:53.000000 satkit-0.2.7/src/orbitprop/satstate.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-25 02:24:53.000000 satkit-0.2.7/src/orbitprop/settings.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.547812 satkit-0.2.7/src/pybindings/
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/mod_utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pyastrotime.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pyconsts.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pydensity.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pyduration.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pyframetransform.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pygravity.rs
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pyitrfcoord.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pyjplephem.rs
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pylpephem_moon.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pylpephem_sun.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pynrlmsise.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pypropagate.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pypropsettings.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pyquaternion.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pysatproperties.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pysatstate.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pysgp4.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pysolarsystem.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pytle.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-25 02:24:53.000000 satkit-0.2.7/src/pybindings/pyutils.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.551812 satkit-0.2.7/src/sgp4/
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/dpper.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/dscom.rs
--rw-r--r--   0 runner    (1001) docker     (127)    12980 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/dsinit.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/dspace.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/getgravconst.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/initl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/satrec.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/sgp4.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15524 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/sgp4_lowlevel.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21970 2024-04-25 02:24:53.000000 satkit-0.2.7/src/sgp4/sgp4init.rs
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-25 02:24:53.000000 satkit-0.2.7/src/solarsystem.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-25 02:24:53.000000 satkit-0.2.7/src/spaceweather.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15457 2024-04-25 02:24:53.000000 satkit-0.2.7/src/tle.rs
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 02:24:53.000000 satkit-0.2.7/src/types.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:29:08.551812 satkit-0.2.7/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-25 02:24:53.000000 satkit-0.2.7/src/utils/datadir.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-25 02:24:53.000000 satkit-0.2.7/src/utils/download.rs
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 02:24:53.000000 satkit-0.2.7/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-25 02:24:53.000000 satkit-0.2.7/src/utils/skerror.rs
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-25 02:24:53.000000 satkit-0.2.7/src/utils/test.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-25 02:24:53.000000 satkit-0.2.7/src/utils/update_data.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.090150 satkit-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-17 01:26:14.000000 satkit-0.2.8/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-17 01:26:14.000000 satkit-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-17 01:26:14.000000 satkit-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-17 01:30:44.086150 satkit-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-17 01:26:14.000000 satkit-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-17 01:26:14.000000 satkit-0.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.066150 satkit-0.2.8/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.066150 satkit-0.2.8/python/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.070150 satkit-0.2.8/python/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-05-17 01:26:14.000000 satkit-0.2.8/python/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.070150 satkit-0.2.8/python/satkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/density.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/frametransform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/jplephem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/moon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42955 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/satkit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/satprop.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/sun.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-17 01:26:14.000000 satkit-0.2.8/python/satkit/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.086150 satkit-0.2.8/python/satkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-17 01:30:44.000000 satkit-0.2.8/python/satkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-17 01:30:44.000000 satkit-0.2.8/python/satkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:30:44.000000 satkit-0.2.8/python/satkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 01:30:44.000000 satkit-0.2.8/python/satkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 01:30:44.000000 satkit-0.2.8/python/satkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.074150 satkit-0.2.8/python/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-17 01:26:14.000000 satkit-0.2.8/python/test/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 01:26:14.000000 satkit-0.2.8/python/test/download_from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-17 01:26:14.000000 satkit-0.2.8/python/test/download_testvecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-17 01:26:14.000000 satkit-0.2.8/python/test/orbitprop_gps_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-17 01:26:14.000000 satkit-0.2.8/python/test/sp3file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26541 2024-05-17 01:26:14.000000 satkit-0.2.8/python/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:30:44.090150 satkit-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.074150 satkit-0.2.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-05-17 01:26:14.000000 satkit-0.2.8/src/astrotime.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-17 01:26:14.000000 satkit-0.2.8/src/consts.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-17 01:26:14.000000 satkit-0.2.8/src/duration.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-17 01:26:14.000000 satkit-0.2.8/src/earth_orientation_params.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    22770 2024-05-17 01:26:14.000000 satkit-0.2.8/src/earthgravity.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.078150 satkit-0.2.8/src/frametransform/
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-17 01:26:14.000000 satkit-0.2.8/src/frametransform/ierstable.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-05-17 01:26:14.000000 satkit-0.2.8/src/frametransform/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-17 01:26:14.000000 satkit-0.2.8/src/frametransform/qcirs2gcrs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21772 2024-05-17 01:26:14.000000 satkit-0.2.8/src/itrfcoord.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-05-17 01:26:14.000000 satkit-0.2.8/src/jplephem.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-17 01:26:14.000000 satkit-0.2.8/src/kepler.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-17 01:26:14.000000 satkit-0.2.8/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.078150 satkit-0.2.8/src/lpephem/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 01:26:14.000000 satkit-0.2.8/src/lpephem/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-17 01:26:14.000000 satkit-0.2.8/src/lpephem/moon.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15305 2024-05-17 01:26:14.000000 satkit-0.2.8/src/lpephem/planets.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-05-17 01:26:14.000000 satkit-0.2.8/src/lpephem/sun.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-17 01:26:14.000000 satkit-0.2.8/src/nrlmsise.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.078150 satkit-0.2.8/src/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/harmonic_oscillator.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/nalgebra.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rk_adaptive.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rk_adaptive_settings.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rk_explicit.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkf45.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkts54.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkv65.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkv65_table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkv87.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkv87_table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkv98.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkv98_nointerp.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkv98_nointerp_table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/rkv98_table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-17 01:26:14.000000 satkit-0.2.8/src/ode/types.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.082150 satkit-0.2.8/src/orbitprop/
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-17 01:26:14.000000 satkit-0.2.8/src/orbitprop/drag.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-17 01:26:14.000000 satkit-0.2.8/src/orbitprop/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 01:26:14.000000 satkit-0.2.8/src/orbitprop/point_gravity.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    27100 2024-05-17 01:26:14.000000 satkit-0.2.8/src/orbitprop/propagator.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-17 01:26:14.000000 satkit-0.2.8/src/orbitprop/satproperties.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-17 01:26:14.000000 satkit-0.2.8/src/orbitprop/satstate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-17 01:26:14.000000 satkit-0.2.8/src/orbitprop/settings.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.086150 satkit-0.2.8/src/pybindings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/mod_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pyastrotime.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pyconsts.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pydensity.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pyduration.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pyframetransform.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pygravity.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pyitrfcoord.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pyjplephem.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pykepler.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pylpephem_moon.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pylpephem_sun.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pynrlmsise.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pypropagate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pypropsettings.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pyquaternion.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pysatproperties.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pysatstate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pysgp4.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pysolarsystem.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pytle.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-17 01:26:14.000000 satkit-0.2.8/src/pybindings/pyutils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.086150 satkit-0.2.8/src/sgp4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/dpper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/dscom.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    12980 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/dsinit.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/dspace.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/getgravconst.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/initl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/satrec.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/sgp4.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15524 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/sgp4_lowlevel.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21970 2024-05-17 01:26:14.000000 satkit-0.2.8/src/sgp4/sgp4init.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-17 01:26:14.000000 satkit-0.2.8/src/solarsystem.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-17 01:26:14.000000 satkit-0.2.8/src/spaceweather.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-17 01:26:14.000000 satkit-0.2.8/src/tle.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 01:26:14.000000 satkit-0.2.8/src/types.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:30:44.086150 satkit-0.2.8/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-17 01:26:14.000000 satkit-0.2.8/src/utils/datadir.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-17 01:26:14.000000 satkit-0.2.8/src/utils/download.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-17 01:26:14.000000 satkit-0.2.8/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-17 01:26:14.000000 satkit-0.2.8/src/utils/skerror.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-17 01:26:14.000000 satkit-0.2.8/src/utils/test.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-17 01:26:14.000000 satkit-0.2.8/src/utils/update_data.rs
```

### Comparing `satkit-0.2.7/Cargo.toml` & `satkit-0.2.8/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "satkit"
-version = "0.2.7"
+version = "0.2.8"
 edition = "2021"
 description = "Satellite Toolkit"
 readme = "README.md"
 licence = "MIT"
 license-file = "LICENSE"
 homepage = "https://github.com/ssmichael1/satkit"
 repository = "https://github.com/ssmichael1/satkit"
```

### Comparing `satkit-0.2.7/LICENSE` & `satkit-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/PKG-INFO` & `satkit-0.2.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satkit
-Version: 0.2.7
+Version: 0.2.8
 Summary: Satellite Orbital Dynamics Toolkit
 Author-email: Steven Michael <ssmichael@gmail.com>
 Maintainer-email: Steven Michael <ssmichael@gmail.com>
 Keywords: satellite,orbit,astrodynamics,SGP4,TLE,JPL,Ephemeris
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -17,14 +17,15 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 
 # Satellite Toolkit with Rust
 
 An accurate, high-performance satellite orbital kinematics toolkit, written in Rust with a sensible interface.
 <br/>
+Also includes python bindings for *all* functions via via [pyo3](https://pyo3.rs/)
 
 ### Github
 
 ![Build Passing?](https://github.com/ssmichael1/satkit/actions/workflows/build.yml/badge.svg)
 ![Wheel Passing?](https://github.com/ssmichael1/satkit/actions/workflows/wheels.yml/badge.svg)
 ![GitHub License](https://img.shields.io/github/license/ssmichael1/satkit)
 
@@ -44,15 +45,15 @@
 ![Read the Docs](https://img.shields.io/readthedocs/satellite-toolkit)
 
 ## Language Bindings
 
 - **Native Rust** bindings
 - **Python bindings** for compiled rust code ... speed of Rust with convenience of Python<br/>
   Install with `pip install satkit`<br/>
-  PyPi includes binaries for windows, macos (Intel & arm), and linux
+  PyPi includes binary packages for windows, macos (Intel & ARM), and linux.  Python documentation is at: <https://satellite-toolkit.readthedocs.io/latest/>
 
 ## Features
 
 - High-precision coordinate transforms between:
   - International Terrestrial Reference Frame (ITRF)
   - Geocentric Celestial Reference Frame (GCRF) using IAU-2000 reduction
   - True-Equinox Mean Equator (TEME) frame used in SGP4 propagation of TLEs
```

### Comparing `satkit-0.2.7/README.md` & `satkit-0.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Satellite Toolkit with Rust
 
 An accurate, high-performance satellite orbital kinematics toolkit, written in Rust with a sensible interface.
 <br/>
+Also includes python bindings for *all* functions via via [pyo3](https://pyo3.rs/)
 
 ### Github
 
 ![Build Passing?](https://github.com/ssmichael1/satkit/actions/workflows/build.yml/badge.svg)
 ![Wheel Passing?](https://github.com/ssmichael1/satkit/actions/workflows/wheels.yml/badge.svg)
 ![GitHub License](https://img.shields.io/github/license/ssmichael1/satkit)
 
@@ -25,15 +26,15 @@
 ![Read the Docs](https://img.shields.io/readthedocs/satellite-toolkit)
 
 ## Language Bindings
 
 - **Native Rust** bindings
 - **Python bindings** for compiled rust code ... speed of Rust with convenience of Python<br/>
   Install with `pip install satkit`<br/>
-  PyPi includes binaries for windows, macos (Intel & arm), and linux
+  PyPi includes binary packages for windows, macos (Intel & ARM), and linux.  Python documentation is at: <https://satellite-toolkit.readthedocs.io/latest/>
 
 ## Features
 
 - High-precision coordinate transforms between:
   - International Terrestrial Reference Frame (ITRF)
   - Geocentric Celestial Reference Frame (GCRF) using IAU-2000 reduction
   - True-Equinox Mean Equator (TEME) frame used in SGP4 propagation of TLEs
```

### Comparing `satkit-0.2.7/pyproject.toml` & `satkit-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-rust"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "satkit"
-version = "0.2.7"
+version = "0.2.8"
 dependencies = ["numpy>=1.20.0"]
 requires-python = ">= 3.8"
 authors = [{ name = "Steven Michael", email = "ssmichael@gmail.com" }]
 maintainers = [{ name = "Steven Michael", email = "ssmichael@gmail.com" }]
 readme = "README.md"
 description = "Satellite Orbital Dynamics Toolkit"
 keywords = [
```

### Comparing `satkit-0.2.7/python/docs/source/conf.py` & `satkit-0.2.8/python/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/satkit/density.pyi` & `satkit-0.2.8/python/satkit/density.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/satkit/frametransform.pyi` & `satkit-0.2.8/python/satkit/frametransform.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/satkit/jplephem.pyi` & `satkit-0.2.8/python/satkit/jplephem.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/satkit/moon.pyi` & `satkit-0.2.8/python/satkit/moon.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/satkit/satkit.pyi` & `satkit-0.2.8/python/satkit/satkit.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1046,14 +1046,61 @@
             frac (float): fractional amount of interpolation, in range [0,1]
             epsilon (float, optional): Value below which the sin of the angle separating both quaternions must be to return an error. Default is 1.0e-6
 
         Returns:
             quaternion: Quaternion representing interpolation between self and other
         """
 
+class kepler:
+    """ Represent Keplerian element sets and convert between cartesian
+    
+    
+    Notes:
+        * This class is used to represent Keplerian elements and convert between Cartesian coordinates
+        * The class uses the semi-major axis (a), not the semiparameter
+        * All angle units are radians
+        * All length units are meters
+        * All velocity units are meters / second
+    """
+
+    def __init__(self, *args):
+        """Create Keplerian element set object from input elements
+
+        # Args:
+            a (float) : Semi-major axis, meters
+            e (float) : Eccentricity, unitless
+            i (float) : Inclination, radians
+            raan (float) : Right ascension of ascending node, radians
+            argp (float) : Argument of perigee, radians
+            nu (float) : True anomaly, radians
+
+        # Returns:
+            satkit.kepler: Keplerian element set object
+        """
+
+    def to_pv(self) -> typing.Tuple[npt.ArrayLike[np.float64], npt.ArrayLike[np.float64]]:
+        """Convert Keplerian element set to position and velocity vectors
+
+        Returns:
+            tuple[npt.ArrayLike[np.float64], npt.ArrayLike[np.float64]]: Tuple with two elements representing the position and velocity vectors
+        """
+
+    def from_pv(
+        pos: npt.ArrayLike[np.float64], vel: npt.ArrayLike[np.float64]
+    ) -> kepler:
+        """Create Keplerian element set from input position and velocity vectors
+
+        Args:
+            pos (npt.ArrayLike[np.float64]): 3-element array representing position vector
+            vel (npt.ArrayLike[np.float64]): 3-element array representing velocity vector
+
+        Returns:
+            satkit.kepler: Keplerian element set object
+        """
+
 class itrfcoord:
     """ Representation of a coordinate in the International Terrestrial Reference Frame (ITRF)
 
     Notes:
         * This coordinate object can be created from and also output to Geodetic coordinates (latitude, longitude, height above ellipsoid).
         * Functions are also available to provide rotation quaternions to the East-North-Up frame and North-East-Down frame at this coordinate
```

### Comparing `satkit-0.2.7/python/satkit/satprop.pyi` & `satkit-0.2.8/python/satkit/satprop.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/satkit/sun.pyi` & `satkit-0.2.8/python/satkit/sun.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/satkit/utils.pyi` & `satkit-0.2.8/python/satkit/utils.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/satkit.egg-info/PKG-INFO` & `satkit-0.2.8/python/satkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satkit
-Version: 0.2.7
+Version: 0.2.8
 Summary: Satellite Orbital Dynamics Toolkit
 Author-email: Steven Michael <ssmichael@gmail.com>
 Maintainer-email: Steven Michael <ssmichael@gmail.com>
 Keywords: satellite,orbit,astrodynamics,SGP4,TLE,JPL,Ephemeris
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -17,14 +17,15 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 
 # Satellite Toolkit with Rust
 
 An accurate, high-performance satellite orbital kinematics toolkit, written in Rust with a sensible interface.
 <br/>
+Also includes python bindings for *all* functions via via [pyo3](https://pyo3.rs/)
 
 ### Github
 
 ![Build Passing?](https://github.com/ssmichael1/satkit/actions/workflows/build.yml/badge.svg)
 ![Wheel Passing?](https://github.com/ssmichael1/satkit/actions/workflows/wheels.yml/badge.svg)
 ![GitHub License](https://img.shields.io/github/license/ssmichael1/satkit)
 
@@ -44,15 +45,15 @@
 ![Read the Docs](https://img.shields.io/readthedocs/satellite-toolkit)
 
 ## Language Bindings
 
 - **Native Rust** bindings
 - **Python bindings** for compiled rust code ... speed of Rust with convenience of Python<br/>
   Install with `pip install satkit`<br/>
-  PyPi includes binaries for windows, macos (Intel & arm), and linux
+  PyPi includes binary packages for windows, macos (Intel & ARM), and linux.  Python documentation is at: <https://satellite-toolkit.readthedocs.io/latest/>
 
 ## Features
 
 - High-precision coordinate transforms between:
   - International Terrestrial Reference Frame (ITRF)
   - Geocentric Celestial Reference Frame (GCRF) using IAU-2000 reduction
   - True-Equinox Mean Equator (TEME) frame used in SGP4 propagation of TLEs
```

### Comparing `satkit-0.2.7/python/satkit.egg-info/SOURCES.txt` & `satkit-0.2.8/python/satkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,39 +16,40 @@
 python/satkit/sun.pyi
 python/satkit/utils.pyi
 python/satkit.egg-info/PKG-INFO
 python/satkit.egg-info/SOURCES.txt
 python/satkit.egg-info/dependency_links.txt
 python/satkit.egg-info/requires.txt
 python/satkit.egg-info/top_level.txt
-python/satkit/astro-data/py.typed
 python/test/download_data.py
 python/test/download_from_json.py
 python/test/download_testvecs.py
 python/test/orbitprop_gps_fit.py
 python/test/sp3file.py
 python/test/test.py
 src/astrotime.rs
 src/consts.rs
 src/duration.rs
 src/earth_orientation_params.rs
 src/earthgravity.rs
 src/itrfcoord.rs
 src/jplephem.rs
+src/kepler.rs
 src/lib.rs
 src/nrlmsise.rs
 src/solarsystem.rs
 src/spaceweather.rs
 src/tle.rs
 src/types.rs
 src/frametransform/ierstable.rs
 src/frametransform/mod.rs
 src/frametransform/qcirs2gcrs.rs
 src/lpephem/mod.rs
 src/lpephem/moon.rs
+src/lpephem/planets.rs
 src/lpephem/sun.rs
 src/ode/harmonic_oscillator.rs
 src/ode/mod.rs
 src/ode/nalgebra.rs
 src/ode/rk_adaptive.rs
 src/ode/rk_adaptive_settings.rs
 src/ode/rk_explicit.rs
@@ -76,14 +77,15 @@
 src/pybindings/pyconsts.rs
 src/pybindings/pydensity.rs
 src/pybindings/pyduration.rs
 src/pybindings/pyframetransform.rs
 src/pybindings/pygravity.rs
 src/pybindings/pyitrfcoord.rs
 src/pybindings/pyjplephem.rs
+src/pybindings/pykepler.rs
 src/pybindings/pylpephem_moon.rs
 src/pybindings/pylpephem_sun.rs
 src/pybindings/pynrlmsise.rs
 src/pybindings/pypropagate.rs
 src/pybindings/pypropsettings.rs
 src/pybindings/pyquaternion.rs
 src/pybindings/pysatproperties.rs
```

### Comparing `satkit-0.2.7/python/test/download_data.py` & `satkit-0.2.8/python/test/download_data.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/test/download_from_json.py` & `satkit-0.2.8/python/test/download_from_json.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/test/download_testvecs.py` & `satkit-0.2.8/python/test/download_testvecs.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/test/sp3file.py` & `satkit-0.2.8/python/test/sp3file.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/python/test/test.py` & `satkit-0.2.8/python/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,52 @@
         assert year == 2021
         assert mon == 1
         assert day == 1
         assert hour == 0
         assert minute == 0
         assert sec == 0
 
+class TestKepler:
+    def test_kepler_from_pv(self):
+        """
+        Test creation of Kepler elements from position and velocity
+        """
+    
+        # Test case from Vallado, example 2-6
+        r = np.array([6524.834, 6862.875, 6448.296])*1.0e3
+        v = np.array([4.901327, 5.533756, -1.976341])*1.0e3
+        kep = sk.kepler.from_pv(r, v)
+        rad2deg = 180.0/m.pi
+        print(kep)
+        assert kep.a == pytest.approx(36127343, 1.0e-3)
+        assert kep.eccen == pytest.approx(0.83285, 1.0e-5)
+        assert kep.inclination*rad2deg == pytest.approx(87.87, 1.0e-3)
+        assert kep.raan*rad2deg == pytest.approx(227.89, 1.0e-3)
+        assert kep.w*rad2deg == pytest.approx(53.38, 1.0e-3)
+        assert kep.nu*rad2deg == pytest.approx(92.335, 1.0e-3)
+
+    def test_kepler_to_pv(self):
+        """
+        Test conversion of Kepler elements to position and velocity
+        """
+        p = 11067790
+        eccen = 0.83285
+        incl = 87.87*m.pi/180
+        raan = 227.89*m.pi/180
+        w = 53.38*m.pi/180
+        nu = 92.335*m.pi/180
+
+        a = p/(1-eccen**2)
+        kep = sk.kepler(a, eccen, incl, raan, w, nu)
+        pos, vel = kep.to_pv()
+        assert pos == pytest.approx(np.array([6525.368, 6861.532, 6449.119])*1.0e3, 1.0e-3)
+        assert vel == pytest.approx(np.array([4.902279, 5.533140, -1.975710])*1.0e3, 1.0e-3)
+
+
+
 class TestJPLEphem:
     def test_jplephem_testvecs(self):
         """
         Test JPL ephemeris against test vectors provided by JPL
         """
 
         # File contains test calculation vectors provided by NASA
```

### Comparing `satkit-0.2.7/src/astrotime.rs` & `satkit-0.2.8/src/astrotime.rs`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,15 @@
     /// * `year` - the year
     /// * `month` - the month, 1 based (1=January, 2=February, ...)
     /// * `day` - Day of month, starting from 1
     ///
     /// # Returns
     ///
     /// * AstroTime Object
-    pub fn from_date(year: u32, month: u32, day: u32) -> AstroTime {
+    pub fn from_date(year: i32, month: u32, day: u32) -> AstroTime {
         AstroTime::from_mjd(date2mjd_utc(year, month, day) as f64, Scale::UTC)
     }
 
     /// Convert AstroTime to UTC Gregorian date
     ///
     /// # Returns
     ///
@@ -496,15 +496,15 @@
     /// * `sec` - Second of minute, including fractions for subsecond, in range \[0,1)
     ///
     /// # Return
     ///
     /// * AstroTime object
     #[inline]
     pub fn from_datetime(
-        year: u32,
+        year: i32,
         month: u32,
         day: u32,
         hour: u32,
         min: u32,
         sec: f64,
     ) -> AstroTime {
         AstroTime::from_datetime_with_scale(year, month, day, hour, min, sec, Scale::UTC)
@@ -522,15 +522,15 @@
     /// * `sec` - Second of minute, including fractions for subsecond, in range \[0,1)
     /// * `scale` - Time Scale represented by input time, e.g. UTC, GPS
     ///
     /// # Return
     ///
     /// * AstroTime object
     pub fn from_datetime_with_scale(
-        year: u32,
+        year: i32,
         month: u32,
         day: u32,
         hour: u32,
         min: u32,
         sec: f64,
         scale: Scale,
     ) -> AstroTime {
@@ -645,15 +645,15 @@
     let day: i32 = (h % S) / U + 1;
     let month: i32 = ((h / S + M) % N) + 1;
     let year: i32 = e / P - Y + (N + M - month) / N;
 
     (year as u32, month as u32, day as u32)
 }
 
-fn date2mjd_utc(year: u32, month: u32, day: u32) -> i32 {
+fn date2mjd_utc(year: i32, month: u32, day: u32) -> i32 {
     // Chapter 15 "Calendars" section 15.11.3 of the
     // Explanatory Suppliment to the Astronomical Almanac
     // Algorithm 3
     const Y: i32 = 4716;
     const J: i32 = 1401;
     const M: i32 = 2;
     const N: i32 = 12;
```

### Comparing `satkit-0.2.7/src/consts.rs` & `satkit-0.2.8/src/consts.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/duration.rs` & `satkit-0.2.8/src/duration.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/earth_orientation_params.rs` & `satkit-0.2.8/src/earth_orientation_params.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/earthgravity.rs` & `satkit-0.2.8/src/earthgravity.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/frametransform/ierstable.rs` & `satkit-0.2.8/src/frametransform/ierstable.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/frametransform/mod.rs` & `satkit-0.2.8/src/frametransform/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 /// * For a reference, see "Eplanatory Supplement to the
 /// Astronomical Almanac", 2013, Ch. 6
 ///
 pub fn qgcrf2itrf_approx(tm: &AstroTime) -> Quat {
     // Neglecting polar motion
     let qitrf2tod_approx: Quat = qrot_zcoord(-gast(tm));
 
-    qmod2gcrf(tm) * qtod2mod_approx(tm) * qitrf2tod_approx
+    (qmod2gcrf(tm) * qtod2mod_approx(tm) * qitrf2tod_approx).conjugate()
 }
 
 ///
 /// Approximate rotation from
 /// International Terrestrial Reference Frame to
 /// Geocentric Celestrial Reference Frame
 ///
```

### Comparing `satkit-0.2.7/src/frametransform/qcirs2gcrs.rs` & `satkit-0.2.8/src/frametransform/qcirs2gcrs.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/itrfcoord.rs` & `satkit-0.2.8/src/itrfcoord.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/jplephem.rs` & `satkit-0.2.8/src/jplephem.rs`

 * *Files 4% similar despite different names*

```diff
@@ -34,25 +34,25 @@
 
 use super::astrotime::{AstroTime, Scale};
 
 impl TryFrom<i32> for SolarSystem {
     type Error = ();
     fn try_from(v: i32) -> Result<Self, Self::Error> {
         match v {
-            x if x == SolarSystem::MERCURY as i32 => Ok(SolarSystem::MERCURY),
-            x if x == SolarSystem::VENUS as i32 => Ok(SolarSystem::VENUS),
+            x if x == SolarSystem::Mercury as i32 => Ok(SolarSystem::Mercury),
+            x if x == SolarSystem::Venus as i32 => Ok(SolarSystem::Venus),
             x if x == SolarSystem::EMB as i32 => Ok(SolarSystem::EMB),
-            x if x == SolarSystem::MARS as i32 => Ok(SolarSystem::MARS),
-            x if x == SolarSystem::JUPITER as i32 => Ok(SolarSystem::JUPITER),
-            x if x == SolarSystem::SATURN as i32 => Ok(SolarSystem::SATURN),
-            x if x == SolarSystem::URANUS as i32 => Ok(SolarSystem::URANUS),
-            x if x == SolarSystem::NEPTUNE as i32 => Ok(SolarSystem::NEPTUNE),
-            x if x == SolarSystem::PLUTO as i32 => Ok(SolarSystem::PLUTO),
-            x if x == SolarSystem::MOON as i32 => Ok(SolarSystem::MOON),
-            x if x == SolarSystem::SUN as i32 => Ok(SolarSystem::SUN),
+            x if x == SolarSystem::Mars as i32 => Ok(SolarSystem::Mars),
+            x if x == SolarSystem::Jupiter as i32 => Ok(SolarSystem::Jupiter),
+            x if x == SolarSystem::Saturn as i32 => Ok(SolarSystem::Saturn),
+            x if x == SolarSystem::Uranus as i32 => Ok(SolarSystem::Uranus),
+            x if x == SolarSystem::Neptune as i32 => Ok(SolarSystem::Neptune),
+            x if x == SolarSystem::Pluto as i32 => Ok(SolarSystem::Pluto),
+            x if x == SolarSystem::Moon as i32 => Ok(SolarSystem::Moon),
+            x if x == SolarSystem::Sun as i32 => Ok(SolarSystem::Sun),
             _ => Err(()),
         }
     }
 }
 
 #[derive(Debug, Clone)]
 struct InvalidSize;
@@ -126,15 +126,15 @@
     /// use satkit::SolarSystem;
     /// use satkit::AstroTime;
     ///
     /// // Construct time: March 1 2021 12:00pm UTC
     /// let t = AstroTime::from_datetime(2021, 3, 1, 12, 0, 0.0);
     ///
     /// // Find geocentric moon position at this time in the GCRF frame
-    /// let p = jplephem::geocentric_pos(SolarSystem::MOON, &t).unwrap();
+    /// let p = jplephem::geocentric_pos(SolarSystem::Moon, &t).unwrap();
     /// println!("p = {}", p);
     /// ```
     ///
     fn from_file(fname: &str) -> SKResult<JPLEphem> {
         use std::collections::HashMap;
         use std::path::PathBuf;
 
@@ -449,19 +449,19 @@
     ///  * tm - The time at which to return position
     ///
     /// # Return
     ///
     ///    3-vector of cartesian Geocentric position in meters
     ///
     fn geocentric_pos(&self, body: SolarSystem, tm: &AstroTime) -> SKResult<Vec3> {
-        if body == SolarSystem::MOON {
+        if body == SolarSystem::Moon {
             return self.barycentric_pos(body, tm);
         } else {
             let emb: Vec3 = self.barycentric_pos(SolarSystem::EMB, tm)?;
-            let moon: Vec3 = self.barycentric_pos(SolarSystem::MOON, tm)?;
+            let moon: Vec3 = self.barycentric_pos(SolarSystem::Moon, tm)?;
             let b: Vec3 = self.barycentric_pos(body, tm)?;
 
             // Compute the position of the body relative to the Earth-moon
             // barycenter, then "correct" to Earth-center by accounting
             // for moon position and Earth/moon mass ratio
             Ok(b - emb + moon / (1.0 + self.emrat))
         }
@@ -479,19 +479,19 @@
     ///
     ///   * 2-element tuple with following elements:
     ///     * 3-vector of cartesian Geocentric position in meters
     ///     * 3-vector of cartesian Geocentric velocity in meters / second
     ///       Note: velocity is relative to Earth
     ///
     fn geocentric_state(&self, body: SolarSystem, tm: &AstroTime) -> SKResult<(Vec3, Vec3)> {
-        if body == SolarSystem::MOON {
+        if body == SolarSystem::Moon {
             return self.barycentric_state(body, tm);
         } else {
             let emb: (Vec3, Vec3) = self.barycentric_state(SolarSystem::EMB, tm)?;
-            let moon: (Vec3, Vec3) = self.barycentric_state(SolarSystem::MOON, tm)?;
+            let moon: (Vec3, Vec3) = self.barycentric_state(SolarSystem::Moon, tm)?;
             let b: (Vec3, Vec3) = self.barycentric_state(body, tm)?;
 
             // Compute the position of the body relative to the Earth-moon
             // barycenter, then "correct" to Earth-center by accounting
             // for moon position and Earth/moon mass ratio
             Ok((
                 b.0 - emb.0 + moon.0 / (1.0 + self.emrat),
@@ -609,15 +609,15 @@
     #[test]
     fn load_test() {
         //let tm = &AstroTime::from_date(2010, 3, 1);
         let jpl = jplephem_singleton().as_ref().unwrap();
 
         let tm = AstroTime::from_jd(2451545.0, Scale::TT);
         //let tm = &AstroTime::from_jd(2451545.0, Scale::UTC);
-        let (_, _): (Vec3, Vec3) = jpl.geocentric_state(SolarSystem::MOON, &tm).unwrap();
+        let (_, _): (Vec3, Vec3) = jpl.geocentric_state(SolarSystem::Moon, &tm).unwrap();
         println!("au = {:.20}", jpl._au);
     }
 
     /// Load the test vectors that come with the JPL ephemeris files
     /// and compare calculated positions to test vectors.
     #[test]
     fn testvecs() {
@@ -668,25 +668,25 @@
                 // in test vectors, index 3 is not EMB, but rather Earth
                 // (this took me a long time to figure out...)
                 if tar == 3 {
                     tpos = Vec3::zeros();
                     let (_mpos, mvel): (Vec3, Vec3) = jplephem_singleton()
                         .as_ref()
                         .unwrap()
-                        .geocentric_state(SolarSystem::MOON, &tm)
+                        .geocentric_state(SolarSystem::Moon, &tm)
                         .unwrap();
                     // Scale Earth velocity
                     tvel = tvel - mvel / (1.0 + jplephem_singleton().as_ref().unwrap().emrat);
                 }
                 if src == 3 {
                     spos = Vec3::zeros();
                     let (_mpos, mvel): (Vec3, Vec3) = jplephem_singleton()
                         .as_ref()
                         .unwrap()
-                        .geocentric_state(SolarSystem::MOON, &tm)
+                        .geocentric_state(SolarSystem::Moon, &tm)
                         .unwrap();
                     //Scale Earth velocity
                     svel = svel - mvel / (1.0 + jplephem_singleton().as_ref().unwrap().emrat);
                 }
                 if src == 10 {
                     // Compute moon velocity in barycentric frame (not relative to Earth)
                     let (_embpos, embvel): (Vec3, Vec3) =
```

### Comparing `satkit-0.2.7/src/lib.rs` & `satkit-0.2.8/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 mod solarsystem;
 /// Space Weather
 pub mod spaceweather;
 /// Two-line Element Set
 pub mod tle;
 /// Utility functions
 pub mod utils;
+/// Keplerian orbital elements
+pub mod kepler;
 
 // Integrate ordinary differential equations
 mod ode;
 
 mod duration;
 
 // Objects available at crate level
```

### Comparing `satkit-0.2.7/src/lpephem/moon.rs` & `satkit-0.2.8/src/lpephem/moon.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/lpephem/sun.rs` & `satkit-0.2.8/src/lpephem/sun.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/nrlmsise.rs` & `satkit-0.2.8/src/nrlmsise.rs`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,37 @@
 ///   2 : 3 hr AP index for 3 hrs before current time
 ///   3 : 3 hr AP index for 6 hrs before current time
 ///   4 : 3 hr AP index for 9 hrs before current time
 ///   5 : Average of eight 3 hr AP indicies from 12 to 33 hrs
 ///           prior to current time
 ///   6 : Average of eight 3 hr AP indicies from 36 to 57 hrs
 ///           prior to current time
+#[allow(non_camel_case_types)]
 #[repr(C)]
 struct ap_array {
     a: [cty::c_double; 7],
 }
 
 ///  
 ///   Switches: to turn on and off particular variations use these switches.
 ///   0 is off, 1 is on, and 2 is main effects off but cross terms on.
 ///
 ///   Standard values are 0 for switch 0 and 1 for switches 1 to 23. The
 ///   array "switches" needs to be set accordingly by the calling program.
 //   The arrays sw and swc are set internally.
 #[repr(C)]
+#[allow(non_camel_case_types)]
 struct nrlmsise_flags {
     switches: [cty::c_int; 24],
     sw: [cty::c_double; 24],
     swc: [cty::c_double; 24],
 }
 
 #[repr(C)]
+#[allow(non_camel_case_types)]
 struct nrlmsise_input {
     year: cty::c_int,     /* Year, currently ignored */
     day: cty::c_int,      /* day of year */
     sec: cty::c_double,   // seconds in day (UT)
     alt: cty::c_double,   // altitude in km
     g_lat: cty::c_double, // geodetic latitude (deg?)
     g_lon: cty::c_double, // geodetic longitude (deg?)
@@ -56,14 +59,15 @@
 ///      d[5] - TOTAL MASS DENSITY(GM/CM3) [includes d[8] in td7d]
 ///      d[6] - H NUMBER DENSITY(CM-3)
 ///      d[7] - N NUMBER DENSITY(CM-3)
 ///      d[8] - Anomalous oxygen NUMBER DENSITY(CM-3)
 ///      t[0] - EXOSPHERIC TEMPERATURE
 ///      t[1] - TEMPERATURE AT ALT
 #[repr(C)]
+#[allow(non_camel_case_types)]
 struct nrlmsise_output {
     d: [cty::c_double; 9],
     t: [cty::c_double; 2],
 }
 
 extern "C" {
     fn gtd7d(input: *mut nrlmsise_input, flags: *mut nrlmsise_flags, output: *mut nrlmsise_output);
@@ -105,15 +109,15 @@
     let mut f107a: f64 = 150.0;
     let mut f107: f64 = 150.0;
     let mut ap: f64 = 4.0;
 
     if time_option.is_some() {
         let time = time_option.unwrap();
         let (year, _mon, _day, dhour, dmin, dsec) = time.to_datetime();
-        let fday: f64 = (time - AstroTime::from_date(year, 1, 1)).days() + 1.0;
+        let fday: f64 = (time - AstroTime::from_date(year as i32, 1, 1)).days() + 1.0;
         day_of_year = fday.floor() as i32;
         sec_of_day = dhour as f64 * 3600.0 + dmin as f64 * 60.0 + dsec;
 
         if use_spaceweather {
             match spaceweather::get(time - 1.0) {
                 Ok(r) => {
                     f107a = r.f10p7_adj_c81;
```

### Comparing `satkit-0.2.7/src/ode/mod.rs` & `satkit-0.2.8/src/ode/mod.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/nalgebra.rs` & `satkit-0.2.8/src/ode/nalgebra.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rk_adaptive.rs` & `satkit-0.2.8/src/ode/rk_adaptive.rs`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         if sol.x > xend {
             return Err(Box::new(ODEError::InterpExceedsSolutionBounds));
         }
         let dense = sol.dense.as_ref().unwrap();
         if sol.x < dense.x[0] {
             return Err(Box::new(ODEError::InterpExceedsSolutionBounds));
         }
-        let n = ((xend - xstart) / dx).ceil() as usize + 1;
+        let n = ((xend - xstart) / dx) as usize + 1;
         let mut xarr: Vec<f64> = (0..n).map(|v| v as f64 * dx + xstart).collect();
         if *xarr.last().unwrap() > xend {
             xarr.pop();
             xarr.push(xend);
         }
 
         let mut lastidx: usize = 0;
```

### Comparing `satkit-0.2.7/src/ode/rk_adaptive_settings.rs` & `satkit-0.2.8/src/ode/rk_adaptive_settings.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rk_explicit.rs` & `satkit-0.2.8/src/ode/rk_explicit.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkf45.rs` & `satkit-0.2.8/src/ode/rkf45.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkts54.rs` & `satkit-0.2.8/src/ode/rkts54.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkv65.rs` & `satkit-0.2.8/src/ode/rkv65.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkv65_table.rs` & `satkit-0.2.8/src/ode/rkv65_table.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkv87.rs` & `satkit-0.2.8/src/ode/rkv87.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkv87_table.rs` & `satkit-0.2.8/src/ode/rkv87_table.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkv98.rs` & `satkit-0.2.8/src/ode/rkv98.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkv98_nointerp.rs` & `satkit-0.2.8/src/ode/rkv98_nointerp.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkv98_nointerp_table.rs` & `satkit-0.2.8/src/ode/rkv98_nointerp_table.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/rkv98_table.rs` & `satkit-0.2.8/src/ode/rkv98_table.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/ode/types.rs` & `satkit-0.2.8/src/ode/types.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/orbitprop/drag.rs` & `satkit-0.2.8/src/orbitprop/drag.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/orbitprop/point_gravity.rs` & `satkit-0.2.8/src/orbitprop/point_gravity.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/orbitprop/propagator.rs` & `satkit-0.2.8/src/orbitprop/propagator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         // get GCRS position & velocity;
         let pos_gcrf: na::Vector3<f64> = y.fixed_view::<3, 1>(0, 0).into();
         let vel_gcrf: na::Vector3<f64> = y.fixed_view::<3, 1>(3, 0).into();
 
         // Moon position
         let (sun_gcrf, moon_gcrf) = match self.settings.use_jplephem {
             true => (
-                jplephem::geocentric_pos(SolarSystem::SUN, &time)?,
-                jplephem::geocentric_pos(SolarSystem::MOON, &time)?,
+                jplephem::geocentric_pos(SolarSystem::Sun, &time)?,
+                jplephem::geocentric_pos(SolarSystem::Moon, &time)?,
             ),
             false => (
                 lpephem::sun::pos_gcrf(&time),
                 lpephem::moon::pos_gcrf(&time),
             ),
         };
 
@@ -96,15 +96,14 @@
         // t should be between 0 & 1
         let t = grav_idx - grav_idx.floor();
 
         let q1 = &self.qgcrs2itrf_table[grav_idx as usize];
         let q2 = &self.qgcrs2itrf_table[grav_idx as usize + 1];
         // Quaternion to go from inertial to terrestrial frame
         let qgcrf2itrf = q1.slerp(q2, t);
-        //let qgcrf2itrf = frametransform::qgcrf2itrf_approx(&tm);
         let qitrf2gcrf = qgcrf2itrf.conjugate();
 
         // Position in ITRF coordinates
         let pos_itrf = qgcrf2itrf * pos_gcrf;
 
         // Propagating a "simple" 6-dof (position, velocity) state
         if C == 1 {
@@ -386,15 +385,15 @@
         qgcrs2itrf_table: {
             let ntimes: u32 = 2 + (duration_secs / settings.gravity_interp_dt_secs).ceil() as u32;
             (0..ntimes)
                 .into_iter()
                 .map(|x| {
                     let tm: AstroTime =
                         *start + x as f64 * tdir * settings.gravity_interp_dt_secs / 86400.0; // Use high-precision transform
-                    frametransform::qgcrf2itrf(&tm)
+                    frametransform::qgcrf2itrf_approx(&tm)
                 })
                 .collect()
         },
         satprops: satprops,
     };
 
     // Duration to end of integration, in seconds
@@ -647,15 +646,15 @@
             .lines()
             .filter(|x: &Result<String, io::Error>| {
                 x.as_ref().unwrap().chars().nth(0).unwrap() == '*'
             })
             .map(|rline| -> SKResult<crate::AstroTime> {
                 let line = rline.unwrap();
                 let lvals: Vec<&str> = line.split_whitespace().collect();
-                let year: u32 = lvals[1].parse()?;
+                let year: i32 = lvals[1].parse()?;
                 let mon: u32 = lvals[2].parse()?;
                 let day: u32 = lvals[3].parse()?;
                 let hour: u32 = lvals[4].parse()?;
                 let min: u32 = lvals[5].parse()?;
                 let sec: f64 = lvals[6].parse()?;
                 Ok(AstroTime::from_datetime(year, mon, day, hour, min, sec))
             })
```

### Comparing `satkit-0.2.7/src/orbitprop/satproperties.rs` & `satkit-0.2.8/src/orbitprop/satproperties.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/orbitprop/satstate.rs` & `satkit-0.2.8/src/orbitprop/satstate.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/orbitprop/settings.rs` & `satkit-0.2.8/src/orbitprop/settings.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/mod.rs` & `satkit-0.2.8/src/pybindings/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 mod pylpephem_sun;
 mod pynrlmsise;
 mod pyquaternion;
 mod pysatstate;
 mod pysgp4;
 mod pysolarsystem;
 mod pytle;
+mod pykepler;
 
 mod pypropagate;
 mod pypropsettings;
 mod pysatproperties;
 
 mod pyutils;
 
 use pyastrotime::PyAstroTime;
 use pyduration::PyDuration;
 use pyframetransform as pyft;
 use pyitrfcoord::PyITRFCoord;
+use pykepler::PyKepler;
 use pyquaternion::Quaternion;
 use pysolarsystem::SolarSystem;
 
 use pypropsettings::PyPropSettings;
 use pysatstate::PySatState;
 
 /// JPL Ephemeris Sub-Module
@@ -131,14 +133,16 @@
 
     m.add_class::<pyconsts::Consts>()?;
     m.add_class::<SolarSystem>()?;
     m.add_class::<pytle::PyTLE>()?;
 
     m.add_class::<PyITRFCoord>()?;
 
+    m.add_class::<PyKepler>()?;
+
     m.add_wrapped(wrap_pymodule!(frametransform))?;
     m.add_wrapped(wrap_pymodule!(jplephem))?;
     m.add_wrapped(wrap_pymodule!(sun))?;
     m.add_wrapped(wrap_pymodule!(moon))?;
     m.add_wrapped(wrap_pymodule!(satprop))?;
 
     m.add_wrapped(wrap_pymodule!(mod_utils::utils))?;
```

### Comparing `satkit-0.2.7/src/pybindings/mod_utils.rs` & `satkit-0.2.8/src/pybindings/mod_utils.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pyastrotime.rs` & `satkit-0.2.8/src/pybindings/pyastrotime.rs`

 * *Files 1% similar despite different names*

```diff
@@ -155,20 +155,20 @@
             match AstroTime::now() {
                 Ok(v) => Ok(PyAstroTime { inner: v }),
                 Err(_) => Err(pyo3::exceptions::PyOSError::new_err(
                     "Could not get current time",
                 )),
             }
         } else if py_args.len() == 3 {
-            let year = py_args.get_item(0)?.extract::<u32>()?;
+            let year = py_args.get_item(0)?.extract::<i32>()?;
             let month = py_args.get_item(1)?.extract::<u32>()?;
             let day = py_args.get_item(2)?.extract::<u32>()?;
             Self::from_date(year, month, day)
         } else if py_args.len() >= 6 {
-            let year = py_args.get_item(0)?.extract::<u32>()?;
+            let year = py_args.get_item(0)?.extract::<i32>()?;
             let month = py_args.get_item(1)?.extract::<u32>()?;
             let day = py_args.get_item(2)?.extract::<u32>()?;
             let hour = py_args.get_item(3)?.extract::<u32>()?;
             let min = py_args.get_item(4)?.extract::<u32>()?;
             let sec = py_args.get_item(5)?.extract::<f64>()?;
             let pyscale = match py_args.len() > 6 {
                 false => pyscale,
@@ -202,15 +202,15 @@
     ///     year (int): Gregorian year (e.g., 2024)
     ///     month (int): Gregorian month (1 = January, 2 = February, ...)
     ///     day (int): Day of month, beginning with 1
     /// 
     /// Returns:
     ///     satkit.time: Time object representing instant of input date
     #[staticmethod]
-    fn from_date(year: u32, month: u32, day: u32) -> PyResult<Self> {
+    fn from_date(year: i32, month: u32, day: u32) -> PyResult<Self> {
         Ok(PyAstroTime {
             inner: AstroTime::from_date(year, month, day),
         })
     }
 
     /// Return time object representing input modified Julian date and time scale
     ///
@@ -271,15 +271,15 @@
     ///     scale (satkit.timescale, optional): Time scale, default is satkit.timescale.UTC
     /// 
     /// Returns:
     ///    satkit.time: satkit.time object representing input Gregorian date and time
     #[staticmethod]
     #[pyo3(signature=(year, month, day, hour, min, sec, scale=PyTimeScale::UTC))]
     fn from_gregorian(
-        year: u32,
+        year: i32,
         month: u32,
         day: u32,
         hour: u32,
         min: u32,
         sec: f64,
         scale: PyTimeScale,
     ) -> PyResult<Self> {
```

### Comparing `satkit-0.2.7/src/pybindings/pyconsts.rs` & `satkit-0.2.8/src/pybindings/pyconsts.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pydensity.rs` & `satkit-0.2.8/src/pybindings/pydensity.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pyduration.rs` & `satkit-0.2.8/src/pybindings/pyduration.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pyframetransform.rs` & `satkit-0.2.8/src/pybindings/pyframetransform.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pygravity.rs` & `satkit-0.2.8/src/pybindings/pygravity.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pyitrfcoord.rs` & `satkit-0.2.8/src/pybindings/pyitrfcoord.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pyjplephem.rs` & `satkit-0.2.8/src/pybindings/pyjplephem.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pylpephem_moon.rs` & `satkit-0.2.8/src/pybindings/pylpephem_moon.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pylpephem_sun.rs` & `satkit-0.2.8/src/pybindings/pylpephem_sun.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pynrlmsise.rs` & `satkit-0.2.8/src/pybindings/pynrlmsise.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pypropagate.rs` & `satkit-0.2.8/src/pybindings/pypropagate.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pypropsettings.rs` & `satkit-0.2.8/src/pybindings/pypropsettings.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pyquaternion.rs` & `satkit-0.2.8/src/pybindings/pyquaternion.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pysatproperties.rs` & `satkit-0.2.8/src/pybindings/pysatproperties.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pysatstate.rs` & `satkit-0.2.8/src/pybindings/pysatstate.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pysgp4.rs` & `satkit-0.2.8/src/pybindings/pysgp4.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pysolarsystem.rs` & `satkit-0.2.8/src/pybindings/pysolarsystem.rs`

 * *Files 13% similar despite different names*

```diff
@@ -11,56 +11,56 @@
 ///     solar system barycenter, with exception of moon,
 ///     which is computed in Geocentric system
 ///   * EMB (2) is the Earth-Moon barycenter
 ///   * The sun position is relative to the solar system barycenter
 ///     (it will be close to origin)
 #[pyclass(name = "solarsystem")]
 pub enum SolarSystem {
-    Mercury = SS::MERCURY as isize,
-    Venus = SS::VENUS as isize,
+    Mercury = SS::Mercury as isize,
+    Venus = SS::Venus as isize,
     EMB = SS::EMB as isize,
-    Mars = SS::MARS as isize,
-    Jupiter = SS::JUPITER as isize,
-    Saturn = SS::SATURN as isize,
-    Uranus = SS::URANUS as isize,
-    Neptune = SS::NEPTUNE as isize,
-    Pluto = SS::PLUTO as isize,
-    Moon = SS::MOON as isize,
-    Sun = SS::SUN as isize,
+    Mars = SS::Mars as isize,
+    Jupiter = SS::Jupiter as isize,
+    Saturn = SS::Saturn as isize,
+    Uranus = SS::Uranus as isize,
+    Neptune = SS::Neptune as isize,
+    Pluto = SS::Pluto as isize,
+    Moon = SS::Moon as isize,
+    Sun = SS::Sun as isize,
 }
 
 impl From<&SolarSystem> for SS {
     fn from(s: &SolarSystem) -> SS {
         match s {
-            &SolarSystem::Mercury => SS::MERCURY,
-            &SolarSystem::Venus => SS::VENUS,
+            &SolarSystem::Mercury => SS::Mercury,
+            &SolarSystem::Venus => SS::Venus,
             &SolarSystem::EMB => SS::EMB,
-            &SolarSystem::Mars => SS::MARS,
-            &SolarSystem::Jupiter => SS::JUPITER,
-            &SolarSystem::Saturn => SS::SATURN,
-            &SolarSystem::Uranus => SS::URANUS,
-            &SolarSystem::Neptune => SS::NEPTUNE,
-            &SolarSystem::Pluto => SS::PLUTO,
-            &SolarSystem::Moon => SS::MOON,
-            &SolarSystem::Sun => SS::SUN,
+            &SolarSystem::Mars => SS::Mars,
+            &SolarSystem::Jupiter => SS::Jupiter,
+            &SolarSystem::Saturn => SS::Saturn,
+            &SolarSystem::Uranus => SS::Uranus,
+            &SolarSystem::Neptune => SS::Neptune,
+            &SolarSystem::Pluto => SS::Pluto,
+            &SolarSystem::Moon => SS::Moon,
+            &SolarSystem::Sun => SS::Sun,
         }
     }
 }
 
 impl IntoPy<PyObject> for SS {
     fn into_py(self, py: Python<'_>) -> PyObject {
         let ss: SolarSystem = match self {
-            SS::MERCURY => SolarSystem::Mercury,
-            SS::VENUS => SolarSystem::Venus,
+            SS::Mercury => SolarSystem::Mercury,
+            SS::Venus => SolarSystem::Venus,
             SS::EMB => SolarSystem::EMB,
-            SS::MARS => SolarSystem::Mars,
-            SS::JUPITER => SolarSystem::Jupiter,
-            SS::SATURN => SolarSystem::Saturn,
-            SS::URANUS => SolarSystem::Uranus,
-            SS::NEPTUNE => SolarSystem::Neptune,
-            SS::PLUTO => SolarSystem::Pluto,
-            SS::MOON => SolarSystem::Moon,
-            SS::SUN => SolarSystem::Sun,
+            SS::Mars => SolarSystem::Mars,
+            SS::Jupiter => SolarSystem::Jupiter,
+            SS::Saturn => SolarSystem::Saturn,
+            SS::Uranus => SolarSystem::Uranus,
+            SS::Neptune => SolarSystem::Neptune,
+            SS::Pluto => SolarSystem::Pluto,
+            SS::Moon => SolarSystem::Moon,
+            SS::Sun => SolarSystem::Sun,
         };
         ss.into_py(py)
     }
 }
```

### Comparing `satkit-0.2.7/src/pybindings/pytle.rs` & `satkit-0.2.8/src/pybindings/pytle.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/pybindings/pyutils.rs` & `satkit-0.2.8/src/pybindings/pyutils.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/dpper.rs` & `satkit-0.2.8/src/sgp4/dpper.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/dscom.rs` & `satkit-0.2.8/src/sgp4/dscom.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/dsinit.rs` & `satkit-0.2.8/src/sgp4/dsinit.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/dspace.rs` & `satkit-0.2.8/src/sgp4/dspace.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/getgravconst.rs` & `satkit-0.2.8/src/sgp4/getgravconst.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/initl.rs` & `satkit-0.2.8/src/sgp4/initl.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/mod.rs` & `satkit-0.2.8/src/sgp4/mod.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/satrec.rs` & `satkit-0.2.8/src/sgp4/satrec.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/sgp4.rs` & `satkit-0.2.8/src/sgp4/sgp4.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/sgp4_lowlevel.rs` & `satkit-0.2.8/src/sgp4/sgp4_lowlevel.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/sgp4/sgp4init.rs` & `satkit-0.2.8/src/sgp4/sgp4init.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/solarsystem.rs` & `satkit-0.2.8/src/solarsystem.rs`

 * *Files 17% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 ///    which is computed in Geocentric system
 ///  * EMB (2) is the Earth-Moon barycenter
 ///  * The sun position is relative to the solar system barycenter
 ///    (it will be close to origin)
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 pub enum SolarSystem {
     /// Mercury
-    MERCURY = 0,
+    Mercury = 0,
     /// Venus
-    VENUS = 1,
+    Venus = 1,
     /// Earth-Moon Barycenter
     EMB = 2,
     /// Mars
-    MARS = 3,
+    Mars = 3,
     /// Jupiter
-    JUPITER = 4,
+    Jupiter = 4,
     /// Saturn
-    SATURN = 5,
+    Saturn = 5,
     /// Uranus
-    URANUS = 6,
+    Uranus = 6,
     /// Neptune
-    NEPTUNE = 7,
+    Neptune = 7,
     /// Pluto
-    PLUTO = 8,
+    Pluto = 8,
     /// Moon (Geocentric)
-    MOON = 9,
+    Moon = 9,
     /// Sun
-    SUN = 10,
+    Sun = 10,
 }
```

### Comparing `satkit-0.2.7/src/spaceweather.rs` & `satkit-0.2.8/src/spaceweather.rs`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 None => return skerror!("Invalid month in file"),
             };
             let day: u32 = match str2num(lvals[0], 8, 10) {
                 Some(v) => v,
                 None => return skerror!("invalid day in file"),
             };
             Ok(SpaceWeatherRecord {
-                date: (AstroTime::from_date(year, mon, day)),
+                date: (AstroTime::from_date(year as i32, mon, day)),
                 bsrn: lvals[1].parse().unwrap_or(-1),
                 nd: lvals[2].parse().unwrap_or(-1),
                 kp: {
                     let mut kparr: [i32; 8] = [-1, -1, -1, -1, -1, -1, -1, -1];
                     for idx in 0..8 {
                         kparr[idx] = lvals[idx + 3].parse().unwrap_or(-1);
                     }
@@ -164,15 +164,15 @@
             None => continue,
         };
         let day: u32 = match str2num(&vline, 8, 10) {
             Some(v) => v,
             None => continue,
         };
         sw.push(SpaceWeatherRecord {
-            date: (AstroTime::from_date(year, mon, day)),
+            date: (AstroTime::from_date(year as i32, mon, day)),
             bsrn: (str2num(&vline, 11, 15).unwrap_or(-1)),
             nd: (str2num(&vline, 16, 18).unwrap_or(-1)),
             kp: {
                 let mut kparr: [i32; 8] = [-1, -1, -1, -1, -1, -1, -1, -1];
                 for idx in 0..8 {
                     kparr[idx] = str2num(&vline, idx * 3 + 19, idx * 3 + 21).unwrap_or(-1);
                 }
```

### Comparing `satkit-0.2.7/src/tle.rs` & `satkit-0.2.8/src/tle.rs`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
             Ok(y) => y,
             Err(_) => return Err("Could not parse day of year".to_string()),
         };
 
         // Note: day_of_year starts from 1, not zero,
         // also, go from Jan 2 to avoid leap-second
         // issues, hence the "-2" at end
-        let epoch = AstroTime::from_date(year, 1, 2).add_utc_days(day_of_year - 2.0);
+        let epoch = AstroTime::from_date(year as i32, 1, 2).add_utc_days(day_of_year - 2.0);
 
         Ok(TLE {
             name: "none".to_string(),
             sat_num: {
                 match line1[2..7].trim().parse() {
                     Ok(y) => y,
                     Err(_) => return Err("Could not parse sat number".to_string()),
```

### Comparing `satkit-0.2.7/src/utils/datadir.rs` & `satkit-0.2.8/src/utils/datadir.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/utils/download.rs` & `satkit-0.2.8/src/utils/download.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/utils/mod.rs` & `satkit-0.2.8/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/utils/skerror.rs` & `satkit-0.2.8/src/utils/skerror.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/utils/test.rs` & `satkit-0.2.8/src/utils/test.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.7/src/utils/update_data.rs` & `satkit-0.2.8/src/utils/update_data.rs`

 * *Files identical despite different names*

