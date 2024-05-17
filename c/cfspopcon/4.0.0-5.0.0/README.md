# Comparing `tmp/cfspopcon-4.0.0.tar.gz` & `tmp/cfspopcon-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfspopcon-4.0.0.tar", max compression
+gzip compressed data, was "cfspopcon-5.0.0.tar", max compression
```

## Comparing `cfspopcon-4.0.0.tar` & `cfspopcon-5.0.0.tar`

### file list

```diff
@@ -1,87 +1,107 @@
--rw-r--r--   0        0        0     1079 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/LICENSE
--rw-r--r--   0        0        0      637 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/README.md
--rw-r--r--   0        0        0     1257 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/__init__.py
--rw-r--r--   0        0        0     3241 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/__init__.py
--rw-r--r--   0        0        0    17319 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/algorithm_class.py
--rw-r--r--   0        0        0     1849 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/beta.py
--rw-r--r--   0        0        0     2291 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/composite_algorithm.py
--rw-r--r--   0        0        0     3435 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/core_radiated_power.py
--rw-r--r--   0        0        0     4404 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/extrinsic_core_radiator.py
--rw-r--r--   0        0        0     2379 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/fusion_gain.py
--rw-r--r--   0        0        0     2031 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/geometry.py
--rw-r--r--   0        0        0     3132 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/heat_exhaust.py
--rw-r--r--   0        0        0     2258 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/ohmic_power.py
--rw-r--r--   0        0        0     3913 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/peaked_profiles.py
--rw-r--r--   0        0        0     1503 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/plasma_current_from_q_star.py
--rw-r--r--   0        0        0     3089 2023-10-30 01:06:34.334181 cfspopcon-4.0.0/cfspopcon/algorithms/power_balance_from_tau_e.py
--rw-r--r--   0        0        0     1508 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/algorithms/q_star_from_plasma_current.py
--rw-r--r--   0        0        0     4077 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/algorithms/single_functions.py
--rw-r--r--   0        0        0     3125 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/algorithms/two_point_model_fixed_fpow.py
--rw-r--r--   0        0        0     2991 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/algorithms/two_point_model_fixed_qpart.py
--rw-r--r--   0        0        0     2751 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/algorithms/two_point_model_fixed_tet.py
--rw-r--r--   0        0        0     3683 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/algorithms/use_LOC_tau_e_below_threshold.py
--rw-r--r--   0        0        0     2043 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/algorithms/zeff_and_dilution_from_impurities.py
--rw-r--r--   0        0        0      121 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/atomic_data/__init__.py
--rw-r--r--   0        0        0     3942 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/atomic_data/read_radas_data.py
--rwxr-xr-x   0        0        0     2613 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/cli.py
--rw-r--r--   0        0        0     3778 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/file_io.py
--rw-r--r--   0        0        0      962 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/Q_thermal_gain_factor.py
--rw-r--r--   0        0        0     3572 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/__init__.py
--rw-r--r--   0        0        0     1289 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/average_fuel_ion_mass.py
--rw-r--r--   0        0        0     5640 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/beta.py
--rw-r--r--   0        0        0     6174 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/confinement_regime_threshold_powers.py
--rw-r--r--   0        0        0     9746 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/current_drive.py
--rw-r--r--   0        0        0     2115 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/density_peaking.py
--rw-r--r--   0        0        0     1415 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/divertor_metrics.py
--rw-r--r--   0        0        0      240 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/energy_confinement_time_scalings/__init__.py
--rw-r--r--   0        0        0     6796 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/energy_confinement_time_scalings/tau_e_from_Wp.py
--rw-r--r--   0        0        0     7857 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/energy_confinement_time_scalings/tau_e_scalings.yaml
--rw-r--r--   0        0        0     3993 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/figures_of_merit.py
--rw-r--r--   0        0        0     9418 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/fusion_rates.py
--rw-r--r--   0        0        0     1668 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/fusion_reaction_data/__init__.py
--rw-r--r--   0        0        0     6320 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/fusion_reaction_data/reaction_energies.py
--rw-r--r--   0        0        0    10136 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/fusion_reaction_data/reaction_rate_coefficients.py
--rw-r--r--   0        0        0     1399 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/geometry.py
--rw-r--r--   0        0        0      697 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/helpers.py
--rw-r--r--   0        0        0     2352 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/impurity_effects.py
--rw-r--r--   0        0        0     2311 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/operational_limits.py
--rw-r--r--   0        0        0     1426 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/plasma_profile_data/PRF/aLT.csv
--rw-r--r--   0        0        0       89 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/plasma_profile_data/PRF/metadata.yaml
--rw-r--r--   0        0        0     1386 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/plasma_profile_data/PRF/width.csv
--rw-r--r--   0        0        0       47 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/plasma_profile_data/__init__.py
--rw-r--r--   0        0        0     7409 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/plasma_profile_data/density_and_temperature_profile_fits.py
--rw-r--r--   0        0        0     8205 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/plasma_profiles.py
--rw-r--r--   0        0        0      805 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/__init__.py
--rw-r--r--   0        0        0     5296 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/inherent.py
--rw-r--r--   0        0        0     7409 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/mavrin_coronal.py
--rw-r--r--   0        0        0    13130 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/mavrin_noncoronal.py
--rw-r--r--   0        0        0     8300 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/post_and_jensen.py
--rw-r--r--   0        0        0     2694 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/radas.py
--rw-r--r--   0        0        0     2501 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/radiated_power.py
--rw-r--r--   0        0        0      533 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/__init__.py
--rw-r--r--   0        0        0     3382 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/lambda_q.py
--rw-r--r--   0        0        0     2737 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/momentum_loss_functions.py
--rw-r--r--   0        0        0     1685 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/parallel_heat_flux_density.py
--rw-r--r--   0        0        0     1448 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/required_power_loss_fraction.py
--rw-r--r--   0        0        0     5782 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/solve_target_first_two_point_model.py
--rw-r--r--   0        0        0    10736 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/solve_two_point_model.py
--rw-r--r--   0        0        0     3603 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/target_electron_density.py
--rw-r--r--   0        0        0     3537 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/target_electron_flux.py
--rw-r--r--   0        0        0     3541 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/target_electron_temp.py
--rw-r--r--   0        0        0     2425 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/total_pressure.py
--rw-r--r--   0        0        0     1090 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/upstream_electron_temp.py
--rw-r--r--   0        0        0     3954 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/helpers.py
--rw-r--r--   0        0        0     2371 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/input_file_handling.py
--rw-r--r--   0        0        0     3522 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/named_options.py
--rw-r--r--   0        0        0      324 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/plotting/__init__.py
--rw-r--r--   0        0        0      847 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/plotting/coordinate_formatter.py
--rw-r--r--   0        0        0     6080 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/plotting/make_plot.py
--rw-r--r--   0        0        0      634 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/plotting/plot_style_handling.py
--rw-r--r--   0        0        0     2278 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/point_selection.py
--rw-r--r--   0        0        0     7243 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/transform.py
--rw-r--r--   0        0        0      806 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/unit_handling/__init__.py
--rw-r--r--   0        0        0    12157 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/unit_handling/decorator.py
--rw-r--r--   0        0        0     7606 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/unit_handling/default_units.py
--rw-r--r--   0        0        0     3311 2023-10-30 01:06:34.338181 cfspopcon-4.0.0/cfspopcon/unit_handling/setup_unit_handling.py
--rw-r--r--   0        0        0     2803 2023-10-30 01:06:34.346181 cfspopcon-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 cfspopcon-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/LICENSE
+-rw-r--r--   0        0        0     1318 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/README.md
+-rw-r--r--   0        0        0      960 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/__init__.py
+-rw-r--r--   0        0        0    20050 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/algorithm_class.py
+-rwxr-xr-x   0        0        0     2844 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/cli.py
+-rw-r--r--   0        0        0     3856 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/default_units.yaml
+-rw-r--r--   0        0        0     4389 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/file_io.py
+-rw-r--r--   0        0        0      682 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/auxillary_power/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/auxillary_power/auxillary_power.py
+-rw-r--r--   0        0        0      653 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/energy_confinement/__init__.py
+-rw-r--r--   0        0        0    10349 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/energy_confinement/energy_confinement_scalings.yaml
+-rw-r--r--   0        0        0     1262 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/energy_confinement/plasma_stored_energy.py
+-rw-r--r--   0        0        0     2240 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/energy_confinement/read_energy_confinement_scalings.py
+-rw-r--r--   0        0        0     6323 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/energy_confinement/solve_for_input_power.py
+-rw-r--r--   0        0        0     3408 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/energy_confinement/switch_confinement_scaling_on_threshold.py
+-rw-r--r--   0        0        0      776 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/fusion_power/__init__.py
+-rw-r--r--   0        0        0     1335 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/fusion_power/average_fuel_ion_mass.py
+-rw-r--r--   0        0        0    21885 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/fusion_power/fusion_data.py
+-rw-r--r--   0        0        0     2004 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/fusion_power/fusion_gain.py
+-rw-r--r--   0        0        0     5222 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/fusion_power/fusion_rates.py
+-rw-r--r--   0        0        0     1000 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/geometry/__init__.py
+-rw-r--r--   0        0        0     3306 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/geometry/analytical.py
+-rw-r--r--   0        0        0      998 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/geometry/volume_integral.py
+-rw-r--r--   0        0        0      802 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/metrics/__init__.py
+-rw-r--r--   0        0        0     6684 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/metrics/collisionality.py
+-rw-r--r--   0        0        0     1784 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/metrics/greenwald_density.py
+-rw-r--r--   0        0        0      946 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/metrics/heat_exhaust_metrics.py
+-rw-r--r--   0        0        0     1366 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/metrics/larmor_radius.py
+-rw-r--r--   0        0        0     1018 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_current/__init__.py
+-rw-r--r--   0        0        0     1791 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_current/bootstrap_fraction.py
+-rw-r--r--   0        0        0     5674 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_current/resistive_heating.py
+-rw-r--r--   0        0        0     4630 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_current/safety_factor.py
+-rw-r--r--   0        0        0      597 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_pressure/__init__.py
+-rw-r--r--   0        0        0     6696 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_pressure/beta.py
+-rw-r--r--   0        0        0      384 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_pressure/plasma_temperature.py
+-rw-r--r--   0        0        0     1308 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_pressure/pressure.py
+-rw-r--r--   0        0        0     1426 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/PRF/aLT.csv
+-rw-r--r--   0        0        0       89 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/PRF/metadata.yaml
+-rw-r--r--   0        0        0     1386 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/PRF/width.csv
+-rw-r--r--   0        0        0      586 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/__init__.py
+-rw-r--r--   0        0        0     4454 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/density_peaking.py
+-rw-r--r--   0        0        0     7458 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/numerical_profile_fits.py
+-rw-r--r--   0        0        0    12288 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/plasma_profiles.py
+-rw-r--r--   0        0        0      883 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/temperature_peaking.py
+-rw-r--r--   0        0        0     1173 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/__init__.py
+-rw-r--r--   0        0        0      486 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/basic_algorithms.py
+-rw-r--r--   0        0        0     2426 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/bremsstrahlung.py
+-rw-r--r--   0        0        0      654 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/__init__.py
+-rw-r--r--   0        0        0     7453 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/mavrin_coronal.py
+-rw-r--r--   0        0        0    13174 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/mavrin_noncoronal.py
+-rw-r--r--   0        0        0     8344 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/post_and_jensen.py
+-rw-r--r--   0        0        0     2432 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/radas.py
+-rw-r--r--   0        0        0     2518 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/radiated_power.py
+-rw-r--r--   0        0        0     3302 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/instrinsic_radiated_power_from_core.py
+-rw-r--r--   0        0        0     3754 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/synchrotron.py
+-rw-r--r--   0        0        0    17738 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/read_atomic_data.py
+-rw-r--r--   0        0        0      915 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/__init__.py
+-rw-r--r--   0        0        0     4189 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/heat_flux_density.py
+-rw-r--r--   0        0        0     3547 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/lambda_q.py
+-rw-r--r--   0        0        0      489 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/separatrix_density.py
+-rw-r--r--   0        0        0     1134 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/separatrix_electron_temp.py
+-rw-r--r--   0        0        0      529 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/__init__.py
+-rw-r--r--   0        0        0    10796 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/model.py
+-rw-r--r--   0        0        0     2739 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/momentum_loss_functions.py
+-rw-r--r--   0        0        0     1449 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/required_power_loss_fraction.py
+-rw-r--r--   0        0        0     2438 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/separatrix_pressure.py
+-rw-r--r--   0        0        0     3604 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/target_electron_density.py
+-rw-r--r--   0        0        0     3538 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/target_electron_flux.py
+-rw-r--r--   0        0        0     3542 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/target_electron_temp.py
+-rw-r--r--   0        0        0     5814 2024-05-17 13:54:23.907571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/target_first_model.py
+-rw-r--r--   0        0        0     7890 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/two_point_model_algorithms.py
+-rw-r--r--   0        0        0     1134 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/upstream_electron_temp.py
+-rw-r--r--   0        0        0      330 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/seeded_radiators/__init__.py
+-rw-r--r--   0        0        0     4757 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/seeded_radiators/core_radiator_conc.py
+-rw-r--r--   0        0        0     7550 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/seeded_radiators/edge_radiator_conc.py
+-rw-r--r--   0        0        0     1186 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/__init__.py
+-rw-r--r--   0        0        0      428 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/power_crossing_separatrix.py
+-rw-r--r--   0        0        0     3068 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/separatrix_operational_space/AUG_SepOS_reference.yml
+-rw-r--r--   0        0        0     2706 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/separatrix_operational_space/LH_transition.py
+-rw-r--r--   0        0        0     2962 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/separatrix_operational_space/MHD_limit.py
+-rw-r--r--   0        0        0      849 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/separatrix_operational_space/__init__.py
+-rw-r--r--   0        0        0     2272 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/separatrix_operational_space/density_limit.py
+-rw-r--r--   0        0        0      581 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/separatrix_operational_space/read_sepos_reference.py
+-rw-r--r--   0        0        0     6164 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/separatrix_operational_space/shared.py
+-rw-r--r--   0        0        0     4063 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/separatrix_operational_space/sustainment_power.py
+-rw-r--r--   0        0        0     4071 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/threshold_power.py
+-rw-r--r--   0        0        0      507 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/zeff_and_dilution/__init__.py
+-rw-r--r--   0        0        0     1773 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/zeff_and_dilution/impurity_charge_state.py
+-rw-r--r--   0        0        0     2931 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/formulas/zeff_and_dilution/zeff_and_dilution_from_impurities.py
+-rw-r--r--   0        0        0     3765 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/helpers.py
+-rw-r--r--   0        0        0     4060 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/input_file_handling.py
+-rw-r--r--   0        0        0     1711 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/named_options.py
+-rw-r--r--   0        0        0      320 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/plotting/__init__.py
+-rw-r--r--   0        0        0      950 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/plotting/coordinate_formatter.py
+-rw-r--r--   0        0        0      634 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/plotting/plot_style_handling.py
+-rw-r--r--   0        0        0     5993 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/plotting/plots.py
+-rw-r--r--   0        0        0      722 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/shaping_and_selection/__init__.py
+-rw-r--r--   0        0        0     2468 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/shaping_and_selection/line_selection.py
+-rw-r--r--   0        0        0     2225 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/shaping_and_selection/point_selection.py
+-rw-r--r--   0        0        0     7235 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/shaping_and_selection/transform_coords.py
+-rw-r--r--   0        0        0      963 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/unit_handling/__init__.py
+-rw-r--r--   0        0        0    12543 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/unit_handling/decorator.py
+-rw-r--r--   0        0        0     4972 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/unit_handling/default_units.py
+-rw-r--r--   0        0        0     4059 2024-05-17 13:54:23.911571 cfspopcon-5.0.0/cfspopcon/unit_handling/setup_unit_handling.py
+-rw-r--r--   0        0        0     3220 2024-05-17 13:54:23.927571 cfspopcon-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 cfspopcon-5.0.0/PKG-INFO
```

### Comparing `cfspopcon-4.0.0/LICENSE` & `cfspopcon-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfspopcon-4.0.0/cfspopcon/__init__.py` & `cfspopcon-5.0.0/cfspopcon/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,34 @@
 """Physics calculations & lumped-parameter models."""
 from importlib.metadata import metadata
 
 __version__ = metadata(__package__)["Version"]
 __author__ = metadata(__package__)["Author"]
 
-from . import algorithms, file_io, formulas, helpers, named_options, unit_handling
-from .algorithms.algorithm_class import Algorithm, CompositeAlgorithm
+from . import file_io, formulas, named_options, shaping_and_selection
+from .algorithm_class import Algorithm, CompositeAlgorithm
+from .formulas.read_atomic_data import AtomicData
 from .input_file_handling import read_case
 from .plotting import read_plot_style
-from .point_selection import find_coords_of_maximum, find_coords_of_minimum
 from .unit_handling import (
-    Quantity,
-    Unit,
     convert_to_default_units,
     convert_units,
-    default_unit,
-    magnitude,
     magnitude_in_default_units,
     set_default_units,
-    ureg,
-    wraps_ufunc,
 )
 
 # export main classes users should need as well as the option enums
 __all__ = [
-    "helpers",
-    "named_options",
-    "algorithms",
     "formulas",
-    "unit_handling",
-    "ureg",
-    "Quantity",
-    "Unit",
-    "wraps_ufunc",
+    "named_options",
     "magnitude_in_default_units",
-    "set_default_units",
-    "default_unit",
     "convert_to_default_units",
+    "set_default_units",
     "convert_units",
-    "magnitude",
     "read_case",
     "read_plot_style",
-    "find_coords_of_maximum",
-    "find_coords_of_minimum",
     "Algorithm",
     "CompositeAlgorithm",
     "file_io",
+    "AtomicData",
+    "shaping_and_selection",
 ]
```

### Comparing `cfspopcon-4.0.0/cfspopcon/algorithms/algorithm_class.py` & `cfspopcon-5.0.0/cfspopcon/algorithm_class.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 """Defines a class for different POPCON algorithms."""
 from __future__ import annotations
 
 import inspect
 from collections.abc import Callable, Sequence
 from functools import wraps
-from typing import Any, Optional, Union
+from pathlib import Path  # noqa: TCH003
+from typing import Any, ClassVar, Optional, Union
 from warnings import warn
 
 import xarray as xr
+import yaml
 
-from ..unit_handling import convert_to_default_units
+from .unit_handling import Quantity, convert_to_default_units, ureg
 
-FunctionType = Callable[..., dict[str, Any]]
+LabelledReturnFunctionType = Callable[..., dict[str, Any]]
+GenericFunctionType = Callable[..., Any]
 
 
 class Algorithm:
     """A class which handles the input and output of POPCON algorithms."""
 
-    def __init__(self, function: FunctionType, return_keys: list[str], name: Optional[str] = None):
+    instances: ClassVar[dict[str, Algorithm]] = dict()
+
+    def __init__(
+        self, function: LabelledReturnFunctionType, return_keys: list[str], name: Optional[str] = None, skip_registration: bool = False
+    ):
         """Initialise an Algorithm.
 
         Args:
             function: a callable function
             return_keys: the arguments which are returned from the function
             name: Descriptive name for algorithm
+            skip_registration: flag to skip adding the Algorithm to 'instances' (useful for testing)
         """
         self._function = function
         self._name = self._function.__name__ if name is None else name
