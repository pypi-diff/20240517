# Comparing `tmp/catasta-0.2.1.tar.gz` & `tmp/catasta-0.2.2.tar.gz`

## Comparing `catasta-0.2.1.tar` & `catasta-0.2.2.tar`

### file list

```diff
@@ -1,1186 +1,1186 @@
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 catasta-0.2.1/requirements.txt
--rw-r--r--   0        0        0    14890 2020-02-02 00:00:00.000000 catasta-0.2.1/assets/catasta.svg
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/archways/__init__.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/archways/archway.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/dataclasses/__init__.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/dataclasses/eval_info.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/dataclasses/prediction_info.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/dataclasses/train_info.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/datasets/__init__.py
--rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/datasets/catasta_dataset.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/__init__.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/classifiers/cnn_classifier.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/classifiers/feedforward_classifier.py
--rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/classifiers/mamba_classifier.py
--rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/classifiers/mamba_fft_classifier.py
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/classifiers/transformer_classifier.py
--rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/classifiers/transformer_fft_classifier.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/regressors/approximate_gp_regressor.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/regressors/feedforward_regressor.py
--rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/regressors/mamba_fft_regressor.py
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/regressors/mamba_regressor.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/regressors/transformer_fft_regressor.py
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/models/regressors/transformer_regressor.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/scaffolds/__init__.py
--rw-r--r--   0        0        0    13035 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/scaffolds/scaffold.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/scaffolds/utils/__init__.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/scaffolds/utils/likelihood_factory.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/scaffolds/utils/loss_function_factory.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/scaffolds/utils/model_state_manager.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/scaffolds/utils/objective_function_factory.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/scaffolds/utils/optimizer_factory.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/scaffolds/utils/training_logger.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/custom.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/decimation.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/diff_and_concat.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/fir_filtering.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/identity.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/kalman_filter.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/normalization.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/slicing.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/transformation.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 catasta-0.2.1/catasta/transformations/window_sliding.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/cnn.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/feedforward.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/mamba.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/mamba_fft.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/transformer.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/transformer_fft.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/10563.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/10747.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/11340.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/11742.png
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/12686.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/12992.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/1346.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/14693.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/14752.png
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/15130.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/15344.png
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/15520.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/15580.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/15971.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/16217.png
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/16396.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/1664.png
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/16679.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/18219.png
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/19009.png
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/19361.png
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/20814.png
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/22596.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/22761.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/22929.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/23120.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/23875.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/25987.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/26389.png
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/26818.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/27283.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/28945.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/2955.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/30034.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/30849.png
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/32531.png
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/33023.png
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/3337.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/34523.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/35655.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/35739.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/36562.png
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/36937.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/36975.png
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/37841.png
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/38055.png
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/3829.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/40042.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/40454.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/40471.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/40844.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/40915.png
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/41374.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/41570.png
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/42038.png
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/42614.png
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/42632.png
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/43443.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/43610.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/43827.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/45676.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/45833.png
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/45905.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/4642.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/47150.png
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/47241.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/47473.png
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/48695.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/49737.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/50042.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/50101.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/5052.png
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/50617.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/51006.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/51638.png
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/51669.png
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/5317.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/5353.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/53657.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/53678.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/54141.png
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/54608.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/54764.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/56005.png
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/56715.png
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/56735.png
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/59103.png
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/59639.png
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/59911.png
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/6008.png
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/6967.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/7271.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/7471.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/7506.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/8193.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/8249.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/8323.png
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/8901.png
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/9142.png
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/0/9485.png
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/1060.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/11079.png
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/11445.png
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/1230.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/14561.png
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/16643.png
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/1665.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/16718.png
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/17560.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/17669.png
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/1786.png
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/18444.png
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/18452.png
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/18880.png
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/19158.png
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/19937.png
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/22464.png
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/23097.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/23530.png
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/23973.png
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/24738.png
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/25397.png
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/25474.png
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/25600.png
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/25697.png
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/25751.png
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/25847.png
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/25885.png
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/26401.png
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/27885.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/28322.png
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/28420.png
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/29323.png
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/29902.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/30457.png
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/30809.png
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/31377.png
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/3155.png
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/31771.png
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/31966.png
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/3272.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/32814.png
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/33750.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/35710.png
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/36814.png
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/37978.png
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/38095.png
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/39033.png
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/39652.png
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/39707.png
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/39717.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/39888.png
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/40007.png
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/4029.png
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/40516.png
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/40884.png
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/40973.png
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/41011.png
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/41526.png
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/41884.png
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/43444.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/43897.png
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/44269.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/4445.png
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/45366.png
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/45683.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/46268.png
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/46539.png
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/4696.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/47019.png
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/47773.png
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/47982.png
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/48189.png
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/48629.png
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/49706.png
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/5006.png
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/50264.png
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/52073.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/52454.png
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/52965.png
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/53599.png
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/53904.png
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/55505.png
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/55961.png
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/57816.png
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/58072.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/58307.png
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/58387.png
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/58820.png
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/58830.png
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/6328.png
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/7536.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/7603.png
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/8092.png
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/8319.png
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/8633.png
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/8704.png
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/8895.png
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/9507.png
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/1/9628.png
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/10009.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/1011.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/10476.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/11193.png
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/11242.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/11531.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/11718.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/1188.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/13086.png
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/14569.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/15614.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/16812.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/17353.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/18097.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/19468.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/19764.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/20831.png
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/21053.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/21274.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/21527.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/21691.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/22036.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/2280.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/22900.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/23028.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/23894.png
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/24462.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/24881.png
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/25718.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/26221.png
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/26883.png
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/26932.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/27426.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/28059.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/28266.png
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/29904.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/30064.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/3042.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/3179.png
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/32035.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/32135.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/32155.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/32216.png
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/32780.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/33743.png
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/34167.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/35393.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/35947.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/36112.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/36718.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/36721.png
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/36805.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/36875.png
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/36958.png
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/37825.png
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/37974.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/4086.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/42065.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/43794.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/43871.png
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/44412.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/45464.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/45745.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/46116.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/46129.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/46835.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/46997.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/47101.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/47235.png
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/47273.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/48107.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/48248.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/48460.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/48934.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/49160.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/50446.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/50875.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/51738.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/52812.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/53239.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/54220.png
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/54519.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/54840.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/55526.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/55857.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/56427.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/5758.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/57966.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/58137.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/58317.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/58783.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/59222.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/59390.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/6143.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/7392.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/7870.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/8251.png
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/8277.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/8640.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/2/9736.png
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/1097.png
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/11565.png
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/12392.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/12780.png
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/12990.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/13099.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/13294.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/1357.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/14447.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/15181.png
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/1529.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/15474.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/16296.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/17471.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/18587.png
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/1994.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/21647.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/21998.png
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/22000.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/22185.png
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/22674.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/22883.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/23239.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/23695.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/25867.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/2587.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/27248.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/28773.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/28858.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/29270.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/31201.png
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/33189.png
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/33432.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/33875.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/34525.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/34642.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/35349.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/35613.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/35898.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/36298.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/36327.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/37361.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/37374.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/37454.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/37649.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/38281.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/38361.png
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/38687.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/38927.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/39099.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/39566.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/39686.png
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/39798.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/40079.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/41110.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/41929.png
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/42445.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/4295.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/43435.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/43537.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/44557.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/44681.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/45509.png
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/45786.png
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/46145.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/46480.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/47367.png
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/48551.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/50658.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/5092.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/51333.png
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/52022.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/52164.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/53167.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/5323.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/53447.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/5370.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/53758.png
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/53815.png
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/53995.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/54020.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/54534.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/54616.png
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/54635.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/54780.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/55474.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/55509.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/56164.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/57391.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/57864.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/57879.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/58513.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/58832.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/58937.png
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/59394.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/629.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/6939.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/7433.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/8055.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/3/8597.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/10262.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/10683.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/11646.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/12064.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/12102.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/12458.png
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/12615.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/12731.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/13418.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/14496.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/14654.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/15207.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/15274.png
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/15373.png
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/15916.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/16450.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/16942.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/17774.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/17931.png
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/17949.png
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/19161.png
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/2176.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/22273.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/22311.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/22553.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/24298.png
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/25056.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/25616.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/2578.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/27097.png
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/27227.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/27476.png
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/28588.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/30815.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/31006.png
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/31412.png
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/32647.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/32997.png
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/34130.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/34290.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/3459.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/34611.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/3496.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/35626.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/36246.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/36359.png
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/36977.png
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/37074.png
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/37505.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/3761.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/3817.png
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/38500.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/38671.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/39635.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/4038.png
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/40903.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/41096.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/41145.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/41568.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/42181.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/42329.png
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/42455.png
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/4264.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/42711.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/43112.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/43636.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/4417.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/44419.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/46057.png
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/46097.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/46939.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/47282.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/48215.png
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/48389.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/48582.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/48972.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/50704.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/51028.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/51396.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/52193.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/54116.png
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/54171.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/54861.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/55323.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/57155.png
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/58047.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/58184.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/58579.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/58630.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/58843.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/6095.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/6189.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/6536.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/682.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/7120.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/7186.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/8278.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/8346.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/8495.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/4/8737.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/10092.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/10277.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/10441.png
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/10661.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/11631.png
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/13843.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/14096.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/14100.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/14623.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/14707.png
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/1490.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/14907.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/16845.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/17138.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/17468.png
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/18083.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/18298.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/19944.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/23200.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/23920.png
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/24043.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/24716.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/26198.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/26204.png
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/2713.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/27375.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/27921.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/27997.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/29157.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/29273.png
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/29539.png
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/29659.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/30396.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/30676.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/31584.png
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/31821.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/33138.png
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/33420.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/33502.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/33511.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/33734.png
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/33773.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/3401.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/34505.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/35268.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/35858.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/3635.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/36516.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/36588.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/36661.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/37448.png
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/3801.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/38934.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/39923.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/40088.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/40154.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/40350.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/40623.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/40748.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/41945.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/42047.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/42317.png
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/42359.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/4247.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/43098.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/43799.png
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/44753.png
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/44802.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/44924.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/45753.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/45872.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/46759.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/47177.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/47866.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/48251.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/48572.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/48769.png
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/50399.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/52491.png
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/5255.png
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/52826.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/54184.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/554.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/55455.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/55794.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/56013.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/56200.png
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/56499.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/5668.png
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/57248.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/57510.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/58359.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/59089.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/59492.png
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/59525.png
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/6077.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/8252.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/8479.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/8676.png
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/5/9464.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/10275.png
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/10540.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/12047.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/12547.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/12866.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/1303.png
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/13167.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/14328.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/14344.png
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/14604.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/15159.png
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/16452.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/1688.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/17008.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/18652.png
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/18732.png
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/19488.png
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/19896.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/20603.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/21331.png
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/22693.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/24585.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/24944.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/24945.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/25113.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/25241.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/25680.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/26160.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/26347.png
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/26384.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/26418.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/27682.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/27724.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/27890.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/28594.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/28890.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/29221.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/29350.png
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/30083.png
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/31000.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/31105.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/32752.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/33073.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/33484.png
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/33910.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/34260.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/35297.png
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/35411.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/35917.png
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/35962.png
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/36590.png
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/36841.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/36866.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/36966.png
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/38322.png
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/38342.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/38571.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/39337.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/39515.png
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/40862.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/40980.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/41308.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/41561.png
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/41572.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/42143.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/42700.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/42767.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/43164.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/43440.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/43625.png
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/44011.png
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/44204.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/44250.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/46511.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/4841.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/48433.png
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/48867.png
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/5084.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/51159.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/52781.png
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/54618.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/5634.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/5671.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/57347.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/57490.png
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/5782.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/57959.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/57971.png
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/58549.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/59132.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/59359.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/649.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/6509.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/6581.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/6907.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/7543.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/7711.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/8376.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/9662.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/6/9692.png
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/1022.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/10759.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/10932.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/11119.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/1153.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/12287.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/12769.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/13665.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/13810.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/14219.png
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/14522.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/148.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/15721.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/15811.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/1589.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/15909.png
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/15922.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/17800.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/19424.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/19893.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/19949.png
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/20019.png
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/20398.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/20588.png
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/21318.png
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/22181.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/23815.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/25011.png
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/25062.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/25817.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/26189.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/26886.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/28417.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/28781.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/29159.png
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/2986.png
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/29998.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/31073.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/31189.png
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/31408.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/32159.png
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/32604.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/33062.png
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/34934.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/34982.png
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/36902.png
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/36916.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/377.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/37971.png
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/38096.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/38243.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/39969.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/40001.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/40357.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/40643.png
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/42780.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/43533.png
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/43890.png
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/4479.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/44803.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/45143.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/45777.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/46429.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/46671.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/47495.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/47537.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/4784.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/48473.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/49125.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/49257.png
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/50038.png
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/50143.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/50375.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/50655.png
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/51070.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/51084.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/51113.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/51203.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/52149.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/52235.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/53478.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/53483.png
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/53719.png
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/54477.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/55082.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/55608.png
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/56052.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/56521.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/57204.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/58480.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/58715.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/5976.png
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/59856.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/59938.png
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/6688.png
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/7092.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/7287.png
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/7547.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/8286.png
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/7/9267.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/10126.png
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/11450.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/12054.png
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/14893.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/15221.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/15333.png
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/15775.png
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/16669.png
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/17362.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/17999.png
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/1856.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/18623.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/1873.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/19392.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/19756.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/20771.png
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/21161.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/21211.png
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/21406.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/22532.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/22773.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/23243.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/23466.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/24027.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/25301.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/25583.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/25686.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/25715.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/25843.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/26664.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/2687.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/27126.png
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/27294.png
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/28188.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/29381.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/30038.png
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/30914.png
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/30967.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/31039.png
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/31781.png
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/31845.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/32615.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/32717.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/32742.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/33424.png
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/33631.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/34375.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/34842.png
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/35018.png
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/35193.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/35619.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/35987.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/3643.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/36585.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/36727.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/36834.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/37202.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/37263.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/37281.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/37933.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/3825.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/39731.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/4063.png
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/40726.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/42417.png
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/43051.png
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/44061.png
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/44171.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/44861.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/45481.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/46739.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/47730.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/48104.png
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/49201.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/49532.png
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/50180.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/50394.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/5042.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/50873.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/53640.png
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/53648.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/54469.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/54645.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/55264.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/56594.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/57118.png
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/57355.png
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/57513.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/57655.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/58020.png
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/58736.png
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/58827.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/59128.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/59949.png
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/6506.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/7121.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/7681.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/8175.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/9554.png
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/8/9861.png
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/1005.png
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/11208.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/116.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/11847.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/12076.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/12237.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/12562.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/13130.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/15018.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/15131.png
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/15195.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/15827.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/15899.png
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/15987.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/16270.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/16635.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/17447.png
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/19494.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/19766.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/20513.png
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/20641.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/20918.png
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/20943.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/22406.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/23224.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/23853.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/24736.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/25969.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/26361.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/2640.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/26631.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/26806.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/28553.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/3055.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/30646.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/30696.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/30776.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/31320.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/322.png
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/32403.png
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/32668.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/3296.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/33174.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/33999.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/34019.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/34044.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/34224.png
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/34865.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/3506.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/35741.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/36225.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/36306.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/36666.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/37781.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/37934.png
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/38118.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/39822.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/40487.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/41563.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/42668.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/42870.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/43001.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/44016.png
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/44028.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/45144.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/45176.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/45415.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/46578.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/46659.png
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/4678.png
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/4754.png
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/48758.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/48888.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/49130.png
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/4929.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/51938.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/53070.png
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/53682.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/53841.png
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/54538.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/54687.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/55063.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/5532.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/56166.png
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/56205.png
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/5658.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/57531.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/58596.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/58967.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/59314.png
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/6376.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/6542.png
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/6934.png
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/7006.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/7538.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/7873.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/8066.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/8216.png
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/8318.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/train/9/9238.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/10.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/1570.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/2531.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/2568.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/525.png
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/5321.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/546.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/7449.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/7703.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/0/9687.png
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/135.png
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/3026.png
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/5318.png
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/5666.png
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/672.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/6789.png
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/7226.png
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/7405.png
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/8636.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/1/9955.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/1065.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/2260.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/237.png
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/3260.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/404.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/5692.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/6084.png
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/6466.png
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/6949.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/2/7683.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/2347.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/245.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/2551.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/2989.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/3129.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/5904.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/6542.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/7656.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/9872.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/3/9882.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/2053.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/2306.png
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/3233.png
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/3282.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/3341.png
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/3544.png
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/3653.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/3841.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/5032.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/4/6369.png
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/2279.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/2515.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/4763.png
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/5518.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/6148.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/6155.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/7067.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/8531.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/8878.png
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/5/9749.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/1886.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/2210.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/3362.png
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/4686.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/5332.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/6630.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/7438.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/7596.png
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/8831.png
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/6/9247.png
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/1012.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/2595.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/3572.png
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/4966.png
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/5190.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/6986.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/8052.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/8248.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/9015.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/7/9837.png
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/2834.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/4797.png
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/5433.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/6485.png
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/693.png
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/8217.png
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/8241.png
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/8866.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/9496.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/8/9926.png
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/4272.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/4410.png
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/5787.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/6496.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/6807.png
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/7813.png
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/8184.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/8298.png
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/9057.png
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/classification/data/reduced_mnist/val/9/9676.png
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/agp.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/feedforward.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/mamba.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/mamba_fft.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/transformer.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/transformer_fft.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/incomplete/create_dataset.py
--rw-r--r--   0        0        0    77880 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/incomplete/data.csv
--rw-r--r--   0        0        0    62316 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/incomplete/train/data.csv
--rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/incomplete/val/data.csv
--rw-r--r--   0        0        0   381773 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/nylon_wire/train/mixed_10_20.csv
--rw-r--r--   0        0        0   357293 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/nylon_wire/train/mixed_15_25.csv
--rw-r--r--   0        0        0   357972 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/nylon_wire/train/mixed_20_30.csv
--rw-r--r--   0        0        0   357304 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/nylon_wire/train/sin_20.csv
--rw-r--r--   0        0        0   438969 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/nylon_wire/train/sin_30.csv
--rw-r--r--   0        0        0   354814 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/nylon_wire/train/sin_40.csv
--rw-r--r--   0        0        0   381390 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/nylon_wire/train/tri_20.csv
--rw-r--r--   0        0        0   590643 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/nylon_wire/train/tri_30.csv
--rw-r--r--   0        0        0   485182 2020-02-02 00:00:00.000000 catasta-0.2.1/examples/regression/data/nylon_wire/val/tri_40.csv
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_classification_dataset.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_decimation.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_deepar_predictor.py
--rw-r--r--   0        0        0    13249 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_gpformer_regressor.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_kalman_filter.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_load_class_model.py
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_load_model.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_regression_dataset.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_save_class_model.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_save_model.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_transformer_signal_classifier.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 catasta-0.2.1/tests/test_window_sliding.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 catasta-0.2.1/.gitignore
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 catasta-0.2.1/LICENSE
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 catasta-0.2.1/README.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 catasta-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 catasta-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 catasta-0.2.2/requirements.txt
+-rw-r--r--   0        0        0    14890 2020-02-02 00:00:00.000000 catasta-0.2.2/assets/catasta.svg
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/archways/__init__.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/archways/archway.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/dataclasses/__init__.py
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/dataclasses/eval_info.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/dataclasses/prediction_info.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/dataclasses/train_info.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/datasets/__init__.py
+-rw-r--r--   0        0        0    11247 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/datasets/catasta_dataset.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/classifiers/cnn_classifier.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/classifiers/feedforward_classifier.py
+-rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/classifiers/mamba_classifier.py
+-rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/classifiers/mamba_fft_classifier.py
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/classifiers/transformer_classifier.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/classifiers/transformer_fft_classifier.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/regressors/approximate_gp_regressor.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/regressors/feedforward_regressor.py
+-rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/regressors/mamba_fft_regressor.py
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/regressors/mamba_regressor.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/regressors/transformer_fft_regressor.py
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/models/regressors/transformer_regressor.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/scaffolds/__init__.py
+-rw-r--r--   0        0        0    13619 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/scaffolds/scaffold.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/scaffolds/utils/__init__.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/scaffolds/utils/likelihood_factory.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/scaffolds/utils/loss_function_factory.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/scaffolds/utils/model_state_manager.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/scaffolds/utils/objective_function_factory.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/scaffolds/utils/optimizer_factory.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/scaffolds/utils/training_logger.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/custom.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/decimation.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/diff_and_concat.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/fir_filtering.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/identity.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/kalman_filter.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/normalization.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/slicing.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/transformation.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 catasta-0.2.2/catasta/transformations/window_sliding.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/cnn.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/feedforward.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/mamba.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/mamba_fft.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/transformer.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/transformer_fft.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/10563.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/10747.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/11340.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/11742.png
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/12686.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/12992.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/1346.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/14693.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/14752.png
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/15130.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/15344.png
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/15520.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/15580.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/15971.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/16217.png
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/16396.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/1664.png
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/16679.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/18219.png
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/19009.png
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/19361.png
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/20814.png
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/22596.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/22761.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/22929.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/23120.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/23875.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/25987.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/26389.png
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/26818.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/27283.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/28945.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/2955.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/30034.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/30849.png
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/32531.png
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/33023.png
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/3337.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/34523.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/35655.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/35739.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/36562.png
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/36937.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/36975.png
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/37841.png
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/38055.png
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/3829.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/40042.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/40454.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/40471.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/40844.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/40915.png
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/41374.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/41570.png
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/42038.png
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/42614.png
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/42632.png
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/43443.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/43610.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/43827.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/45676.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/45833.png
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/45905.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/4642.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/47150.png
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/47241.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/47473.png
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/48695.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/49737.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/50042.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/50101.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/5052.png
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/50617.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/51006.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/51638.png
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/51669.png
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/5317.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/5353.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/53657.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/53678.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/54141.png
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/54608.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/54764.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/56005.png
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/56715.png
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/56735.png
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/59103.png
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/59639.png
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/59911.png
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/6008.png
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/6967.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/7271.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/7471.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/7506.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/8193.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/8249.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/8323.png
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/8901.png
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/9142.png
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/0/9485.png
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/1060.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/11079.png
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/11445.png
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/1230.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/14561.png
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/16643.png
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/1665.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/16718.png
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/17560.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/17669.png
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/1786.png
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/18444.png
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/18452.png
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/18880.png
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/19158.png
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/19937.png
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/22464.png
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/23097.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/23530.png
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/23973.png
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/24738.png
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/25397.png
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/25474.png
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/25600.png
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/25697.png
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/25751.png
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/25847.png
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/25885.png
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/26401.png
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/27885.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/28322.png
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/28420.png
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/29323.png
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/29902.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/30457.png
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/30809.png
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/31377.png
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/3155.png
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/31771.png
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/31966.png
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/3272.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/32814.png
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/33750.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/35710.png
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/36814.png
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/37978.png
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/38095.png
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/39033.png
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/39652.png
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/39707.png
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/39717.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/39888.png
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/40007.png
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/4029.png
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/40516.png
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/40884.png
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/40973.png
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/41011.png
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/41526.png
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/41884.png
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/43444.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/43897.png
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/44269.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/4445.png
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/45366.png
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/45683.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/46268.png
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/46539.png
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/4696.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/47019.png
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/47773.png
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/47982.png
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/48189.png
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/48629.png
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/49706.png
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/5006.png
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/50264.png
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/52073.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/52454.png
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/52965.png
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/53599.png
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/53904.png
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/55505.png
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/55961.png
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/57816.png
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/58072.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/58307.png
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/58387.png
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/58820.png
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/58830.png
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/6328.png
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/7536.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/7603.png
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/8092.png
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/8319.png
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/8633.png
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/8704.png
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/8895.png
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/9507.png
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/1/9628.png
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/10009.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/1011.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/10476.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/11193.png
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/11242.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/11531.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/11718.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/1188.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/13086.png
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/14569.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/15614.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/16812.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/17353.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/18097.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/19468.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/19764.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/20831.png
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/21053.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/21274.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/21527.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/21691.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/22036.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/2280.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/22900.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/23028.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/23894.png
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/24462.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/24881.png
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/25718.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/26221.png
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/26883.png
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/26932.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/27426.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/28059.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/28266.png
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/29904.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/30064.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/3042.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/3179.png
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/32035.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/32135.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/32155.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/32216.png
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/32780.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/33743.png
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/34167.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/35393.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/35947.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/36112.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/36718.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/36721.png
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/36805.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/36875.png
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/36958.png
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/37825.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/37974.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/4086.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/42065.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/43794.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/43871.png
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/44412.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/45464.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/45745.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/46116.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/46129.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/46835.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/46997.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/47101.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/47235.png
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/47273.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/48107.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/48248.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/48460.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/48934.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/49160.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/50446.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/50875.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/51738.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/52812.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/53239.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/54220.png
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/54519.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/54840.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/55526.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/55857.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/56427.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/5758.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/57966.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/58137.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/58317.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/58783.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/59222.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/59390.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/6143.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/7392.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/7870.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/8251.png
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/8277.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/8640.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/2/9736.png
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/1097.png
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/11565.png
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/12392.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/12780.png
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/12990.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/13099.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/13294.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/1357.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/14447.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/15181.png
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/1529.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/15474.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/16296.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/17471.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/18587.png
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/1994.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/21647.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/21998.png
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/22000.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/22185.png
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/22674.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/22883.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/23239.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/23695.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/25867.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/2587.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/27248.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/28773.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/28858.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/29270.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/31201.png
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/33189.png
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/33432.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/33875.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/34525.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/34642.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/35349.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/35613.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/35898.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/36298.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/36327.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/37361.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/37374.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/37454.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/37649.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/38281.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/38361.png
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/38687.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/38927.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/39099.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/39566.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/39686.png
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/39798.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/40079.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/41110.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/41929.png
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/42445.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/4295.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/43435.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/43537.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/44557.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/44681.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/45509.png
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/45786.png
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/46145.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/46480.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/47367.png
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/48551.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/50658.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/5092.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/51333.png
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/52022.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/52164.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/53167.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/5323.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/53447.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/5370.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/53758.png
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/53815.png
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/53995.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/54020.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/54534.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/54616.png
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/54635.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/54780.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/55474.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/55509.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/56164.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/57391.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/57864.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/57879.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/58513.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/58832.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/58937.png
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/59394.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/629.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/6939.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/7433.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/8055.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/3/8597.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/10262.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/10683.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/11646.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/12064.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/12102.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/12458.png
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/12615.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/12731.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/13418.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/14496.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/14654.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/15207.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/15274.png
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/15373.png
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/15916.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/16450.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/16942.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/17774.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/17931.png
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/17949.png
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/19161.png
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/2176.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/22273.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/22311.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/22553.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/24298.png
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/25056.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/25616.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/2578.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/27097.png
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/27227.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/27476.png
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/28588.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/30815.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/31006.png
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/31412.png
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/32647.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/32997.png
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/34130.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/34290.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/3459.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/34611.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/3496.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/35626.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/36246.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/36359.png
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/36977.png
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/37074.png
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/37505.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/3761.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/3817.png
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/38500.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/38671.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/39635.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/4038.png
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/40903.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/41096.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/41145.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/41568.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/42181.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/42329.png
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/42455.png
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/4264.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/42711.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/43112.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/43636.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/4417.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/44419.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/46057.png
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/46097.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/46939.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/47282.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/48215.png
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/48389.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/48582.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/48972.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/50704.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/51028.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/51396.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/52193.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/54116.png
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/54171.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/54861.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/55323.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/57155.png
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/58047.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/58184.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/58579.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/58630.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/58843.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/6095.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/6189.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/6536.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/682.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/7120.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/7186.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/8278.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/8346.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/8495.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/4/8737.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/10092.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/10277.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/10441.png
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/10661.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/11631.png
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/13843.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/14096.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/14100.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/14623.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/14707.png
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/1490.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/14907.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/16845.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/17138.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/17468.png
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/18083.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/18298.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/19944.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/23200.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/23920.png
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/24043.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/24716.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/26198.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/26204.png
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/2713.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/27375.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/27921.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/27997.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/29157.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/29273.png
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/29539.png
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/29659.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/30396.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/30676.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/31584.png
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/31821.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/33138.png
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/33420.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/33502.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/33511.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/33734.png
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/33773.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/3401.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/34505.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/35268.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/35858.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/3635.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/36516.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/36588.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/36661.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/37448.png
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/3801.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/38934.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/39923.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/40088.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/40154.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/40350.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/40623.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/40748.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/41945.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/42047.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/42317.png
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/42359.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/4247.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/43098.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/43799.png
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/44753.png
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/44802.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/44924.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/45753.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/45872.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/46759.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/47177.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/47866.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/48251.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/48572.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/48769.png
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/50399.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/52491.png
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/5255.png
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/52826.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/54184.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/554.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/55455.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/55794.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/56013.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/56200.png
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/56499.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/5668.png
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/57248.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/57510.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/58359.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/59089.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/59492.png
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/59525.png
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/6077.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/8252.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/8479.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/8676.png
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/5/9464.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/10275.png
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/10540.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/12047.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/12547.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/12866.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/1303.png
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/13167.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/14328.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/14344.png
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/14604.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/15159.png
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/16452.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/1688.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/17008.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/18652.png
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/18732.png
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/19488.png
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/19896.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/20603.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/21331.png
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/22693.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/24585.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/24944.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/24945.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/25113.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/25241.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/25680.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/26160.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/26347.png
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/26384.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/26418.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/27682.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/27724.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/27890.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/28594.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/28890.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/29221.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/29350.png
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/30083.png
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/31000.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/31105.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/32752.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/33073.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/33484.png
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/33910.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/34260.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/35297.png
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/35411.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/35917.png
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/35962.png
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/36590.png
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/36841.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/36866.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/36966.png
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/38322.png
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/38342.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/38571.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/39337.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/39515.png
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/40862.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/40980.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/41308.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/41561.png
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/41572.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/42143.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/42700.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/42767.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/43164.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/43440.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/43625.png
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/44011.png
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/44204.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/44250.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/46511.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/4841.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/48433.png
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/48867.png
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/5084.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/51159.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/52781.png
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/54618.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/5634.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/5671.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/57347.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/57490.png
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/5782.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/57959.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/57971.png
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/58549.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/59132.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/59359.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/649.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/6509.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/6581.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/6907.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/7543.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/7711.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/8376.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/9662.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/6/9692.png
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/1022.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/10759.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/10932.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/11119.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/1153.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/12287.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/12769.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/13665.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/13810.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/14219.png
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/14522.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/148.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/15721.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/15811.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/1589.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/15909.png
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/15922.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/17800.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/19424.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/19893.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/19949.png
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/20019.png
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/20398.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/20588.png
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/21318.png
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/22181.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/23815.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/25011.png
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/25062.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/25817.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/26189.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/26886.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/28417.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/28781.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/29159.png
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/2986.png
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/29998.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/31073.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/31189.png
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/31408.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/32159.png
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/32604.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/33062.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/34934.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/34982.png
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/36902.png
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/36916.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/377.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/37971.png
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/38096.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/38243.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/39969.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/40001.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/40357.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/40643.png
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/42780.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/43533.png
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/43890.png
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/4479.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/44803.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/45143.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/45777.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/46429.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/46671.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/47495.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/47537.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/4784.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/48473.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/49125.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/49257.png
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/50038.png
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/50143.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/50375.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/50655.png
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/51070.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/51084.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/51113.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/51203.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/52149.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/52235.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/53478.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/53483.png
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/53719.png
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/54477.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/55082.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/55608.png
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/56052.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/56521.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/57204.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/58480.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/58715.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/5976.png
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/59856.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/59938.png
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/6688.png
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/7092.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/7287.png
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/7547.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/8286.png
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/7/9267.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/10126.png
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/11450.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/12054.png
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/14893.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/15221.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/15333.png
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/15775.png
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/16669.png
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/17362.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/17999.png
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/1856.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/18623.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/1873.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/19392.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/19756.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/20771.png
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/21161.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/21211.png
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/21406.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/22532.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/22773.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/23243.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/23466.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/24027.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/25301.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/25583.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/25686.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/25715.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/25843.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/26664.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/2687.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/27126.png
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/27294.png
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/28188.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/29381.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/30038.png
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/30914.png
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/30967.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/31039.png
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/31781.png
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/31845.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/32615.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/32717.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/32742.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/33424.png
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/33631.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/34375.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/34842.png
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/35018.png
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/35193.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/35619.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/35987.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/3643.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/36585.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/36727.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/36834.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/37202.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/37263.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/37281.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/37933.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/3825.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/39731.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/4063.png
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/40726.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/42417.png
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/43051.png
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/44061.png
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/44171.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/44861.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/45481.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/46739.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/47730.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/48104.png
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/49201.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/49532.png
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/50180.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/50394.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/5042.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/50873.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/53640.png
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/53648.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/54469.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/54645.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/55264.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/56594.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/57118.png
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/57355.png
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/57513.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/57655.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/58020.png
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/58736.png
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/58827.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/59128.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/59949.png
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/6506.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/7121.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/7681.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/8175.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/9554.png
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/8/9861.png
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/1005.png
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/11208.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/116.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/11847.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/12076.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/12237.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/12562.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/13130.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/15018.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/15131.png
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/15195.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/15827.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/15899.png
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/15987.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/16270.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/16635.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/17447.png
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/19494.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/19766.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/20513.png
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/20641.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/20918.png
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/20943.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/22406.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/23224.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/23853.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/24736.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/25969.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/26361.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/2640.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/26631.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/26806.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/28553.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/3055.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/30646.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/30696.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/30776.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/31320.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/322.png
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/32403.png
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/32668.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/3296.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/33174.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/33999.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/34019.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/34044.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/34224.png
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/34865.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/3506.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/35741.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/36225.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/36306.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/36666.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/37781.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/37934.png
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/38118.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/39822.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/40487.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/41563.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/42668.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/42870.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/43001.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/44016.png
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/44028.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/45144.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/45176.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/45415.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/46578.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/46659.png
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/4678.png
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/4754.png
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/48758.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/48888.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/49130.png
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/4929.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/51938.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/53070.png
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/53682.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/53841.png
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/54538.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/54687.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/55063.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/5532.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/56166.png
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/56205.png
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/5658.png
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/57531.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/58596.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/58967.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/59314.png
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/6376.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/6542.png
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/6934.png
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/7006.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/7538.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/7873.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/8066.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/8216.png
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/8318.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/train/9/9238.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/10.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/1570.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/2531.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/2568.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/525.png
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/5321.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/546.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/7449.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/7703.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/0/9687.png
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/135.png
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/3026.png
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/5318.png
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/5666.png
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/672.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/6789.png
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/7226.png
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/7405.png
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/8636.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/1/9955.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/1065.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/2260.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/237.png
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/3260.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/404.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/5692.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/6084.png
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/6466.png
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/6949.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/2/7683.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/2347.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/245.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/2551.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/2989.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/3129.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/5904.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/6542.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/7656.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/9872.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/3/9882.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/2053.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/2306.png
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/3233.png
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/3282.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/3341.png
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/3544.png
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/3653.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/3841.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/5032.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/4/6369.png
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/2279.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/2515.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/4763.png
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/5518.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/6148.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/6155.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/7067.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/8531.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/8878.png
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/5/9749.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/1886.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/2210.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/3362.png
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/4686.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/5332.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/6630.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/7438.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/7596.png
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/8831.png
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/6/9247.png
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/1012.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/2595.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/3572.png
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/4966.png
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/5190.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/6986.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/8052.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/8248.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/9015.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/7/9837.png
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/2834.png
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/4797.png
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/5433.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/6485.png
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/693.png
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/8217.png
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/8241.png
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/8866.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/9496.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/8/9926.png
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/4272.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/4410.png
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/5787.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/6496.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/6807.png
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/7813.png
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/8184.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/8298.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/9057.png
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/classification/data/reduced_mnist/val/9/9676.png
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/agp.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/feedforward.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/mamba.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/mamba_fft.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/transformer.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/transformer_fft.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/incomplete/create_dataset.py
+-rw-r--r--   0        0        0    77880 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/incomplete/data.csv
+-rw-r--r--   0        0        0    62316 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/incomplete/train/data.csv
+-rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/incomplete/val/data.csv
+-rw-r--r--   0        0        0   381773 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/nylon_wire/train/mixed_10_20.csv
+-rw-r--r--   0        0        0   357293 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/nylon_wire/train/mixed_15_25.csv
+-rw-r--r--   0        0        0   357972 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/nylon_wire/train/mixed_20_30.csv
+-rw-r--r--   0        0        0   357304 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/nylon_wire/train/sin_20.csv
+-rw-r--r--   0        0        0   438969 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/nylon_wire/train/sin_30.csv
+-rw-r--r--   0        0        0   354814 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/nylon_wire/train/sin_40.csv
+-rw-r--r--   0        0        0   381390 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/nylon_wire/train/tri_20.csv
+-rw-r--r--   0        0        0   590643 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/nylon_wire/train/tri_30.csv
+-rw-r--r--   0        0        0   485182 2020-02-02 00:00:00.000000 catasta-0.2.2/examples/regression/data/nylon_wire/val/tri_40.csv
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_classification_dataset.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_decimation.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_deepar_predictor.py
+-rw-r--r--   0        0        0    13249 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_gpformer_regressor.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_kalman_filter.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_load_class_model.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_load_model.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_regression_dataset.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_save_class_model.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_save_model.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_transformer_signal_classifier.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 catasta-0.2.2/tests/test_window_sliding.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 catasta-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 catasta-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 catasta-0.2.2/README.md
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 catasta-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 catasta-0.2.2/PKG-INFO
```

