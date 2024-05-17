# Comparing `tmp/autotuning_methodology-1.0.0b2.tar.gz` & `tmp/autotuning_methodology-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotuning_methodology-1.0.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "autotuning_methodology-1.0.0b3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `autotuning_methodology-1.0.0b2.tar` & `autotuning_methodology-1.0.0b3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0      112 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.coveragerc
--rw-r--r--   0        0        0     1424 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.github/workflows/build-test-python-package.yml
--rw-r--r--   0        0        0      658 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.github/workflows/publish-documentation.yml
--rw-r--r--   0        0        0     1227 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.github/workflows/publish-package.yml
--rwxr-xr-x   0        0        0     3571 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.gitignore
--rw-r--r--   0        0        0      144 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.vscode/extensions.json
--rw-r--r--   0        0        0      605 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.vscode/settings.json
--rw-r--r--   0        0        0     1077 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/LICENSE
--rw-r--r--   0        0        0     7566 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/README.md
--rw-r--r--   0        0        0     2597 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/UML/.$Sequence Diagram.drawio.bkp
--rw-r--r--   0        0        0   302745 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/UML/.$flowchart.drawio.bkp
--rw-r--r--   0        0        0     2585 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/UML/Sequence Diagram.drawio
--rw-r--r--   0        0        0    26889 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/UML/classes.pdf
--rw-r--r--   0        0        0   303637 2024-05-15 09:37:30.284802 autotuning_methodology-1.0.0b2/UML/flowchart/.$flowchart.drawio.bkp
--rw-r--r--   0        0        0   303637 2024-05-15 09:37:30.284802 autotuning_methodology-1.0.0b2/UML/flowchart/flowchart.drawio
--rw-r--r--   0        0        0   315705 2024-05-15 09:37:30.284802 autotuning_methodology-1.0.0b2/UML/flowchart/flowchart_output_generation.png
--rw-r--r--   0        0        0   267296 2024-05-15 09:37:30.284802 autotuning_methodology-1.0.0b2/UML/flowchart/flowchart_performance_curve_generation.png
--rw-r--r--   0        0        0   131133 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plot_aggregated.png
--rw-r--r--   0        0        0    95756 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plot_individual.png
--rw-r--r--   0        0        0     1074 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plots.py
--rw-r--r--   0        0        0    15114 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/UML/packages.pdf
--rw-r--r--   0        0        0     5736 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py
--rw-r--r--   0        0        0      634 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/Makefile
--rw-r--r--   0        0        0     1722 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/autotuning_methodology.rst
--rw-r--r--   0        0        0     2541 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/conf.py
--rw-r--r--   0        0        0     2225 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/contributing.rst
--rw-r--r--   0        0        0     2409 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/getting_started.rst
--rw-r--r--   0        0        0     1144 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/index.rst
--rw-r--r--   0        0        0      800 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/make.bat
--rw-r--r--   0        0        0   609663 2024-05-15 09:37:30.292802 autotuning_methodology-1.0.0b2/docs/source/example_aggregated.png
--rw-r--r--   0        0        0   315705 2024-05-15 09:37:30.292802 autotuning_methodology-1.0.0b2/docs/source/flowchart_output_generation.png
--rw-r--r--   0        0        0   267296 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/flowchart_performance_curve_generation.png
--rw-r--r--   0        0        0     5034 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/logo_autotuning_methodology.svg
--rw-r--r--   0        0        0    36351 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/logo_kernel_dashboard.svg
--rw-r--r--   0        0        0    42513 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/logo_kernel_launcher.svg
--rw-r--r--   0        0        0    39816 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/logo_kernel_tuner.svg
--rwxr-xr-x   0        0        0      983 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/bootstrap_hyperparams.json
--rw-r--r--   0        0        0     1625 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/example_visualizations.json
--rw-r--r--   0        0        0     1971 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/methodology_paper_evaluation.json
--rw-r--r--   0        0        0     1647 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/milo_hotspot.json
--rw-r--r--   0        0        0     1403 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/presentation_comparison.json
--rw-r--r--   0        0        0     2364 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/simple_example.json
--rw-r--r--   0        0        0     1745 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/test_random_calculated.json
--rw-r--r--   0        0        0     1409 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/test_scatter.json
--rwxr-xr-x   0        0        0     2275 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/test_searchspace_algorithms.json
--rw-r--r--   0        0        0      132 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/.vscode/settings.json
--rwxr-xr-x   0        0        0    18897 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/bootstrap_hyperparams_visualizer.py
--rwxr-xr-x   0        0        0    19811 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/experiments_strategies.py
--rwxr-xr-x   0        0        0   119690 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/experiments_strategies_hyperparamtuning.py
--rwxr-xr-x   0        0        0     7475 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/generate_cachefile.py
--rw-r--r--   0        0        0    20608 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/max_draw_k_from_n.py
--rw-r--r--   0        0        0     3259 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/speedtest_index_performance.py
--rw-r--r--   0        0        0     1174 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/speedtest_python_reversed_nan_sort.py
--rwxr-xr-x   0        0        0     2545 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/try_BOtorch.py
--rwxr-xr-x   0        0        0     8426 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/try_GPytorch.py
--rw-r--r--   0        0        0    20822 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/try_isotonic_regression.py
--rwxr-xr-x   0        0        0      435 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/mypy.ini
--rw-r--r--   0        0        0     1089 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/noxfile.py
--rwxr-xr-x   0        0        0       17 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/profilings/.gitignore
--rw-r--r--   0        0        0     2816 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0       95 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/__init__.py
--rw-r--r--   0        0        0    17647 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/baseline.py
--rwxr-xr-x   0        0        0     8418 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/caching.py
--rw-r--r--   0        0        0    51986 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/curves.py
--rwxr-xr-x   0        0        0     9764 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/experiments.py
--rwxr-xr-x   0        0        0    24377 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/runner.py
--rwxr-xr-x   0        0        0     4138 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/schema.json
--rw-r--r--   0        0        0    25701 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/searchspace_statistics.py
--rw-r--r--   0        0        0     1787 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/validators.py
--rwxr-xr-x   0        0        0    48490 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/visualize_experiments.py
--rw-r--r--   0        0        0  3269061 2024-05-15 09:37:30.308802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json
--rw-r--r--   0        0        0  3255846 2024-05-15 09:37:30.312802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json
--rw-r--r--   0        0        0  3483805 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json
--rw-r--r--   0        0        0     2967 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py
--rw-r--r--   0        0        0     1489 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test.json
--rw-r--r--   0        0        0     1476 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json
--rw-r--r--   0        0        0     1465 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_cached.json
--rw-r--r--   0        0        0     1453 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json
--rw-r--r--   0        0        0     8913 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/test_run_experiment.py
--rw-r--r--   0        0        0     2934 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/test_visualization.py
--rw-r--r--   0        0        0     1978 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/release/test_toml_file.py
--rw-r--r--   0        0        0       34 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/unit/test_caching.py
--rw-r--r--   0        0        0     3464 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/unit/test_curves.py
--rw-r--r--   0        0        0     9534 1970-01-01 00:00:00.000000 autotuning_methodology-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0      112 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/.coveragerc
+-rw-r--r--   0        0        0     1424 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/.github/workflows/build-test-python-package.yml
+-rw-r--r--   0        0        0      658 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/.github/workflows/publish-documentation.yml
+-rw-r--r--   0        0        0     1227 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/.github/workflows/publish-package.yml
+-rwxr-xr-x   0        0        0     3571 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/.gitignore
+-rw-r--r--   0        0        0      144 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/.vscode/extensions.json
+-rw-r--r--   0        0        0      605 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/.vscode/settings.json
+-rw-r--r--   0        0        0     1077 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0     7852 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/README.md
+-rw-r--r--   0        0        0     2597 2024-05-17 06:54:13.640654 autotuning_methodology-1.0.0b3/UML/.$Sequence Diagram.drawio.bkp
+-rw-r--r--   0        0        0   302745 2024-05-17 06:54:13.644654 autotuning_methodology-1.0.0b3/UML/.$flowchart.drawio.bkp
+-rw-r--r--   0        0        0     2585 2024-05-17 06:54:13.644654 autotuning_methodology-1.0.0b3/UML/Sequence Diagram.drawio
+-rw-r--r--   0        0        0    26889 2024-05-17 06:54:13.644654 autotuning_methodology-1.0.0b3/UML/classes.pdf
+-rw-r--r--   0        0        0   303637 2024-05-17 06:54:13.644654 autotuning_methodology-1.0.0b3/UML/flowchart/.$flowchart.drawio.bkp
+-rw-r--r--   0        0        0   303637 2024-05-17 06:54:13.648654 autotuning_methodology-1.0.0b3/UML/flowchart/flowchart.drawio
+-rw-r--r--   0        0        0   315705 2024-05-17 06:54:13.648654 autotuning_methodology-1.0.0b3/UML/flowchart/flowchart_output_generation.png
+-rw-r--r--   0        0        0   267296 2024-05-17 06:54:13.648654 autotuning_methodology-1.0.0b3/UML/flowchart/flowchart_performance_curve_generation.png
+-rw-r--r--   0        0        0   131133 2024-05-17 06:54:13.648654 autotuning_methodology-1.0.0b3/UML/flowchart/mini_plots/flowchart_plot_aggregated.png
+-rw-r--r--   0        0        0    95756 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/UML/flowchart/mini_plots/flowchart_plot_individual.png
+-rw-r--r--   0        0        0     1074 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/UML/flowchart/mini_plots/flowchart_plots.py
+-rw-r--r--   0        0        0    15114 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/UML/packages.pdf
+-rw-r--r--   0        0        0     5736 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py
+-rw-r--r--   0        0        0      634 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/docs/Makefile
+-rw-r--r--   0        0        0     1722 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/docs/autotuning_methodology.rst
+-rw-r--r--   0        0        0     2541 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/docs/conf.py
+-rw-r--r--   0        0        0     2225 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/docs/contributing.rst
+-rw-r--r--   0        0        0     2409 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/docs/getting_started.rst
+-rw-r--r--   0        0        0     1144 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-17 06:54:13.652654 autotuning_methodology-1.0.0b3/docs/make.bat
+-rw-r--r--   0        0        0   609663 2024-05-17 06:54:13.656654 autotuning_methodology-1.0.0b3/docs/source/example_aggregated.png
+-rw-r--r--   0        0        0   315705 2024-05-17 06:54:13.656654 autotuning_methodology-1.0.0b3/docs/source/flowchart_output_generation.png
+-rw-r--r--   0        0        0   267296 2024-05-17 06:54:13.656654 autotuning_methodology-1.0.0b3/docs/source/flowchart_performance_curve_generation.png
+-rw-r--r--   0        0        0     5034 2024-05-17 06:54:13.656654 autotuning_methodology-1.0.0b3/docs/source/logo_autotuning_methodology.svg
+-rw-r--r--   0        0        0    36351 2024-05-17 06:54:13.656654 autotuning_methodology-1.0.0b3/docs/source/logo_kernel_dashboard.svg
+-rw-r--r--   0        0        0    42513 2024-05-17 06:54:13.656654 autotuning_methodology-1.0.0b3/docs/source/logo_kernel_launcher.svg
+-rw-r--r--   0        0        0    39816 2024-05-17 06:54:13.656654 autotuning_methodology-1.0.0b3/docs/source/logo_kernel_tuner.svg
+-rwxr-xr-x   0        0        0      983 2024-05-17 06:54:13.656654 autotuning_methodology-1.0.0b3/experiment_files/bootstrap_hyperparams.json
+-rw-r--r--   0        0        0     1625 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/experiment_files/example_visualizations.json
+-rw-r--r--   0        0        0     1971 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/experiment_files/methodology_paper_evaluation.json
+-rw-r--r--   0        0        0     1647 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/experiment_files/milo_hotspot.json
+-rw-r--r--   0        0        0     1403 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/experiment_files/presentation_comparison.json
+-rw-r--r--   0        0        0     2364 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/experiment_files/simple_example.json
+-rw-r--r--   0        0        0     1745 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/experiment_files/test_random_calculated.json
+-rw-r--r--   0        0        0     1409 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/experiment_files/test_scatter.json
+-rwxr-xr-x   0        0        0     2275 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/experiment_files/test_searchspace_algorithms.json
+-rw-r--r--   0        0        0      132 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/.vscode/settings.json
+-rwxr-xr-x   0        0        0    18897 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/bootstrap_hyperparams_visualizer.py
+-rwxr-xr-x   0        0        0    19811 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/experiments_strategies.py
+-rwxr-xr-x   0        0        0   119690 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/experiments_strategies_hyperparamtuning.py
+-rwxr-xr-x   0        0        0     7475 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/generate_cachefile.py
+-rw-r--r--   0        0        0    20608 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/max_draw_k_from_n.py
+-rw-r--r--   0        0        0     3259 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/speedtest_index_performance.py
+-rw-r--r--   0        0        0     1174 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/speedtest_python_reversed_nan_sort.py
+-rwxr-xr-x   0        0        0     2545 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/try_BOtorch.py
+-rwxr-xr-x   0        0        0     8426 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/try_GPytorch.py
+-rw-r--r--   0        0        0    20822 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/extra/try_isotonic_regression.py
+-rwxr-xr-x   0        0        0      435 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/mypy.ini
+-rw-r--r--   0        0        0     1089 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/noxfile.py
+-rwxr-xr-x   0        0        0       17 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/profilings/.gitignore
+-rw-r--r--   0        0        0     2816 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0       95 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/__init__.py
+-rw-r--r--   0        0        0    17647 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/baseline.py
+-rwxr-xr-x   0        0        0     8418 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/caching.py
+-rw-r--r--   0        0        0    51986 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/curves.py
+-rwxr-xr-x   0        0        0     9764 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/experiments.py
+-rwxr-xr-x   0        0        0    24377 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/runner.py
+-rwxr-xr-x   0        0        0     4138 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/schema.json
+-rw-r--r--   0        0        0    25701 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/searchspace_statistics.py
+-rw-r--r--   0        0        0     1787 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/validators.py
+-rwxr-xr-x   0        0        0    48490 2024-05-17 06:54:13.660654 autotuning_methodology-1.0.0b3/src/autotuning_methodology/visualize_experiments.py
+-rw-r--r--   0        0        0  3269061 2024-05-17 06:54:13.668654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json
+-rw-r--r--   0        0        0  3255846 2024-05-17 06:54:13.676654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json
+-rw-r--r--   0        0        0  3483805 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json
+-rw-r--r--   0        0        0     2967 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py
+-rw-r--r--   0        0        0     1489 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/test.json
+-rw-r--r--   0        0        0     1476 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json
+-rw-r--r--   0        0        0     1465 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/test_cached.json
+-rw-r--r--   0        0        0     1453 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json
+-rw-r--r--   0        0        0     8913 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/test_run_experiment.py
+-rw-r--r--   0        0        0     2934 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/test_visualization.py
+-rw-r--r--   0        0        0     1978 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/release/test_toml_file.py
+-rw-r--r--   0        0        0       34 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/unit/test_caching.py
+-rw-r--r--   0        0        0     3464 2024-05-17 06:54:13.688654 autotuning_methodology-1.0.0b3/tests/autotuning_methodology/unit/test_curves.py
+-rw-r--r--   0        0        0     9820 1970-01-01 00:00:00.000000 autotuning_methodology-1.0.0b3/PKG-INFO
```

### Comparing `autotuning_methodology-1.0.0b2/.github/workflows/build-test-python-package.yml` & `autotuning_methodology-1.0.0b3/.github/workflows/build-test-python-package.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/.github/workflows/publish-documentation.yml` & `autotuning_methodology-1.0.0b3/.github/workflows/publish-documentation.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/.github/workflows/publish-package.yml` & `autotuning_methodology-1.0.0b3/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/.gitignore` & `autotuning_methodology-1.0.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/.vscode/settings.json` & `autotuning_methodology-1.0.0b3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/LICENSE` & `autotuning_methodology-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/README.md` & `autotuning_methodology-1.0.0b3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 [![PyPI Downloads](https://img.shields.io/pypi/dm/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 ![PyPI - Status](https://img.shields.io/pypi/status/autotuning_methodology)
 
  
 This repository contains the software package accompanying the paper "A Methodology for Comparing Auto-Tuning Optimization Algorithms". 
 It makes the guidelines in the methodology easy to apply: simply specify the  `.json` file, run `autotuning_visualize [path_to_json]` and wait for the results!
 
+### Limitations & Future Work
+Currently, the stable releases of this software package are compatible with [Kernel Tuner](https://github.com/KernelTuner/kernel_tuner) and [KTT](https://github.com/HiPerCoRe/KTT), as in the paper. We plan to soon extend this to support more frameworks. 
+
 ## Installation
 The package can be installed with `pip install autotuning_methodology`. 
 Alternatively, it can be installed by cloning this repository and running `pip install .` in the root of the cloned project. 
 Python >= 3.9 is supported. 
 
 ## Notable features
 - Official software by the authors of the methodology-defining paper.
```

### Comparing `autotuning_methodology-1.0.0b2/UML/.$Sequence Diagram.drawio.bkp` & `autotuning_methodology-1.0.0b3/UML/.$Sequence Diagram.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/.$flowchart.drawio.bkp` & `autotuning_methodology-1.0.0b3/UML/.$flowchart.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/Sequence Diagram.drawio` & `autotuning_methodology-1.0.0b3/UML/Sequence Diagram.drawio`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/classes.pdf` & `autotuning_methodology-1.0.0b3/UML/classes.pdf`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/flowchart/.$flowchart.drawio.bkp` & `autotuning_methodology-1.0.0b3/UML/flowchart/.$flowchart.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/flowchart/flowchart.drawio` & `autotuning_methodology-1.0.0b3/UML/flowchart/flowchart.drawio`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/flowchart/flowchart_output_generation.png` & `autotuning_methodology-1.0.0b3/UML/flowchart/flowchart_output_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/flowchart/flowchart_performance_curve_generation.png` & `autotuning_methodology-1.0.0b3/UML/flowchart/flowchart_performance_curve_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plot_aggregated.png` & `autotuning_methodology-1.0.0b3/UML/flowchart/mini_plots/flowchart_plot_aggregated.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plot_individual.png` & `autotuning_methodology-1.0.0b3/UML/flowchart/mini_plots/flowchart_plot_individual.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plots.py` & `autotuning_methodology-1.0.0b3/UML/flowchart/mini_plots/flowchart_plots.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/UML/packages.pdf` & `autotuning_methodology-1.0.0b3/UML/packages.pdf`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py` & `autotuning_methodology-1.0.0b3/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/Makefile` & `autotuning_methodology-1.0.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/autotuning_methodology.rst` & `autotuning_methodology-1.0.0b3/docs/autotuning_methodology.rst`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/conf.py` & `autotuning_methodology-1.0.0b3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/contributing.rst` & `autotuning_methodology-1.0.0b3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/getting_started.rst` & `autotuning_methodology-1.0.0b3/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/index.rst` & `autotuning_methodology-1.0.0b3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/make.bat` & `autotuning_methodology-1.0.0b3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/source/example_aggregated.png` & `autotuning_methodology-1.0.0b3/docs/source/example_aggregated.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/source/flowchart_output_generation.png` & `autotuning_methodology-1.0.0b3/docs/source/flowchart_output_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/source/flowchart_performance_curve_generation.png` & `autotuning_methodology-1.0.0b3/docs/source/flowchart_performance_curve_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/source/logo_autotuning_methodology.svg` & `autotuning_methodology-1.0.0b3/docs/source/logo_autotuning_methodology.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/source/logo_kernel_dashboard.svg` & `autotuning_methodology-1.0.0b3/docs/source/logo_kernel_dashboard.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/source/logo_kernel_launcher.svg` & `autotuning_methodology-1.0.0b3/docs/source/logo_kernel_launcher.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/docs/source/logo_kernel_tuner.svg` & `autotuning_methodology-1.0.0b3/docs/source/logo_kernel_tuner.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/experiment_files/bootstrap_hyperparams.json` & `autotuning_methodology-1.0.0b3/experiment_files/bootstrap_hyperparams.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/experiment_files/example_visualizations.json` & `autotuning_methodology-1.0.0b3/experiment_files/example_visualizations.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/experiment_files/methodology_paper_evaluation.json` & `autotuning_methodology-1.0.0b3/experiment_files/methodology_paper_evaluation.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/experiment_files/milo_hotspot.json` & `autotuning_methodology-1.0.0b3/experiment_files/milo_hotspot.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/experiment_files/presentation_comparison.json` & `autotuning_methodology-1.0.0b3/experiment_files/presentation_comparison.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/experiment_files/simple_example.json` & `autotuning_methodology-1.0.0b3/experiment_files/simple_example.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/experiment_files/test_random_calculated.json` & `autotuning_methodology-1.0.0b3/experiment_files/test_random_calculated.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/experiment_files/test_scatter.json` & `autotuning_methodology-1.0.0b3/experiment_files/test_scatter.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/experiment_files/test_searchspace_algorithms.json` & `autotuning_methodology-1.0.0b3/experiment_files/test_searchspace_algorithms.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/bootstrap_hyperparams_visualizer.py` & `autotuning_methodology-1.0.0b3/extra/bootstrap_hyperparams_visualizer.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/experiments_strategies.py` & `autotuning_methodology-1.0.0b3/extra/experiments_strategies.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/experiments_strategies_hyperparamtuning.py` & `autotuning_methodology-1.0.0b3/extra/experiments_strategies_hyperparamtuning.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/generate_cachefile.py` & `autotuning_methodology-1.0.0b3/extra/generate_cachefile.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/max_draw_k_from_n.py` & `autotuning_methodology-1.0.0b3/extra/max_draw_k_from_n.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/speedtest_index_performance.py` & `autotuning_methodology-1.0.0b3/extra/speedtest_index_performance.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/speedtest_python_reversed_nan_sort.py` & `autotuning_methodology-1.0.0b3/extra/speedtest_python_reversed_nan_sort.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/try_BOtorch.py` & `autotuning_methodology-1.0.0b3/extra/try_BOtorch.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/try_GPytorch.py` & `autotuning_methodology-1.0.0b3/extra/try_GPytorch.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/extra/try_isotonic_regression.py` & `autotuning_methodology-1.0.0b3/extra/try_isotonic_regression.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/noxfile.py` & `autotuning_methodology-1.0.0b3/noxfile.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/pyproject.toml` & `autotuning_methodology-1.0.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project] # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
 name = "autotuning_methodology"
-version = "1.0.0b2"
+version = "1.0.0b3"
 authors = [{ name = "Floris-Jan Willemsen", email = "fjwillemsen97@gmail.com" }]
 description = "Software package easing implementation of the guidelines of the 2024 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'."
 keywords = ["autotuning", "auto-tuning", "methodology", "scientific"]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `autotuning_methodology-1.0.0b2/src/autotuning_methodology/baseline.py` & `autotuning_methodology-1.0.0b3/src/autotuning_methodology/baseline.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/src/autotuning_methodology/caching.py` & `autotuning_methodology-1.0.0b3/src/autotuning_methodology/caching.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/src/autotuning_methodology/curves.py` & `autotuning_methodology-1.0.0b3/src/autotuning_methodology/curves.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/src/autotuning_methodology/experiments.py` & `autotuning_methodology-1.0.0b3/src/autotuning_methodology/experiments.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/src/autotuning_methodology/runner.py` & `autotuning_methodology-1.0.0b3/src/autotuning_methodology/runner.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/src/autotuning_methodology/schema.json` & `autotuning_methodology-1.0.0b3/src/autotuning_methodology/schema.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/src/autotuning_methodology/searchspace_statistics.py` & `autotuning_methodology-1.0.0b3/src/autotuning_methodology/searchspace_statistics.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/src/autotuning_methodology/validators.py` & `autotuning_methodology-1.0.0b3/src/autotuning_methodology/validators.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/src/autotuning_methodology/visualize_experiments.py` & `autotuning_methodology-1.0.0b3/src/autotuning_methodology/visualize_experiments.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test.json` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/test.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_cached.json` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/test_cached.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/test_run_experiment.py` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/test_run_experiment.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/test_visualization.py` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/integration/test_visualization.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/release/test_toml_file.py` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/release/test_toml_file.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/unit/test_curves.py` & `autotuning_methodology-1.0.0b3/tests/autotuning_methodology/unit/test_curves.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b2/PKG-INFO` & `autotuning_methodology-1.0.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotuning_methodology
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Software package easing implementation of the guidelines of the 2024 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'.
 Keywords: autotuning,auto-tuning,methodology,scientific
 Author-email: Floris-Jan Willemsen <fjwillemsen97@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -54,14 +54,17 @@
 [![PyPI Downloads](https://img.shields.io/pypi/dm/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 ![PyPI - Status](https://img.shields.io/pypi/status/autotuning_methodology)
 
  
 This repository contains the software package accompanying the paper "A Methodology for Comparing Auto-Tuning Optimization Algorithms". 
 It makes the guidelines in the methodology easy to apply: simply specify the  `.json` file, run `autotuning_visualize [path_to_json]` and wait for the results!
 
+### Limitations & Future Work
+Currently, the stable releases of this software package are compatible with [Kernel Tuner](https://github.com/KernelTuner/kernel_tuner) and [KTT](https://github.com/HiPerCoRe/KTT), as in the paper. We plan to soon extend this to support more frameworks. 
+
 ## Installation
 The package can be installed with `pip install autotuning_methodology`. 
 Alternatively, it can be installed by cloning this repository and running `pip install .` in the root of the cloned project. 
 Python >= 3.9 is supported. 
 
 ## Notable features
 - Official software by the authors of the methodology-defining paper.
```