+        key = self._name.removeprefix("run_")
+        if key in self.instances:
+            raise RuntimeError(f"Algorithm {key} has been defined multiple times.")
+        if not skip_registration:
+            self.instances[key] = self
 
         self._signature = inspect.signature(function)
         for p in self._signature.parameters.values():
             if p.kind not in (
                 inspect.Parameter.POSITIONAL_OR_KEYWORD,
                 inspect.Parameter.KEYWORD_ONLY,
                 inspect.Parameter.VAR_KEYWORD,
@@ -60,15 +73,15 @@
         return return_string
 
     def __repr__(self) -> str:
         """Return a simple string description of the Algorithm."""
         return f"Algorithm: {self._name}"
 
     @classmethod
-    def _make_run(cls, func: FunctionType) -> Callable[..., xr.Dataset]:
+    def _make_run(cls, func: LabelledReturnFunctionType) -> Callable[..., xr.Dataset]:
         """Helper to create the `run()` function with correct doc string.
 
         Args:
             func: function to be wrapped
 
         Returns: a xarray DataSet of the result
         """
@@ -77,87 +90,137 @@
         def run(**kwargs: Any) -> xr.Dataset:
             result = func(**kwargs)
             dataset = xr.Dataset(result)
             return dataset
 
         return run
 
-    def update_dataset(self, dataset: xr.Dataset, in_place: bool = False) -> Optional[xr.Dataset]:
+    def update_dataset(self, dataset: xr.Dataset, allow_overwrite: bool = True) -> xr.Dataset:
         """Retrieve inputs from passed dataset and return a new dataset combining input and output quantities.
 
-        Specifying in_place=True modifies the dataset in place (changing the input), whereas in_place=False will
-        return a copy of the dataset with the outputs appended.
-
         Args:
             dataset: input dataset
-            in_place: modify the dataset in place, otherwise return a modified dataset keeping the input unchanged.
+            allow_overwrite: if False, raise an error if trying to write a variable which is already defined in dataset
 
         Returns: modified dataset
         """
-        if not in_place:
-            dataset = dataset.copy(deep=True)
-
         input_values = {}
         for key in self.input_keys:
             if key in dataset.keys():
                 input_values[key] = dataset[key]
             elif key in self.default_keys:
                 input_values[key] = self.default_values[key]
             else:
                 sorted_dataset_keys = ", ".join(sorted(dataset.keys()))  # type:ignore[arg-type]
                 sorted_default_keys = ", ".join(sorted(self.default_keys))
-                raise KeyError(f"Key '{key}' not in dataset keys [{sorted_dataset_keys}] or default values [{sorted_default_keys}]")
+                raise KeyError(
+                    f"KeyError for {self._name}: Key '{key}' not in dataset keys [{sorted_dataset_keys}] or default values [{sorted_default_keys}]"
+                )
 
         result = self._function(**input_values)
-
-        for key, val in result.items():
-            dataset[key] = val
-
-        if not in_place:
-            return dataset
-        else:
-            return None
+        return xr.Dataset(result).merge(dataset, join="left", compat=("override" if allow_overwrite else "no_conflicts"))
 
     def __add__(self, other: Union[Algorithm, CompositeAlgorithm]) -> CompositeAlgorithm:
         """Build a CompositeAlgorithm composed of this Algorithm and another Algorithm or CompositeAlgorithm."""
         if isinstance(other, CompositeAlgorithm):
             return CompositeAlgorithm(algorithms=[self, *other.algorithms])
         else:
             return CompositeAlgorithm(algorithms=[self, other])
 
     @classmethod
     def from_single_function(
-        cls, func: Callable, return_keys: list[str], name: Optional[str] = None, skip_unit_conversion: bool = False
+        cls,
+        func: Callable,
+        return_keys: list[str],
+        name: Optional[str] = None,
+        skip_unit_conversion: bool = False,
+        skip_registration: bool = False,
     ) -> Algorithm:
         """Build an Algorithm which wraps a single function."""
 
         @wraps(func)
         def wrapped_function(**kwargs: Any) -> dict:
             result = func(**kwargs)
 
             if not isinstance(result, tuple):
                 result = (result,)
 
             result_dict = {}
             for i, key in enumerate(return_keys):
                 if skip_unit_conversion:
                     result_dict[key] = result[i]
+                elif isinstance(result[i], float):
+                    result_dict[key] = convert_to_default_units(Quantity(result[i], ureg.dimensionless), key)
                 else:
                     result_dict[key] = convert_to_default_units(result[i], key)
 
             return result_dict
 
-        return cls(wrapped_function, return_keys, name=name)
+        return cls(wrapped_function, return_keys, name=name if name is not None else func.__name__, skip_registration=skip_registration)
+
+    @classmethod
+    def register_algorithm(
+        cls, return_keys: list[str], name: Optional[str] = None, skip_unit_conversion: bool = False
+    ) -> GenericFunctionType:
+        """Decorate a function and turn it into an Algorithm. Usage: @Algorithm.register_algorithm(return_keys=["..."])."""  # noqa: D402
+
+        def function_wrapper(func: GenericFunctionType) -> GenericFunctionType:
+
+            Algorithm.from_single_function(
+                func, return_keys=return_keys, name=name if name is not None else func.__name__, skip_unit_conversion=skip_unit_conversion
+            )
+            return func
+
+        return function_wrapper
 
     def validate_inputs(
         self, configuration: Union[dict, xr.Dataset], quiet: bool = False, raise_error_on_missing_inputs: bool = False
     ) -> bool:
         """Check that all required inputs are defined, and warn if inputs are unused."""
         return _validate_inputs(self, configuration, quiet=quiet, raise_error_on_missing_inputs=raise_error_on_missing_inputs)
 
+    @classmethod
+    def write_yaml(cls, filepath: Path) -> None:
+        """Writes a file 'algorithms.yaml' documenting the available algorithms."""
+        data = dict()
+
+        for name, alg in cls.instances.items():
+            alg_data = dict()
+            alg_data["inputs"] = alg.required_input_keys
+            alg_data["optionals"] = alg.default_keys
+            alg_data["returns"] = alg.return_keys
+
+            data[name] = alg_data
+
+        yaml_text = yaml.dump(dict(sorted(data.items())))
+
+        with open(filepath, "w") as f:
+            f.write("# Autogenerated by Algorithm.write_yaml()\n\n")
+            f.write(yaml_text)
+
+    @classmethod
+    def algorithms(cls) -> list[str]:
+        """Make a list of the available algorithms."""
+        return list(cls.instances.keys())
+
+    @classmethod
+    def get_algorithm(cls, key: str) -> Algorithm:
+        """Retrieves an algorithm by name."""
+        if key not in cls.algorithms():
+            error_message = (
+                f"algorithm '{key}' not found. "
+                "If you have constructed or registered an Algorithm of this name, "
+                "make sure that it is imported in the top-level cfspopcon __init__.py. "
+                "Algorithms which have been successfully registered and imported will "
+                "appear in the algorithms.yaml file."
+            )
+            raise KeyError(error_message)
+
+        return cls.instances[key]
+
 
 class CompositeAlgorithm:
     """A class which combined multiple Algorithms into a single object which behaves like an Algorithm."""
 
     def __init__(self, algorithms: Sequence[Union[Algorithm, CompositeAlgorithm]], name: Optional[str] = None):
         """Initialise a CompositeAlgorithm, combining several other Algorithms.
 
@@ -260,53 +323,50 @@
         Will throw a warning if parameters are not used by any sub-Algorithm.
         """
         result = kwargs
 
         parameters_extra = set(kwargs) - set(self.required_input_keys)
         parameters_missing = set(self.required_input_keys) - set(kwargs)
         if parameters_missing:
-            raise TypeError(f"CompositeAlgorithm.run() missing arguments: {', '.join(parameters_missing)}")
+            needed_by: dict[str, list] = dict()
+
+            for parameter in parameters_missing:
+                needed_by[parameter] = []
+                for alg in self.algorithms:
+                    if parameter in alg.input_keys:
+                        needed_by[parameter].append(alg._name)
+
+            error_string = ", ".join(f"{key} needed by [{', '.join(val)}]" for key, val in needed_by.items())
+            raise TypeError(f"CompositeAlgorithm.run() missing arguments: {error_string}")
         if parameters_extra:
             warn(f"Not all input parameters were used. Unused parameters: [{', '.join(parameters_extra)}]", stacklevel=3)
 
         for alg in self.algorithms:
-
             alg_kwargs = {key: result[key] for key in result.keys() if key in alg.input_keys}
 
             alg_result = alg.run(**alg_kwargs)
             result.update(alg_result)  # type:ignore[arg-type]  # dict.update() doesn't like KeysView[Hashable]
 
         return xr.Dataset(result)
 
-    def update_dataset(self, dataset: xr.Dataset, in_place: bool = False) -> Optional[xr.Dataset]:
+    def update_dataset(self, dataset: xr.Dataset, allow_overwrite: bool = True) -> xr.Dataset:
         """Retrieve inputs from passed dataset and return a new dataset combining input and output quantities.
 
-        Specifying in_place=True modifies the dataset in place (changing the input), whereas in_place=False will
-        return a copy of the dataset with the outputs appended.
-
         N.b. will not throw a warning if the dataset contains unused elements.
 
         Args:
             dataset: input dataset
-            in_place: modify the dataset in place, otherwise return a modified dataset keeping the input unchanged.
+            allow_overwrite: if False, raise an error if trying to write a variable which is already defined in dataset
 
         Returns: modified dataset
         """
-        if not in_place:
-            dataset = dataset.copy(deep=True)
-
         for alg in self.algorithms:
-            # We've already used copy on the dataset, so can now call update_dataset with
-            # in_place = True for each of the algorithms.
-            alg.update_dataset(dataset, in_place=True)
+            dataset = alg.update_dataset(dataset, allow_overwrite=allow_overwrite)
 
-        if not in_place:
-            return dataset
-        else:
-            return None
+        return dataset
 
     def __add__(self, other: Union[Algorithm, CompositeAlgorithm]) -> CompositeAlgorithm:
         """Build a CompositeAlgorithm composed of this CompositeAlgorithm and another Algorithm or CompositeAlgorithm."""
         if isinstance(other, Algorithm):
             return CompositeAlgorithm(algorithms=[*self.algorithms, other])
         else:
             return CompositeAlgorithm(algorithms=[*self.algorithms, *other.algorithms])
```

### Comparing `cfspopcon-4.0.0/cfspopcon/algorithms/beta.py` & `cfspopcon-5.0.0/cfspopcon/formulas/energy_confinement/plasma_stored_energy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,34 @@
-"""Calculate toroidal, poloidal, total and normalized beta."""
-from .. import formulas
-from ..unit_handling import Unitfull, convert_to_default_units
-from .algorithm_class import Algorithm
+"""Calculate the plasma stored energy."""
+from ...algorithm_class import Algorithm
+from ...unit_handling import Unitfull, convert_units, ureg
 
-RETURN_KEYS = [
-    "beta_toroidal",
-    "beta_poloidal",
-    "beta",
-    "normalized_beta",
-]
 
-
-def run_calc_beta(
+@Algorithm.register_algorithm(return_keys=["plasma_stored_energy"])
+def calc_plasma_stored_energy(
     average_electron_density: Unitfull,
     average_electron_temp: Unitfull,
+    average_ion_density: Unitfull,
+    summed_impurity_density: Unitfull,
     average_ion_temp: Unitfull,
-    magnetic_field_on_axis: Unitfull,
-    plasma_current: Unitfull,
-    minor_radius: Unitfull,
-) -> dict[str, Unitfull]:
-    """Calculate toroidal, poloidal, total and normalized beta.
+    plasma_volume: Unitfull,
+) -> Unitfull:
+    """Calculates the plasma thermal stored energy.
 
     Args:
         average_electron_density: :term:`glossary link<average_electron_density>`
         average_electron_temp: :term:`glossary link<average_electron_temp>`
+        average_ion_density: :term:`glossary link<average_ion_density>`
+        summed_impurity_density: :term:`glossary link<summed_impurity_density>`
         average_ion_temp: :term:`glossary link<average_ion_temp>`
-        magnetic_field_on_axis: :term:`glossary link<magnetic_field_on_axis>`
-        plasma_current: :term:`glossary link<plasma_current>`
-        minor_radius: :term:`glossary link<minor_radius>`
+        plasma_volume: :term:`glossary link<plasma_volume>`
 
     Returns:
-        :term:`beta_toroidal`, :term:`beta_poloidal`, :term:`beta_total`, :term:`beta_N`
+        :term:`plasma_stored_energy`
     """
-    beta_toroidal = formulas.calc_beta_toroidal(average_electron_density, average_electron_temp, average_ion_temp, magnetic_field_on_axis)
-    beta_poloidal = formulas.calc_beta_poloidal(
-        average_electron_density, average_electron_temp, average_ion_temp, plasma_current, minor_radius
+    Wp = (
+        (3.0 / 2.0)
+        * ((average_electron_density * average_electron_temp) + ((average_ion_density + summed_impurity_density) * average_ion_temp))
+        * plasma_volume
     )
 
-    beta = formulas.calc_beta_total(beta_toroidal=beta_toroidal, beta_poloidal=beta_poloidal)
-    normalized_beta = formulas.calc_beta_normalised(beta, minor_radius, magnetic_field_on_axis, plasma_current)
-
-    local_vars = locals()
-    return {key: convert_to_default_units(local_vars[key], key) for key in RETURN_KEYS}
-
-
-calc_beta = Algorithm(
-    function=run_calc_beta,
-    return_keys=RETURN_KEYS,
-)
+    return convert_units(Wp, ureg.MJ)
```

### Comparing `cfspopcon-4.0.0/cfspopcon/algorithms/core_radiated_power.py` & `cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/instrinsic_radiated_power_from_core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """Calculate the power radiated from the confined region due to the fuel and impurity species."""
 import xarray as xr
 
-from .. import formulas, named_options
-from ..atomic_data import read_atomic_data
-from ..unit_handling import Unitfull, convert_to_default_units
-from .algorithm_class import Algorithm
+from ... import named_options
+from ...algorithm_class import Algorithm
+from ...unit_handling import Unitfull
+from .bremsstrahlung import calc_bremsstrahlung_radiation
+from .impurity_radiated_power import calc_impurity_radiated_power
+from .synchrotron import calc_synchrotron_radiation
 
-RETURN_KEYS = ["P_radiation"]
 
-
-def run_calc_core_radiated_power(
+@Algorithm.register_algorithm(return_keys=["P_radiation"])
+def calc_instrinsic_radiated_power_from_core(
     rho: Unitfull,
     electron_density_profile: Unitfull,
     electron_temp_profile: Unitfull,
     z_effective: Unitfull,
     plasma_volume: Unitfull,
     major_radius: Unitfull,
     minor_radius: Unitfull,
     magnetic_field_on_axis: Unitfull,
     separatrix_elongation: Unitfull,
     radiated_power_method: named_options.RadiationMethod,
     radiated_power_scalar: Unitfull,
     impurities: xr.DataArray,
-) -> dict[str, Unitfull]:
+    atomic_data: xr.DataArray,
+) -> Unitfull:
     """Calculate the power radiated from the confined region due to the fuel and impurity species.
 
     Args:
         rho: :term:`glossary link<rho>`
         electron_density_profile: :term:`glossary link<electron_density_profile>`
         electron_temp_profile: :term:`glossary link<electron_temp_profile>`
         z_effective: :term:`glossary link<z_effective>`
@@ -34,57 +36,43 @@
         major_radius: :term:`glossary link<major_radius>`
         minor_radius: :term:`glossary link<minor_radius>`
         magnetic_field_on_axis: :term:`glossary link<magnetic_field_on_axis>`
         separatrix_elongation: :term:`glossary link<separatrix_elongation>`
         radiated_power_method: :term:`glossary link<radiated_power_method>`
         radiated_power_scalar: :term:`glossary link<radiated_power_scalar>`
         impurities: :term:`glossary link<impurities>`
+        atomic_data: :term:`glossary link<atomic_data>`
 
     Returns:
         :term:`P_radiation`
 
     """
-    P_rad_bremsstrahlung = formulas.calc_bremsstrahlung_radiation(
-        rho, electron_density_profile, electron_temp_profile, z_effective, plasma_volume
-    )
-    P_rad_bremsstrahlung_from_hydrogen = formulas.calc_bremsstrahlung_radiation(
+    P_rad_bremsstrahlung = calc_bremsstrahlung_radiation(rho, electron_density_profile, electron_temp_profile, z_effective, plasma_volume)
+    P_rad_bremsstrahlung_from_hydrogen = calc_bremsstrahlung_radiation(
         rho, electron_density_profile, electron_temp_profile, 1.0, plasma_volume
     )
-    P_rad_synchrotron = formulas.calc_synchrotron_radiation(
+    P_rad_synchrotron = calc_synchrotron_radiation(
         rho,
         electron_density_profile,
         electron_temp_profile,
         major_radius,
         minor_radius,
         magnetic_field_on_axis,
         separatrix_elongation,
         plasma_volume,
     )
 
     # Calculate radiated power due to Bremsstrahlung, Synchrotron and impurities
     if radiated_power_method == named_options.RadiationMethod.Inherent:
-        P_radiation = radiated_power_scalar * (P_rad_bremsstrahlung + P_rad_synchrotron)
+        return radiated_power_scalar * (P_rad_bremsstrahlung + P_rad_synchrotron)
     else:
-        atomic_data = read_atomic_data()
-
-        P_rad_impurity = formulas.calc_impurity_radiated_power(
+        P_rad_impurity = calc_impurity_radiated_power(
             radiated_power_method=radiated_power_method,
             rho=rho,
             electron_temp_profile=electron_temp_profile,
             electron_density_profile=electron_density_profile,
             impurities=impurities,
             plasma_volume=plasma_volume,
-            atomic_data=atomic_data,
+            atomic_data=atomic_data.item(),
         )
 
-        P_radiation = radiated_power_scalar * (
-            P_rad_bremsstrahlung_from_hydrogen + P_rad_synchrotron + P_rad_impurity.sum(dim="dim_species")
-        )
-
-    local_vars = locals()
-    return {key: convert_to_default_units(local_vars[key], key) for key in RETURN_KEYS}
-
-
-calc_core_radiated_power = Algorithm(
-    function=run_calc_core_radiated_power,
-    return_keys=RETURN_KEYS,
-)
+        return radiated_power_scalar * (P_rad_bremsstrahlung_from_hydrogen + P_rad_synchrotron + P_rad_impurity.sum(dim="dim_species"))
```

### Comparing `cfspopcon-4.0.0/cfspopcon/algorithms/extrinsic_core_radiator.py` & `cfspopcon-5.0.0/cfspopcon/formulas/seeded_radiators/core_radiator_conc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 """Calculate the concentration and effect of a core radiator required to achieve above a defined core radiative fraction."""
 import numpy as np
 import xarray as xr
 
-from .. import formulas, named_options
-from ..atomic_data import read_atomic_data
-from ..helpers import make_impurities_array
-from ..unit_handling import Unitfull, convert_to_default_units
-from .algorithm_class import Algorithm
-
-RETURN_KEYS = [
-    "core_radiator_concentration",
-    "P_radiated_by_core_radiator",
-    "P_radiation",
-    "core_radiator_concentration",
-    "core_radiator_charge_state",
-    "zeff_change_from_core_rad",
-    "dilution_change_from_core_rad",
-    "z_effective",
-    "dilution",
-]
-
-
-def run_calc_extrinsic_core_radiator(
+from ... import named_options
+from ...algorithm_class import Algorithm
+from ...helpers import make_impurities_array
+from ...unit_handling import Unitfull
+from .. import radiated_power, zeff_and_dilution
+
+
+@Algorithm.register_algorithm(
+    return_keys=[
+        "core_radiator_concentration",
+        "P_radiated_by_core_radiator",
+        "P_radiation",
+        "core_radiator_concentration",
+        "core_radiator_charge_state",
+        "zeff_change_from_core_rad",
+        "dilution_change_from_core_rad",
+        "z_effective",
+        "dilution",
+    ]
+)
+def calc_extrinsic_core_radiator(
     minimum_core_radiated_fraction: Unitfull,
     P_in: Unitfull,
     P_radiation: Unitfull,
     average_electron_density: Unitfull,
     average_electron_temp: Unitfull,
     z_effective: Unitfull,
     dilution: Unitfull,
     rho: Unitfull,
     electron_density_profile: Unitfull,
     electron_temp_profile: Unitfull,
     plasma_volume: Unitfull,
     radiated_power_method: named_options.RadiationMethod,
     radiated_power_scalar: Unitfull,
-    core_radiator: named_options.Impurity,
-) -> dict[str, Unitfull]:
+    core_radiator: named_options.AtomicSpecies,
+    atomic_data: xr.DataArray,
+) -> tuple[Unitfull, ...]:
     """Calculate the concentration and effect of a core radiator required to achieve above a defined core radiative fraction.
 
     Args:
         minimum_core_radiated_fraction: :term:`glossary link<minimum_core_radiated_fraction>`
         P_in: :term:`glossary link<P_in>`
         P_radiation: :term:`glossary link<P_radiation>`
         average_electron_density: :term:`glossary link<average_electron_density>`
@@ -50,50 +52,56 @@
         rho: :term:`glossary link<rho>`
         electron_density_profile: :term:`glossary link<electron_density_profile>`
         electron_temp_profile: :term:`glossary link<electron_temp_profile>`
         plasma_volume: :term:`glossary link<plasma_volume>`
         radiated_power_method: :term:`glossary link<radiated_power_method>`
         radiated_power_scalar: :term:`radiated_power_scalar`
         core_radiator: :term:`glossary link<core_radiator>`
+        atomic_data: :term:`glossary link<atomic_data>`
 
     Returns:
         :term:`core_radiator_concentration`, :term:`P_radiated_by_core_radiator`, :term:`P_radiation`, :term:`core_radiator_concentration`, :term:`core_radiator_charge_state`, :term:`zeff_change_from_core_rad` :term:`dilution_change_from_core_rad`, :term:`z_effective`, :term:`dilution`
 
     """
-    atomic_data = read_atomic_data()
-
     # Force P_radiated_by_core_radiator to be >= 0.0 (core radiator cannot reduce radiated power)
     P_radiated_by_core_radiator = np.maximum(minimum_core_radiated_fraction * P_in - P_radiation, 0.0)
     P_radiation = np.maximum(minimum_core_radiated_fraction * P_in, P_radiation)
 
-    P_rad_per_core_radiator = radiated_power_scalar * formulas.calc_impurity_radiated_power(
+    P_rad_per_core_radiator = radiated_power_scalar * radiated_power.impurity_radiated_power.calc_impurity_radiated_power(
         radiated_power_method=named_options.RadiationMethod.Radas
         if radiated_power_method == named_options.RadiationMethod.Inherent
         else radiated_power_method,
         rho=rho,
         electron_temp_profile=electron_temp_profile,
         electron_density_profile=electron_density_profile,
         impurities=make_impurities_array(core_radiator, 1.0),
         plasma_volume=plasma_volume,
-        atomic_data=atomic_data,
+        atomic_data=atomic_data.item(),
     ).sum(dim="dim_species")
     core_radiator_concentration = xr.where(  # type:ignore[no-untyped-call]
         P_radiated_by_core_radiator > 0, P_radiated_by_core_radiator / P_rad_per_core_radiator, 0.0
     )
 
-    core_radiator_charge_state = formulas.calc_impurity_charge_state(
-        average_electron_density, average_electron_temp, core_radiator, atomic_data
+    core_radiator_charge_state = zeff_and_dilution.impurity_charge_state.calc_impurity_charge_state(
+        average_electron_density, average_electron_temp, core_radiator, atomic_data.item()
+    )
+    zeff_change_from_core_rad = zeff_and_dilution.zeff_and_dilution_from_impurities.calc_change_in_zeff(
+        core_radiator_charge_state, core_radiator_concentration
+    )
+    dilution_change_from_core_rad = zeff_and_dilution.zeff_and_dilution_from_impurities.calc_change_in_dilution(
+        core_radiator_charge_state, core_radiator_concentration
     )
-    zeff_change_from_core_rad = formulas.calc_change_in_zeff(core_radiator_charge_state, core_radiator_concentration)
-    dilution_change_from_core_rad = formulas.calc_change_in_dilution(core_radiator_charge_state, core_radiator_concentration)
 
     z_effective = z_effective + zeff_change_from_core_rad
     dilution = (dilution - dilution_change_from_core_rad).clip(min=0.0)
 
-    local_vars = locals()
-    return {key: convert_to_default_units(local_vars[key], key) for key in RETURN_KEYS}
-
-
-calc_extrinsic_core_radiator = Algorithm(
-    function=run_calc_extrinsic_core_radiator,
-    return_keys=RETURN_KEYS,
-)
+    return (
+        core_radiator_concentration,
+        P_radiated_by_core_radiator,
+        P_radiation,
+        core_radiator_concentration,
+        core_radiator_charge_state,
+        zeff_change_from_core_rad,
+        dilution_change_from_core_rad,
+        z_effective,
+        dilution,
+    )
```

### Comparing `cfspopcon-4.0.0/cfspopcon/algorithms/power_balance_from_tau_e.py` & `cfspopcon-5.0.0/cfspopcon/formulas/energy_confinement/switch_confinement_scaling_on_threshold.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-"""Calculate the input power required to maintain the stored energy, given a tau_e scaling."""
-from .. import formulas, named_options
-from ..unit_handling import Unitfull, convert_to_default_units
-from .algorithm_class import Algorithm
-
-RETURN_KEYS = [
-    "energy_confinement_time",
-    "P_in",
-]
+"""Switch the confinement scaling used if below a threshold power or density."""
+import xarray as xr
 
+from ...algorithm_class import Algorithm
+from ...unit_handling import Unitfull
+from .solve_for_input_power import solve_tau_e_scaling_for_input_power
 
-def run_calc_power_balance_from_tau_e(
+
+@Algorithm.register_algorithm(return_keys=["energy_confinement_time", "P_in", "SOC_LOC_ratio"])
+def switch_to_linearised_ohmic_confinement_below_threshold(
     plasma_stored_energy: Unitfull,
+    energy_confinement_time: Unitfull,
+    P_in: Unitfull,
     average_electron_density: Unitfull,
     confinement_time_scalar: Unitfull,
     plasma_current: Unitfull,
     magnetic_field_on_axis: Unitfull,
     major_radius: Unitfull,
     areal_elongation: Unitfull,
     separatrix_elongation: Unitfull,
     inverse_aspect_ratio: Unitfull,
     fuel_average_mass_number: Unitfull,
     triangularity_psi95: Unitfull,
     separatrix_triangularity: Unitfull,
     q_star: Unitfull,
-    energy_confinement_scaling: named_options.ConfinementScaling,
-) -> dict[str, Unitfull]:
-    """Calculate the input power required to maintain the stored energy, given a tau_e scaling.
+) -> tuple[Unitfull, ...]:
+    """Switch to the LOC scaling if it predicts a worse energy confinement than our selected tau_e scaling.
 
     Args:
         plasma_stored_energy: :term:`glossary link<plasma_stored_energy>`
+        energy_confinement_time: :term:`glossary link<energy_confinement_time>`
+        P_in: :term:`glossary link<P_in>`
         average_electron_density: :term:`glossary link<average_electron_density>`
         confinement_time_scalar: :term:`glossary link<confinement_time_scalar>`
         plasma_current: :term:`glossary link<plasma_current>`
         magnetic_field_on_axis: :term:`glossary link<magnetic_field_on_axis>`
         major_radius: :term:`glossary link<major_radius>`
         areal_elongation: :term:`glossary link<areal_elongation>`
         separatrix_elongation: :term:`glossary link<separatrix_elongation>`
         inverse_aspect_ratio: :term:`glossary link<inverse_aspect_ratio>`
         fuel_average_mass_number: :term:`glossary link<fuel_average_mass_number>`
         triangularity_psi95: :term:`glossary link<triangularity_psi95>`
         separatrix_triangularity: :term:`glossary link<separatrix_triangularity>`
         q_star: :term:`glossary link<q_star>`
-        energy_confinement_scaling: :term:`glossary link<energy_confinement_scaling>`
 
     Returns:
-    :term:`energy_confinement_time`, :term:`P_in`
-
+        :term:`energy_confinement_time`, :term:`P_in`, :term:`SOC_LOC_ratio`
     """
-    energy_confinement_time, P_in = formulas.calc_tau_e_and_P_in_from_scaling(
+    tau_e_LOC, P_in_LOC = solve_tau_e_scaling_for_input_power(
         confinement_time_scalar=confinement_time_scalar,
         plasma_current=plasma_current,
         magnetic_field_on_axis=magnetic_field_on_axis,
         average_electron_density=average_electron_density,
         major_radius=major_radius,
         areal_elongation=areal_elongation,
         separatrix_elongation=separatrix_elongation,
         inverse_aspect_ratio=inverse_aspect_ratio,
         fuel_average_mass_number=fuel_average_mass_number,
         triangularity_psi95=triangularity_psi95,
         separatrix_triangularity=separatrix_triangularity,
         plasma_stored_energy=plasma_stored_energy,
         q_star=q_star,
-        tau_e_scaling=energy_confinement_scaling,
+        tau_e_scaling="LOC",
     )
 
-    local_vars = locals()
-    return {key: convert_to_default_units(local_vars[key], key) for key in RETURN_KEYS}
+    # Use Linearized Ohmic Confinement if it gives worse energy confinement.
+    SOC_LOC_ratio = energy_confinement_time / tau_e_LOC
+    energy_confinement_time = xr.where(SOC_LOC_ratio > 1.0, tau_e_LOC, energy_confinement_time)  # type:ignore[no-untyped-call]
+    P_in = xr.where(SOC_LOC_ratio > 1.0, P_in_LOC, P_in)  # type:ignore[no-untyped-call]
+
+    return (energy_confinement_time, P_in, SOC_LOC_ratio)
 
 
-calc_power_balance_from_tau_e = Algorithm(
-    function=run_calc_power_balance_from_tau_e,
-    return_keys=RETURN_KEYS,
-)
+# TODO implement switch to L-mode below PLH
```

### Comparing `cfspopcon-4.0.0/cfspopcon/algorithms/zeff_and_dilution_from_impurities.py` & `cfspopcon-5.0.0/cfspopcon/formulas/zeff_and_dilution/zeff_and_dilution_from_impurities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,76 @@
 """Calculate the impact of core impurities on z_effective and dilution."""
 import xarray as xr
 
-from .. import formulas
-from ..atomic_data import read_atomic_data
-from ..unit_handling import Unitfull, convert_to_default_units
-from .algorithm_class import Algorithm
-
-RETURN_KEYS = [
-    "impurity_charge_state",
-    "z_effective",
-    "dilution",
-    "summed_impurity_density",
-    "average_ion_density",
-]
+from ...algorithm_class import Algorithm
+from ...unit_handling import Unitfull
+from .impurity_charge_state import calc_impurity_charge_state
 
 
-def run_calc_zeff_and_dilution_from_impurities(
+@Algorithm.register_algorithm(
+    return_keys=[
+        "impurity_charge_state",
+        "z_effective",
+        "dilution",
+        "summed_impurity_density",
+        "average_ion_density",
+    ]
+)
+def calc_zeff_and_dilution_due_to_impurities(
     average_electron_density: Unitfull,
     average_electron_temp: Unitfull,
     impurities: xr.DataArray,
-) -> dict[str, Unitfull]:
+    atomic_data: xr.DataArray,
+) -> tuple[Unitfull, ...]:
     """Calculate the impact of core impurities on z_effective and dilution.
 
     Args:
         average_electron_density: :term:`glossary link<average_electron_density>`
         average_electron_temp: :term:`glossary link<average_electron_temp>`
         impurities: :term:`glossary link<impurities>`
+        atomic_data: :term:`glossary link<atomic_data>`
 
     Returns:
         :term:`impurity_charge_state`, :term:`z_effective`, :term:`dilution`, :term:`summed_impurity_density`, :term:`average_ion_density`
 
     """
     starting_zeff = 1.0
     starting_dilution = 1.0
 
-    atomic_data = read_atomic_data()
-
-    impurity_charge_state = formulas.calc_impurity_charge_state(
-        average_electron_density, average_electron_temp, impurities.dim_species, atomic_data
+    impurity_charge_state = calc_impurity_charge_state(
+        average_electron_density, average_electron_temp, impurities.dim_species, atomic_data.item()
     )
-    change_in_zeff = formulas.calc_change_in_zeff(impurity_charge_state, impurities)
-    change_in_dilution = formulas.calc_change_in_dilution(impurity_charge_state, impurities)
+    change_in_zeff = calc_change_in_zeff(impurity_charge_state, impurities)
+    change_in_dilution = calc_change_in_dilution(impurity_charge_state, impurities)
 
     z_effective = starting_zeff + change_in_zeff.sum(dim="dim_species")
     dilution = starting_dilution - change_in_dilution.sum(dim="dim_species")
     summed_impurity_density = impurities.sum(dim="dim_species") * average_electron_density
     average_ion_density = dilution * average_electron_density
 
-    local_vars = locals()
-    return {key: convert_to_default_units(local_vars[key], key) for key in RETURN_KEYS}
+    return (impurity_charge_state, z_effective, dilution, summed_impurity_density, average_ion_density)
 
 
-calc_zeff_and_dilution_from_impurities = Algorithm(
-    function=run_calc_zeff_and_dilution_from_impurities,
-    return_keys=RETURN_KEYS,
-)
+def calc_change_in_zeff(impurity_charge_state: float, impurity_concentration: xr.DataArray) -> xr.DataArray:
+    """Calculate the change in the effective charge due to the specified impurities.
+
+    Args:
+        impurity_charge_state: [~] :term:`glossary link<impurity_charge_state>`
+        impurity_concentration: [~] :term:`glossary link<impurity_concentration>`
+
+    Returns:
+        change in zeff [~]
+    """
+    return impurity_charge_state * (impurity_charge_state - 1.0) * impurity_concentration
+
+
+def calc_change_in_dilution(impurity_charge_state: float, impurity_concentration: xr.DataArray) -> xr.DataArray:
+    """Calculate the change in n_fuel/n_e due to the specified impurities.
+
+    Args:
+        impurity_charge_state: [~] :term:`glossary link<impurity_charge_state>`
+        impurity_concentration: [~] :term:`glossary link<impurity_concentration>`
+
+    Returns:
+        change in dilution [~]
+    """
+    return impurity_charge_state * impurity_concentration
```

### Comparing `cfspopcon-4.0.0/cfspopcon/cli.py` & `cfspopcon-5.0.0/cfspopcon/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,80 @@
 #!.venv/bin/python
 # Run this script from the repository directory.
 """CLI for cfspopcon."""
-import sys
 from pathlib import Path
 
 import click
-import matplotlib.pyplot as plt  # type:ignore[import]
+import matplotlib.pyplot as plt
 import xarray as xr
-from ipdb import launch_ipdb_on_exception  # type:ignore[import]
+from ipdb import launch_ipdb_on_exception  # type:ignore[import-untyped]
 
 from cfspopcon import file_io
 from cfspopcon.input_file_handling import read_case
 from cfspopcon.plotting import make_plot, read_plot_style
 
 
 @click.command()
 @click.argument("case", type=click.Path(exists=True))
-@click.option(
-    "--plots",
-    "-p",
-    type=click.Path(exists=True),
-    multiple=True,
-)
-@click.option("--show", is_flag=True, help="Display an interactive figure of the result")
-@click.option("--debug", is_flag=True, help="Enable the ipdb exception catcher")
-def run_popcon_cli(case: str, plots: tuple[str], show: bool, debug: bool) -> None:
+@click.option("--dict", "-d", "kwargs", type=(str, str), multiple=True, help="Command-line arguments, takes precedence over config.")
+@click.option("--show", is_flag=True, help="Display an interactive figure of the result.")
+@click.option("--debug", is_flag=True, help="Enable the ipdb exception catcher.")
+def run_popcon_cli(case: str, show: bool, debug: bool, kwargs: tuple[tuple[str, str]]) -> None:
     """Run POPCON from the command line.
 
     This function uses "Click" to develop the command line interface. You can execute it using
     poetry run python cfspopcon/cli.py --help
-
-    You can specify a set of plots to create by specifying a plot style file after `-p` on the command-line. Multiple entries are supported.
     """
-    if show and not plots:
-        print(f"Speficied show={show}, but did not specify a plot style, see --plots!")
-        sys.exit(1)
+    cli_args: dict[str, str] = dict(kwargs)
 
     if not debug:
-        run_popcon(case, plots, show)
+        run_popcon(case, show, cli_args)
     else:
         with launch_ipdb_on_exception():
-            run_popcon(case, plots, show)
+            run_popcon(case, show, cli_args)
+
+
+@click.command()
+@click.option("-o", "--output", default="./popcon_algorithms.yaml", type=click.Path(exists=False))
+def write_algorithms_yaml(output: str) -> None:
+    """Write all available algorithms to a yaml helper file."""
+    from cfspopcon import Algorithm
+
+    Algorithm.write_yaml(Path(output))
 
 
-def run_popcon(case: str, plots: tuple[str], show: bool) -> None:
+def run_popcon(case: str, show: bool, cli_args: dict[str, str]) -> None:
     """Run popcon case.
 
     Args:
         case: specify case to run (corresponding to a case in cases)
-        plots: specify which plots to make (corresponding to a plot_style in plot_styles)
         show: show the resulting plots
+        cli_args: command-line arguments, takes precedence over config.
     """
-    input_parameters, algorithm, points = read_case(case)
+    input_parameters, algorithm, points, plots = read_case(case, cli_args)
 
     dataset = xr.Dataset(input_parameters)
 
     algorithm.validate_inputs(dataset)
-    algorithm.update_dataset(dataset, in_place=True)
+    dataset = algorithm.update_dataset(dataset)
 
     output_dir = Path(case) / "output" if Path(case).is_dir() else Path(case).parent / "output"
     output_dir.mkdir(exist_ok=True)
 
     file_io.write_dataset_to_netcdf(dataset, filepath=output_dir / "dataset.nc")
 
-    for point, point_params in points.items():
-        file_io.write_point_to_file(dataset, point, point_params, output_dir=output_dir)
+    if points is not None:
+        for point, point_params in points.items():
+            file_io.write_point_to_file(dataset, point, point_params, output_dir=output_dir)
 
     # Plot the results
-    for plot_style in plots:
-        make_plot(dataset, read_plot_style(plot_style), points, title=input_parameters.get("plot_title", "POPCON"), output_dir=output_dir)
+    if plots is not None:
+        for plot_name, plot_style in plots.items():
+            print(f"Plotting {plot_name}")
+            make_plot(dataset, read_plot_style(plot_style), points, title=plot_name, output_dir=output_dir, save_name=plot_style.stem)
 
     print("Done")
     if show:
         plt.show()
 
 
 if __name__ == "__main__":
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/beta.py` & `cfspopcon-5.0.0/cfspopcon/formulas/plasma_pressure/beta.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Calculate the ratio of magnetic to plasma (kinetic) pressure."""
 import numpy as np
 
-from ..unit_handling import Quantity, Unitfull, convert_units, ureg
+from ...algorithm_class import Algorithm
+from ...unit_handling import Quantity, Unitfull, convert_units, ureg, wraps_ufunc
 
 
 def _calc_beta_general(
     average_electron_density: Unitfull, average_electron_temp: Unitfull, average_ion_temp: Unitfull, magnetic_field: Unitfull
 ) -> Unitfull:
     """Calculate the average ratio of the plasma pressure to the magnetic pressure due to a magnetic_field.
 
@@ -14,15 +15,15 @@
     The unit_conversion_factor comes from cancelling the units to get a dimensionless quantity
 
         >>> from pint import Quantity
         >>> n = Quantity(1e19, "m^-3")
         >>> T = Quantity(1, "keV")
         >>> B = Quantity(1, "T")
         >>> mu_0 = Quantity(1, "mu_0")
-        >>> ((2*mu_0 * n * T / (B**2)).to('').units
+        >>> (2*mu_0 * n * T / (B**2)).to('').units
         <Unit('dimensionless')>
 
     Args:
         average_electron_density: [1e19 m^-3] :term:`glossary link<average_electron_density>`
         average_electron_temp: [keV] :term:`glossary link<average_electron_temp>`
         average_ion_temp: [keV] :term:`glossary link<average_ion_temp>`
         magnetic_field: magnetic field generating magnetic pressure [T]
@@ -33,14 +34,15 @@
     mu_0 = Quantity(1, "mu_0")
     # to make the result dimensionless
     unit_conversion_factor = 2 * mu_0
     ret = unit_conversion_factor * (average_electron_density * (average_electron_temp + average_ion_temp)) / (magnetic_field**2)
     return convert_units(ret, ureg.dimensionless)
 
 
+@Algorithm.register_algorithm(return_keys=["beta_toroidal"])
 def calc_beta_toroidal(
     average_electron_density: Unitfull, average_electron_temp: Unitfull, average_ion_temp: Unitfull, magnetic_field_on_axis: Unitfull
 ) -> Unitfull:
     """Calculate the average ratio of the plasma pressure to the magnetic pressure due to the toroidal field.
 
     Also called beta_external, since the toroidal field is generated by external toroidal field coils.
     Using equation 11.58 from Freidberg, "Plasma Physics and Fusion Energy" :cite:`freidberg_plasma_2007`
@@ -53,14 +55,15 @@
 
     Returns:
          :term:`beta_toroidal` [~]
     """
     return _calc_beta_general(average_electron_density, average_electron_temp, average_ion_temp, magnetic_field=magnetic_field_on_axis)
 
 
+@Algorithm.register_algorithm(return_keys=["beta_poloidal"])
 def calc_beta_poloidal(
     average_electron_density: Unitfull,
     average_electron_temp: Unitfull,
     average_ion_temp: Unitfull,
     plasma_current: Unitfull,
     minor_radius: Unitfull,
 ) -> Unitfull:
@@ -95,41 +98,62 @@
     # to ensure the final result is in units of tesla
     units_conversion_factor = mu_0 / (2 * np.pi)
     B_pol = units_conversion_factor * plasma_current / minor_radius
 
     return _calc_beta_general(average_electron_density, average_electron_temp, average_ion_temp, magnetic_field=B_pol)
 
 
+@Algorithm.register_algorithm(return_keys=["beta"])
 def calc_beta_total(beta_toroidal: Unitfull, beta_poloidal: Unitfull) -> Unitfull:
     """Calculate the total beta from the toroidal and poloidal betas.
 
     Using equation 11.59 from Freidberg, "Plasma Physics and Fusion Energy" :cite:`freidberg_plasma_2007`
 
     Args:
         beta_toroidal: [~] :term:`glossary link<beta_toroidal>`
         beta_poloidal: [~] :term:`glossary link<beta_poloidal>`
 
     Returns:
-         :term:`beta_total` [~]
+         :term:`beta` [~]
     """
     return 1.0 / (1.0 / beta_toroidal + 1.0 / beta_poloidal)
 
 
-def calc_beta_normalised(beta: Unitfull, minor_radius: Unitfull, magnetic_field_on_axis: Unitfull, plasma_current: Unitfull) -> Unitfull:
+@Algorithm.register_algorithm(return_keys=["normalized_beta"])
+def calc_beta_normalized(beta: Unitfull, minor_radius: Unitfull, magnetic_field_on_axis: Unitfull, plasma_current: Unitfull) -> Unitfull:
     """Normalize beta to stability (Troyon) parameters.
 
     See section 6.18 in Wesson :cite:`wesson_tokamaks_2011`.
 
     Args:
         beta: plasma pressure normalized against toroidal B-on-axis [%]
         minor_radius: [m] :term:`glossary link<minor_radius>`
         magnetic_field_on_axis: [T] :term:`glossary link<magnetic_field_on_axis>`
         plasma_current: [MA] :term:`glossary link<plasma_current>`
 
     Returns:
-         :term:`beta_N`
+         :term:`normalized_beta`
     """
     normalisation = plasma_current / (minor_radius * magnetic_field_on_axis)
 
     beta_N = beta / normalisation
 
     return beta_N
+
+
+@Algorithm.register_algorithm(return_keys=["troyon_max_beta"])
+@wraps_ufunc(
+    return_units=dict(troyon_max_beta=ureg.percent),
+    input_units=dict(minor_radius=ureg.m, magnetic_field_on_axis=ureg.T, plasma_current=ureg.MA),
+)
+def calc_troyon_limit(minor_radius: float, magnetic_field_on_axis: float, plasma_current: float) -> float:
+    """Calculate the maximum value for beta, according to the Troyon limit.
+
+    Args:
+        minor_radius: [m] :term:`glossary link<minor_radius>`
+        magnetic_field_on_axis: [T] :term:`glossary link<magnetic_field_on_axis>`
+        plasma_current: [MA] :term:`glossary link<plasma_current>`
+
+    Returns:
+         troyon_max_beta [~]
+    """
+    return 2.8 * plasma_current / (minor_radius * magnetic_field_on_axis)
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/confinement_regime_threshold_powers.py` & `cfspopcon-5.0.0/cfspopcon/formulas/separatrix_conditions/threshold_power.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,153 +1,99 @@
-"""Threshold powers required to enter improved confinement regimes."""
-from ..named_options import ConfinementScaling
-from ..unit_handling import ureg, wraps_ufunc
+"""Calculate the threshold values for the power crossing the separatrix."""
 
-
-def _calc_Martin_LH_threshold(
-    magnetic_field_on_axis: float, surface_area: float, fuel_average_mass_number: float, electron_density_profile: float
-) -> float:
-    """See below."""
-    _DEUTERIUM_MASS_NUMBER = 2.0
-
-    return float(0.0488 * ((electron_density_profile / 10.0) ** 0.717) * (magnetic_field_on_axis**0.803) * (surface_area**0.941)) * (
-        _DEUTERIUM_MASS_NUMBER / fuel_average_mass_number
-    )
+from ...algorithm_class import Algorithm
+from ...unit_handling import ureg, wraps_ufunc
 
 
+@Algorithm.register_algorithm(return_keys=["P_LH_thresh"])
 @wraps_ufunc(
     return_units=dict(P_LH_thresh=ureg.MW),
     input_units=dict(
         plasma_current=ureg.MA,
         magnetic_field_on_axis=ureg.T,
         minor_radius=ureg.m,
         major_radius=ureg.m,
         surface_area=ureg.m**2,
         fuel_average_mass_number=ureg.amu,
         average_electron_density=ureg.n19,
-        scale=ureg.dimensionless,
+        confinement_threshold_scalar=ureg.dimensionless,
     ),
 )
 def calc_LH_transition_threshold_power(
     plasma_current: float,
     magnetic_field_on_axis: float,
     minor_radius: float,
     major_radius: float,
     surface_area: float,
     fuel_average_mass_number: float,
     average_electron_density: float,
-    scale: float = 1.0,
+    confinement_threshold_scalar: float = 1.0,
 ) -> float:
     """Calculate the threshold power (crossing the separatrix) to transition into H-mode.
 
     From Martin NF 2008 Scaling, with mass correction :cite:`martin_power_2008`
     Added in low density branch from Ryter 2014 :cite:`Ryter_2014`
 
     Args:
         plasma_current: [MA] :term:`glossary link<plasma_current>`
         magnetic_field_on_axis: [T] :term:`glossary link<magnetic_field_on_axis>`
         minor_radius: [m] :term:`glossary link<minor_radius>`
         major_radius: [m] :term:`glossary link<major_radius>`
         surface_area: [m^2] :term:`glossary link<surface_area>`
         fuel_average_mass_number: [amu] :term:`glossary link<fuel_average_mass_number>`
         average_electron_density: [1e19 m^-3] :term:`glossary link<average_electron_density>`
-        scale: (optional) scaling factor for P_LH adjustment studies [~]
+        confinement_threshold_scalar: [~] :term:`glossary link<confinement_threshold_scalar>`
 
     Returns:
          :term:`P_LH_thresh` [MW]
     """
+
+    def _calc_Martin_LH_threshold(electron_density: float) -> float:
+        _DEUTERIUM_MASS_NUMBER = 2.0
+
+        return float(0.0488 * ((electron_density / 10.0) ** 0.717) * (magnetic_field_on_axis**0.803) * (surface_area**0.941)) * (
+            _DEUTERIUM_MASS_NUMBER / fuel_average_mass_number
+        )
+
     neMin19 = (
         0.7 * (plasma_current**0.34) * (magnetic_field_on_axis**0.62) * (minor_radius**-0.95) * ((major_radius / minor_radius) ** 0.4)
     )
 
     if average_electron_density < neMin19:
-        P_LH_thresh = _calc_Martin_LH_threshold(
-            magnetic_field_on_axis, surface_area, fuel_average_mass_number, electron_density_profile=neMin19
-        )
-        return float(P_LH_thresh * (neMin19 / average_electron_density) ** 2.0) * scale
+        P_LH_thresh = _calc_Martin_LH_threshold(electron_density=neMin19)
+        return float(P_LH_thresh * (neMin19 / average_electron_density) ** 2.0) * confinement_threshold_scalar
     else:
-        P_LH_thresh = _calc_Martin_LH_threshold(
-            magnetic_field_on_axis, surface_area, fuel_average_mass_number, electron_density_profile=average_electron_density
-        )
-        return P_LH_thresh * scale
+        P_LH_thresh = _calc_Martin_LH_threshold(electron_density=average_electron_density)
+        return P_LH_thresh * confinement_threshold_scalar
+
 
+calc_ratio_P_LH = Algorithm.from_single_function(
+    func=lambda P_sol, P_LH_thresh: P_sol / P_LH_thresh, return_keys=["ratio_of_P_SOL_to_P_LH"], name="calc_ratio_P_LH"
+)
 
+
+@Algorithm.register_algorithm(return_keys=["P_LI_thresh"])
 @wraps_ufunc(
     return_units=dict(P_LI_thresh=ureg.MW),
-    input_units=dict(plasma_current=ureg.MA, average_electron_density=ureg.n19, scale=ureg.dimensionless),
+    input_units=dict(plasma_current=ureg.MA, average_electron_density=ureg.n19, confinement_threshold_scalar=ureg.dimensionless),
 )
-def calc_LI_transition_threshold_power(plasma_current: float, average_electron_density: float, scale: float = 1.0) -> float:
+def calc_LI_transition_threshold_power(
+    plasma_current: float, average_electron_density: float, confinement_threshold_scalar: float = 1.0
+) -> float:
     """Calculate the threshold power (crossing the separatrix) to transition into I-mode.
 
     Note: uses scaling described in Fig 5 of ref :cite:`hubbard_threshold_2012`
 
     Args:
         plasma_current: [MA] :term:`glossary link<plasma_current>`
         average_electron_density: [1e19 m^-3] :term:`glossary link<average_electron_density>`
-        scale: (optional) scaling factor for P_LI adjustment studies [~]
+        confinement_threshold_scalar: [~] :term:`glossary link<confinement_threshold_scalar>`
 
     Returns:
         :term:`P_LI_thresh` [MW]
     """
-    return float(2.11 * plasma_current**0.94 * ((average_electron_density / 10.0) ** 0.65)) * scale
+    return float(2.11 * plasma_current**0.94 * ((average_electron_density / 10.0) ** 0.65)) * confinement_threshold_scalar
 
 
-@wraps_ufunc(
-    return_units=dict(P_LH_thresh=ureg.MW),
-    input_units=dict(
-        energy_confinement_scaling=None,
-        plasma_current=ureg.MA,
-        magnetic_field_on_axis=ureg.T,
-        minor_radius=ureg.m,
-        major_radius=ureg.m,
-        surface_area=ureg.m**2,
-        fuel_average_mass_number=ureg.amu,
-        average_electron_density=ureg.n19,
-        confinement_threshold_scalar=ureg.dimensionless,
-    ),
+calc_ratio_P_LI = Algorithm.from_single_function(
+    func=lambda P_sol, P_LI_thresh: P_sol / P_LI_thresh, return_keys=["ratio_of_P_SOL_to_P_LI"], name="calc_ratio_P_LI"
 )
-def calc_confinement_transition_threshold_power(
-    energy_confinement_scaling: ConfinementScaling,
-    plasma_current: float,
-    magnetic_field_on_axis: float,
-    minor_radius: float,
-    major_radius: float,
-    surface_area: float,
-    fuel_average_mass_number: float,
-    average_electron_density: float,
-    confinement_threshold_scalar: float = 1.0,
-) -> float:
-    """Calculate the threshold power (crossing the separatrix) to transition into an improved confinement mode.
-
-    Args:
-        energy_confinement_scaling: [] :term:`glossary link<energy_confinement_scaling>`
-        plasma_current: [MA] :term:`glossary link<plasma_current>`
-        magnetic_field_on_axis: [T] :term:`glossary link<magnetic_field_on_axis>`
-        minor_radius: [m] :term:`glossary link<minor_radius>`
-        major_radius: [m] :term:`glossary link<major_radius>`
-        surface_area: [m^2] :term:`glossary link<surface_area>`
-        fuel_average_mass_number: [amu] :term:`glossary link<fuel_average_mass_number>`
-        average_electron_density: [1e19 m^-3] :term:`glossary link<average_electron_density>`
-        confinement_threshold_scalar: (optional) scaling factor for P_LH adjustment studies [~]
-
-    Returns:
-        :term:`P_LH_thresh` [MW]
-    """
-    if energy_confinement_scaling not in [ConfinementScaling.LOC, ConfinementScaling.IModey2]:
-        P_LH_thresh = calc_LH_transition_threshold_power.__wrapped__(
-            plasma_current,
-            magnetic_field_on_axis,
-            minor_radius,
-            major_radius,
-            surface_area,
-            fuel_average_mass_number,
-            average_electron_density,
-            scale=confinement_threshold_scalar,
-        )
-    elif energy_confinement_scaling == ConfinementScaling.IModey2:
-        P_LH_thresh = calc_LI_transition_threshold_power.__wrapped__(
-            plasma_current, average_electron_density, scale=confinement_threshold_scalar
-        )
-    else:
-        raise ValueError("Encountered unhandled confinement time scaling.")
-
-    return float(P_LH_thresh)
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/energy_confinement_time_scalings/tau_e_from_Wp.py` & `cfspopcon-5.0.0/cfspopcon/formulas/energy_confinement/solve_for_input_power.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-"""Calculate tau_e and P_in from a tau_e scaling and the stored energy."""
-from pathlib import Path
-
+"""Rearrange a tau_e scaling to give a value for the input power, given the stored energy."""
 import numpy as np
-import yaml
 
-from ...named_options import ConfinementScaling
+from ...algorithm_class import Algorithm
 from ...unit_handling import ureg, wraps_ufunc
-
-# Preload the scalings (instead of doing fileio in loop)
-with open(Path(__file__).parent / "tau_e_scalings.yaml") as f:
-    TAU_E_SCALINGS = yaml.safe_load(f)
+from .read_energy_confinement_scalings import ConfinementScaling
 
 
+@Algorithm.register_algorithm(return_keys=["energy_confinement_time", "P_in"])
 @wraps_ufunc(
     return_units=dict(tau_e=ureg.s, P_tau=ureg.MW),
     input_units=dict(
         confinement_time_scalar=ureg.dimensionless,
         plasma_current=ureg.MA,
         magnetic_field_on_axis=ureg.T,
         average_electron_density=ureg.n19,
@@ -28,29 +23,29 @@
         separatrix_triangularity=ureg.dimensionless,
         plasma_stored_energy=ureg.MJ,
         q_star=ureg.dimensionless,
         tau_e_scaling=None,
     ),
     output_core_dims=[(), ()],
 )
-def calc_tau_e_and_P_in_from_scaling(
+def solve_tau_e_scaling_for_input_power(
     confinement_time_scalar: float,
     plasma_current: float,
     magnetic_field_on_axis: float,
     average_electron_density: float,
     major_radius: float,
     areal_elongation: float,
     separatrix_elongation: float,
     inverse_aspect_ratio: float,
     fuel_average_mass_number: float,
     triangularity_psi95: float,
     separatrix_triangularity: float,
     plasma_stored_energy: float,
     q_star: float,
-    tau_e_scaling: ConfinementScaling,
+    tau_e_scaling: str,
 ) -> tuple[float, float]:
     r"""Calculate energy confinement time and input power from a tau_E scaling.
 
     The energy confinement time can generally be written as
 
     .. math::
         \tau_e = H \cdot C \cdot P_{\tau}^{\alpha_P}
@@ -89,16 +84,17 @@
 
     However, it is also possible that the core radiated power is subtracted when calculating :math:`\tau_e`
     [Freidberg definition of :math:`W_p`], giving
 
     .. math::
         P_{\tau} = P_{ohmic} + P_{\alpha} + P_{aux} - P_{rad} = P_{loss} = P_{SOL}
 
-    If you are using a scaling where this is the case, set ``tau_e_scaling_uses_P_in=False``.
-    Then, the returned value should be interpreted as :math:`P_{SOL}`.
+    Then, the returned value should be interpreted as :math:`P_{SOL}`. We currently don't allow this case, since the
+    general consensus is that the radiated power has not been consistently removed from scaling relationship. However,
+    if you want to explore the effect of changing this assumption, you can implement a new feature.
 
     N.b. there are two more possible cases, where different powers are used in the two :math:`\tau_e` scalings.
     We don't allow these cases, since 1) experiments generally pick a consistent definition for :math:`P`
     and 2) this results in an equation for :math:`P` which cannot be solved analytically.
 
     Args:
         confinement_time_scalar: [~] confinement scaling factor
@@ -113,57 +109,34 @@
         triangularity_psi95: [~] :term:`glossary link<triangularity_psi95>`
         separatrix_triangularity: [~] :term:`glossary link<separatrix_triangularity>`
         plasma_stored_energy: [MJ] :term:`glossary link<plasma_stored_energy>`
         q_star: [~] :term:`glossary link<q_star>`
         tau_e_scaling: [] :term:`glossary link<tau_e_scaling>`
 
     Returns:
-        :term:`energy_confinement_time` [s], :term:`P_in` if tau_e_scaling_uses_P_in=False, else :term:`P_SOL` [MW]
+        :term:`energy_confinement_time` [s], :term:`P_in` [MW]
     """
-    scaling = TAU_E_SCALINGS[tau_e_scaling.name]
+    scaling = ConfinementScaling.instances[tau_e_scaling]
 
     gamma = (
         confinement_time_scalar
-        * scaling["params"]["C"]
-        * plasma_current ** scaling["params"]["a_I"]
-        * magnetic_field_on_axis ** scaling["params"]["a_B"]
-        * average_electron_density ** scaling["params"]["a_n"]
-        * major_radius ** scaling["params"]["a_R"]
-        * areal_elongation ** scaling["params"]["a_ka"]
-        * separatrix_elongation ** scaling["params"]["a_ks"]
-        * inverse_aspect_ratio ** scaling["params"]["a_e"]
-        * fuel_average_mass_number ** scaling["params"]["a_A"]
-        * (1.0 + np.mean([triangularity_psi95, separatrix_triangularity])) ** scaling["params"]["a_d"]
-        * q_star ** scaling["params"]["a_q"]
+        * scaling.constant
+        * plasma_current**scaling.plasma_current_alpha
+        * magnetic_field_on_axis**scaling.field_on_axis_alpha
+        * average_electron_density**scaling.average_density_alpha
+        * major_radius**scaling.major_radius_alpha
+        * areal_elongation**scaling.areal_elongation_alpha
+        * separatrix_elongation**scaling.separatrix_elongation_alpha
+        * inverse_aspect_ratio**scaling.inverse_aspect_ratio_alpha
+        * fuel_average_mass_number**scaling.mass_ratio_alpha
+        * (1.0 + np.mean([triangularity_psi95, separatrix_triangularity])) ** scaling.triangularity_alpha
+        * q_star**scaling.qstar_alpha
     )
 
     if gamma > 0.0:
-        P_tau = (plasma_stored_energy / gamma) ** (1.0 / (1.0 + scaling["params"]["a_P"]))
+        P_tau = (plasma_stored_energy / gamma) ** (1.0 / (1.0 + scaling.input_power_alpha))
     else:
         P_tau = np.inf
 
     tau_E = plasma_stored_energy / P_tau
 
-    return float(tau_E), float(P_tau)
-
-
-def load_metadata(dataset: str) -> dict[str, str]:
-    """Load dataset metadata from YAML file.
-
-    Args:
-        dataset: name of scaling in ./energy_confinement_time.yaml
-
-    Returns:
-        Metadata
-    """
-    metadata: dict[str, str] = TAU_E_SCALINGS[dataset]["metadata"]
-    return metadata
-
-
-def get_datasets() -> list[str]:
-    """Get a list of names of valid datasets.
-
-    Returns:
-        List of names of valid datasets
-    """
-    datasets: list[str] = list(TAU_E_SCALINGS.keys())  # Unpack iterator to list
-    return datasets
+    return tau_E, P_tau
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/impurity_effects.py` & `cfspopcon-5.0.0/cfspopcon/formulas/zeff_and_dilution/impurity_charge_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""Calculate the effect of impurities on the effective charge and dilution."""
+"""Calculate the mean charge state of an impurity for given plasma conditions."""
 import numpy as np
-import xarray as xr
 
-from ..named_options import Impurity
-from ..unit_handling import ureg, wraps_ufunc
+from ...named_options import AtomicSpecies
+from ...unit_handling import ureg, wraps_ufunc
+from ..read_atomic_data import AtomicData
 
 
 @wraps_ufunc(
     return_units=dict(mean_charge_state=ureg.dimensionless),
     input_units=dict(
         average_electron_density=ureg.m**-3,
         average_electron_temp=ureg.eV,
@@ -15,51 +15,30 @@
         atomic_data=None,
     ),
     pass_as_kwargs=("atomic_data",),
 )
 def calc_impurity_charge_state(
     average_electron_density: float,
     average_electron_temp: float,
-    impurity_species: Impurity,
-    atomic_data: dict[Impurity, xr.DataArray],
+    impurity_species: AtomicSpecies,
+    atomic_data: AtomicData,
 ) -> float:
     """Calculate the impurity charge state of the specified impurity species.
 
     Args:
-        average_electron_density: [1e19 m^-3] :term:`glossary link<average_electron_density>`
-        average_electron_temp: [keV] :term:`glossary link<average_electron_temp>`
+        average_electron_density: [m^-3] :term:`glossary link<average_electron_density>`
+        average_electron_temp: [eV] :term:`glossary link<average_electron_temp>`
         impurity_species: [] :term:`glossary link<impurity_species>`
         atomic_data: :term:`glossary link<atomic_data>`
 
     Returns:
         :term:`impurity_charge_state`
     """
-    mean_charge_curve = atomic_data[impurity_species].coronal_mean_Z_interpolator
-    return float(
-        np.squeeze(np.power(10, mean_charge_curve(np.log10(average_electron_temp), np.log10(average_electron_density), grid=True)))
+    average_electron_temp, average_electron_density = atomic_data.nearest_neighbour_off_grid(  # type:ignore[assignment]
+        impurity_species, average_electron_temp, average_electron_density  # type:ignore[arg-type]
     )
+    interpolator = atomic_data.coronal_Z_interpolators[impurity_species]
+    interpolated_values = np.power(10, interpolator((np.log10(average_electron_temp), np.log10(average_electron_density))))
 
-
-def calc_change_in_zeff(impurity_charge_state: float, impurity_concentration: xr.DataArray) -> xr.DataArray:
-    """Calculate the change in the effective charge due to the specified impurities.
-
-    Args:
-        impurity_charge_state: [~] :term:`glossary link<impurity_charge_state>`
-        impurity_concentration: [~] :term:`glossary link<impurity_concentration>`
-
-    Returns:
-        change in zeff [~]
-    """
-    return impurity_charge_state * (impurity_charge_state - 1.0) * impurity_concentration
-
-
-def calc_change_in_dilution(impurity_charge_state: float, impurity_concentration: xr.DataArray) -> xr.DataArray:
-    """Calculate the change in n_fuel/n_e due to the specified impurities.
-
-    Args:
-        impurity_charge_state: [~] :term:`glossary link<impurity_charge_state>`
-        impurity_concentration: [~] :term:`glossary link<impurity_concentration>`
-
-    Returns:
-        change in dilution [~]
-    """
-    return impurity_charge_state * impurity_concentration
+    interpolated_values = np.minimum(interpolated_values, impurity_species.value)
+    interpolated_values = np.maximum(interpolated_values, 0)
+    return interpolated_values  # type:ignore[no-any-return]
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/operational_limits.py` & `cfspopcon-5.0.0/cfspopcon/formulas/metrics/greenwald_density.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-"""Operational limits to avoid disruptive regions."""
+"""Calculate the Greenwald density limit."""
 import numpy as np
 
-from ..unit_handling import ureg, wraps_ufunc
+from ...algorithm_class import Algorithm
+from ...unit_handling import ureg, wraps_ufunc
 
 
+@Algorithm.register_algorithm(return_keys=["greenwald_fraction"])
 @wraps_ufunc(
     return_units=dict(greenwald_fraction=ureg.dimensionless),
     input_units=dict(
         average_electron_density=ureg.n20, inverse_aspect_ratio=ureg.dimensionless, major_radius=ureg.m, plasma_current=ureg.MA
     ),
 )
 def calc_greenwald_fraction(
@@ -20,42 +22,25 @@
         inverse_aspect_ratio: [~] :term:`glossary link<inverse_aspect_ratio>`
         major_radius: [m] :term:`glossary link<major_radius>`
         plasma_current: [MA] :term:`glossary link<plasma_current>`
 
     Returns:
         :term:`greenwald_fraction` [~]
     """
-    n_Greenwald = calc_greenwald_density_limit.__wrapped__(plasma_current, inverse_aspect_ratio * major_radius)
+    n_Greenwald = calc_greenwald_density_limit.unitless_func(plasma_current, inverse_aspect_ratio * major_radius)
 
     return float(average_electron_density / n_Greenwald)
 
 
+@Algorithm.register_algorithm(return_keys=["greenwald_density_limit"])
 @wraps_ufunc(return_units=dict(nG=ureg.n20), input_units=dict(plasma_current=ureg.MA, minor_radius=ureg.m))
 def calc_greenwald_density_limit(plasma_current: float, minor_radius: float) -> float:
     """Calculate the Greenwald density limit.
 
     Args:
         plasma_current: [MA] :term:`glossary link<plasma_current>`
         minor_radius: [m] :term:`glossary link<minor_radius>`
 
     Returns:
         nG Greenwald density limit [n20]
     """
     return plasma_current / (np.pi * minor_radius**2)
-
-
-@wraps_ufunc(
-    return_units=dict(troyon_max_beta=ureg.percent),
-    input_units=dict(minor_radius=ureg.m, magnetic_field_on_axis=ureg.T, plasma_current=ureg.MA),
-)
-def calc_troyon_limit(minor_radius: float, magnetic_field_on_axis: float, plasma_current: float) -> float:
-    """Calculate the maximum value for beta, according to the Troyon limit.
-
-    Args:
-        minor_radius: [m] :term:`glossary link<minor_radius>`
-        magnetic_field_on_axis: [T] :term:`glossary link<magnetic_field_on_axis>`
-        plasma_current: [MA] :term:`glossary link<plasma_current>`
-
-    Returns:
-         troyon_max_beta [~]
-    """
-    return 2.8 * plasma_current / (minor_radius * magnetic_field_on_axis)
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/plasma_profile_data/PRF/aLT.csv` & `cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/PRF/aLT.csv`

 * *Files identical despite different names*

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/plasma_profile_data/PRF/width.csv` & `cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/PRF/width.csv`

 * *Files identical despite different names*

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/plasma_profile_data/density_and_temperature_profile_fits.py` & `cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/numerical_profile_fits.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,17 @@
 from pathlib import Path
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 import yaml
 from numpy.typing import NDArray
-from scipy.interpolate import RectBivariateSpline  # type: ignore[import]
+from scipy.interpolate import RectBivariateSpline  # type: ignore[import-untyped]
 
+# TODO: Replace with importlib.resources
 plasma_profiles_directory = Path(__file__).parent
 
 
 def load_dataframe(dataset: str, df_name: str) -> pd.DataFrame:
     """Load specified dataframe for given dataset."""
     filepath = plasma_profiles_directory / dataset / f"{df_name}.csv"
     with warnings.catch_warnings():
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/plasma_profiles.py` & `cfspopcon-5.0.0/cfspopcon/formulas/plasma_profiles/plasma_profiles.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,113 @@
 
 from typing import Optional
 
 import numpy as np
 from numpy import float64
 from numpy.typing import NDArray
 
-from ..named_options import ProfileForm
-from ..unit_handling import ureg, wraps_ufunc
-from .plasma_profile_data.density_and_temperature_profile_fits import evaluate_density_and_temperature_profile_fits
+from ...algorithm_class import Algorithm
+from ...named_options import ProfileForm
+from ...unit_handling import Unitfull, ureg, wraps_ufunc
+from .density_peaking import calc_density_peaking, calc_effective_collisionality
+from .numerical_profile_fits import evaluate_density_and_temperature_profile_fits
 
 
+@Algorithm.register_algorithm(
+    return_keys=[
+        "effective_collisionality",
+        "ion_density_peaking",
+        "electron_density_peaking",
+        "peak_electron_density",
+        "peak_fuel_ion_density",
+        "peak_electron_temp",
+        "peak_ion_temp",
+        "rho",
+        "electron_density_profile",
+        "fuel_ion_density_profile",
+        "electron_temp_profile",
+        "ion_temp_profile",
+    ]
+)
+def calc_peaked_profiles(
+    profile_form: ProfileForm,
+    average_electron_density: Unitfull,
+    average_electron_temp: Unitfull,
+    average_ion_temp: Unitfull,
+    ion_density_peaking_offset: Unitfull,
+    electron_density_peaking_offset: Unitfull,
+    temperature_peaking: Unitfull,
+    major_radius: Unitfull,
+    z_effective: Unitfull,
+    dilution: Unitfull,
+    beta_toroidal: Unitfull,
+    normalized_inverse_temp_scale_length: Unitfull,
+) -> tuple[Unitfull, ...]:
+    """Calculate density peaking and the corresponding density and temperature profiles.
+
+    Args:
+        profile_form: :term:`glossary link<profile_form>`
+        average_electron_density: :term:`glossary link<average_electron_density>`
+        average_electron_temp: :term:`glossary link<average_electron_temp>`
+        average_ion_temp: :term:`glossary link<average_ion_temp>`
+        ion_density_peaking_offset: :term:`glossary link<ion_density_peaking_offset>`
+        electron_density_peaking_offset: :term:`glossary link<electron_density_peaking_offset>`
+        temperature_peaking: :term:`glossary link<temperature_peaking>`
+        major_radius: :term:`glossary link<major_radius>`
+        z_effective: :term:`glossary link<z_effective>`
+        dilution: :term:`glossary link<dilution>`
+        beta_toroidal: :term:`glossary link<beta_toroidal>`
+        normalized_inverse_temp_scale_length: :term:`glossary link<normalized_inverse_temp_scale_length>`
+
+    Returns:
+    `effective_collisionality`, :term:`ion_density_peaking`, :term:`electron_density_peaking`, :term:`peak_electron_density`, :term:`peak_electron_temp`, :term:`peak_ion_temp`, :term:`rho`, :term:`electron_density_profile`, :term:`fuel_ion_density_profile`, :term:`electron_temp_profile`, :term:`ion_temp_profile`
+
+    """
+    effective_collisionality = calc_effective_collisionality(average_electron_density, average_electron_temp, major_radius, z_effective)
+    ion_density_peaking = calc_density_peaking(effective_collisionality, beta_toroidal, nu_noffset=ion_density_peaking_offset)
+    electron_density_peaking = calc_density_peaking(effective_collisionality, beta_toroidal, nu_noffset=electron_density_peaking_offset)
+
+    peak_electron_density = average_electron_density * electron_density_peaking
+    peak_fuel_ion_density = average_electron_density * dilution * ion_density_peaking
+    peak_electron_temp = average_electron_temp * temperature_peaking
+    peak_ion_temp = average_ion_temp * temperature_peaking
+
+    # Calculate the total fusion power by estimating density and temperature profiles and
+    # using this to calculate fusion power profiles.
+    (rho, electron_density_profile, fuel_ion_density_profile, electron_temp_profile, ion_temp_profile,) = calc_1D_plasma_profiles(
+        profile_form,
+        average_electron_density,
+        average_electron_temp,
+        average_ion_temp,
+        electron_density_peaking,
+        ion_density_peaking,
+        temperature_peaking,
+        dilution,
+        normalized_inverse_temp_scale_length,
+    )
+
+    return (
+        effective_collisionality,
+        ion_density_peaking,
+        electron_density_peaking,
+        peak_electron_density,
+        peak_fuel_ion_density,
+        peak_electron_temp,
+        peak_ion_temp,
+        rho,
+        electron_density_profile,
+        fuel_ion_density_profile,
+        electron_temp_profile,
+        ion_temp_profile,
+    )
+
+
+@Algorithm.register_algorithm(
+    return_keys=["rho", "electron_density_profile", "fuel_ion_density_profile", "electron_temp_profile", "ion_temp_profile"]
+)
 @wraps_ufunc(
     return_units=dict(
         rho=ureg.dimensionless,
         electron_density_profile=ureg.n19,
         fuel_ion_density_profile=ureg.n19,
         electron_temp_profile=ureg.keV,
         ion_temp_profile=ureg.keV,
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/mavrin_coronal.py` & `cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/mavrin_coronal.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import warnings
 
 import numpy as np
 from numpy import float64
 from numpy.polynomial.polynomial import polyval
 from numpy.typing import NDArray
 
-from ...named_options import Impurity
-from ...unit_handling import ureg, wraps_ufunc
-from ..helpers import integrate_profile_over_volume
+from ....named_options import AtomicSpecies
+from ....unit_handling import ureg, wraps_ufunc
+from ...geometry.volume_integral import integrate_profile_over_volume
 
 
 @wraps_ufunc(
     return_units=dict(radiated_power=ureg.MW),
     input_units=dict(
         rho=ureg.dimensionless,
         electron_temp_profile=ureg.keV,
@@ -25,15 +25,15 @@
     input_core_dims=[("dim_rho",), ("dim_rho",), ("dim_rho",), (), (), ()],
 )
 def calc_impurity_radiated_power_mavrin_coronal(  # noqa: PLR0912, PLR0915
     rho: NDArray[float64],
     electron_temp_profile: NDArray[float64],
     electron_density_profile: NDArray[float64],
     impurity_concentration: float,
-    impurity_species: Impurity,
+    impurity_species: AtomicSpecies,
     plasma_volume: float,
 ) -> float:
     """Calculation of radiated power, using fits from A.A. Mavrin's 2018 paper.
 
     "Improved fits of coronal radiative cooling rates for high-temperature plasmas."
 
     :cite:`mavrin_improved_2018`
@@ -183,10 +183,10 @@
             log10_Lz[it] = polyval(Tlog[it], radc[i])  # type: ignore[no-untyped-call]
 
     radrate = 10.0**log10_Lz
     radrate[np.isnan(radrate)] = 0
 
     # 1e38 factor to account for the fact that our n_e values are electron_density_profile values
     qRad = radrate * electron_temp_profile * electron_temp_profile * impurity_concentration * 1e38  # W / (m^3 s)
-    radiated_power = integrate_profile_over_volume(qRad, rho, plasma_volume)  # [W]
+    radiated_power = integrate_profile_over_volume.unitless_func(qRad, rho, plasma_volume)  # [W]
 
     return float(radiated_power) / 1e6  # MW
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/mavrin_noncoronal.py` & `cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/mavrin_noncoronal.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import warnings
 
 import numpy as np
 from numpy import float64
 from numpy.typing import NDArray
 
-from ...named_options import Impurity
-from ...unit_handling import Quantity, ureg, wraps_ufunc
-from ..helpers import integrate_profile_over_volume
+from ....named_options import AtomicSpecies
+from ....unit_handling import Quantity, ureg, wraps_ufunc
+from ...geometry.volume_integral import integrate_profile_over_volume
 
 
 @wraps_ufunc(
     return_units=dict(radiated_power=ureg.MW),
     input_units=dict(
         rho=ureg.dimensionless,
         electron_temp_profile=ureg.keV,
@@ -26,15 +26,15 @@
 )
 def calc_impurity_radiated_power_mavrin_noncoronal(  # noqa: PLR0912
     rho: NDArray[float64],
     electron_temp_profile: NDArray[float64],
     electron_density_profile: NDArray[float64],
     tau_i: Quantity,
     impurity_concentration: float,
-    impurity_species: Impurity,
+    impurity_species: AtomicSpecies,
     plasma_volume: float,
 ) -> float:
     """Calculation of radiated power, using fits from A.A. Mavrin's 2017 paper.
 
     "Radiative Cooling Rates for Low-Z Impurities in Non-coronal Equilibrium State."
 
     :cite:`mavrin_radiative_2017`
@@ -242,10 +242,10 @@
                     + radc[9, j] * Y**3
                 )
                 continue
 
     radrate = 10.0**log10_Lz
 
     qRad = radrate * electron_density_profile * electron_density_profile * impurity_concentration  # W / (m^3 s)
-    radiated_power = integrate_profile_over_volume(qRad, rho, plasma_volume)  # [W]
+    radiated_power = integrate_profile_over_volume.unitless_func(qRad, rho, plasma_volume)  # [W]
 
     return float(radiated_power) / 1e6  # MW
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/post_and_jensen.py` & `cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/post_and_jensen.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import warnings
 
 import numpy as np
 from numpy import float64
 from numpy.polynomial.polynomial import polyval
 from numpy.typing import NDArray
 
-from ...named_options import Impurity
-from ...unit_handling import ureg, wraps_ufunc
-from ..helpers import integrate_profile_over_volume
+from ....named_options import AtomicSpecies
+from ....unit_handling import ureg, wraps_ufunc
+from ...geometry.volume_integral import integrate_profile_over_volume
 
 
 @wraps_ufunc(
     return_units=dict(radiated_power=ureg.MW),
     input_units=dict(
         rho=ureg.dimensionless,
         electron_temp_profile=ureg.keV,
@@ -25,15 +25,15 @@
     input_core_dims=[("dim_rho",), ("dim_rho",), ("dim_rho",), (), (), ()],
 )
 def calc_impurity_radiated_power_post_and_jensen(
     rho: NDArray[float64],
     electron_temp_profile: NDArray[float64],
     electron_density_profile: NDArray[float64],
     impurity_concentration: float,
-    impurity_species: Impurity,
+    impurity_species: AtomicSpecies,
     plasma_volume: float,
 ) -> float:
     """Calculation of radiated power using Post & Jensen 1977.
 
     Radiation fits to the Post & Jensen cooling curves, which use the
     coronal equilibrium model with data in :cite:`post_steady_1977`.
 
@@ -150,9 +150,9 @@
 
     radrate = 10.0**log10_Lz
     radrate[np.isnan(radrate)] = 0
     radrate /= 1e13  # convert from erg cm^3 -> J m^3  (erg == 1e-7 J)
 
     # 1e38 factor to account for the fact that our n_e values are electron_density_profile values
     qRad = radrate * electron_density_profile * electron_density_profile * impurity_concentration * 1e38  # W / (m^3 s)
-    radiated_power = integrate_profile_over_volume(qRad, rho, plasma_volume)  # [W]
+    radiated_power = integrate_profile_over_volume.unitless_func(qRad, rho, plasma_volume)  # [W]
     return float(radiated_power) / 1e6  # MW
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/radas.py` & `cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/radas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Calculate the impurity radiated power using the radas atomic_data."""
 import numpy as np
-import xarray as xr
 from numpy import float64
 from numpy.typing import NDArray
 
-from ...named_options import Impurity
-from ...unit_handling import magnitude, ureg, wraps_ufunc
-from ..helpers import integrate_profile_over_volume
+from ....named_options import AtomicSpecies
+from ....unit_handling import ureg, wraps_ufunc
+from ...geometry.volume_integral import integrate_profile_over_volume
+from ...read_atomic_data import AtomicData
 
 
 @wraps_ufunc(
     return_units=dict(radiated_power=ureg.MW),
     input_units=dict(
         rho=ureg.dimensionless,
         electron_temp_profile=ureg.eV,
@@ -24,44 +24,39 @@
     pass_as_kwargs=("atomic_data",),
 )
 def calc_impurity_radiated_power_radas(
     rho: NDArray[float64],
     electron_temp_profile: NDArray[float64],
     electron_density_profile: NDArray[float64],
     impurity_concentration: float,
-    impurity_species: Impurity,
+    impurity_species: AtomicSpecies,
     plasma_volume: float,
-    atomic_data: dict[Impurity, xr.DataArray],
+    atomic_data: AtomicData,
 ) -> float:
     """Calculation of radiated power using radas atomic_data datasets.
 
     Args:
         rho: [~] :term:`glossary link<rho>`
-        electron_temp_profile: [keV] :term:`glossary link<electron_temp_profile>`
-        electron_density_profile: [1e19 m^-3] :term:`glossary link<electron_density_profile>`
+        electron_temp_profile: [eV] :term:`glossary link<electron_temp_profile>`
+        electron_density_profile: [m^-3] :term:`glossary link<electron_density_profile>`
         impurity_species: [] :term:`glossary link<impurity_species>`
         impurity_concentration: [~] :term:`glossary link<impurity_concentration>`
         plasma_volume: [m^3] :term:`glossary link<plasma_volume>`
         atomic_data: :term:`glossary link<atomic_data>`
 
     Returns:
          [MW] Estimated radiation power due to this impurity
     """
     MW_per_W = 1e6
 
-    ds = atomic_data[impurity_species]
-    Lz_curve = ds.coronal_Lz_interpolator
-
-    # Use nearest neighbor extrapolation if evaluating for a
-    # point off-grid
-
-    electron_temp_profile = np.minimum(electron_temp_profile, magnitude(ds.electron_temperature.max()))
-    electron_temp_profile = np.maximum(electron_temp_profile, magnitude(ds.electron_temperature.min()))
-    electron_density_profile = np.minimum(electron_density_profile, magnitude(ds.electron_density.max()))
-    electron_density_profile = np.maximum(electron_density_profile, magnitude(ds.electron_density.min()))
-
-    Lz = np.power(10, Lz_curve(np.log10(electron_temp_profile), np.log10(electron_density_profile), grid=False))
+    electron_temp_profile, electron_density_profile = atomic_data.nearest_neighbour_off_grid(  # type:ignore[assignment]
+        impurity_species, electron_temp_profile, electron_density_profile
+    )
+    interpolator = atomic_data.coronal_Lz_interpolators[impurity_species]
+    Lz = np.power(10, interpolator((np.log10(electron_temp_profile), np.log10(electron_density_profile))))
     radiated_power_profile = electron_density_profile**2 * Lz
 
-    radiated_power = impurity_concentration * integrate_profile_over_volume(radiated_power_profile, rho, plasma_volume) / MW_per_W
+    radiated_power: float = (
+        impurity_concentration * integrate_profile_over_volume.unitless_func(radiated_power_profile, rho, plasma_volume) / MW_per_W
+    )
 
     return radiated_power
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/radiated_power/radiated_power.py` & `cfspopcon-5.0.0/cfspopcon/formulas/radiated_power/impurity_radiated_power/radiated_power.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Compute the total radiated power."""
 import numpy as np
 import xarray as xr
 
-from ...named_options import Impurity, RadiationMethod
-from ...unit_handling import Unitfull, ureg
+from ....named_options import RadiationMethod
+from ....unit_handling import Unitfull, ureg
+from ...read_atomic_data import AtomicData
 from .mavrin_coronal import calc_impurity_radiated_power_mavrin_coronal
 from .mavrin_noncoronal import calc_impurity_radiated_power_mavrin_noncoronal
 from .post_and_jensen import calc_impurity_radiated_power_post_and_jensen
 from .radas import calc_impurity_radiated_power_radas
 
 
 def calc_impurity_radiated_power(
     radiated_power_method: RadiationMethod,
     rho: Unitfull,
     electron_temp_profile: Unitfull,
     electron_density_profile: Unitfull,
     impurities: xr.DataArray,
     plasma_volume: Unitfull,
-    atomic_data: dict[Impurity, xr.DataArray],
+    atomic_data: AtomicData,
 ) -> xr.DataArray:
     """Compute the total radiated power due to fuel and impurity species.
 
     Args:
         radiated_power_method: [] :term:`glossary link<radiated_power_method>`
         rho: [~] :term:`glossary link<rho>`
         electron_temp_profile: [keV] :term:`glossary link<electron_temp_profile>`
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/__init__.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-"""Module to perform simple scrape-off-layer calculations.
-
-These are mostly based on the two-point-model, from :cite:`stangeby_2018`.
-"""
-from .lambda_q import calc_lambda_q
-from .parallel_heat_flux_density import calc_parallel_heat_flux_density
-from .solve_target_first_two_point_model import solve_target_first_two_point_model
-from .solve_two_point_model import solve_two_point_model
+"""The extended two point model, based on the two-point-model from :cite:`stangeby_2018`."""
+from .model import solve_two_point_model
+from .target_first_model import solve_target_first_two_point_model
+from .two_point_model_algorithms import (
+    two_point_model_fixed_fpow,
+    two_point_model_fixed_qpart,
+    two_point_model_fixed_tet,
+)
 
 __all__ = [
     "solve_two_point_model",
-    "calc_parallel_heat_flux_density",
-    "calc_lambda_q",
     "solve_target_first_two_point_model",
+    "two_point_model_fixed_fpow",
+    "two_point_model_fixed_qpart",
+    "two_point_model_fixed_tet",
 ]
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/lambda_q.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/lambda_q.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 """Routines to calculate the heat flux decay length (lambda_q), for several different scalings."""
 
+from ...algorithm_class import Algorithm
 from ...named_options import LambdaQScaling
 from ...unit_handling import ureg, wraps_ufunc
 
 
+@Algorithm.register_algorithm(return_keys=["lambda_q"])
 @wraps_ufunc(
     return_units=dict(lambda_q=ureg.millimeter),
     input_units=dict(
         lambda_q_scaling=None,
         average_total_pressure=ureg.atm,
-        power_crossing_separatrix=ureg.megawatt,
+        P_sol=ureg.megawatt,
         major_radius=ureg.meter,
-        B_pol_omp=ureg.tesla,
+        B_pol_out_mid=ureg.tesla,
         inverse_aspect_ratio=ureg.dimensionless,
+        lambda_q_factor=ureg.dimensionless,
     ),
 )
 def calc_lambda_q(
     lambda_q_scaling: LambdaQScaling,
     average_total_pressure: float,
-    power_crossing_separatrix: float,
+    P_sol: float,
     major_radius: float,
-    B_pol_omp: float,
+    B_pol_out_mid: float,
     inverse_aspect_ratio: float,
+    lambda_q_factor: float = 1.0,
 ) -> float:
     """Calculate SOL heat flux decay length (lambda_q) from a scaling.
 
     Args:
         lambda_q_scaling: :term:`glossary link<lambda_q_scaling>`
         average_total_pressure: [atm] :term:`glossary link <average_total_pressure>`
-        power_crossing_separatrix: [MW] :term:`glossary link<power_crossing_separatrix>`
+        P_sol: [MW] :term:`glossary link<P_sol>`
         major_radius: [m] :term:`glossary link<major_radius>`
-        B_pol_omp: [T] :term:`glossary link<B_pol_omp>`
+        B_pol_out_mid: [T] :term:`glossary link<B_pol_out_mid>`
         inverse_aspect_ratio: [~] :term:`glossary link<inverse_aspect_ratio>`
+        lambda_q_factor: [~] :term:`glossary link<lambda_q_factor>`
 
     Returns:
         :term:`lambda_q` [mm]
     """
     if lambda_q_scaling == LambdaQScaling.Brunner:
-        return float(calc_lambda_q_with_brunner.__wrapped__(average_total_pressure))
+        return lambda_q_factor * float(calc_lambda_q_with_brunner.unitless_func(average_total_pressure))
     elif lambda_q_scaling == LambdaQScaling.EichRegression14:
-        return float(calc_lambda_q_with_eich_regression_14.__wrapped__(B_pol_omp))
+        return lambda_q_factor * float(calc_lambda_q_with_eich_regression_14.unitless_func(B_pol_out_mid))
     elif lambda_q_scaling == LambdaQScaling.EichRegression15:
-        return float(
-            calc_lambda_q_with_eich_regression_15.__wrapped__(power_crossing_separatrix, major_radius, B_pol_omp, inverse_aspect_ratio)
+        return lambda_q_factor * float(
+            calc_lambda_q_with_eich_regression_15.unitless_func(P_sol, major_radius, B_pol_out_mid, inverse_aspect_ratio)
         )
     else:
         raise NotImplementedError(f"No implementation for lambda_q scaling {lambda_q_scaling}")
 
 
 @wraps_ufunc(
     return_units=dict(lambda_q=ureg.millimeter),
@@ -56,37 +61,35 @@
     """Return lambda_q according to the Brunner scaling.
 
     Equation 4 in :cite:`brunner_2018_heat_flux`
     """
     return float(0.91 * average_total_pressure**-0.48)
 
 
-@wraps_ufunc(return_units=dict(lambda_q=ureg.millimeter), input_units=dict(B_pol_omp=ureg.tesla))
-def calc_lambda_q_with_eich_regression_14(B_pol_omp: float) -> float:
+@wraps_ufunc(return_units=dict(lambda_q=ureg.millimeter), input_units=dict(B_pol_out_mid=ureg.tesla))
+def calc_lambda_q_with_eich_regression_14(B_pol_out_mid: float) -> float:
     """Return lambda_q according to Eich regression 14.
 
     #14 in Table 3 in :cite:`eich_scaling_2013`
     """
-    return float(0.63 * B_pol_omp**-1.19)
+    return float(0.63 * B_pol_out_mid**-1.19)
 
 
 @wraps_ufunc(
     return_units=dict(lambda_q=ureg.millimeter),
     input_units=dict(
-        power_crossing_separatrix=ureg.megawatt,
+        P_sol=ureg.megawatt,
         major_radius=ureg.meter,
-        B_pol_omp=ureg.tesla,
+        B_pol_out_mid=ureg.tesla,
         inverse_aspect_ratio=ureg.dimensionless,
     ),
 )
-def calc_lambda_q_with_eich_regression_15(
-    power_crossing_separatrix: float, major_radius: float, B_pol_omp: float, inverse_aspect_ratio: float
-) -> float:
+def calc_lambda_q_with_eich_regression_15(P_sol: float, major_radius: float, B_pol_out_mid: float, inverse_aspect_ratio: float) -> float:
     """Return lambda_q according to Eich regression 15.
 
     #15 in Table 3 in :cite:`eich_scaling_2013`
     """
-    lambda_q = 1.35 * major_radius**0.04 * B_pol_omp**-0.92 * inverse_aspect_ratio**0.42
-    if power_crossing_separatrix > 0:
-        return float(lambda_q * power_crossing_separatrix**-0.02)
+    lambda_q = 1.35 * major_radius**0.04 * B_pol_out_mid**-0.92 * inverse_aspect_ratio**0.42
+    if P_sol > 0:
+        return float(lambda_q * P_sol**-0.02)
     else:
         return float(lambda_q)
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/momentum_loss_functions.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/momentum_loss_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Calculate SOL momentum loss as a function target electron temperature.
 
 See Figure 15 of :cite:`stangeby_2018`.
 """
 import numpy as np
 
-from ...named_options import MomentumLossFunction
-from ...unit_handling import Quantity, ureg, wraps_ufunc
+from ....named_options import MomentumLossFunction
+from ....unit_handling import Quantity, ureg, wraps_ufunc
 
 
 def _calc_SOL_momentum_loss_fraction(A: float, Tstar: float, n: float, target_electron_temp: float) -> float:
     """Calculates the fraction of momentum lost in the SOL, for a generic SOL momentum loss function.
 
     This is equation 33 of :cite:`stangeby_2018`, rearranged for $f^{total}_{mom-loss}$
     """
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/required_power_loss_fraction.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/required_power_loss_fraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Calculate the SOL power loss fraction required to achieve a specified target electron temperature."""
 
 from typing import Union
 
 import numpy as np
 import xarray as xr
 
-from ...unit_handling import Quantity
+from ....unit_handling import Quantity
 
 
 def calc_required_SOL_power_loss_fraction(
     target_electron_temp_basic: Union[Quantity, xr.DataArray],
     f_other_target_electron_temp: Union[float, xr.DataArray],
     SOL_momentum_loss_fraction: Union[Quantity, xr.DataArray],
     required_target_electron_temp: Union[Quantity, xr.DataArray],
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/solve_target_first_two_point_model.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/target_first_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Compute all terms in the two-point-model for a fixed target electron temperature."""
 from typing import Union
 
 import xarray as xr
 
-from ...named_options import MomentumLossFunction
-from ...unit_handling import Unitfull, ureg
+from ....named_options import MomentumLossFunction
+from ....unit_handling import Unitfull, ureg
+from ..separatrix_electron_temp import calc_separatrix_electron_temp
 from .momentum_loss_functions import calc_SOL_momentum_loss_fraction
 from .required_power_loss_fraction import calc_required_SOL_power_loss_fraction
+from .separatrix_pressure import calc_upstream_total_pressure
 from .target_electron_density import (
     calc_f_other_target_electron_density,
     calc_f_vol_loss_target_electron_density,
     calc_target_electron_density,
     calc_target_electron_density_basic,
 )
 from .target_electron_flux import (
     calc_f_other_target_electron_flux,
     calc_f_vol_loss_target_electron_flux,
     calc_target_electron_flux,
     calc_target_electron_flux_basic,
 )
 from .target_electron_temp import calc_f_other_target_electron_temp, calc_target_electron_temp_basic
-from .total_pressure import calc_upstream_total_pressure
-from .upstream_electron_temp import calc_upstream_electron_temp
 
 
 def solve_target_first_two_point_model(
     target_electron_temp: Unitfull,
     parallel_heat_flux_density: Unitfull,
     parallel_connection_length: Unitfull,
-    upstream_electron_density: Unitfull,
+    separatrix_electron_density: Unitfull,
     toroidal_flux_expansion: Unitfull,
     fuel_average_mass_number: Unitfull,
     kappa_e0: Unitfull,
     SOL_momentum_loss_function: Union[MomentumLossFunction, xr.DataArray],
     sheath_heat_transmission_factor: Unitfull = 7.5 * ureg.dimensionless,
     SOL_conduction_fraction: Unitfull = 1.0 * ureg.dimensionless,
     target_ratio_of_ion_to_electron_temp: Unitfull = 1.0 * ureg.dimensionless,
@@ -44,44 +44,44 @@
 ) -> tuple[Unitfull, Unitfull, Unitfull, Unitfull]:
     """Calculate the SOL_power_loss_fraction required to keep the target temperature at a given value.
 
     Args:
         target_electron_temp: [eV]
         parallel_heat_flux_density: [GW/m^2]
         parallel_connection_length: [m]
-        upstream_electron_density: [m^-3]
+        separatrix_electron_density: [m^-3]
         toroidal_flux_expansion: [~]
         fuel_average_mass_number: [~]
         kappa_e0: electron heat conductivity constant [W / (eV^3.5 * m)]
         SOL_momentum_loss_function: which momentum loss function to use
         sheath_heat_transmission_factor: [~]
         SOL_conduction_fraction: [~]
         target_ratio_of_ion_to_electron_temp: [~]
         target_ratio_of_electron_to_ion_density: [~]
         target_mach_number: [~]
         upstream_ratio_of_ion_to_electron_temp: [~]
         upstream_ratio_of_electron_to_ion_density: [~]
         upstream_mach_number: [~]
 
     Returns:
-        SOL_power_loss_fraction [~], upstream_electron_temp [eV], target_electron_density [m^-3], target_electron_flux [m^-2 s^-1]
+        SOL_power_loss_fraction [~], separatrix_electron_temp [eV], target_electron_density [m^-3], target_electron_flux [m^-2 s^-1]
     """
     SOL_momentum_loss_fraction = calc_SOL_momentum_loss_fraction(SOL_momentum_loss_function, target_electron_temp)
 
-    upstream_electron_temp = calc_upstream_electron_temp(
+    separatrix_electron_temp = calc_separatrix_electron_temp(
         target_electron_temp=target_electron_temp,
         parallel_heat_flux_density=parallel_heat_flux_density,
         parallel_connection_length=parallel_connection_length,
         SOL_conduction_fraction=SOL_conduction_fraction,
         kappa_e0=kappa_e0,
     )
 
     upstream_total_pressure = calc_upstream_total_pressure(
-        upstream_electron_density=upstream_electron_density,
-        upstream_electron_temp=upstream_electron_temp,
+        separatrix_electron_density=separatrix_electron_density,
+        separatrix_electron_temp=separatrix_electron_temp,
         upstream_ratio_of_ion_to_electron_temp=upstream_ratio_of_ion_to_electron_temp,
         upstream_ratio_of_electron_to_ion_density=upstream_ratio_of_electron_to_ion_density,
         upstream_mach_number=upstream_mach_number,
     )
 
     f_basic_kwargs = dict(
         fuel_average_mass_number=fuel_average_mass_number,
@@ -114,8 +114,8 @@
 
     target_electron_flux = calc_target_electron_flux(
         target_electron_flux_basic=calc_target_electron_flux_basic(**f_basic_kwargs),
         f_vol_loss_target_electron_flux=calc_f_vol_loss_target_electron_flux(**f_vol_loss_kwargs),
         f_other_target_electron_flux=calc_f_other_target_electron_flux(**f_other_kwargs),
     )
 
-    return SOL_power_loss_fraction, upstream_electron_temp, target_electron_density, target_electron_flux
+    return SOL_power_loss_fraction, separatrix_electron_temp, target_electron_density, target_electron_flux
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/solve_two_point_model.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Compute all terms in the two-point-model for a fixed SOL power loss fraction."""
 from typing import Union
 
 import numpy as np
 import xarray as xr
 
-from ...named_options import MomentumLossFunction
-from ...unit_handling import Quantity, Unitfull, ureg
+from ....named_options import MomentumLossFunction
+from ....unit_handling import Quantity, Unitfull, ureg
+from ..separatrix_electron_temp import calc_separatrix_electron_temp
 from .momentum_loss_functions import calc_SOL_momentum_loss_fraction
+from .separatrix_pressure import calc_upstream_total_pressure
 from .target_electron_density import (
     calc_f_other_target_electron_density,
     calc_f_vol_loss_target_electron_density,
     calc_target_electron_density,
     calc_target_electron_density_basic,
 )
 from .target_electron_flux import (
@@ -21,23 +23,21 @@
 )
 from .target_electron_temp import (
     calc_f_other_target_electron_temp,
     calc_f_vol_loss_target_electron_temp,
     calc_target_electron_temp,
     calc_target_electron_temp_basic,
 )
-from .total_pressure import calc_upstream_total_pressure
-from .upstream_electron_temp import calc_upstream_electron_temp
 
 
 def solve_two_point_model(
     SOL_power_loss_fraction: Unitfull,
     parallel_heat_flux_density: Unitfull,
     parallel_connection_length: Unitfull,
-    upstream_electron_density: Unitfull,
+    separatrix_electron_density: Unitfull,
     toroidal_flux_expansion: Unitfull,
     fuel_average_mass_number: Unitfull,
     kappa_e0: Unitfull,
     SOL_momentum_loss_function: Union[MomentumLossFunction, xr.DataArray],
     initial_target_electron_temp: Unitfull = 10.0 * ureg.eV,
     sheath_heat_transmission_factor: Unitfull = 7.5 * ureg.dimensionless,
     SOL_conduction_fraction: Unitfull = 1.0 * ureg.dimensionless,
@@ -62,15 +62,15 @@
 ) -> tuple[Union[Quantity, xr.DataArray], Union[Quantity, xr.DataArray], Union[Quantity, xr.DataArray], Union[Quantity, xr.DataArray]]:
     """Calculate the upstream and target electron temperature and target electron density according to the extended two-point-model.
 
     Args:
         SOL_power_loss_fraction: [~]
         parallel_heat_flux_density: [GW/m^2]
         parallel_connection_length: [m]
-        upstream_electron_density: [m^-3]
+        separatrix_electron_density: [m^-3]
         toroidal_flux_expansion: [~]
         fuel_average_mass_number: [~]
         kappa_e0: electron heat conductivity constant [W / (eV^3.5 * m)]
         SOL_momentum_loss_function: which momentum loss function to use
         initial_target_electron_temp: starting guess for target electron temp [eV]
         sheath_heat_transmission_factor: [~]
         SOL_conduction_fraction: [~]
@@ -86,15 +86,15 @@
         target_temp_relaxation: step-size for target Te evolution
         upstream_temp_max_residual: relative rate of change for convergence for upstream Te evolution
         target_electron_density_max_residual: relative rate of change for convergence for target ne evolution
         target_temp_max_residual: relative rate of change for convergence for target Te evolution
         raise_error_if_not_converged: raise an error if not all point converge within max iterations (otherwise return NaN)
         quiet: if not True, print additional information about the iterative solve to terminal
     Returns:
-        upstream_electron_temp [eV], target_electron_density [m^-3], target_electron_temp [eV], target_electron_flux [m^-2 s^-1]
+        separatrix_electron_temp [eV], target_electron_density [m^-3], target_electron_temp [eV], target_electron_flux [m^-2 s^-1]
     """
     f_other_kwargs = dict(
         target_ratio_of_ion_to_electron_temp=target_ratio_of_ion_to_electron_temp,
         target_ratio_of_electron_to_ion_density=target_ratio_of_electron_to_ion_density,
         target_mach_number=target_mach_number,
         toroidal_flux_expansion=toroidal_flux_expansion,
     )
@@ -104,25 +104,25 @@
 
     iteration = 0
     target_electron_temp = initial_target_electron_temp
 
     while iteration < max_iterations:
         iteration += 1
 
-        new_upstream_electron_temp = calc_upstream_electron_temp(
+        new_separatrix_electron_temp = calc_separatrix_electron_temp(
             target_electron_temp=target_electron_temp,
             parallel_heat_flux_density=parallel_heat_flux_density,
             parallel_connection_length=parallel_connection_length,
             SOL_conduction_fraction=SOL_conduction_fraction,
             kappa_e0=kappa_e0,
         )
 
         upstream_total_pressure = calc_upstream_total_pressure(
-            upstream_electron_density=upstream_electron_density,
-            upstream_electron_temp=new_upstream_electron_temp,
+            separatrix_electron_density=separatrix_electron_density,
+            separatrix_electron_temp=new_separatrix_electron_temp,
             upstream_ratio_of_ion_to_electron_temp=upstream_ratio_of_ion_to_electron_temp,
             upstream_ratio_of_electron_to_ion_density=upstream_ratio_of_electron_to_ion_density,
             upstream_mach_number=upstream_mach_number,
         )
 
         f_vol_loss_kwargs = dict(
             SOL_power_loss_fraction=SOL_power_loss_fraction,
@@ -151,30 +151,30 @@
         new_target_electron_temp = calc_target_electron_temp(
             target_electron_temp_basic=target_electron_temp_basic,
             f_vol_loss_target_electron_temp=f_vol_loss_target_electron_temp,
             f_other_target_electron_temp=f_other_target_electron_temp,
         )
 
         if iteration == 1:
-            upstream_electron_temp = new_upstream_electron_temp
+            separatrix_electron_temp = new_separatrix_electron_temp
             target_electron_density = new_target_electron_density
             target_electron_temp = new_target_electron_temp
             continue
 
-        change_in_upstream_electron_temp = new_upstream_electron_temp - upstream_electron_temp
+        change_in_separatrix_electron_temp = new_separatrix_electron_temp - separatrix_electron_temp
         change_in_target_electron_density = new_target_electron_density - target_electron_density
         change_in_target_electron_temp = new_target_electron_temp - target_electron_temp
 
-        upstream_electron_temp = upstream_electron_temp + upstream_temp_relaxation * change_in_upstream_electron_temp
+        separatrix_electron_temp = separatrix_electron_temp + upstream_temp_relaxation * change_in_separatrix_electron_temp
         target_electron_density = target_electron_density + target_electron_density_relaxation * change_in_target_electron_density
         target_electron_temp = target_electron_temp + target_temp_relaxation * change_in_target_electron_temp
 
         if np.all(
             [
-                np.abs(change_in_upstream_electron_temp / upstream_electron_temp).max() < upstream_temp_max_residual,
+                np.abs(change_in_separatrix_electron_temp / separatrix_electron_temp).max() < upstream_temp_max_residual,
                 np.abs(change_in_target_electron_density / target_electron_density).max() < target_electron_density_max_residual,
                 np.abs(change_in_target_electron_temp / target_electron_temp).max() < target_temp_max_residual,
             ]
         ):
             if not quiet:
                 print(f"Converged in {iteration} iterations")
             break
@@ -188,22 +188,22 @@
     target_electron_flux = calc_target_electron_flux(
         target_electron_flux_basic=target_electron_flux_basic,
         f_vol_loss_target_electron_flux=f_vol_loss_target_electron_flux,
         f_other_target_electron_flux=f_other_target_electron_flux,
     )
 
     mask = (
-        (np.abs(change_in_upstream_electron_temp / upstream_electron_temp) < upstream_temp_max_residual)
+        (np.abs(change_in_separatrix_electron_temp / separatrix_electron_temp) < upstream_temp_max_residual)
         & (np.abs(change_in_target_electron_density / target_electron_density) < target_electron_density_max_residual)
         & (np.abs(change_in_target_electron_temp / target_electron_temp) < target_temp_max_residual)
     )
 
     number_nonconverged = np.count_nonzero(~mask)
     if number_nonconverged > 0 and not quiet:
         print(f"{number_nonconverged} values did not converge in {max_iterations} iterations.")
 
-    upstream_electron_temp = xr.where(mask, upstream_electron_temp, np.nan)  # type:ignore[no-untyped-call]
+    separatrix_electron_temp = xr.where(mask, separatrix_electron_temp, np.nan)  # type:ignore[no-untyped-call]
     target_electron_density = xr.where(mask, target_electron_density, np.nan)  # type:ignore[no-untyped-call]
     target_electron_temp = xr.where(mask, target_electron_temp, np.nan)  # type:ignore[no-untyped-call]
     target_electron_flux = xr.where(mask, target_electron_flux, np.nan)  # type:ignore[no-untyped-call]
 
-    return upstream_electron_temp, target_electron_density, target_electron_temp, target_electron_flux
+    return separatrix_electron_temp, target_electron_density, target_electron_temp, target_electron_flux
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/target_electron_density.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/target_electron_density.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Routines to calculate the target electron density, following the 2-point-model method of Stangeby, PPCF 2018."""
 from typing import Union
 
 import xarray as xr
 
-from ...unit_handling import Quantity
+from ....unit_handling import Quantity
 
 
 def calc_target_electron_density(
     target_electron_density_basic: Union[Quantity, xr.DataArray],
     f_vol_loss_target_electron_density: Union[float, xr.DataArray],
     f_other_target_electron_density: Union[float, xr.DataArray],
 ) -> Union[Quantity, xr.DataArray]:
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/target_electron_flux.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/target_electron_flux.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Routines to calculate the target electron flux, following the 2-point-model method of Stangeby, PPCF 2018."""
 from typing import Union
 
 import xarray as xr
 
-from ...unit_handling import Quantity
+from ....unit_handling import Quantity
 
 
 def calc_target_electron_flux(
     target_electron_flux_basic: Union[Quantity, xr.DataArray],
     f_vol_loss_target_electron_flux: Union[float, xr.DataArray],
     f_other_target_electron_flux: Union[float, xr.DataArray],
 ) -> Union[Quantity, xr.DataArray]:
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/target_electron_temp.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/target_electron_temp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Routines to calculate the target electron temperature, following the 2-point-model method of Stangeby, PPCF 2018."""
 from typing import Union
 
 import xarray as xr
 
-from ...unit_handling import Quantity
+from ....unit_handling import Quantity
 
 
 def calc_target_electron_temp(
     target_electron_temp_basic: Union[Quantity, xr.DataArray],
     f_vol_loss_target_electron_temp: Union[float, xr.DataArray],
     f_other_target_electron_temp: Union[float, xr.DataArray],
 ) -> Union[Quantity, xr.DataArray]:
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/total_pressure.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/two_point_model/separatrix_pressure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """Routines to calculate the combined electron and ion pressure in the SOL."""
 from typing import Union
 
 import xarray as xr
 
-from ...unit_handling import Quantity
+from ....unit_handling import Quantity
 
 
 def calc_upstream_total_pressure(
-    upstream_electron_density: Union[Quantity, xr.DataArray],
-    upstream_electron_temp: Union[Quantity, xr.DataArray],
+    separatrix_electron_density: Union[Quantity, xr.DataArray],
+    separatrix_electron_temp: Union[Quantity, xr.DataArray],
     upstream_ratio_of_ion_to_electron_temp: Union[float, xr.DataArray],
     upstream_ratio_of_electron_to_ion_density: Union[float, xr.DataArray],
     upstream_mach_number: Union[float, xr.DataArray] = 0.0,
 ) -> Union[Quantity, xr.DataArray]:
     """Calculate the upstream total pressure (including the ion temperature contribution).
 
     Same as calc_total_pressure, but with a default value upstream_mach_number=0.0.
 
     Args:
-        upstream_electron_density: [m^-3]
-        upstream_electron_temp: [eV]
+        separatrix_electron_density: [m^-3]
+        separatrix_electron_temp: [eV]
         upstream_ratio_of_ion_to_electron_temp: tau_t = (T_i / T_e) [~]
         upstream_ratio_of_electron_to_ion_density: z_t = (ne / ni) [~]
         upstream_mach_number: M_t = (parallel ion velocity / sound speed) [~]
 
     Returns:
         upstream_total_pressure [atm]
     """
     return calc_total_pressure(
-        electron_density=upstream_electron_density,
-        electron_temp=upstream_electron_temp,
+        electron_density=separatrix_electron_density,
+        electron_temp=separatrix_electron_temp,
         ratio_of_ion_to_electron_temp=upstream_ratio_of_ion_to_electron_temp,
         ratio_of_electron_to_ion_density=upstream_ratio_of_electron_to_ion_density,
         mach_number=upstream_mach_number,
     )
 
 
 def calc_total_pressure(
```

### Comparing `cfspopcon-4.0.0/cfspopcon/formulas/scrape_off_layer_model/upstream_electron_temp.py` & `cfspopcon-5.0.0/cfspopcon/formulas/scrape_off_layer/separatrix_electron_temp.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from typing import Union
 
 import xarray as xr
 
 from ...unit_handling import Quantity
 
 
-def calc_upstream_electron_temp(
+def calc_separatrix_electron_temp(
     target_electron_temp: Union[Quantity, xr.DataArray],
     parallel_heat_flux_density: Union[Quantity, xr.DataArray],
     parallel_connection_length: Union[Quantity, xr.DataArray],
     kappa_e0: Union[Quantity, xr.DataArray],
     SOL_conduction_fraction: Union[float, xr.DataArray] = 1.0,
 ) -> Union[Quantity, xr.DataArray]:
-    """Calculate the upstream electron temperature.
+    """Calculate the upstream electron temperature assuming Spitzer-Harm heat conductivity.
 
     Equation 38 from :cite:`stangeby_2018`, keeping the dependence on target_electron_temp.
 
     Args:
         target_electron_temp: [eV]
         parallel_heat_flux_density: [GW/m^2]
         parallel_connection_length: [m]
         kappa_e0: [W / (eV**3.5 m)]
         SOL_conduction_fraction: [eV]
 
     Returns:
-        upstream_electron_temp [eV]
+        separatrix_electron_temp [eV]
     """
     return (
         target_electron_temp**3.5 + 3.5 * (SOL_conduction_fraction * parallel_heat_flux_density * parallel_connection_length / kappa_e0)
     ) ** (2.0 / 7.0)
```

### Comparing `cfspopcon-4.0.0/cfspopcon/helpers.py` & `cfspopcon-5.0.0/cfspopcon/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,59 @@
 """Constructors and helper functions."""
 from typing import Any, Union
 
 import xarray as xr
 
 from .named_options import (
-    Algorithms,
-    ConfinementScaling,
-    Impurity,
+    AtomicSpecies,
     LambdaQScaling,
     MomentumLossFunction,
     ProfileForm,
     RadiationMethod,
-    ReactionType,
 )
 
 
-def convert_named_options(key: str, val: Any) -> Any:  # noqa: PLR0911, PLR0912
+def convert_named_options(key: str, val: Any) -> Any:  # noqa: PLR0911
     """Given a 'key' matching a named_option, return the corresponding Enum value."""
-    if key == "algorithms":
-        return Algorithms[val]
-    elif key == "energy_confinement_scaling":
-        return ConfinementScaling[val]
-    elif key == "profile_form":
+    if key == "profile_form":
         return ProfileForm[val]
     elif key == "radiated_power_method":
         return RadiationMethod[val]
-    elif key == "fusion_reaction":
-        return ReactionType[val]
     elif key == "impurity":
-        return Impurity[val]
+        return AtomicSpecies[val]
     elif key == "impurities":
         return make_impurities_array(list(val.keys()), list(val.values()))
     elif key == "core_radiator":
-        return Impurity[val]
+        return AtomicSpecies[val]
+    elif key == "edge_impurity_species":
+        return AtomicSpecies[val]
     elif key == "lambda_q_scaling":
         return LambdaQScaling[val]
     elif key == "SOL_momentum_loss_function":
         return MomentumLossFunction[val]
-    elif key == "tauE_scaling":
-        return ConfinementScaling[val]
-    elif key == "reaction_type":
-        return ReactionType[val]
     elif key == "radiation_method":
         return RadiationMethod[val]
     else:
         # If the key doesn't match, don't convert the value
         return val
 
 
 def make_impurities_array(
-    species_list: Union[list[Union[str, Impurity]], Union[str, Impurity]],
+    species_list: Union[list[Union[str, AtomicSpecies]], Union[str, AtomicSpecies]],
     concentrations_list: Union[list[Union[float, xr.DataArray]], Union[float, xr.DataArray]],
 ) -> xr.DataArray:
     """Make an xr.DataArray with impurity species and their corresponding concentrations.
 
     This array should be used as the `impurities` variable.
     """
-    # Convert DataArrays of species into plain lists. This is useful if you want to store Impurity objects in a dataset.
+    # Convert DataArrays of species into plain lists. This is useful if you want to store AtomicSpecies objects in a dataset.
     if isinstance(species_list, (xr.DataArray)):
         species_list = species_list.values.tolist()
     # Deal with single-value input (not recommended, but avoids a confusing user error)
-    if isinstance(species_list, (str, Impurity)):
+    if isinstance(species_list, (str, AtomicSpecies)):
         species_list = [
             species_list,
         ]
     if isinstance(concentrations_list, (float, xr.DataArray)):
         concentrations_list = [
             concentrations_list,
         ]
@@ -80,26 +69,31 @@
 
 
 def make_impurities_array_from_kwargs(**kwargs: Any) -> xr.DataArray:
     """Make an xr.DataArray with impurity species and their corresponding concentrations, using the format (species1=concentration1, ...)."""
     return make_impurities_array(list(kwargs.keys()), list(kwargs.values()))
 
 
-def extend_impurities_array(array: xr.DataArray, species: Union[str, Impurity], concentration: Union[float, xr.DataArray]) -> xr.DataArray:
+def extend_impurities_array(
+    array: xr.DataArray, species: Union[str, AtomicSpecies], concentration: Union[float, xr.DataArray]
+) -> xr.DataArray:
     """Append a new element to the impurities array.
 
     This method automatically handles broadcasting.
 
     N.b. You can also 'extend' an empty array, constructed via xr.DataArray()
     """
-    if not isinstance(species, Impurity):
-        species = Impurity[species.capitalize()]
+    if isinstance(species, xr.DataArray):
+        species = species.item()
+
+    if not isinstance(species, AtomicSpecies):
+        species = AtomicSpecies[species.capitalize()]
 
     if not isinstance(concentration, xr.DataArray):
         concentration = xr.DataArray(concentration)
     concentration = concentration.expand_dims("dim_species").assign_coords(dim_species=[species])
 
     if array.ndim == 0:
         return concentration
     else:
         other_species = array.sel(dim_species=[s for s in array.dim_species if s != species])
-        return xr.concat((other_species, concentration), dim="dim_species")
+        return xr.concat((other_species, concentration), dim="dim_species").sortby("dim_species")
```

### Comparing `cfspopcon-4.0.0/cfspopcon/plotting/coordinate_formatter.py` & `cfspopcon-5.0.0/cfspopcon/plotting/coordinate_formatter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Adds a readout of the field at the current mouse position for a colormapped field plotted with pcolormesh, contour, quiver, etc.
 
 Usage:
->>> fig, ax = plt.subplots()
->>> ax.format_coord = CoordinateFormatter(x, y, z)
+    >>> import matplotlib.pyplot as plt
+    >>> from cfspopcon.plotting import CoordinateFormatter
+    >>> fig, ax = plt.subplots()
+    >>> ax.format_coord = CoordinateFormatter(...)
 """
 import xarray as xr
 
 
 class CoordinateFormatter:
     """Data storage object used for providing a coordinate formatter."""
```

### Comparing `cfspopcon-4.0.0/cfspopcon/plotting/make_plot.py` & `cfspopcon-5.0.0/cfspopcon/plotting/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,39 +5,45 @@
 import matplotlib
 import matplotlib.contour
 import matplotlib.pyplot as plt
 import numpy as np
 import xarray as xr
 from matplotlib.axes import Axes
 
-from cfspopcon import __version__
-
-from ..point_selection import build_mask_from_dict, find_coords_of_minimum
-from ..transform import build_transform_function_from_dict
+from ..shaping_and_selection.point_selection import build_mask_from_dict, find_coords_of_minimum
+from ..shaping_and_selection.transform_coords import build_transform_function_from_dict
 from ..unit_handling import Quantity, Unit, dimensionless_magnitude
 from .coordinate_formatter import CoordinateFormatter
 
 
 def make_plot(
-    dataset: xr.Dataset, plot_params: dict, points: dict, title: str, ax: Optional[Axes] = None, output_dir: Path = Path(".")
+    dataset: xr.Dataset,
+    plot_params: dict,
+    points: dict,
+    title: str,
+    save_name: Optional[str] = None,
+    ax: Optional[Axes] = None,
+    output_dir: Path = Path("."),
 ) -> None:
     """Given a dictionary corresponding to a plotting style, build a standard plot from the results of the POPCON."""
     if plot_params["type"] == "popcon":
         if ax is None:
             _, ax = plt.subplots(figsize=plot_params["figsize"], dpi=plot_params["show_dpi"])
         fig, ax = make_popcon_plot(dataset, title, plot_params, points, ax=ax)
     else:
         raise NotImplementedError(f"No plotting method for type '{plot_params['type']}'")
 
-    if "save_as" in plot_params.keys() and output_dir is not None:
-        fig.savefig(output_dir / plot_params["save_as"])
+    if save_name is not None:
+        fig.savefig(output_dir / save_name)
 
 
 def make_popcon_plot(dataset: xr.Dataset, title: str, plot_params: dict, points: dict, ax: Axes):
     """Make a plot."""
+    from cfspopcon import __version__
+
     fig = ax.figure
     transform_func = build_transform_function_from_dict(dataset, plot_params)
 
     coords = plot_params["coords"] if "coords" in plot_params else plot_params["new_coords"]
     legend_elements = dict()
 
     if "fill" in plot_params:
@@ -61,15 +67,14 @@
             labelpad=subplot_params.get("labelpad", 15.0),
         )
 
     if "contour" in plot_params:
         # Overlay contour plots
 
         for variable, subplot_params in plot_params["contour"].items():
-
             field = dataset[variable]
             units = subplot_params.get("units", field.pint.units)
             field = field.pint.to(units)
 
             mask = build_mask_from_dict(dataset, plot_params=subplot_params)
             transformed_field = transform_func(field.where(mask))
 
@@ -133,17 +138,14 @@
 
 
 def label_contour(ax: plt.Axes, contour_set: matplotlib.contour.QuadContourSet, format_spec: str = "1.1f", fontsize: float = 10.0):
     """Add in-line labels to contours.
 
     Returns the first label element, which can be used to construct a legend.
     Works best with contour sets with only one color.
-    >>> contour_labels = dict()
-    >>> contour_labels["key"] = label_contour(...)
-    >>> ax.legend(contour_labels.values(), contour_labels.keys())
 
     Inputs:
         ax: the matplotlib axis of the contour plot
         contour_set: the return argument of plt.contour(...)
         format_spec: a format specification for the string formatting
         fontsize: the font size of the label
     """
```

### Comparing `cfspopcon-4.0.0/cfspopcon/plotting/plot_style_handling.py` & `cfspopcon-5.0.0/cfspopcon/plotting/plot_style_handling.py`

 * *Files identical despite different names*

### Comparing `cfspopcon-4.0.0/cfspopcon/point_selection.py` & `cfspopcon-5.0.0/cfspopcon/shaping_and_selection/point_selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,57 +2,54 @@
 from collections.abc import Sequence
 from typing import Optional
 
 import numpy as np
 import xarray as xr
 from xarray.core.coordinates import DataArrayCoordinates
 
-from .unit_handling import Quantity
+from ..unit_handling import Quantity
 
 
 def find_coords_of_minimum(array: xr.DataArray, keep_dims: Sequence[str] = [], mask: Optional[xr.DataArray] = None) -> DataArrayCoordinates:
     """Find the coordinates the minimum value of array.
 
     These coordinates can be used to find the value of other arrays at the same point.
 
     For example
-    >>> import xarray as xr
-    >>> import matplotlib.pyplot as plt
-    >>> import numpy as np
-    >>> from cfspopcon.operational_space import find_coords_of_minimum
-    >>> x = xr.DataArray(np.linspace(0, 1, num=10), dims="x")
-    >>> y = xr.DataArray(np.linspace(-1, 1, num=20), dims="y")
-    >>> z = xr.DataArray(np.abs(x + y), coords=dict(x=x, y=y))
-    >>> z.T.plot()
-    >>> line = z.isel(find_coords_of_minimum(z, keep_dims="y"))
-    >>> plt.scatter(line.x, line.y)
+        >>> import xarray as xr
+        >>> import numpy as np
+        >>> from cfspopcon.point_selection import find_coords_of_minimum
+        >>> x = xr.DataArray(np.linspace(0, 1, num=10), dims="x")
+        >>> y = xr.DataArray(np.linspace(-1, 1, num=20), dims="y")
+        >>> z = xr.DataArray(np.abs(x + y), coords=dict(x=x, y=y))
+        >>> line = z.isel(find_coords_of_minimum(z, keep_dims="y"))
     """
     large = Quantity(np.inf, array.pint.units)
 
-    along_dims = [dim for dim in array.dims if dim not in keep_dims]
-
     if mask is None:
-        point_coords = array.fillna(large).argmin(dim=along_dims)
+        masked_array = array.fillna(large)
     else:
-        point_coords = array.where(mask).fillna(large).argmin(dim=along_dims)
+        masked_array = array.where(mask).fillna(large)
+
+    along_dims = [dim for dim in masked_array.dims if dim not in keep_dims]
+    point_coords = masked_array.argmin(dim=along_dims)
 
     return point_coords  # type:ignore[return-value]
 
 
 def find_coords_of_maximum(array: xr.DataArray, keep_dims: Sequence[str] = [], mask: Optional[xr.DataArray] = None) -> DataArrayCoordinates:
     """Find the coordinates of the maximum value of array."""
     return find_coords_of_minimum(-array, keep_dims=keep_dims, mask=mask)
 
 
 def build_mask_from_dict(dataset: xr.Dataset, plot_params: dict) -> xr.DataArray:
     """Build a mask field which hides inaccessible parts of the operational space."""
     mask = xr.DataArray(True)
 
     for mask_key, mask_range in plot_params.get("where", dict()).items():
-
         mask_field = dataset[mask_key]
         mask_min = Quantity(mask_range.get("min", -np.inf), mask_range.get("units", ""))
         mask_max = Quantity(mask_range.get("max", +np.inf), mask_range.get("units", ""))
 
         mask = mask & ((mask_field > mask_min) & (mask_field < mask_max))
 
     return mask
```

### Comparing `cfspopcon-4.0.0/cfspopcon/transform.py` & `cfspopcon-5.0.0/cfspopcon/shaping_and_selection/transform_coords.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Functions to reshape xarrays."""
 from collections.abc import Sequence
 from typing import Callable, Optional, Union
 
 import numpy as np
 import xarray as xr
-from scipy.interpolate import griddata  # type:ignore[import]
+from scipy.interpolate import griddata  # type:ignore[import-untyped]
 
 from cfspopcon.unit_handling import Unit, magnitude
 
 
 def order_dimensions(
     array: xr.DataArray,
     dims: Sequence[str],
@@ -114,17 +114,17 @@
         # Iterate over each grid point
         mesh_point = [mesh_coords[dimension][index] for dimension in range(len(index))]
         broadcast_mesh_point = np.broadcast_to(np.expand_dims(mesh_point, axis=-1), stacked_samples.shape)
 
         distance_to_points = ((broadcast_mesh_point - stacked_samples) / spacing) ** 2
         distance_to_nearest[index] = np.min(np.sum(distance_to_points, axis=0))
 
-    clipped_array = interpolated_array.where(distance_to_nearest < max_distance).clip(min=array.min(), max=array.max())
+    clipped_array: xr.DataArray = interpolated_array.where(distance_to_nearest < max_distance).clip(min=array.min(), max=array.max())
 
-    return clipped_array  # type:ignore[no-any-return]
+    return clipped_array
 
 
 def build_transform_function_from_dict(dataset: xr.Dataset, plot_params: dict) -> Callable[[xr.DataArray], xr.DataArray]:
     """Build a function which can be called on a field to return an array with transformed coordinates.
 
     The simplest function is a transpose function, which makes sure that the dimensions are correctly ordered
     for plotting.
```

### Comparing `cfspopcon-4.0.0/cfspopcon/unit_handling/__init__.py` & `cfspopcon-5.0.0/cfspopcon/unit_handling/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 """Uses pint and xarray to enable unit-handling over multi-dimensional arrays."""
 from typing import Union
 
 import xarray as xr
-from pint import DimensionalityError, UnitStrippedWarning
+from pint import DimensionalityError, UndefinedUnitError, UnitStrippedWarning
 
 from .decorator import wraps_ufunc
 from .default_units import convert_to_default_units, default_unit, magnitude_in_default_units, set_default_units
-from .setup_unit_handling import Quantity, Unit, convert_units, dimensionless_magnitude, magnitude, ureg
+from .setup_unit_handling import (
+    Quantity,
+    Unit,
+    convert_units,
+    dimensionless_magnitude,
+    get_units,
+    magnitude,
+    magnitude_in_units,
+    ureg,
+)
 
 Unitfull = Union[Quantity, xr.DataArray]
 
 __all__ = [
     "ureg",
     "Quantity",
     "Unit",
     "Unitfull",
     "wraps_ufunc",
     "magnitude_in_default_units",
+    "magnitude_in_units",
     "set_default_units",
     "default_unit",
     "convert_to_default_units",
     "convert_units",
     "magnitude",
     "dimensionless_magnitude",
-    "DimensionalityError",
     "UnitStrippedWarning",
+    "UndefinedUnitError",
+    "DimensionalityError",
+    "get_units",
 ]
```

### Comparing `cfspopcon-4.0.0/cfspopcon/unit_handling/decorator.py` & `cfspopcon-5.0.0/cfspopcon/unit_handling/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,14 @@
             raise ValueError(
                 f"input_core_dims (len {len(input_core_dims)}) must the same length as positional_args ({pass_as_positional_args}, len {len(pass_as_positional_args)})"
             )
     else:
         input_core_dims = len(pass_as_positional_args) * [()]
 
     def _wraps_ufunc(func: FunctionType) -> FunctionType:
-
         func_signature = signature(func)
         func_parameters = func_signature.parameters
 
         if not list(input_units.keys()) == list(func_parameters.keys()):
             raise ValueError(
                 f"Keys for input_units {input_units.keys()} did not match func_parameters {func_parameters.keys()} (n.b. order matters!)"
             )
@@ -171,28 +170,26 @@
         popcon_ufunc_wrapped_call.__signature__ = _make_new_sig(func_signature, input_units, return_units)  # type:ignore[attr-defined]
         return popcon_ufunc_wrapped_call
 
     return _wraps_ufunc
 
 
 def _check_units(units_dict: dict[str, Union[str, Unit, None]]) -> dict[str, Union[str, Unit, None]]:
-
     for key, unit in units_dict.items():
         if unit is None:
             pass
         elif isinstance(unit, str):
             units_dict[key] = ureg(unit).units
         elif not isinstance(unit, Unit):
             raise TypeError(f"wraps_ufunc units for {key} must by of type str or Unit, not {str(type(unit))[1:-1]} (value was {unit})")
 
     return units_dict
 
 
 def _return_magnitude_in_specified_units(vals: Any, units_mapping: dict[str, Union[str, Unit, None]]) -> dict[str, Any]:
-
     if not set(vals.keys()) == set(units_mapping):
         raise ValueError(f"Argument keys {vals.keys()} did not match units_mapping keys {units_mapping.keys()}")
 
     converted_vals = {}
 
     for key in vals.keys():
         val = vals[key]
@@ -213,15 +210,14 @@
         else:
             raise NotImplementedError(f"Cannot convert {key} of type {str(type(val))[1:-1]} to units {unit}")
 
     return converted_vals
 
 
 def _convert_return_to_quantities(vals: Any, units_mapping: dict[str, Union[str, Unit, None]]) -> dict[str, Any]:
-
     if not isinstance(vals, tuple):
         vals = (vals,)
 
     if not len(vals) == len(units_mapping):
         raise ValueError(f"Number of returned values ({len(vals)}) did not match length of units_mapping ({len(units_mapping)})")
     vals = dict(zip(units_mapping.keys(), vals))
 
@@ -271,21 +267,29 @@
         old_types: list[Any] = list(ret_annotation.__args__)
     elif ret_annotation == Parameter.empty:
         old_types = [Any for _ in range(len(units_list))]
     else:
         old_types = [ret_annotation]
 
     if len(old_types) != len(units_list):
-        warnings.warn(
-            (
-                f"Return type annotation {ret_annotation} has {len(old_types)} return values"
-                f", while the return_units: {return_units} specifies {len(return_units)} values"
-            ),
-            stacklevel=3,
-        )
+        if not (
+            # Catches an error where some multiple-return types are handled as strings. These can
+            # be safely ignored.
+            isinstance(ret_annotation, str)
+            and ret_annotation.startswith("tuple")
+            and len(ret_annotation.removeprefix("tuple[").removesuffix("]").split(",")) == len(units_list)
+        ):
+            warnings.warn(
+                (
+                    f"Return type annotation {ret_annotation} has {len(old_types)} return values"
+                    f", while the return_units: {return_units} specifies {len(return_units)} values"
+                ),
+                stacklevel=3,
+            )
+
     ret_types = tuple(xr.DataArray if units_list[i] is not None else old_types[i] for i in range(len(units_list)))
 
     if len(ret_types) == 0:
         new_ret_ann: Union[type, None, GenericAlias] = None
     elif len(ret_types) == 1:
         new_ret_ann = ret_types[0]
     else:
```

### Comparing `cfspopcon-4.0.0/cfspopcon/unit_handling/setup_unit_handling.py` & `cfspopcon-5.0.0/cfspopcon/unit_handling/setup_unit_handling.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 from collections.abc import Callable
 from functools import wraps
 from typing import Any, TypeVar, Union, overload
 
 import numpy as np
 import numpy.typing as npt
 import pint
-import pint_xarray  # type:ignore[import]
+import pint_xarray  # type:ignore[import-untyped]
 import xarray as xr
-from pint.errors import DimensionalityError
 from typing_extensions import ParamSpec
 
 ureg = pint_xarray.setup_registry(
     pint.UnitRegistry(
         force_ndarray_like=True,
-        cache_folder=":auto:",
     )
 )
 
 Quantity = ureg.Quantity
 Unit = ureg.Unit
 
 Params = ParamSpec("Params")
@@ -54,45 +52,54 @@
 @overload
 def convert_units(array: pint.Quantity, units: Union[str, pint.Unit]) -> pint.Quantity:
     ...
 
 
 def convert_units(array: Union[xr.DataArray, pint.Quantity], units: Any) -> Union[xr.DataArray, pint.Quantity]:
     """Convert an array to specified units, handling both Quantities and xr.DataArrays."""
+    if units is None:
+        # Replace None with ureg.dimensionless.
+        # Otherwise, convert_units(Quantity([1.0], ""), None) will fail with an AttributeError
+        units = ureg.dimensionless
+
     if isinstance(array, xr.DataArray):
         if not hasattr(array.pint, "units") or array.pint.units is None:
             array = array.pint.quantify(ureg.dimensionless)
 
         return array.pint.to(units)  # type: ignore[no-any-return]
     elif isinstance(array, Quantity):
         return array.to(units)  # type:ignore[no-any-return]
+    elif isinstance(array, float) and Quantity(1.0, units).check("[]"):
+        return (array * ureg.dimensionless).to(units)
     else:
         raise NotImplementedError(f"No implementation for 'convert_units' with an array of type {type(array)} ({array})")
 
 
 @suppress_downcast_warning
 def magnitude(array: Union[xr.DataArray, pint.Quantity]) -> Union[npt.NDArray[np.float32], float]:
     """Return the magnitude of an array, handling both Quantities and xr.DataArrays."""
     if isinstance(array, xr.DataArray):
-        return array.values
+        return array.pint.dequantify()  # type: ignore[no-any-return]
     elif isinstance(array, Quantity):
         return array.magnitude  # type: ignore[no-any-return]
     else:
         raise NotImplementedError(f"No implementation for 'magnitude' with an array of type {type(array)} ({array})")
 
 
-def dimensionless_magnitude(array: Union[xr.DataArray, pint.Quantity]) -> Union[npt.NDArray[np.float32], float]:
-    """Converts the array to dimensionless and returns the magnitude."""
-    return magnitude(convert_units(array, ureg.dimensionless))
+def get_units(array: Union[xr.DataArray, pint.Quantity]) -> Any:
+    """Returns the unit of an array, handling both Quantities and xr.DataArrays."""
+    if isinstance(array, xr.DataArray):
+        return array.pint.units
+    elif isinstance(array, Quantity):
+        return array.units
+    else:
+        raise NotImplementedError(f"No implementation for 'get_units' with an array of type {type(array)} ({array})")
+
+
+def magnitude_in_units(array: Union[xr.DataArray, pint.Quantity], units: Any) -> Union[npt.NDArray[np.float32], float]:
+    """Convert the array to the specified units and then return the magnitude."""
+    return magnitude(convert_units(array, units))
 
 
-__all__ = [
-    "DimensionalityError",
-    "ureg",
-    "Quantity",
-    "Unit",
-    "suppress_downcast_warning",
-    "convert_units",
-    "magnitude",
-    "suppress_downcast_warning",
-    "dimensionless_magnitude",
-]
+def dimensionless_magnitude(array: Union[xr.DataArray, pint.Quantity]) -> Union[npt.NDArray[np.float32], float]:
+    """Converts the array to dimensionless and returns the magnitude."""
+    return magnitude_in_units(array, ureg.dimensionless)
```

### Comparing `cfspopcon-4.0.0/pyproject.toml` & `cfspopcon-5.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.black]
 line-length = 140
 target-version = ['py39', 'py310', 'py311']
 
 [tool.poetry]
 name = "cfspopcon"
-version = "4.0.0"
+version = "5.0.0"
 description = "Empirically-derived scoping of tokamak operational space."
 authors = ["Commonwealth Fusion Systems"]
 readme = "README.md"
 classifiers = [
 "Development Status :: 5 - Production/Stable",
 "Intended Audience :: Science/Research",
 "Programming Language :: Python :: 3",
@@ -19,14 +19,15 @@
 "Topic :: Scientific/Engineering :: Physics",
 "License :: OSI Approved :: MIT License",
 ]
 
 
 [tool.poetry.scripts]
 popcon = 'cfspopcon.cli:run_popcon_cli'
+popcon_algorithms = 'cfspopcon.cli:write_algorithms_yaml'
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 numpy = "^1.22.4"
 pandas = "^1.4"
 scipy = "^1.8"
 seaborn = "^0.12"
@@ -34,26 +35,29 @@
 toml = "^0.10.2"
 typing-extensions = "^4.0.1"
 pint = "^0.22"
 xarray = "^2023.4.1"
 pint-xarray = "^0.3"
 ipdb = "^0.13.13"
 click = "^8.1.0"
+netcdf4 = "^1.6.5"
+radas = "^2024.3.1"
+contourpy = "^1.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 black = "^22.10.0"
 pytest = "^7.2.0"
 coverage = "^6.5.0"
 pytest-cov = "^4.0.0"
 types-pyyaml = "^6.0.12.2"
 pandas-stubs = "^1.5.1.221024"
 mypy = "^1.4.1"
-sphinx = "^7.2.6"
-sphinx-rtd-theme = "^2.0.0rc2"
+sphinx = "^7.3.7"
+sphinx-rtd-theme = "^2.0.0"
 sphinxcontrib-bibtex = "^2.6.1"
 sphinx-copybutton = "^0.5.2"
 ruff = "^0.0.292"
 nbmake = "^1.4.3"
 nbsphinx = "^0.9.3"
 
 [tool.coverage.report]
@@ -61,14 +65,19 @@
 
 [tool.pytest.ini_options]
 addopts = "--cov=cfspopcon --cov-report term-missing --cov-report xml:coverage.xml --verbose -s --nbmake"
 testpaths = [
   "tests",
   "docs/doc_sources"
 ]
+markers = [
+    "docs: marks tests as testing the documentation (deselect with '-m \"not docs\"')",
+    "cli: marks tests as testing the command-line-interface (deselect with '-m \"not cli\"')",
+    "regression: marks tests as checking the regression result (deselect with '-m \"not regression\"')",
+]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 plugins = "numpy.typing.mypy_plugin"
```

