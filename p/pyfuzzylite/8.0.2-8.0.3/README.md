# Comparing `tmp/pyfuzzylite-8.0.2.tar.gz` & `tmp/pyfuzzylite-8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfuzzylite-8.0.2.tar", max compression
+gzip compressed data, was "pyfuzzylite-8.0.3.tar", max compression
```

## Comparing `pyfuzzylite-8.0.2.tar` & `pyfuzzylite-8.0.3.tar`

### file list

```diff
@@ -1,245 +1,244 @@
--rw-r--r--   0        0        0       71 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/AUTHOR
--rw-r--r--   0        0        0      807 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/CITATION.cff
--rw-r--r--   0        0        0      142 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/LICENSE.FuzzyLite.txt
--rw-r--r--   0        0        0    35148 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/LICENSE.GPL.txt
--rw-r--r--   0        0        0     8480 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/README.md
--rw-r--r--   0        0        0     1082 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/__init__.py
--rw-r--r--   0        0        0    17447 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/activation.py
--rw-r--r--   0        0        0     7896 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/benchmark.py
--rw-r--r--   0        0        0    21720 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/defuzzifier.py
--rw-r--r--   0        0        0    24441 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/engine.py
--rw-r--r--   0        0        0      134 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/__init__.py
--rw-r--r--   0        0        0       84 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/__init__.py
--rw-r--r--   0        0        0    36888 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.fld
--rw-r--r--   0        0        0     1073 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.fll
--rw-r--r--   0        0        0     2435 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.py
--rw-r--r--   0        0        0    50840 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.fld
--rw-r--r--   0        0        0     2103 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.fll
--rw-r--r--   0        0        0     4431 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.py
--rw-r--r--   0        0        0      347 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/__init__.py
--rw-r--r--   0        0        0    24605 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.fld
--rw-r--r--   0        0        0     2986 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.fll
--rw-r--r--   0        0        0     6258 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.py
--rw-r--r--   0        0        0    49885 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.fld
--rw-r--r--   0        0        0     1645 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.fll
--rw-r--r--   0        0        0     5788 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.py
--rw-r--r--   0        0        0      142 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/__init__.py
--rw-r--r--   0        0        0    38421 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.fld
--rw-r--r--   0        0        0     1034 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.fll
--rw-r--r--   0        0        0     2392 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.py
--rw-r--r--   0        0        0    51228 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.fld
--rw-r--r--   0        0        0     1454 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.fll
--rw-r--r--   0        0        0     3206 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.py
--rw-r--r--   0        0        0    51731 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.fld
--rw-r--r--   0        0        0     2101 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.fll
--rw-r--r--   0        0        0     4507 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.py
--rw-r--r--   0        0        0    38427 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.fld
--rw-r--r--   0        0        0     1211 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.fll
--rw-r--r--   0        0        0     2754 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.py
--rw-r--r--   0        0        0    38441 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.fld
--rw-r--r--   0        0        0     1194 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.fll
--rw-r--r--   0        0        0     2681 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.py
--rw-r--r--   0        0        0    37749 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.fld
--rw-r--r--   0        0        0      985 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.fll
--rw-r--r--   0        0        0     2338 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.py
--rw-r--r--   0        0        0    25357 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.fld
--rw-r--r--   0        0        0      766 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.fll
--rw-r--r--   0        0        0     1863 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.py
--rw-r--r--   0        0        0    24592 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.fld
--rw-r--r--   0        0        0      621 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.fll
--rw-r--r--   0        0        0     1501 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.py
--rw-r--r--   0        0        0      120 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/__init__.py
--rw-r--r--   0        0        0    39013 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.fld
--rw-r--r--   0        0        0     1209 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.fll
--rw-r--r--   0        0        0     2616 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.py
--rw-r--r--   0        0        0    50277 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fld
--rw-r--r--   0        0        0     1651 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fll
--rw-r--r--   0        0        0     3516 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.py
--rw-r--r--   0        0        0    24574 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.fld
--rw-r--r--   0        0        0      765 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.fll
--rw-r--r--   0        0        0     1862 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.py
--rw-r--r--   0        0        0    36859 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.fld
--rw-r--r--   0        0        0     1195 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.fll
--rw-r--r--   0        0        0     2723 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.py
--rw-r--r--   0        0        0    36859 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.fld
--rw-r--r--   0        0        0     1195 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.fll
--rw-r--r--   0        0        0     2723 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.py
--rw-r--r--   0        0        0      215 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/__init__.py
--rw-r--r--   0        0        0    49859 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.fld
--rw-r--r--   0        0        0     1927 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.fll
--rw-r--r--   0        0        0     3984 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.py
--rw-r--r--   0        0        0      410 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/__init__.py
--rw-r--r--   0        0        0    38334 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fld
--rw-r--r--   0        0        0     2524 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fll
--rw-r--r--   0        0        0     4762 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.py
--rw-r--r--   0        0        0    38262 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fld
--rw-r--r--   0        0        0     6722 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fll
--rw-r--r--   0        0        0    13825 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.py
--rw-r--r--   0        0        0    38259 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fld
--rw-r--r--   0        0        0     5133 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fll
--rw-r--r--   0        0        0    10674 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.py
--rw-r--r--   0        0        0    37614 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.fld
--rw-r--r--   0        0        0     1751 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.fll
--rw-r--r--   0        0        0     3943 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.py
--rw-r--r--   0        0        0    38551 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fld
--rw-r--r--   0        0        0     1076 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fll
--rw-r--r--   0        0        0     2669 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.py
--rw-r--r--   0        0        0    38522 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fld
--rw-r--r--   0        0        0     1705 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fll
--rw-r--r--   0        0        0     3939 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.py
--rw-r--r--   0        0        0    38833 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.fld
--rw-r--r--   0        0        0     3394 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.fll
--rw-r--r--   0        0        0     6518 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.py
--rw-r--r--   0        0        0    39172 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.fld
--rw-r--r--   0        0        0     3386 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.fll
--rw-r--r--   0        0        0     6512 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.py
--rw-r--r--   0        0        0    76882 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fld
--rw-r--r--   0        0        0     1103 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fll
--rw-r--r--   0        0        0     2302 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.py
--rw-r--r--   0        0        0    13064 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fld
--rw-r--r--   0        0        0     2744 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fll
--rw-r--r--   0        0        0     5057 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.py
--rw-r--r--   0        0        0    50135 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fld
--rw-r--r--   0        0        0      816 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fll
--rw-r--r--   0        0        0     1891 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.py
--rw-r--r--   0        0        0    25487 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fld
--rw-r--r--   0        0        0      614 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fll
--rw-r--r--   0        0        0     1485 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.py
--rw-r--r--   0        0        0    38427 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fld
--rw-r--r--   0        0        0     1145 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fll
--rw-r--r--   0        0        0     2693 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.py
--rw-r--r--   0        0        0    37709 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fld
--rw-r--r--   0        0        0      986 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fll
--rw-r--r--   0        0        0     2338 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.py
--rw-r--r--   0        0        0    24593 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fld
--rw-r--r--   0        0        0      620 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fll
--rw-r--r--   0        0        0     1501 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.py
--rw-r--r--   0        0        0      244 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/__init__.py
--rw-r--r--   0        0        0    26243 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fld
--rw-r--r--   0        0        0     2109 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fll
--rw-r--r--   0        0        0     3994 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.py
--rw-r--r--   0        0        0    39580 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fld
--rw-r--r--   0        0        0     2505 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fll
--rw-r--r--   0        0        0     5136 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.py
--rw-r--r--   0        0        0    37976 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fld
--rw-r--r--   0        0        0     1124 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fll
--rw-r--r--   0        0        0     2659 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.py
--rw-r--r--   0        0        0    64628 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fld
--rw-r--r--   0        0        0     2646 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fll
--rw-r--r--   0        0        0     5360 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.py
--rw-r--r--   0        0        0    24574 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.fld
--rw-r--r--   0        0        0      743 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.fll
--rw-r--r--   0        0        0     1840 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.py
--rw-r--r--   0        0        0      707 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/__init__.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.fld
--rw-r--r--   0        0        0      818 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.fll
--rw-r--r--   0        0        0     1837 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.fld
--rw-r--r--   0        0        0      833 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.fll
--rw-r--r--   0        0        0     1855 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.fld
--rw-r--r--   0        0        0      824 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.fll
--rw-r--r--   0        0        0     1856 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.fld
--rw-r--r--   0        0        0      830 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.fll
--rw-r--r--   0        0        0     1853 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.fld
--rw-r--r--   0        0        0      835 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.fll
--rw-r--r--   0        0        0     1857 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.fld
--rw-r--r--   0        0        0      827 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.fll
--rw-r--r--   0        0        0     1853 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.fld
--rw-r--r--   0        0        0     3233 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.fll
--rw-r--r--   0        0        0    15622 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.fld
--rw-r--r--   0        0        0     1007 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.fll
--rw-r--r--   0        0        0     2274 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.fld
--rw-r--r--   0        0        0      833 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.fll
--rw-r--r--   0        0        0     1861 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.fld
--rw-r--r--   0        0        0      878 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.fll
--rw-r--r--   0        0        0     1988 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.fld
--rw-r--r--   0        0        0      841 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.fll
--rw-r--r--   0        0        0     1863 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.fld
--rw-r--r--   0        0        0      854 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.fll
--rw-r--r--   0        0        0     1952 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.fld
--rw-r--r--   0        0        0      821 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.fll
--rw-r--r--   0        0        0     1837 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.fld
--rw-r--r--   0        0        0      836 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.fll
--rw-r--r--   0        0        0     1861 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.fld
--rw-r--r--   0        0        0      842 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.fll
--rw-r--r--   0        0        0     1869 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.fld
--rw-r--r--   0        0        0      833 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.fll
--rw-r--r--   0        0        0     1852 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.fld
--rw-r--r--   0        0        0      888 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.fll
--rw-r--r--   0        0        0     1988 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.fld
--rw-r--r--   0        0        0      881 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.fll
--rw-r--r--   0        0        0     1978 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.fld
--rw-r--r--   0        0        0      824 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.fll
--rw-r--r--   0        0        0     1849 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.fld
--rw-r--r--   0        0        0      860 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.fll
--rw-r--r--   0        0        0     1956 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.fld
--rw-r--r--   0        0        0      845 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.fll
--rw-r--r--   0        0        0     1942 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.py
--rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.fld
--rw-r--r--   0        0        0      828 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.fll
--rw-r--r--   0        0        0     1847 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.py
--rw-r--r--   0        0        0       48 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/__init__.py
--rw-r--r--   0        0        0    61997 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.fld
--rw-r--r--   0        0        0     1629 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.fll
--rw-r--r--   0        0        0     3722 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.py
--rw-r--r--   0        0        0    27206 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/exporter.py
--rw-r--r--   0        0        0    24708 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/factory.py
--rw-r--r--   0        0        0    40263 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/hedge.py
--rw-r--r--   0        0        0    17083 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/importer.py
--rw-r--r--   0        0        0    15021 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/library.py
--rw-r--r--   0        0        0    23089 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/norm.py
--rw-r--r--   0        0        0    16996 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/operation.py
--rw-r--r--   0        0        0        0 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/py.typed
--rw-r--r--   0        0        0    34909 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/rule.py
--rw-r--r--   0        0        0   101160 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/term.py
--rw-r--r--   0        0        0      278 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/types.py
--rw-r--r--   0        0        0    17502 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/variable.py
--rw-r--r--   0        0        0    17073 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite.png
--rw-r--r--   0        0        0     5163 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/noxfile.py
--rw-r--r--   0        0        0       48 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/poetry.toml
--rw-r--r--   0        0        0     8471 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/pyproject.toml
--rw-r--r--   0        0        0       29 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/__init__.py
--rw-r--r--   0        0        0     4150 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/assert_component.py
--rw-r--r--   0        0        0     8974 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/notebooks/Hedges.ipynb
--rw-r--r--   0        0        0     4683 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/notebooks/Norms.ipynb
--rw-r--r--   0        0        0     9050 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/notebooks/Terms.ipynb
--rw-r--r--   0        0        0    25527 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_activation.py
--rw-r--r--   0        0        0    12037 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_benchmark.py
--rw-r--r--   0        0        0     7820 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_benchmark_codspeed.py
--rw-r--r--   0        0        0     8366 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_benchmark_pytest.py
--rw-r--r--   0        0        0    32083 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_defuzzifier.py
--rw-r--r--   0        0        0     3008 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_documentation.py
--rw-r--r--   0        0        0    40351 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_engine.py
--rw-r--r--   0        0        0     6106 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_examples.py
--rw-r--r--   0        0        0    39909 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_exporter.py
--rw-r--r--   0        0        0    18414 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_factory.py
--rw-r--r--   0        0        0     5297 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_hedge.py
--rw-r--r--   0        0        0    13578 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_importer.py
--rw-r--r--   0        0        0     8354 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_library.py
--rw-r--r--   0        0        0    16869 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_norm.py
--rw-r--r--   0        0        0    18108 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_operation.py
--rw-r--r--   0        0        0    40319 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_rule.py
--rw-r--r--   0        0        0    88012 2024-04-26 03:53:28.091707 pyfuzzylite-8.0.2/tests/test_term.py
--rw-r--r--   0        0        0    30049 2024-04-26 03:53:28.091707 pyfuzzylite-8.0.2/tests/test_variable.py
--rw-r--r--   0        0        0     7933 2024-04-26 03:53:28.091707 pyfuzzylite-8.0.2/tests/test_vectorization.py
--rw-r--r--   0        0        0    10096 1970-01-01 00:00:00.000000 pyfuzzylite-8.0.2/PKG-INFO
+-rw-r--r--   0        0        0       71 2024-05-17 01:12:03.784356 pyfuzzylite-8.0.3/AUTHOR
+-rw-r--r--   0        0        0      799 2024-05-17 01:12:03.784356 pyfuzzylite-8.0.3/CITATION.cff
+-rw-r--r--   0        0        0      142 2024-05-17 01:12:03.784356 pyfuzzylite-8.0.3/LICENSE.FuzzyLite.txt
+-rw-r--r--   0        0        0    35148 2024-05-17 01:12:03.784356 pyfuzzylite-8.0.3/LICENSE.GPL.txt
+-rw-r--r--   0        0        0     8389 2024-05-17 01:12:03.784356 pyfuzzylite-8.0.3/README.md
+-rw-r--r--   0        0        0      827 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/__init__.py
+-rw-r--r--   0        0        0    17082 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/activation.py
+-rw-r--r--   0        0        0     7530 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/benchmark.py
+-rw-r--r--   0        0        0    21355 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/defuzzifier.py
+-rw-r--r--   0        0        0    24076 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/engine.py
+-rw-r--r--   0        0        0      134 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/__init__.py
+-rw-r--r--   0        0        0       84 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/__init__.py
+-rw-r--r--   0        0        0    36888 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/obstacle_avoidance.fld
+-rw-r--r--   0        0        0     1073 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/obstacle_avoidance.fll
+-rw-r--r--   0        0        0     2435 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/obstacle_avoidance.py
+-rw-r--r--   0        0        0    50840 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/tipper.fld
+-rw-r--r--   0        0        0     2103 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/tipper.fll
+-rw-r--r--   0        0        0     4431 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/tipper.py
+-rw-r--r--   0        0        0      347 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/__init__.py
+-rw-r--r--   0        0        0    24605 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/all_terms.fld
+-rw-r--r--   0        0        0     2986 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/all_terms.fll
+-rw-r--r--   0        0        0     6258 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/all_terms.py
+-rw-r--r--   0        0        0    49885 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/laundry.fld
+-rw-r--r--   0        0        0     1645 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/laundry.fll
+-rw-r--r--   0        0        0     5788 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/laundry.py
+-rw-r--r--   0        0        0      142 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/__init__.py
+-rw-r--r--   0        0        0    38421 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam21.fld
+-rw-r--r--   0        0        0     1034 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam21.fll
+-rw-r--r--   0        0        0     2392 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam21.py
+-rw-r--r--   0        0        0    51228 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam22.fld
+-rw-r--r--   0        0        0     1454 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam22.fll
+-rw-r--r--   0        0        0     3206 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam22.py
+-rw-r--r--   0        0        0    51731 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/shower.fld
+-rw-r--r--   0        0        0     2101 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/shower.fll
+-rw-r--r--   0        0        0     4507 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/shower.py
+-rw-r--r--   0        0        0    38427 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank.fld
+-rw-r--r--   0        0        0     1211 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank.fll
+-rw-r--r--   0        0        0     2754 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank.py
+-rw-r--r--   0        0        0    38441 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank2.fld
+-rw-r--r--   0        0        0     1194 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank2.fll
+-rw-r--r--   0        0        0     2681 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank2.py
+-rw-r--r--   0        0        0    37749 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper.fld
+-rw-r--r--   0        0        0      985 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper.fll
+-rw-r--r--   0        0        0     2338 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper.py
+-rw-r--r--   0        0        0    25357 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper1.fld
+-rw-r--r--   0        0        0      766 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper1.fll
+-rw-r--r--   0        0        0     1863 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper1.py
+-rw-r--r--   0        0        0    24592 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/obstacle_avoidance.fld
+-rw-r--r--   0        0        0      621 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/obstacle_avoidance.fll
+-rw-r--r--   0        0        0     1501 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/obstacle_avoidance.py
+-rw-r--r--   0        0        0      120 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/__init__.py
+-rw-r--r--   0        0        0    39013 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/investment_portfolio.fld
+-rw-r--r--   0        0        0     1209 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/investment_portfolio.fll
+-rw-r--r--   0        0        0     2616 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/investment_portfolio.py
+-rw-r--r--   0        0        0    50277 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fld
+-rw-r--r--   0        0        0     1651 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fll
+-rw-r--r--   0        0        0     3516 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.py
+-rw-r--r--   0        0        0    24574 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer.fld
+-rw-r--r--   0        0        0      765 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer.fll
+-rw-r--r--   0        0        0     1862 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer.py
+-rw-r--r--   0        0        0    36859 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_chained.fld
+-rw-r--r--   0        0        0     1195 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_chained.fll
+-rw-r--r--   0        0        0     2723 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_chained.py
+-rw-r--r--   0        0        0    36859 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_inverse.fld
+-rw-r--r--   0        0        0     1195 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_inverse.fll
+-rw-r--r--   0        0        0     2723 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_inverse.py
+-rw-r--r--   0        0        0      215 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/__init__.py
+-rw-r--r--   0        0        0    49859 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/approximation.fld
+-rw-r--r--   0        0        0     1927 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/approximation.fll
+-rw-r--r--   0        0        0     3984 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/approximation.py
+-rw-r--r--   0        0        0      410 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/__init__.py
+-rw-r--r--   0        0        0    38334 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fld
+-rw-r--r--   0        0        0     2524 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fll
+-rw-r--r--   0        0        0     4762 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.py
+-rw-r--r--   0        0        0    38262 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fld
+-rw-r--r--   0        0        0     6722 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fll
+-rw-r--r--   0        0        0    13825 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine1.py
+-rw-r--r--   0        0        0    38259 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fld
+-rw-r--r--   0        0        0     5133 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fll
+-rw-r--r--   0        0        0    10674 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine2.py
+-rw-r--r--   0        0        0    37614 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/juggler.fld
+-rw-r--r--   0        0        0     1751 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/juggler.fll
+-rw-r--r--   0        0        0     3943 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/juggler.py
+-rw-r--r--   0        0        0    38551 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fld
+-rw-r--r--   0        0        0     1076 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fll
+-rw-r--r--   0        0        0     2669 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn1.py
+-rw-r--r--   0        0        0    38522 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fld
+-rw-r--r--   0        0        0     1705 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fll
+-rw-r--r--   0        0        0     3939 2024-05-17 01:12:03.828356 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn2.py
+-rw-r--r--   0        0        0    38833 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slbb.fld
+-rw-r--r--   0        0        0     3394 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slbb.fll
+-rw-r--r--   0        0        0     6518 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slbb.py
+-rw-r--r--   0        0        0    39172 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp.fld
+-rw-r--r--   0        0        0     3386 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp.fll
+-rw-r--r--   0        0        0     6512 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp.py
+-rw-r--r--   0        0        0    76882 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fld
+-rw-r--r--   0        0        0     1103 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fll
+-rw-r--r--   0        0        0     2302 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp1.py
+-rw-r--r--   0        0        0    13064 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fld
+-rw-r--r--   0        0        0     2744 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fll
+-rw-r--r--   0        0        0     5057 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.py
+-rw-r--r--   0        0        0    50135 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fld
+-rw-r--r--   0        0        0      816 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fll
+-rw-r--r--   0        0        0     1891 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.py
+-rw-r--r--   0        0        0    25487 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fld
+-rw-r--r--   0        0        0      614 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fll
+-rw-r--r--   0        0        0     1485 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.py
+-rw-r--r--   0        0        0    38427 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fld
+-rw-r--r--   0        0        0     1145 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fll
+-rw-r--r--   0        0        0     2693 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tanksg.py
+-rw-r--r--   0        0        0    37709 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fld
+-rw-r--r--   0        0        0      986 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fll
+-rw-r--r--   0        0        0     2338 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tippersg.py
+-rw-r--r--   0        0        0    24593 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fld
+-rw-r--r--   0        0        0      620 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fll
+-rw-r--r--   0        0        0     1501 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.py
+-rw-r--r--   0        0        0      244 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/__init__.py
+-rw-r--r--   0        0        0    26243 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fld
+-rw-r--r--   0        0        0     2109 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fll
+-rw-r--r--   0        0        0     3994 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.py
+-rw-r--r--   0        0        0    39580 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fld
+-rw-r--r--   0        0        0     2505 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fll
+-rw-r--r--   0        0        0     5136 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.py
+-rw-r--r--   0        0        0    37976 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fld
+-rw-r--r--   0        0        0     1124 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fll
+-rw-r--r--   0        0        0     2659 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.py
+-rw-r--r--   0        0        0    64628 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fld
+-rw-r--r--   0        0        0     2646 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fll
+-rw-r--r--   0        0        0     5360 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.py
+-rw-r--r--   0        0        0    24574 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/simple_dimmer.fld
+-rw-r--r--   0        0        0      743 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/simple_dimmer.fll
+-rw-r--r--   0        0        0     1840 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/simple_dimmer.py
+-rw-r--r--   0        0        0      707 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/__init__.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/arc.fld
+-rw-r--r--   0        0        0      818 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/arc.fll
+-rw-r--r--   0        0        0     1837 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/arc.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/bell.fld
+-rw-r--r--   0        0        0      833 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/bell.fll
+-rw-r--r--   0        0        0     1855 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/bell.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/binary.fld
+-rw-r--r--   0        0        0      824 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/binary.fll
+-rw-r--r--   0        0        0     1856 2024-05-17 01:12:03.832357 pyfuzzylite-8.0.3/fuzzylite/examples/terms/binary.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/concave.fld
+-rw-r--r--   0        0        0      830 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/concave.fll
+-rw-r--r--   0        0        0     1853 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/concave.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/constant.fld
+-rw-r--r--   0        0        0      835 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/constant.fll
+-rw-r--r--   0        0        0     1857 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/constant.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/cosine.fld
+-rw-r--r--   0        0        0      827 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/cosine.fll
+-rw-r--r--   0        0        0     1853 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/cosine.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/discrete.fld
+-rw-r--r--   0        0        0     3233 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/discrete.fll
+-rw-r--r--   0        0        0    15622 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/discrete.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/function.fld
+-rw-r--r--   0        0        0     1007 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/function.fll
+-rw-r--r--   0        0        0     2274 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/function.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian.fld
+-rw-r--r--   0        0        0      833 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian.fll
+-rw-r--r--   0        0        0     1861 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian_product.fld
+-rw-r--r--   0        0        0      878 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian_product.fll
+-rw-r--r--   0        0        0     1988 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian_product.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/linear.fld
+-rw-r--r--   0        0        0      841 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/linear.fll
+-rw-r--r--   0        0        0     1863 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/linear.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/pi_shape.fld
+-rw-r--r--   0        0        0      854 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/pi_shape.fll
+-rw-r--r--   0        0        0     1952 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/pi_shape.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/ramp.fld
+-rw-r--r--   0        0        0      821 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/ramp.fll
+-rw-r--r--   0        0        0     1837 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/ramp.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/rectangle.fld
+-rw-r--r--   0        0        0      836 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/rectangle.fll
+-rw-r--r--   0        0        0     1861 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/rectangle.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/semi_ellipse.fld
+-rw-r--r--   0        0        0      842 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/semi_ellipse.fll
+-rw-r--r--   0        0        0     1869 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/semi_ellipse.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid.fld
+-rw-r--r--   0        0        0      833 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid.fll
+-rw-r--r--   0        0        0     1852 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_difference.fld
+-rw-r--r--   0        0        0      888 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_difference.fll
+-rw-r--r--   0        0        0     1988 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_difference.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_product.fld
+-rw-r--r--   0        0        0      881 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_product.fll
+-rw-r--r--   0        0        0     1978 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_product.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/spike.fld
+-rw-r--r--   0        0        0      824 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/spike.fll
+-rw-r--r--   0        0        0     1849 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/spike.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/trapezoid.fld
+-rw-r--r--   0        0        0      860 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/trapezoid.fll
+-rw-r--r--   0        0        0     1956 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/trapezoid.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/triangle.fld
+-rw-r--r--   0        0        0      845 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/triangle.fll
+-rw-r--r--   0        0        0     1942 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/triangle.py
+-rw-r--r--   0        0        0    24575 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/zs_shape.fld
+-rw-r--r--   0        0        0      828 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/zs_shape.fll
+-rw-r--r--   0        0        0     1847 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/terms/zs_shape.py
+-rw-r--r--   0        0        0       48 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/tsukamoto/__init__.py
+-rw-r--r--   0        0        0    61997 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/tsukamoto/tsukamoto.fld
+-rw-r--r--   0        0        0     1629 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/tsukamoto/tsukamoto.fll
+-rw-r--r--   0        0        0     3722 2024-05-17 01:12:03.836356 pyfuzzylite-8.0.3/fuzzylite/examples/tsukamoto/tsukamoto.py
+-rw-r--r--   0        0        0    26879 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/exporter.py
+-rw-r--r--   0        0        0    24343 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/factory.py
+-rw-r--r--   0        0        0    39898 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/hedge.py
+-rw-r--r--   0        0        0    16686 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/importer.py
+-rw-r--r--   0        0        0    14760 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/library.py
+-rw-r--r--   0        0        0    22723 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/norm.py
+-rw-r--r--   0        0        0    16639 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/operation.py
+-rw-r--r--   0        0        0        0 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/py.typed
+-rw-r--r--   0        0        0    34732 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/rule.py
+-rw-r--r--   0        0        0   100863 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/term.py
+-rw-r--r--   0        0        0      522 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/types.py
+-rw-r--r--   0        0        0    17121 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/fuzzylite/variable.py
+-rw-r--r--   0        0        0    17073 2024-05-17 01:12:03.824356 pyfuzzylite-8.0.3/fuzzylite.png
+-rw-r--r--   0        0        0     5292 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/noxfile.py
+-rw-r--r--   0        0        0       48 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/poetry.toml
+-rw-r--r--   0        0        0     8288 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3785 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/assert_component.py
+-rw-r--r--   0        0        0     8974 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/notebooks/Hedges.ipynb
+-rw-r--r--   0        0        0     4683 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/notebooks/Norms.ipynb
+-rw-r--r--   0        0        0     9050 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/notebooks/Terms.ipynb
+-rw-r--r--   0        0        0    25168 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_activation.py
+-rw-r--r--   0        0        0    11672 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_benchmark.py
+-rw-r--r--   0        0        0     7455 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_benchmark_codspeed.py
+-rw-r--r--   0        0        0     8000 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_benchmark_pytest.py
+-rw-r--r--   0        0        0    31490 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_defuzzifier.py
+-rw-r--r--   0        0        0     2643 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_documentation.py
+-rw-r--r--   0        0        0    39999 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_engine.py
+-rw-r--r--   0        0        0     5741 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_examples.py
+-rw-r--r--   0        0        0    40944 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_exporter.py
+-rw-r--r--   0        0        0    18049 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_factory.py
+-rw-r--r--   0        0        0     4932 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_hedge.py
+-rw-r--r--   0        0        0    13213 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_importer.py
+-rw-r--r--   0        0        0     8522 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_library.py
+-rw-r--r--   0        0        0    19378 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_norm.py
+-rw-r--r--   0        0        0    17743 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_operation.py
+-rw-r--r--   0        0        0    40089 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_rule.py
+-rw-r--r--   0        0        0    78806 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_term.py
+-rw-r--r--   0        0        0    29740 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_variable.py
+-rw-r--r--   0        0        0     7568 2024-05-17 01:12:03.840356 pyfuzzylite-8.0.3/tests/test_vectorization.py
+-rw-r--r--   0        0        0    10005 1970-01-01 00:00:00.000000 pyfuzzylite-8.0.3/PKG-INFO
```

### Comparing `pyfuzzylite-8.0.2/CITATION.cff` & `pyfuzzylite-8.0.3/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   If you use this software, please cite it using the
   metadata from this file.
 type: software
 authors:
   - given-names: Juan
     family-names: Rada-Vilela
     email: jcrada@fuzzylite.com
-    affiliation: FuzzyLite Limited
+    affiliation: FuzzyLite
 repository-code: 'https://github.com/fuzzylite/pyfuzzylite'
 url: 'https://fuzzylite.com'
 abstract: >-
   The goal of the FuzzyLite Libraries is to easily design
   and efficiently operate fuzzy logic controllers following
   an object-oriented programming model with minimal
   dependency on external libraries.
```

### Comparing `pyfuzzylite-8.0.2/LICENSE.GPL.txt` & `pyfuzzylite-8.0.3/LICENSE.GPL.txt`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/README.md` & `pyfuzzylite-8.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,530 +1,525 @@
-00000000: 2320 7079 6675 7a7a 796c 6974 6520 382e  # pyfuzzylite 8.
-00000010: 302e 320a 0a3c 696d 6720 7372 633d 2268  0.2..<img src="h
-00000020: 7474 7073 3a2f 2f66 757a 7a79 6c69 7465  ttps://fuzzylite
-00000030: 2e67 6974 6875 622e 696f 2f70 7966 757a  .github.io/pyfuz
-00000040: 7a79 6c69 7465 2f69 6d61 6765 2f66 757a  zylite/image/fuz
-00000050: 7a79 6c69 7465 2e73 7667 2220 616c 6967  zylite.svg" alig
-00000060: 6e3d 226c 6566 7422 2061 6c74 3d22 6675  n="left" alt="fu
-00000070: 7a7a 796c 6974 6522 3e0a 0a23 2320 4120  zzylite">..## A 
-00000080: 4675 7a7a 7920 4c6f 6769 6320 436f 6e74  Fuzzy Logic Cont
-00000090: 726f 6c20 4c69 6272 6172 7920 696e 2050  rol Library in P
-000000a0: 7974 686f 6e0a 0a62 7920 5b2a 2a4a 7561  ython..by [**Jua
-000000b0: 6e20 5261 6461 2d56 696c 656c 612c 2050  n Rada-Vilela, P
-000000c0: 6844 2a2a 5d28 6874 7470 733a 2f2f 6675  hD**](https://fu
-000000d0: 7a7a 796c 6974 652e 636f 6d2f 6162 6f75  zzylite.com/abou
-000000e0: 7429 0a0a 3c62 723e 0a3c 6272 3e0a 0a5b  t)..<br>.<br>..[
-000000f0: 215b 4c69 6365 6e73 653a 2047 504c 2076  ![License: GPL v
-00000100: 335d 2868 7474 7073 3a2f 2f69 6d67 2e73  3](https://img.s
-00000110: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000120: 4c69 6365 6e73 652d 4750 4c25 3230 7633  License-GPL%20v3
-00000130: 2d62 6c75 652e 7376 6729 5d28 6874 7470  -blue.svg)](http
-00000140: 733a 2f2f 6f70 656e 736f 7572 6365 2e6f  s://opensource.o
-00000150: 7267 2f6c 6963 656e 7365 2f67 706c 2d33  rg/license/gpl-3
-00000160: 2d30 2f29 0a5b 215b 4c69 6365 6e73 653a  -0/).[![License:
-00000170: 2050 6169 645d 2868 7474 7073 3a2f 2f69   Paid](https://i
-00000180: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000190: 6467 652f 4c69 6365 6e73 652d 7072 6f70  dge/License-prop
-000001a0: 7269 6574 6172 792d 626c 7565 295d 286d  rietary-blue)](m
-000001b0: 6169 6c74 6f3a 7361 6c65 7340 6675 7a7a  ailto:sales@fuzz
-000001c0: 796c 6974 652e 636f 6d29 0a5b 215b 436f  ylite.com).[![Co
-000001d0: 7665 7261 6765 2053 7461 7475 735d 280a  verage Status](.
-000001e0: 6874 7470 733a 2f2f 636f 7665 7261 6c6c  https://coverall
-000001f0: 732e 696f 2f72 6570 6f73 2f67 6974 6875  s.io/repos/githu
-00000200: 622f 6675 7a7a 796c 6974 652f 7079 6675  b/fuzzylite/pyfu
-00000210: 7a7a 796c 6974 652f 6261 6467 652e 7376  zzylite/badge.sv
-00000220: 673f 6272 616e 6368 3d6d 6169 6e29 5d28  g?branch=main)](
-00000230: 0a68 7474 7073 3a2f 2f63 6f76 6572 616c  .https://coveral
-00000240: 6c73 2e69 6f2f 6769 7468 7562 2f66 757a  ls.io/github/fuz
-00000250: 7a79 6c69 7465 2f70 7966 757a 7a79 6c69  zylite/pyfuzzyli
-00000260: 7465 3f62 7261 6e63 683d 6d61 696e 290a  te?branch=main).
-00000270: 5b21 5b42 7569 6c64 5d28 6874 7470 733a  [![Build](https:
-00000280: 2f2f 6769 7468 7562 2e63 6f6d 2f66 757a  //github.com/fuz
-00000290: 7a79 6c69 7465 2f70 7966 757a 7a79 6c69  zylite/pyfuzzyli
-000002a0: 7465 2f61 6374 696f 6e73 2f77 6f72 6b66  te/actions/workf
-000002b0: 6c6f 7773 2f62 7569 6c64 2e79 6d6c 2f62  lows/build.yml/b
-000002c0: 6164 6765 2e73 7667 295d 280a 6874 7470  adge.svg)](.http
-000002d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-000002e0: 757a 7a79 6c69 7465 2f70 7966 757a 7a79  uzzylite/pyfuzzy
-000002f0: 6c69 7465 2f61 6374 696f 6e73 2f77 6f72  lite/actions/wor
-00000300: 6b66 6c6f 7773 2f62 7569 6c64 2e79 6d6c  kflows/build.yml
-00000310: 290a 5b21 5b54 6573 745d 2868 7474 7073  ).[![Test](https
-00000320: 3a2f 2f67 6974 6875 622e 636f 6d2f 6675  ://github.com/fu
-00000330: 7a7a 796c 6974 652f 7079 6675 7a7a 796c  zzylite/pyfuzzyl
-00000340: 6974 652f 6163 7469 6f6e 732f 776f 726b  ite/actions/work
-00000350: 666c 6f77 732f 7465 7374 2e79 6d6c 2f62  flows/test.yml/b
-00000360: 6164 6765 2e73 7667 295d 280a 6874 7470  adge.svg)](.http
-00000370: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-00000380: 757a 7a79 6c69 7465 2f70 7966 757a 7a79  uzzylite/pyfuzzy
-00000390: 6c69 7465 2f61 6374 696f 6e73 2f77 6f72  lite/actions/wor
-000003a0: 6b66 6c6f 7773 2f74 6573 742e 796d 6c29  kflows/test.yml)
-000003b0: 0a5b 215b 5075 626c 6973 685d 2868 7474  .[![Publish](htt
-000003c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000003d0: 6675 7a7a 796c 6974 652f 7079 6675 7a7a  fuzzylite/pyfuzz
-000003e0: 796c 6974 652f 6163 7469 6f6e 732f 776f  ylite/actions/wo
-000003f0: 726b 666c 6f77 732f 7075 626c 6973 682e  rkflows/publish.
-00000400: 796d 6c2f 6261 6467 652e 7376 6729 5d28  yml/badge.svg)](
-00000410: 0a68 7474 7073 3a2f 2f67 6974 6875 622e  .https://github.
-00000420: 636f 6d2f 6675 7a7a 796c 6974 652f 7079  com/fuzzylite/py
-00000430: 6675 7a7a 796c 6974 652f 6163 7469 6f6e  fuzzylite/action
-00000440: 732f 776f 726b 666c 6f77 732f 7075 626c  s/workflows/publ
-00000450: 6973 682e 796d 6c29 0a0a 2323 203c 6120  ish.yml)..## <a 
-00000460: 6e61 6d65 3d22 6675 7a7a 796c 6974 6522  name="fuzzylite"
-00000470: 3e46 757a 7a79 4c69 7465 3c2f 613e 0a0a  >FuzzyLite</a>..
-00000480: 2a2a 5468 6520 4675 7a7a 794c 6974 6520  **The FuzzyLite 
-00000490: 4c69 6272 6172 6965 7320 666f 7220 4675  Libraries for Fu
-000004a0: 7a7a 7920 4c6f 6769 6320 436f 6e74 726f  zzy Logic Contro
-000004b0: 6c2a 2a20 7265 6665 7220 746f 205b 6066  l** refer to [`f
-000004c0: 757a 7a79 6c69 7465 605d 2868 7474 7073  uzzylite`](https
-000004d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6675  ://github.com/fu
-000004e0: 7a7a 796c 6974 652f 6675 7a7a 796c 6974  zzylite/fuzzylit
-000004f0: 652f 290a 2843 2b2b 292c 205b 6070 7966  e/).(C++), [`pyf
-00000500: 757a 7a79 6c69 7465 605d 2868 7474 7073  uzzylite`](https
-00000510: 3a2f 2f67 6974 6875 622e 636f 6d2f 6675  ://github.com/fu
-00000520: 7a7a 796c 6974 652f 7079 6675 7a7a 796c  zzylite/pyfuzzyl
-00000530: 6974 652f 2920 2850 7974 686f 6e29 2c0a  ite/) (Python),.
-00000540: 616e 6420 5b60 6a66 757a 7a79 6c69 7465  and [`jfuzzylite
-00000550: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
-00000560: 622e 636f 6d2f 6675 7a7a 796c 6974 652f  b.com/fuzzylite/
-00000570: 6a66 757a 7a79 6c69 7465 2f29 2028 4a61  jfuzzylite/) (Ja
-00000580: 7661 292e 0a0a 5468 6520 2a2a 676f 616c  va)...The **goal
-00000590: 2a2a 206f 6620 7468 6520 4675 7a7a 794c  ** of the FuzzyL
-000005a0: 6974 6520 4c69 6272 6172 6965 7320 6973  ite Libraries is
-000005b0: 2074 6f20 2a2a 6561 7369 6c79 2a2a 2064   to **easily** d
-000005c0: 6573 6967 6e20 616e 6420 2a2a 6566 6669  esign and **effi
-000005d0: 6369 656e 746c 792a 2a20 6f70 6572 6174  ciently** operat
-000005e0: 6520 6675 7a7a 7920 6c6f 6769 6320 636f  e fuzzy logic co
-000005f0: 6e74 726f 6c6c 6572 730a 666f 6c6c 6f77  ntrollers.follow
-00000600: 696e 6720 616e 202a 2a6f 626a 6563 742d  ing an **object-
-00000610: 6f72 6965 6e74 6564 2a2a 2070 726f 6772  oriented** progr
-00000620: 616d 6d69 6e67 206d 6f64 656c 2077 6974  amming model wit
-00000630: 6820 6d69 6e69 6d61 6c20 6465 7065 6e64  h minimal depend
-00000640: 656e 6379 206f 6e20 6578 7465 726e 616c  ency on external
-00000650: 206c 6962 7261 7269 6573 2e0a 0a23 2320   libraries...## 
-00000660: 3c61 206e 616d 653d 226c 6963 656e 7365  <a name="license
-00000670: 223e 4c69 6365 6e73 653c 2f61 3e0a 0a60  ">License</a>..`
-00000680: 7079 6675 7a7a 796c 6974 6560 2069 7320  pyfuzzylite` is 
-00000690: 6475 616c 2d6c 6963 656e 7365 6420 756e  dual-licensed un
-000006a0: 6465 7220 7468 6520 5b2a 2a47 4e55 2047  der the [**GNU G
-000006b0: 504c 2033 2e30 2a2a 5d28 6874 7470 733a  PL 3.0**](https:
-000006c0: 2f2f 6f70 656e 736f 7572 6365 2e6f 7267  //opensource.org
-000006d0: 2f6c 6963 656e 7365 2f67 706c 2d33 2d30  /license/gpl-3-0
-000006e0: 2f29 2061 6e64 2075 6e64 6572 2061 0a2a  /) and under a.*
-000006f0: 2a70 726f 7072 6965 7461 7279 206c 6963  *proprietary lic
-00000700: 656e 7365 2066 6f72 2063 6f6d 6d65 7263  ense for commerc
-00000710: 6961 6c20 7075 7270 6f73 6573 2a2a 2e0a  ial purposes**..
-00000720: 0a59 6f75 2061 7265 202a 2a73 7472 6f6e  .You are **stron
-00000730: 676c 792a 2a20 656e 636f 7572 6167 6564  gly** encouraged
-00000740: 2074 6f20 7375 7070 6f72 7420 7468 6520   to support the 
-00000750: 6465 7665 6c6f 706d 656e 7420 6f66 2074  development of t
-00000760: 6865 2046 757a 7a79 4c69 7465 204c 6962  he FuzzyLite Lib
-00000770: 7261 7269 6573 2062 7920 7075 7263 6861  raries by purcha
-00000780: 7369 6e67 2061 206c 6963 656e 7365 0a6f  sing a license.o
-00000790: 6620 5b60 5174 4675 7a7a 794c 6974 6560  f [`QtFuzzyLite`
-000007a0: 5d28 6874 7470 733a 2f2f 6675 7a7a 796c  ](https://fuzzyl
-000007b0: 6974 652e 636f 6d2f 646f 776e 6c6f 6164  ite.com/download
-000007c0: 7329 2e0a 0a5b 6051 7446 757a 7a79 4c69  s)...[`QtFuzzyLi
-000007d0: 7465 605d 2868 7474 7073 3a2f 2f66 757a  te`](https://fuz
-000007e0: 7a79 6c69 7465 2e63 6f6d 2f64 6f77 6e6c  zylite.com/downl
-000007f0: 6f61 6473 2f29 2069 7320 7468 6520 6265  oads/) is the be
-00000800: 7374 2067 7261 7068 6963 616c 2075 7365  st graphical use
-00000810: 7220 696e 7465 7266 6163 6520 6176 6169  r interface avai
-00000820: 6c61 626c 6520 746f 2065 6173 696c 7920  lable to easily 
-00000830: 6465 7369 676e 2061 6e64 0a64 6972 6563  design and.direc
-00000840: 746c 7920 6f70 6572 6174 6520 6675 7a7a  tly operate fuzz
-00000850: 7920 6c6f 6769 6320 636f 6e74 726f 6c6c  y logic controll
-00000860: 6572 7320 696e 2072 6561 6c20 7469 6d65  ers in real time
-00000870: 2e20 4176 6169 6c61 626c 6520 666f 7220  . Available for 
-00000880: 5769 6e64 6f77 732c 204d 6163 2c20 616e  Windows, Mac, an
-00000890: 6420 4c69 6e75 782c 2069 7473 2067 6f61  d Linux, its goa
-000008a0: 6c20 6973 2074 6f0a 7369 676e 6966 6963  l is to.signific
-000008b0: 616e 746c 7920 2a2a 7370 6565 6420 7570  antly **speed up
-000008c0: 2a2a 2074 6865 2064 6573 6967 6e20 6f66  ** the design of
-000008d0: 2079 6f75 7220 6675 7a7a 7920 6c6f 6769   your fuzzy logi
-000008e0: 6320 636f 6e74 726f 6c6c 6572 732c 2077  c controllers, w
-000008f0: 6869 6c65 2070 726f 7669 6469 6e67 2061  hile providing a
-00000900: 2076 6572 7920 2a2a 7573 6566 756c 2a2a   very **useful**
-00000910: 2c20 2a2a 6675 6e63 7469 6f6e 616c 2a2a  , **functional**
-00000920: 0a61 6e64 202a 2a62 6561 7574 6966 756c  .and **beautiful
-00000930: 2a2a 2075 7365 7220 696e 7465 7266 6163  ** user interfac
-00000940: 652e 0a50 6c65 6173 652c 2064 6f77 6e6c  e..Please, downl
-00000950: 6f61 6420 6974 2061 6e64 2063 6865 636b  oad it and check
-00000960: 2069 7420 6f75 7420 666f 7220 6672 6565   it out for free
-00000970: 2061 7420 5b66 757a 7a79 6c69 7465 2e63   at [fuzzylite.c
-00000980: 6f6d 2f64 6f77 6e6c 6f61 6473 5d28 6874  om/downloads](ht
-00000990: 7470 733a 2f2f 6675 7a7a 796c 6974 652e  tps://fuzzylite.
-000009a0: 636f 6d2f 646f 776e 6c6f 6164 7329 2e0a  com/downloads)..
-000009b0: 0a23 2320 3c61 206e 616d 653d 2269 6e73  .## <a name="ins
-000009c0: 7461 6c6c 223e 496e 7374 616c 6c3c 2f61  tall">Install</a
-000009d0: 3e0a 0a60 6060 636f 6d6d 616e 646c 696e  >..```commandlin
-000009e0: 650a 7069 7020 696e 7374 616c 6c20 7079  e.pip install py
-000009f0: 6675 7a7a 796c 6974 650a 6060 600a 0a23  fuzzylite.```..#
-00000a00: 2320 3c61 206e 616d 653d 2266 6561 7475  # <a name="featu
-00000a10: 7265 7322 3e46 6561 7475 7265 733c 2f61  res">Features</a
-00000a20: 3e0a 0a2a 2a44 6f63 756d 656e 7461 7469  >..**Documentati
-00000a30: 6f6e 2a2a 3a20 5b66 757a 7a79 6c69 7465  on**: [fuzzylite
-00000a40: 2e67 6974 6875 622e 696f 2f70 7966 757a  .github.io/pyfuz
-00000a50: 7a79 6c69 7465 2f5d 2868 7474 7073 3a2f  zylite/](https:/
-00000a60: 2f66 757a 7a79 6c69 7465 2e67 6974 6875  /fuzzylite.githu
-00000a70: 622e 696f 2f70 7966 757a 7a79 6c69 7465  b.io/pyfuzzylite
-00000a80: 2f29 0a0a 2a2a 2836 2920 436f 6e74 726f  /)..**(6) Contro
-00000a90: 6c6c 6572 732a 2a3a 204d 616d 6461 6e69  llers**: Mamdani
-00000aa0: 2c20 5461 6b61 6769 2d53 7567 656e 6f2c  , Takagi-Sugeno,
-00000ab0: 204c 6172 7365 6e2c 2054 7375 6b61 6d6f   Larsen, Tsukamo
-00000ac0: 746f 2c20 496e 7665 7273 6520 5473 756b  to, Inverse Tsuk
-00000ad0: 616d 6f74 6f2c 2048 7962 7269 640a 0a2a  amoto, Hybrid..*
-00000ae0: 2a28 3235 2920 4c69 6e67 7569 7374 6963  *(25) Linguistic
-00000af0: 2074 6572 6d73 2a2a 3a20 2028 3529 202a   terms**:  (5) *
-00000b00: 4261 7369 632a 3a20 5472 6961 6e67 6c65  Basic*: Triangle
-00000b10: 2c20 5472 6170 657a 6f69 642c 2052 6563  , Trapezoid, Rec
-00000b20: 7461 6e67 6c65 2c20 4469 7363 7265 7465  tangle, Discrete
-00000b30: 2c20 5365 6d69 456c 6c69 7073 652e 0a28  , SemiEllipse..(
-00000b40: 3829 202a 4578 7465 6e64 6564 2a3a 2042  8) *Extended*: B
-00000b50: 656c 6c2c 2043 6f73 696e 652c 2047 6175  ell, Cosine, Gau
-00000b60: 7373 6961 6e2c 2047 6175 7373 6961 6e50  ssian, GaussianP
-00000b70: 726f 6475 6374 2c20 5069 5368 6170 652c  roduct, PiShape,
-00000b80: 2053 6967 6d6f 6964 4469 6666 6572 656e   SigmoidDifferen
-00000b90: 6365 2c20 5369 676d 6f69 6450 726f 6475  ce, SigmoidProdu
-00000ba0: 6374 2c20 5370 696b 652e 0a28 3729 202a  ct, Spike..(7) *
-00000bb0: 4564 6765 732a 3a20 4172 632c 2042 696e  Edges*: Arc, Bin
-00000bc0: 6172 792c 2043 6f6e 6361 7665 2c20 5261  ary, Concave, Ra
-00000bd0: 6d70 2c20 5369 676d 6f69 642c 2053 5368  mp, Sigmoid, SSh
-00000be0: 6170 652c 205a 5368 6170 652e 0a28 3329  ape, ZShape..(3)
-00000bf0: 202a 4675 6e63 7469 6f6e 732a 3a20 436f   *Functions*: Co
-00000c00: 6e73 7461 6e74 2c20 4c69 6e65 6172 2c20  nstant, Linear, 
-00000c10: 4675 6e63 7469 6f6e 2e20 2832 2920 2a53  Function. (2) *S
-00000c20: 7065 6369 616c 2a3a 2041 6767 7265 6761  pecial*: Aggrega
-00000c30: 7465 642c 2041 6374 6976 6174 6564 2e0a  ted, Activated..
-00000c40: 0a2a 2a28 3729 2041 6374 6976 6174 696f  .**(7) Activatio
-00000c50: 6e20 6d65 7468 6f64 732a 2a3a 2020 4765  n methods**:  Ge
-00000c60: 6e65 7261 6c2c 2050 726f 706f 7274 696f  neral, Proportio
-00000c70: 6e61 6c2c 2054 6872 6573 686f 6c64 2c20  nal, Threshold, 
-00000c80: 4669 7273 742c 204c 6173 742c 204c 6f77  First, Last, Low
-00000c90: 6573 742c 2048 6967 6865 7374 2e0a 0a2a  est, Highest...*
-00000ca0: 2a28 3929 2043 6f6e 6a75 6e63 7469 6f6e  *(9) Conjunction
-00000cb0: 2061 6e64 2049 6d70 6c69 6361 7469 6f6e   and Implication
-00000cc0: 2028 542d 4e6f 726d 7329 2a2a 3a20 4d69   (T-Norms)**: Mi
-00000cd0: 6e69 6d75 6d2c 2041 6c67 6562 7261 6963  nimum, Algebraic
-00000ce0: 5072 6f64 7563 742c 2042 6f75 6e64 6564  Product, Bounded
-00000cf0: 4469 6666 6572 656e 6365 2c20 4472 6173  Difference, Dras
-00000d00: 7469 6350 726f 6475 6374 2c0a 4569 6e73  ticProduct,.Eins
-00000d10: 7465 696e 5072 6f64 7563 742c 2048 616d  teinProduct, Ham
-00000d20: 6163 6865 7250 726f 6475 6374 2c20 4e69  acherProduct, Ni
-00000d30: 6c70 6f74 656e 744d 696e 696d 756d 2c20  lpotentMinimum, 
-00000d40: 4c61 6d62 6461 4e6f 726d 2c20 4675 6e63  LambdaNorm, Func
-00000d50: 7469 6f6e 4e6f 726d 2e0a 0a2a 2a28 3131  tionNorm...**(11
-00000d60: 2920 4469 736a 756e 6374 696f 6e20 616e  ) Disjunction an
-00000d70: 6420 4167 6772 6567 6174 696f 6e20 2853  d Aggregation (S
-00000d80: 2d4e 6f72 6d73 292a 2a3a 2020 4d61 7869  -Norms)**:  Maxi
-00000d90: 6d75 6d2c 2041 6c67 6562 7261 6963 5375  mum, AlgebraicSu
-00000da0: 6d2c 2042 6f75 6e64 6564 5375 6d2c 2044  m, BoundedSum, D
-00000db0: 7261 7374 6963 5375 6d2c 2045 696e 7374  rasticSum, Einst
-00000dc0: 6569 6e53 756d 2c0a 4861 6d61 6368 6572  einSum,.Hamacher
-00000dd0: 5375 6d2c 204e 696c 706f 7465 6e74 4d61  Sum, NilpotentMa
-00000de0: 7869 6d75 6d2c 204e 6f72 6d61 6c69 7a65  ximum, Normalize
-00000df0: 6453 756d 2c20 556e 626f 756e 6465 6453  dSum, UnboundedS
-00000e00: 756d 2c20 4c61 6d62 6461 4e6f 726d 2c20  um, LambdaNorm, 
-00000e10: 4675 6e63 7469 6f6e 4e6f 726d 2e0a 0a2a  FunctionNorm...*
-00000e20: 2a28 3729 2044 6566 757a 7a69 6669 6572  *(7) Defuzzifier
-00000e30: 732a 2a3a 2020 2835 2920 2a49 6e74 6567  s**:  (5) *Integ
-00000e40: 7261 6c2a 3a20 4365 6e74 726f 6964 2c20  ral*: Centroid, 
-00000e50: 4269 7365 6374 6f72 2c20 536d 616c 6c65  Bisector, Smalle
-00000e60: 7374 4f66 4d61 7869 6d75 6d2c 204c 6172  stOfMaximum, Lar
-00000e70: 6765 7374 4f66 4d61 7869 6d75 6d2c 204d  gestOfMaximum, M
-00000e80: 6561 6e4f 664d 6178 696d 756d 2e0a 2832  eanOfMaximum..(2
-00000e90: 2920 2a57 6569 6768 7465 642a 3a20 5765  ) *Weighted*: We
-00000ea0: 6967 6874 6564 4176 6572 6167 652c 2057  ightedAverage, W
-00000eb0: 6569 6768 7465 6453 756d 2e0a 0a2a 2a28  eightedSum...**(
-00000ec0: 3729 2048 6564 6765 732a 2a3a 2041 6e79  7) Hedges**: Any
-00000ed0: 2c20 4e6f 742c 2045 7874 7265 6d65 6c79  , Not, Extremely
-00000ee0: 2c20 5365 6c64 6f6d 2c20 536f 6d65 7768  , Seldom, Somewh
-00000ef0: 6174 2c20 5665 7279 2c20 4675 6e63 7469  at, Very, Functi
-00000f00: 6f6e 2e0a 0a2a 2a28 3329 2049 6d70 6f72  on...**(3) Impor
-00000f10: 7465 7273 2a2a 3a20 4675 7a7a 794c 6974  ters**: FuzzyLit
-00000f20: 6520 4c61 6e67 7561 6765 2060 666c 6c60  e Language `fll`
-00000f30: 2e20 5769 7468 2060 6675 7a7a 796c 6974  . With `fuzzylit
-00000f40: 6560 3a20 4675 7a7a 7920 496e 6665 7265  e`: Fuzzy Infere
-00000f50: 6e63 6520 5379 7374 656d 2060 6669 7360  nce System `fis`
-00000f60: 2c20 4675 7a7a 7920 436f 6e74 726f 6c0a  , Fuzzy Control.
-00000f70: 4c61 6e67 7561 6765 2060 6663 6c60 2e0a  Language `fcl`..
-00000f80: 0a2a 2a28 3729 2045 7870 6f72 7465 7273  .**(7) Exporters
-00000f90: 2a2a 3a20 6050 7974 686f 6e60 2c20 4675  **: `Python`, Fu
-00000fa0: 7a7a 794c 6974 6520 4c61 6e67 7561 6765  zzyLite Language
-00000fb0: 2060 666c 6c60 2c20 4675 7a7a 794c 6974   `fll`, FuzzyLit
-00000fc0: 6520 4461 7461 7365 7420 6066 6c64 602e  e Dataset `fld`.
-00000fd0: 2057 6974 6820 6066 757a 7a79 6c69 7465   With `fuzzylite
-00000fe0: 603a 2060 432b 2b60 2c20 604a 6176 6160  `: `C++`, `Java`
-00000ff0: 2c0a 4675 7a7a 794c 6974 6520 4c61 6e67  ,.FuzzyLite Lang
-00001000: 7561 6765 2060 666c 6c60 2c20 4675 7a7a  uage `fll`, Fuzz
-00001010: 794c 6974 6520 4461 7461 7365 7420 6066  yLite Dataset `f
-00001020: 6c64 602c 2060 5260 2073 6372 6970 742c  ld`, `R` script,
-00001030: 2046 757a 7a79 2049 6e66 6572 656e 6365   Fuzzy Inference
-00001040: 2053 7973 7465 6d20 6066 6973 602c 2046   System `fis`, F
-00001050: 757a 7a79 2043 6f6e 7472 6f6c 0a4c 616e  uzzy Control.Lan
-00001060: 6775 6167 6520 6066 636c 602e 0a0a 2a2a  guage `fcl`...**
-00001070: 2833 302b 2920 4578 616d 706c 6573 2a2a  (30+) Examples**
-00001080: 2020 6f66 204d 616d 6461 6e69 2c20 5461    of Mamdani, Ta
-00001090: 6b61 6769 2d53 7567 656e 6f2c 2054 7375  kagi-Sugeno, Tsu
-000010a0: 6b61 6d6f 746f 2c20 616e 6420 4879 6272  kamoto, and Hybr
-000010b0: 6964 2063 6f6e 7472 6f6c 6c65 7273 2066  id controllers f
-000010c0: 726f 6d20 6066 757a 7a79 6c69 7465 602c  rom `fuzzylite`,
-000010d0: 204f 6374 6176 652c 2061 6e64 204d 6174   Octave, and Mat
-000010e0: 6c61 622c 0a65 6163 6820 696e 636c 7564  lab,.each includ
-000010f0: 6564 2069 6e20 7468 6520 666f 6c6c 6f77  ed in the follow
-00001100: 696e 6720 666f 726d 6174 733a 2060 7079  ing formats: `py
-00001110: 602c 2060 666c 6c60 2c20 6066 6c64 602e  `, `fll`, `fld`.
-00001120: 2057 6974 6820 6066 757a 7a79 6c69 7465   With `fuzzylite
-00001130: 603a 2060 432b 2b60 2c20 604a 6176 6160  `: `C++`, `Java`
-00001140: 2c20 6052 602c 2060 6669 7360 2c20 616e  , `R`, `fis`, an
-00001150: 6420 6066 636c 602e 0a0a 2323 203c 6120  d `fcl`...## <a 
-00001160: 6e61 6d65 3d22 6578 616d 706c 6573 223e  name="examples">
-00001170: 4578 616d 706c 6573 3c2f 613e 0a0a 2323  Examples</a>..##
-00001180: 2320 4675 7a7a 794c 6974 6520 4c61 6e67  # FuzzyLite Lang
-00001190: 7561 6765 0a0a 6060 6079 616d 6c0a 2320  uage..```yaml.# 
-000011a0: 4669 6c65 3a20 6578 616d 706c 6573 2f6d  File: examples/m
-000011b0: 616d 6461 6e69 2f4f 6273 7461 636c 6541  amdani/ObstacleA
-000011c0: 766f 6964 616e 6365 2e66 6c6c 0a45 6e67  voidance.fll.Eng
-000011d0: 696e 653a 204f 6273 7461 636c 6541 766f  ine: ObstacleAvo
-000011e0: 6964 616e 6365 0a49 6e70 7574 5661 7269  idance.InputVari
-000011f0: 6162 6c65 3a20 6f62 7374 6163 6c65 0a20  able: obstacle. 
-00001200: 2065 6e61 626c 6564 3a20 7472 7565 0a20   enabled: true. 
-00001210: 2072 616e 6765 3a20 302e 3030 3020 312e   range: 0.000 1.
-00001220: 3030 300a 2020 6c6f 636b 2d72 616e 6765  000.  lock-range
-00001230: 3a20 6661 6c73 650a 2020 7465 726d 3a20  : false.  term: 
-00001240: 6c65 6674 2052 616d 7020 312e 3030 3020  left Ramp 1.000 
-00001250: 302e 3030 300a 2020 7465 726d 3a20 7269  0.000.  term: ri
-00001260: 6768 7420 5261 6d70 2030 2e30 3030 2031  ght Ramp 0.000 1
-00001270: 2e30 3030 0a4f 7574 7075 7456 6172 6961  .000.OutputVaria
-00001280: 626c 653a 206d 5374 6565 720a 2020 656e  ble: mSteer.  en
-00001290: 6162 6c65 643a 2074 7275 650a 2020 7261  abled: true.  ra
-000012a0: 6e67 653a 2030 2e30 3030 2031 2e30 3030  nge: 0.000 1.000
-000012b0: 0a20 206c 6f63 6b2d 7261 6e67 653a 2066  .  lock-range: f
-000012c0: 616c 7365 0a20 2061 6767 7265 6761 7469  alse.  aggregati
-000012d0: 6f6e 3a20 4d61 7869 6d75 6d0a 2020 6465  on: Maximum.  de
-000012e0: 6675 7a7a 6966 6965 723a 2043 656e 7472  fuzzifier: Centr
-000012f0: 6f69 6420 3130 300a 2020 6465 6661 756c  oid 100.  defaul
-00001300: 743a 206e 616e 0a20 206c 6f63 6b2d 7072  t: nan.  lock-pr
-00001310: 6576 696f 7573 3a20 6661 6c73 650a 2020  evious: false.  
-00001320: 7465 726d 3a20 6c65 6674 2052 616d 7020  term: left Ramp 
-00001330: 312e 3030 3020 302e 3030 300a 2020 7465  1.000 0.000.  te
-00001340: 726d 3a20 7269 6768 7420 5261 6d70 2030  rm: right Ramp 0
-00001350: 2e30 3030 2031 2e30 3030 0a52 756c 6542  .000 1.000.RuleB
-00001360: 6c6f 636b 3a20 6d61 6d64 616e 690a 2020  lock: mamdani.  
-00001370: 656e 6162 6c65 643a 2074 7275 650a 2020  enabled: true.  
-00001380: 636f 6e6a 756e 6374 696f 6e3a 206e 6f6e  conjunction: non
-00001390: 650a 2020 6469 736a 756e 6374 696f 6e3a  e.  disjunction:
-000013a0: 206e 6f6e 650a 2020 696d 706c 6963 6174   none.  implicat
-000013b0: 696f 6e3a 2041 6c67 6562 7261 6963 5072  ion: AlgebraicPr
-000013c0: 6f64 7563 740a 2020 6163 7469 7661 7469  oduct.  activati
-000013d0: 6f6e 3a20 4765 6e65 7261 6c0a 2020 7275  on: General.  ru
-000013e0: 6c65 3a20 6966 206f 6273 7461 636c 6520  le: if obstacle 
-000013f0: 6973 206c 6566 7420 7468 656e 206d 5374  is left then mSt
-00001400: 6565 7220 6973 2072 6967 6874 0a20 2072  eer is right.  r
-00001410: 756c 653a 2069 6620 6f62 7374 6163 6c65  ule: if obstacle
-00001420: 2069 7320 7269 6768 7420 7468 656e 206d   is right then m
-00001430: 5374 6565 7220 6973 206c 6566 740a 6060  Steer is left.``
-00001440: 600a 0a60 6060 7079 7468 6f6e 0a23 2050  `..```python.# P
-00001450: 7974 686f 6e0a 696d 706f 7274 2066 757a  ython.import fuz
-00001460: 7a79 6c69 7465 2061 7320 666c 0a0a 656e  zylite as fl..en
-00001470: 6769 6e65 203d 2066 6c2e 466c 6c49 6d70  gine = fl.FllImp
-00001480: 6f72 7465 7228 292e 6672 6f6d 5f66 696c  orter().from_fil
-00001490: 6528 2265 7861 6d70 6c65 732f 6d61 6d64  e("examples/mamd
-000014a0: 616e 692f 4f62 7374 6163 6c65 4176 6f69  ani/ObstacleAvoi
-000014b0: 6461 6e63 652e 666c 6c22 290a 6060 600a  dance.fll").```.
-000014c0: 0a23 2323 2050 7974 686f 6e0a 0a60 6060  .### Python..```
-000014d0: 7079 7468 6f6e 0a69 6d70 6f72 7420 6675  python.import fu
-000014e0: 7a7a 796c 6974 6520 6173 2066 6c0a 0a65  zzylite as fl..e
-000014f0: 6e67 696e 6520 3d20 666c 2e45 6e67 696e  ngine = fl.Engin
-00001500: 6528 0a20 2020 206e 616d 653d 224f 6273  e(.    name="Obs
-00001510: 7461 636c 6541 766f 6964 616e 6365 222c  tacleAvoidance",
-00001520: 0a20 2020 2069 6e70 7574 5f76 6172 6961  .    input_varia
-00001530: 626c 6573 3d5b 0a20 2020 2020 2020 2066  bles=[.        f
-00001540: 6c2e 496e 7075 7456 6172 6961 626c 6528  l.InputVariable(
-00001550: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-00001560: 653d 226f 6273 7461 636c 6522 2c0a 2020  e="obstacle",.  
-00001570: 2020 2020 2020 2020 2020 6d69 6e69 6d75            minimu
-00001580: 6d3d 302e 302c 0a20 2020 2020 2020 2020  m=0.0,.         
-00001590: 2020 206d 6178 696d 756d 3d31 2e30 2c0a     maximum=1.0,.
-000015a0: 2020 2020 2020 2020 2020 2020 6c6f 636b              lock
-000015b0: 5f72 616e 6765 3d46 616c 7365 2c0a 2020  _range=False,.  
-000015c0: 2020 2020 2020 2020 2020 7465 726d 733d            terms=
-000015d0: 5b66 6c2e 5261 6d70 2822 6c65 6674 222c  [fl.Ramp("left",
-000015e0: 2031 2e30 2c20 302e 3029 2c20 666c 2e52   1.0, 0.0), fl.R
-000015f0: 616d 7028 2272 6967 6874 222c 2030 2e30  amp("right", 0.0
-00001600: 2c20 312e 3029 5d2c 0a20 2020 2020 2020  , 1.0)],.       
-00001610: 2029 0a20 2020 205d 2c0a 2020 2020 6f75   ).    ],.    ou
-00001620: 7470 7574 5f76 6172 6961 626c 6573 3d5b  tput_variables=[
-00001630: 0a20 2020 2020 2020 2066 6c2e 4f75 7470  .        fl.Outp
-00001640: 7574 5661 7269 6162 6c65 280a 2020 2020  utVariable(.    
-00001650: 2020 2020 2020 2020 6e61 6d65 3d22 6d53          name="mS
-00001660: 7465 6572 222c 0a20 2020 2020 2020 2020  teer",.         
-00001670: 2020 206d 696e 696d 756d 3d30 2e30 2c0a     minimum=0.0,.
-00001680: 2020 2020 2020 2020 2020 2020 6d61 7869              maxi
-00001690: 6d75 6d3d 312e 302c 0a20 2020 2020 2020  mum=1.0,.       
-000016a0: 2020 2020 206c 6f63 6b5f 7261 6e67 653d       lock_range=
-000016b0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-000016c0: 2020 206c 6f63 6b5f 7072 6576 696f 7573     lock_previous
-000016d0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-000016e0: 2020 2020 6465 6661 756c 745f 7661 6c75      default_valu
-000016f0: 653d 666c 2e6e 616e 2c0a 2020 2020 2020  e=fl.nan,.      
-00001700: 2020 2020 2020 6167 6772 6567 6174 696f        aggregatio
-00001710: 6e3d 666c 2e4d 6178 696d 756d 2829 2c0a  n=fl.Maximum(),.
-00001720: 2020 2020 2020 2020 2020 2020 6465 6675              defu
-00001730: 7a7a 6966 6965 723d 666c 2e43 656e 7472  zzifier=fl.Centr
-00001740: 6f69 6428 7265 736f 6c75 7469 6f6e 3d31  oid(resolution=1
-00001750: 3030 292c 0a20 2020 2020 2020 2020 2020  00),.           
-00001760: 2074 6572 6d73 3d5b 666c 2e52 616d 7028   terms=[fl.Ramp(
-00001770: 226c 6566 7422 2c20 312e 302c 2030 2e30  "left", 1.0, 0.0
-00001780: 292c 2066 6c2e 5261 6d70 2822 7269 6768  ), fl.Ramp("righ
-00001790: 7422 2c20 302e 302c 2031 2e30 295d 2c0a  t", 0.0, 1.0)],.
-000017a0: 2020 2020 2020 2020 290a 2020 2020 5d2c          ).    ],
-000017b0: 0a20 2020 2072 756c 655f 626c 6f63 6b73  .    rule_blocks
-000017c0: 3d5b 0a20 2020 2020 2020 2066 6c2e 5275  =[.        fl.Ru
-000017d0: 6c65 426c 6f63 6b28 0a20 2020 2020 2020  leBlock(.       
-000017e0: 2020 2020 206e 616d 653d 226d 616d 6461       name="mamda
-000017f0: 6e69 222c 0a20 2020 2020 2020 2020 2020  ni",.           
-00001800: 2063 6f6e 6a75 6e63 7469 6f6e 3d4e 6f6e   conjunction=Non
-00001810: 652c 0a20 2020 2020 2020 2020 2020 2064  e,.            d
-00001820: 6973 6a75 6e63 7469 6f6e 3d4e 6f6e 652c  isjunction=None,
-00001830: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
-00001840: 6c69 6361 7469 6f6e 3d66 6c2e 416c 6765  lication=fl.Alge
-00001850: 6272 6169 6350 726f 6475 6374 2829 2c0a  braicProduct(),.
-00001860: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-00001870: 7661 7469 6f6e 3d66 6c2e 4765 6e65 7261  vation=fl.Genera
-00001880: 6c28 292c 0a20 2020 2020 2020 2020 2020  l(),.           
-00001890: 2072 756c 6573 3d5b 0a20 2020 2020 2020   rules=[.       
-000018a0: 2020 2020 2020 2020 2066 6c2e 5275 6c65           fl.Rule
-000018b0: 2e63 7265 6174 6528 2269 6620 6f62 7374  .create("if obst
-000018c0: 6163 6c65 2069 7320 6c65 6674 2074 6865  acle is left the
-000018d0: 6e20 6d53 7465 6572 2069 7320 7269 6768  n mSteer is righ
-000018e0: 7422 292c 0a20 2020 2020 2020 2020 2020  t"),.           
-000018f0: 2020 2020 2066 6c2e 5275 6c65 2e63 7265       fl.Rule.cre
-00001900: 6174 6528 2269 6620 6f62 7374 6163 6c65  ate("if obstacle
-00001910: 2069 7320 7269 6768 7420 7468 656e 206d   is right then m
-00001920: 5374 6565 7220 6973 206c 6566 7422 292c  Steer is left"),
-00001930: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
-00001940: 2020 2020 2020 2020 290a 2020 2020 5d2c          ).    ],
-00001950: 0a29 0a60 6060 0a0a 2323 2320 6066 6c6f  .).```..### `flo
-00001960: 6174 6020 616e 6420 7665 6374 6f72 697a  at` and vectoriz
-00001970: 6174 696f 6e0a 0a60 6060 7079 7468 6f6e  ation..```python
-00001980: 0a23 2073 696e 676c 6520 6066 6c6f 6174  .# single `float
-00001990: 6020 6f70 6572 6174 696f 6e0a 656e 6769  ` operation.engi
-000019a0: 6e65 2e69 6e70 7574 5f76 6172 6961 626c  ne.input_variabl
-000019b0: 6528 226f 6273 7461 636c 6522 292e 7661  e("obstacle").va
-000019c0: 6c75 6520 3d20 302e 350a 656e 6769 6e65  lue = 0.5.engine
-000019d0: 2e70 726f 6365 7373 2829 0a70 7269 6e74  .process().print
-000019e0: 2822 7920 3d22 2c20 656e 6769 6e65 2e6f  ("y =", engine.o
-000019f0: 7574 7075 745f 7661 7269 6162 6c65 2822  utput_variable("
-00001a00: 6d53 7465 6572 2229 2e76 616c 7565 290a  mSteer").value).
-00001a10: 2320 3e20 7920 3d20 302e 350a 7072 696e  # > y = 0.5.prin
-00001a20: 7428 22e1 bbb9 203d 222c 2065 6e67 696e  t("... =", engin
-00001a30: 652e 6f75 7470 7574 5f76 6172 6961 626c  e.output_variabl
-00001a40: 6528 226d 5374 6565 7222 292e 6675 7a7a  e("mSteer").fuzz
-00001a50: 795f 7661 6c75 6528 2929 0a23 203e 20e1  y_value()).# > .
-00001a60: bbb9 203d 2030 2e35 3030 2f6c 6566 7420  .. = 0.500/left 
-00001a70: 2b20 302e 3530 302f 7269 6768 740a 0a23  + 0.500/right..#
-00001a80: 2076 6563 746f 7269 7a61 7469 6f6e 0a65   vectorization.e
-00001a90: 6e67 696e 652e 696e 7075 745f 7661 7269  ngine.input_vari
-00001aa0: 6162 6c65 2822 6f62 7374 6163 6c65 2229  able("obstacle")
-00001ab0: 2e76 616c 7565 203d 2066 6c2e 6172 7261  .value = fl.arra
-00001ac0: 7928 5b30 2c20 302e 3235 2c20 302e 352c  y([0, 0.25, 0.5,
-00001ad0: 2030 2e37 352c 2031 2e30 5d29 0a65 6e67   0.75, 1.0]).eng
-00001ae0: 696e 652e 7072 6f63 6573 7328 290a 7072  ine.process().pr
-00001af0: 696e 7428 2279 203d 222c 2072 6570 7228  int("y =", repr(
-00001b00: 656e 6769 6e65 2e6f 7574 7075 745f 7661  engine.output_va
-00001b10: 7269 6162 6c65 2822 6d53 7465 6572 2229  riable("mSteer")
-00001b20: 2e76 616c 7565 2929 0a23 203e 2079 203d  .value)).# > y =
-00001b30: 2061 7272 6179 285b 302e 3636 3636 3636   array([0.666666
-00001b40: 3520 2c20 302e 3632 3137 3934 3737 2c20  5 , 0.62179477, 
-00001b50: 302e 3520 2020 2020 2020 2c20 302e 3337  0.5       , 0.37
-00001b60: 3832 3035 3233 2c20 302e 3333 3333 3333  820523, 0.333333
-00001b70: 3520 5d29 0a70 7269 6e74 2822 e1bb b920  5 ]).print("... 
-00001b80: 3d22 2c20 7265 7072 2865 6e67 696e 652e  =", repr(engine.
-00001b90: 6f75 7470 7574 5f76 6172 6961 626c 6528  output_variable(
-00001ba0: 226d 5374 6565 7222 292e 6675 7a7a 795f  "mSteer").fuzzy_
-00001bb0: 7661 6c75 6528 2929 290a 2320 3e20 e1bb  value())).# > ..
-00001bc0: b920 3d20 6172 7261 7928 5b27 302e 3030  . = array(['0.00
-00001bd0: 302f 6c65 6674 202b 2031 2e30 3030 2f72  0/left + 1.000/r
-00001be0: 6967 6874 272c 0a23 2020 2020 2020 2020  ight',.#        
-00001bf0: 2020 2020 2020 2730 2e32 3530 2f6c 6566        '0.250/lef
-00001c00: 7420 2b20 302e 3735 302f 7269 6768 7427  t + 0.750/right'
-00001c10: 2c0a 2320 2020 2020 2020 2020 2020 2020  ,.#             
-00001c20: 2027 302e 3530 302f 6c65 6674 202b 2030   '0.500/left + 0
-00001c30: 2e35 3030 2f72 6967 6874 272c 0a23 2020  .500/right',.#  
-00001c40: 2020 2020 2020 2020 2020 2020 2730 2e37              '0.7
-00001c50: 3530 2f6c 6566 7420 2b20 302e 3235 302f  50/left + 0.250/
-00001c60: 7269 6768 7427 2c0a 2320 2020 2020 2020  right',.#       
-00001c70: 2020 2020 2020 2027 312e 3030 302f 6c65         '1.000/le
-00001c80: 6674 202b 2030 2e30 3030 2f72 6967 6874  ft + 0.000/right
-00001c90: 275d 2c20 6474 7970 653d 273c 5532 3627  '], dtype='<U26'
-00001ca0: 290a 6060 600a 0a50 6c65 6173 6520 7265  ).```..Please re
-00001cb0: 6665 7220 746f 2074 6865 2064 6f63 756d  fer to the docum
-00001cc0: 656e 7461 7469 6f6e 2066 6f72 206d 6f72  entation for mor
-00001cd0: 650a 696e 666f 726d 6174 696f 6e3a 205b  e.information: [
-00001ce0: 2a2a 6675 7a7a 796c 6974 652e 6769 7468  **fuzzylite.gith
-00001cf0: 7562 2e69 6f2f 7079 6675 7a7a 796c 6974  ub.io/pyfuzzylit
-00001d00: 652f 2a2a 5d28 6874 7470 733a 2f2f 6675  e/**](https://fu
-00001d10: 7a7a 796c 6974 652e 6769 7468 7562 2e69  zzylite.github.i
-00001d20: 6f2f 7079 6675 7a7a 796c 6974 652f 290a  o/pyfuzzylite/).
-00001d30: 0a23 2320 3c61 206e 616d 653d 2263 6f6e  .## <a name="con
-00001d40: 7472 6962 7574 696e 6722 3e43 6f6e 7472  tributing">Contr
-00001d50: 6962 7574 696e 673c 2f61 3e0a 0a41 6c6c  ibuting</a>..All
-00001d60: 2063 6f6e 7472 6962 7574 696f 6e73 2061   contributions a
-00001d70: 7265 2077 656c 636f 6d65 2c20 7072 6f76  re welcome, prov
-00001d80: 6964 6564 2074 6865 7920 666f 6c6c 6f77  ided they follow
-00001d90: 2074 6865 2066 6f6c 6c6f 7769 6e67 2067   the following g
-00001da0: 7569 6465 6c69 6e65 733a 0a0a 2d20 536f  uidelines:..- So
-00001db0: 7572 6365 2063 6f64 6520 6973 2063 6f6e  urce code is con
-00001dc0: 7369 7374 656e 7420 7769 7468 2073 7461  sistent with sta
-00001dd0: 6e64 6172 6473 2069 6e20 7468 6520 6c69  ndards in the li
-00001de0: 6272 6172 790a 2d20 436f 6e74 7269 6275  brary.- Contribu
-00001df0: 7469 6f6e 2069 7320 7072 6f70 6572 6c79  tion is properly
-00001e00: 2064 6f63 756d 656e 7465 6420 616e 6420   documented and 
-00001e10: 7465 7374 6564 2c20 7261 6973 696e 6720  tested, raising 
-00001e20: 6973 7375 6573 2077 6865 7265 2061 7070  issues where app
-00001e30: 726f 7072 6961 7465 0a2d 2043 6f6e 7472  ropriate.- Contr
-00001e40: 6962 7574 696f 6e20 6973 206c 6963 656e  ibution is licen
-00001e50: 7365 6420 756e 6465 7220 7468 6520 4675  sed under the Fu
-00001e60: 7a7a 794c 6974 6520 4c69 6365 6e73 650a  zzyLite License.
-00001e70: 0a23 2320 3c61 206e 616d 653d 2272 6566  .## <a name="ref
-00001e80: 6572 656e 6365 223e 5265 6665 7265 6e63  erence">Referenc
-00001e90: 653c 2f61 3e0a 0a49 6620 796f 7520 6172  e</a>..If you ar
-00001ea0: 6520 7573 696e 6720 7468 6520 4675 7a7a  e using the Fuzz
-00001eb0: 794c 6974 6520 4c69 6272 6172 6965 732c  yLite Libraries,
-00001ec0: 2070 6c65 6173 6520 6369 7465 2074 6865   please cite the
-00001ed0: 2066 6f6c 6c6f 7769 6e67 2072 6566 6572   following refer
-00001ee0: 656e 6365 2069 6e20 796f 7572 2061 7274  ence in your art
-00001ef0: 6963 6c65 3a0a 0a3e 204a 7561 6e20 5261  icle:..> Juan Ra
-00001f00: 6461 2d56 696c 656c 612e 2054 6865 2046  da-Vilela. The F
-00001f10: 757a 7a79 4c69 7465 204c 6962 7261 7269  uzzyLite Librari
-00001f20: 6573 2066 6f72 2046 757a 7a79 204c 6f67  es for Fuzzy Log
-00001f30: 6963 2043 6f6e 7472 6f6c 2c20 3230 3138  ic Control, 2018
-00001f40: 2e20 5552 4c20 6874 7470 733a 2f2f 6675  . URL https://fu
-00001f50: 7a7a 796c 6974 652e 636f 6d2e 0a0a 4f72  zzylite.com...Or
-00001f60: 2075 7369 6e67 2060 6269 6274 6578 603a   using `bibtex`:
-00001f70: 0a0a 6060 6062 6962 7465 780a 406d 6973  ..```bibtex.@mis
-00001f80: 637b 666c 3a3a 6675 7a7a 796c 6974 652c  c{fl::fuzzylite,
-00001f90: 0a20 2020 2061 7574 686f 723d 7b4a 7561  .    author={Jua
-00001fa0: 6e20 5261 6461 2d56 696c 656c 617d 2c0a  n Rada-Vilela},.
-00001fb0: 2020 2020 7469 746c 653d 7b54 6865 2046      title={The F
-00001fc0: 757a 7a79 4c69 7465 204c 6962 7261 7269  uzzyLite Librari
-00001fd0: 6573 2066 6f72 2046 757a 7a79 204c 6f67  es for Fuzzy Log
-00001fe0: 6963 2043 6f6e 7472 6f6c 7d2c 0a20 2020  ic Control},.   
-00001ff0: 2075 726c 3d7b 6874 7470 733a 2f2f 6675   url={https://fu
-00002000: 7a7a 796c 6974 652e 636f 6d7d 2c0a 2020  zzylite.com},.  
-00002010: 2020 7965 6172 3d7b 3230 3138 7d0a 7d0a    year={2018}.}.
-00002020: 6060 600a 0a2a 2a2a 0a0a 6675 7a7a 796c  ```..***..fuzzyl
-00002030: 6974 6526 7265 673b 2069 7320 6120 7265  ite&reg; is a re
-00002040: 6769 7374 6572 6564 2074 7261 6465 6d61  gistered tradema
-00002050: 726b 206f 6620 4675 7a7a 794c 6974 6520  rk of FuzzyLite 
-00002060: 4c69 6d69 7465 6420 3c62 723e 0a6a 6675  Limited <br>.jfu
-00002070: 7a7a 796c 6974 6526 7472 6164 653b 2069  zzylite&trade; i
-00002080: 7320 6120 7472 6164 656d 6172 6b20 6f66  s a trademark of
-00002090: 2046 757a 7a79 4c69 7465 204c 696d 6974   FuzzyLite Limit
-000020a0: 6564 203c 6272 3e0a 7079 6675 7a7a 796c  ed <br>.pyfuzzyl
-000020b0: 6974 6526 7472 6164 653b 2069 7320 6120  ite&trade; is a 
-000020c0: 7472 6164 656d 6172 6b20 6f66 2046 757a  trademark of Fuz
-000020d0: 7a79 4c69 7465 204c 696d 6974 6564 203c  zyLite Limited <
-000020e0: 6272 3e0a 5174 4675 7a7a 794c 6974 6526  br>.QtFuzzyLite&
-000020f0: 7472 6164 653b 2069 7320 6120 7472 6164  trade; is a trad
-00002100: 656d 6172 6b20 6f66 2046 757a 7a79 4c69  emark of FuzzyLi
-00002110: 7465 204c 696d 6974 6564 203c 6272 3e0a  te Limited <br>.
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a3c 696d 6720 7372 633d 222f  er">.<img src="/
+00000020: 6675 7a7a 796c 6974 652e 706e 6722 2061  fuzzylite.png" a
+00000030: 6c74 3d22 6675 7a7a 796c 6974 6522 2077  lt="fuzzylite" w
+00000040: 6964 7468 3d22 3130 2522 3e0a 3c68 313e  idth="10%">.<h1>
+00000050: 7079 6675 7a7a 796c 6974 6520 382e 302e  pyfuzzylite 8.0.
+00000060: 333c 2f68 313e 0a3c 6832 3e41 2046 757a  3</h1>.<h2>A Fuz
+00000070: 7a79 204c 6f67 6963 2043 6f6e 7472 6f6c  zy Logic Control
+00000080: 204c 6962 7261 7279 2069 6e20 5079 7468   Library in Pyth
+00000090: 6f6e 3c2f 6832 3e0a 3c68 333e 6279 203c  on</h2>.<h3>by <
+000000a0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000000b0: 6675 7a7a 796c 6974 652e 636f 6d2f 6162  fuzzylite.com/ab
+000000c0: 6f75 7422 3e3c 623e 4a75 616e 2052 6164  out"><b>Juan Rad
+000000d0: 612d 5669 6c65 6c61 2c20 5068 443c 2f62  a-Vilela, PhD</b
+000000e0: 3e3c 2f61 3e3c 2f68 333e 0a0a 5b21 5b4c  ></a></h3>..[![L
+000000f0: 6963 656e 7365 3a20 4750 4c20 7633 5d28  icense: GPL v3](
+00000100: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000110: 6c64 732e 696f 2f62 6164 6765 2f4c 6963  lds.io/badge/Lic
+00000120: 656e 7365 2d47 504c 2532 3076 332d 626c  ense-GPL%20v3-bl
+00000130: 7565 2e73 7667 295d 2868 7474 7073 3a2f  ue.svg)](https:/
+00000140: 2f6f 7065 6e73 6f75 7263 652e 6f72 672f  /opensource.org/
+00000150: 6c69 6365 6e73 652f 6770 6c2d 332d 302f  license/gpl-3-0/
+00000160: 290a 5b21 5b4c 6963 656e 7365 3a20 5061  ).[![License: Pa
+00000170: 6964 5d28 6874 7470 733a 2f2f 696d 672e  id](https://img.
+00000180: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000190: 2f4c 6963 656e 7365 2d70 726f 7072 6965  /License-proprie
+000001a0: 7461 7279 2d62 6c75 6529 5d28 6d61 696c  tary-blue)](mail
+000001b0: 746f 3a73 616c 6573 4066 757a 7a79 6c69  to:sales@fuzzyli
+000001c0: 7465 2e63 6f6d 290a 5b21 5b43 6f76 6572  te.com).[![Cover
+000001d0: 6167 6520 5374 6174 7573 5d28 0a68 7474  age Status](.htt
+000001e0: 7073 3a2f 2f63 6f76 6572 616c 6c73 2e69  ps://coveralls.i
+000001f0: 6f2f 7265 706f 732f 6769 7468 7562 2f66  o/repos/github/f
+00000200: 757a 7a79 6c69 7465 2f70 7966 757a 7a79  uzzylite/pyfuzzy
+00000210: 6c69 7465 2f62 6164 6765 2e73 7667 3f62  lite/badge.svg?b
+00000220: 7261 6e63 683d 6d61 696e 295d 280a 6874  ranch=main)](.ht
+00000230: 7470 733a 2f2f 636f 7665 7261 6c6c 732e  tps://coveralls.
+00000240: 696f 2f67 6974 6875 622f 6675 7a7a 796c  io/github/fuzzyl
+00000250: 6974 652f 7079 6675 7a7a 796c 6974 653f  ite/pyfuzzylite?
+00000260: 6272 616e 6368 3d6d 6169 6e29 2020 0a5b  branch=main)  .[
+00000270: 215b 4275 696c 645d 2868 7474 7073 3a2f  ![Build](https:/
+00000280: 2f67 6974 6875 622e 636f 6d2f 6675 7a7a  /github.com/fuzz
+00000290: 796c 6974 652f 7079 6675 7a7a 796c 6974  ylite/pyfuzzylit
+000002a0: 652f 6163 7469 6f6e 732f 776f 726b 666c  e/actions/workfl
+000002b0: 6f77 732f 6275 696c 642e 796d 6c2f 6261  ows/build.yml/ba
+000002c0: 6467 652e 7376 6729 5d28 0a68 7474 7073  dge.svg)](.https
+000002d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6675  ://github.com/fu
+000002e0: 7a7a 796c 6974 652f 7079 6675 7a7a 796c  zzylite/pyfuzzyl
+000002f0: 6974 652f 6163 7469 6f6e 732f 776f 726b  ite/actions/work
+00000300: 666c 6f77 732f 6275 696c 642e 796d 6c29  flows/build.yml)
+00000310: 0a5b 215b 5465 7374 5d28 6874 7470 733a  .[![Test](https:
+00000320: 2f2f 6769 7468 7562 2e63 6f6d 2f66 757a  //github.com/fuz
+00000330: 7a79 6c69 7465 2f70 7966 757a 7a79 6c69  zylite/pyfuzzyli
+00000340: 7465 2f61 6374 696f 6e73 2f77 6f72 6b66  te/actions/workf
+00000350: 6c6f 7773 2f74 6573 742e 796d 6c2f 6261  lows/test.yml/ba
+00000360: 6467 652e 7376 6729 5d28 0a68 7474 7073  dge.svg)](.https
+00000370: 3a2f 2f67 6974 6875 622e 636f 6d2f 6675  ://github.com/fu
+00000380: 7a7a 796c 6974 652f 7079 6675 7a7a 796c  zzylite/pyfuzzyl
+00000390: 6974 652f 6163 7469 6f6e 732f 776f 726b  ite/actions/work
+000003a0: 666c 6f77 732f 7465 7374 2e79 6d6c 290a  flows/test.yml).
+000003b0: 5b21 5b50 7562 6c69 7368 5d28 6874 7470  [![Publish](http
+000003c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
+000003d0: 757a 7a79 6c69 7465 2f70 7966 757a 7a79  uzzylite/pyfuzzy
+000003e0: 6c69 7465 2f61 6374 696f 6e73 2f77 6f72  lite/actions/wor
+000003f0: 6b66 6c6f 7773 2f70 7562 6c69 7368 2e79  kflows/publish.y
+00000400: 6d6c 2f62 6164 6765 2e73 7667 295d 280a  ml/badge.svg)](.
+00000410: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000420: 6f6d 2f66 757a 7a79 6c69 7465 2f70 7966  om/fuzzylite/pyf
+00000430: 757a 7a79 6c69 7465 2f61 6374 696f 6e73  uzzylite/actions
+00000440: 2f77 6f72 6b66 6c6f 7773 2f70 7562 6c69  /workflows/publi
+00000450: 7368 2e79 6d6c 290a 0a3c 2f64 6976 3e0a  sh.yml)..</div>.
+00000460: 0a23 2320 3c61 206e 616d 653d 2266 757a  .## <a name="fuz
+00000470: 7a79 6c69 7465 223e 4675 7a7a 794c 6974  zylite">FuzzyLit
+00000480: 653c 2f61 3e0a 0a2a 2a54 6865 2046 757a  e</a>..**The Fuz
+00000490: 7a79 4c69 7465 204c 6962 7261 7269 6573  zyLite Libraries
+000004a0: 2066 6f72 2046 757a 7a79 204c 6f67 6963   for Fuzzy Logic
+000004b0: 2043 6f6e 7472 6f6c 2a2a 2072 6566 6572   Control** refer
+000004c0: 2074 6f20 5b60 6675 7a7a 796c 6974 6560   to [`fuzzylite`
+000004d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000004e0: 2e63 6f6d 2f66 757a 7a79 6c69 7465 2f66  .com/fuzzylite/f
+000004f0: 757a 7a79 6c69 7465 2f29 0a28 432b 2b29  uzzylite/).(C++)
+00000500: 2c20 5b60 7079 6675 7a7a 796c 6974 6560  , [`pyfuzzylite`
+00000510: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000520: 2e63 6f6d 2f66 757a 7a79 6c69 7465 2f70  .com/fuzzylite/p
+00000530: 7966 757a 7a79 6c69 7465 2f29 2028 5079  yfuzzylite/) (Py
+00000540: 7468 6f6e 292c 0a61 6e64 205b 606a 6675  thon),.and [`jfu
+00000550: 7a7a 796c 6974 6560 5d28 6874 7470 733a  zzylite`](https:
+00000560: 2f2f 6769 7468 7562 2e63 6f6d 2f66 757a  //github.com/fuz
+00000570: 7a79 6c69 7465 2f6a 6675 7a7a 796c 6974  zylite/jfuzzylit
+00000580: 652f 2920 284a 6176 6129 2e0a 0a54 6865  e/) (Java)...The
+00000590: 202a 2a67 6f61 6c2a 2a20 6f66 2074 6865   **goal** of the
+000005a0: 2046 757a 7a79 4c69 7465 204c 6962 7261   FuzzyLite Libra
+000005b0: 7269 6573 2069 7320 746f 202a 2a65 6173  ries is to **eas
+000005c0: 696c 792a 2a20 6465 7369 676e 2061 6e64  ily** design and
+000005d0: 202a 2a65 6666 6963 6965 6e74 6c79 2a2a   **efficiently**
+000005e0: 206f 7065 7261 7465 2066 757a 7a79 206c   operate fuzzy l
+000005f0: 6f67 6963 2063 6f6e 7472 6f6c 6c65 7273  ogic controllers
+00000600: 0a66 6f6c 6c6f 7769 6e67 2061 6e20 2a2a  .following an **
+00000610: 6f62 6a65 6374 2d6f 7269 656e 7465 642a  object-oriented*
+00000620: 2a20 7072 6f67 7261 6d6d 696e 6720 6d6f  * programming mo
+00000630: 6465 6c20 7769 7468 206d 696e 696d 616c  del with minimal
+00000640: 2064 6570 656e 6465 6e63 7920 6f6e 2065   dependency on e
+00000650: 7874 6572 6e61 6c20 6c69 6272 6172 6965  xternal librarie
+00000660: 732e 0a0a 2323 203c 6120 6e61 6d65 3d22  s...## <a name="
+00000670: 6c69 6365 6e73 6522 3e4c 6963 656e 7365  license">License
+00000680: 3c2f 613e 0a0a 6070 7966 757a 7a79 6c69  </a>..`pyfuzzyli
+00000690: 7465 6020 6973 2064 7561 6c2d 6c69 6365  te` is dual-lice
+000006a0: 6e73 6564 2075 6e64 6572 2074 6865 205b  nsed under the [
+000006b0: 2a2a 474e 5520 4750 4c20 332e 302a 2a5d  **GNU GPL 3.0**]
+000006c0: 2868 7474 7073 3a2f 2f6f 7065 6e73 6f75  (https://opensou
+000006d0: 7263 652e 6f72 672f 6c69 6365 6e73 652f  rce.org/license/
+000006e0: 6770 6c2d 332d 302f 2920 616e 6420 756e  gpl-3-0/) and un
+000006f0: 6465 7220 610a 2a2a 7072 6f70 7269 6574  der a.**propriet
+00000700: 6172 7920 6c69 6365 6e73 6520 666f 7220  ary license for 
+00000710: 636f 6d6d 6572 6369 616c 2070 7572 706f  commercial purpo
+00000720: 7365 732a 2a2e 0a0a 596f 7520 6172 6520  ses**...You are 
+00000730: 2a2a 7374 726f 6e67 6c79 2a2a 2065 6e63  **strongly** enc
+00000740: 6f75 7261 6765 6420 746f 2073 7570 706f  ouraged to suppo
+00000750: 7274 2074 6865 2064 6576 656c 6f70 6d65  rt the developme
+00000760: 6e74 206f 6620 7468 6520 4675 7a7a 794c  nt of the FuzzyL
+00000770: 6974 6520 4c69 6272 6172 6965 7320 6279  ite Libraries by
+00000780: 2070 7572 6368 6173 696e 6720 6120 6c69   purchasing a li
+00000790: 6365 6e73 650a 6f66 205b 6051 7446 757a  cense.of [`QtFuz
+000007a0: 7a79 4c69 7465 605d 2868 7474 7073 3a2f  zyLite`](https:/
+000007b0: 2f66 757a 7a79 6c69 7465 2e63 6f6d 2f64  /fuzzylite.com/d
+000007c0: 6f77 6e6c 6f61 6473 292e 0a0a 5b60 5174  ownloads)...[`Qt
+000007d0: 4675 7a7a 794c 6974 6560 5d28 6874 7470  FuzzyLite`](http
+000007e0: 733a 2f2f 6675 7a7a 796c 6974 652e 636f  s://fuzzylite.co
+000007f0: 6d2f 646f 776e 6c6f 6164 732f 2920 6973  m/downloads/) is
+00000800: 2074 6865 2062 6573 7420 6772 6170 6869   the best graphi
+00000810: 6361 6c20 7573 6572 2069 6e74 6572 6661  cal user interfa
+00000820: 6365 2061 7661 696c 6162 6c65 2074 6f20  ce available to 
+00000830: 6561 7369 6c79 2064 6573 6967 6e20 616e  easily design an
+00000840: 640a 6469 7265 6374 6c79 206f 7065 7261  d.directly opera
+00000850: 7465 2066 757a 7a79 206c 6f67 6963 2063  te fuzzy logic c
+00000860: 6f6e 7472 6f6c 6c65 7273 2069 6e20 7265  ontrollers in re
+00000870: 616c 2074 696d 652e 2041 7661 696c 6162  al time. Availab
+00000880: 6c65 2066 6f72 2057 696e 646f 7773 2c20  le for Windows, 
+00000890: 4d61 632c 2061 6e64 204c 696e 7578 2c20  Mac, and Linux, 
+000008a0: 6974 7320 676f 616c 2069 7320 746f 0a73  its goal is to.s
+000008b0: 6967 6e69 6669 6361 6e74 6c79 202a 2a73  ignificantly **s
+000008c0: 7065 6564 2075 702a 2a20 7468 6520 6465  peed up** the de
+000008d0: 7369 676e 206f 6620 796f 7572 2066 757a  sign of your fuz
+000008e0: 7a79 206c 6f67 6963 2063 6f6e 7472 6f6c  zy logic control
+000008f0: 6c65 7273 2c20 7768 696c 6520 7072 6f76  lers, while prov
+00000900: 6964 696e 6720 6120 7665 7279 202a 2a75  iding a very **u
+00000910: 7365 6675 6c2a 2a2c 202a 2a66 756e 6374  seful**, **funct
+00000920: 696f 6e61 6c2a 2a0a 616e 6420 2a2a 6265  ional**.and **be
+00000930: 6175 7469 6675 6c2a 2a20 7573 6572 2069  autiful** user i
+00000940: 6e74 6572 6661 6365 2e0a 506c 6561 7365  nterface..Please
+00000950: 2c20 646f 776e 6c6f 6164 2069 7420 616e  , download it an
+00000960: 6420 6368 6563 6b20 6974 206f 7574 2066  d check it out f
+00000970: 6f72 2066 7265 6520 6174 205b 6675 7a7a  or free at [fuzz
+00000980: 796c 6974 652e 636f 6d2f 646f 776e 6c6f  ylite.com/downlo
+00000990: 6164 735d 2868 7474 7073 3a2f 2f66 757a  ads](https://fuz
+000009a0: 7a79 6c69 7465 2e63 6f6d 2f64 6f77 6e6c  zylite.com/downl
+000009b0: 6f61 6473 292e 0a0a 2323 203c 6120 6e61  oads)...## <a na
+000009c0: 6d65 3d22 696e 7374 616c 6c22 3e49 6e73  me="install">Ins
+000009d0: 7461 6c6c 3c2f 613e 0a0a 6060 6063 6f6d  tall</a>..```com
+000009e0: 6d61 6e64 6c69 6e65 0a70 6970 2069 6e73  mandline.pip ins
+000009f0: 7461 6c6c 2070 7966 757a 7a79 6c69 7465  tall pyfuzzylite
+00000a00: 0a60 6060 0a0a 2323 203c 6120 6e61 6d65  .```..## <a name
+00000a10: 3d22 6665 6174 7572 6573 223e 4665 6174  ="features">Feat
+00000a20: 7572 6573 3c2f 613e 0a0a 2a2a 446f 6375  ures</a>..**Docu
+00000a30: 6d65 6e74 6174 696f 6e2a 2a3a 205b 6675  mentation**: [fu
+00000a40: 7a7a 796c 6974 652e 6769 7468 7562 2e69  zzylite.github.i
+00000a50: 6f2f 7079 6675 7a7a 796c 6974 652f 5d28  o/pyfuzzylite/](
+00000a60: 6874 7470 733a 2f2f 6675 7a7a 796c 6974  https://fuzzylit
+00000a70: 652e 6769 7468 7562 2e69 6f2f 7079 6675  e.github.io/pyfu
+00000a80: 7a7a 796c 6974 652f 290a 0a2a 2a28 3629  zzylite/)..**(6)
+00000a90: 2043 6f6e 7472 6f6c 6c65 7273 2a2a 3a20   Controllers**: 
+00000aa0: 4d61 6d64 616e 692c 2054 616b 6167 692d  Mamdani, Takagi-
+00000ab0: 5375 6765 6e6f 2c20 4c61 7273 656e 2c20  Sugeno, Larsen, 
+00000ac0: 5473 756b 616d 6f74 6f2c 2049 6e76 6572  Tsukamoto, Inver
+00000ad0: 7365 2054 7375 6b61 6d6f 746f 2c20 4879  se Tsukamoto, Hy
+00000ae0: 6272 6964 0a0a 2a2a 2832 3529 204c 696e  brid..**(25) Lin
+00000af0: 6775 6973 7469 6320 7465 726d 732a 2a3a  guistic terms**:
+00000b00: 2020 2835 2920 2a42 6173 6963 2a3a 2054    (5) *Basic*: T
+00000b10: 7269 616e 676c 652c 2054 7261 7065 7a6f  riangle, Trapezo
+00000b20: 6964 2c20 5265 6374 616e 676c 652c 2044  id, Rectangle, D
+00000b30: 6973 6372 6574 652c 2053 656d 6945 6c6c  iscrete, SemiEll
+00000b40: 6970 7365 2e0a 2838 2920 2a45 7874 656e  ipse..(8) *Exten
+00000b50: 6465 642a 3a20 4265 6c6c 2c20 436f 7369  ded*: Bell, Cosi
+00000b60: 6e65 2c20 4761 7573 7369 616e 2c20 4761  ne, Gaussian, Ga
+00000b70: 7573 7369 616e 5072 6f64 7563 742c 2050  ussianProduct, P
+00000b80: 6953 6861 7065 2c20 5369 676d 6f69 6444  iShape, SigmoidD
+00000b90: 6966 6665 7265 6e63 652c 2053 6967 6d6f  ifference, Sigmo
+00000ba0: 6964 5072 6f64 7563 742c 2053 7069 6b65  idProduct, Spike
+00000bb0: 2e0a 2837 2920 2a45 6467 6573 2a3a 2041  ..(7) *Edges*: A
+00000bc0: 7263 2c20 4269 6e61 7279 2c20 436f 6e63  rc, Binary, Conc
+00000bd0: 6176 652c 2052 616d 702c 2053 6967 6d6f  ave, Ramp, Sigmo
+00000be0: 6964 2c20 5353 6861 7065 2c20 5a53 6861  id, SShape, ZSha
+00000bf0: 7065 2e0a 2833 2920 2a46 756e 6374 696f  pe..(3) *Functio
+00000c00: 6e73 2a3a 2043 6f6e 7374 616e 742c 204c  ns*: Constant, L
+00000c10: 696e 6561 722c 2046 756e 6374 696f 6e2e  inear, Function.
+00000c20: 2028 3229 202a 5370 6563 6961 6c2a 3a20   (2) *Special*: 
+00000c30: 4167 6772 6567 6174 6564 2c20 4163 7469  Aggregated, Acti
+00000c40: 7661 7465 642e 0a0a 2a2a 2837 2920 4163  vated...**(7) Ac
+00000c50: 7469 7661 7469 6f6e 206d 6574 686f 6473  tivation methods
+00000c60: 2a2a 3a20 2047 656e 6572 616c 2c20 5072  **:  General, Pr
+00000c70: 6f70 6f72 7469 6f6e 616c 2c20 5468 7265  oportional, Thre
+00000c80: 7368 6f6c 642c 2046 6972 7374 2c20 4c61  shold, First, La
+00000c90: 7374 2c20 4c6f 7765 7374 2c20 4869 6768  st, Lowest, High
+00000ca0: 6573 742e 0a0a 2a2a 2839 2920 436f 6e6a  est...**(9) Conj
+00000cb0: 756e 6374 696f 6e20 616e 6420 496d 706c  unction and Impl
+00000cc0: 6963 6174 696f 6e20 2854 2d4e 6f72 6d73  ication (T-Norms
+00000cd0: 292a 2a3a 204d 696e 696d 756d 2c20 416c  )**: Minimum, Al
+00000ce0: 6765 6272 6169 6350 726f 6475 6374 2c20  gebraicProduct, 
+00000cf0: 426f 756e 6465 6444 6966 6665 7265 6e63  BoundedDifferenc
+00000d00: 652c 2044 7261 7374 6963 5072 6f64 7563  e, DrasticProduc
+00000d10: 742c 0a45 696e 7374 6569 6e50 726f 6475  t,.EinsteinProdu
+00000d20: 6374 2c20 4861 6d61 6368 6572 5072 6f64  ct, HamacherProd
+00000d30: 7563 742c 204e 696c 706f 7465 6e74 4d69  uct, NilpotentMi
+00000d40: 6e69 6d75 6d2c 204c 616d 6264 614e 6f72  nimum, LambdaNor
+00000d50: 6d2c 2046 756e 6374 696f 6e4e 6f72 6d2e  m, FunctionNorm.
+00000d60: 0a0a 2a2a 2831 3129 2044 6973 6a75 6e63  ..**(11) Disjunc
+00000d70: 7469 6f6e 2061 6e64 2041 6767 7265 6761  tion and Aggrega
+00000d80: 7469 6f6e 2028 532d 4e6f 726d 7329 2a2a  tion (S-Norms)**
+00000d90: 3a20 204d 6178 696d 756d 2c20 416c 6765  :  Maximum, Alge
+00000da0: 6272 6169 6353 756d 2c20 426f 756e 6465  braicSum, Bounde
+00000db0: 6453 756d 2c20 4472 6173 7469 6353 756d  dSum, DrasticSum
+00000dc0: 2c20 4569 6e73 7465 696e 5375 6d2c 0a48  , EinsteinSum,.H
+00000dd0: 616d 6163 6865 7253 756d 2c20 4e69 6c70  amacherSum, Nilp
+00000de0: 6f74 656e 744d 6178 696d 756d 2c20 4e6f  otentMaximum, No
+00000df0: 726d 616c 697a 6564 5375 6d2c 2055 6e62  rmalizedSum, Unb
+00000e00: 6f75 6e64 6564 5375 6d2c 204c 616d 6264  oundedSum, Lambd
+00000e10: 614e 6f72 6d2c 2046 756e 6374 696f 6e4e  aNorm, FunctionN
+00000e20: 6f72 6d2e 0a0a 2a2a 2837 2920 4465 6675  orm...**(7) Defu
+00000e30: 7a7a 6966 6965 7273 2a2a 3a20 2028 3529  zzifiers**:  (5)
+00000e40: 202a 496e 7465 6772 616c 2a3a 2043 656e   *Integral*: Cen
+00000e50: 7472 6f69 642c 2042 6973 6563 746f 722c  troid, Bisector,
+00000e60: 2053 6d61 6c6c 6573 744f 664d 6178 696d   SmallestOfMaxim
+00000e70: 756d 2c20 4c61 7267 6573 744f 664d 6178  um, LargestOfMax
+00000e80: 696d 756d 2c20 4d65 616e 4f66 4d61 7869  imum, MeanOfMaxi
+00000e90: 6d75 6d2e 0a28 3229 202a 5765 6967 6874  mum..(2) *Weight
+00000ea0: 6564 2a3a 2057 6569 6768 7465 6441 7665  ed*: WeightedAve
+00000eb0: 7261 6765 2c20 5765 6967 6874 6564 5375  rage, WeightedSu
+00000ec0: 6d2e 0a0a 2a2a 2837 2920 4865 6467 6573  m...**(7) Hedges
+00000ed0: 2a2a 3a20 416e 792c 204e 6f74 2c20 4578  **: Any, Not, Ex
+00000ee0: 7472 656d 656c 792c 2053 656c 646f 6d2c  tremely, Seldom,
+00000ef0: 2053 6f6d 6577 6861 742c 2056 6572 792c   Somewhat, Very,
+00000f00: 2046 756e 6374 696f 6e2e 0a0a 2a2a 2833   Function...**(3
+00000f10: 2920 496d 706f 7274 6572 732a 2a3a 2046  ) Importers**: F
+00000f20: 757a 7a79 4c69 7465 204c 616e 6775 6167  uzzyLite Languag
+00000f30: 6520 6066 6c6c 602e 2057 6974 6820 6066  e `fll`. With `f
+00000f40: 757a 7a79 6c69 7465 603a 2046 757a 7a79  uzzylite`: Fuzzy
+00000f50: 2049 6e66 6572 656e 6365 2053 7973 7465   Inference Syste
+00000f60: 6d20 6066 6973 602c 2046 757a 7a79 2043  m `fis`, Fuzzy C
+00000f70: 6f6e 7472 6f6c 0a4c 616e 6775 6167 6520  ontrol.Language 
+00000f80: 6066 636c 602e 0a0a 2a2a 2837 2920 4578  `fcl`...**(7) Ex
+00000f90: 706f 7274 6572 732a 2a3a 2060 5079 7468  porters**: `Pyth
+00000fa0: 6f6e 602c 2046 757a 7a79 4c69 7465 204c  on`, FuzzyLite L
+00000fb0: 616e 6775 6167 6520 6066 6c6c 602c 2046  anguage `fll`, F
+00000fc0: 757a 7a79 4c69 7465 2044 6174 6173 6574  uzzyLite Dataset
+00000fd0: 2060 666c 6460 2e20 5769 7468 2060 6675   `fld`. With `fu
+00000fe0: 7a7a 796c 6974 6560 3a20 6043 2b2b 602c  zzylite`: `C++`,
+00000ff0: 2060 4a61 7661 602c 0a46 757a 7a79 4c69   `Java`,.FuzzyLi
+00001000: 7465 204c 616e 6775 6167 6520 6066 6c6c  te Language `fll
+00001010: 602c 2046 757a 7a79 4c69 7465 2044 6174  `, FuzzyLite Dat
+00001020: 6173 6574 2060 666c 6460 2c20 6052 6020  aset `fld`, `R` 
+00001030: 7363 7269 7074 2c20 4675 7a7a 7920 496e  script, Fuzzy In
+00001040: 6665 7265 6e63 6520 5379 7374 656d 2060  ference System `
+00001050: 6669 7360 2c20 4675 7a7a 7920 436f 6e74  fis`, Fuzzy Cont
+00001060: 726f 6c0a 4c61 6e67 7561 6765 2060 6663  rol.Language `fc
+00001070: 6c60 2e0a 0a2a 2a28 3330 2b29 2045 7861  l`...**(30+) Exa
+00001080: 6d70 6c65 732a 2a20 206f 6620 4d61 6d64  mples**  of Mamd
+00001090: 616e 692c 2054 616b 6167 692d 5375 6765  ani, Takagi-Suge
+000010a0: 6e6f 2c20 5473 756b 616d 6f74 6f2c 2061  no, Tsukamoto, a
+000010b0: 6e64 2048 7962 7269 6420 636f 6e74 726f  nd Hybrid contro
+000010c0: 6c6c 6572 7320 6672 6f6d 2060 6675 7a7a  llers from `fuzz
+000010d0: 796c 6974 6560 2c20 4f63 7461 7665 2c20  ylite`, Octave, 
+000010e0: 616e 6420 4d61 746c 6162 2c0a 6561 6368  and Matlab,.each
+000010f0: 2069 6e63 6c75 6465 6420 696e 2074 6865   included in the
+00001100: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
+00001110: 7473 3a20 6070 7960 2c20 6066 6c6c 602c  ts: `py`, `fll`,
+00001120: 2060 666c 6460 2e20 5769 7468 2060 6675   `fld`. With `fu
+00001130: 7a7a 796c 6974 6560 3a20 6043 2b2b 602c  zzylite`: `C++`,
+00001140: 2060 4a61 7661 602c 2060 5260 2c20 6066   `Java`, `R`, `f
+00001150: 6973 602c 2061 6e64 2060 6663 6c60 2e0a  is`, and `fcl`..
+00001160: 0a23 2320 3c61 206e 616d 653d 2265 7861  .## <a name="exa
+00001170: 6d70 6c65 7322 3e45 7861 6d70 6c65 733c  mples">Examples<
+00001180: 2f61 3e0a 0a23 2323 2046 757a 7a79 4c69  /a>..### FuzzyLi
+00001190: 7465 204c 616e 6775 6167 650a 0a60 6060  te Language..```
+000011a0: 7961 6d6c 0a23 2046 696c 653a 2065 7861  yaml.# File: exa
+000011b0: 6d70 6c65 732f 6d61 6d64 616e 692f 4f62  mples/mamdani/Ob
+000011c0: 7374 6163 6c65 4176 6f69 6461 6e63 652e  stacleAvoidance.
+000011d0: 666c 6c0a 456e 6769 6e65 3a20 4f62 7374  fll.Engine: Obst
+000011e0: 6163 6c65 4176 6f69 6461 6e63 650a 496e  acleAvoidance.In
+000011f0: 7075 7456 6172 6961 626c 653a 206f 6273  putVariable: obs
+00001200: 7461 636c 650a 2020 656e 6162 6c65 643a  tacle.  enabled:
+00001210: 2074 7275 650a 2020 7261 6e67 653a 2030   true.  range: 0
+00001220: 2e30 3030 2031 2e30 3030 0a20 206c 6f63  .000 1.000.  loc
+00001230: 6b2d 7261 6e67 653a 2066 616c 7365 0a20  k-range: false. 
+00001240: 2074 6572 6d3a 206c 6566 7420 5261 6d70   term: left Ramp
+00001250: 2031 2e30 3030 2030 2e30 3030 0a20 2074   1.000 0.000.  t
+00001260: 6572 6d3a 2072 6967 6874 2052 616d 7020  erm: right Ramp 
+00001270: 302e 3030 3020 312e 3030 300a 4f75 7470  0.000 1.000.Outp
+00001280: 7574 5661 7269 6162 6c65 3a20 6d53 7465  utVariable: mSte
+00001290: 6572 0a20 2065 6e61 626c 6564 3a20 7472  er.  enabled: tr
+000012a0: 7565 0a20 2072 616e 6765 3a20 302e 3030  ue.  range: 0.00
+000012b0: 3020 312e 3030 300a 2020 6c6f 636b 2d72  0 1.000.  lock-r
+000012c0: 616e 6765 3a20 6661 6c73 650a 2020 6167  ange: false.  ag
+000012d0: 6772 6567 6174 696f 6e3a 204d 6178 696d  gregation: Maxim
+000012e0: 756d 0a20 2064 6566 757a 7a69 6669 6572  um.  defuzzifier
+000012f0: 3a20 4365 6e74 726f 6964 2031 3030 0a20  : Centroid 100. 
+00001300: 2064 6566 6175 6c74 3a20 6e61 6e0a 2020   default: nan.  
+00001310: 6c6f 636b 2d70 7265 7669 6f75 733a 2066  lock-previous: f
+00001320: 616c 7365 0a20 2074 6572 6d3a 206c 6566  alse.  term: lef
+00001330: 7420 5261 6d70 2031 2e30 3030 2030 2e30  t Ramp 1.000 0.0
+00001340: 3030 0a20 2074 6572 6d3a 2072 6967 6874  00.  term: right
+00001350: 2052 616d 7020 302e 3030 3020 312e 3030   Ramp 0.000 1.00
+00001360: 300a 5275 6c65 426c 6f63 6b3a 206d 616d  0.RuleBlock: mam
+00001370: 6461 6e69 0a20 2065 6e61 626c 6564 3a20  dani.  enabled: 
+00001380: 7472 7565 0a20 2063 6f6e 6a75 6e63 7469  true.  conjuncti
+00001390: 6f6e 3a20 6e6f 6e65 0a20 2064 6973 6a75  on: none.  disju
+000013a0: 6e63 7469 6f6e 3a20 6e6f 6e65 0a20 2069  nction: none.  i
+000013b0: 6d70 6c69 6361 7469 6f6e 3a20 416c 6765  mplication: Alge
+000013c0: 6272 6169 6350 726f 6475 6374 0a20 2061  braicProduct.  a
+000013d0: 6374 6976 6174 696f 6e3a 2047 656e 6572  ctivation: Gener
+000013e0: 616c 0a20 2072 756c 653a 2069 6620 6f62  al.  rule: if ob
+000013f0: 7374 6163 6c65 2069 7320 6c65 6674 2074  stacle is left t
+00001400: 6865 6e20 6d53 7465 6572 2069 7320 7269  hen mSteer is ri
+00001410: 6768 740a 2020 7275 6c65 3a20 6966 206f  ght.  rule: if o
+00001420: 6273 7461 636c 6520 6973 2072 6967 6874  bstacle is right
+00001430: 2074 6865 6e20 6d53 7465 6572 2069 7320   then mSteer is 
+00001440: 6c65 6674 0a60 6060 0a0a 6060 6070 7974  left.```..```pyt
+00001450: 686f 6e0a 2320 5079 7468 6f6e 0a69 6d70  hon.# Python.imp
+00001460: 6f72 7420 6675 7a7a 796c 6974 6520 6173  ort fuzzylite as
+00001470: 2066 6c0a 0a65 6e67 696e 6520 3d20 666c   fl..engine = fl
+00001480: 2e46 6c6c 496d 706f 7274 6572 2829 2e66  .FllImporter().f
+00001490: 726f 6d5f 6669 6c65 2822 6578 616d 706c  rom_file("exampl
+000014a0: 6573 2f6d 616d 6461 6e69 2f4f 6273 7461  es/mamdani/Obsta
+000014b0: 636c 6541 766f 6964 616e 6365 2e66 6c6c  cleAvoidance.fll
+000014c0: 2229 0a60 6060 0a0a 2323 2320 5079 7468  ").```..### Pyth
+000014d0: 6f6e 0a0a 6060 6070 7974 686f 6e0a 696d  on..```python.im
+000014e0: 706f 7274 2066 757a 7a79 6c69 7465 2061  port fuzzylite a
+000014f0: 7320 666c 0a0a 656e 6769 6e65 203d 2066  s fl..engine = f
+00001500: 6c2e 456e 6769 6e65 280a 2020 2020 6e61  l.Engine(.    na
+00001510: 6d65 3d22 4f62 7374 6163 6c65 4176 6f69  me="ObstacleAvoi
+00001520: 6461 6e63 6522 2c0a 2020 2020 696e 7075  dance",.    inpu
+00001530: 745f 7661 7269 6162 6c65 733d 5b0a 2020  t_variables=[.  
+00001540: 2020 2020 2020 666c 2e49 6e70 7574 5661        fl.InputVa
+00001550: 7269 6162 6c65 280a 2020 2020 2020 2020  riable(.        
+00001560: 2020 2020 6e61 6d65 3d22 6f62 7374 6163      name="obstac
+00001570: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
+00001580: 206d 696e 696d 756d 3d30 2e30 2c0a 2020   minimum=0.0,.  
+00001590: 2020 2020 2020 2020 2020 6d61 7869 6d75            maximu
+000015a0: 6d3d 312e 302c 0a20 2020 2020 2020 2020  m=1.0,.         
+000015b0: 2020 206c 6f63 6b5f 7261 6e67 653d 4661     lock_range=Fa
+000015c0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+000015d0: 2074 6572 6d73 3d5b 666c 2e52 616d 7028   terms=[fl.Ramp(
+000015e0: 226c 6566 7422 2c20 312e 302c 2030 2e30  "left", 1.0, 0.0
+000015f0: 292c 2066 6c2e 5261 6d70 2822 7269 6768  ), fl.Ramp("righ
+00001600: 7422 2c20 302e 302c 2031 2e30 295d 2c0a  t", 0.0, 1.0)],.
+00001610: 2020 2020 2020 2020 290a 2020 2020 5d2c          ).    ],
+00001620: 0a20 2020 206f 7574 7075 745f 7661 7269  .    output_vari
+00001630: 6162 6c65 733d 5b0a 2020 2020 2020 2020  ables=[.        
+00001640: 666c 2e4f 7574 7075 7456 6172 6961 626c  fl.OutputVariabl
+00001650: 6528 0a20 2020 2020 2020 2020 2020 206e  e(.            n
+00001660: 616d 653d 226d 5374 6565 7222 2c0a 2020  ame="mSteer",.  
+00001670: 2020 2020 2020 2020 2020 6d69 6e69 6d75            minimu
+00001680: 6d3d 302e 302c 0a20 2020 2020 2020 2020  m=0.0,.         
+00001690: 2020 206d 6178 696d 756d 3d31 2e30 2c0a     maximum=1.0,.
+000016a0: 2020 2020 2020 2020 2020 2020 6c6f 636b              lock
+000016b0: 5f72 616e 6765 3d46 616c 7365 2c0a 2020  _range=False,.  
+000016c0: 2020 2020 2020 2020 2020 6c6f 636b 5f70            lock_p
+000016d0: 7265 7669 6f75 733d 4661 6c73 652c 0a20  revious=False,. 
+000016e0: 2020 2020 2020 2020 2020 2064 6566 6175             defau
+000016f0: 6c74 5f76 616c 7565 3d66 6c2e 6e61 6e2c  lt_value=fl.nan,
+00001700: 0a20 2020 2020 2020 2020 2020 2061 6767  .            agg
+00001710: 7265 6761 7469 6f6e 3d66 6c2e 4d61 7869  regation=fl.Maxi
+00001720: 6d75 6d28 292c 0a20 2020 2020 2020 2020  mum(),.         
+00001730: 2020 2064 6566 757a 7a69 6669 6572 3d66     defuzzifier=f
+00001740: 6c2e 4365 6e74 726f 6964 2872 6573 6f6c  l.Centroid(resol
+00001750: 7574 696f 6e3d 3130 3029 2c0a 2020 2020  ution=100),.    
+00001760: 2020 2020 2020 2020 7465 726d 733d 5b66          terms=[f
+00001770: 6c2e 5261 6d70 2822 6c65 6674 222c 2031  l.Ramp("left", 1
+00001780: 2e30 2c20 302e 3029 2c20 666c 2e52 616d  .0, 0.0), fl.Ram
+00001790: 7028 2272 6967 6874 222c 2030 2e30 2c20  p("right", 0.0, 
+000017a0: 312e 3029 5d2c 0a20 2020 2020 2020 2029  1.0)],.        )
+000017b0: 0a20 2020 205d 2c0a 2020 2020 7275 6c65  .    ],.    rule
+000017c0: 5f62 6c6f 636b 733d 5b0a 2020 2020 2020  _blocks=[.      
+000017d0: 2020 666c 2e52 756c 6542 6c6f 636b 280a    fl.RuleBlock(.
+000017e0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000017f0: 3d22 6d61 6d64 616e 6922 2c0a 2020 2020  ="mamdani",.    
+00001800: 2020 2020 2020 2020 636f 6e6a 756e 6374          conjunct
+00001810: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ion=None,.      
+00001820: 2020 2020 2020 6469 736a 756e 6374 696f        disjunctio
+00001830: 6e3d 4e6f 6e65 2c0a 2020 2020 2020 2020  n=None,.        
+00001840: 2020 2020 696d 706c 6963 6174 696f 6e3d      implication=
+00001850: 666c 2e41 6c67 6562 7261 6963 5072 6f64  fl.AlgebraicProd
+00001860: 7563 7428 292c 0a20 2020 2020 2020 2020  uct(),.         
+00001870: 2020 2061 6374 6976 6174 696f 6e3d 666c     activation=fl
+00001880: 2e47 656e 6572 616c 2829 2c0a 2020 2020  .General(),.    
+00001890: 2020 2020 2020 2020 7275 6c65 733d 5b0a          rules=[.
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 666c 2e52 756c 652e 6372 6561 7465 2822  fl.Rule.create("
+000018c0: 6966 206f 6273 7461 636c 6520 6973 206c  if obstacle is l
+000018d0: 6566 7420 7468 656e 206d 5374 6565 7220  eft then mSteer 
+000018e0: 6973 2072 6967 6874 2229 2c0a 2020 2020  is right"),.    
+000018f0: 2020 2020 2020 2020 2020 2020 666c 2e52              fl.R
+00001900: 756c 652e 6372 6561 7465 2822 6966 206f  ule.create("if o
+00001910: 6273 7461 636c 6520 6973 2072 6967 6874  bstacle is right
+00001920: 2074 6865 6e20 6d53 7465 6572 2069 7320   then mSteer is 
+00001930: 6c65 6674 2229 2c0a 2020 2020 2020 2020  left"),.        
+00001940: 2020 2020 5d2c 0a20 2020 2020 2020 2029      ],.        )
+00001950: 0a20 2020 205d 2c0a 290a 6060 600a 0a23  .    ],.).```..#
+00001960: 2323 2060 666c 6f61 7460 2061 6e64 2076  ## `float` and v
+00001970: 6563 746f 7269 7a61 7469 6f6e 0a0a 6060  ectorization..``
+00001980: 6070 7974 686f 6e0a 2320 7369 6e67 6c65  `python.# single
+00001990: 2060 666c 6f61 7460 206f 7065 7261 7469   `float` operati
+000019a0: 6f6e 0a65 6e67 696e 652e 696e 7075 745f  on.engine.input_
+000019b0: 7661 7269 6162 6c65 2822 6f62 7374 6163  variable("obstac
+000019c0: 6c65 2229 2e76 616c 7565 203d 2030 2e35  le").value = 0.5
+000019d0: 0a65 6e67 696e 652e 7072 6f63 6573 7328  .engine.process(
+000019e0: 290a 7072 696e 7428 2279 203d 222c 2065  ).print("y =", e
+000019f0: 6e67 696e 652e 6f75 7470 7574 5f76 6172  ngine.output_var
+00001a00: 6961 626c 6528 226d 5374 6565 7222 292e  iable("mSteer").
+00001a10: 7661 6c75 6529 0a23 203e 2079 203d 2030  value).# > y = 0
+00001a20: 2e35 0a70 7269 6e74 2822 e1bb b920 3d22  .5.print("... ="
+00001a30: 2c20 656e 6769 6e65 2e6f 7574 7075 745f  , engine.output_
+00001a40: 7661 7269 6162 6c65 2822 6d53 7465 6572  variable("mSteer
+00001a50: 2229 2e66 757a 7a79 5f76 616c 7565 2829  ").fuzzy_value()
+00001a60: 290a 2320 3e20 e1bb b920 3d20 302e 3530  ).# > ... = 0.50
+00001a70: 302f 6c65 6674 202b 2030 2e35 3030 2f72  0/left + 0.500/r
+00001a80: 6967 6874 0a0a 2320 7665 6374 6f72 697a  ight..# vectoriz
+00001a90: 6174 696f 6e0a 656e 6769 6e65 2e69 6e70  ation.engine.inp
+00001aa0: 7574 5f76 6172 6961 626c 6528 226f 6273  ut_variable("obs
+00001ab0: 7461 636c 6522 292e 7661 6c75 6520 3d20  tacle").value = 
+00001ac0: 666c 2e61 7272 6179 285b 302c 2030 2e32  fl.array([0, 0.2
+00001ad0: 352c 2030 2e35 2c20 302e 3735 2c20 312e  5, 0.5, 0.75, 1.
+00001ae0: 305d 290a 656e 6769 6e65 2e70 726f 6365  0]).engine.proce
+00001af0: 7373 2829 0a70 7269 6e74 2822 7920 3d22  ss().print("y ="
+00001b00: 2c20 7265 7072 2865 6e67 696e 652e 6f75  , repr(engine.ou
+00001b10: 7470 7574 5f76 6172 6961 626c 6528 226d  tput_variable("m
+00001b20: 5374 6565 7222 292e 7661 6c75 6529 290a  Steer").value)).
+00001b30: 2320 3e20 7920 3d20 6172 7261 7928 5b30  # > y = array([0
+00001b40: 2e36 3636 3636 3635 202c 2030 2e36 3231  .6666665 , 0.621
+00001b50: 3739 3437 372c 2030 2e35 2020 2020 2020  79477, 0.5      
+00001b60: 202c 2030 2e33 3738 3230 3532 332c 2030   , 0.37820523, 0
+00001b70: 2e33 3333 3333 3335 205d 290a 7072 696e  .3333335 ]).prin
+00001b80: 7428 22e1 bbb9 203d 222c 2072 6570 7228  t("... =", repr(
+00001b90: 656e 6769 6e65 2e6f 7574 7075 745f 7661  engine.output_va
+00001ba0: 7269 6162 6c65 2822 6d53 7465 6572 2229  riable("mSteer")
+00001bb0: 2e66 757a 7a79 5f76 616c 7565 2829 2929  .fuzzy_value()))
+00001bc0: 0a23 203e 20e1 bbb9 203d 2061 7272 6179  .# > ... = array
+00001bd0: 285b 2730 2e30 3030 2f6c 6566 7420 2b20  (['0.000/left + 
+00001be0: 312e 3030 302f 7269 6768 7427 2c0a 2320  1.000/right',.# 
+00001bf0: 2020 2020 2020 2020 2020 2020 2027 302e               '0.
+00001c00: 3235 302f 6c65 6674 202b 2030 2e37 3530  250/left + 0.750
+00001c10: 2f72 6967 6874 272c 0a23 2020 2020 2020  /right',.#      
+00001c20: 2020 2020 2020 2020 2730 2e35 3030 2f6c          '0.500/l
+00001c30: 6566 7420 2b20 302e 3530 302f 7269 6768  eft + 0.500/righ
+00001c40: 7427 2c0a 2320 2020 2020 2020 2020 2020  t',.#           
+00001c50: 2020 2027 302e 3735 302f 6c65 6674 202b     '0.750/left +
+00001c60: 2030 2e32 3530 2f72 6967 6874 272c 0a23   0.250/right',.#
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2731                '1
+00001c80: 2e30 3030 2f6c 6566 7420 2b20 302e 3030  .000/left + 0.00
+00001c90: 302f 7269 6768 7427 5d2c 2064 7479 7065  0/right'], dtype
+00001ca0: 3d27 3c55 3236 2729 0a60 6060 0a0a 506c  ='<U26').```..Pl
+00001cb0: 6561 7365 2072 6566 6572 2074 6f20 7468  ease refer to th
+00001cc0: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
+00001cd0: 666f 7220 6d6f 7265 0a69 6e66 6f72 6d61  for more.informa
+00001ce0: 7469 6f6e 3a20 5b2a 2a66 757a 7a79 6c69  tion: [**fuzzyli
+00001cf0: 7465 2e67 6974 6875 622e 696f 2f70 7966  te.github.io/pyf
+00001d00: 757a 7a79 6c69 7465 2f2a 2a5d 2868 7474  uzzylite/**](htt
+00001d10: 7073 3a2f 2f66 757a 7a79 6c69 7465 2e67  ps://fuzzylite.g
+00001d20: 6974 6875 622e 696f 2f70 7966 757a 7a79  ithub.io/pyfuzzy
+00001d30: 6c69 7465 2f29 0a0a 2323 203c 6120 6e61  lite/)..## <a na
+00001d40: 6d65 3d22 636f 6e74 7269 6275 7469 6e67  me="contributing
+00001d50: 223e 436f 6e74 7269 6275 7469 6e67 3c2f  ">Contributing</
+00001d60: 613e 0a0a 416c 6c20 636f 6e74 7269 6275  a>..All contribu
+00001d70: 7469 6f6e 7320 6172 6520 7765 6c63 6f6d  tions are welcom
+00001d80: 652c 2070 726f 7669 6465 6420 7468 6579  e, provided they
+00001d90: 2066 6f6c 6c6f 7720 7468 6520 666f 6c6c   follow the foll
+00001da0: 6f77 696e 6720 6775 6964 656c 696e 6573  owing guidelines
+00001db0: 3a0a 0a2d 2053 6f75 7263 6520 636f 6465  :..- Source code
+00001dc0: 2069 7320 636f 6e73 6973 7465 6e74 2077   is consistent w
+00001dd0: 6974 6820 7374 616e 6461 7264 7320 696e  ith standards in
+00001de0: 2074 6865 206c 6962 7261 7279 0a2d 2043   the library.- C
+00001df0: 6f6e 7472 6962 7574 696f 6e20 6973 2070  ontribution is p
+00001e00: 726f 7065 726c 7920 646f 6375 6d65 6e74  roperly document
+00001e10: 6564 2061 6e64 2074 6573 7465 642c 2072  ed and tested, r
+00001e20: 6169 7369 6e67 2069 7373 7565 7320 7768  aising issues wh
+00001e30: 6572 6520 6170 7072 6f70 7269 6174 650a  ere appropriate.
+00001e40: 2d20 436f 6e74 7269 6275 7469 6f6e 2069  - Contribution i
+00001e50: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00001e60: 2074 6865 2046 757a 7a79 4c69 7465 204c   the FuzzyLite L
+00001e70: 6963 656e 7365 0a0a 2323 203c 6120 6e61  icense..## <a na
+00001e80: 6d65 3d22 7265 6665 7265 6e63 6522 3e52  me="reference">R
+00001e90: 6566 6572 656e 6365 3c2f 613e 0a0a 4966  eference</a>..If
+00001ea0: 2079 6f75 2061 7265 2075 7369 6e67 2074   you are using t
+00001eb0: 6865 2046 757a 7a79 4c69 7465 204c 6962  he FuzzyLite Lib
+00001ec0: 7261 7269 6573 2c20 706c 6561 7365 2063  raries, please c
+00001ed0: 6974 6520 7468 6520 666f 6c6c 6f77 696e  ite the followin
+00001ee0: 6720 7265 6665 7265 6e63 6520 696e 2079  g reference in y
+00001ef0: 6f75 7220 6172 7469 636c 653a 0a0a 3e20  our article:..> 
+00001f00: 4a75 616e 2052 6164 612d 5669 6c65 6c61  Juan Rada-Vilela
+00001f10: 2e20 5468 6520 4675 7a7a 794c 6974 6520  . The FuzzyLite 
+00001f20: 4c69 6272 6172 6965 7320 666f 7220 4675  Libraries for Fu
+00001f30: 7a7a 7920 4c6f 6769 6320 436f 6e74 726f  zzy Logic Contro
+00001f40: 6c2c 2032 3031 382e 2055 524c 2068 7474  l, 2018. URL htt
+00001f50: 7073 3a2f 2f66 757a 7a79 6c69 7465 2e63  ps://fuzzylite.c
+00001f60: 6f6d 2e0a 0a4f 7220 7573 696e 6720 6062  om...Or using `b
+00001f70: 6962 7465 7860 3a0a 0a60 6060 6269 6274  ibtex`:..```bibt
+00001f80: 6578 0a40 6d69 7363 7b66 6c3a 3a66 757a  ex.@misc{fl::fuz
+00001f90: 7a79 6c69 7465 2c0a 2020 2020 6175 7468  zylite,.    auth
+00001fa0: 6f72 3d7b 4a75 616e 2052 6164 612d 5669  or={Juan Rada-Vi
+00001fb0: 6c65 6c61 7d2c 0a20 2020 2074 6974 6c65  lela},.    title
+00001fc0: 3d7b 5468 6520 4675 7a7a 794c 6974 6520  ={The FuzzyLite 
+00001fd0: 4c69 6272 6172 6965 7320 666f 7220 4675  Libraries for Fu
+00001fe0: 7a7a 7920 4c6f 6769 6320 436f 6e74 726f  zzy Logic Contro
+00001ff0: 6c7d 2c0a 2020 2020 7572 6c3d 7b68 7474  l},.    url={htt
+00002000: 7073 3a2f 2f66 757a 7a79 6c69 7465 2e63  ps://fuzzylite.c
+00002010: 6f6d 7d2c 0a20 2020 2079 6561 723d 7b32  om},.    year={2
+00002020: 3031 387d 0a7d 0a60 6060 0a0a 2a2a 2a0a  018}.}.```..***.
+00002030: 0a66 757a 7a79 6c69 7465 2672 6567 3b20  .fuzzylite&reg; 
+00002040: 6973 2061 2072 6567 6973 7465 7265 6420  is a registered 
+00002050: 7472 6164 656d 6172 6b20 6f66 2046 757a  trademark of Fuz
+00002060: 7a79 4c69 7465 203c 6272 3e0a 6a66 757a  zyLite <br>.jfuz
+00002070: 7a79 6c69 7465 2674 7261 6465 3b2c 2070  zylite&trade;, p
+00002080: 7966 757a 7a79 6c69 7465 2674 7261 6465  yfuzzylite&trade
+00002090: 3b20 616e 6420 5174 4675 7a7a 794c 6974  ; and QtFuzzyLit
+000020a0: 6526 7472 6164 653b 2061 7265 2074 7261  e&trade; are tra
+000020b0: 6465 6d61 726b 7320 6f66 2046 757a 7a79  demarks of Fuzzy
+000020c0: 4c69 7465 0a                             Lite.
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/activation.py` & `pyfuzzylite-8.0.3/fuzzylite/activation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = [
     "Activation",
     "General",
     "First",
     "Last",
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/benchmark.py` & `pyfuzzylite-8.0.3/fuzzylite/benchmark.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
 
 from __future__ import annotations
 
 __all__ = ["Benchmark"]
 
 import inspect
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/defuzzifier.py` & `pyfuzzylite-8.0.3/fuzzylite/defuzzifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = [
     "Defuzzifier",
     "IntegralDefuzzifier",
     "Bisector",
     "Centroid",
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/engine.py` & `pyfuzzylite-8.0.3/fuzzylite/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = ["Engine"]
 
 import enum
 from collections.abc import Iterable
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/obstacle_avoidance.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/obstacle_avoidance.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/obstacle_avoidance.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/tipper.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/tipper.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/hybrid/tipper.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/all_terms.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/all_terms.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/all_terms.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/laundry.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/laundry.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/laundry.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam21.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam21.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam21.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam22.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam22.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/mam22.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/shower.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/shower.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/shower.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank2.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank2.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tank2.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/matlab/tipper1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/obstacle_avoidance.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/obstacle_avoidance.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/obstacle_avoidance.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/investment_portfolio.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/investment_portfolio.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/investment_portfolio.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_chained.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_chained.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_chained.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_inverse.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_inverse.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/mamdani/simple_dimmer_inverse.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/approximation.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/approximation.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/approximation.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/invkine2.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/juggler.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/juggler.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/juggler.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/membrn2.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slbb.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slbb.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slbb.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcp1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tanksg.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/matlab/tippersg.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/simple_dimmer.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/simple_dimmer.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/takagi_sugeno/simple_dimmer.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/__init__.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/arc.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/arc.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/arc.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/bell.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/bell.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/bell.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/binary.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/binary.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/binary.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/concave.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/concave.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/concave.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/constant.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/constant.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/constant.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/cosine.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/cosine.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/cosine.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/discrete.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/discrete.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/discrete.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/function.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/function.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/function.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian_product.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian_product.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/gaussian_product.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/linear.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/linear.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/linear.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/pi_shape.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/pi_shape.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/pi_shape.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/ramp.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/ramp.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/ramp.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/rectangle.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/rectangle.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/rectangle.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/semi_ellipse.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/semi_ellipse.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/semi_ellipse.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_difference.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_difference.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_difference.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_product.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_product.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/sigmoid_product.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/spike.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/spike.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/spike.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/trapezoid.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/trapezoid.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/trapezoid.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/triangle.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/triangle.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/triangle.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/zs_shape.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/zs_shape.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/terms/zs_shape.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.fld` & `pyfuzzylite-8.0.3/fuzzylite/examples/tsukamoto/tsukamoto.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.fll` & `pyfuzzylite-8.0.3/fuzzylite/examples/tsukamoto/tsukamoto.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.py` & `pyfuzzylite-8.0.3/fuzzylite/examples/tsukamoto/tsukamoto.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/fuzzylite/exporter.py` & `pyfuzzylite-8.0.3/fuzzylite/exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = ["Exporter", "FllExporter", "PythonExporter", "FldExporter"]
 
 import enum
 import io
 import typing
@@ -382,19 +376,20 @@
 
         Args:
             code: code to format.
             **kwargs: keyword arguments to pass to `black.Mode`
         Returns:
             code formatted if `black` is installed, otherwise the code without format
         """
-        kwargs = {"line_length": 100} | kwargs
         try:
             import black
 
-            return black.format_str(code, mode=black.Mode(**kwargs))
+            kwargs = dict(line_length=100) | kwargs
+            formatted = black.format_str(code, mode=black.Mode(**kwargs))
+            return formatted
         except ModuleNotFoundError:
             settings.logger.error("expected `black` module to be installed, but could not be found")
         except ValueError:  # black.parsing.InvalidInput
             raise
         return code
 
     def encapsulate(self, instance: Any) -> str:
@@ -410,15 +405,14 @@
         from .engine import Engine
         from .library import representation
 
         code = f"{representation.import_statement()}\n\n"
         if isinstance(instance, Engine):
             code += f"""\
 class {Op.pascal_case(instance.name)}:
-
     def __init__(self) -> None:
         self.engine = {repr(instance)}
 """
         else:
             code += f"""\
 def create() -> {Op.class_name(instance, qualname=True)}:
     return {repr(instance)}
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/factory.py` & `pyfuzzylite-8.0.3/fuzzylite/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = [
     "ConstructionFactory",
     "CloningFactory",
     "ActivationFactory",
     "DefuzzifierFactory",
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/hedge.py` & `pyfuzzylite-8.0.3/fuzzylite/hedge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = [
     "Hedge",
     "Any",
     "Extremely",
     "Not",
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/importer.py` & `pyfuzzylite-8.0.3/fuzzylite/importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = ["Importer", "FllImporter"]
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import overload
@@ -379,28 +373,24 @@
         parameters = values[1] if len(values) > 1 else None
         result = settings.factory_manager.defuzzifier.construct(name)
         if parameters:
             result.configure(parameters)
         return result
 
     @overload
-    def component(self, cls: type[Activation], fll: str) -> Activation | None:
-        ...
+    def component(self, cls: type[Activation], fll: str) -> Activation | None: ...
 
     @overload
-    def component(self, cls: type[Defuzzifier], fll: str) -> Defuzzifier | None:
-        ...
+    def component(self, cls: type[Defuzzifier], fll: str) -> Defuzzifier | None: ...
 
     @overload
-    def component(self, cls: type[SNorm], fll: str) -> SNorm | None:
-        ...
+    def component(self, cls: type[SNorm], fll: str) -> SNorm | None: ...
 
     @overload
-    def component(self, cls: type[TNorm], fll: str) -> TNorm | None:
-        ...
+    def component(self, cls: type[TNorm], fll: str) -> TNorm | None: ...
 
     def component(
         self,
         cls: type[Activation | Defuzzifier | TNorm | SNorm],
         fll: str,
     ) -> Activation | Defuzzifier | TNorm | SNorm | None:
         """Return the component described using the FuzzyLite Language.
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/library.py` & `pyfuzzylite-8.0.3/fuzzylite/library.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = [
     "information",
     "Information",
     "settings",
     "Settings",
@@ -71,21 +65,19 @@
     Returns:
         converted value
     """
     return settings.float_type(x)  # type: ignore
 
 
 @overload
-def scalar(x: Sequence[Any] | Array[Any], /) -> ScalarArray:
-    ...
+def scalar(x: Sequence[Any] | Array[Any], /) -> ScalarArray: ...
 
 
 @overload
-def scalar(x: Any, /) -> Scalar:
-    ...
+def scalar(x: Any, /) -> Scalar: ...
 
 
 def scalar(x: Sequence[Any] | Array[Any] | Any, /, **kwargs: Any) -> ScalarArray | Scalar:
     """Convert the values into a floating point value defined by the library.
 
     Args:
         x: value to convert.
@@ -248,16 +240,19 @@
     """Information about the library."""
 
     name: Final[str] = "fuzzylite"
     description: Final[str] = "a fuzzy logic control library in Python"
     license: Final[str] = "FuzzyLite License"
     author: Final[str] = "Juan Rada-Vilela, PhD"
     author_email: Final[str] = "jcrada@fuzzylite.com"
-    company: Final[str] = "FuzzyLite Limited"
+    company: Final[str] = "FuzzyLite"
     website: Final[str] = "https://fuzzylite.com/"
+    copyright: Final[str] = (
+        "Copyright (C) 2010-2024 FuzzyLite by Juan Rada-Vilela. All rights reserved."
+    )
 
     def __repr__(self) -> str:
         """Return code to construct the information in Python.
 
         Returns:
             code to construct the information in Python
         """
@@ -268,15 +263,15 @@
     @property
     def version(self) -> str:
         """Automatic version of the library handled by poetry using `[tool.poetry_bumpversion.file."fuzzylite/library.py"]`.
 
         Returns:
             version of the library
         """
-        __version__ = "8.0.2"
+        __version__ = "8.0.3"
         return __version__
 
 
 information: Final = Information()
 
 
 class Representation(reprlib.Repr):
@@ -374,15 +369,15 @@
 
         Returns:
             Python code to use the constructor of the object.
         """
         arguments = self.construction_arguments(
             x, fields=fields, positional=positional, cast_as=cast_as
         )
-        return f"{self.package_of((cast_as or x))}{(cast_as or x.__class__).__name__}({', '.join(arguments)})"
+        return f"{self.package_of(cast_as or x)}{(cast_as or x.__class__).__name__}({', '.join(arguments)})"
 
     def construction_arguments(  # noqa: D417 # Missing argument description in the docstring: `self`
         self,
         x: T,
         /,
         fields: dict[str, Any] | None = None,
         *,
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/norm.py` & `pyfuzzylite-8.0.3/fuzzylite/norm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
 
 from __future__ import annotations
 
 __all__ = [
     "Norm",
     "TNorm",
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/operation.py` & `pyfuzzylite-8.0.3/fuzzylite/operation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = ["Operation", "Op"]
 
 import builtins
 import importlib
 import importlib.util
@@ -408,62 +402,59 @@
 
     @staticmethod
     @overload
     def glob_examples(
         return_type: Literal["module"],
         module: ModuleType | None = None,
         recursive: bool = True,
-    ) -> Iterable[ModuleType]:
-        ...
+    ) -> Iterable[ModuleType]: ...
 
     @staticmethod
     @overload
     def glob_examples(
         return_type: Literal["engine"],
         module: ModuleType | None = None,
         recursive: bool = True,
-    ) -> Iterable[Engine]:
-        ...
+    ) -> Iterable[Engine]: ...
 
     @staticmethod
     @overload
     def glob_examples(
         return_type: Literal["dataset"] | Literal["fld"],
         module: ModuleType | None = None,
         recursive: bool = True,
-    ) -> Iterable[ScalarArray]:
-        ...
+    ) -> Iterable[ScalarArray]: ...
 
     @staticmethod
     @overload
     def glob_examples(
         return_type: Literal["language"] | Literal["fll"],
         module: ModuleType | None = None,
         recursive: bool = True,
-    ) -> Iterable[str]:
-        ...
+    ) -> Iterable[str]: ...
 
     @staticmethod
     @overload
     def glob_examples(
         return_type: Literal["files"],
         module: ModuleType | None = None,
         recursive: bool = True,
-    ) -> Iterable[Path]:
-        ...
+    ) -> Iterable[Path]: ...
 
     @staticmethod
     def glob_examples(
-        return_type: Literal["module"]
-        | Literal["engine"]
-        | Literal["dataset"]
-        | Literal["fld"]
-        | Literal["language"]
-        | Literal["fll"]
-        | Literal["files"] = "engine",
+        return_type: (
+            Literal["module"]
+            | Literal["engine"]
+            | Literal["dataset"]
+            | Literal["fld"]
+            | Literal["language"]
+            | Literal["fll"]
+            | Literal["files"]
+        ) = "engine",
         module: ModuleType | None = None,
         recursive: bool = True,
     ) -> Iterable[ModuleType | Engine | ScalarArray | str | Path]:
         """Glob the examples (alphabetically and in ascending order) returning the specified type.
 
         Args:
             return_type: type of objects to return
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/rule.py` & `pyfuzzylite-8.0.3/fuzzylite/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = [
     "Expression",
     "Proposition",
     "Operator",
     "Antecedent",
@@ -325,15 +319,15 @@
         stack: deque[Expression] = deque()
 
         proposition: Proposition | None = None
         variables = {v.name: v for v in engine.variables}
         token: str | None = None
         for token in postfix.split():
             if state & s_variable:
-                variable = variables.get(token, None)
+                variable = variables.get(token)
                 if variable:
                     proposition = Proposition(variable)
                     stack.append(proposition)
                     state = s_is
                     settings.logger.debug(f"token '{token}' is a variable")
                     continue
 
@@ -350,15 +344,15 @@
                     proposition.hedges.append(hedge)  # type: ignore
                     state = s_variable | s_and_or if isinstance(hedge, Any) else s_hedge | s_term
                     settings.logger.debug(f"token '{token} is hedge")
                     continue
 
             if state & s_term:
                 terms = {t.name: t for t in proposition.variable.terms}  # type: ignore
-                term = terms.get(token, None)
+                term = terms.get(token)
                 if term:
                     proposition.term = term  # type: ignore
                     state = s_variable | s_and_or
                     settings.logger.debug(f"token '{token} is term")
                     continue
 
             if state & s_and_or:
@@ -605,15 +599,15 @@
 
         proposition: Proposition | None = None
         conclusions: list[Proposition] = []
         output_variables = {v.name: v for v in engine.output_variables}
         token: str | None = None
         for token in self.text.split():
             if state & s_variable:
-                variable = output_variables.get(token, None)
+                variable = output_variables.get(token)
                 if variable:
                     proposition = Proposition(variable)
                     conclusions.append(proposition)
                     state = s_is
                     continue
 
             if state & s_is and Rule.IS == token:
@@ -626,15 +620,15 @@
                     hedge = factory.construct(token)
                     proposition.hedges.append(hedge)  # type: ignore
                     state = s_hedge | s_term
                     continue
 
             if state & s_term:
                 terms = {t.name: t for t in proposition.variable.terms}  # type: ignore
-                term = terms.get(token, None)
+                term = terms.get(token)
                 if term:
                     proposition.term = term  # type: ignore
                     state = s_and | s_with
                     continue
 
             if state & s_and and Rule.AND == token:
                 state = s_variable
@@ -956,20 +950,18 @@
 
         Returns:
             iterator of the rules
         """
         return iter(self.rules)
 
     @overload
-    def __getitem__(self, item: int) -> Rule:
-        ...
+    def __getitem__(self, item: int) -> Rule: ...
 
     @overload
-    def __getitem__(self, item: slice) -> list[Rule]:
-        ...
+    def __getitem__(self, item: slice) -> list[Rule]: ...
 
     def __getitem__(self, item: int | slice) -> Rule | list[Rule]:
         """Allow indexing rules in rule block (eg, `rule_block[0]`).
 
         Args:
             item: rule index or slice
 
@@ -1040,7 +1032,18 @@
         """Reload all the rules in the rule block.
 
         Args:
             engine: engine where this rule block is registered.
         """
         self.unload_rules()
         self.load_rules(engine)
+
+    def rule(self, index: int, /) -> Rule:
+        """Get the rule at the index.
+
+        Args:
+            index: index of the rule.
+
+        Returns:
+            rule at the index
+        """
+        return self.rules[index]
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/term.py` & `pyfuzzylite-8.0.3/fuzzylite/term.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = [
     "Activated",
     "Aggregated",
     "Arc",
     "Bell",
@@ -1189,18 +1183,20 @@
             list of values in the form `[x1,y1, ..., xn, yn]`.
         """
         return self.values.flatten().tolist()  # type: ignore
 
     @staticmethod
     def create(
         name: str,
-        xy: str
-        | Sequence[Floatable]
-        | tuple[Sequence[Floatable], Sequence[Floatable]]
-        | dict[Floatable, Floatable],
+        xy: (
+            str
+            | Sequence[Floatable]
+            | tuple[Sequence[Floatable], Sequence[Floatable]]
+            | dict[Floatable, Floatable]
+        ),
         height: float = 1.0,
     ) -> Discrete:
         """Create a discrete term from the parameters.
 
         Args:
             name: name of the term
             xy: coordinates
@@ -2754,31 +2750,31 @@
         """
 
         def __init__(
             self,
             element: Function.Element | None = None,
             variable: str = "",
             constant: float = nan,
-            right: Function.Node | None = None,
             left: Function.Node | None = None,
+            right: Function.Node | None = None,
         ) -> None:
             """Constructor.
 
             Args:
                 element: node refers to a function or an operator
                 variable: node refers to a variable by name
                 constant: node refers to an arbitrary floating-point value
                 right: node has an expression tree on the right
                 left: node has an expression tree on the left.
             """
             self.element = element
             self.variable = variable
             self.constant = constant
-            self.right = right
             self.left = left
+            self.right = right
 
         def __repr__(self) -> str:
             """Return the code to construct the node in Python.
 
             Returns:
                 code to construct the node in Python.
             """
@@ -2817,17 +2813,18 @@
             """
             result = scalar(nan)
             if self.element:
                 arity = self.element.arity
                 if arity == 0:
                     result = self.element.method()
                 elif arity == 1:
-                    if not self.right:
-                        raise ValueError("expected a right node, but found none")
-                    result = self.element.method(self.right.evaluate(local_variables))
+                    if node := (self.left or self.right):
+                        result = self.element.method(node.evaluate(local_variables))
+                    else:
+                        raise ValueError("expected a node, but found none")
                 elif arity == 2:
                     if not self.right:
                         raise ValueError("expected a right node, but found none")
                     if not self.left:
                         raise ValueError("expected a left node, but found none")
                     result = self.element.method(
                         self.left.evaluate(local_variables),
@@ -2894,15 +2891,18 @@
                 children.append(self.infix(node.right))
 
             is_function = node.element and node.element.type == Function.Element.Type.Function
 
             if is_function:
                 result = node.value() + f" ( {' '.join(children)} )"
             else:  # is operator
-                result = f" {node.value()} ".join(children)
+                if len(children) == 1:
+                    result = f"{node.value()} {children[0]}"
+                else:
+                    result = f" {node.value()} ".join(children)
 
             return result
 
         def postfix(self, node: Function.Node | None = None) -> str:
             """Return the postfix notation of the node.
 
             Args:
@@ -3139,17 +3139,16 @@
         for token in formula.split():
             if settings.debugging:
                 settings.logger.debug("=" * 20)
                 settings.logger.debug(f"formula: {formula}")
                 settings.logger.debug(f"queue: {queue}")
                 settings.logger.debug(f"stack: {stack}")
 
-            element: Function.Element | None = (
-                factory.objects[token] if token in factory.objects else None
-            )
+            element: Function.Element | None = factory.objects.get(token)
+
             is_operand = not element and token not in {"(", ")", ","}
 
             if is_operand:
                 queue.append(token)
 
             elif element and element.is_function():
                 stack.append(token)
@@ -3215,17 +3214,15 @@
             SyntaxError: when the formula has syntax errors.
         """
         postfix = cls.infix_to_postfix(formula)
         stack: list[Function.Node] = []
         factory = settings.factory_manager.function
 
         for token in postfix.split():
-            element: Function.Element | None = (
-                factory.objects[token] if token in factory.objects else None
-            )
+            element: Function.Element | None = factory.objects.get(token)
             is_operand = not element and token not in {"(", ")", ","}
 
             if element:
                 if element.arity > len(stack):
                     raise SyntaxError(
                         f"function element {element.name} has arity {element.arity}, "
                         f"but the size of the stack is {len(stack)}"
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite/variable.py` & `pyfuzzylite-8.0.3/fuzzylite/variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 __all__ = ["Variable", "InputVariable", "OutputVariable"]
 
 import contextlib
 from collections.abc import Iterable, Iterator
 from typing import overload
@@ -77,20 +71,18 @@
     #         return self[item]
     #     except ValueError:
     #         raise AttributeError(
     #             f"'{self.__class__.__name__}' object has no attribute '{item}'"
     #         ) from None
 
     @overload
-    def __getitem__(self, item: int | str) -> Term:
-        ...
+    def __getitem__(self, item: int | str) -> Term: ...
 
     @overload
-    def __getitem__(self, item: slice) -> list[Term]:
-        ...
+    def __getitem__(self, item: slice) -> list[Term]: ...
 
     def __getitem__(self, item: int | str | slice) -> Term | list[Term]:
         """Allow indexing terms by index, name, or slices (eg, `engine["power"]["low"]`).
 
         Args:
             item: index, name, or slice of terms
```

### Comparing `pyfuzzylite-8.0.2/fuzzylite.png` & `pyfuzzylite-8.0.3/fuzzylite.png`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/noxfile.py` & `pyfuzzylite-8.0.3/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
 
 import nox
 
 nox.options.sessions = ["check", "freeze", "install", "lint", "test"]
 
 PYTHON_FILES = ["fuzzylite/", "tests/", "noxfile.py"]
@@ -29,56 +22,74 @@
     """Check the `pyproject.toml` is valid."""
     session.run(*"poetry check".split(), external=True)
 
 
 @nox.session(python=False)
 def format(session: nox.Session) -> None:
     """Run code formatting."""
-    files = PYTHON_FILES
+    formatters = {
+        "ruff": format_ruff,
+        "black": format_black,
+    }
+    posargs = list(session.posargs)
+    if not posargs:
+        posargs = list(formatters.keys())
+    for formatter in posargs:
+        formatters[formatter](session)
+
 
+@nox.session(python=False)
+def format_black(session: nox.Session) -> None:
+    """Run code formatting with black."""
+    files = PYTHON_FILES
     session.run(*"black --version".split(), external=True)
     session.run("black", *files, external=True)
 
+
+@nox.session(python=False)
+def format_ruff(session: nox.Session) -> None:
+    """Run code formatting with ruff."""
+    files = PYTHON_FILES
     session.run(*"ruff --version".split(), external=True)
-    session.run(*"ruff --fix".split(), *files, external=True)
+    session.run(*"ruff format".split(), *files, external=True)
 
 
 @nox.session(python=False)
 def lint(session: nox.Session) -> None:
     """Run static code analysis and checks format is correct."""
     linters = {
-        "black": "lint_black",
-        "ruff": "lint_ruff",
-        "pyright": "lint_pyright",
-        "mypy": "lint_mypy",
-        "markdown": "lint_markdown",
+        "ruff": lint_ruff,
+        "black": lint_black,
+        "pyright": lint_pyright,
+        "mypy": lint_mypy,
+        "markdown": lint_markdown,
     }
     # Case 1: posargs is empty, run all linters
     # Case 2: posargs is not empty, run only the specified linters
     posargs = list(session.posargs)
     if not posargs:
         posargs = list(linters.keys())
     for linter in posargs:
-        session.notify(linters[linter])
+        linters[linter](session)
 
 
 @nox.session(python=False)
 def lint_black(session: nox.Session) -> None:
     """Run black linter."""
     files = PYTHON_FILES
     session.run(*"black --version".split(), external=True)
     session.run(*"black --check".split(), *files, external=True)
 
 
 @nox.session(python=False)
 def lint_ruff(session: nox.Session) -> None:
     """Run ruff linter."""
     files = PYTHON_FILES
-    session.run(*"ruff check".split(), *files, external=True)
     session.run(*"ruff --version".split(), external=True)
+    session.run(*"ruff check".split(), *files, external=True)
 
 
 @nox.session(python=False)
 def lint_pyright(session: nox.Session) -> None:
     """Run pyright linter."""
     session.run(*"pyright --version".split(), external=True)
     session.run("pyright", external=True)
```

### Comparing `pyfuzzylite-8.0.2/pyproject.toml` & `pyfuzzylite-8.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyfuzzylite"
-version = "8.0.2"
+version = "8.0.3"
 description = "a fuzzy logic control library in Python"
 license = "Proprietary"
 readme = "README.md"
 keywords = ["fuzzy logic control", "soft computing", "artificial intelligence"]
 authors = ["Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>"]
 maintainers = ["Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>"]
 repository = "https://github.com/fuzzylite/pyfuzzylite.git"
@@ -44,64 +44,60 @@
 ]
 
 [tool.poetry_bumpversion.file."fuzzylite/library.py"]
 [tool.poetry_bumpversion.file."tests/test_library.py"]
 
 [[tool.poetry_bumpversion.replacements]]
 files = ["README.md", "docs/index.md"]
-search = "# pyfuzzylite {current_version}"
-replace = "# pyfuzzylite {new_version}"
+search = "<h1>pyfuzzylite {current_version}</h1>"
+replace = "<h1>pyfuzzylite {new_version}</h1>"
 
 [[tool.poetry.packages]]
 include = "fuzzylite"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/fuzzylite/pyfuzzylite"
 Documentation = "https://fuzzylite.github.io/pyfuzzylite/"
 "Bug Tracker" = "https://github.com/fuzzylite/pyfuzzylite/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.20" # Numeric manipulation and vectorisation
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.11.0" # Code formatting
-#black = { extras = [
-#    "jupyter",
-#], version = "^23.11.0" }
+black = "^24.4.2" # Code formatting
 coverage = "^7.2.3" # Code coverage
-#jupyter-contrib-nbextensions = "^0.7.0" # Extensions for Jupyter Notebooks
-#kaleido = "0.2.1" # Use static charts with plotly
 mkdocs-material = "^9.1.21" # Documentation with material theme for mkdocs
 mkdocstrings = { extras = [
     "python",
 ], version = "^0.22.0" } # Source code documentation for mkdocs
-mypy = "^1.2.0" # Static code analysis
-#notebook = "6.5.6" # Jupyter Notebooks
-#plotly = "^5.18.0" # Interactive plots
+mypy = "^1.10.0" # Static code analysis
 poetry-bumpversion = "^0.3.0" # Version management
 pymarkdownlnt = "^0.9.12" # Markdown linter
-pyright = "^1.1.305" # Static code analysis
+pyright = "^1.1.362" # Static code analysis
 pytest = "^7.3.1" # Test driven development
 pytest-benchmark = "^4.0.0" # Local benchmarks
 pytest-codspeed = "^2.0.1" # Cloud benchmarks
-ruff = "^0.0.256" # Code formatting
-#twine = "^4.0.2" # Publish package
+ruff = "^0.4.4" # Code formatting
 
-# Packages below are ground truth for version management. See requirements.txt.
-poetry = "~=1.7.1" # Build management
-nox = "~=2023.4.22" # Command-line build management
+# Packages below are ground truth for version management. See requirements-dev.txt.
+# poetry = "~=1.8.3" # Build management
+# nox = "~=2024.4.15" # Command-line build management
 
 
 
 [tool.black]
 target-version = ["py39"]
 line-length = 100
 
 [tool.ruff]
+target-version = "py39"
+line-length = 100
+
+[tool.ruff.lint]
 # https://beta.ruff.rs/docs/rules/
 select = [
     "A", # flake8-builtins
     "ANN", # flake8-annotations
     # "ARG", # flake8-unused-arguments
     "B", # flake8-bugbear
     # "C",  # flake8-comprehensions
@@ -189,32 +185,30 @@
     #    "D400", # First line should end with a period
     #    "D415", # First line should end with a period, question mark, or exclamation point
     #    "W291", # Trailing whitespace # hinders markdown
 ]
 
 exclude = []
 
-# Same as Black.
-line-length = 100
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-target-version = "py39"
 
-[tool.ruff.per-file-ignores]
+
+[tool.ruff.lint.per-file-ignores]
 "fuzzylite/examples/**/*.py" = [
     "D101", # Missing docstring in public class
     "D107", # Missing docstring in `__init__`
 ]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 10
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.pyright]
 include = ["fuzzylite/", "noxfile.py", "tests/"]
 pythonVersion = "3.9"
 # strict =  ["fuzzylite/", "noxfile.py", "tests/"] # This is too strict, but useful at times
 venv = ".venv"
@@ -252,7 +246,9 @@
 plugins.line-length.line_length = 120
 # docs/index.md:324:1: MD046: Code block style [Expected: indented; Actual: fenced] (code-block-style)
 plugins.MD046.enabled = false
 # MD033: Inline HTML [Element: a] (no-inline-html)
 plugins.MD033.enabled = false
 # MD034: Bare URL used (no-bare-urls)
 plugins.MD034.enabled = false
+# MD041: First line in file should be a top level heading
+plugins.MD041.enabled = false
```

### Comparing `pyfuzzylite-8.0.2/tests/assert_component.py` & `pyfuzzylite-8.0.3/tests/assert_component.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import unittest
 from typing import Any, Generic, TypeVar
 
 import numpy as np
 from typing_extensions import Self
```

### Comparing `pyfuzzylite-8.0.2/tests/notebooks/Hedges.ipynb` & `pyfuzzylite-8.0.3/tests/notebooks/Hedges.ipynb`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/tests/notebooks/Norms.ipynb` & `pyfuzzylite-8.0.3/tests/notebooks/Norms.ipynb`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/tests/notebooks/Terms.ipynb` & `pyfuzzylite-8.0.3/tests/notebooks/Terms.ipynb`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.2/tests/test_activation.py` & `pyfuzzylite-8.0.3/tests/test_activation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import unittest
 from unittest.mock import MagicMock
 
 import numpy as np
 
@@ -161,17 +155,17 @@
         """Asserts the general activation is correct."""
         # All combinations
         expected_a = [True] * 4 + [False] * 4
         expected_b = 2 * ([True] * 2 + [False] * 2)
         expected_c = [True, False] * 4
 
         ActivationAssert(self, fl.RuleBlock()).given(
-            rule="a", activation_degree=fl.array(expected_a, dtype=np.float_)
-        ).given(rule="b", activation_degree=fl.array(expected_b, dtype=np.float_)).given(
-            rule="c", activation_degree=fl.array(expected_c, dtype=np.float_)
+            rule="a", activation_degree=fl.array(expected_a, dtype=np.float64)
+        ).given(rule="b", activation_degree=fl.array(expected_b, dtype=np.float64)).given(
+            rule="c", activation_degree=fl.array(expected_c, dtype=np.float64)
         ).activate(
             fl.General()
         ).then_triggers(
             rules={"a": expected_a, "b": expected_b, "c": expected_c}
         )
 
         unsupported_activations = [
@@ -180,17 +174,17 @@
             fl.Highest(),
             fl.Lowest(),
             fl.Proportional(),
             fl.Threshold(),
         ]
         for activation in unsupported_activations:
             ActivationAssert(self, fl.RuleBlock()).given(
-                rule="a", activation_degree=fl.array(expected_a, dtype=np.float_)
-            ).given(rule="b", activation_degree=fl.array(expected_b, dtype=np.float_)).given(
-                rule="c", activation_degree=fl.array(expected_c, dtype=np.float_)
+                rule="a", activation_degree=fl.array(expected_a, dtype=np.float64)
+            ).given(rule="b", activation_degree=fl.array(expected_b, dtype=np.float64)).given(
+                rule="c", activation_degree=fl.array(expected_c, dtype=np.float64)
             ).activate_fails(
                 activation
             )
 
     def test_first_activation(self) -> None:
         """Asserts the first activation is correct."""
         BaseAssert(self, fl.First()).repr_is("fl.First(rules=1, threshold=0.0)").exports_fll(
```

### Comparing `pyfuzzylite-8.0.2/tests/test_benchmark.py` & `pyfuzzylite-8.0.3/tests/test_benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 import time
 import unittest
 
 import numpy as np
 
 import fuzzylite as fl
 from fuzzylite.examples.mamdani import simple_dimmer
```

### Comparing `pyfuzzylite-8.0.2/tests/test_benchmark_codspeed.py` & `pyfuzzylite-8.0.3/tests/test_benchmark_codspeed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import inspect
 from types import ModuleType
 from typing import Any, Callable
 
 from pytest_codspeed.plugin import BenchmarkFixture
```

### Comparing `pyfuzzylite-8.0.2/tests/test_benchmark_pytest.py` & `pyfuzzylite-8.0.3/tests/test_benchmark_pytest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
 
 from __future__ import annotations
 
 import inspect
 from types import ModuleType
 from typing import Any, Callable
```

### Comparing `pyfuzzylite-8.0.2/tests/test_defuzzifier.py` & `pyfuzzylite-8.0.3/tests/test_defuzzifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import re
 import unittest
 from typing import Any
 
 import numpy as np
@@ -85,20 +79,15 @@
                 expected_vector,
                 atol=fl.settings.atol,
                 rtol=fl.settings.rtol,
             )
         return self
 
 
-class NanTerm(fl.Term):
-    """A term that always returns NaN as its membership value."""
-
-    def membership(self, x: Scalar) -> Scalar:
-        """Returns NaN as the membership value of the term."""
-        return np.full_like(x, np.nan)
+NaN = fl.Constant
 
 
 class TestDefuzzifier(unittest.TestCase):
     """Tests the defuzzifiers."""
 
     def test_bisector(self) -> None:
         """Test the bisector defuzzifier."""
@@ -153,15 +142,15 @@
                 ): -0.001
             },
         )
 
         DefuzzifierAssert(self, fl.Bisector()).defuzzifies(
             0,
             2,
-            {NanTerm(): np.nan},  # mean of range of variable
+            {NaN(): np.nan},  # mean of range of variable
         )
 
     def test_centroid(self) -> None:
         """Test the centroid defuzzifier."""
         DefuzzifierAssert(self, fl.Centroid()).exports_fll("Centroid").has_attribute(
             resolution=1000
         ).configured_as("200").has_parameters("200").exports_fll("Centroid 200")
@@ -203,15 +192,15 @@
                     ],
                 ): 0.6896552,
             },
         )
         DefuzzifierAssert(self, fl.Centroid()).defuzzifies(
             -1,
             1,
-            {NanTerm(): np.nan},
+            {NaN(): np.nan},
         )
 
     def test_som_defuzzifier(self) -> None:
         """Test the Smallest of Maximum defuzzifier."""
         DefuzzifierAssert(self, fl.SmallestOfMaximum()).exports_fll(
             "SmallestOfMaximum"
         ).has_attribute(resolution=1000).configured_as("200").exports_fll("SmallestOfMaximum 200")
@@ -273,15 +262,15 @@
                 term: 0.5,
                 fl.Trapezoid("", 0.0, 0.2, 0.4, 0.6): 0.2,
             },
         )
         DefuzzifierAssert(self, fl.SmallestOfMaximum()).defuzzifies(
             -1,
             1,
-            {NanTerm(): np.nan},
+            {NaN(): np.nan},
         )
 
     def test_lom_defuzzifier(self) -> None:
         """Test the Largest of Maximum defuzzifier."""
         DefuzzifierAssert(self, fl.LargestOfMaximum()).exports_fll(
             "LargestOfMaximum"
         ).has_attribute(resolution=1000).configured_as("200").has_parameters("200").exports_fll(
@@ -345,15 +334,15 @@
                 term: 0.9,
                 fl.Trapezoid("", 0.0, 0.2, 0.4, 0.6): 0.4,
             },
         )
         DefuzzifierAssert(self, fl.LargestOfMaximum()).defuzzifies(
             -1,
             1,
-            {NanTerm(): np.nan},
+            {NaN(): np.nan},
         )
 
     def test_mom_defuzzifier(self) -> None:
         """Test the Largest of Maximum defuzzifier."""
         DefuzzifierAssert(self, fl.MeanOfMaximum()).exports_fll("MeanOfMaximum").has_attribute(
             resolution=1000
         ).configured_as("200").has_parameters("200").exports_fll("MeanOfMaximum 200")
@@ -416,15 +405,15 @@
                 term: 0.7,
                 fl.Trapezoid("", 0.0, 0.2, 0.4, 0.6): 0.3,
             },
         )
         DefuzzifierAssert(self, fl.MeanOfMaximum()).defuzzifies(
             -1,
             1,
-            {NanTerm(): np.nan},
+            {NaN(): np.nan},
         )
 
     def test_weighted_defuzzifier(self) -> None:
         """Test the weighted defuzzifier and its methods."""
 
         class BaseWeightedDefuzzifier(fl.WeightedDefuzzifier):
             def defuzzify(
@@ -617,15 +606,15 @@
                     terms=[
                         fl.Activated(fl.Constant("A", 1.0), 1.0),
                         fl.Activated(fl.Constant("B", -2.0), 1.0),
                         fl.Activated(fl.Constant("C", -3.0), 0.5),
                         fl.Activated(fl.Constant("C", -3.0), 0.5),
                     ],
                     aggregation=fl.AlgebraicSum(),
-                ): ((1 * 1 + 1 * -2 + (0.5 + 0.5 - (0.25)) * -3) / (1 + 1 + (0.5 + 0.5 - 0.25))),
+                ): -1.181818,  # ((1 * 1 + 1 * -2 + (0.5 + 0.5 - (0.25)) * -3) / (1 + 1 + (0.5 + 0.5 - 0.25))),
             },
             vectorized=False,
         )
 
     def test_weighted_sum(self) -> None:
         """Test the weighted sum defuzzifier."""
         DefuzzifierAssert(self, fl.WeightedSum()).exports_fll("WeightedSum")
```

### Comparing `pyfuzzylite-8.0.2/tests/test_documentation.py` & `pyfuzzylite-8.0.3/tests/test_documentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import shutil
 import unittest
 from pathlib import Path
 
 import fuzzylite as fl
```

### Comparing `pyfuzzylite-8.0.2/tests/test_engine.py` & `pyfuzzylite-8.0.3/tests/test_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import unittest
 from typing import cast
 
 import black
 import numpy as np
@@ -597,15 +591,15 @@
         np.testing.assert_allclose(
             [fl.nan, 0.75, 0.5, 0.25, fl.nan],
             engine.Power.value,  # type: ignore
         )
 
         # Non-existing component by name
         with self.assertRaises(AttributeError) as error:
-            engine.Variable  # type: ignore
+            engine.Variable  # type: ignore # noqa: B018
         self.assertEqual("'Engine' object has no attribute 'Variable'", str(error.exception))
 
         # engine's members are retrieved first
         engine.name = "Test my name"
         engine.input_variables.append(fl.InputVariable("name"))
         self.assertEqual("Test my name", engine.name)
```

### Comparing `pyfuzzylite-8.0.2/tests/test_examples.py` & `pyfuzzylite-8.0.3/tests/test_examples.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import inspect
 import logging
 import pathlib
 import unittest
 from pathlib import Path
```

### Comparing `pyfuzzylite-8.0.2/tests/test_exporter.py` & `pyfuzzylite-8.0.3/tests/test_exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import io
 import logging
 import os
 import random
 import string
@@ -426,14 +420,36 @@
                 self.assertEqual("None", none_formatted)
                 logger.error.assert_called_with(
                     "expected `black` module to be installed, but could not be found"
                 )
         finally:
             sys.modules["black"] = black  # type: ignore
 
+    def test_black_format_options(self) -> None:
+        """Test overriding black format options."""
+        engine = mamdani.simple_dimmer.SimpleDimmer().engine
+        obtained = fl.PythonExporter().format(repr(engine), line_length=1000)
+        expected = (
+            'fl.Engine(name="SimpleDimmer", '
+            'input_variables=[fl.InputVariable(name="Ambient", minimum=0.0, maximum=1.0, '
+            'lock_range=False, terms=[fl.Triangle("DARK", 0.0, 0.25, 0.5), '
+            'fl.Triangle("MEDIUM", 0.25, 0.5, 0.75), fl.Triangle("BRIGHT", 0.5, 0.75, '
+            '1.0)])], output_variables=[fl.OutputVariable(name="Power", minimum=0.0, '
+            "maximum=1.0, lock_range=False, lock_previous=False, default_value=fl.nan, "
+            "aggregation=fl.Maximum(), defuzzifier=fl.Centroid(), "
+            'terms=[fl.Triangle("LOW", 0.0, 0.25, 0.5), fl.Triangle("MEDIUM", 0.25, 0.5, '
+            '0.75), fl.Triangle("HIGH", 0.5, 0.75, 1.0)])], '
+            'rule_blocks=[fl.RuleBlock(name="", conjunction=None, disjunction=None, '
+            'implication=fl.Minimum(), activation=fl.General(), rules=[fl.Rule.create("if '
+            'Ambient is DARK then Power is HIGH"), fl.Rule.create("if Ambient is MEDIUM '
+            'then Power is MEDIUM"), fl.Rule.create("if Ambient is BRIGHT then Power is '
+            'LOW")])])\n'
+        )
+        self.assertEqual(expected, obtained)
+
     def test_none_export(self) -> None:
         """Tests export of None values, like in Norm, Activation, or Defuzzifier."""
         self.assert_that(None, "None\n")
 
     def test_empty_engine(self) -> None:
         """Test an empty engine is exported."""
         engine = fl.Engine(name="Choo Choo", description="My Choo-Choo engine")
```

### Comparing `pyfuzzylite-8.0.2/tests/test_factory.py` & `pyfuzzylite-8.0.3/tests/test_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import itertools
 import unittest
 from collections.abc import Iterable, Sequence
 from typing import (
     Any,
```

### Comparing `pyfuzzylite-8.0.2/tests/test_hedge.py` & `pyfuzzylite-8.0.3/tests/test_hedge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
 
 import fuzzylite as fl
```

### Comparing `pyfuzzylite-8.0.2/tests/test_importer.py` & `pyfuzzylite-8.0.3/tests/test_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import glob
 import os
 import re
 import tempfile
 import unittest
```

### Comparing `pyfuzzylite-8.0.2/tests/test_library.py` & `pyfuzzylite-8.0.3/tests/test_library.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import logging
 import unittest
 
 import numpy as np
 
@@ -27,15 +21,15 @@
 
 class TestLibrary(unittest.TestCase):
     """Test the library class."""
 
     def test_library_exports_dir(self) -> None:
         """Test the library exports expected components."""
         expected = """
-__builtins__ __cached__ __doc__ __file__ __loader__
+__author__ __builtins__ __cached__ __copyright__ __doc__ __file__ __license__ __loader__
 __name__ __package__ __path__ __spec__ __version__
 
 activation Activation First General Highest Last Lowest Proportional Threshold
 
 benchmark Benchmark
 
 defuzzifier Bisector Centroid Defuzzifier IntegralDefuzzifier LargestOfMaximum MeanOfMaximum
@@ -72,18 +66,27 @@
 
 variable InputVariable OutputVariable Variable
 """
         self.assertSetEqual(set(expected.split()), set(vars(fl)))
 
     def test_library_vars(self) -> None:
         """Test the library variables."""
-        __version__ = "8.0.2"
-        self.assertEqual(fl.__name__, "fuzzylite")
-        self.assertEqual(fl.__version__, __version__)
-        self.assertEqual(fl.__doc__, fl.information.description)
+        __version__ = "8.0.3"
+        self.assertTrue("fuzzylite" == fl.__name__ == fl.information.name)
+        self.assertTrue(__version__ == fl.__version__ == fl.information.version)
+        self.assertTrue(
+            "a fuzzy logic control library in Python" == fl.__doc__ == fl.information.description
+        )
+        self.assertTrue("Juan Rada-Vilela, PhD" == fl.__author__ == fl.information.author)
+        self.assertTrue("FuzzyLite License" == fl.__license__ == fl.information.license)
+        self.assertTrue(
+            "Copyright (C) 2010-2024 FuzzyLite by Juan Rada-Vilela. All rights reserved."
+            == fl.__copyright__
+            == fl.information.copyright
+        )
 
     def test_context(self) -> None:
         """Tests the context."""
         # float_type
         self.assertEqual(fl.settings.float_type, np.float64)
         with fl.settings.context(float_type=np.float16):
             self.assertEqual(fl.settings.float_type, np.float16)
```

### Comparing `pyfuzzylite-8.0.2/tests/test_norm.py` & `pyfuzzylite-8.0.3/tests/test_norm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
+import numpy.testing as npt
 
 import fuzzylite as fl
+from fuzzylite import inf, nan
 from tests.assert_component import BaseAssert
 
 
 class NormAssert(BaseAssert[fl.Norm]):
     """Assert norms."""
 
     def is_t_norm(self) -> NormAssert:
@@ -42,21 +38,28 @@
         self,
         abz: dict[tuple[float, float], float],
         commutative: bool = True,
         associative: bool = True,
     ) -> NormAssert:
         """Assert the norm produces the expected values."""
         for ab, z in abz.items():
-            self.test.assertEqual(z, self.actual.compute(*ab), f"in ({ab})")
+            npt.assert_allclose(z, self.actual.compute(*ab), equal_nan=True, err_msg=f"in ({ab})")
+            # self.test.assertEqual(z, self.actual.compute(*ab), f"in ({ab})")
             if commutative:
-                self.test.assertEqual(
+                npt.assert_allclose(
                     z,
                     self.actual.compute(*reversed(ab)),
-                    f"when ({tuple(reversed(ab))})",
+                    equal_nan=True,
+                    err_msg=f"when ({tuple(reversed(ab))})",
                 )
+                # self.test.assertEqual(
+                #     z,
+                #     self.actual.compute(*reversed(ab)),
+                #     f"when ({tuple(reversed(ab))})",
+                # )
             if associative:
                 a: fl.Scalar = ab[0]
                 b: fl.Scalar = ab[1]
                 c: fl.Scalar = sum(ab) / 2
                 abc = self.actual.compute(self.actual.compute(a, b), c)
                 bca = self.actual.compute(self.actual.compute(b, c), a)
                 cab = self.actual.compute(self.actual.compute(c, a), b)
@@ -99,14 +102,18 @@
                 (0.50, 0.50): 0.250,
                 (0.50, 0.75): 0.375,
                 (1.00, 0.00): 0.00,
                 (1.00, 0.25): 0.25,
                 (1.00, 0.50): 0.50,
                 (1.00, 0.75): 0.75,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): inf,
+                (inf, -inf): -inf,
+                (-inf, -inf): inf,
             }
         )
 
     def test_bounded_difference(self) -> None:
         """Test the bounded difference."""
         NormAssert(self, fl.BoundedDifference()).is_t_norm().repr_is(
             "fl.BoundedDifference()"
@@ -121,14 +128,18 @@
                 (0.50, 0.50): 0.0,
                 (0.50, 0.75): 0.25,
                 (1.00, 0.00): 0.00,
                 (1.00, 0.25): 0.25,
                 (1.00, 0.50): 0.50,
                 (1.00, 0.75): 0.75,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): inf,
+                (inf, -inf): nan,
+                (-inf, -inf): 0,
             }
         )
 
     def test_drastic_product(self) -> None:
         """Test the drastic product."""
         NormAssert(self, fl.DrasticProduct()).is_t_norm().repr_is(
             "fl.DrasticProduct()"
@@ -143,14 +154,18 @@
                 (0.50, 0.50): 0.00,
                 (0.50, 0.75): 0.00,
                 (1.00, 0.00): 0.00,
                 (1.00, 0.25): 0.25,
                 (1.00, 0.50): 0.50,
                 (1.00, 0.75): 0.75,
                 (1.00, 1.00): 1.00,
+                (nan, nan): 0.0,
+                (inf, inf): 0.0,
+                (inf, -inf): 0.0,
+                (-inf, -inf): 0.0,
             }
         )
 
     def test_einstein_product(self) -> None:
         """Test the einstein product."""
         NormAssert(self, fl.EinsteinProduct()).is_t_norm().repr_is(
             "fl.EinsteinProduct()"
@@ -165,14 +180,18 @@
                 (0.50, 0.50): 0.20,
                 (0.50, 0.75): 0.3333333333333333,
                 (1.00, 0.00): 0.00,
                 (1.00, 0.25): 0.25,
                 (1.00, 0.50): 0.50,
                 (1.00, 0.75): 0.75,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): nan,
+                (inf, -inf): nan,
+                (-inf, -inf): nan,
             }
         )
 
     def test_hamacher_product(self) -> None:
         """Test the hamacher product."""
         NormAssert(self, fl.HamacherProduct()).is_t_norm().repr_is(
             "fl.HamacherProduct()"
@@ -187,14 +206,18 @@
                 (0.50, 0.50): 0.3333333333333333,
                 (0.50, 0.75): 0.42857142857142855,
                 (1.00, 0.00): 0.00,
                 (1.00, 0.25): 0.25,
                 (1.00, 0.50): 0.50,
                 (1.00, 0.75): 0.75,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): nan,
+                (inf, -inf): nan,
+                (-inf, -inf): nan,
             }
         )
 
     def test_minimum(self) -> None:
         """Test the minimum."""
         NormAssert(self, fl.Minimum()).is_t_norm().repr_is("fl.Minimum()").exports_fll(
             "Minimum"
@@ -209,14 +232,18 @@
                 (0.50, 0.50): 0.50,
                 (0.50, 0.75): 0.50,
                 (1.00, 0.00): 0.00,
                 (1.00, 0.25): 0.25,
                 (1.00, 0.50): 0.50,
                 (1.00, 0.75): 0.75,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): inf,
+                (inf, -inf): -inf,
+                (-inf, -inf): -inf,
             }
         )
 
     def test_nilpotent_minimum(self) -> None:
         """Test the nilpotent minimum."""
         NormAssert(self, fl.NilpotentMinimum()).is_t_norm().repr_is(
             "fl.NilpotentMinimum()"
@@ -231,14 +258,18 @@
                 (0.50, 0.50): 0.00,
                 (0.50, 0.75): 0.50,
                 (1.00, 0.00): 0.00,
                 (1.00, 0.25): 0.25,
                 (1.00, 0.50): 0.50,
                 (1.00, 0.75): 0.75,
                 (1.00, 1.00): 1.00,
+                (nan, nan): 0.0,
+                (inf, inf): inf,
+                (inf, -inf): 0.0,
+                (-inf, -inf): 0.0,
             }
         )
 
 
 class TestSNorm(unittest.TestCase):
     """Test the S-Norms."""
 
@@ -257,14 +288,18 @@
                 (0.50, 0.50): 0.75,
                 (0.50, 0.75): 0.875,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): nan,
+                (inf, -inf): nan,
+                (-inf, -inf): -inf,
             }
         )
 
     def test_bounded_sum(self) -> None:
         """Test the bounded sum."""
         NormAssert(self, fl.BoundedSum()).is_s_norm().repr_is("fl.BoundedSum()").exports_fll(
             "BoundedSum"
@@ -279,14 +314,18 @@
                 (0.50, 0.50): 1.00,
                 (0.50, 0.75): 1.00,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): 1.0,
+                (inf, -inf): nan,
+                (-inf, -inf): -inf,
             }
         )
 
     def test_drastic_sum(self) -> None:
         """Test the drastic sum."""
         NormAssert(self, fl.DrasticSum()).is_s_norm().repr_is("fl.DrasticSum()").exports_fll(
             "DrasticSum"
@@ -301,14 +340,18 @@
                 (0.50, 0.50): 1.00,
                 (0.50, 0.75): 1.00,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): 1.0,
+                (inf, inf): 1.0,
+                (inf, -inf): 1.0,
+                (-inf, -inf): 1.0,
             }
         )
 
     def test_einstein_sum(self) -> None:
         """Test the einstein sum."""
         NormAssert(self, fl.EinsteinSum()).is_s_norm().repr_is("fl.EinsteinSum()").exports_fll(
             "EinsteinSum"
@@ -323,14 +366,18 @@
                 (0.50, 0.50): 0.80,
                 (0.50, 0.75): 0.9090909090909091,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): nan,
+                (inf, -inf): nan,
+                (-inf, -inf): nan,
             }
         )
 
     def test_hamacher_sum(self) -> None:
         """Test the hamacher sum."""
         NormAssert(self, fl.HamacherSum()).is_s_norm().repr_is("fl.HamacherSum()").exports_fll(
             "HamacherSum"
@@ -345,14 +392,18 @@
                 (0.50, 0.50): 0.6666666666666666,
                 (0.50, 0.75): 0.80,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): nan,
+                (inf, -inf): nan,
+                (-inf, -inf): nan,
             }
         )
 
     def test_maximum(self) -> None:
         """Test the maximum."""
         NormAssert(self, fl.Maximum()).is_s_norm().repr_is("fl.Maximum()").exports_fll(
             "Maximum"
@@ -367,14 +418,18 @@
                 (0.50, 0.50): 0.50,
                 (0.50, 0.75): 0.75,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): inf,
+                (inf, -inf): inf,
+                (-inf, -inf): -inf,
             }
         )
 
     def test_nilpotent_maximum(self) -> None:
         """Test the nilpotent maximum."""
         NormAssert(self, fl.NilpotentMaximum()).is_s_norm().repr_is(
             "fl.NilpotentMaximum()"
@@ -389,14 +444,18 @@
                 (0.50, 0.50): 1.00,
                 (0.50, 0.75): 1.00,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): 1.0,
+                (inf, inf): 1.0,
+                (inf, -inf): 1.0,
+                (-inf, -inf): -inf,
             }
         )
 
     def test_normalized_sum(self) -> None:
         """Test the normalised sum."""
         NormAssert(self, fl.NormalizedSum()).is_s_norm().repr_is("fl.NormalizedSum()").exports_fll(
             "NormalizedSum"
@@ -411,14 +470,18 @@
                 (0.50, 0.50): 1.00,
                 (0.50, 0.75): 1.00,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): nan,
+                (inf, -inf): nan,
+                (-inf, -inf): -inf,
             }
         )
 
     def test_unbounded_sum(self) -> None:
         """Test the unbounded sum."""
         NormAssert(self, fl.UnboundedSum()).is_s_norm().repr_is("fl.UnboundedSum()").exports_fll(
             "UnboundedSum"
@@ -433,14 +496,18 @@
                 (0.50, 0.50): 1.00,
                 (0.50, 0.75): 1.25,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.25,
                 (1.00, 0.50): 1.50,
                 (1.00, 0.75): 1.75,
                 (1.00, 1.00): 2.00,
+                (nan, nan): nan,
+                (inf, inf): inf,
+                (inf, -inf): nan,
+                (-inf, -inf): -inf,
             }
         )
 
 
 class TestNormFunctions(unittest.TestCase):
     """Test the norm functions."""
 
@@ -461,14 +528,18 @@
                 (0.50, 0.50): 0.75,
                 (0.50, 0.75): 0.875,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): nan,
+                (inf, -inf): nan,
+                (-inf, -inf): -inf,
             }
         )
 
     def test_norm_lambda(self) -> None:
         """Test the norm lambda."""
         NormAssert(self, fl.NormLambda(lambda a, b: a + b - (a * b))).exports_fll(
             "NormLambda"
@@ -483,13 +554,18 @@
                 (0.50, 0.50): 0.75,
                 (0.50, 0.75): 0.875,
                 (1.00, 0.00): 1.00,
                 (1.00, 0.25): 1.00,
                 (1.00, 0.50): 1.00,
                 (1.00, 0.75): 1.00,
                 (1.00, 1.00): 1.00,
+                (nan, nan): nan,
+                (inf, inf): nan,
+                (-inf, inf): nan,
+                (inf, -inf): nan,
+                (-inf, -inf): -inf,
             }
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyfuzzylite-8.0.2/tests/test_operation.py` & `pyfuzzylite-8.0.3/tests/test_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import math
 import unittest
 from types import ModuleType
 from typing import Callable
```

### Comparing `pyfuzzylite-8.0.2/tests/test_rule.py` & `pyfuzzylite-8.0.3/tests/test_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import unittest
 from unittest.mock import MagicMock
 
 import numpy as np
 
@@ -123,16 +117,17 @@
         antecedent = fl.Antecedent(text)
         with self.test.assertRaisesRegex(exception, regex):
             antecedent.load(self.engine)
         return self
 
     def has_activation_degrees(
         self,
-        inputs: dict[fl.InputVariable, list[float]]
-        | dict[fl.OutputVariable, list[list[fl.Activated]]],
+        inputs: (
+            dict[fl.InputVariable, list[float]] | dict[fl.OutputVariable, list[list[fl.Activated]]]
+        ),
         rules: dict[str, list[float]],
         conjunction: fl.TNorm | None = None,
         disjunction: fl.SNorm | None = None,
     ) -> AssertAntecedent:
         """Assert the rules have the expected activation degrees."""
         self.test.assertTrue(inputs, msg="inputs is empty")
         self.test.assertTrue(rules, msg="rules is empty")
@@ -990,14 +985,18 @@
         )
 
     def test_len_iter_getitem(self) -> None:
         """Test iter, len, and getitem of rule blocks."""
         a, b = [fl.Rule.create("if a then z"), fl.Rule.create("if b then y")]
         rule_block = fl.RuleBlock("test", rules=[a, b])
 
+        # test rule()
+        self.assertEqual(rule_block.rule(0), a)
+        self.assertEqual(rule_block.rule(1), b)
+
         # test getitem
         self.assertEqual(rule_block[0], a)
         self.assertEqual(rule_block[1], b)
         with self.assertRaises(IndexError) as error:
             rule_block[2]
         self.assertEqual("list index out of range", str(error.exception))
         # test slice
```

### Comparing `pyfuzzylite-8.0.2/tests/test_term.py` & `pyfuzzylite-8.0.3/tests/test_term.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import copy
 import operator
 import re
 import unittest
 from collections.abc import Sequence
 from typing import Callable, NoReturn
 
 import numpy as np
-from numpy import inf, nan
 from typing_extensions import Self
 
 import fuzzylite as fl
-from fuzzylite import Scalar
+import fuzzylite.library
+from fuzzylite import Scalar, inf, nan
 from tests.assert_component import BaseAssert
 
 
 class TermAssert(BaseAssert[fl.Term]):
     """Term assert."""
 
     def has_name(self, name: str, height: float = 1.0) -> Self:
@@ -78,18 +72,31 @@
         return self
 
     def configured_as(self, parameters: str) -> Self:
         """Configure the term with the parameters."""
         self.actual.configure(parameters)
         return self
 
-    def has_memberships(self, x_mf: dict[float, float], height: float = 1.0) -> Self:
+    def has_memberships(
+        self, x_mf: dict[float, float], heights: Sequence[float] | None = None
+    ) -> Self:
+        """Assert the term's membership function produces $f(x{_keys}) = mf_{values}$."""
+        inputs = fl.scalar(list(x_mf.keys()))
+        if heights is None:
+            heights = [0.0, 0.25, 0.5, 0.75, 1.0]
+        for height in heights:
+            self.actual.height = height
+            outputs = height * fl.scalar(list(x_mf.values()))
+            self.has_membership(dict(zip(inputs, outputs)))
+        return self
+
+    def has_membership(self, x_mf: dict[float, float]) -> Self:
         """Assert the term's membership function produces $f(x{_keys}) = mf_{values}$."""
-        inputs = fl.scalar([x for x in x_mf])
-        expected = height * fl.scalar([mf for mf in x_mf.values()])
+        inputs = fl.scalar(list(x_mf.keys()))
+        expected = fl.scalar(list(x_mf.values()))
         if isinstance(self.actual, fl.Linear):
             self.test.assertIsNotNone(self.actual.engine)
             # membership function of linear terms do not depend on parameter inputs,
             # instead it depends on the input values of the variables.
             # here we extend each input value to match the length of the inputs
             # so the obtained membership has the same shape as the expected values
             for input_variable in self.actual.engine.input_variables:  # type: ignore
@@ -208,15 +215,15 @@
                 fl.AlgebraicProduct(),
             ),
         ).repr_is(
             "fl.Activated(term=fl.Triangle('triangle', -0.4, 0.0, 0.4), "
             "degree=1.0, implication=fl.AlgebraicProduct())"
         ).exports_fll(
             "term: _ Activated AlgebraicProduct(1.000,triangle)"
-        ).is_not_monotonic().has_memberships(
+        ).is_not_monotonic().has_membership(
             {
                 -1.0: 0.0,
                 -0.5: 0.000,
                 -0.4: 0.000,
                 -0.25: 0.375,
                 -0.1: 0.750,
                 0.0: 1.000,
@@ -236,15 +243,15 @@
             fl.Activated(
                 fl.Triangle("triangle", -0.400, 0.000, 0.400),
                 0.5,
                 fl.AlgebraicProduct(),
             ),
         ).exports_fll(
             "term: _ Activated AlgebraicProduct(0.500,triangle)"
-        ).is_not_monotonic().has_memberships(
+        ).is_not_monotonic().has_membership(
             {
                 -1.0: 0.0,
                 -0.5: 0.000,
                 -0.4: 0.000,
                 -0.25: 0.18750000000000003,
                 -0.1: 0.37500000000000006,
                 0.0: 0.5,
@@ -302,15 +309,16 @@
                 0.25: 0.4,
                 0.4: 0.2,
                 0.5: 0.0,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
                 -inf: 0.0,
-            }
+            },
+            heights=[1.0],
         )
 
         self.assertEqual(aggregated.activation_degree(low), 0.6)
         self.assertEqual(aggregated.activation_degree(medium), 0.4)
 
         self.assertEqual(aggregated.highest_activated_term().term, low)  # type: ignore
 
@@ -403,32 +411,15 @@
                 inf: nan,
                 -inf: nan,
             }
         )
 
         TermAssert(self, fl.Arc("arc")).configured_as(".50 -.50").exports_fll(
             "term: arc Arc 0.500 -0.500"
-        ).repr_is("fl.Arc('arc', 0.5, -0.5)").has_memberships(
-            {
-                -1.0: 1.0,
-                -0.5: 1.0,
-                -0.4: 0.995,
-                -0.25: 0.968,
-                -0.1: 0.916,
-                0.0: 0.866,
-                0.1: 0.8,
-                0.25: 0.661,
-                0.4: 0.436,
-                0.5: 0.0,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 1.0,
-            }
-        ).has_tsukamotos(
+        ).repr_is("fl.Arc('arc', 0.5, -0.5)").has_tsukamotos(
             {
                 0.0: 0.5,
                 0.25: 0.468,
                 0.5: 0.366,
                 0.75: 0.161,
                 1.0: -0.5,
                 # invalid values:
@@ -438,32 +429,14 @@
                 inf: nan,
                 -inf: nan,
             }
         )
 
         TermAssert(self, fl.Arc("arc")).configured_as("-.50 .50 .5").exports_fll(
             "term: arc Arc -0.500 0.500 0.500"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0,
-                -0.4: 0.436,
-                -0.25: 0.661,
-                -0.1: 0.8,
-                0.0: 0.866,
-                0.1: 0.916,
-                0.25: 0.968,
-                0.4: 0.995,
-                0.5: 1.0,
-                1.0: 1.0,
-                nan: nan,
-                inf: 1.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         ).has_tsukamotos(
             {
                 0.0: -0.5,
                 0.25: -0.366,
                 0.5: 0.5,
                 # invalid values:
                 0.75: nan,
@@ -474,32 +447,14 @@
                 inf: nan,
                 -inf: nan,
             }
         )
 
         TermAssert(self, fl.Arc("arc")).configured_as(".50 -.50 .5").exports_fll(
             "term: arc Arc 0.500 -0.500 0.500"
-        ).has_memberships(
-            {
-                -1.0: 1.0,
-                -0.5: 1.0,
-                -0.4: 0.995,
-                -0.25: 0.968,
-                -0.1: 0.916,
-                0.0: 0.866,
-                0.1: 0.8,
-                0.25: 0.661,
-                0.4: 0.436,
-                0.5: 0.0,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 1.0,
-            },
-            height=0.5,
         ).has_tsukamotos(
             {
                 0.0: 0.5,
                 0.25: 0.366,
                 0.5: -0.5,
                 0.75: nan,
                 1.0: nan,
@@ -537,32 +492,14 @@
             }
         ).configured_as(
             "0 0.25 3.0 0.5"
         ).exports_fll(
             "term: bell Bell 0.000 0.250 3.000 0.500"
         ).repr_is(
             "fl.Bell('bell', 0.0, 0.25, 3.0, 0.5)"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.015384615384615385,
-                -0.4: 0.05625177755617076,
-                -0.25: 0.5,
-                -0.1: 0.9959207087768499,
-                0.0: 1.0,
-                0.1: 0.9959207087768499,
-                0.25: 0.5,
-                0.4: 0.05625177755617076,
-                0.5: 0.015384615384615385,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
     def test_binary(self) -> None:
         """Test the binary term."""
         TermAssert(self, fl.Binary("binary")).exports_fll("term: binary Binary nan nan").repr_is(
             "fl.Binary('binary', fl.nan, fl.nan)"
         ).takes_parameters(2).is_not_monotonic().configured_as("0 inf").exports_fll(
@@ -585,28 +522,28 @@
                 -inf: 0.0,
             }
         )
         TermAssert(self, fl.Binary("binary")).configured_as("0 -inf 0.5").exports_fll(
             "term: binary Binary 0.000 -inf 0.500"
         ).repr_is("fl.Binary('binary', 0.0, -fl.inf, 0.5)").has_memberships(
             {
-                -1: 0.5,
-                -0.5: 0.5,
-                -0.4: 0.5,
-                -0.25: 0.5,
-                -0.1: 0.5,
-                0.0: 0.5,
+                -1: 1.0,
+                -0.5: 1.0,
+                -0.4: 1.0,
+                -0.25: 1.0,
+                -0.1: 1.0,
+                0.0: 1.0,
                 0.1: 0.0,
                 0.25: 0.0,
                 0.4: 0.0,
                 0.5: 0.0,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
-                -inf: 0.5,
+                -inf: 1.0,
             }
         )
 
     def test_concave(self) -> None:
         """Test the concave term."""
         TermAssert(self, fl.Concave("concave")).exports_fll(
             "term: concave Concave nan nan"
@@ -682,15 +619,15 @@
                 inf: -1,
                 -inf: -1,
             }
         )
 
         TermAssert(self, fl.Concave("concave")).configured_as("0.00 -0.500 0.5").repr_is(
             "fl.Concave('concave', 0.0, -0.5, 0.5)"
-        ).exports_fll("term: concave Concave 0.000 -0.500 0.500").has_memberships(
+        ).exports_fll("term: concave Concave 0.000 -0.500 0.500").has_membership(
             {
                 -1.0: 0.5,
                 -0.5: 0.5,
                 -0.4: 0.416,
                 -0.25: 0.333,
                 -0.1: 0.277,
                 0.0: 0.25,
@@ -729,15 +666,15 @@
             1
         ).is_not_monotonic().configured_as(
             "0.5"
         ).exports_fll(
             "term: constant Constant 0.500"
         ).repr_is(
             "fl.Constant('constant', 0.5)"
-        ).has_memberships(
+        ).has_membership(
             {
                 -1.0: 0.5,
                 -0.5: 0.5,
                 -0.4: 0.5,
                 -0.25: 0.5,
                 -0.1: 0.5,
                 0.0: 0.5,
@@ -752,15 +689,15 @@
             }
         ).configured_as(
             "-0.500"
         ).repr_is(
             "fl.Constant('constant', -0.5)"
         ).exports_fll(
             "term: constant Constant -0.500"
-        ).has_memberships(
+        ).has_membership(
             {
                 -1.0: -0.5,
                 -0.5: -0.5,
                 -0.4: -0.5,
                 -0.25: -0.5,
                 -0.1: -0.5,
                 0.0: -0.5,
@@ -802,32 +739,14 @@
             }
         ).configured_as(
             "0.0 1.0 0.5"
         ).exports_fll(
             "term: cosine Cosine 0.000 1.000 0.500"
         ).repr_is(
             "fl.Cosine('cosine', 0.0, 1.0, 0.5)"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.0,
-                -0.4: 0.09549150281252633,
-                -0.25: 0.5,
-                -0.1: 0.9045084971874737,
-                0.0: 1.0,
-                0.1: 0.9045084971874737,
-                0.25: 0.5,
-                0.4: 0.09549150281252633,
-                0.5: 0.0,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
     def test_discrete(self) -> None:
         """Test the discrete term."""
         TermAssert(self, fl.Discrete("discrete")).exports_fll(
             "term: discrete Discrete"
         ).is_not_monotonic().configured_as("0 1 8 9 4 5 2 3 6 7").exports_fll(
@@ -873,32 +792,14 @@
                 -inf: 0.0,
             }
         ).configured_as(
             " -0.500 0.000 -0.250 1.000 0.000 0.500 0.250 1.000 0.500 0.000 0.5"
         ).exports_fll(
             "term: discrete Discrete "
             "-0.500 0.000 -0.250 1.000 0.000 0.500 0.250 1.000 0.500 0.000 0.500"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.0,
-                -0.4: 0.3999999999999999,
-                -0.25: 1.0,
-                -0.1: 0.7,
-                0.0: 0.5,
-                0.1: 0.7,
-                0.25: 1.0,
-                0.4: 0.3999999999999999,
-                0.5: 0.0,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
         term = fl.Discrete()
         with self.assertRaisesRegex(
             ValueError,
             re.escape("expected xy to contain coordinate pairs, but it is empty"),
         ):
@@ -995,32 +896,14 @@
             }
         ).configured_as(
             "0.0 0.25 0.5"
         ).repr_is(
             "fl.Gaussian('gaussian', 0.0, 0.25, 0.5)"
         ).exports_fll(
             "term: gaussian Gaussian 0.000 0.250 0.500"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.1353352832366127,
-                -0.4: 0.2780373004531941,
-                -0.25: 0.6065306597126334,
-                -0.1: 0.9231163463866358,
-                0.0: 1.0,
-                0.1: 0.9231163463866358,
-                0.25: 0.6065306597126334,
-                0.4: 0.2780373004531941,
-                0.5: 0.1353352832366127,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
     def test_gaussian_product(self) -> None:
         """Test the gaussian product term."""
         TermAssert(self, fl.GaussianProduct("gaussian_product")).exports_fll(
             "term: gaussian_product GaussianProduct nan nan nan nan"
         ).repr_is(
@@ -1052,32 +935,14 @@
             }
         ).configured_as(
             "0.0 0.25 0.1 0.5 0.5"
         ).exports_fll(
             "term: gaussian_product GaussianProduct 0.000 0.250 0.100 0.500 0.500"
         ).repr_is(
             "fl.GaussianProduct('gaussian_product', 0.0, 0.25, 0.1, 0.5, 0.5)"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.1353352832366127,
-                -0.4: 0.2780373004531941,
-                -0.25: 0.6065306597126334,
-                -0.1: 0.9231163463866358,
-                0.0: 1.0,
-                0.1: 1.0,
-                0.25: 0.9559974818331,
-                0.4: 0.835270211411272,
-                0.5: 0.7261490370736908,
-                1.0: 0.198,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
     def test_linear(self) -> None:
         """Test the linear term."""
         engine = fl.Engine(
             input_variables=[
                 fl.InputVariable("A"),
@@ -1099,15 +964,15 @@
 
         TermAssert(self, linear).exports_fll("term: linear Linear 1.000 2.000").repr_is(
             "fl.Linear('linear', [1.0, 2.0])"
         ).is_not_monotonic().configured_as("1.0 2.0 3").exports_fll(
             "term: linear Linear 1.000 2.000 3.000"
         ).repr_is(
             "fl.Linear('linear', [1.0, 2.0, 3.0])"
-        ).has_memberships(
+        ).has_membership(
             {
                 -1.0: 1 * 0 + 2 * 1 + 3 * 2,  # = 8
                 -0.5: 8,
                 -0.4: 8,
                 -0.25: 8,
                 -0.1: 8,
                 0.0: 8,
@@ -1119,15 +984,15 @@
                 nan: 8,
                 inf: 8,
                 -inf: 8,
             }
         )
         TermAssert(self, linear).configured_as("1 2 3 5").exports_fll(
             "term: linear Linear 1.000 2.000 3.000 5.000"
-        ).has_memberships(
+        ).has_membership(
             {
                 -1.0: 1 * 0 + 2 * 1 + 3 * 2 + 5,  # = 13
                 -0.5: 13,
                 -0.4: 13,
                 -0.25: 13,
                 -0.1: 13,
                 0.0: 13,
@@ -1182,33 +1047,14 @@
             }
         ).configured_as(
             "-.9 -.1 .1 1 .5"
         ).exports_fll(
             "term: pi_shape PiShape -0.900 -0.100 0.100 1.000 0.500"
         ).repr_is(
             "fl.PiShape('pi_shape', -0.9, -0.1, 0.1, 1.0, 0.5)"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.5,
-                -0.4: 0.71875,
-                -0.25: 0.9296875,
-                -0.1: 1.0,
-                0.0: 1.0,
-                0.1: 1.0,
-                0.25: 0.9444444444444444,
-                0.4: 0.7777777777777777,
-                0.5: 0.6049382716049383,
-                0.95: 0.00617283950617285,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
     def test_ramp(self) -> None:
         """Test the ramp term."""
         TermAssert(self, fl.Ramp("ramp")).exports_fll("term: ramp Ramp nan nan").repr_is(
             "fl.Ramp('ramp', fl.nan, fl.nan)"
         ).takes_parameters(2).is_monotonic()
@@ -1311,33 +1157,15 @@
                 inf: -inf,
                 -inf: inf,
             }
         )
 
         TermAssert(self, fl.Ramp("ramp")).configured_as("0.250 -0.750 0.5").exports_fll(
             "term: ramp Ramp 0.250 -0.750 0.500"
-        ).repr_is("fl.Ramp('ramp', 0.25, -0.75, 0.5)").has_memberships(
-            {
-                -1.0: 1.0,
-                -0.5: 0.750,
-                -0.4: 0.650,
-                -0.25: 0.500,
-                -0.1: 0.350,
-                0.0: 0.250,
-                0.1: 0.150,
-                0.25: 0.0,
-                0.4: 0.0,
-                0.5: 0.0,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 1.0,
-            },
-            height=0.5,
-        ).has_tsukamotos(
+        ).repr_is("fl.Ramp('ramp', 0.25, -0.75, 0.5)").has_tsukamotos(
             {
                 0.0: 0.25,
                 0.125: 0,
                 0.25: -0.25,
                 0.375: -0.5,
                 0.5: -0.75,
                 # invalid values
@@ -1382,32 +1210,14 @@
             }
         ).configured_as(
             "-0.4 0.4 0.5"
         ).exports_fll(
             "term: rectangle Rectangle -0.400 0.400 0.500"
         ).repr_is(
             "fl.Rectangle('rectangle', -0.4, 0.4, 0.5)"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.0,
-                -0.4: 1.0,
-                -0.25: 1.0,
-                -0.1: 1.0,
-                0.0: 1.0,
-                0.1: 1.0,
-                0.25: 1.0,
-                0.4: 1.0,
-                0.5: 0.0,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
     def test_semiellipse(self) -> None:
         """Test the spike term."""
         TermAssert(self, fl.SemiEllipse("semiellipse")).exports_fll(
             "term: semiellipse SemiEllipse nan nan"
         ).repr_is("fl.SemiEllipse('semiellipse', fl.nan, fl.nan)").takes_parameters(
@@ -1454,33 +1264,15 @@
                 inf: 0.0,
                 -inf: 0.0,
             }
         )
 
         TermAssert(self, fl.SemiEllipse("semiellipse")).configured_as("-0.5 0.5 0.5").exports_fll(
             "term: semiellipse SemiEllipse -0.500 0.500 0.500"
-        ).repr_is("fl.SemiEllipse('semiellipse', -0.5, 0.5, 0.5)").has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.0,
-                -0.4: 0.6,
-                -0.25: 0.866,
-                -0.1: 0.979,
-                0.0: 1.0,
-                0.1: 0.979,
-                0.25: 0.866,
-                0.4: 0.6,
-                0.5: 0.0,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
-        )
+        ).repr_is("fl.SemiEllipse('semiellipse', -0.5, 0.5, 0.5)")
 
     def test_sigmoid(self) -> None:
         """Test the sigmoid term."""
         TermAssert(self, fl.Sigmoid("sigmoid")).exports_fll(
             "term: sigmoid Sigmoid nan nan"
         ).repr_is("fl.Sigmoid('sigmoid', fl.nan, fl.nan)").takes_parameters(
             2
@@ -1556,33 +1348,15 @@
                 inf: nan,
                 -inf: nan,
             }
         )
 
         TermAssert(self, fl.Sigmoid("sigmoid")).configured_as("0 10 .5").exports_fll(
             "term: sigmoid Sigmoid 0.000 10.000 0.500"
-        ).repr_is("fl.Sigmoid('sigmoid', 0.0, 10.0, 0.5)").has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.007,
-                -0.4: 0.018,
-                -0.25: 0.076,
-                -0.1: 0.269,
-                0.0: 0.5,
-                0.1: 0.731,
-                0.25: 0.924,
-                0.4: 0.982,
-                0.5: 0.993,
-                1.0: 0.999,
-                nan: nan,
-                inf: 1.0,
-                -inf: 0.0,
-            },
-            height=0.5,
-        ).has_tsukamotos(
+        ).repr_is("fl.Sigmoid('sigmoid', 0.0, 10.0, 0.5)").has_tsukamotos(
             {
                 0.0: -inf,
                 0.125: -0.11,
                 0.25: 0,
                 0.375: 0.11,
                 0.5: inf,
                 # invalid values
@@ -1629,32 +1403,14 @@
             }
         ).configured_as(
             "-0.25 25.00 50.00 0.25 0.5"
         ).repr_is(
             "fl.SigmoidDifference('sigmoid_difference', -0.25, 25.0, 50.0, 0.25, 0.5)"
         ).exports_fll(
             "term: sigmoid_difference SigmoidDifference -0.250 25.000 50.000 0.250 0.500"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.0019267346633274238,
-                -0.4: 0.022977369910017923,
-                -0.25: 0.49999999998611205,
-                -0.1: 0.9770226049799834,
-                0.0: 0.9980695386973883,
-                0.1: 0.9992887851439739,
-                0.25: 0.49999627336071584,
-                0.4: 0.000552690994449101,
-                0.5: 3.7194451510957904e-06,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
     def test_sigmoid_product(self) -> None:
         """Test the sigmoid product term."""
         TermAssert(self, fl.SigmoidProduct("sigmoid_product")).exports_fll(
             "term: sigmoid_product SigmoidProduct nan nan nan nan"
         ).repr_is(
@@ -1686,32 +1442,14 @@
             }
         ).configured_as(
             "-0.250 20.000 -20.000 0.250 0.5"
         ).repr_is(
             "fl.SigmoidProduct('sigmoid_product', -0.25, 20.0, -20.0, 0.25, 0.5)"
         ).exports_fll(
             "term: sigmoid_product SigmoidProduct -0.250 20.000 -20.000 0.250 0.500"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.006692848876926853,
-                -0.4: 0.04742576597971327,
-                -0.25: 0.4999773010656488,
-                -0.1: 0.9517062830264366,
-                0.0: 0.9866590924049252,
-                0.1: 0.9517062830264366,
-                0.25: 0.4999773010656488,
-                0.4: 0.04742576597971327,
-                0.5: 0.006692848876926853,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
     def test_spike(self) -> None:
         """Test the spike term."""
         TermAssert(self, fl.Spike("spike")).exports_fll("term: spike Spike nan nan").repr_is(
             "fl.Spike('spike', fl.nan, fl.nan)"
         ).takes_parameters(2).is_not_monotonic().configured_as("0 1.0").exports_fll(
@@ -1737,32 +1475,14 @@
             }
         ).configured_as(
             "0 1.0 .5"
         ).repr_is(
             "fl.Spike('spike', 0.0, 1.0, 0.5)"
         ).exports_fll(
             "term: spike Spike 0.000 1.000 0.500"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.006737946999085467,
-                -0.4: 0.01831563888873418,
-                -0.25: 0.0820849986238988,
-                -0.1: 0.36787944117144233,
-                0.0: 1.0,
-                0.1: 0.36787944117144233,
-                0.25: 0.0820849986238988,
-                0.4: 0.01831563888873418,
-                0.5: 0.006737946999085467,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
         )
 
     def test_s_shape(self) -> None:
         """Test the s-shape term."""
         TermAssert(self, fl.SShape("s_shape")).exports_fll("term: s_shape SShape nan nan").repr_is(
             "fl.SShape('s_shape', fl.nan, fl.nan)"
         ).takes_parameters(2).is_monotonic().configured_as("-0.5 0.5").exports_fll(
@@ -1800,33 +1520,15 @@
                 inf: nan,
                 -inf: nan,
             }
         )
 
         TermAssert(self, fl.SShape("s_shape")).configured_as("-0.5 0.5 0.5").repr_is(
             "fl.SShape('s_shape', -0.5, 0.5, 0.5)"
-        ).exports_fll("term: s_shape SShape -0.500 0.500 0.500").has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.0,
-                -0.4: 0.02,
-                -0.25: 0.125,
-                -0.1: 0.32,
-                0.0: 0.5,
-                0.1: 0.68,
-                0.25: 0.875,
-                0.4: 0.98,
-                0.5: 1.0,
-                1.0: 1.0,
-                nan: nan,
-                inf: 1.0,
-                -inf: 0.0,
-            },
-            height=0.5,
-        ).has_tsukamotos(
+        ).exports_fll("term: s_shape SShape -0.500 0.500 0.500").has_tsukamotos(
             {
                 0.0: -0.5,
                 0.125: -0.146,
                 0.25: 0,
                 0.375: 0.146,
                 0.5: 0.5,
                 # invalid values
@@ -1867,43 +1569,24 @@
                 0.4: 0.000,
                 0.5: 0.000,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
                 -inf: 0.0,
             }
-        ).configured_as(
+        )
+        TermAssert(self, fl.Trapezoid("trapezoid")).configured_as(
             "-0.400 -0.100 0.100 0.400 .5"
-        ).exports_fll(
-            "term: trapezoid Trapezoid -0.400 -0.100 0.100 0.400 0.500"
-        ).repr_is(
+        ).exports_fll("term: trapezoid Trapezoid -0.400 -0.100 0.100 0.400 0.500").repr_is(
             "fl.Trapezoid('trapezoid', -0.4, -0.1, 0.1, 0.4, 0.5)"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.000,
-                -0.4: 0.000,
-                -0.25: 0.500,
-                -0.1: 1.000,
-                0.0: 1.000,
-                0.1: 1.000,
-                0.25: 0.500,
-                0.4: 0.000,
-                0.5: 0.000,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
-        ).configured_as(
+        )
+
+        TermAssert(self, fl.Trapezoid("trapezoid")).configured_as(
             "-0.400 -0.400 0.100 0.400"
-        ).exports_fll(
-            "term: trapezoid Trapezoid -0.400 -0.400 0.100 0.400"
-        ).has_memberships(
+        ).exports_fll("term: trapezoid Trapezoid -0.400 -0.400 0.100 0.400").has_memberships(
             {
                 -1.0: 0.0,
                 -0.5: 0.000,
                 -0.4: 1.000,
                 -0.25: 1.000,
                 -0.1: 1.000,
                 0.0: 1.000,
@@ -1912,19 +1595,18 @@
                 0.4: 0.000,
                 0.5: 0.000,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
                 -inf: 0.0,
             }
-        ).configured_as(
+        )
+        TermAssert(self, fl.Trapezoid("trapezoid")).configured_as(
             "-0.400 -0.100 0.400 0.400"
-        ).exports_fll(
-            "term: trapezoid Trapezoid -0.400 -0.100 0.400 0.400"
-        ).has_memberships(
+        ).exports_fll("term: trapezoid Trapezoid -0.400 -0.100 0.400 0.400").has_memberships(
             {
                 -1.0: 0.0,
                 -0.5: 0.000,
                 -0.4: 0.000,
                 -0.25: 0.5,
                 -0.1: 1.000,
                 0.0: 1.000,
@@ -1933,19 +1615,18 @@
                 0.4: 1.000,
                 0.5: 0.000,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
                 -inf: 0.0,
             }
-        ).configured_as(
+        )
+        TermAssert(self, fl.Trapezoid("trapezoid")).configured_as(
             "-inf -0.100 0.100 .4"
-        ).exports_fll(
-            "term: trapezoid Trapezoid -inf -0.100 0.100 0.400"
-        ).has_memberships(
+        ).exports_fll("term: trapezoid Trapezoid -inf -0.100 0.100 0.400").has_memberships(
             {
                 -1.0: 1.0,
                 -0.5: 1.000,
                 -0.4: 1.000,
                 -0.25: 1.000,
                 -0.1: 1.000,
                 0.0: 1.000,
@@ -1954,36 +1635,34 @@
                 0.4: 0.000,
                 0.5: 0.000,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
                 -inf: 1.0,
             }
-        ).configured_as(
+        )
+        TermAssert(self, fl.Trapezoid("trapezoid")).configured_as(
             "-.4 -0.100 0.100 inf .5"
-        ).exports_fll(
-            "term: trapezoid Trapezoid -0.400 -0.100 0.100 inf 0.500"
-        ).has_memberships(
+        ).exports_fll("term: trapezoid Trapezoid -0.400 -0.100 0.100 inf 0.500").has_membership(
             {
                 -1.0: 0.0,
                 -0.5: 0.000,
                 -0.4: 0.000,
-                -0.25: 0.500,
-                -0.1: 1.000,
-                0.0: 1.000,
-                0.1: 1.000,
-                0.25: 1.000,
-                0.4: 1.000,
-                0.5: 1.000,
-                1.0: 1.0,
+                -0.25: 0.500 * 0.5,
+                -0.1: 1.000 * 0.5,
+                0.0: 1.000 * 0.5,
+                0.1: 1.000 * 0.5,
+                0.25: 1.000 * 0.5,
+                0.4: 1.000 * 0.5,
+                0.5: 1.000 * 0.5,
+                1.0: 1.0 * 0.5,
                 nan: nan,
-                inf: 1.0,
+                inf: 1.0 * 0.5,
                 -inf: 0.0,
             },
-            height=0.5,
         )
 
     def test_triangle(self) -> None:
         """Test the triangle term."""
         TermAssert(self, fl.Triangle("triangle", 0.0, 1.0)).exports_fll(
             "term: triangle Triangle 0.000 0.500 1.000"
         ).repr_is("fl.Triangle('triangle', 0.0, 0.5, 1.0)")
@@ -2009,41 +1688,19 @@
                 0.4: 0.000,
                 0.5: 0.000,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
                 -inf: 0.0,
             }
-        ).configured_as(
-            "-0.400 0.000 0.400 .5"
-        ).repr_is(
+        )
+        TermAssert(self, fl.Triangle("triangle")).configured_as("-0.400 0.000 0.400 .5").repr_is(
             "fl.Triangle('triangle', -0.4, 0.0, 0.4, 0.5)"
-        ).exports_fll(
-            "term: triangle Triangle -0.400 0.000 0.400 0.500"
-        ).has_memberships(
-            {
-                -1.0: 0.0,
-                -0.5: 0.000,
-                -0.4: 0.000,
-                -0.25: 0.37500000000000006,
-                -0.1: 0.7500000000000001,
-                0.0: 1.000,
-                0.1: 0.7500000000000001,
-                0.25: 0.37500000000000006,
-                0.4: 0.000,
-                0.5: 0.000,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 0.0,
-            },
-            height=0.5,
-        ).configured_as(
-            "-0.500 0.000 0.500"
-        ).exports_fll(
+        ).exports_fll("term: triangle Triangle -0.400 0.000 0.400 0.500")
+        TermAssert(self, fl.Triangle("triangle")).configured_as("-0.500 0.000 0.500").exports_fll(
             "term: triangle Triangle -0.500 0.000 0.500"
         ).has_memberships(
             {
                 -1.0: 0.0,
                 -0.5: 0.000,
                 -0.4: 0.2,
                 -0.25: 0.5,
@@ -2054,17 +1711,16 @@
                 0.4: 0.2,
                 0.5: 0.000,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
                 -inf: 0.0,
             }
-        ).configured_as(
-            "-0.500 -0.500 0.500"
-        ).exports_fll(
+        )
+        TermAssert(self, fl.Triangle("triangle")).configured_as("-0.500 -0.500 0.500").exports_fll(
             "term: triangle Triangle -0.500 -0.500 0.500"
         ).has_memberships(
             {
                 -1.0: 0.0,
                 -0.5: 1.000,
                 -0.4: 0.900,
                 -0.25: 0.75,
@@ -2075,17 +1731,16 @@
                 0.4: 0.1,
                 0.5: 0.000,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
                 -inf: 0.0,
             }
-        ).configured_as(
-            "-0.500 0.500 0.500"
-        ).exports_fll(
+        )
+        TermAssert(self, fl.Triangle("triangle")).configured_as("-0.500 0.500 0.500").exports_fll(
             "term: triangle Triangle -0.500 0.500 0.500"
         ).has_memberships(
             {
                 1.0: 0.0,
                 -0.5: 0.000,
                 -0.4: 0.1,
                 -0.25: 0.25,
@@ -2095,17 +1750,16 @@
                 0.25: 0.75,
                 0.4: 0.900,
                 0.5: 1.000,
                 nan: nan,
                 inf: 0.0,
                 -inf: 0.0,
             }
-        ).configured_as(
-            "-inf 0.000 0.400"
-        ).exports_fll(
+        )
+        TermAssert(self, fl.Triangle("triangle")).configured_as("-inf 0.000 0.400").exports_fll(
             "term: triangle Triangle -inf 0.000 0.400"
         ).has_memberships(
             {
                 -1.0: 1.0,
                 -0.5: 1.000,
                 -0.4: 1.000,
                 -0.25: 1.000,
@@ -2116,36 +1770,34 @@
                 0.4: 0.000,
                 0.5: 0.000,
                 1.0: 0.0,
                 nan: nan,
                 inf: 0.0,
                 -inf: 1.000,
             }
-        ).configured_as(
-            "-0.400 0.000 inf .5"
-        ).exports_fll(
+        )
+        TermAssert(self, fl.Triangle("triangle")).configured_as("-0.400 0.000 inf .5").exports_fll(
             "term: triangle Triangle -0.400 0.000 inf 0.500"
-        ).has_memberships(
+        ).has_membership(
             {
                 -1.0: 0.0,
                 -0.5: 0.000,
                 -0.4: 0.000,
-                -0.25: 0.375,
-                -0.1: 0.750,
-                0.0: 1.000,
-                0.1: 1.000,
-                0.25: 1.000,
-                0.4: 1.000,
-                0.5: 1.000,
-                1.0: 1.0,
+                -0.25: 0.375 * 0.5,
+                -0.1: 0.750 * 0.5,
+                0.0: 1.000 * 0.5,
+                0.1: 1.000 * 0.5,
+                0.25: 1.000 * 0.5,
+                0.4: 1.000 * 0.5,
+                0.5: 1.000 * 0.5,
+                1.0: 1.0 * 0.5,
                 nan: nan,
-                inf: 1.000,
+                inf: 1.000 * 0.5,
                 -inf: 0.0,
             },
-            height=0.5,
         )
 
     def test_z_shape(self) -> None:
         """Test the z-shape term."""
         TermAssert(self, fl.ZShape("z_shape")).exports_fll("term: z_shape ZShape nan nan").repr_is(
             "fl.ZShape('z_shape', fl.nan, fl.nan)"
         ).takes_parameters(2).is_monotonic().configured_as("-0.5 0.5").exports_fll(
@@ -2183,33 +1835,15 @@
                 inf: nan,
                 -inf: nan,
             }
         )
 
         TermAssert(self, fl.ZShape("z_shape")).configured_as("-0.5 0.5 0.5").repr_is(
             "fl.ZShape('z_shape', -0.5, 0.5, 0.5)"
-        ).exports_fll("term: z_shape ZShape -0.500 0.500 0.500").has_memberships(
-            {
-                -1.0: 1.0,
-                -0.5: 1.0,
-                -0.4: 0.98,
-                -0.25: 0.875,
-                -0.1: 0.68,
-                0.0: 0.5,
-                0.1: 0.32,
-                0.25: 0.125,
-                0.4: 0.02,
-                0.5: 0.0,
-                1.0: 0.0,
-                nan: nan,
-                inf: 0.0,
-                -inf: 1.0,
-            },
-            height=0.5,
-        ).has_tsukamotos(
+        ).exports_fll("term: z_shape ZShape -0.500 0.500 0.500").has_tsukamotos(
             {
                 0.0: 0.5,
                 0.125: 0.146,
                 0.25: 0.0,
                 0.375: -0.146,
                 0.5: -0.5,
                 # invalid values
@@ -2223,39 +1857,31 @@
             }
         )
 
     def test_division_by_zero_does_not_fail_with_numpy_float(self) -> None:
         """Test the division by zero is not raised when using numpy floats."""
         import numpy as np
 
-        default_float = fl.settings.float_type
-        fl.settings.float_type = np.float64
-        np.seterr(divide="ignore")  # ignore "errors", (e.g., division by zero)
-        try:
-            TermAssert(self, fl.Function.create("dbz", "0.0/x")).has_memberships(
+        with fl.settings.context(float_type=np.float64):
+            np.seterr(divide="ignore")  # ignore "errors", (e.g., division by zero)
+            TermAssert(self, fl.Function.create("dbz", "0.0/x")).has_membership(
                 {0.0: fl.nan, fl.inf: 0.0, -fl.inf: -0.0, fl.nan: fl.nan}
             )
 
-            TermAssert(self, fl.Function.create("dbz", "inf/x")).has_memberships(
+            TermAssert(self, fl.Function.create("dbz", "inf/x")).has_membership(
                 {0.0: fl.inf, fl.inf: fl.nan, -fl.inf: fl.nan, -fl.nan: fl.nan}
             )
 
-            TermAssert(self, fl.Function.create("dbz", "~inf/x")).has_memberships(
+            TermAssert(self, fl.Function.create("dbz", "~inf/x")).has_membership(
                 {0.0: -fl.inf, fl.inf: fl.nan, -fl.inf: fl.nan, -fl.nan: fl.nan}
             )
 
-            TermAssert(self, fl.Function.create("dbz", "nan/x")).has_memberships(
+            TermAssert(self, fl.Function.create("dbz", "nan/x")).has_membership(
                 {0.0: fl.nan, fl.inf: fl.nan, -fl.inf: fl.nan, -fl.nan: fl.nan}
             )
-        except Exception:
-            fl.settings.float_type = default_float
-            raise
-
-        fl.settings.float_type = default_float
-        self.assertEqual(fl.settings.float_type, default_float)
 
     def test_some_function(self) -> None:
         """Test function results."""
         f = fl.Function("X", "ge(x, 5)", load=True)
         np.testing.assert_allclose(0.0, f.membership(4))
         np.testing.assert_allclose(1.0, f.membership(5))
 
@@ -2341,15 +1967,16 @@
                 0.1: 0.0019999999999997797,
                 0.25: 0.03125,
                 0.4: 0.1280000000000001,
                 0.5: 0.25,
                 nan: nan,
                 inf: inf,
                 -inf: -inf,
-            }
+            },
+            heights=[1.0],
         )
 
         input_a = fl.InputVariable("i_A")
         output_a = fl.OutputVariable("o_A")
         engine_a = fl.Engine("A", "Engine A", [input_a], [output_a])
         with self.assertRaisesRegex(
             ValueError,
@@ -2373,15 +2000,16 @@
                 -0.5: 6.5,
                 0.0: 7.0,
                 0.5: 7.5,
                 1.0: 8.0,
                 nan: nan,
                 inf: inf,
                 -inf: -inf,
-            }
+            },
+            heights=[1.0],
         )
 
         function_a.variables = {"x": nan}
         with self.assertRaisesRegex(
             ValueError,
             re.escape(
                 "variable 'x' is reserved for internal use of Function term, "
@@ -2493,15 +2121,15 @@
             "pow ( sin ( 3.000 ** 4.000 ) two ) + pow ( sin ( 3.000 ** 4.000 ) two )"
         ).evaluates_to(
             0.7935177706621891, {"two": 2}
         )
 
         FunctionNodeAssert(
             self, fl.Function.Node(element=functions.copy("cos"), right=None)
-        ).fails_to_evaluate(ValueError, re.escape("expected a right node, but found none"))
+        ).fails_to_evaluate(ValueError, re.escape("expected a node, but found none"))
 
         FunctionNodeAssert(
             self,
             fl.Function.Node(
                 element=functions.copy("cos"),
                 right=fl.Function.Node(constant=np.pi),
                 left=None,
@@ -2599,16 +2227,30 @@
                 variable="x",
                 constant=1,
             ),
         ).value_is("+")
 
         FunctionNodeAssert(self, fl.Function.Node(variable="x")).value_is("x")
         FunctionNodeAssert(self, fl.Function.Node(variable="x", constant=1.0)).value_is("x")
-
         FunctionNodeAssert(self, fl.Function.Node(constant=1)).value_is("1")
+        negate = fuzzylite.library.settings.factory_manager.function.copy("~")
+        (
+            FunctionNodeAssert(self, fl.Function.Node(negate, right=fl.Function.Node(constant=5.0)))
+            .prefix_is("~ 5.000")
+            .infix_is("~ 5.000")
+            .postfix_is("5.000 ~")
+            .evaluates_to(-5.000)
+        )
+        (
+            FunctionNodeAssert(self, fl.Function.Node(negate, left=fl.Function.Node(constant=5.0)))
+            .prefix_is("~ 5.000")
+            .infix_is("~ 5.000")
+            .postfix_is("5.000 ~")
+            .evaluates_to(-5.000)
+        )
 
     def test_function_format_infix(self) -> None:
         """Test formatting infix equations."""
         self.assertEqual(
             "a + b * 1 ( True or True ) / ( False and False )",
             fl.Function.format_infix(f"a+b*1(True {fl.Rule.OR} True)/(False {fl.Rule.AND} False)"),
         )
```

### Comparing `pyfuzzylite-8.0.2/tests/test_variable.py` & `pyfuzzylite-8.0.3/tests/test_variable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import math
 import unittest
 from collections.abc import Sequence
 from typing import Any, TypeVar
 from unittest.mock import MagicMock
@@ -400,21 +394,23 @@
         return fl.OutputVariable(
             enabled=enabled,
             name=name,
             description=description,
             minimum=minimum,
             maximum=maximum,
             default_value=default_value,
-            terms=terms
-            if terms is not None
-            else [
-                fl.Triangle("low", -1.0, -1.0, 0.0),
-                fl.Triangle("medium", -0.5, 0.0, 0.5),
-                fl.Triangle("high", 0.0, 1.0, 1.0),
-            ],
+            terms=(
+                terms
+                if terms is not None
+                else [
+                    fl.Triangle("low", -1.0, -1.0, 0.0),
+                    fl.Triangle("medium", -0.5, 0.0, 0.5),
+                    fl.Triangle("high", 0.0, 1.0, 1.0),
+                ]
+            ),
         )
 
     def test_constructor(self) -> None:
         """Test the constructor."""
         OutputVariableAssert(self, fl.OutputVariable("name", "description")).exports_fll(
             "\n".join(
                 [
```

### Comparing `pyfuzzylite-8.0.2/tests/test_vectorization.py` & `pyfuzzylite-8.0.3/tests/test_vectorization.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-"""pyfuzzylite (TM), a fuzzy logic control library in Python.
-
-Copyright (C) 2010-2023 FuzzyLite Limited. All rights reserved.
-Author: Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>.
+"""pyfuzzylite: a fuzzy logic control library in Python.
 
 This file is part of pyfuzzylite.
 
-pyfuzzylite is free software: you can redistribute it and/or modify it under
-the terms of the FuzzyLite License included with the software.
-
-You should have received a copy of the FuzzyLite License along with
-pyfuzzylite. If not, see <https://github.com/fuzzylite/pyfuzzylite/>.
+Repository: https://github.com/fuzzylite/pyfuzzylite/
 
-pyfuzzylite is a trademark of FuzzyLite Limited.
+License: FuzzyLite License
 
-fuzzylite is a registered trademark of FuzzyLite Limited.
+Copyright: FuzzyLite by Juan Rada-Vilela. All rights reserved.
 """
+
 from __future__ import annotations
 
 import copy
 import unittest
 
 import numpy as np
```

### Comparing `pyfuzzylite-8.0.2/PKG-INFO` & `pyfuzzylite-8.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6675  : 2.1.Name: pyfu
 00000020: 7a7a 796c 6974 650a 5665 7273 696f 6e3a  zzylite.Version:
-00000030: 2038 2e30 2e32 0a53 756d 6d61 7279 3a20   8.0.2.Summary: 
+00000030: 2038 2e30 2e33 0a53 756d 6d61 7279 3a20   8.0.3.Summary: 
 00000040: 6120 6675 7a7a 7920 6c6f 6769 6320 636f  a fuzzy logic co
 00000050: 6e74 726f 6c20 6c69 6272 6172 7920 696e  ntrol library in
 00000060: 2050 7974 686f 6e0a 486f 6d65 2d70 6167   Python.Home-pag
 00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000080: 622e 636f 6d2f 6675 7a7a 796c 6974 652f  b.com/fuzzylite/
 00000090: 7079 6675 7a7a 796c 6974 652e 6769 740a  pyfuzzylite.git.
 000000a0: 4c69 6365 6e73 653a 2050 726f 7072 6965  License: Proprie
@@ -94,538 +94,533 @@
 000005d0: 7465 2f70 7966 757a 7a79 6c69 7465 2e67  te/pyfuzzylite.g
 000005e0: 6974 0a50 726f 6a65 6374 2d55 524c 3a20  it.Project-URL: 
 000005f0: 536f 7572 6365 2043 6f64 652c 2068 7474  Source Code, htt
 00000600: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000610: 6675 7a7a 796c 6974 652f 7079 6675 7a7a  fuzzylite/pyfuzz
 00000620: 796c 6974 650a 4465 7363 7269 7074 696f  ylite.Descriptio
 00000630: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000640: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
-00000650: 2070 7966 757a 7a79 6c69 7465 2038 2e30   pyfuzzylite 8.0
-00000660: 2e32 0a0a 3c69 6d67 2073 7263 3d22 6874  .2..<img src="ht
-00000670: 7470 733a 2f2f 6675 7a7a 796c 6974 652e  tps://fuzzylite.
-00000680: 6769 7468 7562 2e69 6f2f 7079 6675 7a7a  github.io/pyfuzz
-00000690: 796c 6974 652f 696d 6167 652f 6675 7a7a  ylite/image/fuzz
-000006a0: 796c 6974 652e 7376 6722 2061 6c69 676e  ylite.svg" align
-000006b0: 3d22 6c65 6674 2220 616c 743d 2266 757a  ="left" alt="fuz
-000006c0: 7a79 6c69 7465 223e 0a0a 2323 2041 2046  zylite">..## A F
-000006d0: 757a 7a79 204c 6f67 6963 2043 6f6e 7472  uzzy Logic Contr
-000006e0: 6f6c 204c 6962 7261 7279 2069 6e20 5079  ol Library in Py
-000006f0: 7468 6f6e 0a0a 6279 205b 2a2a 4a75 616e  thon..by [**Juan
-00000700: 2052 6164 612d 5669 6c65 6c61 2c20 5068   Rada-Vilela, Ph
-00000710: 442a 2a5d 2868 7474 7073 3a2f 2f66 757a  D**](https://fuz
-00000720: 7a79 6c69 7465 2e63 6f6d 2f61 626f 7574  zylite.com/about
-00000730: 290a 0a3c 6272 3e0a 3c62 723e 0a0a 5b21  )..<br>.<br>..[!
-00000740: 5b4c 6963 656e 7365 3a20 4750 4c20 7633  [License: GPL v3
-00000750: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000760: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
-00000770: 6963 656e 7365 2d47 504c 2532 3076 332d  icense-GPL%20v3-
-00000780: 626c 7565 2e73 7667 295d 2868 7474 7073  blue.svg)](https
-00000790: 3a2f 2f6f 7065 6e73 6f75 7263 652e 6f72  ://opensource.or
-000007a0: 672f 6c69 6365 6e73 652f 6770 6c2d 332d  g/license/gpl-3-
-000007b0: 302f 290a 5b21 5b4c 6963 656e 7365 3a20  0/).[![License: 
-000007c0: 5061 6964 5d28 6874 7470 733a 2f2f 696d  Paid](https://im
-000007d0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000007e0: 6765 2f4c 6963 656e 7365 2d70 726f 7072  ge/License-propr
-000007f0: 6965 7461 7279 2d62 6c75 6529 5d28 6d61  ietary-blue)](ma
-00000800: 696c 746f 3a73 616c 6573 4066 757a 7a79  ilto:sales@fuzzy
-00000810: 6c69 7465 2e63 6f6d 290a 5b21 5b43 6f76  lite.com).[![Cov
-00000820: 6572 6167 6520 5374 6174 7573 5d28 0a68  erage Status](.h
-00000830: 7474 7073 3a2f 2f63 6f76 6572 616c 6c73  ttps://coveralls
-00000840: 2e69 6f2f 7265 706f 732f 6769 7468 7562  .io/repos/github
-00000850: 2f66 757a 7a79 6c69 7465 2f70 7966 757a  /fuzzylite/pyfuz
-00000860: 7a79 6c69 7465 2f62 6164 6765 2e73 7667  zylite/badge.svg
-00000870: 3f62 7261 6e63 683d 6d61 696e 295d 280a  ?branch=main)](.
-00000880: 6874 7470 733a 2f2f 636f 7665 7261 6c6c  https://coverall
-00000890: 732e 696f 2f67 6974 6875 622f 6675 7a7a  s.io/github/fuzz
-000008a0: 796c 6974 652f 7079 6675 7a7a 796c 6974  ylite/pyfuzzylit
-000008b0: 653f 6272 616e 6368 3d6d 6169 6e29 0a5b  e?branch=main).[
-000008c0: 215b 4275 696c 645d 2868 7474 7073 3a2f  ![Build](https:/
-000008d0: 2f67 6974 6875 622e 636f 6d2f 6675 7a7a  /github.com/fuzz
-000008e0: 796c 6974 652f 7079 6675 7a7a 796c 6974  ylite/pyfuzzylit
-000008f0: 652f 6163 7469 6f6e 732f 776f 726b 666c  e/actions/workfl
-00000900: 6f77 732f 6275 696c 642e 796d 6c2f 6261  ows/build.yml/ba
-00000910: 6467 652e 7376 6729 5d28 0a68 7474 7073  dge.svg)](.https
-00000920: 3a2f 2f67 6974 6875 622e 636f 6d2f 6675  ://github.com/fu
-00000930: 7a7a 796c 6974 652f 7079 6675 7a7a 796c  zzylite/pyfuzzyl
-00000940: 6974 652f 6163 7469 6f6e 732f 776f 726b  ite/actions/work
-00000950: 666c 6f77 732f 6275 696c 642e 796d 6c29  flows/build.yml)
-00000960: 0a5b 215b 5465 7374 5d28 6874 7470 733a  .[![Test](https:
-00000970: 2f2f 6769 7468 7562 2e63 6f6d 2f66 757a  //github.com/fuz
-00000980: 7a79 6c69 7465 2f70 7966 757a 7a79 6c69  zylite/pyfuzzyli
-00000990: 7465 2f61 6374 696f 6e73 2f77 6f72 6b66  te/actions/workf
-000009a0: 6c6f 7773 2f74 6573 742e 796d 6c2f 6261  lows/test.yml/ba
-000009b0: 6467 652e 7376 6729 5d28 0a68 7474 7073  dge.svg)](.https
-000009c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6675  ://github.com/fu
-000009d0: 7a7a 796c 6974 652f 7079 6675 7a7a 796c  zzylite/pyfuzzyl
-000009e0: 6974 652f 6163 7469 6f6e 732f 776f 726b  ite/actions/work
-000009f0: 666c 6f77 732f 7465 7374 2e79 6d6c 290a  flows/test.yml).
-00000a00: 5b21 5b50 7562 6c69 7368 5d28 6874 7470  [![Publish](http
-00000a10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-00000a20: 757a 7a79 6c69 7465 2f70 7966 757a 7a79  uzzylite/pyfuzzy
-00000a30: 6c69 7465 2f61 6374 696f 6e73 2f77 6f72  lite/actions/wor
-00000a40: 6b66 6c6f 7773 2f70 7562 6c69 7368 2e79  kflows/publish.y
-00000a50: 6d6c 2f62 6164 6765 2e73 7667 295d 280a  ml/badge.svg)](.
-00000a60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000a70: 6f6d 2f66 757a 7a79 6c69 7465 2f70 7966  om/fuzzylite/pyf
-00000a80: 757a 7a79 6c69 7465 2f61 6374 696f 6e73  uzzylite/actions
-00000a90: 2f77 6f72 6b66 6c6f 7773 2f70 7562 6c69  /workflows/publi
-00000aa0: 7368 2e79 6d6c 290a 0a23 2320 3c61 206e  sh.yml)..## <a n
-00000ab0: 616d 653d 2266 757a 7a79 6c69 7465 223e  ame="fuzzylite">
-00000ac0: 4675 7a7a 794c 6974 653c 2f61 3e0a 0a2a  FuzzyLite</a>..*
-00000ad0: 2a54 6865 2046 757a 7a79 4c69 7465 204c  *The FuzzyLite L
-00000ae0: 6962 7261 7269 6573 2066 6f72 2046 757a  ibraries for Fuz
-00000af0: 7a79 204c 6f67 6963 2043 6f6e 7472 6f6c  zy Logic Control
-00000b00: 2a2a 2072 6566 6572 2074 6f20 5b60 6675  ** refer to [`fu
-00000b10: 7a7a 796c 6974 6560 5d28 6874 7470 733a  zzylite`](https:
-00000b20: 2f2f 6769 7468 7562 2e63 6f6d 2f66 757a  //github.com/fuz
-00000b30: 7a79 6c69 7465 2f66 757a 7a79 6c69 7465  zylite/fuzzylite
-00000b40: 2f29 0a28 432b 2b29 2c20 5b60 7079 6675  /).(C++), [`pyfu
-00000b50: 7a7a 796c 6974 6560 5d28 6874 7470 733a  zzylite`](https:
-00000b60: 2f2f 6769 7468 7562 2e63 6f6d 2f66 757a  //github.com/fuz
-00000b70: 7a79 6c69 7465 2f70 7966 757a 7a79 6c69  zylite/pyfuzzyli
-00000b80: 7465 2f29 2028 5079 7468 6f6e 292c 0a61  te/) (Python),.a
-00000b90: 6e64 205b 606a 6675 7a7a 796c 6974 6560  nd [`jfuzzylite`
-00000ba0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000bb0: 2e63 6f6d 2f66 757a 7a79 6c69 7465 2f6a  .com/fuzzylite/j
-00000bc0: 6675 7a7a 796c 6974 652f 2920 284a 6176  fuzzylite/) (Jav
-00000bd0: 6129 2e0a 0a54 6865 202a 2a67 6f61 6c2a  a)...The **goal*
-00000be0: 2a20 6f66 2074 6865 2046 757a 7a79 4c69  * of the FuzzyLi
-00000bf0: 7465 204c 6962 7261 7269 6573 2069 7320  te Libraries is 
-00000c00: 746f 202a 2a65 6173 696c 792a 2a20 6465  to **easily** de
-00000c10: 7369 676e 2061 6e64 202a 2a65 6666 6963  sign and **effic
-00000c20: 6965 6e74 6c79 2a2a 206f 7065 7261 7465  iently** operate
-00000c30: 2066 757a 7a79 206c 6f67 6963 2063 6f6e   fuzzy logic con
-00000c40: 7472 6f6c 6c65 7273 0a66 6f6c 6c6f 7769  trollers.followi
-00000c50: 6e67 2061 6e20 2a2a 6f62 6a65 6374 2d6f  ng an **object-o
-00000c60: 7269 656e 7465 642a 2a20 7072 6f67 7261  riented** progra
-00000c70: 6d6d 696e 6720 6d6f 6465 6c20 7769 7468  mming model with
-00000c80: 206d 696e 696d 616c 2064 6570 656e 6465   minimal depende
-00000c90: 6e63 7920 6f6e 2065 7874 6572 6e61 6c20  ncy on external 
-00000ca0: 6c69 6272 6172 6965 732e 0a0a 2323 203c  libraries...## <
-00000cb0: 6120 6e61 6d65 3d22 6c69 6365 6e73 6522  a name="license"
-00000cc0: 3e4c 6963 656e 7365 3c2f 613e 0a0a 6070  >License</a>..`p
-00000cd0: 7966 757a 7a79 6c69 7465 6020 6973 2064  yfuzzylite` is d
-00000ce0: 7561 6c2d 6c69 6365 6e73 6564 2075 6e64  ual-licensed und
-00000cf0: 6572 2074 6865 205b 2a2a 474e 5520 4750  er the [**GNU GP
-00000d00: 4c20 332e 302a 2a5d 2868 7474 7073 3a2f  L 3.0**](https:/
-00000d10: 2f6f 7065 6e73 6f75 7263 652e 6f72 672f  /opensource.org/
-00000d20: 6c69 6365 6e73 652f 6770 6c2d 332d 302f  license/gpl-3-0/
-00000d30: 2920 616e 6420 756e 6465 7220 610a 2a2a  ) and under a.**
-00000d40: 7072 6f70 7269 6574 6172 7920 6c69 6365  proprietary lice
-00000d50: 6e73 6520 666f 7220 636f 6d6d 6572 6369  nse for commerci
-00000d60: 616c 2070 7572 706f 7365 732a 2a2e 0a0a  al purposes**...
-00000d70: 596f 7520 6172 6520 2a2a 7374 726f 6e67  You are **strong
-00000d80: 6c79 2a2a 2065 6e63 6f75 7261 6765 6420  ly** encouraged 
-00000d90: 746f 2073 7570 706f 7274 2074 6865 2064  to support the d
-00000da0: 6576 656c 6f70 6d65 6e74 206f 6620 7468  evelopment of th
-00000db0: 6520 4675 7a7a 794c 6974 6520 4c69 6272  e FuzzyLite Libr
-00000dc0: 6172 6965 7320 6279 2070 7572 6368 6173  aries by purchas
-00000dd0: 696e 6720 6120 6c69 6365 6e73 650a 6f66  ing a license.of
-00000de0: 205b 6051 7446 757a 7a79 4c69 7465 605d   [`QtFuzzyLite`]
-00000df0: 2868 7474 7073 3a2f 2f66 757a 7a79 6c69  (https://fuzzyli
-00000e00: 7465 2e63 6f6d 2f64 6f77 6e6c 6f61 6473  te.com/downloads
-00000e10: 292e 0a0a 5b60 5174 4675 7a7a 794c 6974  )...[`QtFuzzyLit
-00000e20: 6560 5d28 6874 7470 733a 2f2f 6675 7a7a  e`](https://fuzz
-00000e30: 796c 6974 652e 636f 6d2f 646f 776e 6c6f  ylite.com/downlo
-00000e40: 6164 732f 2920 6973 2074 6865 2062 6573  ads/) is the bes
-00000e50: 7420 6772 6170 6869 6361 6c20 7573 6572  t graphical user
-00000e60: 2069 6e74 6572 6661 6365 2061 7661 696c   interface avail
-00000e70: 6162 6c65 2074 6f20 6561 7369 6c79 2064  able to easily d
-00000e80: 6573 6967 6e20 616e 640a 6469 7265 6374  esign and.direct
-00000e90: 6c79 206f 7065 7261 7465 2066 757a 7a79  ly operate fuzzy
-00000ea0: 206c 6f67 6963 2063 6f6e 7472 6f6c 6c65   logic controlle
-00000eb0: 7273 2069 6e20 7265 616c 2074 696d 652e  rs in real time.
-00000ec0: 2041 7661 696c 6162 6c65 2066 6f72 2057   Available for W
-00000ed0: 696e 646f 7773 2c20 4d61 632c 2061 6e64  indows, Mac, and
-00000ee0: 204c 696e 7578 2c20 6974 7320 676f 616c   Linux, its goal
-00000ef0: 2069 7320 746f 0a73 6967 6e69 6669 6361   is to.significa
-00000f00: 6e74 6c79 202a 2a73 7065 6564 2075 702a  ntly **speed up*
-00000f10: 2a20 7468 6520 6465 7369 676e 206f 6620  * the design of 
-00000f20: 796f 7572 2066 757a 7a79 206c 6f67 6963  your fuzzy logic
-00000f30: 2063 6f6e 7472 6f6c 6c65 7273 2c20 7768   controllers, wh
-00000f40: 696c 6520 7072 6f76 6964 696e 6720 6120  ile providing a 
-00000f50: 7665 7279 202a 2a75 7365 6675 6c2a 2a2c  very **useful**,
-00000f60: 202a 2a66 756e 6374 696f 6e61 6c2a 2a0a   **functional**.
-00000f70: 616e 6420 2a2a 6265 6175 7469 6675 6c2a  and **beautiful*
-00000f80: 2a20 7573 6572 2069 6e74 6572 6661 6365  * user interface
-00000f90: 2e0a 506c 6561 7365 2c20 646f 776e 6c6f  ..Please, downlo
-00000fa0: 6164 2069 7420 616e 6420 6368 6563 6b20  ad it and check 
-00000fb0: 6974 206f 7574 2066 6f72 2066 7265 6520  it out for free 
-00000fc0: 6174 205b 6675 7a7a 796c 6974 652e 636f  at [fuzzylite.co
-00000fd0: 6d2f 646f 776e 6c6f 6164 735d 2868 7474  m/downloads](htt
-00000fe0: 7073 3a2f 2f66 757a 7a79 6c69 7465 2e63  ps://fuzzylite.c
-00000ff0: 6f6d 2f64 6f77 6e6c 6f61 6473 292e 0a0a  om/downloads)...
-00001000: 2323 203c 6120 6e61 6d65 3d22 696e 7374  ## <a name="inst
-00001010: 616c 6c22 3e49 6e73 7461 6c6c 3c2f 613e  all">Install</a>
-00001020: 0a0a 6060 6063 6f6d 6d61 6e64 6c69 6e65  ..```commandline
-00001030: 0a70 6970 2069 6e73 7461 6c6c 2070 7966  .pip install pyf
-00001040: 757a 7a79 6c69 7465 0a60 6060 0a0a 2323  uzzylite.```..##
-00001050: 203c 6120 6e61 6d65 3d22 6665 6174 7572   <a name="featur
-00001060: 6573 223e 4665 6174 7572 6573 3c2f 613e  es">Features</a>
-00001070: 0a0a 2a2a 446f 6375 6d65 6e74 6174 696f  ..**Documentatio
-00001080: 6e2a 2a3a 205b 6675 7a7a 796c 6974 652e  n**: [fuzzylite.
-00001090: 6769 7468 7562 2e69 6f2f 7079 6675 7a7a  github.io/pyfuzz
-000010a0: 796c 6974 652f 5d28 6874 7470 733a 2f2f  ylite/](https://
-000010b0: 6675 7a7a 796c 6974 652e 6769 7468 7562  fuzzylite.github
-000010c0: 2e69 6f2f 7079 6675 7a7a 796c 6974 652f  .io/pyfuzzylite/
-000010d0: 290a 0a2a 2a28 3629 2043 6f6e 7472 6f6c  )..**(6) Control
-000010e0: 6c65 7273 2a2a 3a20 4d61 6d64 616e 692c  lers**: Mamdani,
-000010f0: 2054 616b 6167 692d 5375 6765 6e6f 2c20   Takagi-Sugeno, 
-00001100: 4c61 7273 656e 2c20 5473 756b 616d 6f74  Larsen, Tsukamot
-00001110: 6f2c 2049 6e76 6572 7365 2054 7375 6b61  o, Inverse Tsuka
-00001120: 6d6f 746f 2c20 4879 6272 6964 0a0a 2a2a  moto, Hybrid..**
-00001130: 2832 3529 204c 696e 6775 6973 7469 6320  (25) Linguistic 
-00001140: 7465 726d 732a 2a3a 2020 2835 2920 2a42  terms**:  (5) *B
-00001150: 6173 6963 2a3a 2054 7269 616e 676c 652c  asic*: Triangle,
-00001160: 2054 7261 7065 7a6f 6964 2c20 5265 6374   Trapezoid, Rect
-00001170: 616e 676c 652c 2044 6973 6372 6574 652c  angle, Discrete,
-00001180: 2053 656d 6945 6c6c 6970 7365 2e0a 2838   SemiEllipse..(8
-00001190: 2920 2a45 7874 656e 6465 642a 3a20 4265  ) *Extended*: Be
-000011a0: 6c6c 2c20 436f 7369 6e65 2c20 4761 7573  ll, Cosine, Gaus
-000011b0: 7369 616e 2c20 4761 7573 7369 616e 5072  sian, GaussianPr
-000011c0: 6f64 7563 742c 2050 6953 6861 7065 2c20  oduct, PiShape, 
-000011d0: 5369 676d 6f69 6444 6966 6665 7265 6e63  SigmoidDifferenc
-000011e0: 652c 2053 6967 6d6f 6964 5072 6f64 7563  e, SigmoidProduc
-000011f0: 742c 2053 7069 6b65 2e0a 2837 2920 2a45  t, Spike..(7) *E
-00001200: 6467 6573 2a3a 2041 7263 2c20 4269 6e61  dges*: Arc, Bina
-00001210: 7279 2c20 436f 6e63 6176 652c 2052 616d  ry, Concave, Ram
-00001220: 702c 2053 6967 6d6f 6964 2c20 5353 6861  p, Sigmoid, SSha
-00001230: 7065 2c20 5a53 6861 7065 2e0a 2833 2920  pe, ZShape..(3) 
-00001240: 2a46 756e 6374 696f 6e73 2a3a 2043 6f6e  *Functions*: Con
-00001250: 7374 616e 742c 204c 696e 6561 722c 2046  stant, Linear, F
-00001260: 756e 6374 696f 6e2e 2028 3229 202a 5370  unction. (2) *Sp
-00001270: 6563 6961 6c2a 3a20 4167 6772 6567 6174  ecial*: Aggregat
-00001280: 6564 2c20 4163 7469 7661 7465 642e 0a0a  ed, Activated...
-00001290: 2a2a 2837 2920 4163 7469 7661 7469 6f6e  **(7) Activation
-000012a0: 206d 6574 686f 6473 2a2a 3a20 2047 656e   methods**:  Gen
-000012b0: 6572 616c 2c20 5072 6f70 6f72 7469 6f6e  eral, Proportion
-000012c0: 616c 2c20 5468 7265 7368 6f6c 642c 2046  al, Threshold, F
-000012d0: 6972 7374 2c20 4c61 7374 2c20 4c6f 7765  irst, Last, Lowe
-000012e0: 7374 2c20 4869 6768 6573 742e 0a0a 2a2a  st, Highest...**
-000012f0: 2839 2920 436f 6e6a 756e 6374 696f 6e20  (9) Conjunction 
-00001300: 616e 6420 496d 706c 6963 6174 696f 6e20  and Implication 
-00001310: 2854 2d4e 6f72 6d73 292a 2a3a 204d 696e  (T-Norms)**: Min
-00001320: 696d 756d 2c20 416c 6765 6272 6169 6350  imum, AlgebraicP
-00001330: 726f 6475 6374 2c20 426f 756e 6465 6444  roduct, BoundedD
-00001340: 6966 6665 7265 6e63 652c 2044 7261 7374  ifference, Drast
-00001350: 6963 5072 6f64 7563 742c 0a45 696e 7374  icProduct,.Einst
-00001360: 6569 6e50 726f 6475 6374 2c20 4861 6d61  einProduct, Hama
-00001370: 6368 6572 5072 6f64 7563 742c 204e 696c  cherProduct, Nil
-00001380: 706f 7465 6e74 4d69 6e69 6d75 6d2c 204c  potentMinimum, L
-00001390: 616d 6264 614e 6f72 6d2c 2046 756e 6374  ambdaNorm, Funct
-000013a0: 696f 6e4e 6f72 6d2e 0a0a 2a2a 2831 3129  ionNorm...**(11)
-000013b0: 2044 6973 6a75 6e63 7469 6f6e 2061 6e64   Disjunction and
-000013c0: 2041 6767 7265 6761 7469 6f6e 2028 532d   Aggregation (S-
-000013d0: 4e6f 726d 7329 2a2a 3a20 204d 6178 696d  Norms)**:  Maxim
-000013e0: 756d 2c20 416c 6765 6272 6169 6353 756d  um, AlgebraicSum
-000013f0: 2c20 426f 756e 6465 6453 756d 2c20 4472  , BoundedSum, Dr
-00001400: 6173 7469 6353 756d 2c20 4569 6e73 7465  asticSum, Einste
-00001410: 696e 5375 6d2c 0a48 616d 6163 6865 7253  inSum,.HamacherS
-00001420: 756d 2c20 4e69 6c70 6f74 656e 744d 6178  um, NilpotentMax
-00001430: 696d 756d 2c20 4e6f 726d 616c 697a 6564  imum, Normalized
-00001440: 5375 6d2c 2055 6e62 6f75 6e64 6564 5375  Sum, UnboundedSu
-00001450: 6d2c 204c 616d 6264 614e 6f72 6d2c 2046  m, LambdaNorm, F
-00001460: 756e 6374 696f 6e4e 6f72 6d2e 0a0a 2a2a  unctionNorm...**
-00001470: 2837 2920 4465 6675 7a7a 6966 6965 7273  (7) Defuzzifiers
-00001480: 2a2a 3a20 2028 3529 202a 496e 7465 6772  **:  (5) *Integr
-00001490: 616c 2a3a 2043 656e 7472 6f69 642c 2042  al*: Centroid, B
-000014a0: 6973 6563 746f 722c 2053 6d61 6c6c 6573  isector, Smalles
-000014b0: 744f 664d 6178 696d 756d 2c20 4c61 7267  tOfMaximum, Larg
-000014c0: 6573 744f 664d 6178 696d 756d 2c20 4d65  estOfMaximum, Me
-000014d0: 616e 4f66 4d61 7869 6d75 6d2e 0a28 3229  anOfMaximum..(2)
-000014e0: 202a 5765 6967 6874 6564 2a3a 2057 6569   *Weighted*: Wei
-000014f0: 6768 7465 6441 7665 7261 6765 2c20 5765  ghtedAverage, We
-00001500: 6967 6874 6564 5375 6d2e 0a0a 2a2a 2837  ightedSum...**(7
-00001510: 2920 4865 6467 6573 2a2a 3a20 416e 792c  ) Hedges**: Any,
-00001520: 204e 6f74 2c20 4578 7472 656d 656c 792c   Not, Extremely,
-00001530: 2053 656c 646f 6d2c 2053 6f6d 6577 6861   Seldom, Somewha
-00001540: 742c 2056 6572 792c 2046 756e 6374 696f  t, Very, Functio
-00001550: 6e2e 0a0a 2a2a 2833 2920 496d 706f 7274  n...**(3) Import
-00001560: 6572 732a 2a3a 2046 757a 7a79 4c69 7465  ers**: FuzzyLite
-00001570: 204c 616e 6775 6167 6520 6066 6c6c 602e   Language `fll`.
-00001580: 2057 6974 6820 6066 757a 7a79 6c69 7465   With `fuzzylite
-00001590: 603a 2046 757a 7a79 2049 6e66 6572 656e  `: Fuzzy Inferen
-000015a0: 6365 2053 7973 7465 6d20 6066 6973 602c  ce System `fis`,
-000015b0: 2046 757a 7a79 2043 6f6e 7472 6f6c 0a4c   Fuzzy Control.L
-000015c0: 616e 6775 6167 6520 6066 636c 602e 0a0a  anguage `fcl`...
-000015d0: 2a2a 2837 2920 4578 706f 7274 6572 732a  **(7) Exporters*
-000015e0: 2a3a 2060 5079 7468 6f6e 602c 2046 757a  *: `Python`, Fuz
-000015f0: 7a79 4c69 7465 204c 616e 6775 6167 6520  zyLite Language 
-00001600: 6066 6c6c 602c 2046 757a 7a79 4c69 7465  `fll`, FuzzyLite
-00001610: 2044 6174 6173 6574 2060 666c 6460 2e20   Dataset `fld`. 
-00001620: 5769 7468 2060 6675 7a7a 796c 6974 6560  With `fuzzylite`
-00001630: 3a20 6043 2b2b 602c 2060 4a61 7661 602c  : `C++`, `Java`,
-00001640: 0a46 757a 7a79 4c69 7465 204c 616e 6775  .FuzzyLite Langu
-00001650: 6167 6520 6066 6c6c 602c 2046 757a 7a79  age `fll`, Fuzzy
-00001660: 4c69 7465 2044 6174 6173 6574 2060 666c  Lite Dataset `fl
-00001670: 6460 2c20 6052 6020 7363 7269 7074 2c20  d`, `R` script, 
-00001680: 4675 7a7a 7920 496e 6665 7265 6e63 6520  Fuzzy Inference 
-00001690: 5379 7374 656d 2060 6669 7360 2c20 4675  System `fis`, Fu
-000016a0: 7a7a 7920 436f 6e74 726f 6c0a 4c61 6e67  zzy Control.Lang
-000016b0: 7561 6765 2060 6663 6c60 2e0a 0a2a 2a28  uage `fcl`...**(
-000016c0: 3330 2b29 2045 7861 6d70 6c65 732a 2a20  30+) Examples** 
-000016d0: 206f 6620 4d61 6d64 616e 692c 2054 616b   of Mamdani, Tak
-000016e0: 6167 692d 5375 6765 6e6f 2c20 5473 756b  agi-Sugeno, Tsuk
-000016f0: 616d 6f74 6f2c 2061 6e64 2048 7962 7269  amoto, and Hybri
-00001700: 6420 636f 6e74 726f 6c6c 6572 7320 6672  d controllers fr
-00001710: 6f6d 2060 6675 7a7a 796c 6974 6560 2c20  om `fuzzylite`, 
-00001720: 4f63 7461 7665 2c20 616e 6420 4d61 746c  Octave, and Matl
-00001730: 6162 2c0a 6561 6368 2069 6e63 6c75 6465  ab,.each include
-00001740: 6420 696e 2074 6865 2066 6f6c 6c6f 7769  d in the followi
-00001750: 6e67 2066 6f72 6d61 7473 3a20 6070 7960  ng formats: `py`
-00001760: 2c20 6066 6c6c 602c 2060 666c 6460 2e20  , `fll`, `fld`. 
-00001770: 5769 7468 2060 6675 7a7a 796c 6974 6560  With `fuzzylite`
-00001780: 3a20 6043 2b2b 602c 2060 4a61 7661 602c  : `C++`, `Java`,
-00001790: 2060 5260 2c20 6066 6973 602c 2061 6e64   `R`, `fis`, and
-000017a0: 2060 6663 6c60 2e0a 0a23 2320 3c61 206e   `fcl`...## <a n
-000017b0: 616d 653d 2265 7861 6d70 6c65 7322 3e45  ame="examples">E
-000017c0: 7861 6d70 6c65 733c 2f61 3e0a 0a23 2323  xamples</a>..###
-000017d0: 2046 757a 7a79 4c69 7465 204c 616e 6775   FuzzyLite Langu
-000017e0: 6167 650a 0a60 6060 7961 6d6c 0a23 2046  age..```yaml.# F
-000017f0: 696c 653a 2065 7861 6d70 6c65 732f 6d61  ile: examples/ma
-00001800: 6d64 616e 692f 4f62 7374 6163 6c65 4176  mdani/ObstacleAv
-00001810: 6f69 6461 6e63 652e 666c 6c0a 456e 6769  oidance.fll.Engi
-00001820: 6e65 3a20 4f62 7374 6163 6c65 4176 6f69  ne: ObstacleAvoi
-00001830: 6461 6e63 650a 496e 7075 7456 6172 6961  dance.InputVaria
-00001840: 626c 653a 206f 6273 7461 636c 650a 2020  ble: obstacle.  
-00001850: 656e 6162 6c65 643a 2074 7275 650a 2020  enabled: true.  
-00001860: 7261 6e67 653a 2030 2e30 3030 2031 2e30  range: 0.000 1.0
-00001870: 3030 0a20 206c 6f63 6b2d 7261 6e67 653a  00.  lock-range:
-00001880: 2066 616c 7365 0a20 2074 6572 6d3a 206c   false.  term: l
-00001890: 6566 7420 5261 6d70 2031 2e30 3030 2030  eft Ramp 1.000 0
-000018a0: 2e30 3030 0a20 2074 6572 6d3a 2072 6967  .000.  term: rig
-000018b0: 6874 2052 616d 7020 302e 3030 3020 312e  ht Ramp 0.000 1.
-000018c0: 3030 300a 4f75 7470 7574 5661 7269 6162  000.OutputVariab
-000018d0: 6c65 3a20 6d53 7465 6572 0a20 2065 6e61  le: mSteer.  ena
-000018e0: 626c 6564 3a20 7472 7565 0a20 2072 616e  bled: true.  ran
-000018f0: 6765 3a20 302e 3030 3020 312e 3030 300a  ge: 0.000 1.000.
-00001900: 2020 6c6f 636b 2d72 616e 6765 3a20 6661    lock-range: fa
-00001910: 6c73 650a 2020 6167 6772 6567 6174 696f  lse.  aggregatio
-00001920: 6e3a 204d 6178 696d 756d 0a20 2064 6566  n: Maximum.  def
-00001930: 757a 7a69 6669 6572 3a20 4365 6e74 726f  uzzifier: Centro
-00001940: 6964 2031 3030 0a20 2064 6566 6175 6c74  id 100.  default
-00001950: 3a20 6e61 6e0a 2020 6c6f 636b 2d70 7265  : nan.  lock-pre
-00001960: 7669 6f75 733a 2066 616c 7365 0a20 2074  vious: false.  t
-00001970: 6572 6d3a 206c 6566 7420 5261 6d70 2031  erm: left Ramp 1
-00001980: 2e30 3030 2030 2e30 3030 0a20 2074 6572  .000 0.000.  ter
-00001990: 6d3a 2072 6967 6874 2052 616d 7020 302e  m: right Ramp 0.
-000019a0: 3030 3020 312e 3030 300a 5275 6c65 426c  000 1.000.RuleBl
-000019b0: 6f63 6b3a 206d 616d 6461 6e69 0a20 2065  ock: mamdani.  e
-000019c0: 6e61 626c 6564 3a20 7472 7565 0a20 2063  nabled: true.  c
-000019d0: 6f6e 6a75 6e63 7469 6f6e 3a20 6e6f 6e65  onjunction: none
-000019e0: 0a20 2064 6973 6a75 6e63 7469 6f6e 3a20  .  disjunction: 
-000019f0: 6e6f 6e65 0a20 2069 6d70 6c69 6361 7469  none.  implicati
-00001a00: 6f6e 3a20 416c 6765 6272 6169 6350 726f  on: AlgebraicPro
-00001a10: 6475 6374 0a20 2061 6374 6976 6174 696f  duct.  activatio
-00001a20: 6e3a 2047 656e 6572 616c 0a20 2072 756c  n: General.  rul
-00001a30: 653a 2069 6620 6f62 7374 6163 6c65 2069  e: if obstacle i
-00001a40: 7320 6c65 6674 2074 6865 6e20 6d53 7465  s left then mSte
-00001a50: 6572 2069 7320 7269 6768 740a 2020 7275  er is right.  ru
-00001a60: 6c65 3a20 6966 206f 6273 7461 636c 6520  le: if obstacle 
-00001a70: 6973 2072 6967 6874 2074 6865 6e20 6d53  is right then mS
-00001a80: 7465 6572 2069 7320 6c65 6674 0a60 6060  teer is left.```
-00001a90: 0a0a 6060 6070 7974 686f 6e0a 2320 5079  ..```python.# Py
-00001aa0: 7468 6f6e 0a69 6d70 6f72 7420 6675 7a7a  thon.import fuzz
-00001ab0: 796c 6974 6520 6173 2066 6c0a 0a65 6e67  ylite as fl..eng
-00001ac0: 696e 6520 3d20 666c 2e46 6c6c 496d 706f  ine = fl.FllImpo
-00001ad0: 7274 6572 2829 2e66 726f 6d5f 6669 6c65  rter().from_file
-00001ae0: 2822 6578 616d 706c 6573 2f6d 616d 6461  ("examples/mamda
-00001af0: 6e69 2f4f 6273 7461 636c 6541 766f 6964  ni/ObstacleAvoid
-00001b00: 616e 6365 2e66 6c6c 2229 0a60 6060 0a0a  ance.fll").```..
-00001b10: 2323 2320 5079 7468 6f6e 0a0a 6060 6070  ### Python..```p
-00001b20: 7974 686f 6e0a 696d 706f 7274 2066 757a  ython.import fuz
-00001b30: 7a79 6c69 7465 2061 7320 666c 0a0a 656e  zylite as fl..en
-00001b40: 6769 6e65 203d 2066 6c2e 456e 6769 6e65  gine = fl.Engine
-00001b50: 280a 2020 2020 6e61 6d65 3d22 4f62 7374  (.    name="Obst
-00001b60: 6163 6c65 4176 6f69 6461 6e63 6522 2c0a  acleAvoidance",.
-00001b70: 2020 2020 696e 7075 745f 7661 7269 6162      input_variab
-00001b80: 6c65 733d 5b0a 2020 2020 2020 2020 666c  les=[.        fl
-00001b90: 2e49 6e70 7574 5661 7269 6162 6c65 280a  .InputVariable(.
-00001ba0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00001bb0: 3d22 6f62 7374 6163 6c65 222c 0a20 2020  ="obstacle",.   
-00001bc0: 2020 2020 2020 2020 206d 696e 696d 756d           minimum
-00001bd0: 3d30 2e30 2c0a 2020 2020 2020 2020 2020  =0.0,.          
-00001be0: 2020 6d61 7869 6d75 6d3d 312e 302c 0a20    maximum=1.0,. 
-00001bf0: 2020 2020 2020 2020 2020 206c 6f63 6b5f             lock_
-00001c00: 7261 6e67 653d 4661 6c73 652c 0a20 2020  range=False,.   
-00001c10: 2020 2020 2020 2020 2074 6572 6d73 3d5b           terms=[
-00001c20: 666c 2e52 616d 7028 226c 6566 7422 2c20  fl.Ramp("left", 
-00001c30: 312e 302c 2030 2e30 292c 2066 6c2e 5261  1.0, 0.0), fl.Ra
-00001c40: 6d70 2822 7269 6768 7422 2c20 302e 302c  mp("right", 0.0,
-00001c50: 2031 2e30 295d 2c0a 2020 2020 2020 2020   1.0)],.        
-00001c60: 290a 2020 2020 5d2c 0a20 2020 206f 7574  ).    ],.    out
-00001c70: 7075 745f 7661 7269 6162 6c65 733d 5b0a  put_variables=[.
-00001c80: 2020 2020 2020 2020 666c 2e4f 7574 7075          fl.Outpu
-00001c90: 7456 6172 6961 626c 6528 0a20 2020 2020  tVariable(.     
-00001ca0: 2020 2020 2020 206e 616d 653d 226d 5374         name="mSt
-00001cb0: 6565 7222 2c0a 2020 2020 2020 2020 2020  eer",.          
-00001cc0: 2020 6d69 6e69 6d75 6d3d 302e 302c 0a20    minimum=0.0,. 
-00001cd0: 2020 2020 2020 2020 2020 206d 6178 696d             maxim
-00001ce0: 756d 3d31 2e30 2c0a 2020 2020 2020 2020  um=1.0,.        
-00001cf0: 2020 2020 6c6f 636b 5f72 616e 6765 3d46      lock_range=F
-00001d00: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00001d10: 2020 6c6f 636b 5f70 7265 7669 6f75 733d    lock_previous=
-00001d20: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-00001d30: 2020 2064 6566 6175 6c74 5f76 616c 7565     default_value
-00001d40: 3d66 6c2e 6e61 6e2c 0a20 2020 2020 2020  =fl.nan,.       
-00001d50: 2020 2020 2061 6767 7265 6761 7469 6f6e       aggregation
-00001d60: 3d66 6c2e 4d61 7869 6d75 6d28 292c 0a20  =fl.Maximum(),. 
-00001d70: 2020 2020 2020 2020 2020 2064 6566 757a             defuz
-00001d80: 7a69 6669 6572 3d66 6c2e 4365 6e74 726f  zifier=fl.Centro
-00001d90: 6964 2872 6573 6f6c 7574 696f 6e3d 3130  id(resolution=10
-00001da0: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
-00001db0: 7465 726d 733d 5b66 6c2e 5261 6d70 2822  terms=[fl.Ramp("
-00001dc0: 6c65 6674 222c 2031 2e30 2c20 302e 3029  left", 1.0, 0.0)
-00001dd0: 2c20 666c 2e52 616d 7028 2272 6967 6874  , fl.Ramp("right
-00001de0: 222c 2030 2e30 2c20 312e 3029 5d2c 0a20  ", 0.0, 1.0)],. 
-00001df0: 2020 2020 2020 2029 0a20 2020 205d 2c0a         ).    ],.
-00001e00: 2020 2020 7275 6c65 5f62 6c6f 636b 733d      rule_blocks=
-00001e10: 5b0a 2020 2020 2020 2020 666c 2e52 756c  [.        fl.Rul
-00001e20: 6542 6c6f 636b 280a 2020 2020 2020 2020  eBlock(.        
-00001e30: 2020 2020 6e61 6d65 3d22 6d61 6d64 616e      name="mamdan
-00001e40: 6922 2c0a 2020 2020 2020 2020 2020 2020  i",.            
-00001e50: 636f 6e6a 756e 6374 696f 6e3d 4e6f 6e65  conjunction=None
-00001e60: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
-00001e70: 736a 756e 6374 696f 6e3d 4e6f 6e65 2c0a  sjunction=None,.
-00001e80: 2020 2020 2020 2020 2020 2020 696d 706c              impl
-00001e90: 6963 6174 696f 6e3d 666c 2e41 6c67 6562  ication=fl.Algeb
-00001ea0: 7261 6963 5072 6f64 7563 7428 292c 0a20  raicProduct(),. 
-00001eb0: 2020 2020 2020 2020 2020 2061 6374 6976             activ
-00001ec0: 6174 696f 6e3d 666c 2e47 656e 6572 616c  ation=fl.General
-00001ed0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00001ee0: 7275 6c65 733d 5b0a 2020 2020 2020 2020  rules=[.        
-00001ef0: 2020 2020 2020 2020 666c 2e52 756c 652e          fl.Rule.
-00001f00: 6372 6561 7465 2822 6966 206f 6273 7461  create("if obsta
-00001f10: 636c 6520 6973 206c 6566 7420 7468 656e  cle is left then
-00001f20: 206d 5374 6565 7220 6973 2072 6967 6874   mSteer is right
-00001f30: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00001f40: 2020 2020 666c 2e52 756c 652e 6372 6561      fl.Rule.crea
-00001f50: 7465 2822 6966 206f 6273 7461 636c 6520  te("if obstacle 
-00001f60: 6973 2072 6967 6874 2074 6865 6e20 6d53  is right then mS
-00001f70: 7465 6572 2069 7320 6c65 6674 2229 2c0a  teer is left"),.
-00001f80: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-00001f90: 2020 2020 2020 2029 0a20 2020 205d 2c0a         ).    ],.
-00001fa0: 290a 6060 600a 0a23 2323 2060 666c 6f61  ).```..### `floa
-00001fb0: 7460 2061 6e64 2076 6563 746f 7269 7a61  t` and vectoriza
-00001fc0: 7469 6f6e 0a0a 6060 6070 7974 686f 6e0a  tion..```python.
-00001fd0: 2320 7369 6e67 6c65 2060 666c 6f61 7460  # single `float`
-00001fe0: 206f 7065 7261 7469 6f6e 0a65 6e67 696e   operation.engin
-00001ff0: 652e 696e 7075 745f 7661 7269 6162 6c65  e.input_variable
-00002000: 2822 6f62 7374 6163 6c65 2229 2e76 616c  ("obstacle").val
-00002010: 7565 203d 2030 2e35 0a65 6e67 696e 652e  ue = 0.5.engine.
-00002020: 7072 6f63 6573 7328 290a 7072 696e 7428  process().print(
-00002030: 2279 203d 222c 2065 6e67 696e 652e 6f75  "y =", engine.ou
-00002040: 7470 7574 5f76 6172 6961 626c 6528 226d  tput_variable("m
-00002050: 5374 6565 7222 292e 7661 6c75 6529 0a23  Steer").value).#
-00002060: 203e 2079 203d 2030 2e35 0a70 7269 6e74   > y = 0.5.print
-00002070: 2822 e1bb b920 3d22 2c20 656e 6769 6e65  ("... =", engine
-00002080: 2e6f 7574 7075 745f 7661 7269 6162 6c65  .output_variable
-00002090: 2822 6d53 7465 6572 2229 2e66 757a 7a79  ("mSteer").fuzzy
-000020a0: 5f76 616c 7565 2829 290a 2320 3e20 e1bb  _value()).# > ..
-000020b0: b920 3d20 302e 3530 302f 6c65 6674 202b  . = 0.500/left +
-000020c0: 2030 2e35 3030 2f72 6967 6874 0a0a 2320   0.500/right..# 
-000020d0: 7665 6374 6f72 697a 6174 696f 6e0a 656e  vectorization.en
-000020e0: 6769 6e65 2e69 6e70 7574 5f76 6172 6961  gine.input_varia
-000020f0: 626c 6528 226f 6273 7461 636c 6522 292e  ble("obstacle").
-00002100: 7661 6c75 6520 3d20 666c 2e61 7272 6179  value = fl.array
-00002110: 285b 302c 2030 2e32 352c 2030 2e35 2c20  ([0, 0.25, 0.5, 
-00002120: 302e 3735 2c20 312e 305d 290a 656e 6769  0.75, 1.0]).engi
-00002130: 6e65 2e70 726f 6365 7373 2829 0a70 7269  ne.process().pri
-00002140: 6e74 2822 7920 3d22 2c20 7265 7072 2865  nt("y =", repr(e
-00002150: 6e67 696e 652e 6f75 7470 7574 5f76 6172  ngine.output_var
-00002160: 6961 626c 6528 226d 5374 6565 7222 292e  iable("mSteer").
-00002170: 7661 6c75 6529 290a 2320 3e20 7920 3d20  value)).# > y = 
-00002180: 6172 7261 7928 5b30 2e36 3636 3636 3635  array([0.6666665
-00002190: 202c 2030 2e36 3231 3739 3437 372c 2030   , 0.62179477, 0
-000021a0: 2e35 2020 2020 2020 202c 2030 2e33 3738  .5       , 0.378
-000021b0: 3230 3532 332c 2030 2e33 3333 3333 3335  20523, 0.3333335
-000021c0: 205d 290a 7072 696e 7428 22e1 bbb9 203d   ]).print("... =
-000021d0: 222c 2072 6570 7228 656e 6769 6e65 2e6f  ", repr(engine.o
-000021e0: 7574 7075 745f 7661 7269 6162 6c65 2822  utput_variable("
-000021f0: 6d53 7465 6572 2229 2e66 757a 7a79 5f76  mSteer").fuzzy_v
-00002200: 616c 7565 2829 2929 0a23 203e 20e1 bbb9  alue())).# > ...
-00002210: 203d 2061 7272 6179 285b 2730 2e30 3030   = array(['0.000
-00002220: 2f6c 6566 7420 2b20 312e 3030 302f 7269  /left + 1.000/ri
-00002230: 6768 7427 2c0a 2320 2020 2020 2020 2020  ght',.#         
-00002240: 2020 2020 2027 302e 3235 302f 6c65 6674       '0.250/left
-00002250: 202b 2030 2e37 3530 2f72 6967 6874 272c   + 0.750/right',
-00002260: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
-00002270: 2730 2e35 3030 2f6c 6566 7420 2b20 302e  '0.500/left + 0.
-00002280: 3530 302f 7269 6768 7427 2c0a 2320 2020  500/right',.#   
-00002290: 2020 2020 2020 2020 2020 2027 302e 3735             '0.75
-000022a0: 302f 6c65 6674 202b 2030 2e32 3530 2f72  0/left + 0.250/r
-000022b0: 6967 6874 272c 0a23 2020 2020 2020 2020  ight',.#        
-000022c0: 2020 2020 2020 2731 2e30 3030 2f6c 6566        '1.000/lef
-000022d0: 7420 2b20 302e 3030 302f 7269 6768 7427  t + 0.000/right'
-000022e0: 5d2c 2064 7479 7065 3d27 3c55 3236 2729  ], dtype='<U26')
-000022f0: 0a60 6060 0a0a 506c 6561 7365 2072 6566  .```..Please ref
-00002300: 6572 2074 6f20 7468 6520 646f 6375 6d65  er to the docume
-00002310: 6e74 6174 696f 6e20 666f 7220 6d6f 7265  ntation for more
-00002320: 0a69 6e66 6f72 6d61 7469 6f6e 3a20 5b2a  .information: [*
-00002330: 2a66 757a 7a79 6c69 7465 2e67 6974 6875  *fuzzylite.githu
-00002340: 622e 696f 2f70 7966 757a 7a79 6c69 7465  b.io/pyfuzzylite
-00002350: 2f2a 2a5d 2868 7474 7073 3a2f 2f66 757a  /**](https://fuz
-00002360: 7a79 6c69 7465 2e67 6974 6875 622e 696f  zylite.github.io
-00002370: 2f70 7966 757a 7a79 6c69 7465 2f29 0a0a  /pyfuzzylite/)..
-00002380: 2323 203c 6120 6e61 6d65 3d22 636f 6e74  ## <a name="cont
-00002390: 7269 6275 7469 6e67 223e 436f 6e74 7269  ributing">Contri
-000023a0: 6275 7469 6e67 3c2f 613e 0a0a 416c 6c20  buting</a>..All 
-000023b0: 636f 6e74 7269 6275 7469 6f6e 7320 6172  contributions ar
-000023c0: 6520 7765 6c63 6f6d 652c 2070 726f 7669  e welcome, provi
-000023d0: 6465 6420 7468 6579 2066 6f6c 6c6f 7720  ded they follow 
-000023e0: 7468 6520 666f 6c6c 6f77 696e 6720 6775  the following gu
-000023f0: 6964 656c 696e 6573 3a0a 0a2d 2053 6f75  idelines:..- Sou
-00002400: 7263 6520 636f 6465 2069 7320 636f 6e73  rce code is cons
-00002410: 6973 7465 6e74 2077 6974 6820 7374 616e  istent with stan
-00002420: 6461 7264 7320 696e 2074 6865 206c 6962  dards in the lib
-00002430: 7261 7279 0a2d 2043 6f6e 7472 6962 7574  rary.- Contribut
-00002440: 696f 6e20 6973 2070 726f 7065 726c 7920  ion is properly 
-00002450: 646f 6375 6d65 6e74 6564 2061 6e64 2074  documented and t
-00002460: 6573 7465 642c 2072 6169 7369 6e67 2069  ested, raising i
-00002470: 7373 7565 7320 7768 6572 6520 6170 7072  ssues where appr
-00002480: 6f70 7269 6174 650a 2d20 436f 6e74 7269  opriate.- Contri
-00002490: 6275 7469 6f6e 2069 7320 6c69 6365 6e73  bution is licens
-000024a0: 6564 2075 6e64 6572 2074 6865 2046 757a  ed under the Fuz
-000024b0: 7a79 4c69 7465 204c 6963 656e 7365 0a0a  zyLite License..
-000024c0: 2323 203c 6120 6e61 6d65 3d22 7265 6665  ## <a name="refe
-000024d0: 7265 6e63 6522 3e52 6566 6572 656e 6365  rence">Reference
-000024e0: 3c2f 613e 0a0a 4966 2079 6f75 2061 7265  </a>..If you are
-000024f0: 2075 7369 6e67 2074 6865 2046 757a 7a79   using the Fuzzy
-00002500: 4c69 7465 204c 6962 7261 7269 6573 2c20  Lite Libraries, 
-00002510: 706c 6561 7365 2063 6974 6520 7468 6520  please cite the 
-00002520: 666f 6c6c 6f77 696e 6720 7265 6665 7265  following refere
-00002530: 6e63 6520 696e 2079 6f75 7220 6172 7469  nce in your arti
-00002540: 636c 653a 0a0a 3e20 4a75 616e 2052 6164  cle:..> Juan Rad
-00002550: 612d 5669 6c65 6c61 2e20 5468 6520 4675  a-Vilela. The Fu
-00002560: 7a7a 794c 6974 6520 4c69 6272 6172 6965  zzyLite Librarie
-00002570: 7320 666f 7220 4675 7a7a 7920 4c6f 6769  s for Fuzzy Logi
-00002580: 6320 436f 6e74 726f 6c2c 2032 3031 382e  c Control, 2018.
-00002590: 2055 524c 2068 7474 7073 3a2f 2f66 757a   URL https://fuz
-000025a0: 7a79 6c69 7465 2e63 6f6d 2e0a 0a4f 7220  zylite.com...Or 
-000025b0: 7573 696e 6720 6062 6962 7465 7860 3a0a  using `bibtex`:.
-000025c0: 0a60 6060 6269 6274 6578 0a40 6d69 7363  .```bibtex.@misc
-000025d0: 7b66 6c3a 3a66 757a 7a79 6c69 7465 2c0a  {fl::fuzzylite,.
-000025e0: 2020 2020 6175 7468 6f72 3d7b 4a75 616e      author={Juan
-000025f0: 2052 6164 612d 5669 6c65 6c61 7d2c 0a20   Rada-Vilela},. 
-00002600: 2020 2074 6974 6c65 3d7b 5468 6520 4675     title={The Fu
-00002610: 7a7a 794c 6974 6520 4c69 6272 6172 6965  zzyLite Librarie
-00002620: 7320 666f 7220 4675 7a7a 7920 4c6f 6769  s for Fuzzy Logi
-00002630: 6320 436f 6e74 726f 6c7d 2c0a 2020 2020  c Control},.    
-00002640: 7572 6c3d 7b68 7474 7073 3a2f 2f66 757a  url={https://fuz
-00002650: 7a79 6c69 7465 2e63 6f6d 7d2c 0a20 2020  zylite.com},.   
-00002660: 2079 6561 723d 7b32 3031 387d 0a7d 0a60   year={2018}.}.`
-00002670: 6060 0a0a 2a2a 2a0a 0a66 757a 7a79 6c69  ``..***..fuzzyli
-00002680: 7465 2672 6567 3b20 6973 2061 2072 6567  te&reg; is a reg
-00002690: 6973 7465 7265 6420 7472 6164 656d 6172  istered trademar
-000026a0: 6b20 6f66 2046 757a 7a79 4c69 7465 204c  k of FuzzyLite L
-000026b0: 696d 6974 6564 203c 6272 3e0a 6a66 757a  imited <br>.jfuz
-000026c0: 7a79 6c69 7465 2674 7261 6465 3b20 6973  zylite&trade; is
-000026d0: 2061 2074 7261 6465 6d61 726b 206f 6620   a trademark of 
-000026e0: 4675 7a7a 794c 6974 6520 4c69 6d69 7465  FuzzyLite Limite
-000026f0: 6420 3c62 723e 0a70 7966 757a 7a79 6c69  d <br>.pyfuzzyli
-00002700: 7465 2674 7261 6465 3b20 6973 2061 2074  te&trade; is a t
-00002710: 7261 6465 6d61 726b 206f 6620 4675 7a7a  rademark of Fuzz
-00002720: 794c 6974 6520 4c69 6d69 7465 6420 3c62  yLite Limited <b
-00002730: 723e 0a51 7446 757a 7a79 4c69 7465 2674  r>.QtFuzzyLite&t
-00002740: 7261 6465 3b20 6973 2061 2074 7261 6465  rade; is a trade
-00002750: 6d61 726b 206f 6620 4675 7a7a 794c 6974  mark of FuzzyLit
-00002760: 6520 4c69 6d69 7465 6420 3c62 723e 0a0a  e Limited <br>..
+00000640: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
+00000650: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00000660: 7222 3e0a 3c69 6d67 2073 7263 3d22 2f66  r">.<img src="/f
+00000670: 757a 7a79 6c69 7465 2e70 6e67 2220 616c  uzzylite.png" al
+00000680: 743d 2266 757a 7a79 6c69 7465 2220 7769  t="fuzzylite" wi
+00000690: 6474 683d 2231 3025 223e 0a3c 6831 3e70  dth="10%">.<h1>p
+000006a0: 7966 757a 7a79 6c69 7465 2038 2e30 2e33  yfuzzylite 8.0.3
+000006b0: 3c2f 6831 3e0a 3c68 323e 4120 4675 7a7a  </h1>.<h2>A Fuzz
+000006c0: 7920 4c6f 6769 6320 436f 6e74 726f 6c20  y Logic Control 
+000006d0: 4c69 6272 6172 7920 696e 2050 7974 686f  Library in Pytho
+000006e0: 6e3c 2f68 323e 0a3c 6833 3e62 7920 3c61  n</h2>.<h3>by <a
+000006f0: 2068 7265 663d 2268 7474 7073 3a2f 2f66   href="https://f
+00000700: 757a 7a79 6c69 7465 2e63 6f6d 2f61 626f  uzzylite.com/abo
+00000710: 7574 223e 3c62 3e4a 7561 6e20 5261 6461  ut"><b>Juan Rada
+00000720: 2d56 696c 656c 612c 2050 6844 3c2f 623e  -Vilela, PhD</b>
+00000730: 3c2f 613e 3c2f 6833 3e0a 0a5b 215b 4c69  </a></h3>..[![Li
+00000740: 6365 6e73 653a 2047 504c 2076 335d 2868  cense: GPL v3](h
+00000750: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000760: 6473 2e69 6f2f 6261 6467 652f 4c69 6365  ds.io/badge/Lice
+00000770: 6e73 652d 4750 4c25 3230 7633 2d62 6c75  nse-GPL%20v3-blu
+00000780: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00000790: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+000007a0: 6963 656e 7365 2f67 706c 2d33 2d30 2f29  icense/gpl-3-0/)
+000007b0: 0a5b 215b 4c69 6365 6e73 653a 2050 6169  .[![License: Pai
+000007c0: 645d 2868 7474 7073 3a2f 2f69 6d67 2e73  d](https://img.s
+000007d0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000007e0: 4c69 6365 6e73 652d 7072 6f70 7269 6574  License-propriet
+000007f0: 6172 792d 626c 7565 295d 286d 6169 6c74  ary-blue)](mailt
+00000800: 6f3a 7361 6c65 7340 6675 7a7a 796c 6974  o:sales@fuzzylit
+00000810: 652e 636f 6d29 0a5b 215b 436f 7665 7261  e.com).[![Covera
+00000820: 6765 2053 7461 7475 735d 280a 6874 7470  ge Status](.http
+00000830: 733a 2f2f 636f 7665 7261 6c6c 732e 696f  s://coveralls.io
+00000840: 2f72 6570 6f73 2f67 6974 6875 622f 6675  /repos/github/fu
+00000850: 7a7a 796c 6974 652f 7079 6675 7a7a 796c  zzylite/pyfuzzyl
+00000860: 6974 652f 6261 6467 652e 7376 673f 6272  ite/badge.svg?br
+00000870: 616e 6368 3d6d 6169 6e29 5d28 0a68 7474  anch=main)](.htt
+00000880: 7073 3a2f 2f63 6f76 6572 616c 6c73 2e69  ps://coveralls.i
+00000890: 6f2f 6769 7468 7562 2f66 757a 7a79 6c69  o/github/fuzzyli
+000008a0: 7465 2f70 7966 757a 7a79 6c69 7465 3f62  te/pyfuzzylite?b
+000008b0: 7261 6e63 683d 6d61 696e 2920 200a 5b21  ranch=main)  .[!
+000008c0: 5b42 7569 6c64 5d28 6874 7470 733a 2f2f  [Build](https://
+000008d0: 6769 7468 7562 2e63 6f6d 2f66 757a 7a79  github.com/fuzzy
+000008e0: 6c69 7465 2f70 7966 757a 7a79 6c69 7465  lite/pyfuzzylite
+000008f0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000900: 7773 2f62 7569 6c64 2e79 6d6c 2f62 6164  ws/build.yml/bad
+00000910: 6765 2e73 7667 295d 280a 6874 7470 733a  ge.svg)](.https:
+00000920: 2f2f 6769 7468 7562 2e63 6f6d 2f66 757a  //github.com/fuz
+00000930: 7a79 6c69 7465 2f70 7966 757a 7a79 6c69  zylite/pyfuzzyli
+00000940: 7465 2f61 6374 696f 6e73 2f77 6f72 6b66  te/actions/workf
+00000950: 6c6f 7773 2f62 7569 6c64 2e79 6d6c 290a  lows/build.yml).
+00000960: 5b21 5b54 6573 745d 2868 7474 7073 3a2f  [![Test](https:/
+00000970: 2f67 6974 6875 622e 636f 6d2f 6675 7a7a  /github.com/fuzz
+00000980: 796c 6974 652f 7079 6675 7a7a 796c 6974  ylite/pyfuzzylit
+00000990: 652f 6163 7469 6f6e 732f 776f 726b 666c  e/actions/workfl
+000009a0: 6f77 732f 7465 7374 2e79 6d6c 2f62 6164  ows/test.yml/bad
+000009b0: 6765 2e73 7667 295d 280a 6874 7470 733a  ge.svg)](.https:
+000009c0: 2f2f 6769 7468 7562 2e63 6f6d 2f66 757a  //github.com/fuz
+000009d0: 7a79 6c69 7465 2f70 7966 757a 7a79 6c69  zylite/pyfuzzyli
+000009e0: 7465 2f61 6374 696f 6e73 2f77 6f72 6b66  te/actions/workf
+000009f0: 6c6f 7773 2f74 6573 742e 796d 6c29 0a5b  lows/test.yml).[
+00000a00: 215b 5075 626c 6973 685d 2868 7474 7073  ![Publish](https
+00000a10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6675  ://github.com/fu
+00000a20: 7a7a 796c 6974 652f 7079 6675 7a7a 796c  zzylite/pyfuzzyl
+00000a30: 6974 652f 6163 7469 6f6e 732f 776f 726b  ite/actions/work
+00000a40: 666c 6f77 732f 7075 626c 6973 682e 796d  flows/publish.ym
+00000a50: 6c2f 6261 6467 652e 7376 6729 5d28 0a68  l/badge.svg)](.h
+00000a60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000a70: 6d2f 6675 7a7a 796c 6974 652f 7079 6675  m/fuzzylite/pyfu
+00000a80: 7a7a 796c 6974 652f 6163 7469 6f6e 732f  zzylite/actions/
+00000a90: 776f 726b 666c 6f77 732f 7075 626c 6973  workflows/publis
+00000aa0: 682e 796d 6c29 0a0a 3c2f 6469 763e 0a0a  h.yml)..</div>..
+00000ab0: 2323 203c 6120 6e61 6d65 3d22 6675 7a7a  ## <a name="fuzz
+00000ac0: 796c 6974 6522 3e46 757a 7a79 4c69 7465  ylite">FuzzyLite
+00000ad0: 3c2f 613e 0a0a 2a2a 5468 6520 4675 7a7a  </a>..**The Fuzz
+00000ae0: 794c 6974 6520 4c69 6272 6172 6965 7320  yLite Libraries 
+00000af0: 666f 7220 4675 7a7a 7920 4c6f 6769 6320  for Fuzzy Logic 
+00000b00: 436f 6e74 726f 6c2a 2a20 7265 6665 7220  Control** refer 
+00000b10: 746f 205b 6066 757a 7a79 6c69 7465 605d  to [`fuzzylite`]
+00000b20: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000b30: 636f 6d2f 6675 7a7a 796c 6974 652f 6675  com/fuzzylite/fu
+00000b40: 7a7a 796c 6974 652f 290a 2843 2b2b 292c  zzylite/).(C++),
+00000b50: 205b 6070 7966 757a 7a79 6c69 7465 605d   [`pyfuzzylite`]
+00000b60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000b70: 636f 6d2f 6675 7a7a 796c 6974 652f 7079  com/fuzzylite/py
+00000b80: 6675 7a7a 796c 6974 652f 2920 2850 7974  fuzzylite/) (Pyt
+00000b90: 686f 6e29 2c0a 616e 6420 5b60 6a66 757a  hon),.and [`jfuz
+00000ba0: 7a79 6c69 7465 605d 2868 7474 7073 3a2f  zylite`](https:/
+00000bb0: 2f67 6974 6875 622e 636f 6d2f 6675 7a7a  /github.com/fuzz
+00000bc0: 796c 6974 652f 6a66 757a 7a79 6c69 7465  ylite/jfuzzylite
+00000bd0: 2f29 2028 4a61 7661 292e 0a0a 5468 6520  /) (Java)...The 
+00000be0: 2a2a 676f 616c 2a2a 206f 6620 7468 6520  **goal** of the 
+00000bf0: 4675 7a7a 794c 6974 6520 4c69 6272 6172  FuzzyLite Librar
+00000c00: 6965 7320 6973 2074 6f20 2a2a 6561 7369  ies is to **easi
+00000c10: 6c79 2a2a 2064 6573 6967 6e20 616e 6420  ly** design and 
+00000c20: 2a2a 6566 6669 6369 656e 746c 792a 2a20  **efficiently** 
+00000c30: 6f70 6572 6174 6520 6675 7a7a 7920 6c6f  operate fuzzy lo
+00000c40: 6769 6320 636f 6e74 726f 6c6c 6572 730a  gic controllers.
+00000c50: 666f 6c6c 6f77 696e 6720 616e 202a 2a6f  following an **o
+00000c60: 626a 6563 742d 6f72 6965 6e74 6564 2a2a  bject-oriented**
+00000c70: 2070 726f 6772 616d 6d69 6e67 206d 6f64   programming mod
+00000c80: 656c 2077 6974 6820 6d69 6e69 6d61 6c20  el with minimal 
+00000c90: 6465 7065 6e64 656e 6379 206f 6e20 6578  dependency on ex
+00000ca0: 7465 726e 616c 206c 6962 7261 7269 6573  ternal libraries
+00000cb0: 2e0a 0a23 2320 3c61 206e 616d 653d 226c  ...## <a name="l
+00000cc0: 6963 656e 7365 223e 4c69 6365 6e73 653c  icense">License<
+00000cd0: 2f61 3e0a 0a60 7079 6675 7a7a 796c 6974  /a>..`pyfuzzylit
+00000ce0: 6560 2069 7320 6475 616c 2d6c 6963 656e  e` is dual-licen
+00000cf0: 7365 6420 756e 6465 7220 7468 6520 5b2a  sed under the [*
+00000d00: 2a47 4e55 2047 504c 2033 2e30 2a2a 5d28  *GNU GPL 3.0**](
+00000d10: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00000d20: 6365 2e6f 7267 2f6c 6963 656e 7365 2f67  ce.org/license/g
+00000d30: 706c 2d33 2d30 2f29 2061 6e64 2075 6e64  pl-3-0/) and und
+00000d40: 6572 2061 0a2a 2a70 726f 7072 6965 7461  er a.**proprieta
+00000d50: 7279 206c 6963 656e 7365 2066 6f72 2063  ry license for c
+00000d60: 6f6d 6d65 7263 6961 6c20 7075 7270 6f73  ommercial purpos
+00000d70: 6573 2a2a 2e0a 0a59 6f75 2061 7265 202a  es**...You are *
+00000d80: 2a73 7472 6f6e 676c 792a 2a20 656e 636f  *strongly** enco
+00000d90: 7572 6167 6564 2074 6f20 7375 7070 6f72  uraged to suppor
+00000da0: 7420 7468 6520 6465 7665 6c6f 706d 656e  t the developmen
+00000db0: 7420 6f66 2074 6865 2046 757a 7a79 4c69  t of the FuzzyLi
+00000dc0: 7465 204c 6962 7261 7269 6573 2062 7920  te Libraries by 
+00000dd0: 7075 7263 6861 7369 6e67 2061 206c 6963  purchasing a lic
+00000de0: 656e 7365 0a6f 6620 5b60 5174 4675 7a7a  ense.of [`QtFuzz
+00000df0: 794c 6974 6560 5d28 6874 7470 733a 2f2f  yLite`](https://
+00000e00: 6675 7a7a 796c 6974 652e 636f 6d2f 646f  fuzzylite.com/do
+00000e10: 776e 6c6f 6164 7329 2e0a 0a5b 6051 7446  wnloads)...[`QtF
+00000e20: 757a 7a79 4c69 7465 605d 2868 7474 7073  uzzyLite`](https
+00000e30: 3a2f 2f66 757a 7a79 6c69 7465 2e63 6f6d  ://fuzzylite.com
+00000e40: 2f64 6f77 6e6c 6f61 6473 2f29 2069 7320  /downloads/) is 
+00000e50: 7468 6520 6265 7374 2067 7261 7068 6963  the best graphic
+00000e60: 616c 2075 7365 7220 696e 7465 7266 6163  al user interfac
+00000e70: 6520 6176 6169 6c61 626c 6520 746f 2065  e available to e
+00000e80: 6173 696c 7920 6465 7369 676e 2061 6e64  asily design and
+00000e90: 0a64 6972 6563 746c 7920 6f70 6572 6174  .directly operat
+00000ea0: 6520 6675 7a7a 7920 6c6f 6769 6320 636f  e fuzzy logic co
+00000eb0: 6e74 726f 6c6c 6572 7320 696e 2072 6561  ntrollers in rea
+00000ec0: 6c20 7469 6d65 2e20 4176 6169 6c61 626c  l time. Availabl
+00000ed0: 6520 666f 7220 5769 6e64 6f77 732c 204d  e for Windows, M
+00000ee0: 6163 2c20 616e 6420 4c69 6e75 782c 2069  ac, and Linux, i
+00000ef0: 7473 2067 6f61 6c20 6973 2074 6f0a 7369  ts goal is to.si
+00000f00: 676e 6966 6963 616e 746c 7920 2a2a 7370  gnificantly **sp
+00000f10: 6565 6420 7570 2a2a 2074 6865 2064 6573  eed up** the des
+00000f20: 6967 6e20 6f66 2079 6f75 7220 6675 7a7a  ign of your fuzz
+00000f30: 7920 6c6f 6769 6320 636f 6e74 726f 6c6c  y logic controll
+00000f40: 6572 732c 2077 6869 6c65 2070 726f 7669  ers, while provi
+00000f50: 6469 6e67 2061 2076 6572 7920 2a2a 7573  ding a very **us
+00000f60: 6566 756c 2a2a 2c20 2a2a 6675 6e63 7469  eful**, **functi
+00000f70: 6f6e 616c 2a2a 0a61 6e64 202a 2a62 6561  onal**.and **bea
+00000f80: 7574 6966 756c 2a2a 2075 7365 7220 696e  utiful** user in
+00000f90: 7465 7266 6163 652e 0a50 6c65 6173 652c  terface..Please,
+00000fa0: 2064 6f77 6e6c 6f61 6420 6974 2061 6e64   download it and
+00000fb0: 2063 6865 636b 2069 7420 6f75 7420 666f   check it out fo
+00000fc0: 7220 6672 6565 2061 7420 5b66 757a 7a79  r free at [fuzzy
+00000fd0: 6c69 7465 2e63 6f6d 2f64 6f77 6e6c 6f61  lite.com/downloa
+00000fe0: 6473 5d28 6874 7470 733a 2f2f 6675 7a7a  ds](https://fuzz
+00000ff0: 796c 6974 652e 636f 6d2f 646f 776e 6c6f  ylite.com/downlo
+00001000: 6164 7329 2e0a 0a23 2320 3c61 206e 616d  ads)...## <a nam
+00001010: 653d 2269 6e73 7461 6c6c 223e 496e 7374  e="install">Inst
+00001020: 616c 6c3c 2f61 3e0a 0a60 6060 636f 6d6d  all</a>..```comm
+00001030: 616e 646c 696e 650a 7069 7020 696e 7374  andline.pip inst
+00001040: 616c 6c20 7079 6675 7a7a 796c 6974 650a  all pyfuzzylite.
+00001050: 6060 600a 0a23 2320 3c61 206e 616d 653d  ```..## <a name=
+00001060: 2266 6561 7475 7265 7322 3e46 6561 7475  "features">Featu
+00001070: 7265 733c 2f61 3e0a 0a2a 2a44 6f63 756d  res</a>..**Docum
+00001080: 656e 7461 7469 6f6e 2a2a 3a20 5b66 757a  entation**: [fuz
+00001090: 7a79 6c69 7465 2e67 6974 6875 622e 696f  zylite.github.io
+000010a0: 2f70 7966 757a 7a79 6c69 7465 2f5d 2868  /pyfuzzylite/](h
+000010b0: 7474 7073 3a2f 2f66 757a 7a79 6c69 7465  ttps://fuzzylite
+000010c0: 2e67 6974 6875 622e 696f 2f70 7966 757a  .github.io/pyfuz
+000010d0: 7a79 6c69 7465 2f29 0a0a 2a2a 2836 2920  zylite/)..**(6) 
+000010e0: 436f 6e74 726f 6c6c 6572 732a 2a3a 204d  Controllers**: M
+000010f0: 616d 6461 6e69 2c20 5461 6b61 6769 2d53  amdani, Takagi-S
+00001100: 7567 656e 6f2c 204c 6172 7365 6e2c 2054  ugeno, Larsen, T
+00001110: 7375 6b61 6d6f 746f 2c20 496e 7665 7273  sukamoto, Invers
+00001120: 6520 5473 756b 616d 6f74 6f2c 2048 7962  e Tsukamoto, Hyb
+00001130: 7269 640a 0a2a 2a28 3235 2920 4c69 6e67  rid..**(25) Ling
+00001140: 7569 7374 6963 2074 6572 6d73 2a2a 3a20  uistic terms**: 
+00001150: 2028 3529 202a 4261 7369 632a 3a20 5472   (5) *Basic*: Tr
+00001160: 6961 6e67 6c65 2c20 5472 6170 657a 6f69  iangle, Trapezoi
+00001170: 642c 2052 6563 7461 6e67 6c65 2c20 4469  d, Rectangle, Di
+00001180: 7363 7265 7465 2c20 5365 6d69 456c 6c69  screte, SemiElli
+00001190: 7073 652e 0a28 3829 202a 4578 7465 6e64  pse..(8) *Extend
+000011a0: 6564 2a3a 2042 656c 6c2c 2043 6f73 696e  ed*: Bell, Cosin
+000011b0: 652c 2047 6175 7373 6961 6e2c 2047 6175  e, Gaussian, Gau
+000011c0: 7373 6961 6e50 726f 6475 6374 2c20 5069  ssianProduct, Pi
+000011d0: 5368 6170 652c 2053 6967 6d6f 6964 4469  Shape, SigmoidDi
+000011e0: 6666 6572 656e 6365 2c20 5369 676d 6f69  fference, Sigmoi
+000011f0: 6450 726f 6475 6374 2c20 5370 696b 652e  dProduct, Spike.
+00001200: 0a28 3729 202a 4564 6765 732a 3a20 4172  .(7) *Edges*: Ar
+00001210: 632c 2042 696e 6172 792c 2043 6f6e 6361  c, Binary, Conca
+00001220: 7665 2c20 5261 6d70 2c20 5369 676d 6f69  ve, Ramp, Sigmoi
+00001230: 642c 2053 5368 6170 652c 205a 5368 6170  d, SShape, ZShap
+00001240: 652e 0a28 3329 202a 4675 6e63 7469 6f6e  e..(3) *Function
+00001250: 732a 3a20 436f 6e73 7461 6e74 2c20 4c69  s*: Constant, Li
+00001260: 6e65 6172 2c20 4675 6e63 7469 6f6e 2e20  near, Function. 
+00001270: 2832 2920 2a53 7065 6369 616c 2a3a 2041  (2) *Special*: A
+00001280: 6767 7265 6761 7465 642c 2041 6374 6976  ggregated, Activ
+00001290: 6174 6564 2e0a 0a2a 2a28 3729 2041 6374  ated...**(7) Act
+000012a0: 6976 6174 696f 6e20 6d65 7468 6f64 732a  ivation methods*
+000012b0: 2a3a 2020 4765 6e65 7261 6c2c 2050 726f  *:  General, Pro
+000012c0: 706f 7274 696f 6e61 6c2c 2054 6872 6573  portional, Thres
+000012d0: 686f 6c64 2c20 4669 7273 742c 204c 6173  hold, First, Las
+000012e0: 742c 204c 6f77 6573 742c 2048 6967 6865  t, Lowest, Highe
+000012f0: 7374 2e0a 0a2a 2a28 3929 2043 6f6e 6a75  st...**(9) Conju
+00001300: 6e63 7469 6f6e 2061 6e64 2049 6d70 6c69  nction and Impli
+00001310: 6361 7469 6f6e 2028 542d 4e6f 726d 7329  cation (T-Norms)
+00001320: 2a2a 3a20 4d69 6e69 6d75 6d2c 2041 6c67  **: Minimum, Alg
+00001330: 6562 7261 6963 5072 6f64 7563 742c 2042  ebraicProduct, B
+00001340: 6f75 6e64 6564 4469 6666 6572 656e 6365  oundedDifference
+00001350: 2c20 4472 6173 7469 6350 726f 6475 6374  , DrasticProduct
+00001360: 2c0a 4569 6e73 7465 696e 5072 6f64 7563  ,.EinsteinProduc
+00001370: 742c 2048 616d 6163 6865 7250 726f 6475  t, HamacherProdu
+00001380: 6374 2c20 4e69 6c70 6f74 656e 744d 696e  ct, NilpotentMin
+00001390: 696d 756d 2c20 4c61 6d62 6461 4e6f 726d  imum, LambdaNorm
+000013a0: 2c20 4675 6e63 7469 6f6e 4e6f 726d 2e0a  , FunctionNorm..
+000013b0: 0a2a 2a28 3131 2920 4469 736a 756e 6374  .**(11) Disjunct
+000013c0: 696f 6e20 616e 6420 4167 6772 6567 6174  ion and Aggregat
+000013d0: 696f 6e20 2853 2d4e 6f72 6d73 292a 2a3a  ion (S-Norms)**:
+000013e0: 2020 4d61 7869 6d75 6d2c 2041 6c67 6562    Maximum, Algeb
+000013f0: 7261 6963 5375 6d2c 2042 6f75 6e64 6564  raicSum, Bounded
+00001400: 5375 6d2c 2044 7261 7374 6963 5375 6d2c  Sum, DrasticSum,
+00001410: 2045 696e 7374 6569 6e53 756d 2c0a 4861   EinsteinSum,.Ha
+00001420: 6d61 6368 6572 5375 6d2c 204e 696c 706f  macherSum, Nilpo
+00001430: 7465 6e74 4d61 7869 6d75 6d2c 204e 6f72  tentMaximum, Nor
+00001440: 6d61 6c69 7a65 6453 756d 2c20 556e 626f  malizedSum, Unbo
+00001450: 756e 6465 6453 756d 2c20 4c61 6d62 6461  undedSum, Lambda
+00001460: 4e6f 726d 2c20 4675 6e63 7469 6f6e 4e6f  Norm, FunctionNo
+00001470: 726d 2e0a 0a2a 2a28 3729 2044 6566 757a  rm...**(7) Defuz
+00001480: 7a69 6669 6572 732a 2a3a 2020 2835 2920  zifiers**:  (5) 
+00001490: 2a49 6e74 6567 7261 6c2a 3a20 4365 6e74  *Integral*: Cent
+000014a0: 726f 6964 2c20 4269 7365 6374 6f72 2c20  roid, Bisector, 
+000014b0: 536d 616c 6c65 7374 4f66 4d61 7869 6d75  SmallestOfMaximu
+000014c0: 6d2c 204c 6172 6765 7374 4f66 4d61 7869  m, LargestOfMaxi
+000014d0: 6d75 6d2c 204d 6561 6e4f 664d 6178 696d  mum, MeanOfMaxim
+000014e0: 756d 2e0a 2832 2920 2a57 6569 6768 7465  um..(2) *Weighte
+000014f0: 642a 3a20 5765 6967 6874 6564 4176 6572  d*: WeightedAver
+00001500: 6167 652c 2057 6569 6768 7465 6453 756d  age, WeightedSum
+00001510: 2e0a 0a2a 2a28 3729 2048 6564 6765 732a  ...**(7) Hedges*
+00001520: 2a3a 2041 6e79 2c20 4e6f 742c 2045 7874  *: Any, Not, Ext
+00001530: 7265 6d65 6c79 2c20 5365 6c64 6f6d 2c20  remely, Seldom, 
+00001540: 536f 6d65 7768 6174 2c20 5665 7279 2c20  Somewhat, Very, 
+00001550: 4675 6e63 7469 6f6e 2e0a 0a2a 2a28 3329  Function...**(3)
+00001560: 2049 6d70 6f72 7465 7273 2a2a 3a20 4675   Importers**: Fu
+00001570: 7a7a 794c 6974 6520 4c61 6e67 7561 6765  zzyLite Language
+00001580: 2060 666c 6c60 2e20 5769 7468 2060 6675   `fll`. With `fu
+00001590: 7a7a 796c 6974 6560 3a20 4675 7a7a 7920  zzylite`: Fuzzy 
+000015a0: 496e 6665 7265 6e63 6520 5379 7374 656d  Inference System
+000015b0: 2060 6669 7360 2c20 4675 7a7a 7920 436f   `fis`, Fuzzy Co
+000015c0: 6e74 726f 6c0a 4c61 6e67 7561 6765 2060  ntrol.Language `
+000015d0: 6663 6c60 2e0a 0a2a 2a28 3729 2045 7870  fcl`...**(7) Exp
+000015e0: 6f72 7465 7273 2a2a 3a20 6050 7974 686f  orters**: `Pytho
+000015f0: 6e60 2c20 4675 7a7a 794c 6974 6520 4c61  n`, FuzzyLite La
+00001600: 6e67 7561 6765 2060 666c 6c60 2c20 4675  nguage `fll`, Fu
+00001610: 7a7a 794c 6974 6520 4461 7461 7365 7420  zzyLite Dataset 
+00001620: 6066 6c64 602e 2057 6974 6820 6066 757a  `fld`. With `fuz
+00001630: 7a79 6c69 7465 603a 2060 432b 2b60 2c20  zylite`: `C++`, 
+00001640: 604a 6176 6160 2c0a 4675 7a7a 794c 6974  `Java`,.FuzzyLit
+00001650: 6520 4c61 6e67 7561 6765 2060 666c 6c60  e Language `fll`
+00001660: 2c20 4675 7a7a 794c 6974 6520 4461 7461  , FuzzyLite Data
+00001670: 7365 7420 6066 6c64 602c 2060 5260 2073  set `fld`, `R` s
+00001680: 6372 6970 742c 2046 757a 7a79 2049 6e66  cript, Fuzzy Inf
+00001690: 6572 656e 6365 2053 7973 7465 6d20 6066  erence System `f
+000016a0: 6973 602c 2046 757a 7a79 2043 6f6e 7472  is`, Fuzzy Contr
+000016b0: 6f6c 0a4c 616e 6775 6167 6520 6066 636c  ol.Language `fcl
+000016c0: 602e 0a0a 2a2a 2833 302b 2920 4578 616d  `...**(30+) Exam
+000016d0: 706c 6573 2a2a 2020 6f66 204d 616d 6461  ples**  of Mamda
+000016e0: 6e69 2c20 5461 6b61 6769 2d53 7567 656e  ni, Takagi-Sugen
+000016f0: 6f2c 2054 7375 6b61 6d6f 746f 2c20 616e  o, Tsukamoto, an
+00001700: 6420 4879 6272 6964 2063 6f6e 7472 6f6c  d Hybrid control
+00001710: 6c65 7273 2066 726f 6d20 6066 757a 7a79  lers from `fuzzy
+00001720: 6c69 7465 602c 204f 6374 6176 652c 2061  lite`, Octave, a
+00001730: 6e64 204d 6174 6c61 622c 0a65 6163 6820  nd Matlab,.each 
+00001740: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
+00001750: 666f 6c6c 6f77 696e 6720 666f 726d 6174  following format
+00001760: 733a 2060 7079 602c 2060 666c 6c60 2c20  s: `py`, `fll`, 
+00001770: 6066 6c64 602e 2057 6974 6820 6066 757a  `fld`. With `fuz
+00001780: 7a79 6c69 7465 603a 2060 432b 2b60 2c20  zylite`: `C++`, 
+00001790: 604a 6176 6160 2c20 6052 602c 2060 6669  `Java`, `R`, `fi
+000017a0: 7360 2c20 616e 6420 6066 636c 602e 0a0a  s`, and `fcl`...
+000017b0: 2323 203c 6120 6e61 6d65 3d22 6578 616d  ## <a name="exam
+000017c0: 706c 6573 223e 4578 616d 706c 6573 3c2f  ples">Examples</
+000017d0: 613e 0a0a 2323 2320 4675 7a7a 794c 6974  a>..### FuzzyLit
+000017e0: 6520 4c61 6e67 7561 6765 0a0a 6060 6079  e Language..```y
+000017f0: 616d 6c0a 2320 4669 6c65 3a20 6578 616d  aml.# File: exam
+00001800: 706c 6573 2f6d 616d 6461 6e69 2f4f 6273  ples/mamdani/Obs
+00001810: 7461 636c 6541 766f 6964 616e 6365 2e66  tacleAvoidance.f
+00001820: 6c6c 0a45 6e67 696e 653a 204f 6273 7461  ll.Engine: Obsta
+00001830: 636c 6541 766f 6964 616e 6365 0a49 6e70  cleAvoidance.Inp
+00001840: 7574 5661 7269 6162 6c65 3a20 6f62 7374  utVariable: obst
+00001850: 6163 6c65 0a20 2065 6e61 626c 6564 3a20  acle.  enabled: 
+00001860: 7472 7565 0a20 2072 616e 6765 3a20 302e  true.  range: 0.
+00001870: 3030 3020 312e 3030 300a 2020 6c6f 636b  000 1.000.  lock
+00001880: 2d72 616e 6765 3a20 6661 6c73 650a 2020  -range: false.  
+00001890: 7465 726d 3a20 6c65 6674 2052 616d 7020  term: left Ramp 
+000018a0: 312e 3030 3020 302e 3030 300a 2020 7465  1.000 0.000.  te
+000018b0: 726d 3a20 7269 6768 7420 5261 6d70 2030  rm: right Ramp 0
+000018c0: 2e30 3030 2031 2e30 3030 0a4f 7574 7075  .000 1.000.Outpu
+000018d0: 7456 6172 6961 626c 653a 206d 5374 6565  tVariable: mStee
+000018e0: 720a 2020 656e 6162 6c65 643a 2074 7275  r.  enabled: tru
+000018f0: 650a 2020 7261 6e67 653a 2030 2e30 3030  e.  range: 0.000
+00001900: 2031 2e30 3030 0a20 206c 6f63 6b2d 7261   1.000.  lock-ra
+00001910: 6e67 653a 2066 616c 7365 0a20 2061 6767  nge: false.  agg
+00001920: 7265 6761 7469 6f6e 3a20 4d61 7869 6d75  regation: Maximu
+00001930: 6d0a 2020 6465 6675 7a7a 6966 6965 723a  m.  defuzzifier:
+00001940: 2043 656e 7472 6f69 6420 3130 300a 2020   Centroid 100.  
+00001950: 6465 6661 756c 743a 206e 616e 0a20 206c  default: nan.  l
+00001960: 6f63 6b2d 7072 6576 696f 7573 3a20 6661  ock-previous: fa
+00001970: 6c73 650a 2020 7465 726d 3a20 6c65 6674  lse.  term: left
+00001980: 2052 616d 7020 312e 3030 3020 302e 3030   Ramp 1.000 0.00
+00001990: 300a 2020 7465 726d 3a20 7269 6768 7420  0.  term: right 
+000019a0: 5261 6d70 2030 2e30 3030 2031 2e30 3030  Ramp 0.000 1.000
+000019b0: 0a52 756c 6542 6c6f 636b 3a20 6d61 6d64  .RuleBlock: mamd
+000019c0: 616e 690a 2020 656e 6162 6c65 643a 2074  ani.  enabled: t
+000019d0: 7275 650a 2020 636f 6e6a 756e 6374 696f  rue.  conjunctio
+000019e0: 6e3a 206e 6f6e 650a 2020 6469 736a 756e  n: none.  disjun
+000019f0: 6374 696f 6e3a 206e 6f6e 650a 2020 696d  ction: none.  im
+00001a00: 706c 6963 6174 696f 6e3a 2041 6c67 6562  plication: Algeb
+00001a10: 7261 6963 5072 6f64 7563 740a 2020 6163  raicProduct.  ac
+00001a20: 7469 7661 7469 6f6e 3a20 4765 6e65 7261  tivation: Genera
+00001a30: 6c0a 2020 7275 6c65 3a20 6966 206f 6273  l.  rule: if obs
+00001a40: 7461 636c 6520 6973 206c 6566 7420 7468  tacle is left th
+00001a50: 656e 206d 5374 6565 7220 6973 2072 6967  en mSteer is rig
+00001a60: 6874 0a20 2072 756c 653a 2069 6620 6f62  ht.  rule: if ob
+00001a70: 7374 6163 6c65 2069 7320 7269 6768 7420  stacle is right 
+00001a80: 7468 656e 206d 5374 6565 7220 6973 206c  then mSteer is l
+00001a90: 6566 740a 6060 600a 0a60 6060 7079 7468  eft.```..```pyth
+00001aa0: 6f6e 0a23 2050 7974 686f 6e0a 696d 706f  on.# Python.impo
+00001ab0: 7274 2066 757a 7a79 6c69 7465 2061 7320  rt fuzzylite as 
+00001ac0: 666c 0a0a 656e 6769 6e65 203d 2066 6c2e  fl..engine = fl.
+00001ad0: 466c 6c49 6d70 6f72 7465 7228 292e 6672  FllImporter().fr
+00001ae0: 6f6d 5f66 696c 6528 2265 7861 6d70 6c65  om_file("example
+00001af0: 732f 6d61 6d64 616e 692f 4f62 7374 6163  s/mamdani/Obstac
+00001b00: 6c65 4176 6f69 6461 6e63 652e 666c 6c22  leAvoidance.fll"
+00001b10: 290a 6060 600a 0a23 2323 2050 7974 686f  ).```..### Pytho
+00001b20: 6e0a 0a60 6060 7079 7468 6f6e 0a69 6d70  n..```python.imp
+00001b30: 6f72 7420 6675 7a7a 796c 6974 6520 6173  ort fuzzylite as
+00001b40: 2066 6c0a 0a65 6e67 696e 6520 3d20 666c   fl..engine = fl
+00001b50: 2e45 6e67 696e 6528 0a20 2020 206e 616d  .Engine(.    nam
+00001b60: 653d 224f 6273 7461 636c 6541 766f 6964  e="ObstacleAvoid
+00001b70: 616e 6365 222c 0a20 2020 2069 6e70 7574  ance",.    input
+00001b80: 5f76 6172 6961 626c 6573 3d5b 0a20 2020  _variables=[.   
+00001b90: 2020 2020 2066 6c2e 496e 7075 7456 6172       fl.InputVar
+00001ba0: 6961 626c 6528 0a20 2020 2020 2020 2020  iable(.         
+00001bb0: 2020 206e 616d 653d 226f 6273 7461 636c     name="obstacl
+00001bc0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00001bd0: 6d69 6e69 6d75 6d3d 302e 302c 0a20 2020  minimum=0.0,.   
+00001be0: 2020 2020 2020 2020 206d 6178 696d 756d           maximum
+00001bf0: 3d31 2e30 2c0a 2020 2020 2020 2020 2020  =1.0,.          
+00001c00: 2020 6c6f 636b 5f72 616e 6765 3d46 616c    lock_range=Fal
+00001c10: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00001c20: 7465 726d 733d 5b66 6c2e 5261 6d70 2822  terms=[fl.Ramp("
+00001c30: 6c65 6674 222c 2031 2e30 2c20 302e 3029  left", 1.0, 0.0)
+00001c40: 2c20 666c 2e52 616d 7028 2272 6967 6874  , fl.Ramp("right
+00001c50: 222c 2030 2e30 2c20 312e 3029 5d2c 0a20  ", 0.0, 1.0)],. 
+00001c60: 2020 2020 2020 2029 0a20 2020 205d 2c0a         ).    ],.
+00001c70: 2020 2020 6f75 7470 7574 5f76 6172 6961      output_varia
+00001c80: 626c 6573 3d5b 0a20 2020 2020 2020 2066  bles=[.        f
+00001c90: 6c2e 4f75 7470 7574 5661 7269 6162 6c65  l.OutputVariable
+00001ca0: 280a 2020 2020 2020 2020 2020 2020 6e61  (.            na
+00001cb0: 6d65 3d22 6d53 7465 6572 222c 0a20 2020  me="mSteer",.   
+00001cc0: 2020 2020 2020 2020 206d 696e 696d 756d           minimum
+00001cd0: 3d30 2e30 2c0a 2020 2020 2020 2020 2020  =0.0,.          
+00001ce0: 2020 6d61 7869 6d75 6d3d 312e 302c 0a20    maximum=1.0,. 
+00001cf0: 2020 2020 2020 2020 2020 206c 6f63 6b5f             lock_
+00001d00: 7261 6e67 653d 4661 6c73 652c 0a20 2020  range=False,.   
+00001d10: 2020 2020 2020 2020 206c 6f63 6b5f 7072           lock_pr
+00001d20: 6576 696f 7573 3d46 616c 7365 2c0a 2020  evious=False,.  
+00001d30: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
+00001d40: 745f 7661 6c75 653d 666c 2e6e 616e 2c0a  t_value=fl.nan,.
+00001d50: 2020 2020 2020 2020 2020 2020 6167 6772              aggr
+00001d60: 6567 6174 696f 6e3d 666c 2e4d 6178 696d  egation=fl.Maxim
+00001d70: 756d 2829 2c0a 2020 2020 2020 2020 2020  um(),.          
+00001d80: 2020 6465 6675 7a7a 6966 6965 723d 666c    defuzzifier=fl
+00001d90: 2e43 656e 7472 6f69 6428 7265 736f 6c75  .Centroid(resolu
+00001da0: 7469 6f6e 3d31 3030 292c 0a20 2020 2020  tion=100),.     
+00001db0: 2020 2020 2020 2074 6572 6d73 3d5b 666c         terms=[fl
+00001dc0: 2e52 616d 7028 226c 6566 7422 2c20 312e  .Ramp("left", 1.
+00001dd0: 302c 2030 2e30 292c 2066 6c2e 5261 6d70  0, 0.0), fl.Ramp
+00001de0: 2822 7269 6768 7422 2c20 302e 302c 2031  ("right", 0.0, 1
+00001df0: 2e30 295d 2c0a 2020 2020 2020 2020 290a  .0)],.        ).
+00001e00: 2020 2020 5d2c 0a20 2020 2072 756c 655f      ],.    rule_
+00001e10: 626c 6f63 6b73 3d5b 0a20 2020 2020 2020  blocks=[.       
+00001e20: 2066 6c2e 5275 6c65 426c 6f63 6b28 0a20   fl.RuleBlock(. 
+00001e30: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+00001e40: 226d 616d 6461 6e69 222c 0a20 2020 2020  "mamdani",.     
+00001e50: 2020 2020 2020 2063 6f6e 6a75 6e63 7469         conjuncti
+00001e60: 6f6e 3d4e 6f6e 652c 0a20 2020 2020 2020  on=None,.       
+00001e70: 2020 2020 2064 6973 6a75 6e63 7469 6f6e       disjunction
+00001e80: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00001e90: 2020 2069 6d70 6c69 6361 7469 6f6e 3d66     implication=f
+00001ea0: 6c2e 416c 6765 6272 6169 6350 726f 6475  l.AlgebraicProdu
+00001eb0: 6374 2829 2c0a 2020 2020 2020 2020 2020  ct(),.          
+00001ec0: 2020 6163 7469 7661 7469 6f6e 3d66 6c2e    activation=fl.
+00001ed0: 4765 6e65 7261 6c28 292c 0a20 2020 2020  General(),.     
+00001ee0: 2020 2020 2020 2072 756c 6573 3d5b 0a20         rules=[. 
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00001f00: 6c2e 5275 6c65 2e63 7265 6174 6528 2269  l.Rule.create("i
+00001f10: 6620 6f62 7374 6163 6c65 2069 7320 6c65  f obstacle is le
+00001f20: 6674 2074 6865 6e20 6d53 7465 6572 2069  ft then mSteer i
+00001f30: 7320 7269 6768 7422 292c 0a20 2020 2020  s right"),.     
+00001f40: 2020 2020 2020 2020 2020 2066 6c2e 5275             fl.Ru
+00001f50: 6c65 2e63 7265 6174 6528 2269 6620 6f62  le.create("if ob
+00001f60: 7374 6163 6c65 2069 7320 7269 6768 7420  stacle is right 
+00001f70: 7468 656e 206d 5374 6565 7220 6973 206c  then mSteer is l
+00001f80: 6566 7422 292c 0a20 2020 2020 2020 2020  eft"),.         
+00001f90: 2020 205d 2c0a 2020 2020 2020 2020 290a     ],.        ).
+00001fa0: 2020 2020 5d2c 0a29 0a60 6060 0a0a 2323      ],.).```..##
+00001fb0: 2320 6066 6c6f 6174 6020 616e 6420 7665  # `float` and ve
+00001fc0: 6374 6f72 697a 6174 696f 6e0a 0a60 6060  ctorization..```
+00001fd0: 7079 7468 6f6e 0a23 2073 696e 676c 6520  python.# single 
+00001fe0: 6066 6c6f 6174 6020 6f70 6572 6174 696f  `float` operatio
+00001ff0: 6e0a 656e 6769 6e65 2e69 6e70 7574 5f76  n.engine.input_v
+00002000: 6172 6961 626c 6528 226f 6273 7461 636c  ariable("obstacl
+00002010: 6522 292e 7661 6c75 6520 3d20 302e 350a  e").value = 0.5.
+00002020: 656e 6769 6e65 2e70 726f 6365 7373 2829  engine.process()
+00002030: 0a70 7269 6e74 2822 7920 3d22 2c20 656e  .print("y =", en
+00002040: 6769 6e65 2e6f 7574 7075 745f 7661 7269  gine.output_vari
+00002050: 6162 6c65 2822 6d53 7465 6572 2229 2e76  able("mSteer").v
+00002060: 616c 7565 290a 2320 3e20 7920 3d20 302e  alue).# > y = 0.
+00002070: 350a 7072 696e 7428 22e1 bbb9 203d 222c  5.print("... =",
+00002080: 2065 6e67 696e 652e 6f75 7470 7574 5f76   engine.output_v
+00002090: 6172 6961 626c 6528 226d 5374 6565 7222  ariable("mSteer"
+000020a0: 292e 6675 7a7a 795f 7661 6c75 6528 2929  ).fuzzy_value())
+000020b0: 0a23 203e 20e1 bbb9 203d 2030 2e35 3030  .# > ... = 0.500
+000020c0: 2f6c 6566 7420 2b20 302e 3530 302f 7269  /left + 0.500/ri
+000020d0: 6768 740a 0a23 2076 6563 746f 7269 7a61  ght..# vectoriza
+000020e0: 7469 6f6e 0a65 6e67 696e 652e 696e 7075  tion.engine.inpu
+000020f0: 745f 7661 7269 6162 6c65 2822 6f62 7374  t_variable("obst
+00002100: 6163 6c65 2229 2e76 616c 7565 203d 2066  acle").value = f
+00002110: 6c2e 6172 7261 7928 5b30 2c20 302e 3235  l.array([0, 0.25
+00002120: 2c20 302e 352c 2030 2e37 352c 2031 2e30  , 0.5, 0.75, 1.0
+00002130: 5d29 0a65 6e67 696e 652e 7072 6f63 6573  ]).engine.proces
+00002140: 7328 290a 7072 696e 7428 2279 203d 222c  s().print("y =",
+00002150: 2072 6570 7228 656e 6769 6e65 2e6f 7574   repr(engine.out
+00002160: 7075 745f 7661 7269 6162 6c65 2822 6d53  put_variable("mS
+00002170: 7465 6572 2229 2e76 616c 7565 2929 0a23  teer").value)).#
+00002180: 203e 2079 203d 2061 7272 6179 285b 302e   > y = array([0.
+00002190: 3636 3636 3636 3520 2c20 302e 3632 3137  6666665 , 0.6217
+000021a0: 3934 3737 2c20 302e 3520 2020 2020 2020  9477, 0.5       
+000021b0: 2c20 302e 3337 3832 3035 3233 2c20 302e  , 0.37820523, 0.
+000021c0: 3333 3333 3333 3520 5d29 0a70 7269 6e74  3333335 ]).print
+000021d0: 2822 e1bb b920 3d22 2c20 7265 7072 2865  ("... =", repr(e
+000021e0: 6e67 696e 652e 6f75 7470 7574 5f76 6172  ngine.output_var
+000021f0: 6961 626c 6528 226d 5374 6565 7222 292e  iable("mSteer").
+00002200: 6675 7a7a 795f 7661 6c75 6528 2929 290a  fuzzy_value())).
+00002210: 2320 3e20 e1bb b920 3d20 6172 7261 7928  # > ... = array(
+00002220: 5b27 302e 3030 302f 6c65 6674 202b 2031  ['0.000/left + 1
+00002230: 2e30 3030 2f72 6967 6874 272c 0a23 2020  .000/right',.#  
+00002240: 2020 2020 2020 2020 2020 2020 2730 2e32              '0.2
+00002250: 3530 2f6c 6566 7420 2b20 302e 3735 302f  50/left + 0.750/
+00002260: 7269 6768 7427 2c0a 2320 2020 2020 2020  right',.#       
+00002270: 2020 2020 2020 2027 302e 3530 302f 6c65         '0.500/le
+00002280: 6674 202b 2030 2e35 3030 2f72 6967 6874  ft + 0.500/right
+00002290: 272c 0a23 2020 2020 2020 2020 2020 2020  ',.#            
+000022a0: 2020 2730 2e37 3530 2f6c 6566 7420 2b20    '0.750/left + 
+000022b0: 302e 3235 302f 7269 6768 7427 2c0a 2320  0.250/right',.# 
+000022c0: 2020 2020 2020 2020 2020 2020 2027 312e               '1.
+000022d0: 3030 302f 6c65 6674 202b 2030 2e30 3030  000/left + 0.000
+000022e0: 2f72 6967 6874 275d 2c20 6474 7970 653d  /right'], dtype=
+000022f0: 273c 5532 3627 290a 6060 600a 0a50 6c65  '<U26').```..Ple
+00002300: 6173 6520 7265 6665 7220 746f 2074 6865  ase refer to the
+00002310: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
+00002320: 6f72 206d 6f72 650a 696e 666f 726d 6174  or more.informat
+00002330: 696f 6e3a 205b 2a2a 6675 7a7a 796c 6974  ion: [**fuzzylit
+00002340: 652e 6769 7468 7562 2e69 6f2f 7079 6675  e.github.io/pyfu
+00002350: 7a7a 796c 6974 652f 2a2a 5d28 6874 7470  zzylite/**](http
+00002360: 733a 2f2f 6675 7a7a 796c 6974 652e 6769  s://fuzzylite.gi
+00002370: 7468 7562 2e69 6f2f 7079 6675 7a7a 796c  thub.io/pyfuzzyl
+00002380: 6974 652f 290a 0a23 2320 3c61 206e 616d  ite/)..## <a nam
+00002390: 653d 2263 6f6e 7472 6962 7574 696e 6722  e="contributing"
+000023a0: 3e43 6f6e 7472 6962 7574 696e 673c 2f61  >Contributing</a
+000023b0: 3e0a 0a41 6c6c 2063 6f6e 7472 6962 7574  >..All contribut
+000023c0: 696f 6e73 2061 7265 2077 656c 636f 6d65  ions are welcome
+000023d0: 2c20 7072 6f76 6964 6564 2074 6865 7920  , provided they 
+000023e0: 666f 6c6c 6f77 2074 6865 2066 6f6c 6c6f  follow the follo
+000023f0: 7769 6e67 2067 7569 6465 6c69 6e65 733a  wing guidelines:
+00002400: 0a0a 2d20 536f 7572 6365 2063 6f64 6520  ..- Source code 
+00002410: 6973 2063 6f6e 7369 7374 656e 7420 7769  is consistent wi
+00002420: 7468 2073 7461 6e64 6172 6473 2069 6e20  th standards in 
+00002430: 7468 6520 6c69 6272 6172 790a 2d20 436f  the library.- Co
+00002440: 6e74 7269 6275 7469 6f6e 2069 7320 7072  ntribution is pr
+00002450: 6f70 6572 6c79 2064 6f63 756d 656e 7465  operly documente
+00002460: 6420 616e 6420 7465 7374 6564 2c20 7261  d and tested, ra
+00002470: 6973 696e 6720 6973 7375 6573 2077 6865  ising issues whe
+00002480: 7265 2061 7070 726f 7072 6961 7465 0a2d  re appropriate.-
+00002490: 2043 6f6e 7472 6962 7574 696f 6e20 6973   Contribution is
+000024a0: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+000024b0: 7468 6520 4675 7a7a 794c 6974 6520 4c69  the FuzzyLite Li
+000024c0: 6365 6e73 650a 0a23 2320 3c61 206e 616d  cense..## <a nam
+000024d0: 653d 2272 6566 6572 656e 6365 223e 5265  e="reference">Re
+000024e0: 6665 7265 6e63 653c 2f61 3e0a 0a49 6620  ference</a>..If 
+000024f0: 796f 7520 6172 6520 7573 696e 6720 7468  you are using th
+00002500: 6520 4675 7a7a 794c 6974 6520 4c69 6272  e FuzzyLite Libr
+00002510: 6172 6965 732c 2070 6c65 6173 6520 6369  aries, please ci
+00002520: 7465 2074 6865 2066 6f6c 6c6f 7769 6e67  te the following
+00002530: 2072 6566 6572 656e 6365 2069 6e20 796f   reference in yo
+00002540: 7572 2061 7274 6963 6c65 3a0a 0a3e 204a  ur article:..> J
+00002550: 7561 6e20 5261 6461 2d56 696c 656c 612e  uan Rada-Vilela.
+00002560: 2054 6865 2046 757a 7a79 4c69 7465 204c   The FuzzyLite L
+00002570: 6962 7261 7269 6573 2066 6f72 2046 757a  ibraries for Fuz
+00002580: 7a79 204c 6f67 6963 2043 6f6e 7472 6f6c  zy Logic Control
+00002590: 2c20 3230 3138 2e20 5552 4c20 6874 7470  , 2018. URL http
+000025a0: 733a 2f2f 6675 7a7a 796c 6974 652e 636f  s://fuzzylite.co
+000025b0: 6d2e 0a0a 4f72 2075 7369 6e67 2060 6269  m...Or using `bi
+000025c0: 6274 6578 603a 0a0a 6060 6062 6962 7465  btex`:..```bibte
+000025d0: 780a 406d 6973 637b 666c 3a3a 6675 7a7a  x.@misc{fl::fuzz
+000025e0: 796c 6974 652c 0a20 2020 2061 7574 686f  ylite,.    autho
+000025f0: 723d 7b4a 7561 6e20 5261 6461 2d56 696c  r={Juan Rada-Vil
+00002600: 656c 617d 2c0a 2020 2020 7469 746c 653d  ela},.    title=
+00002610: 7b54 6865 2046 757a 7a79 4c69 7465 204c  {The FuzzyLite L
+00002620: 6962 7261 7269 6573 2066 6f72 2046 757a  ibraries for Fuz
+00002630: 7a79 204c 6f67 6963 2043 6f6e 7472 6f6c  zy Logic Control
+00002640: 7d2c 0a20 2020 2075 726c 3d7b 6874 7470  },.    url={http
+00002650: 733a 2f2f 6675 7a7a 796c 6974 652e 636f  s://fuzzylite.co
+00002660: 6d7d 2c0a 2020 2020 7965 6172 3d7b 3230  m},.    year={20
+00002670: 3138 7d0a 7d0a 6060 600a 0a2a 2a2a 0a0a  18}.}.```..***..
+00002680: 6675 7a7a 796c 6974 6526 7265 673b 2069  fuzzylite&reg; i
+00002690: 7320 6120 7265 6769 7374 6572 6564 2074  s a registered t
+000026a0: 7261 6465 6d61 726b 206f 6620 4675 7a7a  rademark of Fuzz
+000026b0: 794c 6974 6520 3c62 723e 0a6a 6675 7a7a  yLite <br>.jfuzz
+000026c0: 796c 6974 6526 7472 6164 653b 2c20 7079  ylite&trade;, py
+000026d0: 6675 7a7a 796c 6974 6526 7472 6164 653b  fuzzylite&trade;
+000026e0: 2061 6e64 2051 7446 757a 7a79 4c69 7465   and QtFuzzyLite
+000026f0: 2674 7261 6465 3b20 6172 6520 7472 6164  &trade; are trad
+00002700: 656d 6172 6b73 206f 6620 4675 7a7a 794c  emarks of FuzzyL
+00002710: 6974 650a 0a                             ite..
```

