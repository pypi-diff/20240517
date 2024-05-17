# Comparing `tmp/mobspy-2.4.3.tar.gz` & `tmp/mobspy-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobspy-2.4.3.tar", last modified: Mon May 13 20:51:02 2024, max compression
+gzip compressed data, was "mobspy-2.4.4.tar", last modified: Fri May 17 16:16:21 2024, max compression
```

## Comparing `mobspy-2.4.3.tar` & `mobspy-2.4.4.tar`

### file list

```diff
@@ -1,431 +1,432 @@
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.845575 mobspy-2.4.3/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.157378 mobspy-2.4.3/.github/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.178272 mobspy-2.4.3/.github/workflows/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-06-15 12:59:57.000000 mobspy-2.4.3/.github/workflows/python-app.yml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      415 2024-04-09 17:41:00.000000 mobspy-2.4.3/.gitignore
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1034 2024-02-26 16:22:21.000000 mobspy-2.4.3/.readthedocs.yaml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-06-15 12:59:57.000000 mobspy-2.4.3/LICENSE
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-13 20:51:02.844972 mobspy-2.4.3/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6331 2024-03-08 01:34:03.000000 mobspy-2.4.3/README.md
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.203851 mobspy-2.4.3/docs/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      634 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Makefile
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.228026 mobspy-2.4.3/docs/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.229796 mobspy-2.4.3/docs/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_autosummary/mobspy.rst
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.159803 mobspy-2.4.3/docs/_build/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.271808 mobspy-2.4.3/docs/_build/doctrees/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.304353 mobspy-2.4.3/docs/_build/doctrees/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    95114 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23601 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30820 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/03_Characteristics.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7466 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    24161 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/05_For_Loops.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21599 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    50076 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18699 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/08_Units.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41471 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/09_Result_Data.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    28500 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15272 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17080 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/12_Born_Species.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    39545 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/13_Events.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15325 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.306459 mobspy-2.4.3/docs/_build/doctrees/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2971 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/_autosummary/mobspy.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4285 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/api.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)  1736636 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2754 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/for_local_use.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4048 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/index.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    26568 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/mobspy.data_handler.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67412 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/mobspy.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   490595 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/mobspy.modules.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16088 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/mobspy.parameter_scripts.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8486 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/mobspy.parameters.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8077 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/mobspy.plot_params.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    86993 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/mobspy.plot_scripts.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    33712 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/mobspy.sbml_simulator.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9059 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/mobspy.simulation_logging.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2767 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/modules.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.334049 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.360563 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2407 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/setup.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2439 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/doctrees/test_script.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.401099 mobspy-2.4.3/docs/_build/html/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      230 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/.buildinfo
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.456196 mobspy-2.4.3/docs/_build/html/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41132 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/01_Basic_Intro.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16265 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/02_Reaction_Inheritance.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17425 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/03_Characteristics.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10225 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/04_Characteristic_restriction.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15743 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/05_For_Loops.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14878 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/06_Order_Matters.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23518 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/07_Initial_Condition.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15642 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/08_Units.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23686 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/09_Result_Data.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23178 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/10_Reaction_Rates.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14337 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/11_Looping_Through_Species.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14032 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/12_Born_Species.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    28370 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/13_Events.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18015 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/14_Concatenating_Simulations.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.460187 mobspy-2.4.3/docs/_build/html/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7201 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_autosummary/mobspy.html
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.488828 mobspy-2.4.3/docs/_build/html/_images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_13_Events_11_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_13_Events_1_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_13_Events_4_3.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_13_Events_8_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.506928 mobspy-2.4.3/docs/_build/html/_sources/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.528933 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.530580 mobspy-2.4.3/docs/_build/html/_sources/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/_autosummary/mobspy.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/api.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/for_local_use.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/mobspy.data_handler.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/mobspy.modules.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/mobspy.parameters.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/mobspy.plot_params.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/mobspy.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/mobspy.simulation_logging.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/setup.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_sources/test_script.rst.txt
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.556765 mobspy-2.4.3/docs/_build/html/_static/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4289 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15094 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.558764 mobspy-2.4.3/docs/_build/html/_static/css/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3229 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.631637 mobspy-2.4.3/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    87624 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67312 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    86288 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    66444 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   165742 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   444379 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   165548 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    98024 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    77160 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   323344 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   193308 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   309728 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   184912 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   328412 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   195704 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   309192 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   182708 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   135314 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4472 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/doctools.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/file.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    89501 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.637609 mobspy-2.4.3/docs/_build/html/_static/js/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      934 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4370 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2734 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5023 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4758 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/language_data.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4467 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6861 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/nbsphinx-code-cells.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      584 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/nbsphinx-gallery.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2871 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4902 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/pygments.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18732 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5123 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7627 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/api.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6551 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/for_local_use.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67727 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/genindex.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10018 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/index.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14863 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/mobspy.data_handler.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    91437 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/mobspy.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   178543 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/mobspy.modules.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11761 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/mobspy.parameter_scripts.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8867 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/mobspy.parameters.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8736 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/mobspy.plot_params.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    36208 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/mobspy.plot_scripts.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16526 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/mobspy.sbml_simulator.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9250 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/mobspy.simulation_logging.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23199 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/modules.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8450 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/objects.inv
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17062 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/py-modindex.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6595 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/search.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    96699 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/searchindex.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6464 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/setup.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6500 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/_build/html/test_script.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/api.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1220 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/conf.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/for_local_use.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/index.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      800 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/make.bat
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/mobspy.data_handler.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/mobspy.modules.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/mobspy.parameter_scripts.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/mobspy.parameters.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/mobspy.plot_params.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/mobspy.plot_scripts.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/mobspy.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/mobspy.sbml_simulator.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/mobspy.simulation_logging.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/modules.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/setup.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.3/docs/test_script.rst
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.163369 mobspy-2.4.3/example_models/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.663795 mobspy-2.4.3/example_models/Tutorial Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   132826 2024-05-05 13:25:04.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6793 2024-05-05 18:27:41.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8153 2024-05-05 20:46:30.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3725 2024-05-06 09:21:49.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5464 2024-05-06 12:26:05.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8168 2024-05-06 13:31:40.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8662 2024-05-11 12:56:11.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    90412 2024-05-11 13:19:54.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25382 2024-05-13 09:35:02.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4029 2023-11-22 12:58:00.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4498 2023-11-22 13:00:12.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    49256 2023-11-22 13:00:32.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2023-04-21 15:54:19.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.667990 mobspy-2.4.3/example_models/Tutorial Notebooks/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12324 2023-04-19 14:32:18.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/images/Matching_Meta.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   141303 2023-04-09 17:03:35.000000 mobspy-2.4.3/example_models/Tutorial Notebooks/images/vectorial_space.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.681989 mobspy-2.4.3/example_models/application_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      572 2024-01-28 20:43:25.000000 mobspy-2.4.3/example_models/application_models/AB_2CD.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1448 2024-01-28 20:44:42.000000 mobspy-2.4.3/example_models/application_models/AND_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2357 2024-01-28 20:43:25.000000 mobspy-2.4.3/example_models/application_models/CRISPR_Oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1447 2024-05-07 17:47:59.000000 mobspy-2.4.3/example_models/application_models/For_The_Trees.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1291 2024-01-28 20:48:26.000000 mobspy-2.4.3/example_models/application_models/NOR_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1237 2024-01-28 20:47:24.000000 mobspy-2.4.3/example_models/application_models/donor_receptor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1371 2024-01-28 20:48:41.000000 mobspy-2.4.3/example_models/application_models/oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      994 2023-07-07 11:50:03.000000 mobspy-2.4.3/example_models/application_models/positive_phage_feedback_loop.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2917 2024-01-28 20:49:35.000000 mobspy-2.4.3/example_models/application_models/random_walk.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      637 2023-07-05 11:46:34.000000 mobspy-2.4.3/example_models/application_models/simple_infection.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      564 2024-01-28 20:50:18.000000 mobspy-2.4.3/example_models/application_models/simple_repressor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      828 2023-07-05 12:49:47.000000 mobspy-2.4.3/example_models/application_models/simple_rule_based_and_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2024-05-13 20:43:59.000000 mobspy-2.4.3/for_local_use.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.683058 mobspy-2.4.3/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-06-15 12:59:57.000000 mobspy-2.4.3/images/img.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.689025 mobspy-2.4.3/mobspy/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-06-15 12:59:57.000000 mobspy-2.4.3/mobspy/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2024-05-13 20:50:28.000000 mobspy-2.4.3/mobspy/_version.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.699553 mobspy-2.4.3/mobspy/data_handler/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.3/mobspy/data_handler/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5759 2024-05-07 13:05:25.000000 mobspy-2.4.3/mobspy/data_handler/process_result_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8085 2024-05-02 12:49:07.000000 mobspy-2.4.3/mobspy/data_handler/time_series_object.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.703710 mobspy-2.4.3/mobspy/import_manager/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 12:02:22.000000 mobspy-2.4.3/mobspy/import_manager/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      639 2024-05-09 20:32:27.000000 mobspy-2.4.3/mobspy/import_manager/lazy_import_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      266 2024-05-11 12:43:21.000000 mobspy-2.4.3/mobspy/import_manager/profiler_import_time_test.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.733187 mobspy-2.4.3/mobspy/modules/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.3/mobspy/modules/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8797 2024-05-13 18:03:50.000000 mobspy-2.4.3/mobspy/modules/assignments_implementation.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5229 2024-05-09 12:06:51.000000 mobspy-2.4.3/mobspy/modules/class_of_meta_specie_named_any.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21459 2024-05-09 17:30:19.000000 mobspy-2.4.3/mobspy/modules/compiler.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1573 2024-05-09 17:30:55.000000 mobspy-2.4.3/mobspy/modules/context_related_scripts.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5331 2024-05-09 18:27:27.000000 mobspy-2.4.3/mobspy/modules/event_functions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12949 2024-05-13 20:43:47.000000 mobspy-2.4.3/mobspy/modules/function_rate_code.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13174 2024-05-09 09:50:51.000000 mobspy-2.4.3/mobspy/modules/logic_operator_objects.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    54494 2024-05-13 16:54:50.000000 mobspy-2.4.3/mobspy/modules/meta_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5620 2024-05-09 17:15:14.000000 mobspy-2.4.3/mobspy/modules/meta_class_utils.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    39955 2024-05-13 20:43:12.000000 mobspy-2.4.3/mobspy/modules/mobspy_expressions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5117 2024-05-09 12:41:41.000000 mobspy-2.4.3/mobspy/modules/mobspy_parameters.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15249 2024-05-09 18:17:38.000000 mobspy-2.4.3/mobspy/modules/order_operators.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17391 2024-05-13 20:43:02.000000 mobspy-2.4.3/mobspy/modules/reaction_construction_nb.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4504 2024-05-09 16:53:50.000000 mobspy-2.4.3/mobspy/modules/set_counts_module.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4175 2024-05-09 18:27:27.000000 mobspy-2.4.3/mobspy/modules/species_string_generator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7715 2024-05-09 16:53:50.000000 mobspy-2.4.3/mobspy/modules/unit_handler.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      428 2024-05-09 16:53:50.000000 mobspy-2.4.3/mobspy/modules/user_functions.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.735983 mobspy-2.4.3/mobspy/parameter_estimation_data_loader/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-02-28 22:21:33.000000 mobspy-2.4.3/mobspy/parameter_estimation_data_loader/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      912 2024-01-31 10:55:41.000000 mobspy-2.4.3/mobspy/parameter_estimation_data_loader/data_loader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7845 2024-05-09 20:49:27.000000 mobspy-2.4.3/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.739879 mobspy-2.4.3/mobspy/parameter_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.3/mobspy/parameter_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8408 2024-05-09 17:27:54.000000 mobspy-2.4.3/mobspy/parameter_scripts/parameter_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1957 2024-02-01 12:50:35.000000 mobspy-2.4.3/mobspy/parameter_scripts/parametric_sweeps.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.744433 mobspy-2.4.3/mobspy/parameters/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-06-15 12:59:57.000000 mobspy-2.4.3/mobspy/parameters/README.md
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.3/mobspy/parameters/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1188 2024-01-30 18:15:37.000000 mobspy-2.4.3/mobspy/parameters/default_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1285 2024-01-30 17:59:16.000000 mobspy-2.4.3/mobspy/parameters/example_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.746780 mobspy-2.4.3/mobspy/patch_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-04-09 18:34:07.000000 mobspy-2.4.3/mobspy/patch_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    71233 2024-05-05 13:14:45.000000 mobspy-2.4.3/mobspy/patch_scripts/basico_task_parametrization.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.752518 mobspy-2.4.3/mobspy/plot_params/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.3/mobspy/plot_params/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2024-05-06 14:50:24.000000 mobspy-2.4.3/mobspy/plot_params/default_plot_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1682 2024-05-06 14:53:26.000000 mobspy-2.4.3/mobspy/plot_params/example_plot_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.760102 mobspy-2.4.3/mobspy/plot_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-03-28 14:29:54.000000 mobspy-2.4.3/mobspy/plot_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10975 2024-05-07 17:42:50.000000 mobspy-2.4.3/mobspy/plot_scripts/default_plots.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17947 2024-05-07 13:15:06.000000 mobspy-2.4.3/mobspy/plot_scripts/hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2483 2024-05-07 13:17:04.000000 mobspy-2.4.3/mobspy/plot_scripts/process_plot_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3885 2024-03-28 14:34:48.000000 mobspy-2.4.3/mobspy/plot_scripts/statistics_calculations.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.763924 mobspy-2.4.3/mobspy/sbml_simulator/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8702 2024-03-20 17:46:34.000000 mobspy-2.4.3/mobspy/sbml_simulator/SBMLWriter.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.3/mobspy/sbml_simulator/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.768554 mobspy-2.4.3/mobspy/sbml_simulator/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5705 2024-04-09 18:33:16.000000 mobspy-2.4.3/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      146 2024-04-09 18:33:16.000000 mobspy-2.4.3/mobspy/sbml_simulator/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1040 2024-04-09 18:33:16.000000 mobspy-2.4.3/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8808 2024-04-09 18:33:16.000000 mobspy-2.4.3/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1070 2024-05-09 18:33:16.000000 mobspy-2.4.3/mobspy/sbml_simulator/builder.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12116 2024-05-09 20:34:41.000000 mobspy-2.4.3/mobspy/sbml_simulator/run.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    42305 2024-05-13 10:44:36.000000 mobspy-2.4.3/mobspy/simulation.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.771631 mobspy-2.4.3/mobspy/simulation_logging/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.3/mobspy/simulation_logging/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1104 2024-05-13 20:43:27.000000 mobspy-2.4.3/mobspy/simulation_logging/log_scripts.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       16 2024-05-13 10:44:36.000000 mobspy-2.4.3/mobspy/variables_and_operators.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.695652 mobspy-2.4.3/mobspy.egg-info/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-13 20:51:01.000000 mobspy-2.4.3/mobspy.egg-info/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16748 2024-05-13 20:51:01.000000 mobspy-2.4.3/mobspy.egg-info/SOURCES.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2024-05-13 20:51:01.000000 mobspy-2.4.3/mobspy.egg-info/dependency_links.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2024-05-13 20:51:01.000000 mobspy-2.4.3/mobspy.egg-info/requires.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2024-05-13 20:51:01.000000 mobspy-2.4.3/mobspy.egg-info/top_level.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-06-15 12:59:57.000000 mobspy-2.4.3/requirements.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2024-05-13 20:51:02.845879 mobspy-2.4.3/setup.cfg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-06-15 12:59:57.000000 mobspy-2.4.3/setup.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.776163 mobspy-2.4.3/test_plot_images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10767 2024-05-13 20:46:07.000000 mobspy-2.4.3/test_plot_images/constant_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    46622 2024-05-13 20:46:07.000000 mobspy-2.4.3/test_plot_images/deterministic_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    56222 2024-05-13 20:46:07.000000 mobspy-2.4.3/test_plot_images/stochastic_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    43663 2024-05-13 19:59:21.000000 mobspy-2.4.3/test_script.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 20:51:02.842894 mobspy-2.4.3/test_tools/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_1.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      241 2023-06-26 11:54:08.000000 mobspy-2.4.3/test_tools/model_10.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_11.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_12.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_13.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_14.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_15.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_16.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_17.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_18.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_19.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_2.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_20.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_21.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      471 2023-07-03 11:25:39.000000 mobspy-2.4.3/test_tools/model_22.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_23.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_24.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_25.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      518 2023-07-03 11:30:10.000000 mobspy-2.4.3/test_tools/model_26.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_27.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_28.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_29.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_3.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_30.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    55662 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_31.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      129 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_32.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      831 2023-07-03 15:00:26.000000 mobspy-2.4.3/test_tools/model_33.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2023-07-03 23:04:22.000000 mobspy-2.4.3/test_tools/model_34.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       61 2023-07-30 20:48:11.000000 mobspy-2.4.3/test_tools/model_35.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      175 2023-08-01 18:04:20.000000 mobspy-2.4.3/test_tools/model_36.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      391 2023-08-03 14:43:06.000000 mobspy-2.4.3/test_tools/model_37.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1427 2023-08-19 22:03:11.000000 mobspy-2.4.3/test_tools/model_38.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2853 2023-08-19 22:23:06.000000 mobspy-2.4.3/test_tools/model_39.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_4.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-11-15 12:57:45.000000 mobspy-2.4.3/test_tools/model_40.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1412 2023-11-15 12:57:45.000000 mobspy-2.4.3/test_tools/model_41.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      178 2023-11-15 12:57:45.000000 mobspy-2.4.3/test_tools/model_42.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      419 2023-11-17 12:18:00.000000 mobspy-2.4.3/test_tools/model_43.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      197 2024-01-31 16:54:44.000000 mobspy-2.4.3/test_tools/model_44.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8874 2024-02-22 02:44:14.000000 mobspy-2.4.3/test_tools/model_45.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      317 2024-02-24 00:21:58.000000 mobspy-2.4.3/test_tools/model_46.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      243 2024-02-24 13:50:27.000000 mobspy-2.4.3/test_tools/model_47.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      119 2024-05-02 10:01:49.000000 mobspy-2.4.3/test_tools/model_48.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      171 2024-05-07 20:34:12.000000 mobspy-2.4.3/test_tools/model_49.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_5.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      271 2024-05-13 15:07:53.000000 mobspy-2.4.3/test_tools/model_50.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      452 2024-05-13 19:52:51.000000 mobspy-2.4.3/test_tools/model_51.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-05-13 19:55:06.000000 mobspy-2.4.3/test_tools/model_52.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      389 2023-07-03 10:56:19.000000 mobspy-2.4.3/test_tools/model_6.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1362 2023-07-03 11:02:54.000000 mobspy-2.4.3/test_tools/model_7.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      433 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_8.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-06-15 12:59:57.000000 mobspy-2.4.3/test_tools/model_9.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-06-15 12:59:57.000000 mobspy-2.4.3/useful_parameters.json
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:21.041458 mobspy-2.4.4/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.839733 mobspy-2.4.4/.github/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.864715 mobspy-2.4.4/.github/workflows/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-06-15 12:59:57.000000 mobspy-2.4.4/.github/workflows/python-app.yml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      415 2024-04-09 17:41:00.000000 mobspy-2.4.4/.gitignore
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1034 2024-02-26 16:22:21.000000 mobspy-2.4.4/.readthedocs.yaml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-06-15 12:59:57.000000 mobspy-2.4.4/LICENSE
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-17 16:16:21.040623 mobspy-2.4.4/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6331 2024-03-08 01:34:03.000000 mobspy-2.4.4/README.md
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.891450 mobspy-2.4.4/docs/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      634 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Makefile
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.924018 mobspy-2.4.4/docs/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.926663 mobspy-2.4.4/docs/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_autosummary/mobspy.rst
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.841544 mobspy-2.4.4/docs/_build/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.982218 mobspy-2.4.4/docs/_build/doctrees/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.008719 mobspy-2.4.4/docs/_build/doctrees/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    95114 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23601 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30820 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/03_Characteristics.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7466 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    24161 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/05_For_Loops.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21599 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    50076 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18699 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/08_Units.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    41471 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/09_Result_Data.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    28500 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15272 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17080 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/12_Born_Species.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    39545 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/13_Events.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15325 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.011128 mobspy-2.4.4/docs/_build/doctrees/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2971 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/_autosummary/mobspy.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4285 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/api.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)  1736636 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2754 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/for_local_use.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4048 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26568 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.data_handler.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67412 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   490595 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.modules.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16088 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.parameter_scripts.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8486 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.parameters.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8077 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.plot_params.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    86993 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.plot_scripts.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    33712 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.sbml_simulator.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9059 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.simulation_logging.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2767 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/modules.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.044739 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.073824 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2407 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/setup.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2439 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/test_script.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.131235 mobspy-2.4.4/docs/_build/html/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      230 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/.buildinfo
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.184126 mobspy-2.4.4/docs/_build/html/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    41132 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/01_Basic_Intro.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16265 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17425 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/03_Characteristics.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10225 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/04_Characteristic_restriction.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15743 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/05_For_Loops.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14878 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/06_Order_Matters.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23518 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/07_Initial_Condition.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15642 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/08_Units.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23686 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/09_Result_Data.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23178 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/10_Reaction_Rates.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14337 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/11_Looping_Through_Species.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14032 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/12_Born_Species.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    28370 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/13_Events.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18015 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.185203 mobspy-2.4.4/docs/_build/html/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7201 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_autosummary/mobspy.html
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.217450 mobspy-2.4.4/docs/_build/html/_images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_11_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_1_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_4_3.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_8_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.235859 mobspy-2.4.4/docs/_build/html/_sources/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.262880 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.265286 mobspy-2.4.4/docs/_build/html/_sources/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/_autosummary/mobspy.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/api.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/for_local_use.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.data_handler.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.modules.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.parameters.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.plot_params.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.simulation_logging.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/setup.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/test_script.rst.txt
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.289483 mobspy-2.4.4/docs/_build/html/_static/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4289 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15094 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.292769 mobspy-2.4.4/docs/_build/html/_static/css/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3229 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.365023 mobspy-2.4.4/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    87624 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67312 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    86288 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    66444 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   165742 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   444379 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   165548 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    98024 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    77160 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   323344 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   193308 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   309728 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   184912 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   328412 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   195704 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   309192 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   182708 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   135314 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4472 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/file.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    89501 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.372284 mobspy-2.4.4/docs/_build/html/_static/js/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      934 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4370 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2734 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5023 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4758 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4467 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6861 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/nbsphinx-code-cells.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      584 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/nbsphinx-gallery.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2871 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4902 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18732 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7627 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/api.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6551 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/for_local_use.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67727 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/genindex.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10018 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/index.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14863 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.data_handler.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    91437 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   178543 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.modules.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11761 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.parameter_scripts.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8867 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.parameters.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8736 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.plot_params.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    36208 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.plot_scripts.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16526 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.sbml_simulator.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9250 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.simulation_logging.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23199 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/modules.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8450 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/objects.inv
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17062 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/py-modindex.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6595 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/search.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    96699 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/searchindex.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6464 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/setup.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6500 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/test_script.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/api.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1220 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/conf.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/for_local_use.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/index.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      800 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/make.bat
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.data_handler.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.modules.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.parameter_scripts.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.parameters.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.plot_params.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.plot_scripts.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.sbml_simulator.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.simulation_logging.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/modules.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/setup.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/test_script.rst
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.847299 mobspy-2.4.4/example_models/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.409247 mobspy-2.4.4/example_models/Tutorial Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   132826 2024-05-05 13:25:04.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7029 2024-05-14 12:30:35.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8153 2024-05-05 20:46:30.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3725 2024-05-06 09:21:49.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5464 2024-05-06 12:26:05.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8168 2024-05-06 13:31:40.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8662 2024-05-11 12:56:11.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    90412 2024-05-11 13:19:54.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30172 2024-05-14 13:24:55.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4201 2024-05-14 14:17:52.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4862 2024-05-14 14:54:54.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    47437 2024-05-14 20:07:50.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    31117 2024-05-15 13:19:46.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.413718 mobspy-2.4.4/example_models/Tutorial Notebooks/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12324 2023-04-19 14:32:18.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/images/Matching_Meta.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   141303 2023-04-09 17:03:35.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/images/vectorial_space.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.655806 mobspy-2.4.4/example_models/application_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      572 2024-01-28 20:43:25.000000 mobspy-2.4.4/example_models/application_models/AB_2CD.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1448 2024-01-28 20:44:42.000000 mobspy-2.4.4/example_models/application_models/AND_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2357 2024-01-28 20:43:25.000000 mobspy-2.4.4/example_models/application_models/CRISPR_Oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1447 2024-05-07 17:47:59.000000 mobspy-2.4.4/example_models/application_models/For_The_Trees.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1291 2024-01-28 20:48:26.000000 mobspy-2.4.4/example_models/application_models/NOR_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1237 2024-01-28 20:47:24.000000 mobspy-2.4.4/example_models/application_models/donor_receptor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1371 2024-01-28 20:48:41.000000 mobspy-2.4.4/example_models/application_models/oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      994 2023-07-07 11:50:03.000000 mobspy-2.4.4/example_models/application_models/positive_phage_feedback_loop.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2917 2024-01-28 20:49:35.000000 mobspy-2.4.4/example_models/application_models/random_walk.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      637 2023-07-05 11:46:34.000000 mobspy-2.4.4/example_models/application_models/simple_infection.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      564 2024-01-28 20:50:18.000000 mobspy-2.4.4/example_models/application_models/simple_repressor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      828 2023-07-05 12:49:47.000000 mobspy-2.4.4/example_models/application_models/simple_rule_based_and_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      100 2024-05-17 12:39:17.000000 mobspy-2.4.4/for_local_use.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.657243 mobspy-2.4.4/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-06-15 12:59:57.000000 mobspy-2.4.4/images/img.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.664164 mobspy-2.4.4/mobspy/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2024-05-17 12:41:21.000000 mobspy-2.4.4/mobspy/_version.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.687986 mobspy-2.4.4/mobspy/data_handler/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/data_handler/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5759 2024-05-07 13:05:25.000000 mobspy-2.4.4/mobspy/data_handler/process_result_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8430 2024-05-15 10:39:35.000000 mobspy-2.4.4/mobspy/data_handler/time_series_object.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.694889 mobspy-2.4.4/mobspy/import_manager/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 12:02:22.000000 mobspy-2.4.4/mobspy/import_manager/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      639 2024-05-09 20:32:27.000000 mobspy-2.4.4/mobspy/import_manager/lazy_import_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      266 2024-05-11 12:43:21.000000 mobspy-2.4.4/mobspy/import_manager/profiler_import_time_test.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.781509 mobspy-2.4.4/mobspy/modules/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/modules/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8797 2024-05-13 18:03:50.000000 mobspy-2.4.4/mobspy/modules/assignments_implementation.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5229 2024-05-09 12:06:51.000000 mobspy-2.4.4/mobspy/modules/class_of_meta_specie_named_any.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21459 2024-05-09 17:30:19.000000 mobspy-2.4.4/mobspy/modules/compiler.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1573 2024-05-09 17:30:55.000000 mobspy-2.4.4/mobspy/modules/context_related_scripts.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5331 2024-05-09 18:27:27.000000 mobspy-2.4.4/mobspy/modules/event_functions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12949 2024-05-13 20:43:47.000000 mobspy-2.4.4/mobspy/modules/function_rate_code.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13174 2024-05-09 09:50:51.000000 mobspy-2.4.4/mobspy/modules/logic_operator_objects.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    54494 2024-05-13 16:54:50.000000 mobspy-2.4.4/mobspy/modules/meta_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5620 2024-05-09 17:15:14.000000 mobspy-2.4.4/mobspy/modules/meta_class_utils.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    39955 2024-05-13 20:43:12.000000 mobspy-2.4.4/mobspy/modules/mobspy_expressions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5117 2024-05-09 12:41:41.000000 mobspy-2.4.4/mobspy/modules/mobspy_parameters.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15249 2024-05-09 18:17:38.000000 mobspy-2.4.4/mobspy/modules/order_operators.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17391 2024-05-13 20:43:02.000000 mobspy-2.4.4/mobspy/modules/reaction_construction_nb.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4504 2024-05-09 16:53:50.000000 mobspy-2.4.4/mobspy/modules/set_counts_module.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4175 2024-05-09 18:27:27.000000 mobspy-2.4.4/mobspy/modules/species_string_generator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7715 2024-05-09 16:53:50.000000 mobspy-2.4.4/mobspy/modules/unit_handler.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      428 2024-05-09 16:53:50.000000 mobspy-2.4.4/mobspy/modules/user_functions.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.788755 mobspy-2.4.4/mobspy/parameter_estimation_data_loader/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-02-28 22:21:33.000000 mobspy-2.4.4/mobspy/parameter_estimation_data_loader/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      912 2024-01-31 10:55:41.000000 mobspy-2.4.4/mobspy/parameter_estimation_data_loader/data_loader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7845 2024-05-09 20:49:27.000000 mobspy-2.4.4/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.793781 mobspy-2.4.4/mobspy/parameter_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/parameter_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8408 2024-05-09 17:27:54.000000 mobspy-2.4.4/mobspy/parameter_scripts/parameter_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1957 2024-02-01 12:50:35.000000 mobspy-2.4.4/mobspy/parameter_scripts/parametric_sweeps.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.799802 mobspy-2.4.4/mobspy/parameters/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/parameters/README.md
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/parameters/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1188 2024-01-30 18:15:37.000000 mobspy-2.4.4/mobspy/parameters/default_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1285 2024-01-30 17:59:16.000000 mobspy-2.4.4/mobspy/parameters/example_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.802453 mobspy-2.4.4/mobspy/patch_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-04-09 18:34:07.000000 mobspy-2.4.4/mobspy/patch_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    71233 2024-05-05 13:14:45.000000 mobspy-2.4.4/mobspy/patch_scripts/basico_task_parametrization.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.814070 mobspy-2.4.4/mobspy/plot_params/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/plot_params/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2024-05-06 14:50:24.000000 mobspy-2.4.4/mobspy/plot_params/default_plot_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1907 2024-05-17 12:30:55.000000 mobspy-2.4.4/mobspy/plot_params/example_plot_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.823408 mobspy-2.4.4/mobspy/plot_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-03-28 14:29:54.000000 mobspy-2.4.4/mobspy/plot_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10975 2024-05-07 17:42:50.000000 mobspy-2.4.4/mobspy/plot_scripts/default_plots.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    20277 2024-05-17 12:33:10.000000 mobspy-2.4.4/mobspy/plot_scripts/hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2852 2024-05-16 20:39:29.000000 mobspy-2.4.4/mobspy/plot_scripts/process_plot_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3885 2024-03-28 14:34:48.000000 mobspy-2.4.4/mobspy/plot_scripts/statistics_calculations.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.829666 mobspy-2.4.4/mobspy/sbml_simulator/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8702 2024-03-20 17:46:34.000000 mobspy-2.4.4/mobspy/sbml_simulator/SBMLWriter.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/sbml_simulator/__init__.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.855762 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5705 2024-04-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      146 2024-04-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1040 2024-04-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8808 2024-04-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1070 2024-05-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/builder.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12116 2024-05-09 20:34:41.000000 mobspy-2.4.4/mobspy/sbml_simulator/run.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    43371 2024-05-16 09:23:48.000000 mobspy-2.4.4/mobspy/simulation.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.858034 mobspy-2.4.4/mobspy/simulation_logging/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/simulation_logging/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1099 2024-05-14 16:05:30.000000 mobspy-2.4.4/mobspy/simulation_logging/log_scripts.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       16 2024-05-13 10:44:36.000000 mobspy-2.4.4/mobspy/variables_and_operators.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.681692 mobspy-2.4.4/mobspy.egg-info/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-17 16:16:18.000000 mobspy-2.4.4/mobspy.egg-info/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16772 2024-05-17 16:16:19.000000 mobspy-2.4.4/mobspy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2024-05-17 16:16:18.000000 mobspy-2.4.4/mobspy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2024-05-17 16:16:18.000000 mobspy-2.4.4/mobspy.egg-info/requires.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2024-05-17 16:16:18.000000 mobspy-2.4.4/mobspy.egg-info/top_level.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-06-15 12:59:57.000000 mobspy-2.4.4/requirements.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2024-05-17 16:16:21.041791 mobspy-2.4.4/setup.cfg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-06-15 12:59:57.000000 mobspy-2.4.4/setup.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.864382 mobspy-2.4.4/test_plot_images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10767 2024-05-16 18:23:19.000000 mobspy-2.4.4/test_plot_images/constant_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    44355 2024-05-16 18:23:19.000000 mobspy-2.4.4/test_plot_images/deterministic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    53864 2024-05-16 18:23:18.000000 mobspy-2.4.4/test_plot_images/stochastic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    44218 2024-05-16 18:24:17.000000 mobspy-2.4.4/test_script.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:21.038268 mobspy-2.4.4/test_tools/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_1.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      241 2023-06-26 11:54:08.000000 mobspy-2.4.4/test_tools/model_10.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_11.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_12.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_13.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_14.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_15.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_16.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_17.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_18.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_19.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_2.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_20.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_21.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      471 2023-07-03 11:25:39.000000 mobspy-2.4.4/test_tools/model_22.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_23.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_24.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_25.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      518 2023-07-03 11:30:10.000000 mobspy-2.4.4/test_tools/model_26.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_27.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_28.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_29.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_3.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_30.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    55662 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_31.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      129 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_32.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      831 2023-07-03 15:00:26.000000 mobspy-2.4.4/test_tools/model_33.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2023-07-03 23:04:22.000000 mobspy-2.4.4/test_tools/model_34.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       61 2023-07-30 20:48:11.000000 mobspy-2.4.4/test_tools/model_35.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      175 2023-08-01 18:04:20.000000 mobspy-2.4.4/test_tools/model_36.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      391 2023-08-03 14:43:06.000000 mobspy-2.4.4/test_tools/model_37.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1427 2023-08-19 22:03:11.000000 mobspy-2.4.4/test_tools/model_38.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2853 2023-08-19 22:23:06.000000 mobspy-2.4.4/test_tools/model_39.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_4.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-11-15 12:57:45.000000 mobspy-2.4.4/test_tools/model_40.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1412 2023-11-15 12:57:45.000000 mobspy-2.4.4/test_tools/model_41.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      178 2023-11-15 12:57:45.000000 mobspy-2.4.4/test_tools/model_42.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      419 2023-11-17 12:18:00.000000 mobspy-2.4.4/test_tools/model_43.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      197 2024-01-31 16:54:44.000000 mobspy-2.4.4/test_tools/model_44.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8874 2024-02-22 02:44:14.000000 mobspy-2.4.4/test_tools/model_45.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      317 2024-02-24 00:21:58.000000 mobspy-2.4.4/test_tools/model_46.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      243 2024-02-24 13:50:27.000000 mobspy-2.4.4/test_tools/model_47.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      119 2024-05-02 10:01:49.000000 mobspy-2.4.4/test_tools/model_48.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      171 2024-05-07 20:34:12.000000 mobspy-2.4.4/test_tools/model_49.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_5.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      271 2024-05-13 15:07:53.000000 mobspy-2.4.4/test_tools/model_50.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      452 2024-05-13 19:52:51.000000 mobspy-2.4.4/test_tools/model_51.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-05-13 19:55:06.000000 mobspy-2.4.4/test_tools/model_52.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      417 2024-05-16 18:22:27.000000 mobspy-2.4.4/test_tools/model_53.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      389 2023-07-03 10:56:19.000000 mobspy-2.4.4/test_tools/model_6.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1362 2023-07-03 11:02:54.000000 mobspy-2.4.4/test_tools/model_7.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      433 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_8.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_9.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-06-15 12:59:57.000000 mobspy-2.4.4/useful_parameters.json
```

### Comparing `mobspy-2.4.3/.github/workflows/python-app.yml` & `mobspy-2.4.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/.readthedocs.yaml` & `mobspy-2.4.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/LICENSE` & `mobspy-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/PKG-INFO` & `mobspy-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.4.3
+Version: 2.4.4
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.4.3/README.md` & `mobspy-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Makefile` & `mobspy-2.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.4/docs/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.4/docs/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.4/docs/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.4/docs/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.4/docs/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.4/docs/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.4/docs/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/08_Units.ipynb` & `mobspy-2.4.4/docs/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.4/docs/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.4/docs/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.4/docs/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.4/docs/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/13_Events.ipynb` & `mobspy-2.4.4/docs/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.4/docs/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/03_Characteristics.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/03_Characteristics.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/05_For_Loops.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/05_For_Loops.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/08_Units.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/08_Units.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/09_Result_Data.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/09_Result_Data.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/12_Born_Species.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/12_Born_Species.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/13_Events.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/13_Events.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree` & `mobspy-2.4.4/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/_autosummary/mobspy.doctree` & `mobspy-2.4.4/docs/_build/doctrees/_autosummary/mobspy.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/api.doctree` & `mobspy-2.4.4/docs/_build/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/environment.pickle` & `mobspy-2.4.4/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/for_local_use.doctree` & `mobspy-2.4.4/docs/_build/doctrees/for_local_use.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/index.doctree` & `mobspy-2.4.4/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/mobspy.data_handler.doctree` & `mobspy-2.4.4/docs/_build/doctrees/mobspy.data_handler.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/mobspy.doctree` & `mobspy-2.4.4/docs/_build/doctrees/mobspy.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/mobspy.modules.doctree` & `mobspy-2.4.4/docs/_build/doctrees/mobspy.modules.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/mobspy.parameter_scripts.doctree` & `mobspy-2.4.4/docs/_build/doctrees/mobspy.parameter_scripts.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/mobspy.parameters.doctree` & `mobspy-2.4.4/docs/_build/doctrees/mobspy.parameters.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/mobspy.plot_params.doctree` & `mobspy-2.4.4/docs/_build/doctrees/mobspy.plot_params.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/mobspy.plot_scripts.doctree` & `mobspy-2.4.4/docs/_build/doctrees/mobspy.plot_scripts.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/mobspy.sbml_simulator.doctree` & `mobspy-2.4.4/docs/_build/doctrees/mobspy.sbml_simulator.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/mobspy.simulation_logging.doctree` & `mobspy-2.4.4/docs/_build/doctrees/mobspy.simulation_logging.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/modules.doctree` & `mobspy-2.4.4/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png` & `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/setup.doctree` & `mobspy-2.4.4/docs/_build/doctrees/setup.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/doctrees/test_script.doctree` & `mobspy-2.4.4/docs/_build/doctrees/test_script.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/01_Basic_Intro.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/01_Basic_Intro.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/02_Reaction_Inheritance.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/03_Characteristics.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/03_Characteristics.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/04_Characteristic_restriction.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/04_Characteristic_restriction.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/05_For_Loops.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/05_For_Loops.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/06_Order_Matters.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/06_Order_Matters.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/07_Initial_Condition.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/07_Initial_Condition.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/08_Units.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/08_Units.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/08_Units.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/09_Result_Data.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/09_Result_Data.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/10_Reaction_Rates.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/10_Reaction_Rates.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/11_Looping_Through_Species.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/11_Looping_Through_Species.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/12_Born_Species.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/12_Born_Species.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/13_Events.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/13_Events.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/13_Events.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/14_Concatenating_Simulations.html` & `mobspy-2.4.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_autosummary/mobspy.html` & `mobspy-2.4.4/docs/_build/html/_autosummary/mobspy.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_13_Events_11_2.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_11_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_13_Events_1_2.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_1_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_13_Events_4_3.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_4_3.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_13_Events_8_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_8_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png` & `mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt` & `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/index.rst.txt` & `mobspy-2.4.4/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/mobspy.data_handler.rst.txt` & `mobspy-2.4.4/docs/_build/html/_sources/mobspy.data_handler.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/mobspy.modules.rst.txt` & `mobspy-2.4.4/docs/_build/html/_sources/mobspy.modules.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt` & `mobspy-2.4.4/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/mobspy.parameters.rst.txt` & `mobspy-2.4.4/docs/_build/html/_sources/mobspy.parameters.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/mobspy.plot_params.rst.txt` & `mobspy-2.4.4/docs/_build/html/_sources/mobspy.plot_params.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt` & `mobspy-2.4.4/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/mobspy.rst.txt` & `mobspy-2.4.4/docs/_build/html/_sources/mobspy.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt` & `mobspy-2.4.4/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `mobspy-2.4.4/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/basic.css` & `mobspy-2.4.4/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/badge_only.css` & `mobspy-2.4.4/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-bold.woff` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-normal.woff` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/css/theme.css` & `mobspy-2.4.4/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/doctools.js` & `mobspy-2.4.4/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/jquery.js` & `mobspy-2.4.4/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/js/badge_only.js` & `mobspy-2.4.4/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `mobspy-2.4.4/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/js/html5shiv.min.js` & `mobspy-2.4.4/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/js/theme.js` & `mobspy-2.4.4/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/language_data.js` & `mobspy-2.4.4/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg` & `mobspy-2.4.4/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/nbsphinx-code-cells.css` & `mobspy-2.4.4/docs/_build/html/_static/nbsphinx-code-cells.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/nbsphinx-gallery.css` & `mobspy-2.4.4/docs/_build/html/_static/nbsphinx-gallery.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/nbsphinx-no-thumbnail.svg` & `mobspy-2.4.4/docs/_build/html/_static/nbsphinx-no-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/pygments.css` & `mobspy-2.4.4/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/searchtools.js` & `mobspy-2.4.4/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/_static/sphinx_highlight.js` & `mobspy-2.4.4/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/api.html` & `mobspy-2.4.4/docs/_build/html/api.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/for_local_use.html` & `mobspy-2.4.4/docs/_build/html/for_local_use.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/genindex.html` & `mobspy-2.4.4/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/index.html` & `mobspy-2.4.4/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/mobspy.data_handler.html` & `mobspy-2.4.4/docs/_build/html/mobspy.data_handler.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/mobspy.html` & `mobspy-2.4.4/docs/_build/html/mobspy.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/mobspy.modules.html` & `mobspy-2.4.4/docs/_build/html/mobspy.modules.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/mobspy.parameter_scripts.html` & `mobspy-2.4.4/docs/_build/html/mobspy.parameter_scripts.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/mobspy.parameters.html` & `mobspy-2.4.4/docs/_build/html/mobspy.parameters.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/mobspy.plot_params.html` & `mobspy-2.4.4/docs/_build/html/mobspy.plot_params.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/mobspy.plot_scripts.html` & `mobspy-2.4.4/docs/_build/html/mobspy.plot_scripts.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/mobspy.sbml_simulator.html` & `mobspy-2.4.4/docs/_build/html/mobspy.sbml_simulator.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/mobspy.simulation_logging.html` & `mobspy-2.4.4/docs/_build/html/mobspy.simulation_logging.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/modules.html` & `mobspy-2.4.4/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/objects.inv` & `mobspy-2.4.4/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/py-modindex.html` & `mobspy-2.4.4/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/search.html` & `mobspy-2.4.4/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/searchindex.js` & `mobspy-2.4.4/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/setup.html` & `mobspy-2.4.4/docs/_build/html/setup.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/_build/html/test_script.html` & `mobspy-2.4.4/docs/_build/html/test_script.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/conf.py` & `mobspy-2.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/index.rst` & `mobspy-2.4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/make.bat` & `mobspy-2.4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/mobspy.data_handler.rst` & `mobspy-2.4.4/docs/mobspy.data_handler.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/mobspy.modules.rst` & `mobspy-2.4.4/docs/mobspy.modules.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/mobspy.parameter_scripts.rst` & `mobspy-2.4.4/docs/mobspy.parameter_scripts.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/mobspy.parameters.rst` & `mobspy-2.4.4/docs/mobspy.parameters.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/mobspy.plot_params.rst` & `mobspy-2.4.4/docs/mobspy.plot_params.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/mobspy.plot_scripts.rst` & `mobspy-2.4.4/docs/mobspy.plot_scripts.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/mobspy.rst` & `mobspy-2.4.4/docs/mobspy.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/docs/mobspy.sbml_simulator.rst` & `mobspy-2.4.4/docs/mobspy.sbml_simulator.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988715277777778%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'data': {'text/plain': ['<mobspy.modules.meta_class.Reactions at "*

 * *            "0x7fec96aa6a90>']}}}}, 11: {'outputs': {0: {'data': {'text/plain': "*

 * *            "['(<mobspy.modules.meta_class.Species at 0x7fec96a7f760>,\\n', ' "*

 * *            "<mobspy.modules.meta_class.Species at 0x7fec96aa6370>,\\n', ' "*

 * *            "<mobspy.modules.meta_class.Species at 0x7fec96a7ffa0>,\\n', ' "*

 * *            "<mobspy.modules.meta_class.Species at 0x7fec96aa66a0>)']}}}}, 12: {'source': ['Now […]*

```diff
@@ -39,15 +39,15 @@
             "execution_count": 2,
             "id": "f9687e7a-abc5-4fde-a61c-aa8b6a2e8181",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fda25321c70>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7fec96aa6a90>"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -130,18 +130,18 @@
             "execution_count": 6,
             "id": "5f0c9765-b7d0-4e26-98ed-8660fcd74f26",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(<mobspy.modules.meta_class.Species at 0x7fda1f179d90>,\n",
-                            " <mobspy.modules.meta_class.Species at 0x7fda1f19f670>,\n",
-                            " <mobspy.modules.meta_class.Species at 0x7fda25321940>,\n",
-                            " <mobspy.modules.meta_class.Species at 0x7fda25321910>)"
+                            "(<mobspy.modules.meta_class.Species at 0x7fec96a7f760>,\n",
+                            " <mobspy.modules.meta_class.Species at 0x7fec96aa6370>,\n",
+                            " <mobspy.modules.meta_class.Species at 0x7fec96a7ffa0>,\n",
+                            " <mobspy.modules.meta_class.Species at 0x7fec96aa66a0>)"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -153,15 +153,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2709519d-a951-4995-a3a3-d048f2b4a6c8",
             "metadata": {},
             "source": [
-                "Now we compile the simulation to show all defined reactions:"
+                "Now, we compile the simulation to show all defined reactions. \n",
+                "The meta-reactions are stored in the meta-species themselves. Once the meta-species are passed to the Simulation constructor, it compiles all meta-reactions in all participating meta-species to get all the model reactions.  "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "98b7da18-0d3e-4e75-8e27-893e99c91a5f",
             "metadata": {},
```

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9769644923941798%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Looping Strategies\\n'), (2, 'In this section, we "*

 * *            'describe some looping strategies in MobsPy regarding both species and '*

 * *            "characteristics. ')], delete: [2, 0]}}, 3: {'source': {insert: [(0, '## "*

 * *            "Characteristic Loop\\n'), (2, 'One can loop through characteristics by keeping them "*

 * *            'in a list and using the .c operator. Furthermore, the method get_characteristics() '*

 * *            "returns the set of characteristic […]*

```diff
@@ -1,15 +1,25 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "7c7b4173-43bb-4bc3-9ff7-c51b9b3ecb70",
             "metadata": {},
             "source": [
-                "# Models\n",
+                "# Looping Strategies\n",
+                "\n",
+                "In this section, we describe some looping strategies in MobsPy regarding both species and characteristics. "
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "629e560c-2423-4452-89e5-7f00f1521ffd",
+            "metadata": {},
+            "source": [
+                "## Model Loop \n",
                 "\n",
                 "The models created used the '|' operator can be iterated through"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
@@ -39,31 +49,31 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c9615979-1e34-471e-9d06-eb57f04b8b5d",
             "metadata": {},
             "source": [
-                "# Characteristics\n",
+                "## Characteristic Loop\n",
                 "\n",
-                "One can loop through characteristics by keeping them in a list and using the .c operator. Futhermore, the method get_characteristics() returns the set of characteristics directly added to that species."
+                "One can loop through characteristics by keeping them in a list and using the .c operator. Furthermore, the method get_characteristics() returns the set of characteristics directly added to that species."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "5391b29f-5a1d-42c7-94f5-90d83a53d75c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "{'a2', 'a1', 'a3'}\n",
-                        "{\"['b1', 'b2', 'b3']\"}\n"
+                        "{'a1', 'a2', 'a3'}\n",
+                        "{'b1', 'b2', 'b3'}\n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "Compiling model\n"
@@ -74,59 +84,61 @@
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "Species\n",
                         "A.a1,0\n",
                         "A.a2,0\n",
                         "A.a3,0\n",
-                        "B.['b1', 'b2', 'b3'],0\n",
+                        "B.b1,0\n",
+                        "B.b2,0\n",
+                        "B.b3,0\n",
                         "\n",
                         "Mappings\n",
                         "A :\n",
                         "A.a1\n",
                         "A.a2\n",
                         "A.a3\n",
                         "B :\n",
-                        "B.['b1', 'b2', 'b3']\n",
+                        "B.b1\n",
+                        "B.b2\n",
+                        "B.b3\n",
                         "\n",
                         "Parameters\n",
                         "volume,1\n",
                         "\n",
                         "Reactions\n",
-                        "reaction_0,{'re': [(1, 'A.a1'), (1, \"B.['b1', 'b2', 'b3']\")], 'pr': [], 'kin': \"A.a1 * B.['b1', 'b2', 'b3'] * 1 * volume^-1\"}\n",
-                        "reaction_1,{'re': [(1, 'A.a2'), (1, \"B.['b1', 'b2', 'b3']\")], 'pr': [], 'kin': \"A.a2 * B.['b1', 'b2', 'b3'] * 1 * volume^-1\"}\n",
-                        "reaction_2,{'re': [(1, 'A.a3'), (1, \"B.['b1', 'b2', 'b3']\")], 'pr': [], 'kin': \"A.a3 * B.['b1', 'b2', 'b3'] * 1 * volume^-1\"}\n",
+                        "reaction_0,{'re': [(1, 'A.a1'), (1, 'B.b1')], 'pr': [], 'kin': 'A.a1 * B.b1 * 1 * volume^-1'}\n",
+                        "reaction_1,{'re': [(1, 'A.a2'), (1, 'B.b2')], 'pr': [], 'kin': 'A.a2 * B.b2 * 1 * volume^-1'}\n",
+                        "reaction_2,{'re': [(1, 'A.a3'), (1, 'B.b3')], 'pr': [], 'kin': 'A.a3 * B.b3 * 1 * volume^-1'}\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "from mobspy import *\n",
-                "\n",
                 "A, B = BaseSpecies()\n",
                 "\n",
                 "l_a = ['a1', 'a2', 'a3']\n",
                 "l_b = ['b1', 'b2', 'b3']\n",
                 "\n",
                 "for a, b in zip(l_a, l_b):\n",
-                "    A.c(a) + B.c(l_b) >> Zero [1]\n",
+                "    A.c(a) + B.c(b) >> Zero [1]\n",
                 "\n",
                 "print(A.get_characteristics())\n",
                 "print(B.get_characteristics())\n",
                 "\n",
                 "S = Simulation(A | B)\n",
                 "print(S.compile())\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0a1e2d9c-0c0c-4073-843e-f8b2f14bb24c",
             "metadata": {},
             "source": [
-                "# List Species\n",
+                "## List Species\n",
                 "\n",
                 "Futhermore, MobsPy provides a ListSpecies constructor. This constructor creates a list of meta-species automatically named with the variable used to construct the ListSpecies plus _ and the number of the species in the list."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
```

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/12_Born_Species.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9925426136363636%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Born Species \\n'), (2, 'In this section, we explain "*

 * *            'how MobsPy deals with meta-species in the products that do not have an equal match in '*

 * *            'the reactants. Firstly, we refer to these species as born species, as these species '*

 * *            'have no matching meta-species in the reactants to define their state in the '*

 * *            "products.\\n'), (3, 'Without a reactant to define its state, MobsPy chooses only to "*

 * *            "create th […]*

```diff
@@ -1,18 +1,22 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "c9cb873f-868b-4de7-8fcd-babd0b5b2927",
             "metadata": {},
             "source": [
-                "# Born Species\n",
+                "# Born Species \n",
                 "\n",
-                "MobsPy deals with meta-species in the products that do not have a match in the meta-reactants in a different way. Firstly, we refer to these species as born species. Since these species have no matching meta-species in the reactans to be used in to construct the product, MobsPy uses their default state (see Initial Conditions). \n",
-                "One can also perform a query for non-default characteristics."
+                "In this section, we explain how MobsPy deals with meta-species in the products that do not have an equal match in the reactants. Firstly, we refer to these species as born species, as these species have no matching meta-species in the reactants to define their state in the products.\n",
+                "Without a reactant to define its state, MobsPy chooses only to create the reaction with the default state of this meta-species. \n",
+                "\n",
+                "As a reminder, the default state is created by combining the first characteristic added to all the inheritors of a meta-species.\n",
+                "\n",
+                "Finally, queries can also be performed on the Born Species to specify the desired state. An example follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "3fa4c83e-e241-4a82-aa9b-e6c1334c9eeb",
             "metadata": {},
@@ -70,16 +74,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "819b0242-9ed9-4c17-8add-2fca1a1f5749",
             "metadata": {},
             "source": [
-                "If one wishes to change this they can use the All operator. With the All operator, all possible states of the meta-species in the product will be used to generate a reaction. Much like the previous case queries can be performed and \n",
-                "here they will act as a filter to determine the subset of all states that will be used in the product."
+                "However, if one wants to define one reaction for each state of the Born Species, the All operator is available. If a Born Species has this operator applied to it, it will result in the change from a single reaction for the default state to the one previously described. The all operator is also compatible with dot operator queries, allowing one to filter the state space.\n",
+                "An example of usage follows: "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "59ddce43-f862-4264-a70e-915c4b8a1d48",
             "metadata": {},
```

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/13_Events.ipynb` & `mobspy-2.4.4/example_models/Tutorial Notebooks/13_Events.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9443165972723264%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'Events are sudden changes to counts in the simulation "*

 * *            "happening at specific times or due to the fulfillment of certain conditions. \\n'), "*

 * *            "(3, 'For the first example, we focus only on the specific time by setting the count "*

 * *            "of a meta-species to 200 every 5 seconds. \\n'), (4, 'The event notation for "*

 * *            "time-based events lies in putting the simulation object under context with Python\\'s "*

 * *            'native "w […]*

```diff
@@ -3,15 +3,18 @@
         {
             "cell_type": "markdown",
             "id": "7a2b09cc-c5da-47d7-ba51-f492767a6518",
             "metadata": {},
             "source": [
                 "# Events\n",
                 "\n",
-                "Events are sudden changes to counts in the simulation happening at specific times or due to the fulfilement of certain conditions. In this example we set the count of the meta-species A to 200 at every 5 seconds."
+                "Events are sudden changes to counts in the simulation happening at specific times or due to the fulfillment of certain conditions. \n",
+                "For the first example, we focus only on the specific time by setting the count of a meta-species to 200 every 5 seconds. \n",
+                "The event notation for time-based events lies in putting the simulation object under context with Python's native \"with\" notation and then using the event\\_time method. \n",
+                "When the simulation is under context with Python's \"with,\" every count assignment performed will not be an initial condition but an event. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "71d02875-b3ad-4474-8d65-86ee2888fc87",
             "metadata": {},
@@ -93,25 +96,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0d21ab0d-ce99-4a71-bc79-53c9299f853f",
             "metadata": {},
             "source": [
-                "As one can see, one can assign counts to events by putting the simulation under context. \n",
-                "Once the simulation is under context every count assign to a meta-species will be assigned as an event. \n",
-                "The count assignment is equal to the one presented in the Initial Conditions with both the queries and All operator working in similar maner. The set_count operator is also accepted for events. "
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "4e3505e6-472b-40db-ab62-d5b140089a97",
-            "metadata": {},
-            "source": [
-                "Besides timed events, one has access to conditional events. Conditional events trigger once a specific logic expression has been satisfied. In the following model, we desing two meta-species, A and B with two characteristics each and we set their counts to 200 if they both go bellow 50. "
+                "The other type of event is condition-based. Condition-based events trigger when the total amount of a meta-species reaches a specific value. \n",
+                "The notation is similar to the time event by putting a simulation under context. However, the method used is called event_condition. This method also receives as an argument a logic expression constructed by using meta-species. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "3f9188eb-84a8-42bc-97c6-a6a9ca530d2d",
             "metadata": {},
@@ -155,32 +149,33 @@
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "Starting Simulator\n",
-                        "Running simulation in parallel\n",
                         "Simulation is Over\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
                     "output_type": "display_data"
                 }
             ],
             "source": [
+                "from mobspy import *\n",
+                "\n",
                 "A, B = BaseSpecies()\n",
                 "\n",
                 "A.a1, A.a2, B.b1, B.b2\n",
                 "\n",
                 "A.a1 + B.b1 >> Zero [0.01]\n",
                 "A.a2 + B.b2 >> Zero [0.02]\n",
                 "\n",
@@ -198,24 +193,28 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "194f9418-78b0-4525-9f80-52bbaa0072f5",
             "metadata": {},
             "source": [
-                "Like in the results, MobsPy automatically maps A = A.a1 + A.a2 and B = B.b1 + B.b2. Once the counts of the species in all states go bellow the defined thresholds the event trigger and set the counts back up. \n",
+                "In logic expressions, MobsPy automatically maps all states of a meta-species through a sum to evaluate their total amount (in the example, A = A.a1 + A.a2 and B = B.b1 + B.b2). If the sum of the counts of the species states satisfies the logic condition, it will trigger. The logic expressions are also compatible with the dot notation query to specify only a sum of substates of a meta-species.\n",
+                "\n",
+                "Unfortunately, logical clauses in MobsPy must be isolated in parenthesis when combined to respect Python operator precedence. As if the parenthesis were not there, Python would try to resolve the and operator '&' before the inequalities. \n",
                 "\n",
-                "Logical clauses in MobsPy must be isolated in parenthesis when combined to respect Python operator precedence other. As if the parenthesis where not there, Python would try to resolve the operator '&' (and) before the inequalities. The operator '|' symbolises or and the operator '&' simbolises and. Finally, the equality operator is not allowed as it can create compatibility issues with python. In the code bellow, there are some examples of MobsPy logical clauses."
+                "The accepted operators and operations are the following: sum of different meta-species, multiplication by constant, greater and equal (>=), smaller and equal (<=), greater (>), smaller (<), and ('&'), and or ('|'). Notice that equality is not accepted as it is not an overridable operator in Python. In that case, the user must use the combination of greater\u00a0and equal (>=), smaller and equal (<=), and the and ('&'). "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "da032cc5-b958-4aa6-aba2-2c1d2bfb5aac",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "# Perform a query \n",
                 "c1 = A.a1 <= 10 \n",
                 "# Combine clauses\n",
                 "c2 = ((A.a1 <= 10) | (B >= 5)) & (A.a2 >= 5)\n",
                 "\n",
@@ -225,34 +224,34 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e99fdd73-49b9-452e-ac6c-894371dd7d67",
             "metadata": {},
             "source": [
-                "Another aspect is to create simulations with a conditional duration by passing a logical clause. For instance, the simulation bellow runs until either A or B reach zero."
+                "Logical expressions can also create simulations with a conditional duration by setting the duration equal to one. \n",
+                "For instance, the simulation below runs until either A or B reaches zero."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "5e2fb56e-3242-4f49-bdad-40824edb06e7",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "Compiling model\n",
                         "Starting Simulator\n",
-                        "Running simulation in parallel\n",
                         "Simulation is Over\n",
                         "\u001b[91mERROR: At:             copier = getattr(x, \"__deepcopy__\", None) \n",
                         "Line number: 151 \n",
-                        "Characteristic name __deepcopy__ is not allowed. Please pick another name\u001b[0m\n"
+                        "Characteristic name __deepcopy__ in object A is not allowed. Please pick another name\u001b[0m\n"
                     ]
                 },
                 {
                     "ename": "SystemExit",
                     "evalue": "1",
                     "output_type": "error",
                     "traceback": [
@@ -266,100 +265,34 @@
                     "text": [
                         "/Users/fabriciocravo/opt/anaconda3/lib/python3.8/site-packages/IPython/core/interactiveshell.py:3445: UserWarning: To exit: use 'exit', 'quit', or Ctrl-D.\n",
                         "  warn(\"To exit: use 'exit', 'quit', or Ctrl-D.\", stacklevel=1)\n"
                     ]
                 }
             ],
             "source": [
+                "from mobspy import *\n",
+                "\n",
                 "A, B = BaseSpecies()\n",
                 "\n",
                 "A + B >> Zero [0.01]\n",
                 "\n",
                 "A(110), B(100)\n",
                 "S = Simulation(A | B)\n",
                 "S.method = 'stochastic'\n",
                 "S.duration = (A <= 0) | (B <= 0)\n",
                 "S.run()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5636f5df-f517-4623-9e08-d6ff695dcf07",
-            "metadata": {},
-            "source": [
-                "As a important note, reactions CANNOT be added as events."
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "id": "55b7ca50-bee4-4b65-9487-8bbf942db978",
             "metadata": {},
             "source": [
-                "If one wishes to desing event assignments based around the value of meta-species, one can pass strings in the count assignment under an event context. For instance, the model bellow uses the meta-species I to count the number of times A reaches zero in an windown of time:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f1685940-304f-4b05-aa31-bf4520c2d4b6",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "A, I = BaseSpecies()\n",
-                "\n",
-                "A >> Zero [1]\n",
-                "\n",
-                "A(10), I(0)\n",
-                "S = Simulation(A | I)\n",
-                "S.method = 'stochastic'\n",
-                "S.duration = 15\n",
-                "S.step_size = 0.01\n",
-                "\n",
-                "with S.event_condition(A <= 0):\n",
-                "    A(10), I(f'{I} + 1')\n",
-                "\n",
-                "print(S.compile())\n",
-                "S.run()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "6b524a60-5161-4d0a-8cdc-5e14801efeda",
-            "metadata": {},
-            "source": [
-                "Again queries can be performed inside the string assignment. If a meta-species is used under this type of assignment the resulting string will be the sum of all the states."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "3dcfa0a6-1316-4dd2-9175-3a53f6be6ce5",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "A = BaseSpecies()\n",
-                "\n",
-                "A.a1, A.a2, A.a3\n",
-                "\n",
-                "S = Simulation(A)\n",
-                "\n",
-                "A(0)\n",
-                "with S.event_time(5):\n",
-                "    All[A](f'{A} + 1')\n",
-                "    \n",
-                "print(S.compile())"
+                "As an important note, reactions CANNOT be added as events."
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "9dd8e493-c6da-42eb-b626-49b50daf6d7e",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/images/Matching_Meta.png` & `mobspy-2.4.4/example_models/Tutorial Notebooks/images/Matching_Meta.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/Tutorial Notebooks/images/vectorial_space.png` & `mobspy-2.4.4/example_models/Tutorial Notebooks/images/vectorial_space.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/AB_2CD.py` & `mobspy-2.4.4/example_models/application_models/AB_2CD.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/AND_gate.py` & `mobspy-2.4.4/example_models/application_models/AND_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/CRISPR_Oscillator.py` & `mobspy-2.4.4/example_models/application_models/CRISPR_Oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/For_The_Trees.py` & `mobspy-2.4.4/example_models/application_models/For_The_Trees.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/NOR_gate.py` & `mobspy-2.4.4/example_models/application_models/NOR_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/donor_receptor.py` & `mobspy-2.4.4/example_models/application_models/donor_receptor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/oscillator.py` & `mobspy-2.4.4/example_models/application_models/oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/positive_phage_feedback_loop.py` & `mobspy-2.4.4/example_models/application_models/positive_phage_feedback_loop.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/random_walk.py` & `mobspy-2.4.4/example_models/application_models/random_walk.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/simple_infection.py` & `mobspy-2.4.4/example_models/application_models/simple_infection.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/simple_repressor.py` & `mobspy-2.4.4/example_models/application_models/simple_repressor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/example_models/application_models/simple_rule_based_and_gate.py` & `mobspy-2.4.4/example_models/application_models/simple_rule_based_and_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/images/img.png` & `mobspy-2.4.4/images/img.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/data_handler/process_result_data.py` & `mobspy-2.4.4/mobspy/data_handler/process_result_data.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/data_handler/time_series_object.py` & `mobspy-2.4.4/mobspy/data_handler/time_series_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,33 +22,41 @@
             self.ts_model_parameters = {}
         else:
             self.ts_model_parameters = model_parameters
 
 
 class MobsPyList_of_TS:
 
+    def check_parameters_for_deepcopy(self):
+        for i, d in enumerate(self.ts_parameters):
+            for par, val in d.items():
+                if not(type(val) == int or type(val) == float or type(val) == str or type(val) == bool):
+                    self.ts_parameters[i][par] = str(val)
+
     def __init__(self, list_of_mspy_ts, model_parameter_objects=None, fres=False):
         """Creates the MobsPy timeseries object
 
             :param data_dict: (dict) resulting dictionary from simulation
             {'data': ...., 'params':....., 'models':.......}
         """
+
         self.ts_data = [dict(x.ts_data) for x in list_of_mspy_ts]
         self.ts_parameters = [dict(x.ts_parameters) for x in list_of_mspy_ts]
 
         # This lines are here to allow the object to be deepcopiable
         for ts_par in self.ts_parameters:
             if ts_par['unit_x'] is not None:
                 ts_par['unit_x'] = str(ts_par['unit_x'])
             if ts_par['unit_y'] is not None:
                 ts_par['unit_y'] = str(ts_par['unit_y'])
 
         self.ts_models = [list(x.ts_models) for x in list_of_mspy_ts]
         self.ts_model_parameters = [dict(x.ts_model_parameters) for x in list_of_mspy_ts]
 
+        self.check_parameters_for_deepcopy()
 
         if model_parameter_objects is not None:
             need_conversion_dict = set()
             for par, par_object in model_parameter_objects.items():
                 if par_object._has_units == 'T':
                     need_conversion_dict.add(par)
```

### Comparing `mobspy-2.4.3/mobspy/import_manager/lazy_import_class.py` & `mobspy-2.4.4/mobspy/import_manager/lazy_import_class.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/assignments_implementation.py` & `mobspy-2.4.4/mobspy/modules/assignments_implementation.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/class_of_meta_specie_named_any.py` & `mobspy-2.4.4/mobspy/modules/class_of_meta_specie_named_any.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/compiler.py` & `mobspy-2.4.4/mobspy/modules/compiler.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/context_related_scripts.py` & `mobspy-2.4.4/mobspy/modules/context_related_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/event_functions.py` & `mobspy-2.4.4/mobspy/modules/event_functions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/function_rate_code.py` & `mobspy-2.4.4/mobspy/modules/function_rate_code.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/logic_operator_objects.py` & `mobspy-2.4.4/mobspy/modules/logic_operator_objects.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/meta_class.py` & `mobspy-2.4.4/mobspy/modules/meta_class.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/meta_class_utils.py` & `mobspy-2.4.4/mobspy/modules/meta_class_utils.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/mobspy_expressions.py` & `mobspy-2.4.4/mobspy/modules/mobspy_expressions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/mobspy_parameters.py` & `mobspy-2.4.4/mobspy/modules/mobspy_parameters.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/order_operators.py` & `mobspy-2.4.4/mobspy/modules/order_operators.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/reaction_construction_nb.py` & `mobspy-2.4.4/mobspy/modules/reaction_construction_nb.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/set_counts_module.py` & `mobspy-2.4.4/mobspy/modules/set_counts_module.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/species_string_generator.py` & `mobspy-2.4.4/mobspy/modules/species_string_generator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/modules/unit_handler.py` & `mobspy-2.4.4/mobspy/modules/unit_handler.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/parameter_estimation_data_loader/data_loader.py` & `mobspy-2.4.4/mobspy/parameter_estimation_data_loader/data_loader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py` & `mobspy-2.4.4/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/parameter_scripts/parameter_reader.py` & `mobspy-2.4.4/mobspy/parameter_scripts/parameter_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/parameter_scripts/parametric_sweeps.py` & `mobspy-2.4.4/mobspy/parameter_scripts/parametric_sweeps.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/parameters/README.md` & `mobspy-2.4.4/mobspy/parameters/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/parameters/default_reader.py` & `mobspy-2.4.4/mobspy/parameters/default_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/parameters/example_reader.py` & `mobspy-2.4.4/mobspy/parameters/example_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/patch_scripts/basico_task_parametrization.py` & `mobspy-2.4.4/mobspy/patch_scripts/basico_task_parametrization.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/plot_params/example_plot_reader.py` & `mobspy-2.4.4/mobspy/plot_params/example_plot_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,31 +24,36 @@
         'xlabel_fontsize': 14,
         'ylabel_fontsize': 14,
         'title': 'Test_Plot',
         'title_fontsize': 16,
         'suptitle': 'Test_Sup_Title',
         'suptitle_fontsize': 18,
 
-        'annotations': ['Test_note', 0, 0],
         'pad': 1,
         'dpi': 3,
         'tight_layout': True,
         "plots": False,
         "species_to_plot": None,
         "save_to": 'example.png',
 
         "figures": [{
             "plots": [{
                 "species_to_plot": ["A"]
             }]
         }],
 
+        "x_from": [0, 1e50],
+        "y_from": [0, 1e50],
         "time_filter": [0, 100000],
+        "y_filter": [0, 1e50],
         "vertical_lines": [1, 2],
 
+        "annotations": [{"text": "S1", "coordinates": [0.54, 1e5], "fontsize": "large"},
+                        {"text": "S2", "coordinates": [0.58, 1e5], "fontsize": "large"}],
+
         # These parameters are not supported by plot_raw
         # Their only function is to alter the plot labels so please use that parameter
         # They are only listed here to avoid printing out errors during parameter checks
         "unit_x": '',
         "unit_y": '',
         "ignore_unit_label_x": True,
         "ignore_unit_label_y": True,
```

### Comparing `mobspy-2.4.3/mobspy/plot_scripts/default_plots.py` & `mobspy-2.4.4/mobspy/plot_scripts/default_plots.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/plot_scripts/hierarchical_plot.py` & `mobspy-2.4.4/mobspy/plot_scripts/hierarchical_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,14 +187,47 @@
 
                 try:
                     return params[key]
                 except (KeyError, IndexError):
                     return None
 
 
+def annotation_handling(axs, figure_index, plot_index, plot_params):
+    print()
+
+    if find_parameter(plot_params, key='annotations', index=(figure_index, plot_index)) is not None:
+        annotations = find_parameter(plot_params, key='annotations', index=(figure_index, plot_index))
+
+        if type(annotations) != list:
+            simlog.warning("On plotting annotations: Annotations must a be list with dictionaries as elements")
+            return 0
+
+        for annotation_dict in annotations:
+            argument_dict = {}
+
+            if "text" not in annotation_dict:
+                text = "Default Annotation"
+            else:
+                text = annotation_dict["text"]
+
+            if 'coordinates' not in annotation_dict:
+                coordinates = (0, 0)
+            else:
+                coordinates = annotation_dict['coordinates']
+
+            arg_list = ["textcoords", "xytext", "ha", "fontsize"]
+            for arg in arg_list:
+                if arg in annotation_dict:
+                    argument_dict[arg] = annotation_dict[arg]
+
+            axs.annotate(text, coordinates, **argument_dict)
+        else:
+            return 0
+
+
 ####################### PLOTING FUNCTIONS
 def plot_curves(data, axs, figure_index, plot_params):
     """
         This function plots the programmed curves in the assigned figure
 
         :param axs: (pyplot axe) axs to plot the data in
         :param data: (dict) data given in MobsPy format results['data']
@@ -212,14 +245,16 @@
         plot_number = 1
 
     # For all plots in the figure
     # Set all parameters and plot
     legend_flag = False
     for plot_index in range(plot_number):
 
+        annotation_handling(axs, figure_index, plot_index, plot_params)
+
         # Get the species from plot parameters
         if find_parameter(plot_params, key='species_to_plot', index=(figure_index, plot_index)) is not None:
             species = find_parameter(plot_params, key='species_to_plot', index=(figure_index, plot_index))
         else:
             simlog.error('No species found for plotting in one of the curves or figures')
 
         species = sorted([spe for spe in species])
@@ -233,14 +268,29 @@
             time_series = list(range(len(data)))
 
         if find_parameter(plot_params, key='time_filter', index=(figure_index, plot_index)) is not None:
             low, high = find_parameter(plot_params, key='time_filter', index=(figure_index, plot_index))
         else:
             low, high = None, None
 
+        if find_parameter(plot_params, key='y_filter', index=(figure_index, plot_index)) is not None:
+            low_y, high_y = find_parameter(plot_params, key='y_filter', index=(figure_index, plot_index))
+        else:
+            low_y, high_y = None, None
+
+        if find_parameter(plot_params, key='x_from', index=(figure_index, plot_index)) is not None:
+            x_start, x_finish = find_parameter(plot_params, key='x_from', index=(figure_index, plot_index))
+        else:
+            x_start, x_finish = None, None
+
+        if find_parameter(plot_params, key='y_from', index=(figure_index, plot_index)) is not None:
+            y_start, y_finish = find_parameter(plot_params, key='y_from', index=(figure_index, plot_index))
+        else:
+            y_start, y_finish = None, None
+
         for spe in species:
 
             # Get the parameters assigned to the species, if not assign empty for None returns
             if find_parameter(plot_params, key=spe, index=(figure_index, plot_index)) is not None:
                 species_characteristics = find_parameter(plot_params, key=spe, index=(figure_index, plot_index))
             else:
                 species_characteristics = {}
@@ -277,17 +327,28 @@
             for ts in time_series:
                 ts_time = data['Time'][ts]
                 if '$' not in spe:
                     ts_data = data[spe][ts]
                 else:
                     ts_data = data[ts][spe]
 
-                if low is not None or high is not None:
+                if low is not None and high is not None:
                     ts_time, ts_data = ppd.time_filter_operation(low, high, ts_time, ts_data)
 
+                if low_y is not None and high_y is not None:
+                    ts_time, ts_data = ppd.y_filter_operation(low_y, high_y, ts_time, ts_data)
+
+                if x_start is not None and x_finish is not None:
+                    ref_point = ts_data[-1]
+                    axs.plot([x_start, x_finish], [ref_point,  ref_point], alpha=0)
+
+                if y_start is not None and y_finish is not None:
+                    ref_point = ts_time[-1]
+                    axs.plot([ref_point, ref_point], [y_start, y_finish], alpha=0)
+
                 try:
                     if find_parameter(plot_params, key='fill_between', index=(figure_index, plot_index)) is not None \
                             and find_parameter(plot_params, key='fill_between', index=(figure_index, plot_index)):
                         try:
                             axs.fill_between(ts_time, ts_data[0], ts_data[1], color=curve_color,
                                              label=label)
                         except IndexError:
@@ -367,18 +428,14 @@
         if find_parameter(plot_params, 'ylabel', i) is not None:
             if find_parameter(plot_params, 'ylabel_fontsize', i) is not None:
                 figure_hash(i, axis_matrix).set_ylabel(find_parameter(plot_params, 'ylabel', i),
                                                        fontsize=plot_params['ylabel_fontsize'])
             else:
                 figure_hash(i, axis_matrix).set_ylabel(find_parameter(plot_params, 'ylabel', i))
 
-        if find_parameter(plot_params, 'annotations', i) is not None:
-            for annotations in find_parameter(plot_params, 'annotations', i):
-                figure_hash(i, axis_matrix).text(annotations[0], annotations[1], annotations[2])
-
 
 def set_global_parameters(fig, plot_params):
     """
         Sets the characteristics the plot window
 
         :param fig: (fig from pyplot subplot) Array of all axis in the grid
         :param plot_params: (dict) Plot parameters received
```

### Comparing `mobspy-2.4.3/mobspy/plot_scripts/process_plot_data.py` & `mobspy-2.4.4/mobspy/plot_scripts/process_plot_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,7 +80,27 @@
             new_data.append(d)
         elif t > high:
             break
 
     return new_time_data, new_data
 
 
+def y_filter_operation(low_y, high_y, time_data, data):
+
+    new_time_data = []
+    new_data = []
+
+    for t, d in zip(time_data, data):
+        if d < low_y:
+            continue
+        elif low_y <= d <= high_y:
+            new_time_data.append(t)
+            new_data.append(d)
+        elif d > high_y:
+            continue
+
+    return new_time_data, new_data
+
+
+
+
+
```

### Comparing `mobspy-2.4.3/mobspy/plot_scripts/statistics_calculations.py` & `mobspy-2.4.4/mobspy/plot_scripts/statistics_calculations.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/sbml_simulator/SBMLWriter.py` & `mobspy-2.4.4/mobspy/sbml_simulator/SBMLWriter.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc` & `mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc` & `mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc` & `mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/sbml_simulator/builder.py` & `mobspy-2.4.4/mobspy/sbml_simulator/builder.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/sbml_simulator/run.py` & `mobspy-2.4.4/mobspy/sbml_simulator/run.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/mobspy/simulation.py` & `mobspy-2.4.4/mobspy/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # For user imports
 from mobspy.modules.meta_class import BaseSpecies, ListSpecies, New, Zero
 from mobspy.modules.set_counts_module import set_counts
 from mobspy.modules.mobspy_parameters import ModelParameters
 from mobspy.modules.assignments_implementation import Assign
-from mobspy.modules.order_operators import All, Default
+from mobspy.modules.order_operators import All, Default, Rev
 from mobspy.modules.class_of_meta_specie_named_any import Any
 from mobspy.parameter_estimation_data_loader.parameter_estimation_scripts import basiCO_parameter_estimation
 
 # Module imports
 from mobspy.modules.meta_class_utils \
     import create_orthogonal_vector_structure as mcu_create_orthogonal_vector_structure
 from mobspy.modules.mobspy_expressions import u
@@ -750,26 +750,50 @@
         self.base_sim = self.list_of_simulations[0]
 
     def __add__(self, other):
         return SimulationComposition(self, other)
 
     def __setattr__(self, name, value):
         white_list = ['list_of_simulations', 'results', 'base_sim', 'fres']
-        multi_cast_parameters = ['simulation_method', 'method', 'volume', 'duration']
+        multi_cast_parameters = ['duration']
         broad_cast_parameters = ['level', 'rate_type', 'plot_type', 'repetitions']
+        double_cast_parameters = ['simulation_method', 'volume', 'method']
 
-        if name in multi_cast_parameters:
+        if name in double_cast_parameters:
+
+            # Broadcast if single value
+            if type(value) == str or type(value) == int or type(value) == float or isinstance(value, Quantity):
+                for sim in self:
+                    sim.__dict__['parameters'][name] = value
+            else:
+                # Multicast if list
+                try:
+                    if not len(self) == len(value):
+                        raise SystemExit
+                except:
+                    simlog.error(f'The parameter {name} was assigned non-accepted type.', stack_index=2)
+
+                for par, sim in zip(value, self):
+                    # DON'T ADD DIRECTLY to the object's dict, changes in volume, duration after compilation are
+                    # checked in the setattr method in the individual simulations
+                    if name == 'volume':
+                        sim.volume = par
+                    elif name == 'duration':
+                        sim.duration = par
+                    else:
+                        sim.__dict__['parameters'][name] = par
+
+        elif name in multi_cast_parameters:
 
             try:
                 if not len(self) == len(value):
                     raise SystemExit
             except:
-                simlog.error('For versions higher than 2.2.2, the parameters simulation_method (or method), volume, '
-                             'and duration must be assigned an iterable for each simulation when using '
-                             'the composition object', stack_index=2)
+                simlog.error('From 2.4.4 duration must be assigned to each simulation individually or a list '
+                             'with all durations must be assigned to the concatenated simulation', stack_index=2)
 
             for par, sim in zip(value, self):
                 # DON'T ADD DIRECTLY to the object's dict, changes in volume, duration after compilation are
                 # checked in the setattr method in the individual simulations
                 if name == 'volume':
                     sim.volume = par
                 elif name == 'duration':
```

### Comparing `mobspy-2.4.3/mobspy/simulation_logging/log_scripts.py` & `mobspy-2.4.4/mobspy/simulation_logging/log_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 global_simlog_level = 3
 
 def error(message, stack_index=-1):
 
     #for i in range(len(inspect.stack())):
     #    print(inspect.stack()[i].code_context[0][:-1])
     #exit()
-    
 
     if stack_index > -1:
         code_line = inspect.stack()[stack_index].code_context[0][:-1]
         line_number = inspect.stack()[stack_index].lineno
         message = f'At: {code_line} \n' + f'Line number: {line_number} \n' + message
 
     if global_simlog_level >= 0:
```

### Comparing `mobspy-2.4.3/mobspy.egg-info/PKG-INFO` & `mobspy-2.4.4/mobspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.4.3
+Version: 2.4.4
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.4.3/mobspy.egg-info/SOURCES.txt` & `mobspy-2.4.4/mobspy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -375,11 +375,12 @@
 test_tools/model_47.txt
 test_tools/model_48.txt
 test_tools/model_49.txt
 test_tools/model_5.txt
 test_tools/model_50.txt
 test_tools/model_51.txt
 test_tools/model_52.txt
+test_tools/model_53.txt
 test_tools/model_6.txt
 test_tools/model_7.txt
 test_tools/model_8.txt
 test_tools/model_9.txt
```

### Comparing `mobspy-2.4.3/setup.py` & `mobspy-2.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_plot_images/constant_tree.png` & `mobspy-2.4.4/test_plot_images/constant_tree.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_script.py` & `mobspy-2.4.4/test_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -1768,14 +1768,40 @@
         with Assign:
             A(5)
         S = Simulation(A)
         S.level = -1
         assert compare_model(S.compile(), 'test_tools/model_52.txt')
 
 
+def test_duration_with_run():
+
+    A, B = BaseSpecies()
+
+    A + B >> Zero[0.01]
+
+    A(10), B(5)
+    S = Simulation(A | B)
+    S.method = 'stochastic'
+    S.duration = (A <= 0) | (B <= 0)
+    S.run(level=-1, plot_data=False)
+    assert S.fres[B][-1] == 0
+
+
+def test_rev():
+
+    A, B, C = BaseSpecies()
+
+    Rev[A + 4*B >> C][1, 2]
+    Rev[A + 4 * B >> C][lambda r1, r2: (100-r1)*(100-r2), lambda r: r**3]
+
+    S = Simulation(A | B | C)
+    S.level = -1
+    assert compare_model(S.compile(), 'test_tools/model_53.txt')
+
+
 # This is here because pytest is slow - but this script works fine with pytest. Just make sure that the
 # python version in terminal is above 3.10
 test_list = [test_model_1, test_model_2, test_model_3, test_model_4, test_model_5, test_model_6, test_model_7,
              test_orthogonal_spaces, test_average_value, test_hybrid_sim, test_concatenated_simulation,
              test_event_type, test_reacting_species_event, test_unit_event_test, test_reaction_deactivation,
              test_double_rate, test_single_rate, test_triple_rate, test_stochastic_event_duration,
              test_logic_operator_syntax, test_stack_position, test_empty_arguments,
@@ -1795,15 +1821,15 @@
              test_parameter_operation_in_rate, test_multi_parameter_with_expression, test_double_parameters_with_units,
              test_parameters_with_units, test_convert_back_parameter, test_parameter_fit_with_units,
              test_multiple_runs_fit, test_simple_fit, test_numpy_in_expression_function, test_numpy_in_rates,
              test_numpy_in_counts, test_numpy_in_set_counts, test_multi_methods_plot, test_unit_x_conversion,
              test_Silicon_valley, test_replacing_species_name_in_expression, test_basic_assignment,
              test_illegal_unit_op_in_assignment, test_all_asgn_ops, test_no_species_in_asg, text_complex_assignments,
              text_assign_context_exit, text_even_more_complex_assignments, test_assign_context_complex,
-             test_assign_context_constant]
+             test_assign_context_constant, test_duration_with_run, test_rev]
 
 sub_test = test_list
 
 
 def perform_tests():
     any_failed = False
     for test in sub_test:
```

### Comparing `mobspy-2.4.3/test_tools/model_15.txt` & `mobspy-2.4.4/test_tools/model_15.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_19.txt` & `mobspy-2.4.4/test_tools/model_19.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_21.txt` & `mobspy-2.4.4/test_tools/model_21.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_24.txt` & `mobspy-2.4.4/test_tools/model_24.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_26.txt` & `mobspy-2.4.4/test_tools/model_26.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_3.txt` & `mobspy-2.4.4/test_tools/model_3.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_31.txt` & `mobspy-2.4.4/test_tools/model_31.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_33.txt` & `mobspy-2.4.4/test_tools/model_33.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_38.txt` & `mobspy-2.4.4/test_tools/model_38.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_39.txt` & `mobspy-2.4.4/test_tools/model_39.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_4.txt` & `mobspy-2.4.4/test_tools/model_4.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_40.txt` & `mobspy-2.4.4/test_tools/model_40.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_41.txt` & `mobspy-2.4.4/test_tools/model_41.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_45.txt` & `mobspy-2.4.4/test_tools/model_45.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_5.txt` & `mobspy-2.4.4/test_tools/model_5.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_7.txt` & `mobspy-2.4.4/test_tools/model_7.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.3/test_tools/model_9.txt` & `mobspy-2.4.4/test_tools/model_9.txt`

 * *Files identical despite different names*