### Comparing `catasta-0.2.1/assets/catasta.svg` & `catasta-0.2.2/assets/catasta.svg`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/archways/archway.py` & `catasta-0.2.2/catasta/archways/archway.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             raise ValueError("Invalid dtype")
 
 
 class Archway:
     """A class for inference with a trained model.
     """
 
-    def __init__(self, *,
+    def __init__(self,
                  path: str,
                  device: str = "auto",
                  dtype: str = "float32",
                  verbose: bool = True,
                  ) -> None:
         """Initialize the Archway object.
```

### Comparing `catasta-0.2.1/catasta/dataclasses/eval_info.py` & `catasta-0.2.2/catasta/dataclasses/eval_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             self._calculate_classification_metrics(self.true_output, self.predicted_output, n_classes)
         else:
             raise ValueError('Invalid task type')
 
     def _calculate_regression_metrics(self, y: np.ndarray, y_pred: np.ndarray) -> None:
         self.mae: float = np.mean(np.abs(y - y_pred)).astype(float)
         self.mse: float = np.mean((y - y_pred)**2).astype(float)
-        self.rmse: float = np.sqrt(np.mean((y - y_pred)**2))
+        self.rmse: float = np.sqrt(np.mean((y - y_pred)**2)).astype(float)
         self.r2: float = 1 - np.sum((y - y_pred)**2) / np.sum((y - np.mean(y))**2).astype(float)
 
     def _calculate_classification_metrics(self, y: np.ndarray, y_pred: np.ndarray, n_classes: int | None) -> None:
         self.confusion_matrix: np.ndarray = self._compute_confusion_matrix(y, y_pred, n_classes)
 
         self.tp: np.ndarray = np.diag(self.confusion_matrix)
         self.fp: np.ndarray = np.sum(self.confusion_matrix, axis=0) - self.tp
```

### Comparing `catasta-0.2.1/catasta/dataclasses/prediction_info.py` & `catasta-0.2.2/catasta/dataclasses/prediction_info.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/dataclasses/train_info.py` & `catasta-0.2.2/catasta/dataclasses/train_info.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/datasets/catasta_dataset.py` & `catasta-0.2.2/catasta/datasets/catasta_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import NamedTuple, Literal
+from typing import NamedTuple
 
 import pandas as pd
 import numpy as np
 from PIL import Image
 
 import torch
 from torch import Tensor
@@ -73,49 +73,52 @@
         The validation subset of the dataset.
     test : Dataset
         The test subset of the dataset.
     """
 
     def __init__(self,
                  root: str,
-                 task: Literal["regression", "classification"],
+                 task: str,
                  input_transformations: list[Transformation] = [],
                  output_transformations: list[Transformation] = [],
                  input_name: str | list[str] = "input",
                  output_name: str = "output",
+                 grayscale: bool = False,
                  ) -> None:
         """Initialize the CatastaDataset object.
 
         Parameters
         ----------
         root : str_
             The root directory of the Catasta dataset.
-        task : Literal["regression", "classification"]
-            The task of the dataset.
+        task : str
+            The task of the dataset. Either 'regression' or 'classification'.
         input_transformations : list[~catasta.transformations.Transformation], optional
             A list of transformations to apply to the input data, by default [].
         output_transformations : list[~catasta.transformations.Transformation], optional
             A list of transformations to apply to the output data, by default [].
         input_name : str | list[str], optional
             The name of the columns in the CSV files that contains the input data, by default "input".
         output_name : str, optional
             The name of the column in the CSV files that contains the output data, by default "output".
+        grayscale : bool, optional
+            Whether to convert the images to grayscale, by default False.
 
         Raises
         ------
         ValueError
             If the root directory does not exist.
             If the task is not 'regression' or 'classification'.
             If the train split is not found.
             If the validation split is not found and the test split is not found.
             If the directories do not contain at least one CSV file (regression).
             If the number of classes in the train and validation splits are not the same (classification).
             If the number of classes in the train and test splits are not the same (classification).
         """
-        self.task: Literal["regression", "classification"] = task
+        self.task: str = task
         self.root: str = root if root.endswith("/") else root + "/"
         if not os.path.isdir(self.root):
             raise ValueError(f"root must be a directory. Found {self.root}")
 
         splits: tuple[str, str, str] = scan_splits(self.root)
 
         if self.task == "regression":
@@ -136,20 +139,23 @@
                                                   output_transformations,
                                                   input_name,
                                                   output_name,
                                                   )
         elif self.task == "classification":
             self.train: Dataset = ClassificationSubset(self.root + splits[0],
                                                        input_transformations,
+                                                       grayscale,
                                                        )
             self.validation: Dataset = ClassificationSubset(self.root + splits[1],
                                                             input_transformations,
+                                                            grayscale,
                                                             )
             self.test: Dataset = ClassificationSubset(self.root + splits[2],
                                                       input_transformations,
+                                                      grayscale,
                                                       )
 
             # same number of classes in all splits
             if len(self.train.classes) == 0:
                 raise ValueError(f"no classes found in {self.train.path}")
 
             if len(self.train.classes) != len(self.validation.classes):
@@ -218,18 +224,19 @@
     label: str
 
 
 class ClassificationSubset(Dataset):
     def __init__(self,
                  path: str,
                  input_transformations: list[Transformation],
+                 grayscale: bool,
                  ) -> None:
         self.path: str = path if path.endswith("/") else path + "/"
-
         self.input_transformations: list[Transformation] = input_transformations
+        self.grayscale: bool = grayscale
 
         self.classes: list[str] = scan_classes(path)
         self.samples: list[Sample] = []
         for class_name in self.classes:
             class_path: str = os.path.join(path, class_name)
 
             # continue if a file is found
@@ -252,15 +259,15 @@
         sample: Sample = self.samples[index]
 
         if sample.path.endswith(".csv"):
             sample_array: np.ndarray = pd.read_csv(sample.path).to_numpy()
         else:
             with open(sample.path, "rb") as f:
                 img: Image.Image = Image.open(f)
-                img = img.convert("RGB")
+                img = img.convert("RGB" if not self.grayscale else "L")
 
             sample_array: np.ndarray = np.array(img)
 
         for transformation in self.input_transformations:
             sample_array = transformation(sample_array)
 
         label: int = self.classes.index(sample.label)
```

### Comparing `catasta-0.2.1/catasta/models/__init__.py` & `catasta-0.2.2/catasta/models/__init__.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/classifiers/cnn_classifier.py` & `catasta-0.2.2/catasta/models/classifiers/cnn_classifier.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/classifiers/feedforward_classifier.py` & `catasta-0.2.2/catasta/models/classifiers/feedforward_classifier.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/classifiers/mamba_classifier.py` & `catasta-0.2.2/catasta/models/classifiers/mamba_classifier.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/classifiers/mamba_fft_classifier.py` & `catasta-0.2.2/catasta/models/classifiers/mamba_fft_classifier.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/classifiers/transformer_classifier.py` & `catasta-0.2.2/catasta/models/classifiers/transformer_classifier.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/classifiers/transformer_fft_classifier.py` & `catasta-0.2.2/catasta/models/classifiers/transformer_fft_classifier.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/regressors/approximate_gp_regressor.py` & `catasta-0.2.2/catasta/models/regressors/approximate_gp_regressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 class ApproximateGPRegressor(ApproximateGP):
     def __init__(self, *,
                  n_inducing_points: int,
                  context_length: int,
                  kernel: str = "rq",
                  mean: str = "constant",
-                 use_ard: bool = False,
+                 use_ard: bool = True,
                  ) -> None:
         '''
         Arguments
         ---------
         n_inducing_points: int
             Number of inducing points
         context_length: int
```

### Comparing `catasta-0.2.1/catasta/models/regressors/feedforward_regressor.py` & `catasta-0.2.2/catasta/models/regressors/feedforward_regressor.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/regressors/mamba_fft_regressor.py` & `catasta-0.2.2/catasta/models/regressors/mamba_fft_regressor.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/regressors/mamba_regressor.py` & `catasta-0.2.2/catasta/models/regressors/mamba_regressor.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/regressors/transformer_fft_regressor.py` & `catasta-0.2.2/catasta/models/regressors/transformer_fft_regressor.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/models/regressors/transformer_regressor.py` & `catasta-0.2.2/catasta/models/regressors/transformer_regressor.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/scaffolds/scaffold.py` & `catasta-0.2.2/catasta/scaffolds/scaffold.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,16 @@
             Whether to print training information or not. Defaults to True.
         """
         self.task: str = dataset.task
 
         self.device: torch.device = _get_device(device)
         self.dtype: torch.dtype = _get_dtype(dtype)
 
+        self.verbose: bool = verbose
+
         self.model: Module = model.to(self.device, self.dtype)
         if isinstance(self.model, GP) and likelihood is None:
             self.likelihood: Module = get_likelihood("gaussian").to(self.device, self.dtype)
         else:
             self.likelihood: Module = get_likelihood(likelihood).to(self.device, self.dtype)
 
         self.dataset: CatastaDataset = dataset
@@ -105,21 +107,32 @@
 
         self.logger: Logger = Logger("catasta", disable=not verbose)
         self._log_training_info()
 
         if probabilistic:
             self.logger.warning("probabilistic models are not yet supported")
 
+    def _log_training_info(self) -> None:
+        n_params: int = sum(p.numel() for p in self.model.parameters() if p.requires_grad)
+        device_name: str = torch.cuda.get_device_name() if self.device.type == "cuda" else platform.processor()
+        n_samples: int = len(self.dataset.train)  # type: ignore
+        self.logger.info(f"""training
+    -> task:     {self.task}
+    -> dataset:  {self.dataset.root} ({n_samples} samples)
+    -> model:    {self.model.__class__.__name__} ({n_params} trainable parameters)
+    -> device:   {self.device} ({device_name})""")
+
     def train(self, *,
               epochs: int,
               batch_size: int,
               lr: float,
               final_lr: float | None = None,
               early_stopping: bool = False,
               shuffle: bool = True,
+              data_loader_workers: int = 0,
               ) -> TrainInfo:
         """Train the model on the dataset.
 
         Arguments
         ---------
         epochs : int
             The number of epochs to train the model.
@@ -129,47 +142,63 @@
             The initial learning rate.
         final_lr : float, optional
             The final learning rate. If not provided, the learning rate is not decayed. Defaults to None.
         early_stopping : bool, optional
             Whether to use early stopping or not. The criterion for early stopping is the derivative of the validation loss. Defaults to False.
         shuffle : bool, optional
             Whether to shuffle the training data or not. Defaults to True.
+        data_loader_workers : int, optional
+            The number of workers to use for the data loader. Defaults to 0.
         """
         # VARIABLES
         optimizer: Optimizer = get_optimizer(self.optimizer_id, [self.model, self.likelihood], lr)
         loss_function: Module = get_loss_function(self.loss_function_id, self.model, self.likelihood, len(self.dataset.train))  # type: ignore
 
         model_state_manager: ModelStateManager = ModelStateManager(early_stopping)
         lr_decay: float = (final_lr / lr) ** (1 / epochs) if final_lr else 1.0
         scheduler: StepLR = StepLR(optimizer, step_size=1, gamma=lr_decay)
 
         training_logger: TrainingLogger = TrainingLogger(self.task, epochs)
 
-        train_data_loader: DataLoader = DataLoader(self.dataset.train, batch_size=batch_size, shuffle=shuffle)
-        val_data_loader: DataLoader = DataLoader(self.dataset.validation, batch_size=batch_size, shuffle=False)
+        train_data_loader: DataLoader = DataLoader(
+            self.dataset.train,
+            batch_size=batch_size,
+            shuffle=shuffle,
+            num_workers=data_loader_workers,
+            pin_memory=True if self.device.type == "cuda" else False,
+        )
+        val_data_loader: DataLoader = DataLoader(
+            self.dataset.validation,
+            batch_size=batch_size,
+            shuffle=False,
+            num_workers=data_loader_workers,
+            pin_memory=True if self.device.type == "cuda" else False,
+        )
 
         # TRAINING LOOP
         for epoch in range(epochs):
             start_time: float = time.time()
 
             # train
             self.model.train()
             self.likelihood.train()
 
-            train_loss, train_accuracy = _epoch(self.task, [self.model, self.likelihood], train_data_loader, optimizer, loss_function, self.device, self.dtype)
+            train_loss, train_accuracy = self._epoch(train_data_loader, optimizer, loss_function)
 
             # validation
             self.model.eval()
             self.likelihood.eval()
 
             with torch.no_grad():
-                val_loss, val_accuracy = _epoch(self.task, [self.model, self.likelihood], val_data_loader, None, loss_function, self.device, self.dtype)
+                val_loss, val_accuracy = self._epoch(val_data_loader, None, loss_function)
 
             scheduler.step()
 
+            torch.cuda.empty_cache() if self.device.type == "cuda" else None
+
             model_state_manager([self.model, self.likelihood], val_loss)
 
             if model_state_manager.stop:
                 self.logger.warning(f"early stopping at epoch {epoch + 1}")
                 break
 
             time_per_epoch = time.time() - start_time
@@ -180,15 +209,15 @@
                 val_loss=val_loss,
                 val_accuracy=val_accuracy,
                 lr=optimizer.param_groups[0]["lr"],
                 epoch=epoch + 1,
                 time_per_epoch=time_per_epoch,
             )
 
-            Logger.plain(training_logger, color="green")
+            Logger.plain(training_logger, color="green") if self.verbose else None
 
         # END OF TRAINING
         train_info = training_logger.get_info()
 
         model_state_manager.load_best_model_state([self.model, self.likelihood])
 
         return train_info
@@ -245,24 +274,14 @@
                 continue
 
             model_path: str = os.path.join(save_path, f"{model.__class__.__name__}.pt")
             torch.save(model, model_path)
 
             self.logger.info(f"model saved to {model_path}")
 
-    def _log_training_info(self) -> None:
-        n_params: int = sum(p.numel() for p in self.model.parameters() if p.requires_grad)
-        device_name: str = torch.cuda.get_device_name() if self.device.type == "cuda" else platform.processor()
-        n_samples: int = len(self.dataset.train)  # type: ignore
-        self.logger.info(f"""training
-    -> task: {self.task}
-    -> dataset: {self.dataset.root} ({n_samples} samples)
-    -> model: {self.model.__class__.__name__} ({n_params} trainable parameters)
-    -> device: {self.device} ({device_name}""")
-
     @torch.no_grad()
     def _evaluate_regression(self, dataset: Dataset) -> EvalInfo:
         x, y = next(iter(DataLoader(dataset, batch_size=len(dataset), shuffle=False)))  # type: ignore
 
         x: Tensor = x.to(self.device, dtype=self.dtype)
         y: Tensor = y.to(self.device, dtype=self.dtype)
 
@@ -301,46 +320,41 @@
 
         return EvalInfo(
             task="classification",
             true_output=np.concatenate(true_labels),
             predicted_output=np.concatenate(predicted_labels),
         )
 
+    def _epoch(self,
+               data_loader: DataLoader,
+               optimizer: Optimizer | None,
+               loss_function: Module,
+               ) -> tuple[float, float]:
+        cumulated_loss: float = 0.0
+        total_samples: int = 0
+        correct_predictions: int = 0
+        for inputs, targets in data_loader:
+            inputs: Tensor = inputs.to(self.device, self.dtype)
+            targets: Tensor = targets.to(self.device, self.dtype if self.task == "regression" else torch.long)
+
+            optimizer.zero_grad() if optimizer is not None else None
+
+            output = self.likelihood(self.model(inputs))
+
+            loss: Tensor = loss_function(output, targets)  # type: ignore
+            if isinstance(loss_function, MarginalLogLikelihood):
+                loss = -loss
+
+            loss.backward() if optimizer is not None else None
+            torch.nn.utils.clip_grad_norm_(self.model.parameters(), 1.0) if optimizer is not None else None  # type: ignore
+
+            optimizer.step() if optimizer is not None else None
+
+            cumulated_loss += loss.item() * inputs.shape[0]
+            total_samples += inputs.shape[0]
+            if self.task == "classification":
+                correct_predictions += (output.argmax(dim=1) == targets).sum().item()  # type: ignore
 
-def _epoch(task: str,
-           models: list[Module],
-           data_loader: DataLoader,
-           optimizer: Optimizer | None,
-           loss_function: Module,
-           device: torch.device,
-           dtype: torch.dtype,
-           ) -> tuple[float, float]:
-    cumulated_loss: float = 0.0
-    total_samples: int = 0
-    correct_predictions: int = 0
-    for inputs, targets in data_loader:
-        inputs: Tensor = inputs.to(device, dtype)
-        targets: Tensor = targets.to(device, dtype if task == "regression" else torch.long)
-
-        optimizer.zero_grad() if optimizer is not None else None
-
-        outputs = models[0](inputs)
-        if len(models) > 1:
-            for model in models[1:]:
-                outputs = model(outputs)
-
-        loss: Tensor = loss_function(outputs, targets)  # type: ignore
-        if isinstance(loss_function, MarginalLogLikelihood):
-            loss = -loss
-
-        loss.backward() if optimizer is not None else None
-        optimizer.step() if optimizer is not None else None
-
-        cumulated_loss += loss.item() * inputs.shape[0]
-        total_samples += inputs.shape[0]
-        if task == "classification":
-            correct_predictions += (outputs.argmax(dim=1) == targets).sum().item()  # type: ignore
-
-    epoch_loss = cumulated_loss / total_samples
-    epoch_accuracy = correct_predictions / total_samples if task == "classification" else -np.inf
+        epoch_loss = cumulated_loss / total_samples
+        epoch_accuracy = correct_predictions / total_samples if self.task == "classification" else -np.inf
 
-    return epoch_loss, epoch_accuracy
+        return epoch_loss, epoch_accuracy
```

### Comparing `catasta-0.2.1/catasta/scaffolds/utils/likelihood_factory.py` & `catasta-0.2.2/catasta/scaffolds/utils/likelihood_factory.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/scaffolds/utils/loss_function_factory.py` & `catasta-0.2.2/catasta/scaffolds/utils/loss_function_factory.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/scaffolds/utils/model_state_manager.py` & `catasta-0.2.2/catasta/scaffolds/utils/model_state_manager.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/scaffolds/utils/objective_function_factory.py` & `catasta-0.2.2/catasta/scaffolds/utils/objective_function_factory.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/scaffolds/utils/optimizer_factory.py` & `catasta-0.2.2/catasta/scaffolds/utils/optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/scaffolds/utils/training_logger.py` & `catasta-0.2.2/catasta/scaffolds/utils/training_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,32 +50,32 @@
             lr_values=np.array(self.lr_values),
         )
 
     def __repr__(self) -> str:
         epoch: int = len(self.train_losses)
         percentage: float = epoch / self.epochs
         percentage_str: str = f"{int(percentage * 100)}%" if percentage > 0.09 else f"0{int(percentage * 100)}%"
-        epoch_msg: str = f"    -> epoch: {epoch}/{self.epochs} ({percentage_str})\n"
+        epoch_msg: str = f"    -> epoch:    {epoch}/{self.epochs} ({percentage_str})\n"
 
         # LOSS
         train_loss: str = f"{self.train_losses[-1]:.4f}"
         val_loss: str = f"{self.val_losses[-1]:.4f}"
         best_val_loss: str = f"{min(self.val_losses):.4f}"
-        loss_msg: str = f"    -> loss: train({train_loss}), val({val_loss}), best({best_val_loss})\n"
+        loss_msg: str = f"    -> loss:     train({train_loss}), val({val_loss}), best({best_val_loss})\n"
 
         # ACCURACY
         train_accuracy: str = f"{self.train_accuracies[-1]:.4f}" if len(self.train_accuracies) > 0 else ""
         val_accuracy: str = f"{self.val_accuracies[-1]:.4f}" if len(self.val_accuracies) > 0 else ""
         best_val_accuracy: str = f"{max(self.val_accuracies):.4f}" if len(self.val_accuracies) > 0 else ""
         accuracy_msg: str = f"    -> accuracy: train({train_accuracy}), val({val_accuracy}), best({best_val_accuracy})\n" if len(self.train_accuracies) > 0 else ""
 
         # TIME
         time_remaining: int = int(self.avg_time_per_epoch * (self.epochs - len(self.train_losses)))
         time_remaining_str: str = f"{int(time_remaining/60)}m {time_remaining%60}s"
-        time_msg: str = f"    -> time remaining: {time_remaining_str}"
+        time_msg: str = f"    -> time:     {time_remaining_str}"
 
         clear_line: str = "\x1b[2K" + "\r" + "\x1b[1A"
 
         msg: str = ""
         if epoch != 1:
             msg += clear_line*4 if self.task == "classification" else clear_line*3
```

### Comparing `catasta-0.2.1/catasta/transformations/custom.py` & `catasta-0.2.2/catasta/transformations/custom.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/transformations/decimation.py` & `catasta-0.2.2/catasta/transformations/decimation.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/transformations/diff_and_concat.py` & `catasta-0.2.2/catasta/transformations/diff_and_concat.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/transformations/fir_filtering.py` & `catasta-0.2.2/catasta/transformations/fir_filtering.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/transformations/kalman_filter.py` & `catasta-0.2.2/catasta/transformations/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/catasta/transformations/normalization.py` & `catasta-0.2.2/catasta/transformations/normalization.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/classification/cnn.py` & `catasta-0.2.2/examples/classification/cnn.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/classification/feedforward.py` & `catasta-0.2.2/examples/classification/feedforward.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/classification/mamba.py` & `catasta-0.2.2/examples/classification/mamba.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/classification/mamba_fft.py` & `catasta-0.2.2/examples/classification/mamba_fft.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/classification/transformer.py` & `catasta-0.2.2/examples/classification/transformer.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/classification/transformer_fft.py` & `catasta-0.2.2/examples/classification/transformer_fft.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/agp.py` & `catasta-0.2.2/examples/regression/agp.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/feedforward.py` & `catasta-0.2.2/examples/regression/feedforward.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/mamba.py` & `catasta-0.2.2/examples/regression/mamba.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/mamba_fft.py` & `catasta-0.2.2/examples/regression/mamba_fft.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/transformer.py` & `catasta-0.2.2/examples/regression/transformer_fft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from catasta import Scaffold, CatastaDataset
-from catasta.models import TransformerRegressor
+from catasta.models import TransformerFFTRegressor
 from catasta.transformations import (
     Normalization,
     WindowSliding,
     Slicing,
     Custom,
 )
 from catasta.dataclasses import EvalInfo
@@ -26,15 +26,15 @@
     dataset = CatastaDataset(
         root=dataset_root,
         task="regression",
         input_transformations=input_trasnsformations,
         output_transformations=output_trasnsformations,
     )
 
-    model = TransformerRegressor(
+    model = TransformerFFTRegressor(
         context_length=n_dim,
         n_patches=8,
         d_model=8,
         n_heads=4,
         n_layers=2,
         feedforward_dim=4,
         head_dim=4,
```

### Comparing `catasta-0.2.1/examples/regression/transformer_fft.py` & `catasta-0.2.2/examples/regression/transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from catasta import Scaffold, CatastaDataset
-from catasta.models import TransformerFFTRegressor
+from catasta.models import TransformerRegressor
 from catasta.transformations import (
     Normalization,
     WindowSliding,
     Slicing,
     Custom,
 )
 from catasta.dataclasses import EvalInfo
@@ -26,15 +26,15 @@
     dataset = CatastaDataset(
         root=dataset_root,
         task="regression",
         input_transformations=input_trasnsformations,
         output_transformations=output_trasnsformations,
     )
 
-    model = TransformerFFTRegressor(
+    model = TransformerRegressor(
         context_length=n_dim,
         n_patches=8,
         d_model=8,
         n_heads=4,
         n_layers=2,
         feedforward_dim=4,
         head_dim=4,
@@ -49,14 +49,15 @@
 
     scaffold.train(
         epochs=10,
         batch_size=256,
         lr=1e-3,
         final_lr=1e-4,
         early_stopping=True,
+        data_loader_workers=4,
     )
 
     info: EvalInfo = scaffold.evaluate()
     print(info)
 
 
 if __name__ == '__main__':
```

### Comparing `catasta-0.2.1/examples/regression/data/incomplete/create_dataset.py` & `catasta-0.2.2/examples/regression/data/incomplete/create_dataset.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/incomplete/data.csv` & `catasta-0.2.2/examples/regression/data/incomplete/data.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/incomplete/train/data.csv` & `catasta-0.2.2/examples/regression/data/incomplete/train/data.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/incomplete/val/data.csv` & `catasta-0.2.2/examples/regression/data/incomplete/val/data.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/nylon_wire/train/mixed_10_20.csv` & `catasta-0.2.2/examples/regression/data/nylon_wire/train/mixed_10_20.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/nylon_wire/train/mixed_15_25.csv` & `catasta-0.2.2/examples/regression/data/nylon_wire/train/mixed_15_25.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/nylon_wire/train/mixed_20_30.csv` & `catasta-0.2.2/examples/regression/data/nylon_wire/train/mixed_20_30.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/nylon_wire/train/sin_20.csv` & `catasta-0.2.2/examples/regression/data/nylon_wire/train/sin_20.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/nylon_wire/train/sin_30.csv` & `catasta-0.2.2/examples/regression/data/nylon_wire/train/sin_30.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/nylon_wire/train/sin_40.csv` & `catasta-0.2.2/examples/regression/data/nylon_wire/train/sin_40.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/nylon_wire/train/tri_20.csv` & `catasta-0.2.2/examples/regression/data/nylon_wire/train/tri_20.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/nylon_wire/train/tri_30.csv` & `catasta-0.2.2/examples/regression/data/nylon_wire/train/tri_30.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/examples/regression/data/nylon_wire/val/tri_40.csv` & `catasta-0.2.2/examples/regression/data/nylon_wire/val/tri_40.csv`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/tests/test_deepar_predictor.py` & `catasta-0.2.2/tests/test_deepar_predictor.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/tests/test_gpformer_regressor.py` & `catasta-0.2.2/tests/test_gpformer_regressor.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/tests/test_kalman_filter.py` & `catasta-0.2.2/tests/test_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/tests/test_load_class_model.py` & `catasta-0.2.2/tests/test_load_class_model.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/tests/test_load_model.py` & `catasta-0.2.2/tests/test_load_model.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/tests/test_regression_dataset.py` & `catasta-0.2.2/tests/test_regression_dataset.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/tests/test_save_class_model.py` & `catasta-0.2.2/tests/test_save_class_model.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/tests/test_save_model.py` & `catasta-0.2.2/tests/test_save_model.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/tests/test_transformer_signal_classifier.py` & `catasta-0.2.2/tests/test_transformer_signal_classifier.py`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/LICENSE` & `catasta-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/README.md` & `catasta-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `catasta-0.2.1/pyproject.toml` & `catasta-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "catasta"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Vistor" },
 ]
 description = "Catasta is a Python library designed to simplify and accelerate the process of machine learning model experimentation. It encapsulates the complexities of model training and evaluation, offering researchers and developers a straightforward pipeline for rapid model assessment with minimal setup required."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `catasta-0.2.1/PKG-INFO` & `catasta-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: catasta
-Version: 0.2.1
+Version: 0.2.2
 Summary: Catasta is a Python library designed to simplify and accelerate the process of machine learning model experimentation. It encapsulates the complexities of model training and evaluation, offering researchers and developers a straightforward pipeline for rapid model assessment with minimal setup required.
 Project-URL: Homepage, https://github.com/vistormu/catasta
 Project-URL: Issues, https://github.com/vistormu/catasta/issues
 Author: Vistor
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

