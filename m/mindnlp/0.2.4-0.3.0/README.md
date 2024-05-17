# Comparing `tmp/mindnlp-0.2.4-py3-none-any.whl.zip` & `tmp/mindnlp-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,36 @@
-Zip file size: 5267764 bytes, number of entries: 1002
+Zip file size: 3742214 bytes, number of entries: 1036
 -r--------  2.0 unx     1162 b- defN 24-Mar-25 11:12 mindnlp/__init__.py
--r--------  2.0 unx     2170 b- defN 24-Mar-20 16:25 mindnlp/configs.py
--r--------  2.0 unx    37726 b- defN 24-Apr-09 06:51 mindnlp/injection.py
--r--------  2.0 unx        0 b- defN 24-Mar-29 08:44 mindnlp/readme.md
--r--------  2.0 unx     5132 b- defN 24-Mar-29 07:53 mindnlp/_csrc/cuda/flash.cu
+-r--------  2.0 unx     2099 b- defN 24-Apr-23 14:20 mindnlp/amp.py
+-r--------  2.0 unx     2302 b- defN 24-Apr-23 15:19 mindnlp/configs.py
+-r--------  2.0 unx    44332 b- defN 24-May-06 12:16 mindnlp/injection.py
+-r--------  2.0 unx    29929 b- defN 24-Apr-23 14:20 mindnlp/_csrc/cuda/flash.cu
 -r--------  2.0 unx     7940 b- defN 23-Jun-01 14:35 mindnlp/_csrc/cuda/wkv.cu
 -r--------  2.0 unx      707 b- defN 23-Mar-22 09:42 mindnlp/_legacy/__init__.py
 -r--------  2.0 unx     7978 b- defN 24-Mar-25 11:12 mindnlp/_legacy/amp.py
--r--------  2.0 unx    67590 b- defN 24-Mar-25 11:12 mindnlp/_legacy/functional.py
+-r--------  2.0 unx    67596 b- defN 24-Apr-23 14:20 mindnlp/_legacy/functional.py
 -r--------  2.0 unx     2633 b- defN 24-Mar-25 11:12 mindnlp/_legacy/initializer.py
 -r--------  2.0 unx     3284 b- defN 24-Mar-25 11:12 mindnlp/_legacy/utils.py
+-r--------  2.0 unx      779 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/__init__.py
+-r--------  2.0 unx     8087 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/evaluator.py
+-r--------  2.0 unx      770 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/export.py
+-r--------  2.0 unx      807 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/train_args.py
+-r--------  2.0 unx     1120 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/utils.py
+-r--------  2.0 unx      927 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/callbacks/__init__.py
+-r--------  2.0 unx     5118 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/callbacks/best_model_callback.py
+-r--------  2.0 unx     4086 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/callbacks/callback_manager.py
+-r--------  2.0 unx     4156 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/callbacks/checkpoint_callback.py
+-r--------  2.0 unx     2464 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/callbacks/earlystop_callback.py
+-r--------  2.0 unx     6079 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/callbacks/timer_callback.py
+-r--------  2.0 unx      753 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/trainer/__init__.py
+-r--------  2.0 unx    16871 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/trainer/base.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/trainer/ppo.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/trainer/rm.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/trainer/sft.py
+-r--------  2.0 unx     3704 b- defN 24-Apr-23 14:20 mindnlp/_legacy/engine/trainer/utils.py
 -r--------  2.0 unx      883 b- defN 24-Mar-25 11:12 mindnlp/_legacy/hypercomplex/__init__.py
 -r--------  2.0 unx     1755 b- defN 24-Mar-25 11:12 mindnlp/_legacy/hypercomplex/utils.py
 -r--------  2.0 unx      882 b- defN 24-Mar-16 11:41 mindnlp/_legacy/hypercomplex/complex/__init__.py
 -r--------  2.0 unx     6981 b- defN 24-Mar-16 11:41 mindnlp/_legacy/hypercomplex/complex/_complex_bn_impl.py
 -r--------  2.0 unx    11071 b- defN 24-Mar-25 11:12 mindnlp/_legacy/hypercomplex/complex/_complex_conv_impl.py
 -r--------  2.0 unx     5878 b- defN 24-Mar-25 11:12 mindnlp/_legacy/hypercomplex/complex/_complex_dense_impl.py
 -r--------  2.0 unx     2146 b- defN 24-Mar-16 11:41 mindnlp/_legacy/hypercomplex/complex/_complex_relu.py
@@ -36,196 +53,173 @@
 -r--------  2.0 unx     5893 b- defN 24-Mar-16 11:41 mindnlp/_legacy/hypercomplex/hypercomplex/_hc_conv_impl.py
 -r--------  2.0 unx     5140 b- defN 24-Mar-16 11:41 mindnlp/_legacy/hypercomplex/hypercomplex/_hc_dense_impl.py
 -r--------  2.0 unx    36029 b- defN 24-Mar-25 11:12 mindnlp/_legacy/hypercomplex/hypercomplex/hc_bn.py
 -r--------  2.0 unx    49241 b- defN 24-Mar-25 11:12 mindnlp/_legacy/hypercomplex/hypercomplex/hc_conv.py
 -r--------  2.0 unx    11082 b- defN 24-Mar-25 11:12 mindnlp/_legacy/hypercomplex/hypercomplex/hc_dense.py
 -r--------  2.0 unx    44353 b- defN 24-Mar-25 11:12 mindnlp/_legacy/hypercomplex/hypercomplex/hc_pool.py
 -r--------  2.0 unx     1691 b- defN 24-Mar-25 11:12 mindnlp/_legacy/hypercomplex/hypercomplex/uniform_operator.py
--r--------  2.0 unx     2915 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/hypercomplex_td.py
--r--------  2.0 unx     4383 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/dual_svd.py
--r--------  2.0 unx     4886 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/qr.py
--r--------  2.0 unx      802 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/star_svd.py
--r--------  2.0 unx     3728 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/svd.py
--r--------  2.0 unx      800 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/t_svd.py
--r--------  2.0 unx     6592 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/matrix.py
--r--------  2.0 unx     1431 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/scalar.py
--r--------  2.0 unx      593 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/scalar_visitor.py
--r--------  2.0 unx     4859 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/vector.py
--r--------  2.0 unx     3088 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/complex/_complex_algebra_impl.py
--r--------  2.0 unx      894 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/complex/complex_algebra_factory.py
--r--------  2.0 unx     2640 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/dual/_dual_algebra_impl.py
--r--------  2.0 unx      873 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/dual/dual_algebra_factory.py
--r--------  2.0 unx      594 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_math_obj_impl.py
--r--------  2.0 unx      456 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_matrix_impl.py
--r--------  2.0 unx      858 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_scalar_impl.py
--r--------  2.0 unx      481 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_vector_impl.py
--r--------  2.0 unx      653 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_algebra_factory.py
--r--------  2.0 unx    13424 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_matrix.py
--r--------  2.0 unx     3020 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_scalar.py
--r--------  2.0 unx     9501 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_vector.py
--r--------  2.0 unx     6240 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/real/real_matrix.py
--r--------  2.0 unx     1650 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/real/real_scalar.py
--r--------  2.0 unx     4089 b- defN 24-Apr-09 08:22 mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/real/real_vector.py
+-r--------  2.0 unx     1576 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/__init__.py
+-r--------  2.0 unx     7525 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/accuracy.py
+-r--------  2.0 unx    10364 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/bleu.py
+-r--------  2.0 unx     6201 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/confusion_matrix.py
+-r--------  2.0 unx     4231 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/distinct.py
+-r--------  2.0 unx     6130 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/em_score.py
+-r--------  2.0 unx     8006 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/f1.py
+-r--------  2.0 unx     7665 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/matthews.py
+-r--------  2.0 unx     7280 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/pearson.py
+-r--------  2.0 unx     9898 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/perplexity.py
+-r--------  2.0 unx     7040 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/precision.py
+-r--------  2.0 unx     6746 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/recall.py
+-r--------  2.0 unx    12329 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/rouge.py
+-r--------  2.0 unx     6735 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/spearman.py
+-r--------  2.0 unx     4407 b- defN 24-Apr-23 14:20 mindnlp/_legacy/metrics/utils.py
 -r--------  2.0 unx     1092 b- defN 23-Jun-01 14:35 mindnlp/_legacy/nn/__init__.py
 -r--------  2.0 unx     3367 b- defN 24-Mar-25 11:12 mindnlp/_legacy/nn/dropout.py
 -r--------  2.0 unx      896 b- defN 24-Mar-25 11:12 mindnlp/_legacy/nn/half_op.py
 -r--------  2.0 unx    33081 b- defN 24-Mar-25 11:12 mindnlp/_legacy/nn/transformer.py
 -r--------  2.0 unx      797 b- defN 23-Jun-01 14:35 mindnlp/_legacy/ops/__init__.py
 -r--------  2.0 unx     1196 b- defN 23-Jun-01 14:35 mindnlp/_legacy/ops/parallel.py
 -r--------  2.0 unx      872 b- defN 23-Mar-22 09:42 mindnlp/_legacy/transforms/__init__.py
 -r--------  2.0 unx     2110 b- defN 23-Nov-14 09:23 mindnlp/_legacy/transforms/add_token.py
 -r--------  2.0 unx     1880 b- defN 24-Mar-25 11:12 mindnlp/_legacy/transforms/truncate.py
 -r--------  2.0 unx      822 b- defN 24-Feb-29 06:56 mindnlp/abc/__init__.py
 -r--------  2.0 unx     2926 b- defN 23-Mar-22 09:42 mindnlp/abc/callback.py
--r--------  2.0 unx     5945 b- defN 24-Mar-25 11:12 mindnlp/abc/container.py
+-r--------  2.0 unx     8313 b- defN 24-Apr-23 14:20 mindnlp/abc/container.py
 -r--------  2.0 unx     2870 b- defN 23-Mar-22 09:42 mindnlp/abc/metric.py
 -r--------  2.0 unx     1466 b- defN 23-Mar-22 09:42 mindnlp/abc/register.py
 -r--------  2.0 unx      823 b- defN 24-Feb-29 06:56 mindnlp/abc/models/__init__.py
 -r--------  2.0 unx     6023 b- defN 23-Jun-01 14:35 mindnlp/abc/models/base_model.py
 -r--------  2.0 unx     3414 b- defN 24-Mar-25 11:12 mindnlp/abc/models/seq2seq_model.py
 -r--------  2.0 unx     2934 b- defN 24-Mar-25 11:12 mindnlp/abc/models/seq2vec_model.py
 -r--------  2.0 unx      811 b- defN 23-Mar-22 09:42 mindnlp/abc/modules/__init__.py
 -r--------  2.0 unx     2816 b- defN 23-Mar-22 09:42 mindnlp/abc/modules/decoder.py
 -r--------  2.0 unx     2408 b- defN 23-Jun-01 14:35 mindnlp/abc/modules/embedding.py
 -r--------  2.0 unx     2360 b- defN 23-Mar-22 09:42 mindnlp/abc/modules/encoder.py
 -r--------  2.0 unx        0 b- defN 23-Mar-22 09:42 mindnlp/abc/modules/generator.py
+-r--------  2.0 unx        0 b- defN 24-May-06 12:16 mindnlp/accelerate/__init__.py
+-r--------  2.0 unx        0 b- defN 24-May-06 12:16 mindnlp/accelerate/accelerator.py
+-r--------  2.0 unx        0 b- defN 24-May-06 12:16 mindnlp/accelerate/inference.py
 -r--------  2.0 unx      790 b- defN 24-Mar-25 11:12 mindnlp/data/__init__.py
 -r--------  2.0 unx      736 b- defN 24-Mar-19 16:41 mindnlp/data/io/__init__.py
 -r--------  2.0 unx    34595 b- defN 24-Mar-25 11:12 mindnlp/data/io/audio.py
 -r--------  2.0 unx      768 b- defN 24-Mar-19 16:41 mindnlp/data/processors/__init__.py
 -r--------  2.0 unx    20407 b- defN 24-Mar-25 11:49 mindnlp/data/processors/squad.py
--r--------  2.0 unx      720 b- defN 24-Feb-29 06:56 mindnlp/dataset/__init__.py
+-r--------  2.0 unx      755 b- defN 24-Apr-23 14:20 mindnlp/dataset/__init__.py
 -r--------  2.0 unx    13264 b- defN 24-Mar-28 15:57 mindnlp/dataset/load.py
+-r--------  2.0 unx      907 b- defN 24-Apr-23 14:20 mindnlp/dataset/map_fn.py
 -r--------  2.0 unx     1921 b- defN 23-Mar-22 09:42 mindnlp/dataset/utils.py
 -r--------  2.0 unx     1211 b- defN 24-Apr-01 15:36 mindnlp/dataset/transforms/__init__.py
 -r--------  2.0 unx     9716 b- defN 24-Mar-25 11:12 mindnlp/dataset/transforms/basic_tokenizer.py
 -r--------  2.0 unx     1608 b- defN 24-Apr-01 15:36 mindnlp/dataset/transforms/jieba_tokenizer.py
 -r--------  2.0 unx     2508 b- defN 24-Feb-29 06:56 mindnlp/dataset/transforms/lookup.py
 -r--------  2.0 unx     2548 b- defN 24-Feb-29 06:56 mindnlp/dataset/transforms/pad_transform.py
--r--------  2.0 unx        0 b- defN 24-Apr-08 10:49 mindnlp/diffusers/__init__.py
--r--------  2.0 unx        0 b- defN 24-Apr-08 14:16 mindnlp/diffusers/loaders/__init__.py
--r--------  2.0 unx        0 b- defN 24-Apr-08 14:16 mindnlp/diffusers/models/__init__.py
--r--------  2.0 unx        0 b- defN 24-Apr-08 14:16 mindnlp/diffusers/pipelines/__init__.py
--r--------  2.0 unx        0 b- defN 24-Apr-08 14:16 mindnlp/diffusers/schedulers/__init__.py
--r--------  2.0 unx        0 b- defN 24-Apr-08 14:16 mindnlp/diffusers/utils/__init__.py
--r--------  2.0 unx      779 b- defN 24-Mar-20 16:25 mindnlp/engine/__init__.py
--r--------  2.0 unx     8106 b- defN 24-Mar-20 16:25 mindnlp/engine/evaluator.py
+-r--------  2.0 unx      787 b- defN 24-Apr-23 14:20 mindnlp/engine/__init__.py
+-r--------  2.0 unx    24684 b- defN 24-Apr-23 14:20 mindnlp/engine/callbacks.py
 -r--------  2.0 unx      770 b- defN 23-Mar-22 09:42 mindnlp/engine/export.py
--r--------  2.0 unx      807 b- defN 24-Mar-20 16:25 mindnlp/engine/train_args.py
--r--------  2.0 unx     1125 b- defN 24-Mar-25 11:12 mindnlp/engine/utils.py
--r--------  2.0 unx      927 b- defN 24-Mar-20 16:25 mindnlp/engine/callbacks/__init__.py
--r--------  2.0 unx     5118 b- defN 24-Mar-20 16:25 mindnlp/engine/callbacks/best_model_callback.py
--r--------  2.0 unx     4086 b- defN 24-Mar-20 16:25 mindnlp/engine/callbacks/callback_manager.py
--r--------  2.0 unx     4156 b- defN 24-Mar-20 16:25 mindnlp/engine/callbacks/checkpoint_callback.py
--r--------  2.0 unx     2464 b- defN 24-Mar-20 16:25 mindnlp/engine/callbacks/earlystop_callback.py
--r--------  2.0 unx     6079 b- defN 24-Mar-20 16:25 mindnlp/engine/callbacks/timer_callback.py
+-r--------  2.0 unx    19087 b- defN 24-Apr-23 14:20 mindnlp/engine/utils.py
+-r--------  2.0 unx       39 b- defN 24-Apr-23 14:20 mindnlp/engine/train_args/__init__.py
+-r--------  2.0 unx    94202 b- defN 24-Apr-23 14:20 mindnlp/engine/train_args/base.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/engine/train_args/ddpo.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/engine/train_args/kto.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/engine/train_args/ppo.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/engine/train_args/reward.py
+-r--------  2.0 unx     4248 b- defN 24-Apr-23 14:20 mindnlp/engine/train_args/seq2seq.py
 -r--------  2.0 unx      753 b- defN 24-Mar-25 11:12 mindnlp/engine/trainer/__init__.py
--r--------  2.0 unx    16949 b- defN 24-Mar-25 11:12 mindnlp/engine/trainer/base.py
--r--------  2.0 unx        0 b- defN 24-Mar-20 16:25 mindnlp/engine/trainer/ppo.py
+-r--------  2.0 unx    93556 b- defN 24-Apr-23 14:20 mindnlp/engine/trainer/base.py
+-r--------  2.0 unx     3703 b- defN 24-Apr-23 14:20 mindnlp/engine/trainer/default_func.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/engine/trainer/ppo_trainer.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/engine/trainer/reward_trainer.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/engine/trainer/rl_base.py
 -r--------  2.0 unx        0 b- defN 23-Jun-01 14:35 mindnlp/engine/trainer/rm.py
--r--------  2.0 unx        0 b- defN 24-Mar-20 16:25 mindnlp/engine/trainer/sft.py
--r--------  2.0 unx     3704 b- defN 24-Mar-20 16:25 mindnlp/engine/trainer/utils.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/__init__.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/suite.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/__init__.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/audio_classification.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/automatic_speech_recognition.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/base.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/image_classification.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/question_answering.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/text2text_generation.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/text_classification.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/text_generation.py
--r--------  2.0 unx        0 b- defN 24-Mar-19 16:41 mindnlp/evaluate/evaluator/token_classification.py
--r--------  2.0 unx     1590 b- defN 23-Mar-22 09:42 mindnlp/metrics/__init__.py
--r--------  2.0 unx     7525 b- defN 23-Mar-22 09:42 mindnlp/metrics/accuracy.py
--r--------  2.0 unx    10364 b- defN 23-Mar-22 09:42 mindnlp/metrics/bleu.py
--r--------  2.0 unx     6201 b- defN 23-Mar-22 09:42 mindnlp/metrics/confusion_matrix.py
--r--------  2.0 unx     4231 b- defN 23-Mar-22 09:42 mindnlp/metrics/distinct.py
--r--------  2.0 unx     6130 b- defN 23-Mar-22 09:42 mindnlp/metrics/em_score.py
--r--------  2.0 unx     8006 b- defN 23-Mar-22 09:42 mindnlp/metrics/f1.py
--r--------  2.0 unx     7665 b- defN 23-Mar-22 09:42 mindnlp/metrics/matthews.py
--r--------  2.0 unx     7280 b- defN 23-Mar-22 09:42 mindnlp/metrics/pearson.py
--r--------  2.0 unx     9898 b- defN 23-Mar-22 09:42 mindnlp/metrics/perplexity.py
--r--------  2.0 unx     7040 b- defN 23-Mar-22 09:42 mindnlp/metrics/precision.py
--r--------  2.0 unx     6746 b- defN 23-Mar-22 09:42 mindnlp/metrics/recall.py
--r--------  2.0 unx    12329 b- defN 24-Feb-29 06:56 mindnlp/metrics/rouge.py
--r--------  2.0 unx     6735 b- defN 23-Mar-22 09:42 mindnlp/metrics/spearman.py
--r--------  2.0 unx     4407 b- defN 23-Mar-22 09:42 mindnlp/metrics/utils.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/engine/trainer/seq2seq_trainer.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/engine/trainer/sft_trainer.py
 -r--------  2.0 unx     2229 b- defN 24-Mar-25 11:12 mindnlp/modules/__init__.py
 -r--------  2.0 unx     1966 b- defN 24-Mar-25 11:12 mindnlp/modules/accumulator.py
 -r--------  2.0 unx    22547 b- defN 24-Feb-29 06:56 mindnlp/modules/attentions.py
 -r--------  2.0 unx    13033 b- defN 24-Mar-25 11:12 mindnlp/modules/crf.py
 -r--------  2.0 unx     6458 b- defN 24-Mar-25 11:12 mindnlp/modules/loss.py
+-r--------  2.0 unx    22616 b- defN 24-Apr-23 14:20 mindnlp/modules/optimization.py
 -r--------  2.0 unx    22885 b- defN 24-Mar-25 11:12 mindnlp/modules/rnns.py
 -r--------  2.0 unx     7136 b- defN 24-Mar-30 02:04 mindnlp/modules/weight_norm.py
 -r--------  2.0 unx      702 b- defN 23-Jun-01 14:35 mindnlp/modules/custom/__init__.py
 -r--------  2.0 unx      773 b- defN 23-Mar-22 09:42 mindnlp/modules/decoder/__init__.py
 -r--------  2.0 unx    10869 b- defN 24-Mar-25 11:12 mindnlp/modules/decoder/rnn_decoder.py
 -r--------  2.0 unx      801 b- defN 23-Mar-22 09:42 mindnlp/modules/embeddings/__init__.py
 -r--------  2.0 unx     8276 b- defN 24-Feb-29 06:56 mindnlp/modules/embeddings/fasttext_embedding.py
 -r--------  2.0 unx     8267 b- defN 24-Feb-29 06:56 mindnlp/modules/embeddings/glove_embedding.py
 -r--------  2.0 unx      824 b- defN 23-Mar-22 09:42 mindnlp/modules/encoder/__init__.py
 -r--------  2.0 unx     4712 b- defN 24-Mar-25 11:12 mindnlp/modules/encoder/cnn_encoder.py
 -r--------  2.0 unx     4145 b- defN 24-Mar-25 11:12 mindnlp/modules/encoder/rnn_encoder.py
--r--------  2.0 unx      787 b- defN 24-Apr-08 07:41 mindnlp/modules/functional/__init__.py
+-r--------  2.0 unx      787 b- defN 24-Apr-23 14:20 mindnlp/modules/functional/__init__.py
 -r--------  2.0 unx     2705 b- defN 24-Mar-25 11:12 mindnlp/modules/functional/graph_func.py
 -r--------  2.0 unx      985 b- defN 24-Feb-29 06:56 mindnlp/modules/functional/neural_network.py
--r--------  2.0 unx      838 b- defN 24-Apr-08 07:40 mindnlp/modules/functional/normalize.py
+-r--------  2.0 unx      838 b- defN 24-Apr-23 14:20 mindnlp/modules/functional/normalize.py
 -r--------  2.0 unx     3298 b- defN 24-Mar-25 11:12 mindnlp/modules/functional/weight_norm.py
 -r--------  2.0 unx      846 b- defN 24-Feb-29 06:56 mindnlp/parallel/__init__.py
 -r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/parallel/pipeline_parallel/__init__.py
 -r--------  2.0 unx      818 b- defN 24-Feb-29 06:56 mindnlp/parallel/tensor_parallel/__init__.py
--r--------  2.0 unx    11750 b- defN 24-Mar-25 11:12 mindnlp/parallel/tensor_parallel/layers.py
+-r--------  2.0 unx    11658 b- defN 24-Apr-23 14:20 mindnlp/parallel/tensor_parallel/layers.py
 -r--------  2.0 unx     4587 b- defN 24-Mar-25 11:12 mindnlp/parallel/tensor_parallel/mappings.py
 -r--------  2.0 unx     3369 b- defN 24-Feb-29 06:56 mindnlp/parallel/tensor_parallel/utils.py
--r--------  2.0 unx     1594 b- defN 24-Feb-29 06:56 mindnlp/peft/__init__.py
--r--------  2.0 unx     6758 b- defN 24-Mar-25 11:12 mindnlp/peft/config.py
--r--------  2.0 unx     3322 b- defN 24-Mar-25 11:12 mindnlp/peft/mapping.py
--r--------  2.0 unx    37352 b- defN 24-Mar-25 11:12 mindnlp/peft/peft_model.py
--r--------  2.0 unx      738 b- defN 23-Jul-16 07:16 mindnlp/peft/tuners/__init__.py
--r--------  2.0 unx    37392 b- defN 24-Mar-25 11:12 mindnlp/peft/tuners/lora.py
--r--------  2.0 unx    11619 b- defN 24-Mar-25 11:12 mindnlp/peft/tuners/tuners_utils.py
--r--------  2.0 unx     1756 b- defN 24-Feb-29 06:56 mindnlp/peft/utils/__init__.py
--r--------  2.0 unx    11128 b- defN 24-Mar-25 11:12 mindnlp/peft/utils/other.py
--r--------  2.0 unx     1242 b- defN 24-Feb-29 06:56 mindnlp/peft/utils/peft_types.py
--r--------  2.0 unx     5767 b- defN 24-Mar-25 11:12 mindnlp/peft/utils/save_and_load.py
--r--------  2.0 unx      763 b- defN 24-Apr-01 15:36 mindnlp/text2vec/__init__.py
--r--------  2.0 unx     8215 b- defN 24-Apr-01 15:36 mindnlp/text2vec/sentence_model.py
--r--------  2.0 unx     6109 b- defN 24-Apr-01 15:36 mindnlp/text2vec/word2vec.py
--r--------  2.0 unx     1287 b- defN 24-Feb-29 06:56 mindnlp/transformers/__init__.py
--r--------  2.0 unx     5438 b- defN 24-Apr-08 07:11 mindnlp/transformers/activations.py
+-r--------  2.0 unx     1711 b- defN 24-May-06 12:16 mindnlp/peft/__init__.py
+-r--------  2.0 unx     6932 b- defN 24-Apr-23 14:20 mindnlp/peft/config.py
+-r--------  2.0 unx     3458 b- defN 24-May-06 12:16 mindnlp/peft/mapping.py
+-r--------  2.0 unx    37530 b- defN 24-May-06 12:16 mindnlp/peft/peft_model.py
+-r--------  2.0 unx      898 b- defN 24-May-06 12:16 mindnlp/peft/tuners/__init__.py
+-r--------  2.0 unx    37353 b- defN 24-May-06 12:16 mindnlp/peft/tuners/lora.py
+-r--------  2.0 unx    21709 b- defN 24-Apr-23 14:20 mindnlp/peft/tuners/tuners_utils.py
+-r--------  2.0 unx      908 b- defN 24-May-06 12:16 mindnlp/peft/tuners/adalora/__init__.py
+-r--------  2.0 unx     2875 b- defN 24-May-06 12:16 mindnlp/peft/tuners/adalora/config.py
+-r--------  2.0 unx    16835 b- defN 24-May-06 12:16 mindnlp/peft/tuners/adalora/layer.py
+-r--------  2.0 unx    17645 b- defN 24-May-06 12:16 mindnlp/peft/tuners/adalora/model.py
+-r--------  2.0 unx      817 b- defN 24-Apr-23 14:20 mindnlp/peft/tuners/adaption_prompt/__init__.py
+-r--------  2.0 unx     2999 b- defN 24-Apr-23 14:20 mindnlp/peft/tuners/adaption_prompt/config.py
+-r--------  2.0 unx     5026 b- defN 24-Apr-23 14:20 mindnlp/peft/tuners/adaption_prompt/layer.py
+-r--------  2.0 unx     6652 b- defN 24-Apr-23 14:20 mindnlp/peft/tuners/adaption_prompt/model.py
+-r--------  2.0 unx     4004 b- defN 24-Apr-23 14:20 mindnlp/peft/tuners/adaption_prompt/utils.py
+-r--------  2.0 unx      860 b- defN 24-Apr-23 14:20 mindnlp/peft/tuners/ia3/__init__.py
+-r--------  2.0 unx     5283 b- defN 24-Apr-23 14:20 mindnlp/peft/tuners/ia3/config.py
+-r--------  2.0 unx    13778 b- defN 24-Apr-23 14:20 mindnlp/peft/tuners/ia3/layer.py
+-r--------  2.0 unx    16862 b- defN 24-May-06 12:16 mindnlp/peft/tuners/ia3/model.py
+-r--------  2.0 unx     1750 b- defN 24-May-06 12:16 mindnlp/peft/utils/__init__.py
+-r--------  2.0 unx    13664 b- defN 24-May-06 12:16 mindnlp/peft/utils/other.py
+-r--------  2.0 unx     1236 b- defN 24-May-06 12:16 mindnlp/peft/utils/peft_types.py
+-r--------  2.0 unx     7130 b- defN 24-May-06 12:16 mindnlp/peft/utils/save_and_load.py
+-r--------  2.0 unx      690 b- defN 24-May-06 12:16 mindnlp/sentence/__init__.py
+-r--------  2.0 unx     1313 b- defN 24-May-06 12:16 mindnlp/transformers/__init__.py
+-r--------  2.0 unx     5438 b- defN 24-Apr-23 14:20 mindnlp/transformers/activations.py
 -r--------  2.0 unx    33460 b- defN 24-Mar-31 16:52 mindnlp/transformers/audio_utils.py
+-r--------  2.0 unx    16335 b- defN 24-May-06 12:16 mindnlp/transformers/backbone_utils.py
 -r--------  2.0 unx    20239 b- defN 24-Mar-25 11:12 mindnlp/transformers/cache_utils.py
--r--------  2.0 unx    35706 b- defN 24-Apr-02 08:27 mindnlp/transformers/configuration_utils.py
+-r--------  2.0 unx    35864 b- defN 24-Apr-23 14:20 mindnlp/transformers/configuration_utils.py
 -r--------  2.0 unx    53285 b- defN 24-Mar-25 11:12 mindnlp/transformers/convert_slow_tokenizer.py
 -r--------  2.0 unx    18222 b- defN 24-Feb-29 06:56 mindnlp/transformers/feature_extraction_sequence_utils.py
 -r--------  2.0 unx    26772 b- defN 24-Apr-02 15:06 mindnlp/transformers/feature_extraction_utils.py
--r--------  2.0 unx    33187 b- defN 24-Mar-28 15:57 mindnlp/transformers/image_processing_utils.py
+-r--------  2.0 unx    34842 b- defN 24-May-06 12:16 mindnlp/transformers/image_processing_utils.py
 -r--------  2.0 unx    32924 b- defN 24-Mar-25 11:12 mindnlp/transformers/image_transforms.py
 -r--------  2.0 unx    29937 b- defN 24-Mar-28 15:57 mindnlp/transformers/image_utils.py
 -r--------  2.0 unx     3025 b- defN 24-Mar-31 10:53 mindnlp/transformers/kernel_utils.py
 -r--------  2.0 unx    10957 b- defN 24-Mar-12 03:14 mindnlp/transformers/modeling_attn_mask_utils.py
 -r--------  2.0 unx   111179 b- defN 24-Mar-12 03:14 mindnlp/transformers/modeling_outputs.py
--r--------  2.0 unx    96613 b- defN 24-Apr-09 05:34 mindnlp/transformers/modeling_utils.py
+-r--------  2.0 unx    95069 b- defN 24-Apr-23 14:20 mindnlp/transformers/modeling_utils.py
 -r--------  2.0 unx     8657 b- defN 24-Mar-25 11:12 mindnlp/transformers/ms_utils.py
 -r--------  2.0 unx    10219 b- defN 24-Mar-28 15:57 mindnlp/transformers/processing_utils.py
 -r--------  2.0 unx     6636 b- defN 24-Mar-25 11:12 mindnlp/transformers/time_series_utils.py
 -r--------  2.0 unx    44063 b- defN 24-Mar-25 11:12 mindnlp/transformers/tokenization_utils.py
--r--------  2.0 unx   175003 b- defN 24-Mar-28 15:57 mindnlp/transformers/tokenization_utils_base.py
+-r--------  2.0 unx   175110 b- defN 24-Apr-23 14:20 mindnlp/transformers/tokenization_utils_base.py
 -r--------  2.0 unx    37089 b- defN 24-Mar-25 11:12 mindnlp/transformers/tokenization_utils_fast.py
--r--------  2.0 unx      829 b- defN 24-Mar-26 08:37 mindnlp/transformers/generation/__init__.py
+-r--------  2.0 unx      854 b- defN 24-May-06 12:16 mindnlp/transformers/generation/__init__.py
 -r--------  2.0 unx    19732 b- defN 24-Mar-25 11:12 mindnlp/transformers/generation/beam_constraints.py
 -r--------  2.0 unx    43463 b- defN 24-Mar-25 11:12 mindnlp/transformers/generation/beam_search.py
--r--------  2.0 unx    32343 b- defN 24-Apr-08 06:51 mindnlp/transformers/generation/configuration_utils.py
--r--------  2.0 unx    66891 b- defN 24-Mar-28 15:57 mindnlp/transformers/generation/logits_process.py
+-r--------  2.0 unx    32343 b- defN 24-Apr-08 03:51 mindnlp/transformers/generation/configuration_utils.py
+-r--------  2.0 unx    67137 b- defN 24-Apr-23 14:20 mindnlp/transformers/generation/logits_process.py
 -r--------  2.0 unx     5067 b- defN 24-Feb-29 06:56 mindnlp/transformers/generation/stopping_criteria.py
 -r--------  2.0 unx     9287 b- defN 24-Mar-25 11:12 mindnlp/transformers/generation/streamers.py
--r--------  2.0 unx   252173 b- defN 24-Apr-08 15:07 mindnlp/transformers/generation/utils.py
--r--------  2.0 unx     7060 b- defN 24-Apr-08 11:52 mindnlp/transformers/models/__init__.py
+-r--------  2.0 unx   250910 b- defN 24-Apr-23 14:20 mindnlp/transformers/generation/utils.py
+-r--------  2.0 unx     7976 b- defN 24-May-06 12:36 mindnlp/transformers/models/__init__.py
 -r--------  2.0 unx     1120 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/albert/__init__.py
 -r--------  2.0 unx     8303 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/albert/configuration_albert.py
 -r--------  2.0 unx    48840 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/albert/modeling_albert.py
 -r--------  2.0 unx    15804 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/albert/tokenization_albert.py
 -r--------  2.0 unx    11024 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/albert/tokenization_albert_fast.py
 -r--------  2.0 unx      989 b- defN 24-Mar-20 16:25 mindnlp/transformers/models/align/__init__.py
 -r--------  2.0 unx    18320 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/align/configuration_align.py
@@ -236,22 +230,22 @@
 -r--------  2.0 unx    73075 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/altclip/modeling_altclip.py
 -r--------  2.0 unx     6589 b- defN 24-Mar-20 16:25 mindnlp/transformers/models/altclip/processing_altclip.py
 -r--------  2.0 unx     1252 b- defN 24-Mar-20 16:25 mindnlp/transformers/models/audio_spectrogram_transformer/__init__.py
 -r--------  2.0 unx     5830 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/audio_spectrogram_transformer/configuration_audio_spectrogram_transformer.py
 -r--------  2.0 unx     9478 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/audio_spectrogram_transformer/feature_extraction_audio_spectrogram_transformer.py
 -r--------  2.0 unx    22723 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/audio_spectrogram_transformer/modeling_audio_spectrogram_transformer.py
 -r--------  2.0 unx     6545 b- defN 24-Mar-25 06:16 mindnlp/transformers/models/auto/__init__.py
--r--------  2.0 unx    10729 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/auto/auto_factory.py
--r--------  2.0 unx    40590 b- defN 24-Apr-08 11:48 mindnlp/transformers/models/auto/configuration_auto.py
+-r--------  2.0 unx    10903 b- defN 24-May-06 12:16 mindnlp/transformers/models/auto/auto_factory.py
+-r--------  2.0 unx    41697 b- defN 24-May-06 12:32 mindnlp/transformers/models/auto/configuration_auto.py
 -r--------  2.0 unx    18666 b- defN 24-Mar-31 13:25 mindnlp/transformers/models/auto/feature_extraction_auto.py
--r--------  2.0 unx    20881 b- defN 24-Mar-31 12:04 mindnlp/transformers/models/auto/image_processing_auto.py
--r--------  2.0 unx    41547 b- defN 24-Apr-08 11:48 mindnlp/transformers/models/auto/modeling_auto.py
+-r--------  2.0 unx    20918 b- defN 24-May-06 12:16 mindnlp/transformers/models/auto/image_processing_auto.py
+-r--------  2.0 unx    42232 b- defN 24-May-06 12:33 mindnlp/transformers/models/auto/modeling_auto.py
 -r--------  2.0 unx    12314 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/auto/modeling_graph_auto.py
 -r--------  2.0 unx    15357 b- defN 24-Apr-02 15:21 mindnlp/transformers/models/auto/processing_auto.py
--r--------  2.0 unx    39882 b- defN 24-Apr-08 11:45 mindnlp/transformers/models/auto/tokenization_auto.py
+-r--------  2.0 unx    40604 b- defN 24-May-06 12:54 mindnlp/transformers/models/auto/tokenization_auto.py
 -r--------  2.0 unx      935 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/autoformer/__init__.py
 -r--------  2.0 unx    12462 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/autoformer/configuration_autoformer.py
 -r--------  2.0 unx    97091 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/autoformer/modeling_autoformer.py
 -r--------  2.0 unx     1028 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/baichuan/__init__.py
 -r--------  2.0 unx     2461 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/baichuan/configuration_baichuan.py
 -r--------  2.0 unx    43284 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/baichuan/modeling_baichuan.py
 -r--------  2.0 unx     9639 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/baichuan/tokenization_baichuan.py
@@ -267,17 +261,17 @@
 -r--------  2.0 unx    14266 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/bart/tokenization_bart_fast.py
 -r--------  2.0 unx      940 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/barthez/__init__.py
 -r--------  2.0 unx    12831 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/barthez/tokenization_barthez.py
 -r--------  2.0 unx     8996 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/barthez/tokenization_barthez_fast.py
 -r--------  2.0 unx      822 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/bartpho/__init__.py
 -r--------  2.0 unx    14087 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/bartpho/tokenization_bartpho.py
 -r--------  2.0 unx      999 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/beit/__init__.py
--r--------  2.0 unx    11381 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/beit/configuration_beit.py
+-r--------  2.0 unx    11370 b- defN 24-May-06 12:16 mindnlp/transformers/models/beit/configuration_beit.py
 -r--------  2.0 unx    25144 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/beit/image_processing_beit.py
--r--------  2.0 unx    56500 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/beit/modeling_beit.py
+-r--------  2.0 unx    56489 b- defN 24-May-06 12:16 mindnlp/transformers/models/beit/modeling_beit.py
 -r--------  2.0 unx     1196 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/bert/__init__.py
 -r--------  2.0 unx     2598 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/bert/configuration_bert.py
 -r--------  2.0 unx    93194 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/bert/modeling_bert.py
 -r--------  2.0 unx    24981 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/bert/modeling_graph_bert.py
 -r--------  2.0 unx    25179 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/bert/tokenization_bert.py
 -r--------  2.0 unx    14885 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/bert/tokenization_bert_fast.py
 -r--------  2.0 unx     1086 b- defN 24-Mar-25 13:50 mindnlp/transformers/models/bert_generation/__init__.py
@@ -300,17 +294,17 @@
 -r--------  2.0 unx     8577 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py
 -r--------  2.0 unx   134691 b- defN 24-Mar-31 10:53 mindnlp/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py
 -r--------  2.0 unx     1007 b- defN 24-Mar-31 12:01 mindnlp/transformers/models/biogpt/__init__.py
 -r--------  2.0 unx     6499 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/biogpt/configuration_biogpt.py
 -r--------  2.0 unx    34793 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/biogpt/modeling_biogpt.py
 -r--------  2.0 unx    13838 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/biogpt/tokenization_biogpt.py
 -r--------  2.0 unx      989 b- defN 24-Mar-31 12:01 mindnlp/transformers/models/bit/__init__.py
--r--------  2.0 unx     6297 b- defN 24-Mar-31 11:53 mindnlp/transformers/models/bit/configuration_bit.py
+-r--------  2.0 unx     6290 b- defN 24-May-06 12:16 mindnlp/transformers/models/bit/configuration_bit.py
 -r--------  2.0 unx    16448 b- defN 24-Mar-31 11:54 mindnlp/transformers/models/bit/image_processing_bit.py
--r--------  2.0 unx    29567 b- defN 24-Mar-31 12:44 mindnlp/transformers/models/bit/modeling_bit.py
+-r--------  2.0 unx    29560 b- defN 24-May-06 12:16 mindnlp/transformers/models/bit/modeling_bit.py
 -r--------  2.0 unx     1174 b- defN 24-Apr-02 03:19 mindnlp/transformers/models/blenderbot/__init__.py
 -r--------  2.0 unx     7560 b- defN 24-Apr-02 03:19 mindnlp/transformers/models/blenderbot/configuration_blenderbot.py
 -r--------  2.0 unx    64667 b- defN 24-Apr-02 03:19 mindnlp/transformers/models/blenderbot/modeling_blenderbot.py
 -r--------  2.0 unx    19111 b- defN 24-Apr-02 03:19 mindnlp/transformers/models/blenderbot/tokenization_blenderbot.py
 -r--------  2.0 unx    19111 b- defN 24-Apr-02 03:19 mindnlp/transformers/models/blenderbot/tokenization_blenderbot_fast.py
 -r--------  2.0 unx     1252 b- defN 24-Apr-02 08:27 mindnlp/transformers/models/blenderbot_small/__init__.py
 -r--------  2.0 unx     7547 b- defN 24-Apr-02 08:27 mindnlp/transformers/models/blenderbot_small/configuration_blenderbot_small.py
@@ -319,31 +313,31 @@
 -r--------  2.0 unx     4354 b- defN 24-Apr-02 08:27 mindnlp/transformers/models/blenderbot_small/tokenization_blenderbot_small_fast.py
 -r--------  2.0 unx     1087 b- defN 24-Apr-02 15:06 mindnlp/transformers/models/blip/__init__.py
 -r--------  2.0 unx    16456 b- defN 24-Apr-02 15:06 mindnlp/transformers/models/blip/configuration_blip.py
 -r--------  2.0 unx    15742 b- defN 24-Apr-02 15:06 mindnlp/transformers/models/blip/image_processing_blip.py
 -r--------  2.0 unx    53787 b- defN 24-Apr-02 15:06 mindnlp/transformers/models/blip/modeling_blip.py
 -r--------  2.0 unx    43537 b- defN 24-Apr-02 15:06 mindnlp/transformers/models/blip/modeling_blip_text.py
 -r--------  2.0 unx     6235 b- defN 24-Apr-02 15:06 mindnlp/transformers/models/blip/processing_blip.py
--r--------  2.0 unx     1000 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/blip_2/__init__.py
--r--------  2.0 unx    16475 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/blip_2/configuration_blip_2.py
--r--------  2.0 unx    71527 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/blip_2/modeling_blip_2.py
--r--------  2.0 unx     6730 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/blip_2/processing_blip_2.py
+-r--------  2.0 unx     1000 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/blip_2/__init__.py
+-r--------  2.0 unx    16475 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/blip_2/configuration_blip_2.py
+-r--------  2.0 unx    71527 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/blip_2/modeling_blip_2.py
+-r--------  2.0 unx     6730 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/blip_2/processing_blip_2.py
 -r--------  2.0 unx     1012 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/bloom/__init__.py
 -r--------  2.0 unx     7089 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/bloom/configuration_bloom.py
 -r--------  2.0 unx    45166 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/bloom/modeling_bloom.py
 -r--------  2.0 unx     8034 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/bloom/tokenization_bloom_fast.py
--r--------  2.0 unx     1178 b- defN 24-Apr-08 07:51 mindnlp/transformers/models/bridgetower/__init__.py
--r--------  2.0 unx    16296 b- defN 24-Apr-08 07:02 mindnlp/transformers/models/bridgetower/configuration_bridgetower.py
--r--------  2.0 unx    26920 b- defN 24-Apr-08 09:27 mindnlp/transformers/models/bridgetower/image_processing_bridgetower.py
--r--------  2.0 unx    81582 b- defN 24-Apr-08 09:28 mindnlp/transformers/models/bridgetower/modeling_bridgetower.py
--r--------  2.0 unx     5094 b- defN 24-Apr-08 07:04 mindnlp/transformers/models/bridgetower/processing_bridgetower.py
--r--------  2.0 unx      981 b- defN 24-Apr-08 08:35 mindnlp/transformers/models/bros/__init__.py
--r--------  2.0 unx     6419 b- defN 24-Apr-08 08:21 mindnlp/transformers/models/bros/configuration_bros.py
--r--------  2.0 unx    51532 b- defN 24-Apr-08 09:31 mindnlp/transformers/models/bros/modeling_bros.py
--r--------  2.0 unx     4223 b- defN 24-Apr-08 08:21 mindnlp/transformers/models/bros/processing_bros.py
+-r--------  2.0 unx     1178 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/bridgetower/__init__.py
+-r--------  2.0 unx    16296 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/bridgetower/configuration_bridgetower.py
+-r--------  2.0 unx    26920 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/bridgetower/image_processing_bridgetower.py
+-r--------  2.0 unx    81582 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/bridgetower/modeling_bridgetower.py
+-r--------  2.0 unx     5094 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/bridgetower/processing_bridgetower.py
+-r--------  2.0 unx      981 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/bros/__init__.py
+-r--------  2.0 unx     6419 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/bros/configuration_bros.py
+-r--------  2.0 unx    51532 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/bros/modeling_bros.py
+-r--------  2.0 unx     4223 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/bros/processing_bros.py
 -r--------  2.0 unx      809 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/byt5/__init__.py
 -r--------  2.0 unx    10025 b- defN 24-Mar-25 09:13 mindnlp/transformers/models/byt5/tokenization_byt5.py
 -r--------  2.0 unx     1131 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/chatglm/__init__.py
 -r--------  2.0 unx     4956 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/chatglm/configuration_chatglm.py
 -r--------  2.0 unx    47697 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/chatglm/modeling_chatglm.py
 -r--------  2.0 unx    45162 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/chatglm/modeling_graph_chatglm.py
 -r--------  2.0 unx    17674 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/chatglm/tokenization_chatglm.py
@@ -362,30 +356,38 @@
 -r--------  2.0 unx    21283 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/clip/tokenization_clip.py
 -r--------  2.0 unx     7387 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/clip/tokenization_clip_fast.py
 -r--------  2.0 unx     1239 b- defN 24-Mar-03 07:54 mindnlp/transformers/models/codegen/__init__.py
 -r--------  2.0 unx     7710 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/codegen/configuration_codegen.py
 -r--------  2.0 unx    26987 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/codegen/modeling_codegen.py
 -r--------  2.0 unx    15302 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/codegen/tokenization_codegen.py
 -r--------  2.0 unx    10395 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/codegen/tokenization_codegen_fast.py
--r--------  2.0 unx     1082 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/convbert/__init__.py
--r--------  2.0 unx    47131 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/convbert/convbert.py
--r--------  2.0 unx     3138 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/convbert/convbert_config.py
--r--------  2.0 unx    21854 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/convbert/convbert_tokenizer.py
--r--------  2.0 unx     8790 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/convbert/convbert_tokenizer_fast.py
+-r--------  2.0 unx     1192 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/convbert/__init__.py
+-r--------  2.0 unx    47625 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/convbert/convbert.py
+-r--------  2.0 unx     3138 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/convbert/convbert_config.py
+-r--------  2.0 unx    21854 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/convbert/convbert_tokenizer.py
+-r--------  2.0 unx     8790 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/convbert/convbert_tokenizer_fast.py
+-r--------  2.0 unx    20684 b- defN 24-May-06 12:16 mindnlp/transformers/models/convbert/graph_convbert.py
+-r--------  2.0 unx     1038 b- defN 24-May-06 12:16 mindnlp/transformers/models/convnext/__init__.py
+-r--------  2.0 unx     5622 b- defN 24-May-06 12:16 mindnlp/transformers/models/convnext/configuration_convnext.py
+-r--------  2.0 unx    16342 b- defN 24-May-06 12:16 mindnlp/transformers/models/convnext/image_processing_convnext.py
+-r--------  2.0 unx    19441 b- defN 24-May-06 12:16 mindnlp/transformers/models/convnext/modeling_convnext.py
 -r--------  2.0 unx     1013 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/cpm/__init__.py
 -r--------  2.0 unx    15403 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/cpm/tokenization_cpm.py
 -r--------  2.0 unx    10855 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/cpm/tokenization_cpm_fast.py
 -r--------  2.0 unx     1110 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/cpmant/__init__.py
 -r--------  2.0 unx     5439 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/cpmant/configuration_cpmant.py
 -r--------  2.0 unx    35004 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/cpmant/modeling_cpmant.py
 -r--------  2.0 unx    10166 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/cpmant/tokenization_cpmant.py
 -r--------  2.0 unx     1110 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/cpmbee/__init__.py
 -r--------  2.0 unx     6080 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/cpmbee/configuration_cpmbee.py
 -r--------  2.0 unx    92050 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/cpmbee/modeling_cpmbee.py
 -r--------  2.0 unx    39889 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/cpmbee/tokenization_cpmbee.py
+-r--------  2.0 unx      890 b- defN 24-May-06 12:16 mindnlp/transformers/models/cvt/__init__.py
+-r--------  2.0 unx     6686 b- defN 24-May-06 12:16 mindnlp/transformers/models/cvt/configuration_cvt.py
+-r--------  2.0 unx    26387 b- defN 24-May-06 12:16 mindnlp/transformers/models/cvt/modeling_cvt.py
 -r--------  2.0 unx     1139 b- defN 24-Mar-19 16:41 mindnlp/transformers/models/deberta/__init__.py
 -r--------  2.0 unx     7765 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/deberta/configuration_deberta.py
 -r--------  2.0 unx    50218 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/deberta/modeling_deberta.py
 -r--------  2.0 unx    19193 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/deberta/tokenization_deberta.py
 -r--------  2.0 unx    12810 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/deberta/tokenization_deberta_fast.py
 -r--------  2.0 unx     1168 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/distilbert/__init__.py
 -r--------  2.0 unx     6538 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/distilbert/configuration_distilbert.py
@@ -447,16 +449,16 @@
 -r--------  2.0 unx     2866 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/gpt_bigcode/gpt_bigcode_config.py
 -r--------  2.0 unx     3451 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/gpt_bigcode/gpt_bigcode_tokenizer.py
 -r--------  2.0 unx      893 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/gpt_neo/__init__.py
 -r--------  2.0 unx    31296 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/gpt_neo/gpt_neo.py
 -r--------  2.0 unx     3658 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/gpt_neo/gpt_neo_config.py
 -r--------  2.0 unx      989 b- defN 24-Mar-25 13:55 mindnlp/transformers/models/gpt_neox/__init__.py
 -r--------  2.0 unx     4201 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/gpt_neox/configuration_gpt_neox.py
--r--------  2.0 unx    47248 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/gpt_neox/modeling_gpt_neox.py
--r--------  2.0 unx     6036 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/gpt_neox/tokenization_gpt_neox_fast.py
+-r--------  2.0 unx    47109 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/gpt_neox/modeling_gpt_neox.py
+-r--------  2.0 unx    10401 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/gpt_neox/tokenization_gpt_neox_fast.py
 -r--------  2.0 unx     1035 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/gpt_pangu/__init__.py
 -r--------  2.0 unx     2478 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/gpt_pangu/configuration_gptpangu.py
 -r--------  2.0 unx    22225 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/gpt_pangu/modeling_gptpangu.py
 -r--------  2.0 unx     5069 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/gpt_pangu/tokenization_gptpangu.py
 -r--------  2.0 unx     1105 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/graphormer/__init__.py
 -r--------  2.0 unx     3633 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/graphormer/algos_graphormer.pyx
 -r--------  2.0 unx     7817 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/graphormer/collating_graphormer.py
@@ -469,21 +471,21 @@
 -r--------  2.0 unx     1028 b- defN 24-Mar-29 11:32 mindnlp/transformers/models/internlm/__init__.py
 -r--------  2.0 unx     5010 b- defN 24-Mar-29 11:31 mindnlp/transformers/models/internlm/configuration_internlm.py
 -r--------  2.0 unx    34104 b- defN 24-Mar-29 11:45 mindnlp/transformers/models/internlm/modeling_internlm.py
 -r--------  2.0 unx     9764 b- defN 24-Mar-29 11:30 mindnlp/transformers/models/internlm/tokenization_internlm.py
 -r--------  2.0 unx      900 b- defN 24-Mar-31 10:53 mindnlp/transformers/models/jamba/__init__.py
 -r--------  2.0 unx    11241 b- defN 24-Mar-31 10:53 mindnlp/transformers/models/jamba/configuration_jamba.py
 -r--------  2.0 unx    65061 b- defN 24-Mar-31 10:57 mindnlp/transformers/models/jamba/modeling_jamba.py
--r--------  2.0 unx      907 b- defN 24-Apr-08 11:34 mindnlp/transformers/models/jetmoe/__init__.py
--r--------  2.0 unx     6280 b- defN 24-Apr-08 14:10 mindnlp/transformers/models/jetmoe/configuration_jetmoe.py
--r--------  2.0 unx    42819 b- defN 24-Apr-09 06:51 mindnlp/transformers/models/jetmoe/modeling_jetmoe.py
--r--------  2.0 unx       83 b- defN 24-Apr-09 06:53 mindnlp/transformers/models/jetmoe/utils/__init__.py
--r--------  2.0 unx     4097 b- defN 24-Apr-09 06:50 mindnlp/transformers/models/jetmoe/utils/gate.py
--r--------  2.0 unx     9590 b- defN 24-Apr-09 06:53 mindnlp/transformers/models/jetmoe/utils/moe.py
--r--------  2.0 unx     3474 b- defN 24-Apr-09 06:50 mindnlp/transformers/models/jetmoe/utils/parallel_experts.py
+-r--------  2.0 unx      907 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/jetmoe/__init__.py
+-r--------  2.0 unx     6280 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/jetmoe/configuration_jetmoe.py
+-r--------  2.0 unx    42819 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/jetmoe/modeling_jetmoe.py
+-r--------  2.0 unx       83 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/jetmoe/utils/__init__.py
+-r--------  2.0 unx     4097 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/jetmoe/utils/gate.py
+-r--------  2.0 unx     9590 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/jetmoe/utils/moe.py
+-r--------  2.0 unx     3474 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/jetmoe/utils/parallel_experts.py
 -r--------  2.0 unx      875 b- defN 24-Mar-16 11:41 mindnlp/transformers/models/layoutlm/__init__.py
 -r--------  2.0 unx     2450 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/layoutlm/configuration_layoutlm.py
 -r--------  2.0 unx    54421 b- defN 24-Mar-28 15:43 mindnlp/transformers/models/layoutlm/modeling_layoutlm.py
 -r--------  2.0 unx    22005 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/layoutlm/tokenization_layoutlm.py
 -r--------  2.0 unx     9082 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/layoutlm/tokenization_layoutlm_fast.py
 -r--------  2.0 unx     1365 b- defN 24-Mar-27 18:05 mindnlp/transformers/models/layoutlmv2/__init__.py
 -r--------  2.0 unx    13789 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/layoutlmv2/configuration_layoutlmv2.py
@@ -496,14 +498,23 @@
 -r--------  2.0 unx     1457 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/llama/__init__.py
 -r--------  2.0 unx     9417 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/llama/configuration_llama.py
 -r--------  2.0 unx    37351 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/llama/modeling_llama.py
 -r--------  2.0 unx    23580 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/llama/tokenization_code_llama.py
 -r--------  2.0 unx    19760 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/llama/tokenization_code_llama_fast.py
 -r--------  2.0 unx    22019 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/llama/tokenization_llama.py
 -r--------  2.0 unx    13087 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/llama/tokenization_llama_fast.py
+-r--------  2.0 unx      916 b- defN 24-May-06 12:16 mindnlp/transformers/models/llava/__init__.py
+-r--------  2.0 unx     6068 b- defN 24-May-06 12:16 mindnlp/transformers/models/llava/configuration_llava.py
+-r--------  2.0 unx    22649 b- defN 24-May-06 12:16 mindnlp/transformers/models/llava/modeling_llava.py
+-r--------  2.0 unx     7201 b- defN 24-May-06 12:16 mindnlp/transformers/models/llava/processing_llava.py
+-r--------  2.0 unx     1137 b- defN 24-May-06 12:16 mindnlp/transformers/models/llava_next/__init__.py
+-r--------  2.0 unx     6131 b- defN 24-May-06 12:16 mindnlp/transformers/models/llava_next/configuration_llava_next.py
+-r--------  2.0 unx    29344 b- defN 24-May-06 12:16 mindnlp/transformers/models/llava_next/image_processing_llava_next.py
+-r--------  2.0 unx    29418 b- defN 24-May-06 12:16 mindnlp/transformers/models/llava_next/modeling_llava_next.py
+-r--------  2.0 unx     7269 b- defN 24-May-06 12:16 mindnlp/transformers/models/llava_next/processing_llava_next.py
 -r--------  2.0 unx     1173 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/longformer/__init__.py
 -r--------  2.0 unx     7354 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/longformer/configuration_longformer.py
 -r--------  2.0 unx   107905 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/longformer/modeling_longformer.py
 -r--------  2.0 unx    19034 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/longformer/tokenization_longformer.py
 -r--------  2.0 unx    14789 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/longformer/tokenization_longformer_fast.py
 -r--------  2.0 unx     1012 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/longt5/__init__.py
 -r--------  2.0 unx     7520 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/longt5/configuration_longt5.py
@@ -518,15 +529,15 @@
 -r--------  2.0 unx    20727 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/mamba/modeling_graph_mamba.py
 -r--------  2.0 unx    22627 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/mamba/modeling_mamba.py
 -r--------  2.0 unx      891 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/maskformer/__init__.py
 -r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/maskformer/maskformer.py
 -r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/maskformer/maskformer_config.py
 -r--------  2.0 unx     1109 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/mbart/__init__.py
 -r--------  2.0 unx     3514 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/mbart/configuration_mbart.py
--r--------  2.0 unx    60039 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/mbart/modeling_mbart.py
+-r--------  2.0 unx    59953 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/mbart/modeling_mbart.py
 -r--------  2.0 unx    13994 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/mbart/tokenization_mbart.py
 -r--------  2.0 unx    12171 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/mbart/tokenization_mbart_fast.py
 -r--------  2.0 unx     1044 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/megatron_bert/__init__.py
 -r--------  2.0 unx     6610 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/megatron_bert/configuration_megatron_bert.py
 -r--------  2.0 unx    72730 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/megatron_bert/modeling_megatron_bert.py
 -r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/megatron_gpt2/__init__.py
 -r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/megatron_gpt2/megatron_gpt2.py
@@ -546,14 +557,22 @@
 -r--------  2.0 unx    57813 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/mobilebert/mobilebert.py
 -r--------  2.0 unx     3205 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/mobilebert/mobilebert_config.py
 -r--------  2.0 unx     5687 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/mobilebert/mobilebert_tokenizer.py
 -r--------  2.0 unx      778 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/moss/__init__.py
 -r--------  2.0 unx    32778 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/moss/moss.py
 -r--------  2.0 unx     2838 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/moss/moss_configuration.py
 -r--------  2.0 unx      867 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/moss/moss_tokenization.py
+-r--------  2.0 unx      997 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/mpnet/__init__.py
+-r--------  2.0 unx     2795 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/mpnet/configuration_mpnet.py
+-r--------  2.0 unx    39308 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/mpnet/modeling_mpnet.py
+-r--------  2.0 unx    22784 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/mpnet/tokenization_mpnet.py
+-r--------  2.0 unx     9861 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/mpnet/tokenization_mpnet_fast.py
+-r--------  2.0 unx      886 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/mpt/__init__.py
+-r--------  2.0 unx    12049 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/mpt/configuration_mpt.py
+-r--------  2.0 unx    33852 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/mpt/modeling_mpt.py
 -r--------  2.0 unx      889 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/mt5/__init__.py
 -r--------  2.0 unx     6755 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/mt5/configuration_mt5.py
 -r--------  2.0 unx    81209 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/mt5/modeling_mt5.py
 -r--------  2.0 unx     1025 b- defN 24-Mar-31 12:57 mindnlp/transformers/models/musicgen/__init__.py
 -r--------  2.0 unx    10700 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/musicgen/configuration_musicgen.py
 -r--------  2.0 unx   110242 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/musicgen/modeling_musicgen.py
 -r--------  2.0 unx     5684 b- defN 24-Mar-26 12:58 mindnlp/transformers/models/musicgen/processing_musicgen.py
@@ -562,23 +581,34 @@
 -r--------  2.0 unx    15630 b- defN 24-Mar-31 16:52 mindnlp/transformers/models/musicgen_melody/feature_extraction_musicgen_melody.py
 -r--------  2.0 unx   106734 b- defN 24-Mar-31 16:52 mindnlp/transformers/models/musicgen_melody/modeling_musicgen_melody.py
 -r--------  2.0 unx     8653 b- defN 24-Mar-31 16:52 mindnlp/transformers/models/musicgen_melody/processing_musicgen_melody.py
 -r--------  2.0 unx      945 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/nezha/__init__.py
 -r--------  2.0 unx    47907 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/nezha/nezha.py
 -r--------  2.0 unx     2431 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/nezha/nezha_config.py
 -r--------  2.0 unx     2953 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/nezha/nezha_tokenizer.py
+-r--------  2.0 unx      897 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/olmo/__init__.py
+-r--------  2.0 unx     8938 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/olmo/configuration_olmo.py
+-r--------  2.0 unx    39292 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/olmo/modeling_olmo.py
+-r--------  2.0 unx      915 b- defN 24-May-06 12:16 mindnlp/transformers/models/openelm/__init__.py
+-r--------  2.0 unx    12715 b- defN 24-May-06 12:16 mindnlp/transformers/models/openelm/configuration_openelm.py
+-r--------  2.0 unx    35961 b- defN 24-May-06 12:16 mindnlp/transformers/models/openelm/modeling_openelm.py
 -r--------  2.0 unx      891 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/opt/__init__.py
 -r--------  2.0 unx     7373 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/opt/configuration_opt.py
--r--------  2.0 unx    47645 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/opt/modeling_opt.py
--r--------  2.0 unx      943 b- defN 24-Mar-28 03:04 mindnlp/transformers/models/pegasus/__init__.py
--r--------  2.0 unx    13184 b- defN 24-Mar-28 06:06 mindnlp/transformers/models/pegasus/tokenization_pegasus.py
--r--------  2.0 unx     9982 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/pegasus/tokenization_pegasus_fast.py
+-r--------  2.0 unx    47645 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/opt/modeling_opt.py
+-r--------  2.0 unx     1140 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/pegasus/__init__.py
+-r--------  2.0 unx     7830 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/pegasus/configuration_pegasus.py
+-r--------  2.0 unx    71916 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/pegasus/modeling_pegasus.py
+-r--------  2.0 unx    13230 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/pegasus/tokenization_pegasus.py
+-r--------  2.0 unx    10028 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/pegasus/tokenization_pegasus_fast.py
 -r--------  2.0 unx      892 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/phi/__init__.py
 -r--------  2.0 unx     9266 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/phi/configuration_phi.py
--r--------  2.0 unx    42961 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/phi/modeling_phi.py
+-r--------  2.0 unx    42961 b- defN 24-May-06 12:33 mindnlp/transformers/models/phi/modeling_phi.py
+-r--------  2.0 unx      898 b- defN 24-May-06 12:32 mindnlp/transformers/models/phi3/__init__.py
+-r--------  2.0 unx    10417 b- defN 24-May-06 12:19 mindnlp/transformers/models/phi3/configuration_phi3.py
+-r--------  2.0 unx    44874 b- defN 24-May-06 13:07 mindnlp/transformers/models/phi3/modeling_phi3.py
 -r--------  2.0 unx      600 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/pop2piano/__init__.py
 -r--------  2.0 unx     6241 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/pop2piano/configuration_pop2piano.py
 -r--------  2.0 unx    20121 b- defN 24-Mar-28 06:07 mindnlp/transformers/models/pop2piano/feature_extraction_pop2piano.py
 -r--------  2.0 unx    60570 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/pop2piano/modeling_pop2piano.py
 -r--------  2.0 unx     5589 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/pop2piano/processing_pop2piano.py
 -r--------  2.0 unx    32281 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/pop2piano/tokenization_pop2piano.py
 -r--------  2.0 unx     1108 b- defN 24-Mar-04 00:35 mindnlp/transformers/models/qwen2/__init__.py
@@ -591,52 +621,73 @@
 -r--------  2.0 unx    45282 b- defN 24-Mar-29 13:12 mindnlp/transformers/models/qwen2_moe/modeling_qwen2_moe.py
 -r--------  2.0 unx     1148 b- defN 24-Mar-19 16:41 mindnlp/transformers/models/reformer/__init__.py
 -r--------  2.0 unx    13575 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/reformer/configuration_reformer.py
 -r--------  2.0 unx   107482 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/reformer/modeling_reformer.py
 -r--------  2.0 unx     7289 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/reformer/tokenization_reformer.py
 -r--------  2.0 unx     5004 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/reformer/tokenization_reformer_fast.py
 -r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/regnet/__init__.py
+-r--------  2.0 unx      905 b- defN 24-May-06 12:16 mindnlp/transformers/models/resnet/__init__.py
+-r--------  2.0 unx     5515 b- defN 24-May-06 12:16 mindnlp/transformers/models/resnet/configuration_resnet.py
+-r--------  2.0 unx    16938 b- defN 24-May-06 12:16 mindnlp/transformers/models/resnet/modeling_resnet.py
 -r--------  2.0 unx     1133 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/roberta/__init__.py
 -r--------  2.0 unx     2420 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/roberta/configuration_roberta.py
 -r--------  2.0 unx    12078 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/roberta/modeling_graph_roberta.py
 -r--------  2.0 unx    60971 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/roberta/modeling_roberta.py
 -r--------  2.0 unx    18177 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/roberta/tokenization_roberta.py
 -r--------  2.0 unx    13885 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/roberta/tokenization_roberta_fast.py
 -r--------  2.0 unx      995 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/rwkv/__init__.py
 -r--------  2.0 unx     6303 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/rwkv/configuration_rwkv.py
 -r--------  2.0 unx    28881 b- defN 24-Mar-29 07:53 mindnlp/transformers/models/rwkv/modeling_rwkv.py
+-r--------  2.0 unx     1078 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/sam/__init__.py
+-r--------  2.0 unx    13877 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/sam/configuration_sam.py
+-r--------  2.0 unx    57684 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/sam/image_processing_sam.py
+-r--------  2.0 unx    58327 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/sam/modeling_sam.py
+-r--------  2.0 unx    10115 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/sam/processing_sam.py
 -r--------  2.0 unx     1459 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/seamless_m4t/__init__.py
 -r--------  2.0 unx    23758 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/seamless_m4t/configuration_seamless_m4t.py
 -r--------  2.0 unx    13061 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/seamless_m4t/feature_extraction_seamless_m4t.py
 -r--------  2.0 unx   189385 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/seamless_m4t/modeling_seamless_m4t.py
 -r--------  2.0 unx     5891 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/seamless_m4t/processing_seamless_m4t.py
 -r--------  2.0 unx    25979 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/seamless_m4t/tokenization_seamless_m4t.py
 -r--------  2.0 unx    20489 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/seamless_m4t/tokenization_seamless_m4t_fast.py
 -r--------  2.0 unx      974 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/seamless_m4t_v2/__init__.py
 -r--------  2.0 unx    24474 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/seamless_m4t_v2/configuration_seamless_m4t_v2.py
--r--------  2.0 unx   211331 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/seamless_m4t_v2/modeling_seamless_m4t_v2.py
+-r--------  2.0 unx   211331 b- defN 24-May-06 13:23 mindnlp/transformers/models/seamless_m4t_v2/modeling_seamless_m4t_v2.py
+-r--------  2.0 unx     1053 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/segformer/__init__.py
+-r--------  2.0 unx     6793 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/segformer/configuration_segformer.py
+-r--------  2.0 unx    23450 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/segformer/image_processing_segformer.py
+-r--------  2.0 unx    32442 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/segformer/modeling_segformer.py
 -r--------  2.0 unx      934 b- defN 24-Mar-09 17:05 mindnlp/transformers/models/starcoder2/__init__.py
 -r--------  2.0 unx     6919 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/starcoder2/configuration_starcoder2.py
 -r--------  2.0 unx    36584 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/starcoder2/modeling_starcoder2.py
 -r--------  2.0 unx     1171 b- defN 24-Mar-24 20:22 mindnlp/transformers/models/t5/__init__.py
 -r--------  2.0 unx     4419 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/t5/chatyuan_tokenizer.py
 -r--------  2.0 unx     6772 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/t5/configuration_t5.py
 -r--------  2.0 unx    70759 b- defN 24-Mar-31 10:53 mindnlp/transformers/models/t5/modeling_t5.py
 -r--------  2.0 unx    20403 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/t5/tokenization_t5.py
 -r--------  2.0 unx    10806 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/t5/tokenization_t5_fast.py
 -r--------  2.0 unx      694 b- defN 24-Mar-31 10:53 mindnlp/transformers/models/table_transformer/__init__.py
--r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/timesformer/__init__.py
+-r--------  2.0 unx     1061 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/timesformer/__init__.py
+-r--------  2.0 unx     5818 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/timesformer/configuration_timesformer.py
+-r--------  2.0 unx    17146 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/timesformer/image_processing_videomae.py
+-r--------  2.0 unx    33020 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/timesformer/modeling_timesformer.py
 -r--------  2.0 unx      879 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/tinybert/__init__.py
 -r--------  2.0 unx    25866 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/tinybert/tinybert.py
 -r--------  2.0 unx     3520 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/tinybert/tinybert_config.py
 -r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/transformer/__init__.py
 -r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/transformer/transformer.py
 -r--------  2.0 unx        0 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/transformer/transformer_config.py
+-r--------  2.0 unx        0 b- defN 24-May-06 12:16 mindnlp/transformers/models/van/__init__.py
+-r--------  2.0 unx     4682 b- defN 24-May-06 12:16 mindnlp/transformers/models/van/configuration_van.py
+-r--------  2.0 unx    18894 b- defN 24-May-06 12:16 mindnlp/transformers/models/van/modeling_van.py
+-r--------  2.0 unx      895 b- defN 24-May-06 12:16 mindnlp/transformers/models/vipllava/__init__.py
+-r--------  2.0 unx     5740 b- defN 24-May-06 12:16 mindnlp/transformers/models/vipllava/configuration_vipllava.py
+-r--------  2.0 unx    29912 b- defN 24-May-06 12:16 mindnlp/transformers/models/vipllava/modeling_vipllava.py
 -r--------  2.0 unx     1598 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/wav2vec2/__init__.py
--r--------  2.0 unx    20372 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/wav2vec2/configuration_wav2vec2.py
+-r--------  2.0 unx    20370 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/wav2vec2/configuration_wav2vec2.py
 -r--------  2.0 unx    11553 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/wav2vec2/feature_extraction_wav2vec2.py
 -r--------  2.0 unx    97015 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/wav2vec2/modeling_wav2vec2.py
 -r--------  2.0 unx     7177 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/wav2vec2/processing_wav2vec2.py
 -r--------  2.0 unx    36485 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/wav2vec2/tokenization_wav2vec2.py
 -r--------  2.0 unx      860 b- defN 24-Mar-19 16:41 mindnlp/transformers/models/wav2vec2_with_lm/__init__.py
 -r--------  2.0 unx    29591 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/wav2vec2_with_lm/processing_wav2vec2_with_lm.py
 -r--------  2.0 unx     1356 b- defN 24-Mar-20 16:25 mindnlp/transformers/models/whisper/__init__.py
@@ -650,355 +701,338 @@
 -r--------  2.0 unx    32375 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/whisper/tokenization_whisper_fast.py
 -r--------  2.0 unx      983 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/xlm/__init__.py
 -r--------  2.0 unx    11328 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/xlm/configuration_xlm.py
 -r--------  2.0 unx    46629 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/xlm/modeling_xlm.py
 -r--------  2.0 unx    34991 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/xlm/tokenization_xlm.py
 -r--------  2.0 unx     1192 b- defN 24-Feb-29 06:56 mindnlp/transformers/models/xlm_roberta/__init__.py
 -r--------  2.0 unx     6980 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/xlm_roberta/configuration_xlm_roberta.py
--r--------  2.0 unx    63314 b- defN 24-Mar-25 11:12 mindnlp/transformers/models/xlm_roberta/modeling_xlm_roberta.py
+-r--------  2.0 unx    62507 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/xlm_roberta/modeling_xlm_roberta.py
 -r--------  2.0 unx    14289 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/xlm_roberta/tokenization_xlm_roberta.py
 -r--------  2.0 unx    10433 b- defN 24-Mar-28 15:57 mindnlp/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py
--r--------  2.0 unx     1109 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/xlnet/__init__.py
--r--------  2.0 unx     4735 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/xlnet/configuration_xlnet.py
--r--------  2.0 unx    85973 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/xlnet/modeling_xlnet.py
--r--------  2.0 unx    16395 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/xlnet/tokenization_xlnet.py
--r--------  2.0 unx    10222 b- defN 24-Apr-08 06:51 mindnlp/transformers/models/xlnet/tokenization_xlnet_fast.py
+-r--------  2.0 unx     1109 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/xlnet/__init__.py
+-r--------  2.0 unx     4735 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/xlnet/configuration_xlnet.py
+-r--------  2.0 unx    79968 b- defN 24-Apr-23 14:20 mindnlp/transformers/models/xlnet/modeling_xlnet.py
+-r--------  2.0 unx    16395 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/xlnet/tokenization_xlnet.py
+-r--------  2.0 unx    10222 b- defN 24-Apr-08 03:51 mindnlp/transformers/models/xlnet/tokenization_xlnet_fast.py
 -r--------  2.0 unx    26016 b- defN 24-Mar-28 00:49 mindnlp/transformers/pipelines/__init__.py
 -r--------  2.0 unx     9793 b- defN 24-Mar-25 11:56 mindnlp/transformers/pipelines/audio_utils.py
 -r--------  2.0 unx    37518 b- defN 24-Mar-28 15:57 mindnlp/transformers/pipelines/automatic_speech_recognition.py
 -r--------  2.0 unx    35984 b- defN 24-Mar-25 11:55 mindnlp/transformers/pipelines/base.py
 -r--------  2.0 unx    27144 b- defN 24-Mar-28 15:57 mindnlp/transformers/pipelines/document_question_answering.py
 -r--------  2.0 unx    28511 b- defN 24-Mar-28 15:57 mindnlp/transformers/pipelines/question_answering.py
 -r--------  2.0 unx    17651 b- defN 24-Mar-28 15:57 mindnlp/transformers/pipelines/text2text_generation.py
 -r--------  2.0 unx     9640 b- defN 24-Mar-28 15:57 mindnlp/transformers/pipelines/text_classification.py
 -r--------  2.0 unx    15366 b- defN 24-Mar-28 15:57 mindnlp/transformers/pipelines/text_generation.py
 -r--------  2.0 unx    13013 b- defN 24-Mar-28 15:57 mindnlp/transformers/pipelines/zero_shot_classification.py
+-r--------  2.0 unx      717 b- defN 24-Apr-23 14:20 mindnlp/trl/__init__.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/trl/core.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/trl/environment/__init__.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/trl/extras/__init__.py
+-r--------  2.0 unx        0 b- defN 24-Apr-23 14:20 mindnlp/trl/models/__init__.py
 -r--------  2.0 unx     1510 b- defN 24-Mar-25 13:50 mindnlp/utils/__init__.py
--r--------  2.0 unx    16335 b- defN 24-Mar-25 11:49 mindnlp/utils/backbone_utils.py
 -r--------  2.0 unx     1458 b- defN 24-Feb-29 06:56 mindnlp/utils/compatibility.py
 -r--------  2.0 unx     2916 b- defN 23-Mar-22 09:42 mindnlp/utils/decompress.py
--r--------  2.0 unx    32202 b- defN 24-Mar-28 15:57 mindnlp/utils/download.py
+-r--------  2.0 unx    33061 b- defN 24-May-06 12:16 mindnlp/utils/download.py
 -r--------  2.0 unx    12029 b- defN 24-Mar-28 15:57 mindnlp/utils/errors.py
--r--------  2.0 unx    11747 b- defN 24-Mar-25 11:12 mindnlp/utils/generic.py
+-r--------  2.0 unx    12652 b- defN 24-Apr-23 14:20 mindnlp/utils/generic.py
 -r--------  2.0 unx    14008 b- defN 24-Mar-27 18:05 mindnlp/utils/import_utils.py
--r--------  2.0 unx    11478 b- defN 24-Mar-25 12:05 mindnlp/utils/logging.py
+-r--------  2.0 unx    11589 b- defN 24-Apr-23 14:20 mindnlp/utils/logging.py
 -r--------  2.0 unx     4451 b- defN 24-Mar-28 15:57 mindnlp/utils/peft_utils.py
 -r--------  2.0 unx     1898 b- defN 24-Mar-25 11:12 mindnlp/utils/save.py
--r--------  2.0 unx    21582 b- defN 24-Apr-02 03:19 mindnlp/utils/serialization.py
--r--------  2.0 unx    50268 b- defN 24-Mar-30 01:45 mindnlp/utils/testing_utils.py
+-r--------  2.0 unx    21980 b- defN 24-Apr-23 14:20 mindnlp/utils/serialization.py
+-r--------  2.0 unx    51172 b- defN 24-Apr-23 14:20 mindnlp/utils/testing_utils.py
 -r--------  2.0 unx      712 b- defN 23-Mar-22 09:42 mindnlp/vocab/__init__.py
 -r--------  2.0 unx    11522 b- defN 24-Apr-01 15:34 mindnlp/vocab/vocab.py
 -r--------  2.0 unx      768 b- defN 23-Mar-22 09:42 mindnlp/workflow/__init__.py
 -r--------  2.0 unx     5813 b- defN 23-Jul-15 13:56 mindnlp/workflow/utils.py
 -r--------  2.0 unx     7577 b- defN 24-Mar-25 11:12 mindnlp/workflow/work.py
 -r--------  2.0 unx     7103 b- defN 23-Jul-15 13:56 mindnlp/workflow/workflow.py
 -r--------  2.0 unx      757 b- defN 23-Mar-22 09:42 mindnlp/workflow/downstream/__init__.py
 -r--------  2.0 unx     1557 b- defN 24-Mar-25 11:12 mindnlp/workflow/downstream/sentiment_analysis_model.py
 -r--------  2.0 unx      780 b- defN 23-Jul-15 13:56 mindnlp/workflow/works/__init__.py
 -r--------  2.0 unx        0 b- defN 23-Mar-22 09:42 mindnlp/workflow/works/classification.py
 -r--------  2.0 unx    26028 b- defN 24-Mar-25 11:12 mindnlp/workflow/works/information_extraction.py
 -r--------  2.0 unx        0 b- defN 23-Mar-22 09:42 mindnlp/workflow/works/ner.py
 -r--------  2.0 unx        0 b- defN 23-Mar-22 09:42 mindnlp/workflow/works/qa.py
 -r--------  2.0 unx     6032 b- defN 24-Feb-29 06:56 mindnlp/workflow/works/sentiment_analysis.py
--rw-r--r--  2.0 unx       65 b- defN 23-Mar-22 09:42 tests/README.md
--rw-r--r--  2.0 unx      708 b- defN 23-Mar-22 09:42 tests/__init__.py
--rw-r--r--  2.0 unx      147 b- defN 24-Feb-29 06:56 tests/common.py
--rw-r--r--  2.0 unx      129 b- defN 23-Jul-15 13:56 tests/pytest.ini
--rw-r--r--  2.0 unx      504 b- defN 24-Feb-29 06:56 tests/fixtures/add_distilbert_like_config.json
--rw-r--r--  2.0 unx       29 b- defN 24-Feb-29 06:56 tests/fixtures/dummy-config.json
--rw-r--r--  2.0 unx      101 b- defN 24-Feb-29 06:56 tests/fixtures/dummy_feature_extractor_config.json
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/fixtures/empty.txt
--rw-r--r--  2.0 unx       52 b- defN 24-Feb-29 06:56 tests/fixtures/input.txt
--rw-r--r--  2.0 unx       36 b- defN 24-Feb-29 06:56 tests/fixtures/merges.txt
--rw-r--r--  2.0 unx      100 b- defN 24-Feb-29 06:56 tests/fixtures/preprocessor_config.json
--rw-r--r--  2.0 unx     4394 b- defN 24-Feb-29 06:56 tests/fixtures/sample_text.txt
--rw-r--r--  2.0 unx     4284 b- defN 24-Feb-29 06:56 tests/fixtures/sample_text_no_unicode.txt
--rw-r--r--  2.0 unx   760289 b- defN 24-Feb-29 06:56 tests/fixtures/spiece.model
--rw-r--r--  2.0 unx       76 b- defN 24-Feb-29 06:56 tests/fixtures/test_entity_vocab.json
--rw-r--r--  2.0 unx   253154 b- defN 24-Feb-29 06:56 tests/fixtures/test_sentencepiece.model
--rw-r--r--  2.0 unx   251527 b- defN 24-Feb-29 06:56 tests/fixtures/test_sentencepiece_bpe.model
--rw-r--r--  2.0 unx   238473 b- defN 24-Feb-29 06:56 tests/fixtures/test_sentencepiece_bpe_char.model
--rw-r--r--  2.0 unx   253134 b- defN 24-Feb-29 06:56 tests/fixtures/test_sentencepiece_no_bos.model
--rw-r--r--  2.0 unx   270096 b- defN 24-Feb-29 06:56 tests/fixtures/test_sentencepiece_with_bytefallback.model
--rw-r--r--  2.0 unx      228 b- defN 24-Feb-29 06:56 tests/fixtures/vocab.json
--rw-r--r--  2.0 unx       85 b- defN 24-Feb-29 06:56 tests/fixtures/vocab.txt
--rw-r--r--  2.0 unx       52 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/.gitignore
--rw-r--r--  2.0 unx   694498 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/COCO/000000039769.png
--rw-r--r--  2.0 unx     4075 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/COCO/coco_annotations.txt
--rw-r--r--  2.0 unx      555 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/COCO/coco_panoptic_annotations.txt
--rw-r--r--  2.0 unx     8269 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/COCO/coco_panoptic/000000039769.png
--rw-r--r--  2.0 unx     1718 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/GermEval/dev.txt
--rw-r--r--  2.0 unx      218 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/GermEval/labels.txt
--rw-r--r--  2.0 unx     1779 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/GermEval/train.txt
--rw-r--r--  2.0 unx     1354 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/MRPC/dev.csv
--rw-r--r--  2.0 unx     1386 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/MRPC/dev.tsv
--rw-r--r--  2.0 unx     1354 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/MRPC/train.csv
--rw-r--r--  2.0 unx     1386 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/MRPC/train.tsv
--rw-r--r--  2.0 unx    17233 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/SQUAD/sample.json
--rw-r--r--  2.0 unx     1126 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/STS-B/dev.tsv
--rw-r--r--  2.0 unx     1121 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/STS-B/train.tsv
--rw-r--r--  2.0 unx     3001 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/conll/sample.json
--rw-r--r--  2.0 unx     3522 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/swag/sample.json
--rw-r--r--  2.0 unx    79924 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/wiki_text/wiki_00
--rw-r--r--  2.0 unx     1423 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/wmt16/sample.json
--rw-r--r--  2.0 unx    27417 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/wmt_en_ro/test.json
--rw-r--r--  2.0 unx    11234 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/wmt_en_ro/train.json
--rw-r--r--  2.0 unx    21699 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/wmt_en_ro/val.json
--rw-r--r--  2.0 unx    15601 b- defN 24-Mar-25 11:12 tests/fixtures/tests_samples/xsum/sample.json
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/st/__init__.py
--rw-r--r--  2.0 unx     2834 b- defN 23-Jun-01 14:35 tests/st/test_bilstm_imdb.py
--rw-r--r--  2.0 unx     2110 b- defN 24-Feb-29 06:56 tests/st/test_longformer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/test_module/__init__.py
--rw-r--r--  2.0 unx      387 b- defN 24-Feb-29 06:56 tests/test_module/custom_configuration.py
--rw-r--r--  2.0 unx      777 b- defN 24-Feb-29 06:56 tests/test_module/custom_modeling.py
--rw-r--r--  2.0 unx     1117 b- defN 24-Feb-29 06:56 tests/test_module/custom_pipeline.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/dataset/__init__.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Feb-29 06:56 tests/ut/dataset/test_imdb.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/dataset/transforms/__init__.py
--rw-r--r--  2.0 unx     2555 b- defN 24-Feb-29 06:56 tests/ut/dataset/transforms/test_add_token.py
--rw-r--r--  2.0 unx     1235 b- defN 24-Feb-29 06:56 tests/ut/dataset/transforms/test_lookup.py
--rw-r--r--  2.0 unx     2560 b- defN 24-Feb-29 06:56 tests/ut/dataset/transforms/test_pad_transform.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/engine/__init__.py
--rw-r--r--  2.0 unx     2248 b- defN 24-Mar-20 16:25 tests/ut/engine/test_callback.py
--rw-r--r--  2.0 unx     2352 b- defN 24-Mar-20 16:25 tests/ut/engine/test_evaluator.py
--rw-r--r--  2.0 unx     6878 b- defN 24-Mar-20 16:25 tests/ut/engine/test_trainer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/legacy/__init__.py
--rw-r--r--  2.0 unx      845 b- defN 24-Feb-29 06:56 tests/ut/legacy/test_einsum.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/metrics/__init__.py
--rw-r--r--  2.0 unx    32965 b- defN 23-Jul-15 13:56 tests/ut/metrics/test_metrics_class.py
--rw-r--r--  2.0 unx    19939 b- defN 23-Mar-22 09:42 tests/ut/metrics/test_metrics_fn.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/__init__.py
--rw-r--r--  2.0 unx    13357 b- defN 24-Feb-29 06:56 tests/ut/modules/test_crf.py
--rw-r--r--  2.0 unx     5675 b- defN 24-Feb-29 06:56 tests/ut/modules/test_decoder.py
--rw-r--r--  2.0 unx     4267 b- defN 24-Feb-29 06:56 tests/ut/modules/test_encoder.py
--rw-r--r--  2.0 unx     1422 b- defN 23-Nov-13 07:20 tests/ut/modules/test_fasttext_embedding.py
--rw-r--r--  2.0 unx     3216 b- defN 24-Mar-30 02:03 tests/ut/modules/test_flashattention.py
--rw-r--r--  2.0 unx     1356 b- defN 24-Feb-29 06:56 tests/ut/modules/test_glove_embedding.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/attentions/__init__.py
--rw-r--r--  2.0 unx     1809 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_additive_attention.py
--rw-r--r--  2.0 unx     1784 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_binary_attention.py
--rw-r--r--  2.0 unx     1779 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_cosine_attention.py
--rw-r--r--  2.0 unx     1831 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_linear_attention.py
--rw-r--r--  2.0 unx     1540 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_scaled_dot_attention.py
--rw-r--r--  2.0 unx     2276 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_self_attention.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 14:35 tests/ut/modules/generation/__init__.py
--rw-r--r--  2.0 unx     1784 b- defN 24-Feb-29 06:56 tests/ut/modules/generation/test_generation_config.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/loss/__init__.py
--rw-r--r--  2.0 unx     2296 b- defN 24-Feb-29 06:56 tests/ut/modules/loss/test_cmrc2018loss.py
--rw-r--r--  2.0 unx     2385 b- defN 24-Feb-29 06:56 tests/ut/modules/loss/test_rdrop_loss.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/rnns/__init__.py
--rw-r--r--  2.0 unx     4872 b- defN 24-Feb-29 06:56 tests/ut/modules/rnns/test_gru.py
--rw-r--r--  2.0 unx     5180 b- defN 24-Feb-29 06:56 tests/ut/modules/rnns/test_lstm.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/transformer/__init__.py
--rw-r--r--  2.0 unx     3775 b- defN 24-Feb-29 06:56 tests/ut/modules/transformer/test_multi_head_attention.py
--rw-r--r--  2.0 unx     2187 b- defN 24-Feb-29 06:56 tests/ut/modules/transformer/test_transformer_encoder.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Feb-29 06:56 tests/ut/modules/transformer/test_transformer_encoder_layer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-16 07:16 tests/ut/peft/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-16 07:16 tests/ut/peft/test_config.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 15:36 tests/ut/text2vec/__init__.py
--rw-r--r--  2.0 unx     2756 b- defN 24-Apr-01 15:36 tests/ut/text2vec/test_sbert_embeddings.py
--rw-r--r--  2.0 unx     2078 b- defN 24-Apr-01 15:36 tests/ut/text2vec/test_w2v_embeddings.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/__init__.py
--rw-r--r--  2.0 unx    10140 b- defN 24-Mar-25 11:12 tests/ut/transformers/test_backbone_common.py
--rw-r--r--  2.0 unx     8097 b- defN 24-Feb-29 06:56 tests/ut/transformers/test_configuration_common.py
--rw-r--r--  2.0 unx     2231 b- defN 24-Mar-31 16:52 tests/ut/transformers/test_feature_extraction_common.py
--rw-r--r--  2.0 unx    73183 b- defN 24-Mar-31 10:53 tests/ut/transformers/test_modeling_common.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-25 11:12 tests/ut/transformers/test_pipeline_mixin.py
--rw-r--r--  2.0 unx    16663 b- defN 24-Mar-31 16:52 tests/ut/transformers/test_sequence_feature_extraction_common.py
--rw-r--r--  2.0 unx   206613 b- defN 24-Feb-29 06:56 tests/ut/transformers/test_tokenization_common.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/generation/__init__.py
--rw-r--r--  2.0 unx    28522 b- defN 24-Feb-29 06:56 tests/ut/transformers/generation/test_framework_agnostic.py
--rw-r--r--  2.0 unx   123394 b- defN 24-Mar-14 17:04 tests/ut/transformers/generation/test_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/albert/__init__.py
--rw-r--r--  2.0 unx    14176 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/albert/test_modeling_albert.py
--rw-r--r--  2.0 unx     8039 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/albert/test_tokenization_albert.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/align/__init__.py
--rw-r--r--  2.0 unx    21247 b- defN 24-Mar-27 18:05 tests/ut/transformers/models/align/test_modeling_align.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/altclip/__init__.py
--rw-r--r--  2.0 unx    20018 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/altclip/test_modeling_altclip.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/audio_spectrogram_transformer/__init__.py
--rw-r--r--  2.0 unx     9381 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/audio_spectrogram_transformer/test_modeling_audio_spectrogram_transformer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/auto/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/auto/test_configuration_auto.py
--rw-r--r--  2.0 unx    15231 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/auto/test_modeling_auto.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/autoformer/__init__.py
--rw-r--r--  2.0 unx    19293 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/autoformer/test_modeling_autoformer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/baichuan/__init__.py
--rw-r--r--  2.0 unx     2793 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/baichuan/test_modeling_baichuan.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bark/__init__.py
--rw-r--r--  2.0 unx    44187 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/bark/test_modeling_bark.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bart/__init__.py
--rw-r--r--  2.0 unx    95343 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/bart/test_modeling_bart.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-25 11:12 tests/ut/transformers/models/beit/__init__.py
--rw-r--r--  2.0 unx    19837 b- defN 24-Mar-25 11:12 tests/ut/transformers/models/beit/test_modeling_beit.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bert/__init__.py
--rw-r--r--  2.0 unx    25734 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/bert/test_modeling_bert.py
--rw-r--r--  2.0 unx     2048 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bert/test_modeling_graph_bert.py
--rw-r--r--  2.0 unx    14288 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/bert/test_tokenization_bert.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-25 13:50 tests/ut/transformers/models/bert_generation/__init__.py
--rw-r--r--  2.0 unx    12696 b- defN 24-Mar-25 13:50 tests/ut/transformers/models/bert_generation/test_modeling_bert_generation.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-09 17:05 tests/ut/transformers/models/big_bird/__init__.py
--rw-r--r--  2.0 unx    46579 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/big_bird/test_modeling_big_bird.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-28 03:06 tests/ut/transformers/models/bigbird_pegasus/__init__.py
--rw-r--r--  2.0 unx   110760 b- defN 24-Mar-28 06:03 tests/ut/transformers/models/bigbird_pegasus/test_modeling_bigbird_pegasus.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/biogpt/__init__.py
--rw-r--r--  2.0 unx    19717 b- defN 24-Mar-19 16:44 tests/ut/transformers/models/biogpt/test_modeling_biogpt.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-31 12:05 tests/ut/transformers/models/bit/__init__.py
--rw-r--r--  2.0 unx    11755 b- defN 24-Mar-31 12:35 tests/ut/transformers/models/bit/test_modeling_bit.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 03:19 tests/ut/transformers/models/blenderbot/__init__.py
--rw-r--r--  2.0 unx    22474 b- defN 24-Apr-02 03:19 tests/ut/transformers/models/blenderbot/test_modeling_blenderbot.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 08:27 tests/ut/transformers/models/blenderbot_small/__init__.py
--rw-r--r--  2.0 unx    22787 b- defN 24-Apr-08 06:51 tests/ut/transformers/models/blenderbot_small/test_modeling_blenderbot_small.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 15:06 tests/ut/transformers/models/blip/__init__.py
--rw-r--r--  2.0 unx    42838 b- defN 24-Apr-02 15:06 tests/ut/transformers/models/blip/test_modeling_blip.py
--rw-r--r--  2.0 unx     6896 b- defN 24-Apr-02 15:06 tests/ut/transformers/models/blip/test_modeling_blip_text.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-08 06:51 tests/ut/transformers/models/blip_2/__init__.py
--rw-r--r--  2.0 unx    39138 b- defN 24-Apr-08 06:51 tests/ut/transformers/models/blip_2/test_modeling_blip_2.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bloom/__init__.py
--rw-r--r--  2.0 unx    35152 b- defN 24-Mar-28 15:57 tests/ut/transformers/models/bloom/test_modeling_bloom.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-08 07:55 tests/ut/transformers/models/bridgetower/__init__.py
--rw-r--r--  2.0 unx    23014 b- defN 24-Apr-08 08:29 tests/ut/transformers/models/bridgetower/test_modeling_bridgetower.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-08 08:41 tests/ut/transformers/models/bros/__init__.py
--rw-r--r--  2.0 unx    16094 b- defN 24-Apr-08 09:16 tests/ut/transformers/models/bros/test_modeling_bros.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/chatglm/__init__.py
--rw-r--r--  2.0 unx    13895 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/chatglm/test_modeling_chatglm.py
--rw-r--r--  2.0 unx    13970 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/chatglm/test_modeling_graph_chatglm.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/clip/__init__.py
--rw-r--r--  2.0 unx    25666 b- defN 24-Mar-03 07:54 tests/ut/transformers/models/clip/test_modeling_clip.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/codegen/__init__.py
--rw-r--r--  2.0 unx    23368 b- defN 24-Mar-03 07:54 tests/ut/transformers/models/codegen/test_modeling_codegen.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-08 06:51 tests/ut/transformers/models/convbert/__init__.py
--rw-r--r--  2.0 unx    19793 b- defN 24-Apr-08 06:51 tests/ut/transformers/models/convbert/test_modeling_convbert.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/cpmant/__init__.py
--rw-r--r--  2.0 unx     9906 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/cpmant/test_modeling_cpmant.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/cpmbee/__init__.py
--rw-r--r--  2.0 unx     8443 b- defN 24-Mar-18 02:46 tests/ut/transformers/models/cpmbee/test_modeling_cpmbee.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/deberta/__init__.py
--rw-r--r--  2.0 unx    12019 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/deberta/test_modeling_deberta.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/encodec/__init__.py
--rw-r--r--  2.0 unx    20901 b- defN 24-Mar-27 05:46 tests/ut/transformers/models/encodec/test_modeling_encodec.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/ernie/__init__.py
--rw-r--r--  2.0 unx    22370 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/ernie/test_modeling_ernie.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/ernie_m/__init__.py
--rw-r--r--  2.0 unx    12542 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/ernie_m/test_modeling_ernie_m.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-03 07:54 tests/ut/transformers/models/esm/__init__.py
--rw-r--r--  2.0 unx    13068 b- defN 24-Mar-03 07:54 tests/ut/transformers/models/esm/test_modeling_esm.py
--rw-r--r--  2.0 unx    10139 b- defN 24-Mar-04 00:35 tests/ut/transformers/models/esm/test_modeling_esmfold.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/falcon/__init__.py
--rw-r--r--  2.0 unx    22507 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/falcon/test_modeling_falcon.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gemma/__init__.py
--rw-r--r--  2.0 unx    22221 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gemma/test_modeling_gemma.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt/__init__.py
--rw-r--r--  2.0 unx    11432 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt/test_modeling_gpt.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt2/__init__.py
--rw-r--r--  2.0 unx    36548 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt2/test_modeling_gpt2.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt_bigcode/__init__.py
--rw-r--r--  2.0 unx    25963 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt_bigcode/test_modeling_gpt_bigcode.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt_neo/__init__.py
--rw-r--r--  2.0 unx     4504 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt_neo/test_gpt_neo.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-25 13:55 tests/ut/transformers/models/gpt_neox/__init__.py
--rw-r--r--  2.0 unx    16620 b- defN 24-Mar-25 13:55 tests/ut/transformers/models/gpt_neox/test_gpt_neox.py
--rw-r--r--  2.0 unx      691 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/graphormer/__init__.py
--rw-r--r--  2.0 unx     6947 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/graphormer/test_graphormer_cells.py
--rw-r--r--  2.0 unx    65804 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/graphormer/test_modeling_graphormer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/hubert/__init__.py
--rw-r--r--  2.0 unx    29210 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/hubert/test_modeling_hubert.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-29 07:53 tests/ut/transformers/models/internlm/__init__.py
--rw-r--r--  2.0 unx     1601 b- defN 24-Mar-29 07:53 tests/ut/transformers/models/internlm/test_modeling_internlm.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-16 11:41 tests/ut/transformers/models/layoutlm/__init__.py
--rw-r--r--  2.0 unx    17742 b- defN 24-Mar-28 15:43 tests/ut/transformers/models/layoutlm/test_modeling_layoutlm.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-24 20:22 tests/ut/transformers/models/layoutlmv2/__init__.py
--rw-r--r--  2.0 unx    28358 b- defN 24-Mar-27 18:05 tests/ut/transformers/models/layoutlmv2/test_modeling_layoutlmv2.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/llama/__init__.py
--rw-r--r--  2.0 unx    27045 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/llama/test_modeling_llama.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/longformer/__init__.py
--rw-r--r--  2.0 unx    31552 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/longformer/test_modeling_longformer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/luke/__init__.py
--rw-r--r--  2.0 unx    11176 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/luke/test_modeling_luke.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-16 11:41 tests/ut/transformers/models/mamba/__init__.py
--rw-r--r--  2.0 unx     5356 b- defN 24-Mar-16 11:41 tests/ut/transformers/models/mamba/test_modeling_graph_mamba.py
--rw-r--r--  2.0 unx    19188 b- defN 24-Mar-16 11:41 tests/ut/transformers/models/mamba/test_modeling_mamba.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mbart/__init__.py
--rw-r--r--  2.0 unx    29265 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/mbart/test_modeling_mbart.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/megatron_bert/__init__.py
--rw-r--r--  2.0 unx    16043 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/megatron_bert/test_modeling_megatron_bert.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mistral/__init__.py
--rw-r--r--  2.0 unx    17577 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/mistral/test_modeling_mistral.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-12 03:14 tests/ut/transformers/models/mixtral/__init__.py
--rw-r--r--  2.0 unx    19377 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/mixtral/test_modeling_mixtral.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mobilebert/__init__.py
--rw-r--r--  2.0 unx    12087 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mobilebert/test_mobilebert.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/moss/__init__.py
--rw-r--r--  2.0 unx     3681 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/moss/test_modeling_moss.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mt5/__init__.py
--rw-r--r--  2.0 unx     2095 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/mt5/test_modeling_mt5.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 08:18 tests/ut/transformers/models/musicgen/__init__.py
--rw-r--r--  2.0 unx    45746 b- defN 24-Mar-31 10:53 tests/ut/transformers/models/musicgen/test_modeling_musicgen.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-31 16:52 tests/ut/transformers/models/musicgen_melody/__init__.py
--rw-r--r--  2.0 unx     9926 b- defN 24-Mar-31 16:52 tests/ut/transformers/models/musicgen_melody/test_feature_extraction_musicgen_melody.py
--rw-r--r--  2.0 unx    46150 b- defN 24-Mar-31 16:52 tests/ut/transformers/models/musicgen_melody/test_modeling_musicgen_melody.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-31 16:52 tests/ut/transformers/models/musicgen_melody/test_processor_musicgen_melody.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/nezha/__init__.py
--rw-r--r--  2.0 unx    10126 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/nezha/test_modeling_nezha.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/opt/__init__.py
--rw-r--r--  2.0 unx    23125 b- defN 24-Apr-08 06:51 tests/ut/transformers/models/opt/test_modeling_opt.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/phi/__init__.py
--rw-r--r--  2.0 unx    18965 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/phi/test_modeling_phi.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/pop2piano/__init__.py
--rw-r--r--  2.0 unx    31317 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/pop2piano/test_modeling_pop2piano.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-04 00:35 tests/ut/transformers/models/qwen2/__init__.py
--rw-r--r--  2.0 unx    19480 b- defN 24-Mar-04 00:35 tests/ut/transformers/models/qwen2/test_modeling_qwen2.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-29 11:29 tests/ut/transformers/models/qwen2_moe/__init__.py
--rw-r--r--  2.0 unx    22239 b- defN 24-Mar-30 00:11 tests/ut/transformers/models/qwen2_moe/test_modeling_qwen2_moe.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/reformer/__init__.py
--rw-r--r--  2.0 unx    43606 b- defN 24-Mar-25 11:12 tests/ut/transformers/models/reformer/test_modeling_reformer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/roberta/__init__.py
--rw-r--r--  2.0 unx    22751 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/roberta/test_modeling_roberta.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/rwkv/__init__.py
--rw-r--r--  2.0 unx    17034 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/rwkv/test_modeling_rwkv.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/seamless_m4t/__init__.py
--rw-r--r--  2.0 unx    45139 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/seamless_m4t/test_modeling_seamless_m4t.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/seamless_m4t_v2/__init__.py
--rw-r--r--  2.0 unx    48018 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/seamless_m4t_v2/test_modeling_seamless_m4t_v2.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-09 17:05 tests/ut/transformers/models/starcoder2/__init__.py
--rw-r--r--  2.0 unx    16333 b- defN 24-Mar-09 17:05 tests/ut/transformers/models/starcoder2/test_modeling_starcoder2.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/t5/__init__.py
--rw-r--r--  2.0 unx    74031 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/t5/test_modeling_t5.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/tinybert/__init__.py
--rw-r--r--  2.0 unx    15357 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/tinybert/test_tinybert.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/wav2vec2/__init__.py
--rw-r--r--  2.0 unx    10497 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/wav2vec2/test_feature_extraction_wav2vec2.py
--rw-r--r--  2.0 unx    72157 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/wav2vec2/test_modeling_wav2vec2.py
--rw-r--r--  2.0 unx     6366 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/wav2vec2/test_processor_wav2vec2.py
--rw-r--r--  2.0 unx    40919 b- defN 24-Mar-28 15:57 tests/ut/transformers/models/wav2vec2/test_tokenization_wav2vec2.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/whisper/__init__.py
--rw-r--r--  2.0 unx    77595 b- defN 24-Mar-19 12:41 tests/ut/transformers/models/whisper/test_modeling_whisper.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/xlm/__init__.py
--rw-r--r--  2.0 unx    19441 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/xlm/test_modeling_xlm.py
--rw-r--r--  2.0 unx     3300 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/xlm/test_tokenization_xlm.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/xlm_roberta/__init__.py
--rw-r--r--  2.0 unx     2827 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/xlm_roberta/test_modeling_xlm_roberta.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-08 06:51 tests/ut/transformers/models/xlnet/__init__.py
--rw-r--r--  2.0 unx    28446 b- defN 24-Apr-08 06:51 tests/ut/transformers/models/xlnet/test_modeling_xlnet.py
--rw-r--r--  2.0 unx    12729 b- defN 24-Apr-08 06:51 tests/ut/transformers/models/xlnet/test_tokenization_xlnet.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/pipelines/__init__.py
--rw-r--r--  2.0 unx    18027 b- defN 24-Feb-29 06:56 tests/ut/transformers/pipelines/test_pipelines_common.py
--rw-r--r--  2.0 unx    12486 b- defN 24-Mar-31 10:53 tests/ut/transformers/pipelines/test_pipelines_document_question_answering.py
--rw-r--r--  2.0 unx    25446 b- defN 24-Mar-16 11:41 tests/ut/transformers/pipelines/test_pipelines_question_answering.py
--rw-r--r--  2.0 unx     3661 b- defN 24-Mar-16 11:41 tests/ut/transformers/pipelines/test_pipelines_text2text_generation.py
--rw-r--r--  2.0 unx     6805 b- defN 24-Feb-29 06:56 tests/ut/transformers/pipelines/test_pipelines_text_classification.py
--rw-r--r--  2.0 unx    13706 b- defN 24-Mar-16 11:41 tests/ut/transformers/pipelines/test_pipelines_text_generation.py
--rw-r--r--  2.0 unx    11105 b- defN 24-Mar-24 20:22 tests/ut/transformers/pipelines/test_pipelines_zero_shot_classification.py
--rw-r--r--  2.0 unx     1996 b- defN 23-Jul-16 07:16 tests/ut/utils/test_download.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/vocab/__init__.py
--rw-r--r--  2.0 unx     2076 b- defN 23-Mar-22 09:42 tests/ut/vocab/test_vocab.py
--rw-r--r--  2.0 unx     1029 b- defN 23-Jun-01 14:35 tests/ut/vocab/test_vocab_fasttext.py
--rw-r--r--  2.0 unx     1238 b- defN 23-Jun-01 14:35 tests/ut/vocab/test_vocab_glove.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-09 08:37 mindnlp-0.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      804 b- defN 24-Apr-09 08:37 mindnlp-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       57 b- defN 24-Apr-09 08:37 mindnlp-0.2.4.dist-info/NOTICE
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 08:37 mindnlp-0.2.4.dist-info/WHEEL
--r--------  2.0 unx       14 b- defN 24-Apr-09 08:37 mindnlp-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx   107234 b- defN 24-Apr-09 08:37 mindnlp-0.2.4.dist-info/RECORD
-1002 files, 17604563 bytes uncompressed, 5090958 bytes compressed:  71.1%
+-rw-rw-r--  2.0 unx      708 b- defN 23-Mar-22 09:42 tests/__init__.py
+-rw-rw-r--  2.0 unx      147 b- defN 24-Feb-29 06:56 tests/common.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/st/__init__.py
+-rw-rw-r--  2.0 unx     2834 b- defN 23-Jun-01 14:35 tests/st/test_bilstm_imdb.py
+-rw-rw-r--  2.0 unx     2110 b- defN 24-Feb-29 06:56 tests/st/test_longformer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/test_module/__init__.py
+-rw-rw-r--  2.0 unx      387 b- defN 24-Feb-29 06:56 tests/test_module/custom_configuration.py
+-rw-rw-r--  2.0 unx      777 b- defN 24-Feb-29 06:56 tests/test_module/custom_modeling.py
+-rw-rw-r--  2.0 unx     1117 b- defN 24-Feb-29 06:56 tests/test_module/custom_pipeline.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/dataset/__init__.py
+-rw-rw-r--  2.0 unx     2423 b- defN 24-Feb-29 06:56 tests/ut/dataset/test_imdb.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/dataset/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2555 b- defN 24-Feb-29 06:56 tests/ut/dataset/transforms/test_add_token.py
+-rw-rw-r--  2.0 unx     1235 b- defN 24-Feb-29 06:56 tests/ut/dataset/transforms/test_lookup.py
+-rw-rw-r--  2.0 unx     2560 b- defN 24-Feb-29 06:56 tests/ut/dataset/transforms/test_pad_transform.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/engine/__init__.py
+-rw-rw-r--  2.0 unx    92214 b- defN 24-Apr-23 14:20 tests/ut/engine/test_trainer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/legacy/__init__.py
+-rw-rw-r--  2.0 unx      845 b- defN 24-Feb-29 06:56 tests/ut/legacy/test_einsum.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/legacy/metrics/__init__.py
+-rw-rw-r--  2.0 unx    32973 b- defN 24-Apr-23 14:20 tests/ut/legacy/metrics/test_metrics_class.py
+-rw-rw-r--  2.0 unx    19947 b- defN 24-Apr-23 14:20 tests/ut/legacy/metrics/test_metrics_fn.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/__init__.py
+-rw-rw-r--  2.0 unx    13357 b- defN 24-Feb-29 06:56 tests/ut/modules/test_crf.py
+-rw-rw-r--  2.0 unx     5675 b- defN 24-Feb-29 06:56 tests/ut/modules/test_decoder.py
+-rw-rw-r--  2.0 unx     4267 b- defN 24-Feb-29 06:56 tests/ut/modules/test_encoder.py
+-rw-rw-r--  2.0 unx     1422 b- defN 23-Nov-13 07:20 tests/ut/modules/test_fasttext_embedding.py
+-rw-rw-r--  2.0 unx     6300 b- defN 24-May-06 12:16 tests/ut/modules/test_flashattention.py
+-rw-rw-r--  2.0 unx     1356 b- defN 24-Feb-29 06:56 tests/ut/modules/test_glove_embedding.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/attentions/__init__.py
+-rw-rw-r--  2.0 unx     1809 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_additive_attention.py
+-rw-rw-r--  2.0 unx     1784 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_binary_attention.py
+-rw-rw-r--  2.0 unx     1779 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_cosine_attention.py
+-rw-rw-r--  2.0 unx     1831 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_linear_attention.py
+-rw-rw-r--  2.0 unx     1540 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_scaled_dot_attention.py
+-rw-rw-r--  2.0 unx     2276 b- defN 24-Feb-29 06:56 tests/ut/modules/attentions/test_self_attention.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-01 14:35 tests/ut/modules/generation/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 24-Feb-29 06:56 tests/ut/modules/generation/test_generation_config.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/loss/__init__.py
+-rw-rw-r--  2.0 unx     2296 b- defN 24-Feb-29 06:56 tests/ut/modules/loss/test_cmrc2018loss.py
+-rw-rw-r--  2.0 unx     2385 b- defN 24-Feb-29 06:56 tests/ut/modules/loss/test_rdrop_loss.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/rnns/__init__.py
+-rw-rw-r--  2.0 unx     4872 b- defN 24-Feb-29 06:56 tests/ut/modules/rnns/test_gru.py
+-rw-rw-r--  2.0 unx     5180 b- defN 24-Feb-29 06:56 tests/ut/modules/rnns/test_lstm.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/modules/transformer/__init__.py
+-rw-rw-r--  2.0 unx     3775 b- defN 24-Feb-29 06:56 tests/ut/modules/transformer/test_multi_head_attention.py
+-rw-rw-r--  2.0 unx     2187 b- defN 24-Feb-29 06:56 tests/ut/modules/transformer/test_transformer_encoder.py
+-rw-rw-r--  2.0 unx     1434 b- defN 24-Feb-29 06:56 tests/ut/modules/transformer/test_transformer_encoder_layer.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-16 07:16 tests/ut/peft/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-16 07:16 tests/ut/peft/test_config.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/__init__.py
+-rw-rw-r--  2.0 unx    10147 b- defN 24-May-06 12:16 tests/ut/transformers/test_backbone_common.py
+-rw-rw-r--  2.0 unx     8097 b- defN 24-Feb-29 06:56 tests/ut/transformers/test_configuration_common.py
+-rw-rw-r--  2.0 unx     2231 b- defN 24-Mar-31 16:52 tests/ut/transformers/test_feature_extraction_common.py
+-rw-rw-r--  2.0 unx    15893 b- defN 24-May-06 12:16 tests/ut/transformers/test_image_processing_common.py
+-rw-rw-r--  2.0 unx    73153 b- defN 24-Apr-23 14:20 tests/ut/transformers/test_modeling_common.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-25 11:12 tests/ut/transformers/test_pipeline_mixin.py
+-rw-rw-r--  2.0 unx    16663 b- defN 24-Mar-31 16:52 tests/ut/transformers/test_sequence_feature_extraction_common.py
+-rw-rw-r--  2.0 unx   206613 b- defN 24-Feb-29 06:56 tests/ut/transformers/test_tokenization_common.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/generation/__init__.py
+-rw-rw-r--  2.0 unx    28522 b- defN 24-Feb-29 06:56 tests/ut/transformers/generation/test_framework_agnostic.py
+-rw-rw-r--  2.0 unx   123388 b- defN 24-Apr-23 14:20 tests/ut/transformers/generation/test_utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/albert/__init__.py
+-rw-rw-r--  2.0 unx    14176 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/albert/test_modeling_albert.py
+-rw-rw-r--  2.0 unx     8039 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/albert/test_tokenization_albert.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/align/__init__.py
+-rw-rw-r--  2.0 unx    21247 b- defN 24-Mar-27 18:05 tests/ut/transformers/models/align/test_modeling_align.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/altclip/__init__.py
+-rw-rw-r--  2.0 unx    20018 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/altclip/test_modeling_altclip.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/audio_spectrogram_transformer/__init__.py
+-rw-rw-r--  2.0 unx     9381 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/audio_spectrogram_transformer/test_modeling_audio_spectrogram_transformer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/auto/__init__.py
+-rw-rw-r--  2.0 unx     3723 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/auto/test_configuration_auto.py
+-rw-rw-r--  2.0 unx    15231 b- defN 24-Mar-20 16:25 tests/ut/transformers/models/auto/test_modeling_auto.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/autoformer/__init__.py
+-rw-rw-r--  2.0 unx    19293 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/autoformer/test_modeling_autoformer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/baichuan/__init__.py
+-rw-rw-r--  2.0 unx     2793 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/baichuan/test_modeling_baichuan.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bark/__init__.py
+-rw-rw-r--  2.0 unx    44187 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/bark/test_modeling_bark.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bart/__init__.py
+-rw-rw-r--  2.0 unx    95343 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/bart/test_modeling_bart.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-25 11:12 tests/ut/transformers/models/beit/__init__.py
+-rw-rw-r--  2.0 unx    19837 b- defN 24-Mar-25 11:12 tests/ut/transformers/models/beit/test_modeling_beit.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bert/__init__.py
+-rw-rw-r--  2.0 unx    25734 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/bert/test_modeling_bert.py
+-rw-rw-r--  2.0 unx     2048 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bert/test_modeling_graph_bert.py
+-rw-rw-r--  2.0 unx    14288 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/bert/test_tokenization_bert.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-25 13:50 tests/ut/transformers/models/bert_generation/__init__.py
+-rw-rw-r--  2.0 unx    12696 b- defN 24-Mar-25 13:50 tests/ut/transformers/models/bert_generation/test_modeling_bert_generation.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-09 17:05 tests/ut/transformers/models/big_bird/__init__.py
+-rw-rw-r--  2.0 unx    46579 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/big_bird/test_modeling_big_bird.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-28 03:06 tests/ut/transformers/models/bigbird_pegasus/__init__.py
+-rw-rw-r--  2.0 unx   110760 b- defN 24-Mar-28 06:03 tests/ut/transformers/models/bigbird_pegasus/test_modeling_bigbird_pegasus.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/biogpt/__init__.py
+-rw-rw-r--  2.0 unx    19717 b- defN 24-Mar-19 16:44 tests/ut/transformers/models/biogpt/test_modeling_biogpt.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-31 12:05 tests/ut/transformers/models/bit/__init__.py
+-rw-rw-r--  2.0 unx    11755 b- defN 24-Mar-31 12:35 tests/ut/transformers/models/bit/test_modeling_bit.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-02 03:19 tests/ut/transformers/models/blenderbot/__init__.py
+-rw-rw-r--  2.0 unx    22474 b- defN 24-Apr-02 03:19 tests/ut/transformers/models/blenderbot/test_modeling_blenderbot.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-02 08:27 tests/ut/transformers/models/blenderbot_small/__init__.py
+-rw-rw-r--  2.0 unx    22787 b- defN 24-Apr-08 03:51 tests/ut/transformers/models/blenderbot_small/test_modeling_blenderbot_small.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-02 15:06 tests/ut/transformers/models/blip/__init__.py
+-rw-rw-r--  2.0 unx    42838 b- defN 24-Apr-02 15:06 tests/ut/transformers/models/blip/test_modeling_blip.py
+-rw-rw-r--  2.0 unx     6896 b- defN 24-Apr-02 15:06 tests/ut/transformers/models/blip/test_modeling_blip_text.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-08 03:51 tests/ut/transformers/models/blip_2/__init__.py
+-rw-rw-r--  2.0 unx    39138 b- defN 24-Apr-08 03:51 tests/ut/transformers/models/blip_2/test_modeling_blip_2.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/bloom/__init__.py
+-rw-rw-r--  2.0 unx    35152 b- defN 24-Mar-28 15:57 tests/ut/transformers/models/bloom/test_modeling_bloom.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/bridgetower/__init__.py
+-rw-rw-r--  2.0 unx    23014 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/bridgetower/test_modeling_bridgetower.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/bros/__init__.py
+-rw-rw-r--  2.0 unx    16094 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/bros/test_modeling_bros.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/chatglm/__init__.py
+-rw-rw-r--  2.0 unx    13928 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/chatglm/test_modeling_chatglm.py
+-rw-rw-r--  2.0 unx    13970 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/chatglm/test_modeling_graph_chatglm.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/clip/__init__.py
+-rw-rw-r--  2.0 unx    25666 b- defN 24-Mar-03 07:54 tests/ut/transformers/models/clip/test_modeling_clip.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/codegen/__init__.py
+-rw-rw-r--  2.0 unx    23368 b- defN 24-Mar-03 07:54 tests/ut/transformers/models/codegen/test_modeling_codegen.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-08 03:51 tests/ut/transformers/models/convbert/__init__.py
+-rw-rw-r--  2.0 unx    19740 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/convbert/test_modeling_convbert.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-06 12:16 tests/ut/transformers/models/convnext/__init__.py
+-rw-rw-r--  2.0 unx    11121 b- defN 24-May-06 12:16 tests/ut/transformers/models/convnext/test_modeling_convnext.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/cpmant/__init__.py
+-rw-rw-r--  2.0 unx     9906 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/cpmant/test_modeling_cpmant.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/cpmbee/__init__.py
+-rw-rw-r--  2.0 unx     8443 b- defN 24-Mar-18 02:46 tests/ut/transformers/models/cpmbee/test_modeling_cpmbee.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-06 12:16 tests/ut/transformers/models/cvt/__init__.py
+-rw-rw-r--  2.0 unx    10006 b- defN 24-May-06 12:16 tests/ut/transformers/models/cvt/test_modeling_cvt.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/deberta/__init__.py
+-rw-rw-r--  2.0 unx    12019 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/deberta/test_modeling_deberta.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/encodec/__init__.py
+-rw-rw-r--  2.0 unx    20901 b- defN 24-Mar-27 05:46 tests/ut/transformers/models/encodec/test_modeling_encodec.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/ernie/__init__.py
+-rw-rw-r--  2.0 unx    22370 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/ernie/test_modeling_ernie.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/ernie_m/__init__.py
+-rw-rw-r--  2.0 unx    12542 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/ernie_m/test_modeling_ernie_m.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-03 07:54 tests/ut/transformers/models/esm/__init__.py
+-rw-rw-r--  2.0 unx    13068 b- defN 24-Mar-03 07:54 tests/ut/transformers/models/esm/test_modeling_esm.py
+-rw-rw-r--  2.0 unx    10139 b- defN 24-Mar-04 00:35 tests/ut/transformers/models/esm/test_modeling_esmfold.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/falcon/__init__.py
+-rw-rw-r--  2.0 unx    22507 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/falcon/test_modeling_falcon.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gemma/__init__.py
+-rw-rw-r--  2.0 unx    22221 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gemma/test_modeling_gemma.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt/__init__.py
+-rw-rw-r--  2.0 unx    11432 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt/test_modeling_gpt.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt2/__init__.py
+-rw-rw-r--  2.0 unx    36548 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt2/test_modeling_gpt2.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt_bigcode/__init__.py
+-rw-rw-r--  2.0 unx    25963 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt_bigcode/test_modeling_gpt_bigcode.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt_neo/__init__.py
+-rw-rw-r--  2.0 unx     4504 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/gpt_neo/test_gpt_neo.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-25 13:55 tests/ut/transformers/models/gpt_neox/__init__.py
+-rw-rw-r--  2.0 unx    16680 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/gpt_neox/test_modeling_gpt_neox.py
+-rw-rw-r--  2.0 unx      691 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/graphormer/__init__.py
+-rw-rw-r--  2.0 unx     6947 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/graphormer/test_graphormer_cells.py
+-rw-rw-r--  2.0 unx    65804 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/graphormer/test_modeling_graphormer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/hubert/__init__.py
+-rw-rw-r--  2.0 unx    29210 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/hubert/test_modeling_hubert.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-29 07:53 tests/ut/transformers/models/internlm/__init__.py
+-rw-rw-r--  2.0 unx     1601 b- defN 24-Mar-29 07:53 tests/ut/transformers/models/internlm/test_modeling_internlm.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-16 11:41 tests/ut/transformers/models/layoutlm/__init__.py
+-rw-rw-r--  2.0 unx    17742 b- defN 24-Mar-28 15:43 tests/ut/transformers/models/layoutlm/test_modeling_layoutlm.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-24 20:22 tests/ut/transformers/models/layoutlmv2/__init__.py
+-rw-rw-r--  2.0 unx    28358 b- defN 24-Mar-27 18:05 tests/ut/transformers/models/layoutlmv2/test_modeling_layoutlmv2.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/llama/__init__.py
+-rw-rw-r--  2.0 unx    27045 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/llama/test_modeling_llama.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-06 12:16 tests/ut/transformers/models/llava/__init__.py
+-rw-rw-r--  2.0 unx    29866 b- defN 24-May-06 12:16 tests/ut/transformers/models/llava/test_modeling_llava.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-06 12:16 tests/ut/transformers/models/llava_next/__init__.py
+-rw-rw-r--  2.0 unx     8896 b- defN 24-May-06 12:16 tests/ut/transformers/models/llava_next/test_image_processor_llava_next.py
+-rw-rw-r--  2.0 unx    20537 b- defN 24-May-06 12:16 tests/ut/transformers/models/llava_next/test_modeling_llava_next.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/longformer/__init__.py
+-rw-rw-r--  2.0 unx    31552 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/longformer/test_modeling_longformer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/luke/__init__.py
+-rw-rw-r--  2.0 unx    11176 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/luke/test_modeling_luke.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-16 11:41 tests/ut/transformers/models/mamba/__init__.py
+-rw-rw-r--  2.0 unx     5356 b- defN 24-Mar-16 11:41 tests/ut/transformers/models/mamba/test_modeling_graph_mamba.py
+-rw-rw-r--  2.0 unx    19188 b- defN 24-Mar-16 11:41 tests/ut/transformers/models/mamba/test_modeling_mamba.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mbart/__init__.py
+-rw-rw-r--  2.0 unx    29265 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/mbart/test_modeling_mbart.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/megatron_bert/__init__.py
+-rw-rw-r--  2.0 unx    16043 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/megatron_bert/test_modeling_megatron_bert.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mistral/__init__.py
+-rw-rw-r--  2.0 unx    17577 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/mistral/test_modeling_mistral.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-12 03:14 tests/ut/transformers/models/mixtral/__init__.py
+-rw-rw-r--  2.0 unx    19377 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/mixtral/test_modeling_mixtral.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mobilebert/__init__.py
+-rw-rw-r--  2.0 unx    12087 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mobilebert/test_mobilebert.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/moss/__init__.py
+-rw-rw-r--  2.0 unx     3681 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/moss/test_modeling_moss.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/mpnet/__init__.py
+-rw-rw-r--  2.0 unx    10618 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/mpnet/test_modeling_mpnet.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/mpt/__init__.py
+-rw-rw-r--  2.0 unx    20662 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/mpt/test_modeling_mpt.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/mt5/__init__.py
+-rw-rw-r--  2.0 unx     2095 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/mt5/test_modeling_mt5.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-26 08:18 tests/ut/transformers/models/musicgen/__init__.py
+-rw-rw-r--  2.0 unx    45746 b- defN 24-Mar-31 10:53 tests/ut/transformers/models/musicgen/test_modeling_musicgen.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-31 16:52 tests/ut/transformers/models/musicgen_melody/__init__.py
+-rw-rw-r--  2.0 unx     9926 b- defN 24-Mar-31 16:52 tests/ut/transformers/models/musicgen_melody/test_feature_extraction_musicgen_melody.py
+-rw-rw-r--  2.0 unx    46150 b- defN 24-Mar-31 16:52 tests/ut/transformers/models/musicgen_melody/test_modeling_musicgen_melody.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-31 16:52 tests/ut/transformers/models/musicgen_melody/test_processor_musicgen_melody.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/nezha/__init__.py
+-rw-rw-r--  2.0 unx    10126 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/nezha/test_modeling_nezha.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/olmo/__init__.py
+-rw-rw-r--  2.0 unx    19188 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/olmo/test_modeling_olmo.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/opt/__init__.py
+-rw-rw-r--  2.0 unx    23125 b- defN 24-Apr-08 03:51 tests/ut/transformers/models/opt/test_modeling_opt.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/pegasus/__init__.py
+-rw-rw-r--  2.0 unx    25878 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/pegasus/test_modeling_pegasus.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/phi/__init__.py
+-rw-rw-r--  2.0 unx    18965 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/phi/test_modeling_phi.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/pop2piano/__init__.py
+-rw-rw-r--  2.0 unx    31317 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/pop2piano/test_modeling_pop2piano.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-04 00:35 tests/ut/transformers/models/qwen2/__init__.py
+-rw-rw-r--  2.0 unx    19480 b- defN 24-Mar-04 00:35 tests/ut/transformers/models/qwen2/test_modeling_qwen2.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-29 11:29 tests/ut/transformers/models/qwen2_moe/__init__.py
+-rw-rw-r--  2.0 unx    22239 b- defN 24-Mar-30 00:11 tests/ut/transformers/models/qwen2_moe/test_modeling_qwen2_moe.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-19 16:41 tests/ut/transformers/models/reformer/__init__.py
+-rw-rw-r--  2.0 unx    43606 b- defN 24-Mar-25 11:12 tests/ut/transformers/models/reformer/test_modeling_reformer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-06 12:16 tests/ut/transformers/models/resnet/__init__.py
+-rw-rw-r--  2.0 unx    11827 b- defN 24-May-06 12:16 tests/ut/transformers/models/resnet/test_modeling_resnet.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/roberta/__init__.py
+-rw-rw-r--  2.0 unx    22751 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/roberta/test_modeling_roberta.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/rwkv/__init__.py
+-rw-rw-r--  2.0 unx    17034 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/rwkv/test_modeling_rwkv.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/sam/__init__.py
+-rw-rw-r--  2.0 unx    27308 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/sam/test_modeling_sam.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/seamless_m4t/__init__.py
+-rw-rw-r--  2.0 unx    45139 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/seamless_m4t/test_modeling_seamless_m4t.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/seamless_m4t_v2/__init__.py
+-rw-rw-r--  2.0 unx    48018 b- defN 24-May-06 13:23 tests/ut/transformers/models/seamless_m4t_v2/test_modeling_seamless_m4t_v2.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/segformer/__init__.py
+-rw-rw-r--  2.0 unx    16779 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/segformer/test_modeling_segformer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-09 17:05 tests/ut/transformers/models/starcoder2/__init__.py
+-rw-rw-r--  2.0 unx    16333 b- defN 24-Mar-09 17:05 tests/ut/transformers/models/starcoder2/test_modeling_starcoder2.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/t5/__init__.py
+-rw-rw-r--  2.0 unx    74031 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/t5/test_modeling_t5.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/timesformer/__init__.py
+-rw-rw-r--  2.0 unx    13192 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/timesformer/test_modeling_timesformer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/tinybert/__init__.py
+-rw-rw-r--  2.0 unx    15357 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/tinybert/test_tinybert.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-06 12:16 tests/ut/transformers/models/vipllava/__init__.py
+-rw-rw-r--  2.0 unx    18077 b- defN 24-May-06 12:16 tests/ut/transformers/models/vipllava/test_modeling_vipllava.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/wav2vec2/__init__.py
+-rw-rw-r--  2.0 unx    10497 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/wav2vec2/test_feature_extraction_wav2vec2.py
+-rw-rw-r--  2.0 unx    72157 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/wav2vec2/test_modeling_wav2vec2.py
+-rw-rw-r--  2.0 unx     6366 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/wav2vec2/test_processor_wav2vec2.py
+-rw-rw-r--  2.0 unx    40919 b- defN 24-Mar-28 15:57 tests/ut/transformers/models/wav2vec2/test_tokenization_wav2vec2.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/whisper/__init__.py
+-rw-rw-r--  2.0 unx    77595 b- defN 24-Mar-19 12:41 tests/ut/transformers/models/whisper/test_modeling_whisper.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/xlm/__init__.py
+-rw-rw-r--  2.0 unx    19441 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/xlm/test_modeling_xlm.py
+-rw-rw-r--  2.0 unx     3300 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/xlm/test_tokenization_xlm.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/models/xlm_roberta/__init__.py
+-rw-rw-r--  2.0 unx     2827 b- defN 24-Mar-04 15:11 tests/ut/transformers/models/xlm_roberta/test_modeling_xlm_roberta.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-08 03:51 tests/ut/transformers/models/xlnet/__init__.py
+-rw-rw-r--  2.0 unx    28389 b- defN 24-Apr-23 14:20 tests/ut/transformers/models/xlnet/test_modeling_xlnet.py
+-rw-rw-r--  2.0 unx    12729 b- defN 24-Apr-08 03:51 tests/ut/transformers/models/xlnet/test_tokenization_xlnet.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-29 06:56 tests/ut/transformers/pipelines/__init__.py
+-rw-rw-r--  2.0 unx    18027 b- defN 24-Feb-29 06:56 tests/ut/transformers/pipelines/test_pipelines_common.py
+-rw-rw-r--  2.0 unx    12486 b- defN 24-Mar-31 10:53 tests/ut/transformers/pipelines/test_pipelines_document_question_answering.py
+-rw-rw-r--  2.0 unx    25446 b- defN 24-Mar-16 11:41 tests/ut/transformers/pipelines/test_pipelines_question_answering.py
+-rw-rw-r--  2.0 unx     3661 b- defN 24-Mar-16 11:41 tests/ut/transformers/pipelines/test_pipelines_text2text_generation.py
+-rw-rw-r--  2.0 unx     6805 b- defN 24-Feb-29 06:56 tests/ut/transformers/pipelines/test_pipelines_text_classification.py
+-rw-rw-r--  2.0 unx    13706 b- defN 24-Mar-16 11:41 tests/ut/transformers/pipelines/test_pipelines_text_generation.py
+-rw-rw-r--  2.0 unx    11105 b- defN 24-Mar-24 20:22 tests/ut/transformers/pipelines/test_pipelines_zero_shot_classification.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:42 tests/ut/vocab/__init__.py
+-rw-rw-r--  2.0 unx     2076 b- defN 23-Mar-22 09:42 tests/ut/vocab/test_vocab.py
+-rw-rw-r--  2.0 unx     1029 b- defN 23-Jun-01 14:35 tests/ut/vocab/test_vocab_fasttext.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-01 14:35 tests/ut/vocab/test_vocab_glove.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-06 13:29 mindnlp-0.3.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      849 b- defN 24-May-06 13:29 mindnlp-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       57 b- defN 24-May-06 13:29 mindnlp-0.3.0.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-06 13:29 mindnlp-0.3.0.dist-info/WHEEL
+-r--------  2.0 unx       14 b- defN 24-May-06 13:29 mindnlp-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx   110646 b- defN 24-May-06 13:29 mindnlp-0.3.0.dist-info/RECORD
+1036 files, 16239595 bytes uncompressed, 3559916 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -1,17 +1,17 @@
 Filename: mindnlp/__init__.py
 Comment: 
 
-Filename: mindnlp/configs.py
+Filename: mindnlp/amp.py
 Comment: 
 
-Filename: mindnlp/injection.py
+Filename: mindnlp/configs.py
 Comment: 
 
-Filename: mindnlp/readme.md
+Filename: mindnlp/injection.py
 Comment: 
 
 Filename: mindnlp/_csrc/cuda/flash.cu
 Comment: 
 
 Filename: mindnlp/_csrc/cuda/wkv.cu
 Comment: 
@@ -27,14 +27,65 @@
 
 Filename: mindnlp/_legacy/initializer.py
 Comment: 
 
 Filename: mindnlp/_legacy/utils.py
 Comment: 
 
+Filename: mindnlp/_legacy/engine/__init__.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/evaluator.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/export.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/train_args.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/utils.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/callbacks/__init__.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/callbacks/best_model_callback.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/callbacks/callback_manager.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/callbacks/checkpoint_callback.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/callbacks/earlystop_callback.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/callbacks/timer_callback.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/trainer/__init__.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/trainer/base.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/trainer/ppo.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/trainer/rm.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/trainer/sft.py
+Comment: 
+
+Filename: mindnlp/_legacy/engine/trainer/utils.py
+Comment: 
+
 Filename: mindnlp/_legacy/hypercomplex/__init__.py
 Comment: 
 
 Filename: mindnlp/_legacy/hypercomplex/utils.py
 Comment: 
 
 Filename: mindnlp/_legacy/hypercomplex/complex/__init__.py
@@ -117,87 +168,57 @@
 
 Filename: mindnlp/_legacy/hypercomplex/hypercomplex/hc_pool.py
 Comment: 
 
 Filename: mindnlp/_legacy/hypercomplex/hypercomplex/uniform_operator.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/hypercomplex_td.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/dual_svd.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/qr.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/star_svd.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/svd.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/t_svd.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/matrix.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/scalar.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/scalar_visitor.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/vector.py
+Filename: mindnlp/_legacy/metrics/__init__.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/complex/_complex_algebra_impl.py
+Filename: mindnlp/_legacy/metrics/accuracy.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/complex/complex_algebra_factory.py
+Filename: mindnlp/_legacy/metrics/bleu.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/dual/_dual_algebra_impl.py
+Filename: mindnlp/_legacy/metrics/confusion_matrix.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/dual/dual_algebra_factory.py
+Filename: mindnlp/_legacy/metrics/distinct.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_math_obj_impl.py
+Filename: mindnlp/_legacy/metrics/em_score.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_matrix_impl.py
+Filename: mindnlp/_legacy/metrics/f1.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_scalar_impl.py
+Filename: mindnlp/_legacy/metrics/matthews.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_vector_impl.py
+Filename: mindnlp/_legacy/metrics/pearson.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_algebra_factory.py
+Filename: mindnlp/_legacy/metrics/perplexity.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_matrix.py
+Filename: mindnlp/_legacy/metrics/precision.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_scalar.py
+Filename: mindnlp/_legacy/metrics/recall.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_vector.py
+Filename: mindnlp/_legacy/metrics/rouge.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/real/real_matrix.py
+Filename: mindnlp/_legacy/metrics/spearman.py
 Comment: 
 
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/real/real_scalar.py
-Comment: 
-
-Filename: mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/real/real_vector.py
+Filename: mindnlp/_legacy/metrics/utils.py
 Comment: 
 
 Filename: mindnlp/_legacy/nn/__init__.py
 Comment: 
 
 Filename: mindnlp/_legacy/nn/dropout.py
 Comment: 
@@ -261,14 +282,23 @@
 
 Filename: mindnlp/abc/modules/encoder.py
 Comment: 
 
 Filename: mindnlp/abc/modules/generator.py
 Comment: 
 
+Filename: mindnlp/accelerate/__init__.py
+Comment: 
+
+Filename: mindnlp/accelerate/accelerator.py
+Comment: 
+
+Filename: mindnlp/accelerate/inference.py
+Comment: 
+
 Filename: mindnlp/data/__init__.py
 Comment: 
 
 Filename: mindnlp/data/io/__init__.py
 Comment: 
 
 Filename: mindnlp/data/io/audio.py
@@ -282,14 +312,17 @@
 
 Filename: mindnlp/dataset/__init__.py
 Comment: 
 
 Filename: mindnlp/dataset/load.py
 Comment: 
 
+Filename: mindnlp/dataset/map_fn.py
+Comment: 
+
 Filename: mindnlp/dataset/utils.py
 Comment: 
 
 Filename: mindnlp/dataset/transforms/__init__.py
 Comment: 
 
 Filename: mindnlp/dataset/transforms/basic_tokenizer.py
@@ -300,162 +333,72 @@
 
 Filename: mindnlp/dataset/transforms/lookup.py
 Comment: 
 
 Filename: mindnlp/dataset/transforms/pad_transform.py
 Comment: 
 
-Filename: mindnlp/diffusers/__init__.py
-Comment: 
-
-Filename: mindnlp/diffusers/loaders/__init__.py
-Comment: 
-
-Filename: mindnlp/diffusers/models/__init__.py
-Comment: 
-
-Filename: mindnlp/diffusers/pipelines/__init__.py
-Comment: 
-
-Filename: mindnlp/diffusers/schedulers/__init__.py
-Comment: 
-
-Filename: mindnlp/diffusers/utils/__init__.py
-Comment: 
-
 Filename: mindnlp/engine/__init__.py
 Comment: 
 
-Filename: mindnlp/engine/evaluator.py
+Filename: mindnlp/engine/callbacks.py
 Comment: 
 
 Filename: mindnlp/engine/export.py
 Comment: 
 
-Filename: mindnlp/engine/train_args.py
+Filename: mindnlp/engine/utils.py
 Comment: 
 
-Filename: mindnlp/engine/utils.py
+Filename: mindnlp/engine/train_args/__init__.py
 Comment: 
 
-Filename: mindnlp/engine/callbacks/__init__.py
+Filename: mindnlp/engine/train_args/base.py
 Comment: 
 
-Filename: mindnlp/engine/callbacks/best_model_callback.py
+Filename: mindnlp/engine/train_args/ddpo.py
 Comment: 
 
-Filename: mindnlp/engine/callbacks/callback_manager.py
+Filename: mindnlp/engine/train_args/kto.py
 Comment: 
 
-Filename: mindnlp/engine/callbacks/checkpoint_callback.py
+Filename: mindnlp/engine/train_args/ppo.py
 Comment: 
 
-Filename: mindnlp/engine/callbacks/earlystop_callback.py
+Filename: mindnlp/engine/train_args/reward.py
 Comment: 
 
-Filename: mindnlp/engine/callbacks/timer_callback.py
+Filename: mindnlp/engine/train_args/seq2seq.py
 Comment: 
 
 Filename: mindnlp/engine/trainer/__init__.py
 Comment: 
 
 Filename: mindnlp/engine/trainer/base.py
 Comment: 
 
-Filename: mindnlp/engine/trainer/ppo.py
-Comment: 
-
-Filename: mindnlp/engine/trainer/rm.py
-Comment: 
-
-Filename: mindnlp/engine/trainer/sft.py
-Comment: 
-
-Filename: mindnlp/engine/trainer/utils.py
-Comment: 
-
-Filename: mindnlp/evaluate/__init__.py
-Comment: 
-
-Filename: mindnlp/evaluate/suite.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/__init__.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/audio_classification.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/automatic_speech_recognition.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/base.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/image_classification.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/question_answering.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/text2text_generation.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/text_classification.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/text_generation.py
-Comment: 
-
-Filename: mindnlp/evaluate/evaluator/token_classification.py
+Filename: mindnlp/engine/trainer/default_func.py
 Comment: 
 
-Filename: mindnlp/metrics/__init__.py
+Filename: mindnlp/engine/trainer/ppo_trainer.py
 Comment: 
 
-Filename: mindnlp/metrics/accuracy.py
+Filename: mindnlp/engine/trainer/reward_trainer.py
 Comment: 
 
-Filename: mindnlp/metrics/bleu.py
+Filename: mindnlp/engine/trainer/rl_base.py
 Comment: 
 
-Filename: mindnlp/metrics/confusion_matrix.py
-Comment: 
-
-Filename: mindnlp/metrics/distinct.py
-Comment: 
-
-Filename: mindnlp/metrics/em_score.py
-Comment: 
-
-Filename: mindnlp/metrics/f1.py
-Comment: 
-
-Filename: mindnlp/metrics/matthews.py
-Comment: 
-
-Filename: mindnlp/metrics/pearson.py
-Comment: 
-
-Filename: mindnlp/metrics/perplexity.py
-Comment: 
-
-Filename: mindnlp/metrics/precision.py
-Comment: 
-
-Filename: mindnlp/metrics/recall.py
-Comment: 
-
-Filename: mindnlp/metrics/rouge.py
+Filename: mindnlp/engine/trainer/rm.py
 Comment: 
 
-Filename: mindnlp/metrics/spearman.py
+Filename: mindnlp/engine/trainer/seq2seq_trainer.py
 Comment: 
 
-Filename: mindnlp/metrics/utils.py
+Filename: mindnlp/engine/trainer/sft_trainer.py
 Comment: 
 
 Filename: mindnlp/modules/__init__.py
 Comment: 
 
 Filename: mindnlp/modules/accumulator.py
 Comment: 
@@ -465,14 +408,17 @@
 
 Filename: mindnlp/modules/crf.py
 Comment: 
 
 Filename: mindnlp/modules/loss.py
 Comment: 
 
+Filename: mindnlp/modules/optimization.py
+Comment: 
+
 Filename: mindnlp/modules/rnns.py
 Comment: 
 
 Filename: mindnlp/modules/weight_norm.py
 Comment: 
 
 Filename: mindnlp/modules/custom/__init__.py
@@ -552,44 +498,80 @@
 
 Filename: mindnlp/peft/tuners/lora.py
 Comment: 
 
 Filename: mindnlp/peft/tuners/tuners_utils.py
 Comment: 
 
-Filename: mindnlp/peft/utils/__init__.py
+Filename: mindnlp/peft/tuners/adalora/__init__.py
 Comment: 
 
-Filename: mindnlp/peft/utils/other.py
+Filename: mindnlp/peft/tuners/adalora/config.py
 Comment: 
 
-Filename: mindnlp/peft/utils/peft_types.py
+Filename: mindnlp/peft/tuners/adalora/layer.py
 Comment: 
 
-Filename: mindnlp/peft/utils/save_and_load.py
+Filename: mindnlp/peft/tuners/adalora/model.py
 Comment: 
 
-Filename: mindnlp/text2vec/__init__.py
+Filename: mindnlp/peft/tuners/adaption_prompt/__init__.py
 Comment: 
 
-Filename: mindnlp/text2vec/sentence_model.py
+Filename: mindnlp/peft/tuners/adaption_prompt/config.py
 Comment: 
 
-Filename: mindnlp/text2vec/word2vec.py
+Filename: mindnlp/peft/tuners/adaption_prompt/layer.py
+Comment: 
+
+Filename: mindnlp/peft/tuners/adaption_prompt/model.py
+Comment: 
+
+Filename: mindnlp/peft/tuners/adaption_prompt/utils.py
+Comment: 
+
+Filename: mindnlp/peft/tuners/ia3/__init__.py
+Comment: 
+
+Filename: mindnlp/peft/tuners/ia3/config.py
+Comment: 
+
+Filename: mindnlp/peft/tuners/ia3/layer.py
+Comment: 
+
+Filename: mindnlp/peft/tuners/ia3/model.py
+Comment: 
+
+Filename: mindnlp/peft/utils/__init__.py
+Comment: 
+
+Filename: mindnlp/peft/utils/other.py
+Comment: 
+
+Filename: mindnlp/peft/utils/peft_types.py
+Comment: 
+
+Filename: mindnlp/peft/utils/save_and_load.py
+Comment: 
+
+Filename: mindnlp/sentence/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/activations.py
 Comment: 
 
 Filename: mindnlp/transformers/audio_utils.py
 Comment: 
 
+Filename: mindnlp/transformers/backbone_utils.py
+Comment: 
+
 Filename: mindnlp/transformers/cache_utils.py
 Comment: 
 
 Filename: mindnlp/transformers/configuration_utils.py
 Comment: 
 
 Filename: mindnlp/transformers/convert_slow_tokenizer.py
@@ -1110,14 +1092,29 @@
 
 Filename: mindnlp/transformers/models/convbert/convbert_tokenizer.py
 Comment: 
 
 Filename: mindnlp/transformers/models/convbert/convbert_tokenizer_fast.py
 Comment: 
 
+Filename: mindnlp/transformers/models/convbert/graph_convbert.py
+Comment: 
+
+Filename: mindnlp/transformers/models/convnext/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/convnext/configuration_convnext.py
+Comment: 
+
+Filename: mindnlp/transformers/models/convnext/image_processing_convnext.py
+Comment: 
+
+Filename: mindnlp/transformers/models/convnext/modeling_convnext.py
+Comment: 
+
 Filename: mindnlp/transformers/models/cpm/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/cpm/tokenization_cpm.py
 Comment: 
 
 Filename: mindnlp/transformers/models/cpm/tokenization_cpm_fast.py
@@ -1143,14 +1140,23 @@
 
 Filename: mindnlp/transformers/models/cpmbee/modeling_cpmbee.py
 Comment: 
 
 Filename: mindnlp/transformers/models/cpmbee/tokenization_cpmbee.py
 Comment: 
 
+Filename: mindnlp/transformers/models/cvt/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/cvt/configuration_cvt.py
+Comment: 
+
+Filename: mindnlp/transformers/models/cvt/modeling_cvt.py
+Comment: 
+
 Filename: mindnlp/transformers/models/deberta/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/deberta/configuration_deberta.py
 Comment: 
 
 Filename: mindnlp/transformers/models/deberta/modeling_deberta.py
@@ -1497,14 +1503,41 @@
 
 Filename: mindnlp/transformers/models/llama/tokenization_llama.py
 Comment: 
 
 Filename: mindnlp/transformers/models/llama/tokenization_llama_fast.py
 Comment: 
 
+Filename: mindnlp/transformers/models/llava/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/llava/configuration_llava.py
+Comment: 
+
+Filename: mindnlp/transformers/models/llava/modeling_llava.py
+Comment: 
+
+Filename: mindnlp/transformers/models/llava/processing_llava.py
+Comment: 
+
+Filename: mindnlp/transformers/models/llava_next/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/llava_next/configuration_llava_next.py
+Comment: 
+
+Filename: mindnlp/transformers/models/llava_next/image_processing_llava_next.py
+Comment: 
+
+Filename: mindnlp/transformers/models/llava_next/modeling_llava_next.py
+Comment: 
+
+Filename: mindnlp/transformers/models/llava_next/processing_llava_next.py
+Comment: 
+
 Filename: mindnlp/transformers/models/longformer/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/longformer/configuration_longformer.py
 Comment: 
 
 Filename: mindnlp/transformers/models/longformer/modeling_longformer.py
@@ -1647,14 +1680,38 @@
 
 Filename: mindnlp/transformers/models/moss/moss_configuration.py
 Comment: 
 
 Filename: mindnlp/transformers/models/moss/moss_tokenization.py
 Comment: 
 
+Filename: mindnlp/transformers/models/mpnet/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/mpnet/configuration_mpnet.py
+Comment: 
+
+Filename: mindnlp/transformers/models/mpnet/modeling_mpnet.py
+Comment: 
+
+Filename: mindnlp/transformers/models/mpnet/tokenization_mpnet.py
+Comment: 
+
+Filename: mindnlp/transformers/models/mpnet/tokenization_mpnet_fast.py
+Comment: 
+
+Filename: mindnlp/transformers/models/mpt/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/mpt/configuration_mpt.py
+Comment: 
+
+Filename: mindnlp/transformers/models/mpt/modeling_mpt.py
+Comment: 
+
 Filename: mindnlp/transformers/models/mt5/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/mt5/configuration_mt5.py
 Comment: 
 
 Filename: mindnlp/transformers/models/mt5/modeling_mt5.py
@@ -1695,26 +1752,50 @@
 
 Filename: mindnlp/transformers/models/nezha/nezha_config.py
 Comment: 
 
 Filename: mindnlp/transformers/models/nezha/nezha_tokenizer.py
 Comment: 
 
+Filename: mindnlp/transformers/models/olmo/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/olmo/configuration_olmo.py
+Comment: 
+
+Filename: mindnlp/transformers/models/olmo/modeling_olmo.py
+Comment: 
+
+Filename: mindnlp/transformers/models/openelm/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/openelm/configuration_openelm.py
+Comment: 
+
+Filename: mindnlp/transformers/models/openelm/modeling_openelm.py
+Comment: 
+
 Filename: mindnlp/transformers/models/opt/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/opt/configuration_opt.py
 Comment: 
 
 Filename: mindnlp/transformers/models/opt/modeling_opt.py
 Comment: 
 
 Filename: mindnlp/transformers/models/pegasus/__init__.py
 Comment: 
 
+Filename: mindnlp/transformers/models/pegasus/configuration_pegasus.py
+Comment: 
+
+Filename: mindnlp/transformers/models/pegasus/modeling_pegasus.py
+Comment: 
+
 Filename: mindnlp/transformers/models/pegasus/tokenization_pegasus.py
 Comment: 
 
 Filename: mindnlp/transformers/models/pegasus/tokenization_pegasus_fast.py
 Comment: 
 
 Filename: mindnlp/transformers/models/phi/__init__.py
@@ -1722,14 +1803,23 @@
 
 Filename: mindnlp/transformers/models/phi/configuration_phi.py
 Comment: 
 
 Filename: mindnlp/transformers/models/phi/modeling_phi.py
 Comment: 
 
+Filename: mindnlp/transformers/models/phi3/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/phi3/configuration_phi3.py
+Comment: 
+
+Filename: mindnlp/transformers/models/phi3/modeling_phi3.py
+Comment: 
+
 Filename: mindnlp/transformers/models/pop2piano/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/pop2piano/configuration_pop2piano.py
 Comment: 
 
 Filename: mindnlp/transformers/models/pop2piano/feature_extraction_pop2piano.py
@@ -1782,14 +1872,23 @@
 
 Filename: mindnlp/transformers/models/reformer/tokenization_reformer_fast.py
 Comment: 
 
 Filename: mindnlp/transformers/models/regnet/__init__.py
 Comment: 
 
+Filename: mindnlp/transformers/models/resnet/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/resnet/configuration_resnet.py
+Comment: 
+
+Filename: mindnlp/transformers/models/resnet/modeling_resnet.py
+Comment: 
+
 Filename: mindnlp/transformers/models/roberta/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/roberta/configuration_roberta.py
 Comment: 
 
 Filename: mindnlp/transformers/models/roberta/modeling_graph_roberta.py
@@ -1809,14 +1908,29 @@
 
 Filename: mindnlp/transformers/models/rwkv/configuration_rwkv.py
 Comment: 
 
 Filename: mindnlp/transformers/models/rwkv/modeling_rwkv.py
 Comment: 
 
+Filename: mindnlp/transformers/models/sam/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/sam/configuration_sam.py
+Comment: 
+
+Filename: mindnlp/transformers/models/sam/image_processing_sam.py
+Comment: 
+
+Filename: mindnlp/transformers/models/sam/modeling_sam.py
+Comment: 
+
+Filename: mindnlp/transformers/models/sam/processing_sam.py
+Comment: 
+
 Filename: mindnlp/transformers/models/seamless_m4t/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/seamless_m4t/configuration_seamless_m4t.py
 Comment: 
 
 Filename: mindnlp/transformers/models/seamless_m4t/feature_extraction_seamless_m4t.py
@@ -1839,14 +1953,26 @@
 
 Filename: mindnlp/transformers/models/seamless_m4t_v2/configuration_seamless_m4t_v2.py
 Comment: 
 
 Filename: mindnlp/transformers/models/seamless_m4t_v2/modeling_seamless_m4t_v2.py
 Comment: 
 
+Filename: mindnlp/transformers/models/segformer/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/segformer/configuration_segformer.py
+Comment: 
+
+Filename: mindnlp/transformers/models/segformer/image_processing_segformer.py
+Comment: 
+
+Filename: mindnlp/transformers/models/segformer/modeling_segformer.py
+Comment: 
+
 Filename: mindnlp/transformers/models/starcoder2/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/starcoder2/configuration_starcoder2.py
 Comment: 
 
 Filename: mindnlp/transformers/models/starcoder2/modeling_starcoder2.py
@@ -1872,14 +1998,23 @@
 
 Filename: mindnlp/transformers/models/table_transformer/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/timesformer/__init__.py
 Comment: 
 
+Filename: mindnlp/transformers/models/timesformer/configuration_timesformer.py
+Comment: 
+
+Filename: mindnlp/transformers/models/timesformer/image_processing_videomae.py
+Comment: 
+
+Filename: mindnlp/transformers/models/timesformer/modeling_timesformer.py
+Comment: 
+
 Filename: mindnlp/transformers/models/tinybert/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/tinybert/tinybert.py
 Comment: 
 
 Filename: mindnlp/transformers/models/tinybert/tinybert_config.py
@@ -1890,14 +2025,32 @@
 
 Filename: mindnlp/transformers/models/transformer/transformer.py
 Comment: 
 
 Filename: mindnlp/transformers/models/transformer/transformer_config.py
 Comment: 
 
+Filename: mindnlp/transformers/models/van/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/van/configuration_van.py
+Comment: 
+
+Filename: mindnlp/transformers/models/van/modeling_van.py
+Comment: 
+
+Filename: mindnlp/transformers/models/vipllava/__init__.py
+Comment: 
+
+Filename: mindnlp/transformers/models/vipllava/configuration_vipllava.py
+Comment: 
+
+Filename: mindnlp/transformers/models/vipllava/modeling_vipllava.py
+Comment: 
+
 Filename: mindnlp/transformers/models/wav2vec2/__init__.py
 Comment: 
 
 Filename: mindnlp/transformers/models/wav2vec2/configuration_wav2vec2.py
 Comment: 
 
 Filename: mindnlp/transformers/models/wav2vec2/feature_extraction_wav2vec2.py
@@ -2013,18 +2166,30 @@
 
 Filename: mindnlp/transformers/pipelines/text_generation.py
 Comment: 
 
 Filename: mindnlp/transformers/pipelines/zero_shot_classification.py
 Comment: 
 
-Filename: mindnlp/utils/__init__.py
+Filename: mindnlp/trl/__init__.py
+Comment: 
+
+Filename: mindnlp/trl/core.py
+Comment: 
+
+Filename: mindnlp/trl/environment/__init__.py
+Comment: 
+
+Filename: mindnlp/trl/extras/__init__.py
+Comment: 
+
+Filename: mindnlp/trl/models/__init__.py
 Comment: 
 
-Filename: mindnlp/utils/backbone_utils.py
+Filename: mindnlp/utils/__init__.py
 Comment: 
 
 Filename: mindnlp/utils/compatibility.py
 Comment: 
 
 Filename: mindnlp/utils/decompress.py
 Comment: 
@@ -2094,149 +2259,20 @@
 
 Filename: mindnlp/workflow/works/qa.py
 Comment: 
 
 Filename: mindnlp/workflow/works/sentiment_analysis.py
 Comment: 
 
-Filename: tests/README.md
-Comment: 
-
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/common.py
 Comment: 
 
-Filename: tests/pytest.ini
-Comment: 
-
-Filename: tests/fixtures/add_distilbert_like_config.json
-Comment: 
-
-Filename: tests/fixtures/dummy-config.json
-Comment: 
-
-Filename: tests/fixtures/dummy_feature_extractor_config.json
-Comment: 
-
-Filename: tests/fixtures/empty.txt
-Comment: 
-
-Filename: tests/fixtures/input.txt
-Comment: 
-
-Filename: tests/fixtures/merges.txt
-Comment: 
-
-Filename: tests/fixtures/preprocessor_config.json
-Comment: 
-
-Filename: tests/fixtures/sample_text.txt
-Comment: 
-
-Filename: tests/fixtures/sample_text_no_unicode.txt
-Comment: 
-
-Filename: tests/fixtures/spiece.model
-Comment: 
-
-Filename: tests/fixtures/test_entity_vocab.json
-Comment: 
-
-Filename: tests/fixtures/test_sentencepiece.model
-Comment: 
-
-Filename: tests/fixtures/test_sentencepiece_bpe.model
-Comment: 
-
-Filename: tests/fixtures/test_sentencepiece_bpe_char.model
-Comment: 
-
-Filename: tests/fixtures/test_sentencepiece_no_bos.model
-Comment: 
-
-Filename: tests/fixtures/test_sentencepiece_with_bytefallback.model
-Comment: 
-
-Filename: tests/fixtures/vocab.json
-Comment: 
-
-Filename: tests/fixtures/vocab.txt
-Comment: 
-
-Filename: tests/fixtures/tests_samples/.gitignore
-Comment: 
-
-Filename: tests/fixtures/tests_samples/COCO/000000039769.png
-Comment: 
-
-Filename: tests/fixtures/tests_samples/COCO/coco_annotations.txt
-Comment: 
-
-Filename: tests/fixtures/tests_samples/COCO/coco_panoptic_annotations.txt
-Comment: 
-
-Filename: tests/fixtures/tests_samples/COCO/coco_panoptic/000000039769.png
-Comment: 
-
-Filename: tests/fixtures/tests_samples/GermEval/dev.txt
-Comment: 
-
-Filename: tests/fixtures/tests_samples/GermEval/labels.txt
-Comment: 
-
-Filename: tests/fixtures/tests_samples/GermEval/train.txt
-Comment: 
-
-Filename: tests/fixtures/tests_samples/MRPC/dev.csv
-Comment: 
-
-Filename: tests/fixtures/tests_samples/MRPC/dev.tsv
-Comment: 
-
-Filename: tests/fixtures/tests_samples/MRPC/train.csv
-Comment: 
-
-Filename: tests/fixtures/tests_samples/MRPC/train.tsv
-Comment: 
-
-Filename: tests/fixtures/tests_samples/SQUAD/sample.json
-Comment: 
-
-Filename: tests/fixtures/tests_samples/STS-B/dev.tsv
-Comment: 
-
-Filename: tests/fixtures/tests_samples/STS-B/train.tsv
-Comment: 
-
-Filename: tests/fixtures/tests_samples/conll/sample.json
-Comment: 
-
-Filename: tests/fixtures/tests_samples/swag/sample.json
-Comment: 
-
-Filename: tests/fixtures/tests_samples/wiki_text/wiki_00
-Comment: 
-
-Filename: tests/fixtures/tests_samples/wmt16/sample.json
-Comment: 
-
-Filename: tests/fixtures/tests_samples/wmt_en_ro/test.json
-Comment: 
-
-Filename: tests/fixtures/tests_samples/wmt_en_ro/train.json
-Comment: 
-
-Filename: tests/fixtures/tests_samples/wmt_en_ro/val.json
-Comment: 
-
-Filename: tests/fixtures/tests_samples/xsum/sample.json
-Comment: 
-
 Filename: tests/st/__init__.py
 Comment: 
 
 Filename: tests/st/test_bilstm_imdb.py
 Comment: 
 
 Filename: tests/st/test_longformer.py
@@ -2274,36 +2310,30 @@
 
 Filename: tests/ut/dataset/transforms/test_pad_transform.py
 Comment: 
 
 Filename: tests/ut/engine/__init__.py
 Comment: 
 
-Filename: tests/ut/engine/test_callback.py
-Comment: 
-
-Filename: tests/ut/engine/test_evaluator.py
-Comment: 
-
 Filename: tests/ut/engine/test_trainer.py
 Comment: 
 
 Filename: tests/ut/legacy/__init__.py
 Comment: 
 
 Filename: tests/ut/legacy/test_einsum.py
 Comment: 
 
-Filename: tests/ut/metrics/__init__.py
+Filename: tests/ut/legacy/metrics/__init__.py
 Comment: 
 
-Filename: tests/ut/metrics/test_metrics_class.py
+Filename: tests/ut/legacy/metrics/test_metrics_class.py
 Comment: 
 
-Filename: tests/ut/metrics/test_metrics_fn.py
+Filename: tests/ut/legacy/metrics/test_metrics_fn.py
 Comment: 
 
 Filename: tests/ut/modules/__init__.py
 Comment: 
 
 Filename: tests/ut/modules/test_crf.py
 Comment: 
@@ -2382,35 +2412,29 @@
 
 Filename: tests/ut/peft/__init__.py
 Comment: 
 
 Filename: tests/ut/peft/test_config.py
 Comment: 
 
-Filename: tests/ut/text2vec/__init__.py
-Comment: 
-
-Filename: tests/ut/text2vec/test_sbert_embeddings.py
-Comment: 
-
-Filename: tests/ut/text2vec/test_w2v_embeddings.py
-Comment: 
-
 Filename: tests/ut/transformers/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/test_backbone_common.py
 Comment: 
 
 Filename: tests/ut/transformers/test_configuration_common.py
 Comment: 
 
 Filename: tests/ut/transformers/test_feature_extraction_common.py
 Comment: 
 
+Filename: tests/ut/transformers/test_image_processing_common.py
+Comment: 
+
 Filename: tests/ut/transformers/test_modeling_common.py
 Comment: 
 
 Filename: tests/ut/transformers/test_pipeline_mixin.py
 Comment: 
 
 Filename: tests/ut/transformers/test_sequence_feature_extraction_common.py
@@ -2607,26 +2631,38 @@
 
 Filename: tests/ut/transformers/models/convbert/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/convbert/test_modeling_convbert.py
 Comment: 
 
+Filename: tests/ut/transformers/models/convnext/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/convnext/test_modeling_convnext.py
+Comment: 
+
 Filename: tests/ut/transformers/models/cpmant/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/cpmant/test_modeling_cpmant.py
 Comment: 
 
 Filename: tests/ut/transformers/models/cpmbee/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/cpmbee/test_modeling_cpmbee.py
 Comment: 
 
+Filename: tests/ut/transformers/models/cvt/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/cvt/test_modeling_cvt.py
+Comment: 
+
 Filename: tests/ut/transformers/models/deberta/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/deberta/test_modeling_deberta.py
 Comment: 
 
 Filename: tests/ut/transformers/models/encodec/__init__.py
@@ -2691,15 +2727,15 @@
 
 Filename: tests/ut/transformers/models/gpt_neo/test_gpt_neo.py
 Comment: 
 
 Filename: tests/ut/transformers/models/gpt_neox/__init__.py
 Comment: 
 
-Filename: tests/ut/transformers/models/gpt_neox/test_gpt_neox.py
+Filename: tests/ut/transformers/models/gpt_neox/test_modeling_gpt_neox.py
 Comment: 
 
 Filename: tests/ut/transformers/models/graphormer/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/graphormer/test_graphormer_cells.py
 Comment: 
@@ -2733,14 +2769,29 @@
 
 Filename: tests/ut/transformers/models/llama/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/llama/test_modeling_llama.py
 Comment: 
 
+Filename: tests/ut/transformers/models/llava/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/llava/test_modeling_llava.py
+Comment: 
+
+Filename: tests/ut/transformers/models/llava_next/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/llava_next/test_image_processor_llava_next.py
+Comment: 
+
+Filename: tests/ut/transformers/models/llava_next/test_modeling_llava_next.py
+Comment: 
+
 Filename: tests/ut/transformers/models/longformer/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/longformer/test_modeling_longformer.py
 Comment: 
 
 Filename: tests/ut/transformers/models/luke/__init__.py
@@ -2790,14 +2841,26 @@
 
 Filename: tests/ut/transformers/models/moss/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/moss/test_modeling_moss.py
 Comment: 
 
+Filename: tests/ut/transformers/models/mpnet/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/mpnet/test_modeling_mpnet.py
+Comment: 
+
+Filename: tests/ut/transformers/models/mpt/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/mpt/test_modeling_mpt.py
+Comment: 
+
 Filename: tests/ut/transformers/models/mt5/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/mt5/test_modeling_mt5.py
 Comment: 
 
 Filename: tests/ut/transformers/models/musicgen/__init__.py
@@ -2820,20 +2883,32 @@
 
 Filename: tests/ut/transformers/models/nezha/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/nezha/test_modeling_nezha.py
 Comment: 
 
+Filename: tests/ut/transformers/models/olmo/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/olmo/test_modeling_olmo.py
+Comment: 
+
 Filename: tests/ut/transformers/models/opt/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/opt/test_modeling_opt.py
 Comment: 
 
+Filename: tests/ut/transformers/models/pegasus/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/pegasus/test_modeling_pegasus.py
+Comment: 
+
 Filename: tests/ut/transformers/models/phi/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/phi/test_modeling_phi.py
 Comment: 
 
 Filename: tests/ut/transformers/models/pop2piano/__init__.py
@@ -2856,56 +2931,86 @@
 
 Filename: tests/ut/transformers/models/reformer/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/reformer/test_modeling_reformer.py
 Comment: 
 
+Filename: tests/ut/transformers/models/resnet/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/resnet/test_modeling_resnet.py
+Comment: 
+
 Filename: tests/ut/transformers/models/roberta/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/roberta/test_modeling_roberta.py
 Comment: 
 
 Filename: tests/ut/transformers/models/rwkv/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/rwkv/test_modeling_rwkv.py
 Comment: 
 
+Filename: tests/ut/transformers/models/sam/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/sam/test_modeling_sam.py
+Comment: 
+
 Filename: tests/ut/transformers/models/seamless_m4t/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/seamless_m4t/test_modeling_seamless_m4t.py
 Comment: 
 
 Filename: tests/ut/transformers/models/seamless_m4t_v2/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/seamless_m4t_v2/test_modeling_seamless_m4t_v2.py
 Comment: 
 
+Filename: tests/ut/transformers/models/segformer/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/segformer/test_modeling_segformer.py
+Comment: 
+
 Filename: tests/ut/transformers/models/starcoder2/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/starcoder2/test_modeling_starcoder2.py
 Comment: 
 
 Filename: tests/ut/transformers/models/t5/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/t5/test_modeling_t5.py
 Comment: 
 
+Filename: tests/ut/transformers/models/timesformer/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/timesformer/test_modeling_timesformer.py
+Comment: 
+
 Filename: tests/ut/transformers/models/tinybert/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/tinybert/test_tinybert.py
 Comment: 
 
+Filename: tests/ut/transformers/models/vipllava/__init__.py
+Comment: 
+
+Filename: tests/ut/transformers/models/vipllava/test_modeling_vipllava.py
+Comment: 
+
 Filename: tests/ut/transformers/models/wav2vec2/__init__.py
 Comment: 
 
 Filename: tests/ut/transformers/models/wav2vec2/test_feature_extraction_wav2vec2.py
 Comment: 
 
 Filename: tests/ut/transformers/models/wav2vec2/test_modeling_wav2vec2.py
@@ -2967,41 +3072,38 @@
 
 Filename: tests/ut/transformers/pipelines/test_pipelines_text_generation.py
 Comment: 
 
 Filename: tests/ut/transformers/pipelines/test_pipelines_zero_shot_classification.py
 Comment: 
 
-Filename: tests/ut/utils/test_download.py
-Comment: 
-
 Filename: tests/ut/vocab/__init__.py
 Comment: 
 
 Filename: tests/ut/vocab/test_vocab.py
 Comment: 
 
 Filename: tests/ut/vocab/test_vocab_fasttext.py
 Comment: 
 
 Filename: tests/ut/vocab/test_vocab_glove.py
 Comment: 
 
-Filename: mindnlp-0.2.4.dist-info/LICENSE
+Filename: mindnlp-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: mindnlp-0.2.4.dist-info/METADATA
+Filename: mindnlp-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: mindnlp-0.2.4.dist-info/NOTICE
+Filename: mindnlp-0.3.0.dist-info/NOTICE
 Comment: 
 
-Filename: mindnlp-0.2.4.dist-info/WHEEL
+Filename: mindnlp-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: mindnlp-0.2.4.dist-info/top_level.txt
+Filename: mindnlp-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mindnlp-0.2.4.dist-info/RECORD
+Filename: mindnlp-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mindnlp/configs.py

```diff
@@ -31,17 +31,21 @@
 GENERATION_CONFIG_NAME = "generation_config.json"
 TOKENIZER_CONFIG_FILE = "tokenizer_config.json"
 
 FEATURE_EXTRACTOR_NAME = "preprocessor_config.json"
 IMAGE_PROCESSOR_NAME = FEATURE_EXTRACTOR_NAME
 PROCESSOR_NAME = "processor_config.json"
 
+ADAPTER_CONFIG_NAME = "adapter_config.json"
+ADAPTER_WEIGHTS_NAME = "adapter_model.bin"
+ADAPTER_SAFE_WEIGHTS_NAME = "adapter_model.safetensors"
+
 DEFAULT_ROOT = os.path.join(os.getcwd(), ".mindnlp")
 # for modelscope models
-MS_URL_BASE = "https://modelscope.cn/api/v1/models/mindnlp/{}/repo?Revision=master&FilePath={}"
+MS_URL_BASE = "https://modelscope.cn/api/v1/models/{}/repo?Revision={}&FilePath={}"
 # for huggingface url
 HF_ENDPOINT = os.environ.get('HF_ENDPOINT', 'https://hf-mirror.com')
 HF_URL_BASE = HF_ENDPOINT + '/{}/resolve/{}/{}'
 
 ENV_VARS_TRUE_VALUES = {"1", "ON", "YES", "TRUE"}
 MINDNLP_CACHE = os.getenv("MINDNLP_CACHE", DEFAULT_ROOT)
```

## mindnlp/injection.py

```diff
@@ -8,35 +8,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
+# pylint: disable=no-name-in-module
 """
 Injection mindspore.nn for MindNLP
 """
 import operator
 from typing import OrderedDict
 from functools import reduce, partial
 import math
+import types
 from uuid import uuid4
+import mindspore.experimental
+import mindspore.experimental.optim
 from packaging import version
 
 import numpy as np
 import mindspore
 import mindspore.common.dtype as mstype
+from mindspore._c_expression import Tensor as Tensor_
 from mindspore import nn, ops, Tensor, Parameter
 from mindspore.common._stub_tensor import StubTensor
 from mindspore.nn.layer.conv import _Conv, _deconv_output_length
 from mindspore.common.initializer import initializer, Normal, HeUniform, Uniform, _calculate_fan_in_and_fan_out
 from mindspore import _checkparam as Validator
 from mindspore.ops import functional as F
 from mindspore.ops._primitive_cache import _get_cache_prim
 from mindnlp._legacy.functional import einsum
+from .utils.logging import get_logger
+from .amp import OP_WHITE_LIST, OP_BLACK_LIST, CELL_WHITE_LIST, get_global_amp
 
 LESS_MS_2_1 = version.parse(mindspore.__version__) < version.parse('2.1.0')
 LESS_MS_2_2 = version.parse(mindspore.__version__) < version.parse('2.2.0')
 
 DEVICE_TARGET = mindspore.get_context('device_target')
 GLOBAL_FP16_PATCH = False
 
@@ -144,14 +151,37 @@
     if -1 not in sizes and _sizes_mul != input_shape[_dim]:
         raise ValueError(f"unflatten: Provided `sizes` {sizes} don't multiply up to the"
             f"size of dim {dim} ({input_shape[_dim]}) in the input tensor")
 
     out_shape = input_shape[:_dim] + tuple(sizes) + input_shape[_dim + 1:]
     return out_shape
 
+old_op_call = ops.Primitive.__call__
+def _op_call(self, *args):
+    GLOBAL_AMP, GLOBAL_AMP_DTYPE = get_global_amp()
+
+    if GLOBAL_AMP:
+        if GLOBAL_AMP and self.__class__.__name__ in OP_WHITE_LIST:
+            args = [arg.astype(GLOBAL_AMP_DTYPE) if isinstance(arg, Tensor) \
+                    else arg for arg in args]
+        elif GLOBAL_AMP and self.__class__.__name__ in OP_BLACK_LIST:
+            args = [arg.astype(mindspore.float32) if isinstance(arg, Tensor) \
+                    else arg for arg in args]
+        else:
+            return old_op_call(self, *args)
+
+        outputs = old_op_call(self, *args)
+
+        return outputs
+
+    return old_op_call(self, *args)
+
+
+ops.Primitive.__call__ = _op_call
+
 # For all backend
 # For functional api
 # matmul
 origin_matmul = ops.matmul
 ops.matmul = fp16_patch_decorator(origin_matmul)
 # mm
 ops.mm = fp16_patch_decorator(origin_matmul)
@@ -446,14 +476,20 @@
 if version.parse(mindspore.__version__) < version.parse('2.3.0'):
     def _stride(self):
         strides = self.strides
         return tuple(stride // 4 for stride in strides)
     Tensor.stride = _stride
     StubTensor.stride = _stride
 
+def _ne(self, other):
+    return ops.ne(self, other)
+
+Tensor.__ne__ = _ne
+StubTensor.__ne__ = _ne
+
 # Ascend only
 if DEVICE_TARGET == 'Ascend':
     # cumsum
     ops.cumsum = int32_patch_decorator(ops.cumsum)
     def _cumsum(self, axis):
         return ops.cumsum(self, axis)
     Tensor.cumsum = _cumsum
@@ -892,28 +928,31 @@
     def extend_repr(self):
         return f'num_features={self.num_features}, eps={self.eps}, momentum={1.0 - self.momentum}, ' \
                f'weight={self.weight}, bias={self.bias}, running_mean={self.running_mean}, running_var={self.running_var}'
 
 
 def _half(self):
     """patched nn.Cell.half"""
-    self.to_float(mindspore.float16)
+    # self.to_float(mindspore.float16), fix t5 fp16 inference error
     for _, param in self.parameters_and_names():
         if param.dtype in (mindspore.float16, mindspore.float32, mindspore.bfloat16):
-            param.set_dtype(mindspore.float16)
+            # param.set_dtype(mindspore.float16) # set_dtype is useless if Parameter copied from host to device(just be used).
+            param.set_data(param.astype(mindspore.float16)) # this is a bug that MindSpore just use new pointer of incoming Tensor
+            param.init_data()
     return self
 
 nn.Cell.half = _half
 
 def _float(self):
     """patched nn.Cell.float"""
-    self.to_float(mindspore.float32)
+    # self.to_float(mindspore.float32)
     for _, param in self.parameters_and_names():
         if param.dtype in (mindspore.float16, mindspore.float32, mindspore.bfloat16):
-            param.set_dtype(mindspore.float32)
+            param.set_data(param.astype(mindspore.float32))
+            # param.set_dtype(mindspore.float32)
     return self
 
 nn.Cell.float = _float
 
 
 if not LESS_MS_2_2:
     def _bfloat16(self):
@@ -953,23 +992,79 @@
             if name_prefix:
                 cells_name_prefix = name_prefix + '.' + cells_name_prefix
             for ele in cell.cells_and_names(cells_name_prefix):
                 yield ele
 
 nn.Cell.cells_and_names = _cells_and_names
 
+def _run_forward_hook(self, inputs, output):
+    """
+    Running forward hook function registered on Cell object.
+
+    Args:
+        inputs: The input objects of Cell object.
+        output: The output object of Cell object.
+
+    Returns:
+        - **output** - New output object or none.
+
+    Supported Platforms:
+    ``Ascend`` ``GPU`` ``CPU``
+    """
+    cell_id = self.cls_name + "(" + str(id(self)) + ")"
+    for fn in self._forward_hook.values():
+        ret = fn(self, inputs, output)
+        if ret is not None:
+            output = ret
+    return output
+
+nn.Cell._run_forward_hook = _run_forward_hook
+
+
 def parameters_dict(self, recurse=True):
     """
     fix ignore tied weights
     """
     param_dict = OrderedDict()
     for name, param in self.parameters_and_names(expand=recurse):
         param_dict[name] = param
     return param_dict
 
+
+logger = get_logger()
+def cell_load_state_dict(self, parameter_dict, strict=False):
+    """
+    Load parameters into network, return parameter list that are not loaded in the network.
+    """
+    if not isinstance(parameter_dict, dict):
+        logger.critical("Failed to combine the net and the parameters.")
+        msg = ("For 'load_state_dict', the argument 'parameter_dict' should be a dict, "
+            "but got {}.".format(type(parameter_dict)))
+        raise TypeError(msg)
+
+    for key, value in parameter_dict.items():
+        if not isinstance(key, str) or not isinstance(value, (Parameter, str, list)):
+            logger.critical("Load parameters into net failed.")
+            msg = ("For 'parameter_dict', the element in the argument 'parameter_dict' should be a "
+                "'str' and 'Parameter' , but got {} and {}.".format(type(key), type(value)))
+            raise TypeError(msg)
+
+    param_not_load = []
+    ckpt_not_load = list(parameter_dict.keys())
+    for name, param in self.parameters_and_names():
+        if name in parameter_dict:
+            new_param = parameter_dict[name]
+            param.set_data(new_param)
+            ckpt_not_load.remove(name)
+        else:
+            param_not_load.append(name)
+
+    return param_not_load, ckpt_not_load
+
+nn.Cell.load_state_dict = cell_load_state_dict
 nn.Cell.parameters_dict = parameters_dict
 
 
 nn.LayerNorm = LayerNorm
 nn.Conv1d = Conv1d
 nn.Conv1dTranspose = Conv1dTranspose
 nn.Embedding = Embedding
@@ -1010,7 +1105,96 @@
             x = x.unsqueeze(-1)
         o = super().construct(x)
         if is_3d_tensor:
             o = o.squeeze(-1)
         return o
 
 nn.GroupNorm = GroupNorm_hijack
+
+def state_dict(self):
+    """Returns the state of the scheduler as a :class:`dict`.
+
+    It contains an entry for every variable in self.__dict__ which
+    is not the optimizer.
+    The learning rate lambda functions will only be saved if they are callable objects
+    and not if they are functions or lambdas.
+
+    When saving or loading the scheduler, please make sure to also save or load the state of the optimizer.
+    """
+
+    state_dict = {key: value for key, value in self.__dict__.items() if key not in ('optimizer', 'lr_lambdas')}
+    state_dict['lr_lambdas'] = [None] * len(self.lr_lambdas)
+
+    for idx, fn in enumerate(self.lr_lambdas):
+        if not isinstance(fn, types.FunctionType):
+            state_dict['lr_lambdas'][idx] = fn.__dict__.copy()
+
+    return state_dict
+
+def load_state_dict(self, state_dict):
+    """Loads the schedulers state.
+
+    When saving or loading the scheduler, please make sure to also save or load the state of the optimizer.
+
+    Args:
+        state_dict (dict): scheduler state. Should be an object returned
+            from a call to :meth:`state_dict`.
+    """
+    def assign_scalar_to_tensor(data, saved_data):
+        if isinstance(saved_data, dict):
+            for key, value in saved_data.items():
+                if key in data:
+                    assign_scalar_to_tensor(data[key], value)  # 递归调用以处理嵌套字典
+        elif isinstance(saved_data, list):
+            for i, item in enumerate(saved_data):
+                assign_scalar_to_tensor(data[i], item)  # 递归调用以处理嵌套列表
+        elif isinstance(data, mindspore.Tensor):
+            data.assign_value(Tensor(saved_data))  # 将标量值填充到Tensor中
+
+    lr_lambdas = state_dict.pop('lr_lambdas')
+    assign_scalar_to_tensor(self.__dict__, state_dict)
+    # Restore state_dict keys in order to prevent side effects
+    # https://github.com/pytorch/pytorch/issues/32756
+    state_dict['lr_lambdas'] = lr_lambdas
+
+    for idx, fn in enumerate(lr_lambdas):
+        if fn is not None:
+            self.lr_lambdas[idx].__dict__.update(fn)
+
+mindspore.experimental.optim.lr_scheduler.LambdaLR.state_dict = state_dict
+mindspore.experimental.optim.lr_scheduler.LambdaLR.load_state_dict = load_state_dict
+
+def _str(self):
+    return f'Parameter ({Tensor_.__str__(self)}, ' \
+           f'requires_grad={self.requires_grad})'
+
+Parameter.__str__ = _str
+
+class CustomDropout(nn.Cell):
+    def __init__(self, p=0.5):
+        super(CustomDropout, self).__init__()
+        self.p = p
+
+    def construct(self, x):
+        if not self.training:
+            return x
+        mask = ops.rand_like(x) > self.p
+        return x * mask / (1 - self.p)
+
+nn.Dropout = CustomDropout
+
+def dropout(input, p=0.5, training=True, seed=None):
+    if training is False:
+        return input
+    mask = ops.rand_like(input) > p
+    return input * mask / (1 - p)
+
+ops.dropout = dropout
+
+old_cell_call = nn.Cell.__call__
+def _cell_call(self, *args, **kwargs):
+    GLOBAL_AMP, GLOBAL_AMP_DTYPE = get_global_amp()
+    if GLOBAL_AMP and self.__class__.__name__ in CELL_WHITE_LIST:
+        self.to_float(GLOBAL_AMP_DTYPE)
+    return old_cell_call(self, *args, **kwargs)
+
+nn.Cell.__call__ = old_cell_call
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## mindnlp/_csrc/cuda/flash.cu

```diff
@@ -1,142 +1,824 @@
-// Modified from: https://github.com/tspeterkim/flash-attention-minimal/blob/main/flash.cu  
+// Modified from: https://github.com/tspeterkim/flash-attention-minimal/blob/main/flash.cu
 #include <stdio.h>
 #include <cuda.h>
 #include <cuda_runtime.h>
 
 #define ENABLE_NOTE_LOG 0
 
+__global__ void initArray(float *arr, const int N, const float val)
+{
+    int idx = blockIdx.x * blockDim.x + threadIdx.x;
+    if (idx < N)
+    {
+        arr[idx] = val;
+    }
+}
+
+__global__ void flash_attn_1_fwd_f32_kernel(
+    const float *Q,
+    const float *K,
+    const float *V,
+    const int N,
+    const int d,
+    const int Tc,
+    const int Tr,
+    const int Bc,
+    const int Br,
+    const float softmax_scale,
+    float *l,
+    float *m,
+    float *O)
+{ // 1D-Block and 2D-Grid
+    int tx = threadIdx.x;
+    int bx = blockIdx.x;
+    int by = blockIdx.y; // batch and head index in the grid
+
+    // Offset into Q,K,V,O,l,m - different for each batch and head
+    int qkv_offset = (bx * gridDim.y + by) * N * d; // gridDim.y = nh  qkv dim: (B, nh, N, d)   it equals to (by * gridDim.x + bx) * N * d
+    int lm_offset = (bx * gridDim.y + by) * N;      // offset for l and m  lm dim: (B, nh, N)
+
+    // Define SRAM for Q,K,V,S
+    extern __shared__ float sram[];
+    int tile_size = Bc * d; // size of Qi, Kj, Vj , Bc >= Br, so choose consistent Bc as tile_size
+    float *Qi = sram;
+    float *Kj = &sram[tile_size];
+    float *Vj = &sram[tile_size * 2];
+    float *S = &sram[tile_size * 3];
+
+    for (int j = 0; j < Tc; j++)
+    {
+
+// Load Kj, Vj to SRAM
+#pragma unroll
+        for (int x = 0; x < d; x++) // one block caculates one tile
+        {                           // tx * d indexes the thread, x indexes the element in the vector
+            Kj[(tx * d) + x] = K[qkv_offset + (tile_size * j) + (tx * d) + x];
+            Vj[(tx * d) + x] = V[qkv_offset + (tile_size * j) + (tx * d) + x];
+        }
+        __syncthreads(); // such that the inner loop can use the correct Kj, Vj
+
+#pragma unroll
+        for (int i = 0; i < Tr; i++)
+        {
+
+// Load Qi to SRAM, l and m to registers
+#pragma unroll
+            for (int x = 0; x < d; x++)
+            { // one thread caculates one row of Qi
+                Qi[(tx * d) + x] = Q[qkv_offset + (tile_size * i) + (tx * d) + x];
+            }
+            __syncthreads(); // such that the inner loop can use the correct Qi
+
+            float row_m_prev = m[lm_offset + (Br * i) + tx];
+            float row_l_prev = l[lm_offset + (Br * i) + tx];
+
+            // S = QK^T, row_m = rowmax(S) row-wise
+            // with causal masking
+            float row_m = -INFINITY;
+#pragma unroll
+            for (int y = 0; y < Bc; y++)
+            {
+                float sum = 0;
+#pragma unroll
+                for (int x = 0; x < d; x++)
+                {
+                    sum += Qi[(tx * d) + x] * Kj[(y * d) + x]; // a thread caculates one element of S
+                }
+                sum *= softmax_scale;
+                if (i * Br + tx < j * Bc + y)
+                    sum = -INFINITY;
+                S[(Bc * tx) + y] = sum; // S dim: (Br, Bc)
+
+                if (sum > row_m)
+                    row_m = sum; // every thread hold one row_m
+            }
+
+            // P = exp(S - row_m), row_l = rowsum(P)
+            float row_l = 0;
+#pragma unroll
+            for (int y = 0; y < Bc; y++)
+            {
+                if (i * Br + tx < j * Bc + y)
+                    S[(Bc * tx) + y] = 0;
+                else
+                    S[(Bc * tx) + y] = __expf(S[(Bc * tx) + y] - row_m);
+                row_l += S[(Bc * tx) + y];
+            }
+
+            // Compute new m and l
+            float row_m_new = max(row_m_prev, row_m);
+            float row_l_new = (__expf(row_m_prev - row_m_new) * row_l_prev) +
+                              (__expf(row_m - row_m_new) * row_l);
+
+// Write O, l, m to HBM
+#pragma unroll
+            for (int x = 0; x < d; x++)
+            {
+                float pv = 0; // Pij * Vj
+#pragma unroll
+                for (int y = 0; y < Bc; y++)
+                {
+                    pv += S[(Bc * tx) + y] * Vj[(y * d) + x];
+                }
+                O[qkv_offset + (tile_size * i) + (tx * d) + x] =
+                    (1 / row_l_new) *
+                    ((row_l_prev * __expf(row_m_prev - row_m_new) *
+                      O[qkv_offset + (tile_size * i) + (tx * d) + x]) +
+                     (__expf(row_m - row_m_new) * pv));
+            }
+            m[lm_offset + (Br * i) + tx] = row_m_new;
+            l[lm_offset + (Br * i) + tx] = row_l_new;
+        }
+        __syncthreads(); // otherwise, thread can use the wrong Kj, Vj in inner loop
+    }
+}
+
 __global__ void flash_attn_2_fwd_f32_kernel(
-  const float* Q, 
-  const float* K, 
-  const float* V, 
-  const int N, 
-  const int d,
-  const int Tc,
-  const int Tr, 
-  const int Bc, 
-  const int Br, 
-  const float softmax_scale,
-  float* l, 
-  float *m, 
-  float* O) {
-  int tx = threadIdx.x;
-  int bx = blockIdx.x; int by = blockIdx.y;  // batch and head index
-
-  // Offset into Q,K,V,O,l,m - different for each batch and head
-  int qkv_offset = (bx * gridDim.y * N * d) + (by * N * d);  // gridDim.y = nh
-  int lm_offset = (bx * gridDim.y * N) + (by * N);  // offset for l and m
-
-  // Define SRAM for Q,K,V,S
-  extern __shared__ float sram[];
-  int tile_size = Bc * d;  // size of Qi, Kj, Vj
-  float* Qi = sram;
-  float* Kj = &sram[tile_size];
-  float* Vj = &sram[tile_size * 2];
-  float* S = &sram[tile_size * 3];
-  
-  // TODO: swap the load order of Kj, Vj and Qi. first load Qi, then Kj, Vj
-  for (int j = 0; j < Tc; j++) {
-
-      // Load Kj, Vj to SRAM
-      for (int x = 0; x < d; x++) {
-          Kj[(tx * d) + x] = K[qkv_offset + (tile_size * j) + (tx * d) + x];
-          Vj[(tx * d) + x] = V[qkv_offset + (tile_size * j) + (tx * d) + x];
-      }
-      __syncthreads();  // such that the inner loop can use the correct Kj, Vj
-
-      for (int i = 0; i < Tr; i++)  {
-
-          // Load Qi to SRAM, l and m to registers
-          for (int x = 0; x < d; x++) {
-              Qi[(tx * d) + x] = Q[qkv_offset + (tile_size * i) + (tx * d) + x];
-          }
-          float row_m_prev = m[lm_offset + (Br * i) + tx];
-          float row_l_prev = l[lm_offset + (Br * i) + tx];
-
-          // S = QK^T, row_m = rowmax(S)
-          float row_m = -INFINITY;
-          for (int y = 0; y < Bc; y++) {
-              float sum = 0;
-              for (int x = 0; x < d; x++) {
-                  sum += Qi[(tx * d) + x] * Kj[(y * d) + x];
-              }
-              sum *= softmax_scale;
-              S[(Bc * tx) + y] = sum;
-
-              if (sum > row_m)
-                  row_m = sum;
-          }
-
-          // P = exp(S - row_m), row_l = rowsum(P)
-          float row_l = 0;
-          for (int y = 0; y < Bc; y++) {
-              S[(Bc * tx) + y] = __expf(S[(Bc * tx) + y] - row_m);
-              row_l += S[(Bc * tx) + y];
-          }
-
-          // Compute new m and l
-          float row_m_new = max(row_m_prev, row_m);
-          float row_l_new = (__expf(row_m_prev - row_m_new) * row_l_prev) + (__expf(row_m - row_m_new) * row_l);
-
-          // Write O, l, m to HBM
-          for (int x = 0; x < d; x++) {
-              float pv = 0;  // Pij * Vj
-              for (int y = 0; y < Bc; y++) {
-                  pv += S[(Bc * tx) + y] * Vj[(y * d) + x];
-              }
-              O[qkv_offset + (tile_size * i) + (tx * d) + x] = (1 / row_l_new) \
-                  * ((row_l_prev * __expf(row_m_prev - row_m_new) * O[qkv_offset + (tile_size * i) + (tx * d) + x]) \
-                  + (__expf(row_m - row_m_new) * pv));
-          }
-          m[lm_offset + (Br * i) + tx] = row_m_new;
-          l[lm_offset + (Br * i) + tx] = row_l_new;
-      }
-      __syncthreads();  // otherwise, thread can use the wrong Kj, Vj in inner loop
-  }
+    const float *Q,
+    const float *K,
+    const float *V,
+    const int N,
+    const int d,
+    const int Tc,
+    const int Tr,
+    const int Bc,
+    const int Br,
+    const float softmax_scale,
+    float *L,
+    float *O)
+{
+    int tx = threadIdx.x;
+    int bx = blockIdx.x;
+    int by = blockIdx.y; // batch and head index
+
+    // Offset into Q,K,V,O - different for each batch and head
+    int qkv_offset = (bx * gridDim.y * N * d) + (by * N * d); // gridDim.y = nh
+    int lm_offset = (bx * gridDim.y * N) + (by * N);          // offset for L
+
+    // Define SRAM for Q,K,V,S
+    extern __shared__ float sram[];
+    int tile_size = Bc * d; // size of Qi, Kj, Vj
+    float *Qi = sram;
+    float *Kj = &sram[tile_size];
+    float *Vj = &sram[tile_size * 2];
+    float *S = &sram[tile_size * 3];
+
+    for (int i = 0; i < Tr; ++i)
+    {
+        if (i * Br + tx >= N)
+            break; // break if we are done with the sequence
+
+        // Load Qi from HBM to SRAM, l and m to registers
+        for (int x = 0; x < d; x++)
+        {
+            Qi[(tx * d) + x] = Q[qkv_offset + (tile_size * i) + (tx * d) + x];
+        }
+        float row_m_prev = -INFINITY;
+        float row_l_prev = 0;
+
+        // Causal mask: j <= i
+        for (int j = 0; j <= Tc; ++j)
+        {
+            __syncthreads();
+            // Load Kj, Vj from HBM to SRAM
+            for (int x = 0; x < d; x++)
+            {
+                Kj[(tx * d) + x] = K[qkv_offset + (tile_size * j) + (tx * d) + x];
+                Vj[(tx * d) + x] = V[qkv_offset + (tile_size * j) + (tx * d) + x];
+            }
+            __syncthreads();
+            // S_i^j = softmax_scale * QiKj^T
+            // S_i^j[tx][y] = softmax_scale * Sum_{x = 0}^{d-1} Qi[tx][x] * Kj[y][x]
+            float row_m = -INFINITY;
+            for (int y = 0; y < Bc; y++)
+            {
+                if (j * Bc + y >= N)
+                    break; // break if we are done with the sequence
+                if (i * Br + tx < j * Bc + y)
+                    break;
+                float sum = 0;
+                for (int x = 0; x < d; x++)
+                    sum += Qi[(tx * d) + x] * Kj[(y * d) + x];
+                sum *= softmax_scale;
+                S[(Bc * tx) + y] = sum;
+
+                if (sum > row_m)
+                    row_m = sum;
+            }
+
+            // m_i^j = max(m_i^j-1, row_max(S_i^j))
+            float new_row_m = max(row_m_prev, row_m);
+
+            // P_i^j = exp(S_i^j - m_i^j)
+            // P_i^j[tx][y] = exp(S_i^j[tx][y] - m_i^j)
+            float row_l = 0;
+            for (int y = 0; y < Bc; y++)
+            {
+                if (j * Bc + y >= N)
+                    break; // break if we are done with the sequence
+                if (i * Br + tx < j * Bc + y)
+                    break;
+                S[(Bc * tx) + y] = __expf(S[(Bc * tx) + y] - new_row_m);
+                row_l += S[(Bc * tx) + y];
+            }
+
+            // l_i^j = (exp(m_i^j-1 - m_i^j) * l_i^j-1) + row_sum(P_i^j)
+            float row_m_exp = __expf(row_m_prev - new_row_m);
+            float new_row_l = (row_m_exp * row_l_prev) + row_l;
+
+            // O_i^j = diag(exp(m_i^j-1 - m_i^j))^-1 * O_i^j-1 + P_i^jVj
+            for (int x = 0; x < d; x++)
+            {
+                float pv = 0; // Pij * Vj
+                for (int y = 0; y < Bc; y++)
+                {
+                    if (j * Bc + y >= N)
+                        break; // break if we are done with the sequence
+                    if (i * Br + tx < j * Bc + y)
+                        break;
+                    pv += S[(Bc * tx) + y] * Vj[(y * d) + x];
+                }
+                O[qkv_offset + (tile_size * i) + (tx * d) + x] =
+                    row_m_exp * O[qkv_offset + (tile_size * i) + (tx * d) + x] + pv;
+            }
+
+            // Update m and l
+            row_m_prev = new_row_m;
+            row_l_prev = new_row_l;
+        }
+
+        // O_i = diag(l_i^{Tc})^-1 * O_i^{Tc}
+        for (int x = 0; x < d; x++)
+            O[qkv_offset + (tile_size * i) + (tx * d) + x] /= row_l_prev;
+        // L_i = m_i^{Tc} + log(l_i^{Tc})
+        L[lm_offset + (Br * i) + tx] = row_m_prev + __logf(row_l_prev);
+    }
+}
+
+__global__ void flash_attn_1_bwd_f32_kernel(
+    const float *Q,
+    const float *K,
+    const float *V,
+    const float *O,
+    const float *dO,
+    const float *l,
+    const float *m,
+    const int N,
+    const int d,
+    const int Tc,
+    const int Tr,
+    const int Bc,
+    const int Br,
+    const float softmax_scale,
+    float *dQ,
+    float *dK,
+    float *dV)
+{
+    int tx = threadIdx.x;
+    int bx = blockIdx.x;
+    int by = blockIdx.y; // batch and head index
+
+    // Offset into Q,K,V,O,l,m - different for each batch and head
+    int qkv_offset = (bx * gridDim.y * N * d) + (by * N * d); // gridDim.y = nh
+    int lm_offset = (bx * gridDim.y * N) + (by * N);          // offset for l and m
+
+    // Define SRAM for Q,K,V,S
+    extern __shared__ float sram[];
+    int col_tile_size = Bc * d; // size of Kj, Vj
+    int row_tile_size = Br * d; // size of Qi
+    float *Kj = sram;
+    float *Vj = &sram[col_tile_size];
+
+    float *dKj = &sram[col_tile_size * 2];
+    float *dVj = &sram[col_tile_size * 3];
+
+    float *Qi = &sram[col_tile_size * 4];
+    float *Oi = &sram[col_tile_size * 4 + row_tile_size];
+    float *dOi = &sram[col_tile_size * 4 + row_tile_size * 2];
+
+    // We also use S for P. Likewise, we use dS for dP.
+    // We can reuse the same memory because we don't need S and P at the same time.
+    // We also don't need dS and dP at the same time.
+    float *S = &sram[col_tile_size * 4 + row_tile_size * 3];
+    float *dS = &sram[col_tile_size * 4 + row_tile_size * 3 + Bc * Br];
+
+    for (int j = 0; j < Tc; j++)
+    {
+
+        // Load Kj, Vj to SRAM
+        for (int x = 0; x < d; x++)
+        {
+            Kj[(tx * d) + x] = K[qkv_offset + (col_tile_size * j) + (tx * d) + x];
+            Vj[(tx * d) + x] = V[qkv_offset + (col_tile_size * j) + (tx * d) + x];
+        }
+
+        // Initialize dKj, dVj to 0
+        for (int x = 0; x < d; x++)
+        {
+            dKj[(tx * d) + x] = 0;
+            dVj[(tx * d) + x] = 0;
+        }
+
+        for (int i = j; i < Tr; i++)
+        {
+            __syncthreads();
+            // Load Qi, Oi, dOi, dQi, li, mi to SRAM
+            // Also load l, m to registers
+            for (int x = 0; x < d; x++)
+            {
+                Qi[(tx * d) + x] = Q[qkv_offset + (row_tile_size * i) + (tx * d) + x];
+                Oi[(tx * d) + x] = O[qkv_offset + (row_tile_size * i) + (tx * d) + x];
+                dOi[(tx * d) + x] = dO[qkv_offset + (row_tile_size * i) + (tx * d) + x];
+            }
+            float m_curr = m[lm_offset + (Br * i) + tx];
+            float l_curr = l[lm_offset + (Br * i) + tx];
+
+            // Sij = softmax_scale * QiKj^T
+            // Sij[tx][y] = softmax_scale * Sum_{y = 0}^{Bc-1} Qi[tx][x] * Kj[y][x]
+            for (int y = 0; y < Bc; y++)
+            {
+                float sum = 0;
+                for (int x = 0; x < d; x++)
+                {
+                    sum += Qi[(tx * d) + x] * Kj[(y * d) + x];
+                }
+                sum *= softmax_scale;
+                if (i * Br + tx < j * Bc + y)
+                    sum = -INFINITY;
+                S[(Bc * tx) + y] = sum;
+            }
+
+            // Pij = diag(li)^-1 * exp(Sij - mi)
+            // Pij[tx][y] = (1 / li[tx]) * exp(Sij[tx][y] - mi[tx])
+            for (int y = 0; y < Bc; y++)
+            {
+                if (i * Br + tx < j * Bc + y)
+                    S[(Bc * tx) + y] = 0;
+                else
+                    S[(Bc * tx) + y] = (1 / l_curr) * __expf(S[(Bc * tx) + y] - m_curr);
+            }
+            __syncthreads();
+            // dVj <- dVj + Pij^T * dOi
+            // dVj[tx][x] = dVj[tx][x] + Sum_{y = 0}^{Br-1} Pij[y][tx] * dOi[tx][x]
+            for (int x = 0; x < d; x++)
+            {
+                float sum = 0;
+                for (int y = 0; y < Br; y++)
+                {
+                    sum += S[(Bc * y) + tx] * dOi[(tx * d) + x];
+                }
+                atomicAdd(&dVj[(tx * d) + x], sum);
+            }
+
+            // dPij <- dOi * Vj^T
+            // dPij[tx][y] = Sum_{x = 0}^{d-1} dOi[tx][x] * Vj[y][x]
+            for (int y = 0; y < Bc; y++)
+            {
+                float sum = 0;
+                for (int x = 0; x < d; x++)
+                {
+                    sum += dOi[(tx * d) + x] * Vj[(y * d) + x];
+                }
+                dS[(Bc * tx) + y] = sum;
+            }
+
+            // Di <- rowsum(dOi * Oi)  (pointwise multiply)
+            // Di[tx] = Sum_{x = 0}^{d-1} dOi[tx][x] * Oi[tx][x]
+            float Di = 0;
+            for (int x = 0; x < d; x++)
+            {
+                Di += dOi[(tx * d) + x] * Oi[(tx * d) + x];
+            }
+
+            // dSij <- Pij * (dPij - Di)
+            // dSij[tx][y] = Pij[tx][y] * (dPij[tx][y] - Di[tx])
+            for (int y = 0; y < Bc; ++y)
+            {
+                dS[(Bc * tx) + y] = S[(Bc * tx) + y] * (dS[(Bc * tx) + y] - Di);
+            }
+
+            // dQi <- dQi + softmax_scale * dSijKj
+            // dQ[tx][x] = dQ[tx][x] + softmax_scale * Sum_{y = 0}^{Bc-1} dSij[tx][y] * Kj[y][x]
+            for (int x = 0; x < d; x++)
+            {
+                float sum = 0;
+                for (int y = 0; y < Bc; y++)
+                {
+                    sum += dS[(Bc * tx) + y] * Kj[(y * d) + x];
+                }
+                sum *= softmax_scale;
+                atomicAdd(&dQ[qkv_offset + (row_tile_size * i) + (tx * d) + x], sum);
+            }
+            __syncthreads();
+            // dKj <- dKj + softmax_scale * dSij^TQi
+            // dKj[tx][x] = dKj[tx][x] + softmax_scale * Sum_{y = 0}^{Br-1} dSij[y][tx] * Qi[y][x]
+            for (int x = 0; x < d; x++)
+            {
+                float sum = 0;
+                for (int y = 0; y < Br; y++)
+                {
+                    sum += dS[(Bc * y) + tx] * Qi[(y * d) + x];
+                }
+                sum *= softmax_scale;
+                atomicAdd(&dKj[(tx * d) + x], sum);
+            }
+        }
+
+        // Upload Kj, Vj to HRAM
+        for (int x = 0; x < d; x++)
+        {
+            dK[qkv_offset + (row_tile_size * j) + (tx * d) + x] = dKj[(tx * d) + x];
+            dV[qkv_offset + (row_tile_size * j) + (tx * d) + x] = dVj[(tx * d) + x];
+        }
+    }
 }
 
+__global__ void flash_attn_2_bwd_f32_kernel(
+    const float *Q,
+    const float *K,
+    const float *V,
+    const float *O,
+    const float *dO,
+    const float *L,
+    const int N,
+    const int d,
+    const int Tc,
+    const int Tr,
+    const int Bc,
+    const int Br,
+    const float softmax_scale,
+    float *dQ,
+    float *dK,
+    float *dV)
+{
+    int tx = threadIdx.x;
+    int bx = blockIdx.x;
+    int by = blockIdx.y; // batch and head index
+
+    // Offset into Q,K,V,O - different for each batch and head
+    int qkv_offset = (bx * gridDim.y * N * d) + (by * N * d); // gridDim.y = nh
+    int lm_offset = (bx * gridDim.y * N) + (by * N);          // offset for L
+
+    // Define SRAM for Q,K,V,S
+    extern __shared__ float sram[];
+    int col_tile_size = Bc * d; // size of Kj, Vj
+    int row_tile_size = Br * d; // size of Qi
+    float *Kj = sram;
+    float *Vj = &sram[col_tile_size];
+
+    float *dKj = &sram[col_tile_size * 2];
+    float *dVj = &sram[col_tile_size * 3];
+
+    float *Qi = &sram[col_tile_size * 4];
+    float *Oi = &sram[col_tile_size * 4 + row_tile_size];
+    float *dOi = &sram[col_tile_size * 4 + row_tile_size * 2];
+
+    // We also use S for P. Likewise, we use dS for dP.
+    // We can reuse the same memory because we don't need S and P at the same time.
+    // We also don't need dS and dP at the same time.
+    float *S = &sram[col_tile_size * 4 + row_tile_size * 3];
+    float *dS = &sram[col_tile_size * 4 + row_tile_size * 3 + Bc * Br];
+
+    for (int j = 0; j < Tc; j++)
+    {
+
+        // Load Kj, Vj to SRAM
+        for (int x = 0; x < d; x++)
+        {
+            Kj[(tx * d) + x] = K[qkv_offset + (col_tile_size * j) + (tx * d) + x];
+            Vj[(tx * d) + x] = V[qkv_offset + (col_tile_size * j) + (tx * d) + x];
+        }
+
+        // Initialize dKj, dVj to 0
+        for (int x = 0; x < d; x++)
+        {
+            dKj[(tx * d) + x] = 0;
+            dVj[(tx * d) + x] = 0;
+        }
+
+        for (int i = j; i < Tr; i++)
+        {
+            __syncthreads();
+            // Load Qi, Oi, dOi, dQi, li, mi to SRAM
+            // Also load l, m to registers
+            float Di = 0;
+            for (int x = 0; x < d; x++)
+            {
+                Qi[(tx * d) + x] = Q[qkv_offset + (row_tile_size * i) + (tx * d) + x];
+                Oi[(tx * d) + x] = O[qkv_offset + (row_tile_size * i) + (tx * d) + x];
+                dOi[(tx * d) + x] = dO[qkv_offset + (row_tile_size * i) + (tx * d) + x];
+                Di += dOi[(tx * d) + x] * Oi[(tx * d) + x];
+            }
+            float l_curr = L[lm_offset + (Br * i) + tx];
+
+            // Sij = softmax_scale * QiKj^T
+            // Sij[tx][y] = softmax_scale * Sum_{y = 0}^{Bc-1} Qi[tx][x] * Kj[y][x]
+            for (int y = 0; y < Bc; y++)
+            {
+                float sum = 0;
+                for (int x = 0; x < d; x++)
+                {
+                    sum += Qi[(tx * d) + x] * Kj[(y * d) + x];
+                }
+                sum *= softmax_scale;
+                if (i * Br + tx < j * Bc + y)
+                    sum = -INFINITY;
+                S[(Bc * tx) + y] = sum;
+            }
+
+            // Pij = diag(li)^-1 * exp(Sij - mi)
+            // Pij[tx][y] = (1 / li[tx]) * exp(Sij[tx][y] - mi[tx])
+            for (int y = 0; y < Bc; y++)
+            {
+                if (i * Br + tx < j * Bc + y)
+                    S[(Bc * tx) + y] = 0;
+                else
+                    S[(Bc * tx) + y] = __expf(S[(Bc * tx) + y] - l_curr);
+            }
+            __syncthreads();
+            // dVj <- dVj + Pij^T * dOi
+            // dVj[tx][x] = dVj[tx][x] + Sum_{y = 0}^{Br-1} Pij[y][tx] * dOi[tx][x]
+            for (int x = 0; x < d; x++)
+            {
+                float sum = 0;
+                for (int y = 0; y < Br; y++)
+                {
+                    sum += S[(Bc * y) + tx] * dOi[(tx * d) + x];
+                }
+                atomicAdd(&dVj[(tx * d) + x], sum);
+            }
+
+            // dPij <- dOi * Vj^T
+            // dPij[tx][y] = Sum_{x = 0}^{d-1} dOi[tx][x] * Vj[y][x]
+            for (int y = 0; y < Bc; y++)
+            {
+                float sum = 0;
+                for (int x = 0; x < d; x++)
+                {
+                    sum += dOi[(tx * d) + x] * Vj[(y * d) + x];
+                }
+                dS[(Bc * tx) + y] = sum;
+            }
+
+            // dSij <- Pij * (dPij - Di)
+            // dSij[tx][y] = Pij[tx][y] * (dPij[tx][y] - Di[tx])
+            for (int y = 0; y < Bc; ++y)
+            {
+                dS[(Bc * tx) + y] = S[(Bc * tx) + y] * (dS[(Bc * tx) + y] - Di);
+            }
+
+            // dQi <- dQi + softmax_scale * dSijKj
+            // dQ[tx][x] = dQ[tx][x] + softmax_scale * Sum_{y = 0}^{Bc-1} dSij[tx][y] * Kj[y][x]
+            for (int x = 0; x < d; x++)
+            {
+                float sum = 0;
+                for (int y = 0; y < Bc; y++)
+                {
+                    sum += dS[(Bc * tx) + y] * Kj[(y * d) + x];
+                }
+                sum *= softmax_scale;
+                atomicAdd(&dQ[qkv_offset + (row_tile_size * i) + (tx * d) + x], sum);
+            }
+            __syncthreads();
+            // dKj <- dKj + softmax_scale * dSij^TQi
+            // dKj[tx][x] = dKj[tx][x] + softmax_scale * Sum_{y = 0}^{Br-1} dSij[y][tx] * Qi[y][x]
+            for (int x = 0; x < d; x++)
+            {
+                float sum = 0;
+                for (int y = 0; y < Br; y++)
+                {
+                    sum += dS[(Bc * y) + tx] * Qi[(y * d) + x];
+                }
+                sum *= softmax_scale;
+                atomicAdd(&dKj[(tx * d) + x], sum);
+            }
+        }
+
+        // Upload Kj, Vj to HRAM
+        for (int x = 0; x < d; x++)
+        {
+            dK[qkv_offset + (row_tile_size * j) + (tx * d) + x] = dKj[(tx * d) + x];
+            dV[qkv_offset + (row_tile_size * j) + (tx * d) + x] = dVj[(tx * d) + x];
+        }
+    }
+}
 
-extern "C" {
+extern "C"
+{
 
-    int flash_forward(int nparam, void **params, int *ndims, int64_t **shapes, const char **dtypes, void *stream,
-                    void *extra) {
+    int flash_attn_1_fwd_f32(int nparam, void **params, int *ndims, int64_t **shapes, const char **dtypes, void *stream,
+                             void *extra)
+    {
         cudaStream_t custream = static_cast<cudaStream_t>(stream);
-        if (nparam != 6) return 1;
+        if (nparam != 6)
+            return 1;
         float *Q = static_cast<float *>(params[0]);
         float *K = static_cast<float *>(params[1]);
         float *V = static_cast<float *>(params[2]);
-        // put l,m as input params
-        float *l = static_cast<float *>(params[3]);
-        float *m = static_cast<float *>(params[4]);
-        float *O = static_cast<float *>(params[5]);
+        float *O = static_cast<float *>(params[3]);
+        float *l = static_cast<float *>(params[4]);
+        float *m = static_cast<float *>(params[5]);
 
         const int B = static_cast<int>(shapes[0][0]);
         const int nh = static_cast<int>(shapes[0][1]);
         const int N = static_cast<int>(shapes[0][2]);
         const int d = static_cast<int>(shapes[0][3]);
 
+        // initialize l to 0 and m to -inf
+        cudaMemset(l, 0, B * nh * N * sizeof(float));
+        initArray<<<64, 512>>>(m, B * nh * N, -INFINITY);
+
+        // set block size, TODO: dynamically set block size
+        const int Bc = 32;
+        const int Br = 32;
+        // const int Bc = ceil(max_sram_size / (4 * d * sizeof(float)));
+        // const int Br = min(Bc, d);
+
+        const int Tc = ceil((float)N / Bc);
+        const int Tr = ceil((float)N / Br);
+        const float softmax_scale = 1.0 / sqrt(d);
+
+        // Calculate SRAM size needed per block
+        int col_tile_size = Bc * d; // size of Kj, Vj
+        int row_tile_size = Br * d; // size of Qi
+        const int sram_size =
+            (2 * col_tile_size * sizeof(float)) // SRAM size for Kj, Vj
+            + (row_tile_size * sizeof(float))   // SRAM size for Qi
+            + (Bc * Br * sizeof(float));        // SRAM size for S
         int max_sram_size;
         cudaDeviceGetAttribute(&max_sram_size, cudaDevAttrMaxSharedMemoryPerBlock, 0);
+        printf("Max shared memory: %d, requested shared memory: %d \n", max_sram_size, sram_size);
+
+        dim3 grid_dim(B, nh); // batch_size x num_heads
+        dim3 block_dim(Bc);   // Bc threads per block
+
+        flash_attn_1_fwd_f32_kernel<<<grid_dim, block_dim, sram_size, custream>>>(
+            Q, K, V, N, d, Tc, Tr, Bc, Br, softmax_scale, l, m, O);
+        return 0;
+    }
+}
+
+extern "C"
+{
+
+    int flash_attn_2_fwd_f32(int nparam, void **params, int *ndims, int64_t **shapes, const char **dtypes, void *stream,
+                             void *extra)
+    {
+        cudaStream_t custream = static_cast<cudaStream_t>(stream);
+        if (nparam != 5)
+            return 1;
+        float *Q = static_cast<float *>(params[0]);
+        float *K = static_cast<float *>(params[1]);
+        float *V = static_cast<float *>(params[2]);
+        float *O = static_cast<float *>(params[3]);
+        float *L = static_cast<float *>(params[4]);
+
+        const int B = static_cast<int>(shapes[0][0]);
+        const int nh = static_cast<int>(shapes[0][1]);
+        const int N = static_cast<int>(shapes[0][2]);
+        const int d = static_cast<int>(shapes[0][3]);
 
         // set block size, TODO: dynamically set block size
         const int Bc = 32;
         const int Br = 32;
 
-        const int Tc = ceil((float) N / Bc);
-        const int Tr = ceil((float) N / Br);
+        // Calculate SRAM size needed per block
+        int col_tile_size = Bc * d; // size of Kj, Vj
+        int row_tile_size = Br * d; // size of Qi
+        const int sram_size =
+            (2 * col_tile_size * sizeof(float)) // SRAM size for Kj, Vj
+            + (row_tile_size * sizeof(float))   // SRAM size for Qi
+            + (Bc * Br * sizeof(float));        // SRAM size for S
+        int max_sram_size;
+        cudaDeviceGetAttribute(&max_sram_size, cudaDevAttrMaxSharedMemoryPerBlock, 0);
+
+        const int Tc = ceil((float)N / Bc);
+        const int Tr = ceil((float)N / Br);
         const float softmax_scale = 1.0 / sqrt(d);
 
-        // Calculate SRAM size needed per block
-        const int sram_size = (2 * Bc * d * sizeof(float)) + (4 * Br * d * sizeof(float));
         printf("Bc: %d, Br: %d, Tc: %d, Tr: %d \n", Bc, Br, Tc, Tr);
         printf("Max shared memory: %d, requested shared memory: %d \n", max_sram_size, sram_size);
 
-        dim3 grid_dim(B, nh);  // batch_size x num_heads
-        dim3 block_dim(Bc);  // Bc threads per block
+        dim3 grid_dim(B, nh); // batch_size x num_heads
+        dim3 block_dim(Bc);   // Bc threads per block
 
         flash_attn_2_fwd_f32_kernel<<<grid_dim, block_dim, sram_size, custream>>>(
-            Q, K, V, N, d, Tc, Tr, Bc, Br, softmax_scale, l, m, O
-        );
+            Q, K, V, N, d, Tc, Tr, Bc, Br, softmax_scale, L, O);
+        return 0;
+    }
+}
+
+extern "C"
+{
+    int flash_attn_1_bwd_f32(int nparam, void **params, int *ndims, int64_t **shapes, const char **dtypes, void *stream,
+                             void *extra)
+    {
+        cudaStream_t custream = static_cast<cudaStream_t>(stream);
+        if (nparam != 10)
+            return 1;
+        float *Q = static_cast<float *>(params[0]);
+        float *K = static_cast<float *>(params[1]);
+        float *V = static_cast<float *>(params[2]);
+        float *O = static_cast<float *>(params[3]);
+        float *dO = static_cast<float *>(params[4]);
+        float *l = static_cast<float *>(params[5]);
+        float *m = static_cast<float *>(params[6]);
+        float *dQ = static_cast<float *>(params[7]);
+        float *dK = static_cast<float *>(params[8]);
+        float *dV = static_cast<float *>(params[9]);
+
+        const int B = static_cast<int>(shapes[0][0]);
+        const int nh = static_cast<int>(shapes[0][1]);
+        const int N = static_cast<int>(shapes[0][2]);
+        const int d = static_cast<int>(shapes[0][3]);
+
+        cudaMemset(dQ, 0, B * nh * N * d * sizeof(float));
+        cudaMemset(dK, 0, B * nh * N * d * sizeof(float));
+        cudaMemset(dV, 0, B * nh * N * d * sizeof(float));
+
+        // set block size, TODO: dynamically set block size
+        const int Bc = 16;
+        const int Br = 16;
+
+        // Calculate SRAM size needed per block
+        int col_tile_size = Bc * d; // size of Kj, Vj
+        int row_tile_size = Br * d; // size of Qi
+        const int sram_size =
+            (4 * col_tile_size * sizeof(float))   // SRAM size for Kj, Vj
+            + (3 * row_tile_size * sizeof(float)) // SRAM size for Qi
+            + (2 * Bc * Br * sizeof(float));      // SRAM size for S
+        int max_sram_size;
+        cudaDeviceGetAttribute(&max_sram_size, cudaDevAttrMaxSharedMemoryPerBlock, 0);
+
+        const int Tc = ceil((float)N / Bc);
+        const int Tr = ceil((float)N / Br);
+        const float softmax_scale = 1.0 / sqrt(d);
+
+        printf("Bc: %d, Br: %d, Tc: %d, Tr: %d \n", Bc, Br, Tc, Tr);
+        printf("Max shared memory: %d, requested shared memory: %d \n", max_sram_size, sram_size);
+
+        dim3 grid_dim(B, nh); // batch_size x num_heads
+        dim3 block_dim(Bc);   // Bc threads per block
+
+        flash_attn_1_bwd_f32_kernel<<<grid_dim, block_dim, sram_size, custream>>>(
+            Q, K, V, O, dO, l, m, N, d, Tc, Tr, Bc, Br, softmax_scale, dQ, dK, dV);
+        return 0;
+    }
+}
+
+extern "C"
+{
+    int flash_attn_2_bwd_f32(int nparam, void **params, int *ndims, int64_t **shapes, const char **dtypes, void *stream,
+                             void *extra)
+    {
+        cudaStream_t custream = static_cast<cudaStream_t>(stream);
+        if (nparam != 9)
+            return 1;
+        float *Q = static_cast<float *>(params[0]);
+        float *K = static_cast<float *>(params[1]);
+        float *V = static_cast<float *>(params[2]);
+        float *O = static_cast<float *>(params[3]);
+        float *dO = static_cast<float *>(params[4]);
+        float *L = static_cast<float *>(params[5]);
+        float *dQ = static_cast<float *>(params[6]);
+        float *dK = static_cast<float *>(params[7]);
+        float *dV = static_cast<float *>(params[8]);
+
+        const int B = static_cast<int>(shapes[0][0]);
+        const int nh = static_cast<int>(shapes[0][1]);
+        const int N = static_cast<int>(shapes[0][2]);
+        const int d = static_cast<int>(shapes[0][3]);
+
+        cudaMemset(dQ, 0, B * nh * N * d * sizeof(float));
+        cudaMemset(dK, 0, B * nh * N * d * sizeof(float));
+        cudaMemset(dV, 0, B * nh * N * d * sizeof(float));
+
+        // set block size, TODO: dynamically set block size
+        const int Bc = 16;
+        const int Br = 16;
+
+        // Calculate SRAM size needed per block
+        int col_tile_size = Bc * d; // size of Kj, Vj
+        int row_tile_size = Br * d; // size of Qi
+        const int sram_size =
+            (4 * col_tile_size * sizeof(float))   // SRAM size for Kj, Vj
+            + (3 * row_tile_size * sizeof(float)) // SRAM size for Qi
+            + (2 * Bc * Br * sizeof(float));      // SRAM size for S
+        int max_sram_size;
+        cudaDeviceGetAttribute(&max_sram_size, cudaDevAttrMaxSharedMemoryPerBlock, 0);
+
+        const int Tc = ceil((float)N / Bc);
+        const int Tr = ceil((float)N / Br);
+        const float softmax_scale = 1.0 / sqrt(d);
+
+        printf("Bc: %d, Br: %d, Tc: %d, Tr: %d \n", Bc, Br, Tc, Tr);
+        printf("Max shared memory: %d, requested shared memory: %d \n", max_sram_size, sram_size);
+
+        dim3 grid_dim(B, nh); // batch_size x num_heads
+        dim3 block_dim(Bc);   // Bc threads per block
+
+        flash_attn_2_bwd_f32_kernel<<<grid_dim, block_dim, sram_size, custream>>>(
+            Q, K, V, O, dO, L, N, d, Tc, Tr, Bc, Br, softmax_scale, dQ, dK, dV);
         return 0;
     }
 }
```

## mindnlp/_legacy/functional.py

```diff
@@ -261,15 +261,15 @@
     else:
         b_q, b_k, b_v = ops.split(b, output_num=3)
     return linear(q, w_q, b_q), linear(k, w_k, b_k), linear(v, w_v, b_v)
 
 
 def _scaled_dot_product_attention(query, key, value, attn_mask, dropout_p, is_causal, is_training):
     embed_size = query.shape[-1]
-    scaling_factor = sqrt(Tensor(embed_size, dtype=query.dtype))
+    scaling_factor = sqrt(sqrt(Tensor(embed_size, dtype=query.dtype)))
     query = query / scaling_factor
 
     if is_causal:
         L = query.shape[-2], S = key.shape[-2]
         attn_mask = ops.ones((L, S), mindspore.bool_).tril()
 
     attn = ops.matmul(query, key.swapaxes(-2, -1) / scaling_factor)
```

## mindnlp/abc/container.py

```diff
@@ -14,16 +14,16 @@
 # ============================================================================
 """Customized mindspore.nn.Cell Dict."""
 
 from __future__ import absolute_import
 from typing import Dict
 from collections import OrderedDict, abc as container_abcs
 from mindspore.nn.cell import Cell
-
-__all__ = ['CellDict']
+from mindspore import Parameter
+__all__ = ['CellDict','ParameterDict']
 
 def _valid_index(cell_num, index, op_name=None):
     """Internal function, used to detect the value and type of index."""
     msg_prefix = f"For '{op_name}', the" if op_name else "The"
     if not isinstance(index, int):
         raise TypeError(f"{msg_prefix} type of 'index' must be int, but got {type(index).__name__}.")
     if not -cell_num <= index < cell_num:
@@ -156,7 +156,77 @@
     def set_grad(self, flag=True):
         self.requires_grad = flag
         for cell in self._cells.values():
             cell.set_grad(flag)
 
     def construct(self, *inputs):
         raise NotImplementedError
+
+class ParameterDict(Cell):
+    _params: Dict[str, Parameter]
+
+    def __init__(self, parameters: Dict[str, Parameter] = None):
+        super(ParameterDict, self).__init__()
+        if parameters is not None:
+            self.update(parameters)
+
+    def __getitem__(self, key):
+        return self._params[key]
+
+    def __setitem__(self, key, parameter):
+        self.insert_param_to_cell(key, parameter)
+
+    def __delitem__(self, key):
+        del self._params[key]
+
+    def __len__(self):
+        return len(self._params)
+
+    def __iter__(self):
+        return iter(self._params.keys())
+
+    def __contains__(self, key):
+        return key in self._params
+
+    def clear(self):
+        self._params.clear()
+
+    def pop(self, key):
+        v = self[key]
+        del self[key]
+        return v
+
+    def keys(self):
+        return self._params.keys()
+
+    def items(self):
+        return self._params.items()
+
+    def values(self):
+        r"""Return an iterable of the ParameterDict values.
+        """
+        return self._params.values()
+
+    def update(self, parameters):
+        if not isinstance(parameters, container_abcs.Iterable):
+            raise TypeError("ParametersDict.update should be called with an "
+                            "iterable of key/value pairs, but got " +
+                            type(parameters).__name__)
+
+        if isinstance(parameters, container_abcs.Mapping):
+            if isinstance(parameters, (OrderedDict, ParameterDict)):
+                for key, parameter in parameters.items():
+                    self[key] = parameter
+            else:
+                for key, parameter in sorted(parameters.items()):
+                    self[key] = parameter
+        else:
+            for j, p in enumerate(parameters):
+                if not isinstance(p, container_abcs.Iterable):
+                    raise TypeError("ParameterDict update sequence element "
+                                    "#" + str(j) + " should be Iterable; is" +
+                                    type(p).__name__)
+                if not len(p) == 2:
+                    raise ValueError("ParameterDict update sequence element "
+                                     "#" + str(j) + " has length " + str(len(p)) +
+                                     "; 2 is required")
+                self[p[0]] = p[1]
```

## mindnlp/dataset/__init__.py

```diff
@@ -13,7 +13,8 @@
 # limitations under the License.
 # ============================================================================
 """
 Dataset init
 """
 
 from .load import load_dataset
+from .map_fn import BaseMapFuction
```

## mindnlp/engine/__init__.py

```diff
@@ -12,10 +12,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 
 """
 Engine of text.
 """
-from .trainer import Trainer
-from .evaluator import Evaluator
+from .trainer import *
+from .train_args import *
+from .utils import *
 from .callbacks import *
```

## mindnlp/engine/utils.py

```diff
@@ -11,24 +11,489 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 Utils for engine
 """
+import os
+import re
 import random
+import functools
+import inspect
+import time
+from dataclasses import dataclass
+from typing import Union, Tuple, Optional, NamedTuple, List, Dict, Any
+from collections.abc import Mapping
+
+import mindspore.experimental
 import numpy as np
+import mindspore
+from mindspore import ops
+
+from mindnlp.utils import is_mindspore_available, ExplicitEnum
+
+
+PREFIX_CHECKPOINT_DIR = "checkpoint"
+_re_checkpoint = re.compile(r"^" + PREFIX_CHECKPOINT_DIR + r"\-(\d+)$")
+
+class EvalPrediction:
+    """
+    Evaluation output (always contains labels), to be used to compute metrics.
+
+    Parameters:
+        predictions (`np.ndarray`): Predictions of the model.
+        label_ids (`np.ndarray`): Targets to be matched.
+        inputs (`np.ndarray`, *optional*):
+    """
+
+    def __init__(
+        self,
+        predictions: Union[np.ndarray, Tuple[np.ndarray]],
+        label_ids: Union[np.ndarray, Tuple[np.ndarray]],
+        inputs: Optional[Union[np.ndarray, Tuple[np.ndarray]]] = None,
+    ):
+        self.predictions = predictions
+        self.label_ids = label_ids
+        self.inputs = inputs
+
+    def __iter__(self):
+        if self.inputs is not None:
+            return iter((self.predictions, self.label_ids, self.inputs))
+        else:
+            return iter((self.predictions, self.label_ids))
+
+    def __getitem__(self, idx):
+        if idx < 0 or idx > 2:
+            raise IndexError("tuple index out of range")
+        if idx == 2 and self.inputs is None:
+            raise IndexError("tuple index out of range")
+        if idx == 0:
+            return self.predictions
+        elif idx == 1:
+            return self.label_ids
+        elif idx == 2:
+            return self.inputs
+
+class IntervalStrategy(ExplicitEnum):
+    NO = "no"
+    STEPS = "steps"
+    EPOCH = "epoch"
+
+
+class EvaluationStrategy(ExplicitEnum):
+    NO = "no"
+    STEPS = "steps"
+    EPOCH = "epoch"
+
+
+
+class HubStrategy(ExplicitEnum):
+    END = "end"
+    EVERY_SAVE = "every_save"
+    CHECKPOINT = "checkpoint"
+    ALL_CHECKPOINTS = "all_checkpoints"
+
+
+class BestRun(NamedTuple):
+    """
+    The best run found by a hyperparameter search (see [`~Trainer.hyperparameter_search`]).
+
+    Parameters:
+        run_id (`str`):
+            The id of the best run (if models were saved, the corresponding checkpoint will be in the folder ending
+            with run-{run_id}).
+        objective (`float`):
+            The objective that was obtained for this run.
+        hyperparameters (`Dict[str, Any]`):
+            The hyperparameters picked to get this run.
+        run_summary (`Optional[Any]`):
+            A summary of tuning experiments. `ray.tune.ExperimentAnalysis` object for Ray backend.
+    """
+
+    run_id: str
+    objective: Union[float, List[float]]
+    hyperparameters: Dict[str, Any]
+    run_summary: Optional[Any] = None
+
+def has_length(dataset):
+    """
+    Checks if the dataset implements __len__() and it doesn't raise an error
+    """
+    try:
+        return len(dataset) is not None
+    except TypeError:
+        # TypeError: len() of unsized object
+        return False
 
-from mindnlp.utils import is_mindspore_available
 
 def set_seed(seed: int):
     """
     Helper function for reproducible behavior to set the seed in `random`, `numpy`, `torch` and/or `tf` (if installed).
 
     Args:
         seed (`int`): The seed to set.
     """
     random.seed(seed)
     np.random.seed(seed)
     if is_mindspore_available():
-        import mindspore
         mindspore.set_seed(seed)
+
+def enable_full_determinism(seed: int, warn_only: bool = False):
+    """
+    Helper function for reproducible behavior during distributed training. See
+    - https://pytorch.org/docs/stable/notes/randomness.html for pytorch
+    - https://www.tensorflow.org/api_docs/python/tf/config/experimental/enable_op_determinism for tensorflow
+    """
+    # set seed first
+    set_seed(seed)
+
+    if is_mindspore_available():
+        mindspore.set_context(deterministic='ON')
+
+@dataclass
+class LabelSmoother:
+    """
+    Adds label-smoothing on a pre-computed output from a Transformers model.
+
+    Args:
+        epsilon (`float`, *optional*, defaults to 0.1):
+            The label smoothing factor.
+        ignore_index (`int`, *optional*, defaults to -100):
+            The index in the labels to ignore when computing the loss.
+    """
+
+    epsilon: float = 0.1
+    ignore_index: int = -100
+
+    def __call__(self, model_output, labels, shift_labels=False):
+        logits = model_output["logits"] if isinstance(model_output, dict) else model_output[0]
+        if shift_labels:
+            logits = logits[..., :-1, :]
+            labels = labels[..., 1:]
+
+        log_probs = -ops.log_softmax(logits, axis=-1)
+        if labels.ndim == log_probs.ndim - 1:
+            labels = labels.unsqueeze(-1)
+
+        padding_mask = labels.eq(self.ignore_index)
+        # In case the ignore_index is -100, the gather will fail, so we replace labels by 0. The padding_mask
+        # will ignore them in any case.
+        labels = ops.clamp(labels, min=0)
+        nll_loss = log_probs.gather_elements(dim=-1, index=labels)
+        # works for fp16 input tensor too, by internally upcasting it to fp32
+        smoothed_loss = log_probs.sum(axis=-1, keep_dims=True, dtype=mindspore.float32)
+
+        nll_loss = nll_loss.masked_fill(padding_mask, 0.0)
+        smoothed_loss = smoothed_loss.masked_fill(padding_mask, 0.0)
+
+        # Take the mean over the label dimensions, then divide by the number of active elements (i.e. not-padded):
+        num_active_elements = padding_mask.numel() - padding_mask.long().sum()
+        nll_loss = nll_loss.sum() / num_active_elements
+        smoothed_loss = smoothed_loss.sum() / (num_active_elements * log_probs.shape[-1])
+        return (1 - self.epsilon) * nll_loss + self.epsilon * smoothed_loss
+
+def number_of_arguments(func):
+    """
+    Return the number of arguments of the passed function, even if it's a partial function.
+    """
+    if isinstance(func, functools.partial):
+        total_args = len(inspect.signature(func.func).parameters)
+        return total_args - len(func.args) - len(func.keywords)
+    return len(inspect.signature(func).parameters)
+
+class EvalLoopOutput(NamedTuple):
+    predictions: Union[np.ndarray, Tuple[np.ndarray]]
+    label_ids: Optional[Union[np.ndarray, Tuple[np.ndarray]]]
+    metrics: Optional[Dict[str, float]]
+    num_samples: Optional[int]
+
+
+class PredictionOutput(NamedTuple):
+    predictions: Union[np.ndarray, Tuple[np.ndarray]]
+    label_ids: Optional[Union[np.ndarray, Tuple[np.ndarray]]]
+    metrics: Optional[Dict[str, float]]
+
+
+class TrainOutput(NamedTuple):
+    global_step: int
+    training_loss: float
+    metrics: Dict[str, float]
+
+
+PREFIX_CHECKPOINT_DIR = "checkpoint"
+_re_checkpoint = re.compile(r"^" + PREFIX_CHECKPOINT_DIR + r"\-(\d+)$")
+
+def get_last_checkpoint(folder):
+    content = os.listdir(folder)
+    checkpoints = [
+        path
+        for path in content
+        if _re_checkpoint.search(path) is not None and os.path.isdir(os.path.join(folder, path))
+    ]
+    if len(checkpoints) == 0:
+        return
+    return os.path.join(folder, max(checkpoints, key=lambda x: int(_re_checkpoint.search(x).groups()[0])))
+
+def find_executable_batch_size(
+    function: callable = None, starting_batch_size: int = 128, auto_find_batch_size: bool = False
+):
+    """
+    Args:
+    A basic decorator that will try to execute `function`. If it fails from exceptions related to out-of-memory or
+    CUDNN, the batch size is cut in half and passed to `function`. `function` must take in a `batch_size` parameter as
+    its first argument.
+        function (`callable`, *optional*)
+            A function to wrap
+        starting_batch_size (`int`, *optional*)
+            The batch size to try and fit into memory
+        auto_find_batch_size (`bool`, *optional*)
+            If False, will just execute `function`
+    """
+    if function is None:
+        return functools.partial(
+            find_executable_batch_size,
+            starting_batch_size=starting_batch_size,
+            auto_find_batch_size=auto_find_batch_size,
+        )
+
+    return functools.partial(function, batch_size=starting_batch_size)
+
+class SchedulerType(ExplicitEnum):
+    LINEAR = "linear"
+    COSINE = "cosine"
+    COSINE_WITH_RESTARTS = "cosine_with_restarts"
+    POLYNOMIAL = "polynomial"
+    CONSTANT = "constant"
+    CONSTANT_WITH_WARMUP = "constant_with_warmup"
+    INVERSE_SQRT = "inverse_sqrt"
+    REDUCE_ON_PLATEAU = "reduce_lr_on_plateau"
+    COSINE_WITH_MIN_LR = "cosine_with_min_lr"
+
+
+def get_parameter_names(model, forbidden_layer_types):
+    """
+    Returns the names of the model parameters that are not inside a forbidden layer.
+    """
+    result = []
+    for name, child in model.name_cells().items():
+        result += [
+            f"{name}.{n}"
+            for n in get_parameter_names(child, forbidden_layer_types)
+            if not isinstance(child, tuple(forbidden_layer_types))
+        ]
+    # Add model specific parameters (defined with nn.Parameter) since they are not in any child.
+    result += list(model._params.keys())
+    return result
+
+def get_model_param_count(model, trainable_only=False):
+    """
+    Calculate model's total param count. If trainable_only is True then count only those requiring grads
+    """
+    return sum(p.numel() for p in model.get_parameters() if not trainable_only or p.requires_grad)
+
+def speed_metrics(split, start_time, num_samples=None, num_steps=None, num_tokens=None):
+    """
+    Measure and return speed performance metrics.
+
+    This function requires a time snapshot `start_time` before the operation to be measured starts and this function
+    should be run immediately after the operation to be measured has completed.
+
+    Args:
+    - split: name to prefix metric (like train, eval, test...)
+    - start_time: operation start time
+    - num_samples: number of samples processed
+    - num_steps: number of steps processed
+    - num_tokens: number of tokens processed
+    """
+    runtime = time.time() - start_time
+    result = {f"{split}_runtime": round(runtime, 4)}
+    if runtime == 0:
+        return result
+    if num_samples is not None:
+        samples_per_second = num_samples / runtime
+        result[f"{split}_samples_per_second"] = round(samples_per_second, 3)
+    if num_steps is not None:
+        steps_per_second = num_steps / runtime
+        result[f"{split}_steps_per_second"] = round(steps_per_second, 3)
+    if num_tokens is not None:
+        tokens_per_second = num_tokens / runtime
+        result[f"{split}_tokens_per_second"] = round(tokens_per_second, 3)
+    return result
+
+def _get_learning_rate(self):
+    if isinstance(self.lr_scheduler, mindspore.experimental.optim.lr_scheduler.ReduceLROnPlateau):
+        last_lr = self.optimizer.param_groups[0]["lr"]
+    else:
+        last_lr = self.lr_scheduler.get_last_lr()[0]
+    if ops.is_tensor(last_lr):
+        last_lr = last_lr.item()
+    return last_lr
+
+def find_batch_size(tensors):
+    """
+    Find the first dimension of a tensor in a nested list/tuple/dict of tensors.
+    """
+    if isinstance(tensors, (list, tuple)):
+        for t in tensors:
+            result = find_batch_size(t)
+            if result is not None:
+                return result
+    elif isinstance(tensors, Mapping):
+        for key, value in tensors.items():
+            result = find_batch_size(value)
+            if result is not None:
+                return result
+    elif isinstance(tensors, mindspore.Tensor):
+        return tensors.shape[0] if len(tensors.shape) >= 1 else None
+    elif isinstance(tensors, np.ndarray):
+        return tensors.shape[0] if len(tensors.shape) >= 1 else None
+
+def denumpify_detensorize(metrics):
+    """
+    Recursively calls `.item()` on the element of the dictionary passed
+    """
+    if isinstance(metrics, (list, tuple)):
+        return type(metrics)(denumpify_detensorize(m) for m in metrics)
+    elif isinstance(metrics, dict):
+        return type(metrics)({k: denumpify_detensorize(v) for k, v in metrics.items()})
+    elif isinstance(metrics, np.generic):
+        return metrics.item()
+    elif is_mindspore_available() and isinstance(metrics, mindspore.Tensor) and metrics.numel() == 1:
+        return metrics.item()
+    return metrics
+
+def convert_tensor_to_scalar(data):
+    if isinstance(data, dict):
+        for key, value in data.items():
+            data[key] = convert_tensor_to_scalar(value)  # 递归调用以处理嵌套字典
+    elif isinstance(data, list):
+        for i, item in enumerate(data):
+            data[i] = convert_tensor_to_scalar(item)  # 递归调用以处理嵌套列表
+    elif isinstance(data, mindspore.Tensor):
+        data = data.item()  # 转换为标量值
+    return data
+
+
+def atleast_1d(tensor_or_array: Union[mindspore.Tensor, np.ndarray]):
+    if isinstance(tensor_or_array, mindspore.Tensor):
+        if hasattr(mindspore.ops, "atleast_1d"):
+            tensor_or_array = ops.atleast_1d(tensor_or_array)
+        elif tensor_or_array.ndim < 1:
+            tensor_or_array = tensor_or_array[None]
+    else:
+        tensor_or_array = np.atleast_1d(tensor_or_array)
+    return tensor_or_array
+
+def ms_pad_and_concatenate(tensor1, tensor2, padding_index=-100):
+    """Concatenates `tensor1` and `tensor2` on first axis, applying padding on the second if necessary."""
+    tensor1 = atleast_1d(tensor1)
+    tensor2 = atleast_1d(tensor2)
+
+    if len(tensor1.shape) == 1 or tensor1.shape[1] == tensor2.shape[1]:
+        return ops.cat((tensor1, tensor2), axis=0)
+
+    # Let's figure out the new shape
+    new_shape = (tensor1.shape[0] + tensor2.shape[0], max(tensor1.shape[1], tensor2.shape[1])) + tensor1.shape[2:]
+
+    # Now let's fill the result tensor
+    result = tensor1.new_full(new_shape, padding_index)
+    result[: tensor1.shape[0], : tensor1.shape[1]] = tensor1
+    result[tensor1.shape[0] :, : tensor2.shape[1]] = tensor2
+    return result
+
+def numpy_pad_and_concatenate(array1, array2, padding_index=-100):
+    """Concatenates `array1` and `array2` on first axis, applying padding on the second if necessary."""
+    array1 = atleast_1d(array1)
+    array2 = atleast_1d(array2)
+
+    if len(array1.shape) == 1 or array1.shape[1] == array2.shape[1]:
+        return np.concatenate((array1, array2), axis=0)
+
+    # Let's figure out the new shape
+    new_shape = (array1.shape[0] + array2.shape[0], max(array1.shape[1], array2.shape[1])) + array1.shape[2:]
+
+    # Now let's fill the result tensor
+    result = np.full_like(array1, padding_index, shape=new_shape)
+    result[: array1.shape[0], : array1.shape[1]] = array1
+    result[array1.shape[0] :, : array2.shape[1]] = array2
+    return result
+
+
+def nested_concat(tensors, new_tensors, padding_index=-100):
+    """
+    Concat the `new_tensors` to `tensors` on the first dim and pad them on the second if needed. Works for tensors or
+    nested list/tuples/dict of tensors.
+    """
+    # assert type(tensors) == type(
+    #     new_tensors
+    # ), f"Expected `tensors` and `new_tensors` to have the same type but found {type(tensors)} and {type(new_tensors)}."
+    if isinstance(tensors, (list, tuple)):
+        return type(tensors)(nested_concat(t, n, padding_index=padding_index) for t, n in zip(tensors, new_tensors))
+    elif isinstance(tensors, mindspore.Tensor):
+        return ms_pad_and_concatenate(tensors, new_tensors, padding_index=padding_index)
+    elif isinstance(tensors, Mapping):
+        return type(tensors)(
+            {k: nested_concat(t, new_tensors[k], padding_index=padding_index) for k, t in tensors.items()}
+        )
+    elif isinstance(tensors, np.ndarray):
+        return numpy_pad_and_concatenate(tensors, new_tensors, padding_index=padding_index)
+    else:
+        raise TypeError(f"Unsupported type for concatenation: got {type(tensors)}")
+
+def nested_numpify(tensors):
+    "Numpify `tensors` (even if it's a nested list/tuple/dict of tensors)."
+    if isinstance(tensors, (list, tuple)):
+        return type(tensors)(nested_numpify(t) for t in tensors)
+    if isinstance(tensors, Mapping):
+        return type(tensors)({k: nested_numpify(t) for k, t in tensors.items()})
+
+    if tensors.dtype == mindspore.bfloat16:
+        # As of Numpy 1.21.4, NumPy does not support bfloat16 (see
+        # https://github.com/numpy/numpy/blob/a47ecdea856986cd60eabbd53265c2ca5916ad5d/doc/source/user/basics.types.rst ).
+        # Until Numpy adds bfloat16, we must convert float32.
+        tensors = tensors.to(mindspore.float32)
+    return tensors.asnumpy()
+
+def neftune_post_forward_hook(module, input, output):
+    """
+    Implements the NEFTune forward pass for the model using forward hooks. Note this works only for torch.nn.Embedding
+    layers. This method is slightly adapted from the original source code that can be found here:
+    https://github.com/neelsjain/NEFTune Simply add it to your model as follows:
+    ```python
+    model = ...
+    model.embed_tokens.neftune_noise_alpha = 0.1
+    model.embed_tokens.register_forward_hook(neftune_post_forward_hook)
+    ```
+    Args:
+        module (`torch.nn.Module`):
+            The embedding module where the hook is attached. Note that you need to set `module.neftune_noise_alpha` to
+            the desired noise alpha value.
+        input (`torch.Tensor`):
+            The input tensor to the model.
+        output (`torch.Tensor`):
+            The output tensor of the model (i.e. the embeddings).
+    """
+    if module.training:
+        dims = mindspore.tensor(output.shape[1] * output.shape[2], mindspore.float32)
+        mag_norm = module.neftune_noise_alpha / ops.sqrt(dims)
+        output = output + ops.uniform(output.shape, -mag_norm, mag_norm, dtype=output.dtype)
+    return output
+
+def mismatch_dataset_col_names(map_fn_args, col_names):
+    return not set(map_fn_args).issubset(set(col_names))
+
+def get_function_args(fn):
+    signature = inspect.signature(fn)
+    parameter_names = [param.name for param in signature.parameters.values()]
+    return parameter_names
+
+def args_only_in_map_fn(map_fn_args, col_names):
+    return [element for element in map_fn_args if element not in col_names]
+
+def check_input_output_count(fn):
+    num_input_params = len(inspect.signature(fn).parameters)
+    return_annotation = inspect.signature(fn).return_annotation
+    num_output_params = 1 if isinstance(return_annotation, type) else len(return_annotation.__args__) \
+        if return_annotation != inspect.Signature.empty else 0
+
+    return num_input_params == num_output_params
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## mindnlp/engine/trainer/base.py

```diff
@@ -1,409 +1,2036 @@
+# coding=utf-8
+# Copyright 2020-present the HuggingFace Inc. team.
 # Copyright 2022 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""
-Trainer for training.
-"""
+# pylint: disable=expression-not-assigned
+# pylint: disable=assignment-from-no-return
+"""Trainer class, to easily train a 🤗 Transformers from scratch or finetune it on a new task."""
 import os
-from typing import Optional, List, Union
-from inspect import signature
-from tqdm.autonotebook import tqdm
-from mindspore import nn, Tensor, context, mutable
-from mindspore import save_checkpoint
-from mindspore.context import K_CONTEXT
-from mindspore.dataset.engine import Dataset, TakeDataset
-
-from mindnlp.injection import set_global_fp16
-from mindnlp.abc import Callback, Metric
-from mindnlp.transformers.configuration_utils import PretrainedConfig
-from mindnlp.engine.callbacks.callback_manager import CallbackManager, RunContext
-from mindnlp.engine.callbacks.earlystop_callback import EarlyStopCallback
-from mindnlp.engine.callbacks.best_model_callback import BestModelCallback
-from mindnlp.engine.evaluator import Evaluator
-from mindnlp._legacy.amp import auto_mixed_precision, StaticLossScaler, NoLossScaler
-from mindnlp.engine.trainer.utils import get_default_forward_fn_with_loss_fn, \
-    get_default_forward_fn_without_loss_fn, get_default_train_step_fn
-from mindnlp.utils import logging
+import re
+import gc
+import sys
+import math
+import time
+import inspect
+import shutil
+import json
+import copy
+from pathlib import Path
+from functools import lru_cache
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+
+import numpy as np
+
+import mindspore
+from mindspore import nn, ops
+from mindspore.dataset import Dataset, BatchDataset, PaddedBatchDataset
+import mindspore.experimental
+import mindspore.experimental.optim
+from mindspore.nn.learning_rate_schedule import LearningRateSchedule
+
+from ...peft import PeftModel
+from ...configs import WEIGHTS_NAME, CONFIG_NAME, ADAPTER_WEIGHTS_NAME, ADAPTER_SAFE_WEIGHTS_NAME, \
+    WEIGHTS_INDEX_NAME, SAFE_WEIGHTS_NAME, SAFE_WEIGHTS_INDEX_NAME
+from ...dataset import BaseMapFuction
+from ...utils import logging, find_labels, can_return_loss
+from ...utils.serialization import safe_load_file, safe_save_file
+from ...utils.import_utils import is_safetensors_available
+from ...modules.optimization import get_scheduler
+from ...transformers.modeling_utils import PreTrainedModel
+from ...transformers.configuration_utils import PretrainedConfig
+from ...transformers.tokenization_utils_base import PreTrainedTokenizerBase
+from ...transformers.models.auto.modeling_auto import MODEL_FOR_CAUSAL_LM_MAPPING_NAMES, MODEL_MAPPING_NAMES
+from ...transformers.ms_utils import ALL_LAYERNORM_LAYERS
+
+from ..utils import (
+    PREFIX_CHECKPOINT_DIR,
+    EvalPrediction,
+    LabelSmoother,
+    TrainOutput,
+    PredictionOutput,
+    EvalLoopOutput,
+    find_batch_size,
+    denumpify_detensorize,
+    set_seed,
+    enable_full_determinism,
+    has_length,
+    number_of_arguments,
+    get_last_checkpoint,
+    find_executable_batch_size,
+    get_parameter_names,
+    get_model_param_count,
+    speed_metrics,
+    convert_tensor_to_scalar,
+    nested_concat,
+    nested_numpify,
+    neftune_post_forward_hook,
+    mismatch_dataset_col_names,
+    get_function_args,
+    args_only_in_map_fn,
+    check_input_output_count
+)
+from ..train_args import TrainingArguments, OptimizerNames
+from ..callbacks import (
+    CallbackHandler,
+    DefaultFlowCallback,
+    PrinterCallback,
+    ProgressCallback,
+    TrainerCallback,
+    TrainerControl,
+    TrainerState,
+)
+
 
 logger = logging.get_logger(__name__)
 
-class Trainer:
-    r"""
-    Trainer to train the model.
+DEFAULT_CALLBACKS = [DefaultFlowCallback]
+DEFAULT_PROGRESS_CALLBACK = ProgressCallback
+
+# Name of the files used for checkpointing
+TRAINING_ARGS_NAME = "training_args.bin"
+TRAINER_STATE_NAME = "trainer_state.json"
+OPTIMIZER_NAME = "optimizer.ckpt"
+SCHEDULER_NAME = "scheduler.json"
+SCALER_NAME = "scaler.json"
+
+def _is_peft_model(model):
+    classes_to_check = (PeftModel,)
+    # Here we also check if the model is an instance of `PeftMixedModel` introduced in peft>=0.7.0: https://github.com/huggingface/transformers/pull/28321
+    return isinstance(model, classes_to_check)
 
-    Args:
-        network (Cell): A training network.
-        train_dataset (Dataset): A training dataset iterator. If `loss_fn` is defined, the data and label will be
-            passed to the `network` and the `loss_fn` respectively, so a tuple (data, label)
-            should be returned from dataset. If there is multiple data or labels, set `loss_fn`
-            to None and implement calculation of loss in `network`,
-            then a tuple (data1, data2, data3, ...) with all data returned from dataset will be
-            passed to the `network`.
-        eval_dataset (Dataset): A evaluating dataset iterator. If `loss_fn` is defined, the data and label will be
-            passed to the `network` and the `loss_fn` respectively, so a tuple (data, label)
-            should be returned from dataset. If there is multiple data or labels, set `loss_fn`
-            to None and implement calculation of loss in `network`,
-            then a tuple (data1, data2, data3, ...) with all data returned from dataset will be
-            passed to the `network`.
-        metrics (Optional[list[Metrics], Metrics]): List of metrics objects which should be used
-            while evaluating. Default:None.
-        epochs (int): Total number of iterations on the data. Default: 10.
-        optimizer (Cell): Optimizer for updating the weights. If `optimizer` is None, the `network` needs to
-            do backpropagation and update weights. Default value: None.
-        loss_fn (Cell): Objective function. If `loss_fn` is None, the `network` should contain the calculation of loss
-            and parallel if needed. Default: None.
-        callbacks (Optional[list[Callback], Callback]): List of callback objects which should be executed
-            while training. Default: None.
-        jit (bool): Whether use Just-In-Time compile.
 
+class Trainer:
+    """
+    Trainer is a simple but feature-complete training and eval loop for PyTorch, optimized for 🤗 Transformers.
     """
 
-    def __init__(self,
-                 network,
-                 args=None,
-                 loss_fn: Optional[nn.Cell] = None,
-                 optimizer: Optional[nn.Cell] = None,
-                 train_dataset: Optional[Dataset] = None,
-                 eval_dataset: Optional[Dataset] = None,
-                 metrics: Optional[Metric] = None,
-                 callbacks: Optional[Union[Callback, List]] = None,
-                 **kwargs):
+    from ..utils import _get_learning_rate
+    def __init__(
+        self,
+        model: Union[PreTrainedModel, nn.Cell] = None,
+        args: TrainingArguments = None,
+        map_fn: Optional[Union[Callable, BaseMapFuction]] = None,
+        train_dataset: Optional[Dataset] = None,
+        eval_dataset: Optional[Union[Dataset, Dict[str, Dataset]]] = None,
+        tokenizer: Optional[PreTrainedTokenizerBase] = None,
+        model_init: Optional[Callable[[], PreTrainedModel]] = None,
+        compute_metrics: Optional[Callable[[EvalPrediction], Dict]] = None,
+        callbacks: Optional[List[TrainerCallback]] = None,
+        optimizers: Tuple[nn.Optimizer, LearningRateSchedule] = (None, None),
+        preprocess_logits_for_metrics: Optional[Callable[[mindspore.Tensor, mindspore.Tensor], mindspore.Tensor]] = None,
+    ):
+        if args is None:
+            output_dir = "tmp_trainer"
+            logger.info(f"No `TrainingArguments` passed, using `output_dir={output_dir}`.")
+            args = TrainingArguments(output_dir=output_dir)
 
         self.args = args
-        epochs = kwargs.pop('epochs', None)
-        jit = kwargs.pop('jit', False)
-        check_gradients = kwargs.pop('check_gradients', False)
-
-        if jit and 'MS' not in str(network.__class__.__name__):
-            raise ValueError(f'{network.__class__.__name__} do not support static graph via jit compile, '
-                             f'please check the supported model list and use MS{network.__class__.__name__} instead.')
-        # deprecated args
-        self.jit = jit
-        self.check_gradients = check_gradients
-
-        if isinstance(train_dataset, TakeDataset):
-            logger.warning("The `train_dataset` is split after the 'batch' operation, "
-                        "which will slow down the training speed and recompile the neural network"
-                        "please split it first, and then use 'map' operation.")
-
-        # model components
-        self.network = network
-        self.loss_fn = loss_fn
-        self.optimizer = optimizer
-        self.forward_fn = None
-        self.train_fn = None
-
-        if loss_fn is None:
-            self.obj_network = True
-        else:
-            self.obj_network = False
-
-        # dataset
-        self.train_dataset = train_dataset
-        self.epochs = epochs
-
-        # amp settings
-        self.amp_level = 'O0'
-        self.loss_scaler = NoLossScaler()
-
-        self.cur_epoch_nums = 0
-        self.cur_step_nums = 0
-        self.earlystop = False
-        if callbacks:
-            callbacks = self._prepare_callbacks(callbacks)
-        self._prepare_eval(eval_dataset, metrics, callbacks, jit)
-
-        self.callback_manager = CallbackManager(callbacks)
-
-    def _prepare_train_func(self):
-        if self.forward_fn is None:
-            self.forward_fn = get_default_forward_fn_with_loss_fn(self.network, self.loss_fn, self.loss_scaler) \
-                if not self.obj_network else get_default_forward_fn_without_loss_fn(self.network, self.loss_scaler)
-
-        if self.train_fn is None:
-            self.train_fn = get_default_train_step_fn(self.forward_fn, self.optimizer, self.loss_scaler,
-                                                      self.check_gradients or self.amp_level != 'O0', self.jit, self.obj_network)
-
-    def _prepare_callbacks(self, callbacks):
-        if isinstance(callbacks, Callback):
-            return [callbacks]
-        if isinstance(callbacks, list):
-            if all(isinstance(cb, Callback) for cb in callbacks) is True:
-                return callbacks
-            obj = [not isinstance(cb, Callback) for cb in callbacks][0]
-            raise TypeError(f"Expect sub-classes of Callback. Got {type(obj)}")
-        raise TypeError(f"Expect callbacks to be list or Callback. Got {type(callbacks)}.")
-
-    def _check_callbacks_type(self, callbacks):
-        for callback in callbacks:
-            if isinstance(callback, EarlyStopCallback):
-                raise ValueError("EarlyStopCallback is not effective when eval_dataset is None.")
-            if isinstance(callback, BestModelCallback):
-                raise ValueError("BestModelCallback is not effective when eval_dataset is None.")
-
-    def _prepare_eval(self, eval_dataset, metrics, callbacks, jit):
-        if eval_dataset is not None and metrics is not None:
-            self.evaluator = Evaluator(network=self.network, eval_dataset=eval_dataset, metrics=metrics,
-                                       callbacks=callbacks, jit=jit)
-        elif eval_dataset is None and metrics is None:
-            if callbacks:
-                self._check_callbacks_type(callbacks)
-            self.evaluator = None
-        else:
-            raise ValueError("For evaluation in training process, both eval dataset and metrics should be not None.")
-
-    def _check_amp_level_arg(self, optimizer, amp_level):
-        """Check mixed-precision argument rules."""
-        raise NotImplementedError
-
-    def _check_for_graph_cell(self, kwargs):
-        """Check network rules of GraphCell."""
-        raise NotImplementedError
-
-    def _build_boost_network(self, *kwargs):
-        """Build boost network."""
-        raise NotImplementedError
-
-    def _check_reuse_dataset(self, dataset):
-        """Check if dataset is being used by other models under the data sink mode."""
-        if not hasattr(dataset, '__model_hash__'):
-            dataset.__model_hash__ = hash(self)
-        if hasattr(dataset, '__model_hash__') and dataset.__model_hash__ != hash(self):
-            raise RuntimeError("The dataset object had been used in other model by model.train(...), "
-                               "please create a new dataset.")
-
-    def run(self, tgt_columns=None):
-        """
-        Training process entry.
-
-        Args:
-            tgt_columns (Optional[list[str], str]): Target label column names for loss function.
-
-        """
-        self._prepare_train_func()
-
-        args_dict = vars(self)
-        run_context = RunContext(args_dict)
-        self.callback_manager.train_begin(run_context)
-
-        self._run(run_context, tgt_columns)
-        self.callback_manager.train_end(run_context)
-
-    def _run(self, run_context, tgt_columns=None):
-        """
-        Training process for non-data sinking mode. The data would be passed to network directly.
-        """
-
-        # set mindspore mode to GRAPH_MODE, since jit mode with
-        # control flow will slow down the training speed.
-        if self.jit:
-            context.set_context(mode=context.GRAPH_MODE)
-        else:
-            os.environ['MS_DEV_FORCE_ACL'] = '1'
-            K_CONTEXT.set_backend_policy('ge')
-            K_CONTEXT.set_backend_policy('ms')
-
-        total = self.train_dataset.get_dataset_size()
-        # train epoch begin
-        for epoch in range(0, self.epochs):
-            self.network.set_train()
-            self.cur_epoch_nums = epoch + 1
-            self.cur_step_nums = 0
-            run_context.cur_epoch_nums = self.cur_epoch_nums
-            run_context.cur_step_nums = 0
-            if self.earlystop is True:
-                break
-            self.callback_manager.train_epoch_begin(run_context)
-            with tqdm(total=total) as progress:
-                progress.set_description(f'Epoch {epoch}')
-                loss_total = 0
-                # step begin
-                for data in self.train_dataset.create_dict_iterator():
-                    data, tgts = self._data_process(data, tgt_columns)
-                    run_context.cur_step_nums += 1
-                    self.cur_step_nums += 1
-                    self.callback_manager.train_step_begin(run_context)
-                    if self.obj_network:
-                        loss = self.train_fn(**data)
+        # Seed must be set before instantiating the model when using model
+        # mindspore do not support full determinisim on 2.2
+        enable_full_determinism(self.args.seed) if self.args.full_determinism else set_seed(self.args.seed)
+        self.is_in_train = False
+
+        # set the correct log level depending on the node
+        log_level = args.get_process_log_level()
+        logging.set_verbosity(log_level)
+        if model is None:
+            if model_init is not None:
+                self.model_init = model_init
+                model = self.call_model_init()
+            else:
+                raise RuntimeError("`Trainer` requires either a `model` or `model_init` argument")
+        else:
+            if model_init is not None:
+                raise RuntimeError(
+                    "`Trainer` requires either a `model` or `model_init` argument, but not both. `model_init` will"
+                    " overwrite your model when calling the `train` method"
+                )
+            self.model_init = model_init
+
+        if model.__class__.__name__ in MODEL_MAPPING_NAMES:
+            raise ValueError(
+                f"The model you have picked ({model.__class__.__name__}) cannot be used as is for training: it only "
+                "computes hidden states and does not accept any labels. You should choose a model with a head "
+                "suitable for your task like any of the `AutoModelForXxx` listed at "
+                "https://huggingface.co/docs/transformers/model_doc/auto"
+            )
+
+        # if hasattr(model, "is_parallelizable") and model.is_parallelizable and model.model_parallel:
+        #     self.is_model_parallel = True
+        # else:
+        self.is_model_parallel = False
+
+        # TODO: support quantized model
+
+        self.data_map_fn = map_fn
+        if map_fn is not None and not (hasattr(map_fn, 'input_columns') and hasattr(map_fn, 'output_columns')) and \
+            not check_input_output_count(map_fn):
+            raise ValueError('`map_fn` must have same number of inputs and outputs when it is callable function'
+                             ' without attributes `input_columns` and `output_columns`')
+
+        self.train_dataset = copy.deepcopy(train_dataset)
+        self.eval_dataset = copy.deepcopy(eval_dataset)
+        self.tokenizer = tokenizer
+
+        # later use `self.model is self.model_wrapped` to check if it's wrapped or not
+        self.model = model
+        self.model.set_train()
+
+        self.neftune_noise_alpha = args.neftune_noise_alpha
+
+        self.compute_metrics = compute_metrics
+        self.preprocess_logits_for_metrics = preprocess_logits_for_metrics
+        self.optimizer, self.lr_scheduler = optimizers
+        if model_init is not None and (self.optimizer is not None or self.lr_scheduler is not None):
+            raise RuntimeError(
+                "Passing a `model_init` is incompatible with providing the `optimizers` argument. "
+                "You should subclass `Trainer` and override the `create_optimizer_and_scheduler` method."
+            )
+
+        default_callbacks = DEFAULT_CALLBACKS
+        callbacks = default_callbacks if callbacks is None else default_callbacks + callbacks
+        self.callback_handler = CallbackHandler(
+            callbacks, self.model, self.tokenizer, self.optimizer, self.lr_scheduler
+        )
+        self.add_callback(PrinterCallback if self.args.disable_tqdm else DEFAULT_PROGRESS_CALLBACK)
+
+
+        # Will be set to True by `self._setup_loggers()` on first call to `self.log()`.
+        self._loggers_initialized = False
+
+        if self.args.should_save:
+            os.makedirs(self.args.output_dir, exist_ok=True)
+
+        if args.max_steps > 0:
+            logger.info("max_steps is given, it will override any value given in num_train_epochs")
+
+        if train_dataset is not None and not has_length(train_dataset) and args.max_steps <= 0:
+            raise ValueError(
+                "The train_dataset does not implement __len__, max_steps has to be specified. "
+                "The number of steps needs to be known in advance for the learning rate scheduler."
+            )
+
+        self._signature_columns = None
+
+        # Mixed precision setup
+        self.use_amp = False
+
+        # Label smoothing
+        if self.args.label_smoothing_factor != 0:
+            self.label_smoother = LabelSmoother(epsilon=self.args.label_smoothing_factor)
+        else:
+            self.label_smoother = None
+
+        self.state = TrainerState(
+            is_local_process_zero=self.is_local_process_zero(),
+            is_world_process_zero=self.is_world_process_zero(),
+        )
+
+        self.control = TrainerControl()
+        # Internal variable to count flos in each process, will be accumulated in `self.state.total_flos` then
+        # returned to 0 every time flos need to be logged
+
+        self.current_flos = 0
+        self.hp_search_backend = None
+        default_label_names = find_labels(self.model.__class__)
+        self.label_names = default_label_names if self.args.label_names is None else self.args.label_names
+        self.can_return_loss = can_return_loss(self.model.__class__)
+        self.control = self.callback_handler.on_init_end(self.args, self.state, self.control)
+        # Internal variables to help with automatic batch size reduction
+        self._train_batch_size = args.train_batch_size
+        self._created_lr_scheduler = False
+
+    def _activate_neftune(self, model):
+        r"""
+        Activates the neftune as presented in this code: https://github.com/neelsjain/NEFTune and paper:
+        https://arxiv.org/abs/2310.05914
+        """
+        # TODO: support neftune
+        unwrapped_model = model
+
+        if _is_peft_model(unwrapped_model):
+            embeddings = unwrapped_model.base_model.model.get_input_embeddings()
+        else:
+            embeddings = unwrapped_model.get_input_embeddings()
+
+        del unwrapped_model
+
+        embeddings.neftune_noise_alpha = self.neftune_noise_alpha
+        hook_handle = embeddings.register_forward_hook(neftune_post_forward_hook)
+        self.neftune_hook_handle = hook_handle
+        return model
+
+    def _deactivate_neftune(self, model):
+        """
+        Deactivates the neftune method. Make sure to call `_activate_neftune` first.
+        """
+        # TODO: support neftune
+        # if not hasattr(self, "neftune_hook_handle"):
+        #     raise ValueError("Neftune is not activated make sure to call `trainer._activate_neftune()` first")
+
+        unwrapped_model = model
+
+        if _is_peft_model(unwrapped_model):
+            embeddings = unwrapped_model.base_model.model.get_input_embeddings()
+        else:
+            embeddings = unwrapped_model.get_input_embeddings()
+
+        self.neftune_hook_handle.remove()
+        del embeddings.neftune_noise_alpha, unwrapped_model
+
+    def add_callback(self, callback):
+        """
+        Add a callback to the current list of [`~transformers.TrainerCallback`].
+
+        Args:
+           callback (`type` or [`~transformers.TrainerCallback`]):
+               A [`~transformers.TrainerCallback`] class or an instance of a [`~transformers.TrainerCallback`]. In the
+               first case, will instantiate a member of that class.
+        """
+        self.callback_handler.add_callback(callback)
+
+    def pop_callback(self, callback):
+        """
+        Remove a callback from the current list of [`~transformers.TrainerCallback`] and returns it.
+
+        If the callback is not found, returns `None` (and no error is raised).
+
+        Args:
+           callback (`type` or [`~transformers.TrainerCallback`]):
+               A [`~transformers.TrainerCallback`] class or an instance of a [`~transformers.TrainerCallback`]. In the
+               first case, will pop the first member of that class found in the list of callbacks.
+
+        Returns:
+            [`~transformers.TrainerCallback`]: The callback removed, if found.
+        """
+        return self.callback_handler.pop_callback(callback)
+
+    def remove_callback(self, callback):
+        """
+        Remove a callback from the current list of [`~transformers.TrainerCallback`].
+
+        Args:
+           callback (`type` or [`~transformers.TrainerCallback`]):
+               A [`~transformers.TrainerCallback`] class or an instance of a [`~transformers.TrainerCallback`]. In the
+               first case, will remove the first member of that class found in the list of callbacks.
+        """
+        self.callback_handler.remove_callback(callback)
+
+    def _set_signature_columns_if_needed(self):
+        if self._signature_columns is None:
+            # Inspect model forward signature to keep only the arguments it accepts.
+            model_to_inspect = self.model
+            if _is_peft_model(self.model):
+                if hasattr(self.model, "get_base_model"):
+                    model_to_inspect = self.model.get_base_model()
+                else:
+                    # PeftMixedModel do not provide a `get_base_model` method
+                    model_to_inspect = self.model.base_model.model
+            signature = inspect.signature(model_to_inspect.construct)
+            self._signature_columns = list(signature.parameters.keys())
+
+            # Labels may be named label or label_ids, the default data collator handles that.
+            self._signature_columns += list(set(["label", "label_ids"] + self.label_names))
+
+    def _remove_unused_columns(self, dataset: "mindspore.dataset.Dataset", description: Optional[str] = None):
+        if not self.args.remove_unused_columns:
+            return dataset
+        self._set_signature_columns_if_needed()
+        signature_columns = self._signature_columns
+
+        ignored_columns = list(set(dataset.get_col_names()) - set(signature_columns))
+        if len(ignored_columns) > 0:
+            dset_description = "" if description is None else f"in the {description} set"
+            logger.info(
+                f"The following columns {dset_description} don't have a corresponding argument in "
+                f"`{self.model.__class__.__name__}.forward` and have been ignored: {', '.join(ignored_columns)}."
+                f" If {', '.join(ignored_columns)} are not expected by `{self.model.__class__.__name__}.forward`, "
+                " you can safely ignore this message."
+            )
+
+        columns = [k for k in dataset.get_col_names() if k not in ignored_columns]
+
+        return dataset.project(columns)
+
+    def create_optimizer_and_scheduler(self, num_training_steps: int):
+        """
+        Setup the optimizer and the learning rate scheduler.
+
+        We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
+        Trainer's init through `optimizers`, or subclass and override this method (or `create_optimizer` and/or
+        `create_scheduler`) in a subclass.
+        """
+        self.create_optimizer()
+        optimizer = self.optimizer
+        self.create_scheduler(num_training_steps=num_training_steps, optimizer=optimizer)
+
+    def get_decay_parameter_names(self, model) -> List[str]:
+        """
+        Get all parameter names that weight decay will be applied to
+
+        Note that some models implement their own layernorm instead of calling nn.LayerNorm, weight decay could still
+        apply to those modules since this function only filter out instance of nn.LayerNorm
+        """
+        decay_parameters = get_parameter_names(model, ALL_LAYERNORM_LAYERS)
+        decay_parameters = [name for name in decay_parameters if "bias" not in name]
+        return decay_parameters
+
+    def create_optimizer(self):
+        """
+        Setup the optimizer.
+
+        We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
+        Trainer's init through `optimizers`, or subclass and override this method in a subclass.
+        """
+        opt_model = self.model
+
+        if self.optimizer is None:
+            decay_parameters = self.get_decay_parameter_names(opt_model)
+            optimizer_grouped_parameters = [
+                {
+                    "params": [
+                        p for p in opt_model.trainable_params() if (p.name in decay_parameters and p.requires_grad)
+                    ],
+                    "weight_decay": self.args.weight_decay,
+                },
+                {
+                    "params": [
+                        p for p in opt_model.trainable_params() if (p.name not in decay_parameters and p.requires_grad)
+                    ],
+                    "weight_decay": 0.0,
+                },
+            ]
+
+            optimizer_cls, optimizer_kwargs = Trainer.get_optimizer_cls_and_kwargs(self.args, opt_model)
+
+            # Overwrite `params` in case it's created by `get_optimizer_cls_and_kwargs`
+            # e.g. for GaLore optimizer.
+            if "params" in optimizer_kwargs:
+                optimizer_grouped_parameters = optimizer_kwargs.pop("params")
+
+            # For layer-wise dummy optimizers we overwrite optimizer_grouped_parameters with `optimizer_dict`
+            # to avoid arguments conflicts.
+            if "optimizer_dict" in optimizer_kwargs:
+                optimizer_grouped_parameters = optimizer_kwargs.pop("optimizer_dict")
+
+            self.optimizer = optimizer_cls(optimizer_grouped_parameters, **optimizer_kwargs)
+
+        return self.optimizer
+
+    @staticmethod
+    def get_optimizer_cls_and_kwargs(
+        args: TrainingArguments, model: Optional[PreTrainedModel] = None
+    ) -> Tuple[Any, Any]:
+        """
+        Returns the optimizer class and optimizer parameters based on the training arguments.
+
+        Args:
+            args (`transformers.training_args.TrainingArguments`):
+                The training arguments for the training session.
+
+        """
+
+        # parse args.optim_args
+        optim_args = {}
+        if args.optim_args:
+            for mapping in args.optim_args.replace(" ", "").split(","):
+                key, value = mapping.split("=")
+                optim_args[key] = value
+
+        optimizer_kwargs = {"lr": args.learning_rate}
+
+        adam_kwargs = {
+            "betas": (args.adam_beta1, args.adam_beta2),
+            "eps": args.adam_epsilon,
+        }
+        # TODO: support Adafactor
+        # if args.optim == OptimizerNames.ADAFACTOR:
+        #     optimizer_cls = Adafactor
+        #     optimizer_kwargs.update({"scale_parameter": False, "relative_step": False})
+        # TODO: support AdamW huggingface version
+        # elif args.optim == OptimizerNames.ADAMW_HF:
+        #     from .optimization import AdamW
+
+        #     optimizer_cls = AdamW
+        #     optimizer_kwargs.update(adam_kwargs)
+        if args.optim == OptimizerNames.ADAMW:
+            from mindspore.experimental.optim import AdamW
+
+            optimizer_cls = AdamW
+            optimizer_kwargs.update(adam_kwargs)
+        elif args.optim == OptimizerNames.SGD:
+            optimizer_cls = mindspore.experimental.optim.SGD
+        # TODO: support Adagrad and Rmsporp
+        # elif args.optim == OptimizerNames.ADAGRAD:
+        #     optimizer_cls = torch.optim.Adagrad
+        # elif args.optim == OptimizerNames.RMSPROP:
+        #     optimizer_cls = torch.optim.RMSprop
+        else:
+            raise ValueError(f"Trainer cannot instantiate unsupported optimizer: {args.optim}")
+        return optimizer_cls, optimizer_kwargs
+
+
+    def create_scheduler(self, num_training_steps: int, optimizer = None):
+        """
+        Setup the scheduler. The optimizer of the trainer must have been set up either before this method is called or
+        passed as an argument.
+
+        Args:
+            num_training_steps (int): The number of training steps to do.
+        """
+        if self.lr_scheduler is None:
+            self.lr_scheduler = get_scheduler(
+                self.args.lr_scheduler_type,
+                optimizer=self.optimizer if optimizer is None else optimizer,
+                num_warmup_steps=self.args.get_warmup_steps(num_training_steps),
+                num_training_steps=num_training_steps,
+                scheduler_specific_kwargs=self.args.lr_scheduler_kwargs,
+            )
+            self._created_lr_scheduler = True
+        return self.lr_scheduler
+
+    def num_examples(self, dataset: 'mindspore.dataset.Dataset') -> int:
+        """
+        Helper to get number of samples in a [`~torch.utils.data.DataLoader`] by accessing its dataset. When
+        dataloader.dataset does not exist or has no length, estimates as best it can
+        """
+        return dataset.get_dataset_size() * dataset.get_batch_size()
+
+    def num_tokens(self, train_ds: 'mindspore.dataset.Dataset', max_steps: Optional[int] = None) -> int:
+        """
+        Helper to get number of tokens in a [`~torch.utils.data.DataLoader`] by enumerating dataloader.
+        """
+        train_tokens = 0
+        try:
+            for step, batch in train_ds.create_dict_iterator():
+                tokens = batch["input_ids"].numel()
+                if max_steps is not None:
+                    return tokens * max_steps
+                train_tokens += tokens
+            return train_tokens
+        except KeyError:
+            logger.warning("Cannot get num_tokens from dataloader")
+            return train_tokens
+
+    def call_model_init(self):
+        model_init_argcount = number_of_arguments(self.model_init)
+        if model_init_argcount == 0:
+            model = self.model_init()
+        else:
+            raise RuntimeError("model_init should have 0 or 1 argument.")
+
+        if model is None:
+            raise RuntimeError("model_init should not return None.")
+
+        return model
+
+    @lru_cache
+    def get_train_dataset(self) -> Dataset:
+        """
+        Returns the training [`~torch.utils.data.DataLoader`].
+
+        Will use no sampler if `train_dataset` does not implement `__len__`, a random sampler (adapted to distributed
+        training if necessary) otherwise.
+
+        Subclass and override this method if you want to inject some custom behavior.
+        """
+        if self.train_dataset is None:
+            raise ValueError("Trainer: training requires a train_dataset.")
+
+        train_dataset = self.train_dataset
+        map_fn = self.data_map_fn
+        if isinstance(train_dataset, (BatchDataset, PaddedBatchDataset)):
+            if self.data_map_fn is not None:
+                logger.warning("The trainer has been passed a `map_fn` and found `BatchDataset` at same time, "
+                               "the `map_fn` will be ignored.")
+            return train_dataset
+
+        if map_fn is not None:
+            if mismatch_dataset_col_names(get_function_args(map_fn), train_dataset.get_col_names()):
+                raise ValueError(f'The arguments of `map_fn` must be subset of useful dataset columns, '
+                                f'but found {args_only_in_map_fn(get_function_args(map_fn), train_dataset.get_col_names())}')
+            train_dataset = train_dataset.map(map_fn, map_fn.input_columns, map_fn.output_columns)
+
+        train_dataset = self._remove_unused_columns(train_dataset, description="training")
+
+        train_dataset = train_dataset.batch(self._train_batch_size, self.args.dataset_drop_last, self.args.dataset_num_workers)
+        return train_dataset
+
+    @lru_cache
+    def get_test_dataset(self, test_dataset: Dataset) -> Dataset:
+        """
+        Returns the test [`~torch.utils.data.DataLoader`].
+
+        Subclass and override this method if you want to inject some custom behavior.
+
+        Args:
+            test_dataset (`torch.utils.data.Dataset`, *optional*):
+                The test dataset to use. If it is a [`~datasets.Dataset`], columns not accepted by the
+                `model.forward()` method are automatically removed. It must implement `__len__`.
+        """
+        # data_collator = self.data_collator
+        if isinstance(test_dataset, (BatchDataset, PaddedBatchDataset)):
+            return test_dataset
+        test_dataset = self._remove_unused_columns(test_dataset, description="test")
+        test_dataset = test_dataset.batch(self.args.eval_batch_size, self.args.dataset_drop_last, self.args.dataset_num_workers)
+
+        # We use the same batch_size as for eval.
+        return test_dataset
+
+    @lru_cache
+    def get_eval_dataset(self, eval_dataset: Dataset = None) -> Dataset:
+        """
+        Returns the test [`~torch.utils.data.DataLoader`].
+
+        Subclass and override this method if you want to inject some custom behavior.
+
+        Args:
+            test_dataset (`torch.utils.data.Dataset`, *optional*):
+                The test dataset to use. If it is a [`~datasets.Dataset`], columns not accepted by the
+                `model.forward()` method are automatically removed. It must implement `__len__`.
+        """
+        # data_collator = self.data_collator
+        if eval_dataset is None and self.eval_dataset is None:
+            raise ValueError("Trainer: evaluation requires an eval_dataset.")
+
+        eval_dataset = eval_dataset if eval_dataset is not None else self.eval_dataset
+
+        if isinstance(eval_dataset, (BatchDataset, PaddedBatchDataset)):
+            return eval_dataset
+
+        eval_dataset = self._remove_unused_columns(eval_dataset, description="test")
+        eval_dataset = eval_dataset.batch(self.args.eval_batch_size, self.args.dataset_drop_last, self.args.dataset_num_workers)
+
+        # We use the same batch_size as for eval.
+        return eval_dataset
+
+
+    def train(
+        self,
+        resume_from_checkpoint: Optional[Union[str, bool]] = None,
+        ignore_keys_for_eval: Optional[List[str]] = None,
+        **kwargs,
+    ):
+        """
+        Main training entry point.
+
+        Args:
+            resume_from_checkpoint (`str` or `bool`, *optional*):
+                If a `str`, local path to a saved checkpoint as saved by a previous instance of [`Trainer`]. If a
+                `bool` and equals `True`, load the last checkpoint in *args.output_dir* as saved by a previous instance
+                of [`Trainer`]. If present, training will resume from the model/optimizer/scheduler states loaded here.
+            ignore_keys_for_eval (`List[str]`, *optional*)
+                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
+                gathering predictions for evaluation during the training.
+            kwargs (`Dict[str, Any]`, *optional*):
+                Additional keyword arguments used to hide deprecated arguments
+        """
+        if resume_from_checkpoint is False:
+            resume_from_checkpoint = None
+
+        args = self.args
+
+        self.is_in_train = True
+
+        # Attach NEFTune hooks if necessary
+        if self.neftune_noise_alpha is not None:
+            self.model = self._activate_neftune(self.model)
+
+        if len(kwargs) > 0:
+            raise TypeError(f"train() received got unexpected keyword arguments: {', '.join(list(kwargs.keys()))}.")
+        # This might change the seed so needs to run first.
+        self._train_batch_size = self.args.train_batch_size
+        # Model re-init
+        model_reloaded = False
+        if self.model_init is not None:
+            # Seed must be set before instantiating the model when using model_init.
+            enable_full_determinism(self.args.seed) if self.args.full_determinism else set_seed(self.args.seed)
+            self.model = self.call_model_init()
+            model_reloaded = True
+            # Reinitializes optimizer and scheduler
+            self.optimizer, self.lr_scheduler = None, None
+
+        self.model_reload = model_reloaded
+
+        # Load potential model checkpoint
+        if isinstance(resume_from_checkpoint, bool) and resume_from_checkpoint:
+            resume_from_checkpoint = get_last_checkpoint(args.output_dir)
+            if resume_from_checkpoint is None:
+                raise ValueError(f"No valid checkpoint found in output directory ({args.output_dir})")
+
+        if resume_from_checkpoint is not None:
+            self._load_from_checkpoint(resume_from_checkpoint)
+            # In case of repeating the find_executable_batch_size, set `self._train_batch_size` properly
+            state = TrainerState.load_from_json(os.path.join(resume_from_checkpoint, TRAINER_STATE_NAME))
+            if state.train_batch_size is not None:
+                self._train_batch_size = state.train_batch_size
+
+        if model_reloaded:
+            self.model_wrapped = self.model
+
+        inner_training_loop = find_executable_batch_size(
+            self._inner_training_loop, self._train_batch_size, args.auto_find_batch_size
+        )
+
+        return inner_training_loop(
+            args=args,
+            resume_from_checkpoint=resume_from_checkpoint,
+            ignore_keys_for_eval=ignore_keys_for_eval,
+        )
+
+    def _load_best_model(self):
+        logger.info(f"Loading best model from {self.state.best_model_checkpoint} (score: {self.state.best_metric}).")
+        best_model_path = os.path.join(self.state.best_model_checkpoint, WEIGHTS_NAME)
+        best_safe_model_path = os.path.join(self.state.best_model_checkpoint, SAFE_WEIGHTS_NAME)
+        best_adapter_model_path = os.path.join(self.state.best_model_checkpoint, ADAPTER_WEIGHTS_NAME)
+        best_safe_adapter_model_path = os.path.join(self.state.best_model_checkpoint, ADAPTER_SAFE_WEIGHTS_NAME)
+
+        model = self.model
+
+        if (
+            os.path.exists(best_model_path)
+            or os.path.exists(best_safe_model_path)
+            or os.path.exists(best_adapter_model_path)
+            or os.path.exists(best_safe_adapter_model_path)
+        ):
+            has_been_loaded = True
+
+            if _is_peft_model(model):
+                # If train a model using PEFT & LoRA, assume that adapter have been saved properly.
+                if hasattr(model, "active_adapter") and hasattr(model, "load_adapter"):
+                    if os.path.exists(best_adapter_model_path) or os.path.exists(best_safe_adapter_model_path):
+                        model.load_adapter(self.state.best_model_checkpoint, model.active_adapter)
+                        # Load_adapter has no return value present, modify it when appropriate.
+                        load_result = [], []
+                    else:
+                        logger.warning(
+                            "The intermediate checkpoints of PEFT may not be saved correctly, "
+                            f"consider using a custom callback to save {ADAPTER_WEIGHTS_NAME} in corresponding saving folders. "
+                            "Check some examples here: https://github.com/huggingface/peft/issues/96"
+                        )
+                        has_been_loaded = False
+                else:
+                    logger.warning("Could not load adapter model, make sure to have `peft>=0.3.0` installed")
+                    has_been_loaded = False
+            else:
+                # We load the model state dict on the CPU to avoid an OOM error.
+                if self.args.save_safetensors and os.path.isfile(best_safe_model_path):
+                    state_dict = safe_load_file(best_safe_model_path)
+                else:
+                    state_dict = mindspore.load_checkpoint(
+                        best_model_path,
+                    )
+
+                # If the model is on the GPU, it still works!
+                # which takes *args instead of **kwargs
+                load_result = model.load_state_dict(state_dict, False)
+            if has_been_loaded:
+                self._issue_warnings_after_load(load_result)
+        elif os.path.exists(os.path.join(self.state.best_model_checkpoint, WEIGHTS_INDEX_NAME)):
+            load_result = load_sharded_checkpoint(
+                model, self.state.best_model_checkpoint, strict=False
+            )
+            self._issue_warnings_after_load(load_result)
+        else:
+            logger.warning(
+                f"Could not locate the best model at {best_model_path}, if you are running a distributed training "
+                "on multiple nodes, you should activate `--save_on_each_node`."
+            )
+
+
+    def _get_output_dir(self):
+        run_dir = self.args.output_dir
+        return run_dir
+
+    def _inner_training_loop(
+        self, batch_size=None, args=None, resume_from_checkpoint=None, ignore_keys_for_eval=None
+    ):
+        self._train_batch_size = batch_size
+        if self.args.auto_find_batch_size:
+            self.state.train_batch_size = self._train_batch_size
+        logger.debug(f"Currently training with a batch size of: {self._train_batch_size}")
+        # Dataset and number of training steps
+        train_dataset = self.get_train_dataset()
+
+        # Setting up training control variables:
+        # number of training epochs: num_train_epochs
+        # number of training steps per epoch: num_update_steps_per_epoch
+        # total number of training steps to execute: max_steps
+        total_train_batch_size = self._train_batch_size * args.gradient_accumulation_steps * args.world_size
+
+        len_dataset = None
+        num_train_tokens = None
+
+        if has_length(train_dataset):
+            len_dataset = len(train_dataset)
+            num_update_steps_per_epoch = len_dataset // args.gradient_accumulation_steps
+            num_update_steps_per_epoch = max(num_update_steps_per_epoch, 1)
+            num_examples = self.num_examples(train_dataset)
+            if args.max_steps > 0:
+                max_steps = args.max_steps
+                num_train_epochs = args.max_steps // num_update_steps_per_epoch + int(
+                    args.max_steps % num_update_steps_per_epoch > 0
+                )
+                # May be slightly incorrect if the last batch in the training dataloader has a smaller size but it's
+                # the best we can do.
+                num_train_samples = args.max_steps * total_train_batch_size
+                if args.include_tokens_per_second:
+                    num_train_tokens = (
+                        self.num_tokens(train_dataset, args.max_steps) * args.gradient_accumulation_steps
+                    )
+            else:
+                max_steps = math.ceil(args.num_train_epochs * num_update_steps_per_epoch)
+                num_train_epochs = math.ceil(args.num_train_epochs)
+                num_train_samples = self.num_examples(train_dataset) * args.num_train_epochs
+                if args.include_tokens_per_second:
+                    num_train_tokens = self.num_tokens(train_dataset) * args.num_train_epochs
+        elif args.max_steps > 0:  # Rely on max_steps when dataloader does not have a working size
+            max_steps = args.max_steps
+            # Setting a very large number of epochs so we go as many times as necessary over the iterator.
+            num_train_epochs = sys.maxsize
+            num_update_steps_per_epoch = max_steps
+            num_examples = total_train_batch_size * args.max_steps
+            num_train_samples = args.max_steps * total_train_batch_size
+            if args.include_tokens_per_second:
+                num_train_tokens = self.num_tokens(train_dataset, args.max_steps) * args.gradient_accumulation_steps
+        else:
+            raise ValueError(
+                "args.max_steps must be set to a positive value if dataloader does not have a length, was"
+                f" {args.max_steps}"
+            )
+
+        delay_optimizer_creation = False # do not delay now
+
+        # We need to reset the scheduler, as its parameters may be different on subsequent calls
+        if self._created_lr_scheduler:
+            self.lr_scheduler = None
+            self._created_lr_scheduler = False
+
+        if not delay_optimizer_creation:
+            self.create_optimizer_and_scheduler(num_training_steps=max_steps)
+
+        self.state = TrainerState()
+        self.state.train_batch_size = self._train_batch_size
+
+        # Compute absolute values for logging, eval, and save if given as ratio
+        if args.logging_steps is not None:
+            if args.logging_steps < 1:
+                self.state.logging_steps = math.ceil(max_steps * args.logging_steps)
+            else:
+                self.state.logging_steps = args.logging_steps
+        if args.eval_steps is not None:
+            if args.eval_steps < 1:
+                self.state.eval_steps = math.ceil(max_steps * args.eval_steps)
+            else:
+                self.state.eval_steps = args.eval_steps
+        if args.save_steps is not None:
+            if args.save_steps < 1:
+                self.state.save_steps = math.ceil(max_steps * args.save_steps)
+            else:
+                self.state.save_steps = args.save_steps
+
+        # Activate gradient checkpointing if needed
+        if args.recompute:
+            if args.recompute_kwargs is None:
+                recompute_kwargs = {}
+            else:
+                recompute_kwargs = args.recompute_kwargs
+
+            self.model.recompute_enable(recompute_kwargs=recompute_kwargs)
+
+        model = self.model
+
+        if delay_optimizer_creation:
+            self.create_optimizer_and_scheduler(num_training_steps=max_steps)
+
+        # # Check if saved optimizer or scheduler states exist
+        self._load_optimizer_and_scheduler(resume_from_checkpoint)
+
+        # important: at this point:
+        # self.model         is the Transformers Model
+
+        # Train!
+        logger.info("***** Running training *****")
+        logger.info(f"  Num examples = {num_examples:,}")
+        logger.info(f"  Num Epochs = {num_train_epochs:,}")
+        logger.info(f"  Instantaneous batch size per device = {self.args.per_device_train_batch_size:,}")
+        if self.args.per_device_train_batch_size != self._train_batch_size:
+            logger.info(f"  Training with DataParallel so batch size has been adjusted to: {self._train_batch_size:,}")
+        logger.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_train_batch_size:,}")
+        logger.info(f"  Gradient Accumulation steps = {args.gradient_accumulation_steps}")
+        logger.info(f"  Total optimization steps = {max_steps:,}")
+        logger.info(f"  Number of trainable parameters = {get_model_param_count(model, trainable_only=True):,}")
+
+        self.state.epoch = 0
+        start_time = time.time()
+        epochs_trained = 0
+        steps_trained_in_current_epoch = 0
+        steps_trained_progress_bar = None
+
+        # Check if continuing training from a checkpoint
+        if resume_from_checkpoint is not None and os.path.isfile(
+            os.path.join(resume_from_checkpoint, TRAINER_STATE_NAME)
+        ):
+            self.state = TrainerState.load_from_json(os.path.join(resume_from_checkpoint, TRAINER_STATE_NAME))
+            epochs_trained = self.state.global_step // num_update_steps_per_epoch
+            if not args.ignore_data_skip:
+                steps_trained_in_current_epoch = self.state.global_step % (num_update_steps_per_epoch)
+                steps_trained_in_current_epoch *= args.gradient_accumulation_steps
+            else:
+                steps_trained_in_current_epoch = 0
+
+            logger.info("  Continuing training from checkpoint, will skip to saved global_step")
+            logger.info(f"  Continuing training from epoch {epochs_trained}")
+            logger.info(f"  Continuing training from global step {self.state.global_step}")
+            if not args.ignore_data_skip:
+                logger.info(
+                    f"  Will skip the first {epochs_trained} epochs then the first"
+                    f" {steps_trained_in_current_epoch} batches in the first epoch."
+                )
+
+        # Update the references
+        self.callback_handler.model = self.model
+        self.callback_handler.optimizer = self.optimizer
+        self.callback_handler.lr_scheduler = self.lr_scheduler
+        self.callback_handler.train_dataset = train_dataset
+        # This should be the same if the state has been saved but in case the training arguments changed, it's safer
+        # to set this after the load.
+        self.state.max_steps = max_steps
+        self.state.num_train_epochs = num_train_epochs
+        self.state.is_local_process_zero = self.is_local_process_zero()
+        self.state.is_world_process_zero = self.is_world_process_zero()
+
+        # tr_loss is a tensor to avoid synchronization of TPUs through .item()
+        tr_loss = mindspore.tensor(0.0)
+        # _total_loss_scalar is updated everytime .item() has to be called on tr_loss and stores the sum of all losses
+        self._total_loss_scalar = 0.0
+        self._globalstep_last_logged = self.state.global_step
+        grad_norm: Optional[float] = None
+
+        self.control = self.callback_handler.on_train_begin(args, self.state, self.control)
+
+        total_batched_samples = 0
+        for epoch in range(epochs_trained, num_train_epochs):
+            epoch_iterator = train_dataset
+            if hasattr(epoch_iterator, "set_epoch"):
+                epoch_iterator.set_epoch(epoch)
+
+            # Reset the past mems state at the beginning of each epoch if necessary.
+            if args.past_index >= 0:
+                self._past = None
+
+            steps_in_epoch = (
+                len(epoch_iterator)
+                if len_dataset is not None
+                else args.max_steps * args.gradient_accumulation_steps
+            )
+            self.control = self.callback_handler.on_epoch_begin(args, self.state, self.control)
+
+            if epoch == epochs_trained and resume_from_checkpoint is not None and steps_trained_in_current_epoch == 0:
+                # self._load_rng_state(resume_from_checkpoint)
+                pass
+
+            rng_to_sync = False
+            steps_skipped = 0
+            if steps_trained_in_current_epoch > 0:
+                # epoch_iterator = skip_first_batches(epoch_iterator, steps_trained_in_current_epoch)
+                steps_skipped = steps_trained_in_current_epoch
+                steps_trained_in_current_epoch = 0
+                rng_to_sync = True
+
+            step = -1
+            for step, inputs in enumerate(epoch_iterator.create_dict_iterator()):
+                total_batched_samples += 1
+
+                if self.args.include_num_input_tokens_seen:
+                    main_input_name = getattr(self.model, "main_input_name", "input_ids")
+                    if main_input_name not in inputs:
+                        logger.warning(
+                            "Tried to track the number of tokens seen, however the current model is "
+                            "not configured properly to know what item is the input. To fix this, add "
+                            "a `main_input_name` attribute to the model class you are using."
+                        )
                     else:
-                        loss = self.train_fn(tgts, **data)
-                    loss_total += loss
-                    run_context.loss = loss_total/self.cur_step_nums
-                    progress.set_postfix(loss=loss_total/self.cur_step_nums)
-                    progress.update(1)
-                    # step end
-                    self.callback_manager.train_step_end(run_context)
-            # train epoch end
-            progress.close()
-            self.callback_manager.train_epoch_end(run_context)
-            # do epoch evaluation
-            if self.evaluator is not None:
-                self._do_eval_epoch(run_context, tgt_columns)
-
-        # restore PYNATIVE_MODE after training.
-        if self.jit:
-            context.set_context(mode=context.PYNATIVE_MODE)
-            os.environ['MS_DEV_FORCE_ACL'] = '1'
-            K_CONTEXT.set_backend_policy('ge')
-            K_CONTEXT.set_backend_policy('ms')
-
-    def _run_ds_sink(self, train_dataset, eval_dataset, list_callback,
-                     cb_params, print_steps, eval_steps):
-        """Training process for data sinking mode."""
-        raise NotImplementedError
-
-    def _load_checkpoint(self, path):
-        """Load checkpoint."""
-        raise NotImplementedError
-
-    def _do_eval_steps(self, steps, eval_dataset):
-        """Evaluate the model after n steps."""
-        raise NotImplementedError
-
-    def _do_eval_epoch(self, run_context, tgt_columns=None):
-        """Evaluate the model after an epoch."""
-        self.callback_manager.evaluate_begin(run_context)
-        self.evaluator.clear_metrics()
-        metrics_result, metrics_names, metrics_values = self.evaluator._run(tgt_columns)
-        setattr(run_context, "metrics_values", metrics_values)
-        setattr(run_context, "metrics_result", metrics_result)
-        setattr(run_context, "metrics_names", metrics_names)
-        self.callback_manager.evaluate_end(run_context)
-        self.earlystop = run_context.earlystop
-
-    def _data_process(self, data, tgt_columns):
-        """Process data match the network construct"""
-        # prepare input dataset.
-        sig = signature(self.network.construct)
-        net_args = sig.parameters
-
-        inputs = {}
-        used_col = set()
-        for arg in net_args:
-            if arg in ('self', 'kwargs'):
-                continue
-            if arg not in data.keys():
-                if str(net_args[arg])[-4:] != 'None':
-                    raise ValueError(f'network inputs need `{arg}`, but not found in dataset columns.')
-            else:
-                inputs[arg] = data.get(arg)
-                used_col.add(arg)
-
-        if self.obj_network:
-            return inputs, None
-
-        # process target dataset.
-        tgts = ()
-        tgt_columns = self._prepare_tgt_columns(tgt_columns)
-        for tgt_column in tgt_columns:
-            if tgt_column in data:
-                tgts += (data.get(tgt_column),)
-                used_col.add(tgt_column)
-            else:
-                raise ValueError(f'Not found `{tgt_column}` in dataset, please check dataset column names.')
-
-        remain_data_keys = set(data.keys()) - used_col
-
-        if remain_data_keys:
-            logger.warning(f'{remain_data_keys} is not match inputs arguments of network or function.')
-
-        return inputs, mutable(tgts)
-
-    def _prepare_tgt_columns(self, tgt_columns):
-        """Check and prepare target columns for training."""
-        out_columns = []
-        if tgt_columns is None:
-            logger.warning("In the process of training model, tgt_column can not be None.")
-            return []
-        if not isinstance(tgt_columns, (str, list)):
-            raise TypeError(f"Expect tgt_columns to be list or str. Got {type(tgt_columns)}.")
-
-        if isinstance(tgt_columns, str):
-            tgt_columns = [tgt_columns]
-
-        for col in tgt_columns:
-            if isinstance(col, str):
-                out_columns.append(col)
-            else:
-                raise TypeError(f"Expect str of tgt_column. Got {type(col)}")
-
-        return out_columns
-
-    def add_callback(self):
-        """add callback"""
-
-    def remove_callback(self, name_or_type):
-        """remove callback"""
-
-    def set_forward_fn(self, forward_fn):
-        """set forward function"""
-        self.forward_fn = forward_fn
-
-    def set_step_fn(self, step_fn):
-        """set step function"""
-        self.train_fn = step_fn
-
-    def set_amp(self, level='O1', loss_scaler=None):
-        """set amp"""
-        self.amp_level = level
-        self.network = auto_mixed_precision(self.network, level)
-        set_global_fp16(True)
-        if loss_scaler is None:
-            logger.warning("Trainer will use 'StaticLossScaler' with `scale_value=2 ** 10` when `loss_scaler` is None.")
-            self.loss_scaler = StaticLossScaler(2 ** 10)
-        else:
-            self.loss_scaler = loss_scaler
-
-    def set_optimizer(self, optimizer):
-        """set optimizer"""
-        self.optimizer = optimizer
-
-    def train(self, target_columns):
-        """train"""
-        return self.run(target_columns)
-
-    def train_step(self, inputs):
-        """train step"""
-        if isinstance(inputs, Tensor):
-            inputs = (inputs,)
-        return self.train_fn(*inputs)
-
-    def train_loop(self, train_dataset):
-        """train loop"""
-
-    def evaluate(self):
-        """evalute"""
-
-    def evaluate_loop(self):
-        """evaluate loop"""
-
-    def predict(self, test_dataset):
-        """predict"""
-
-    def predict_step(self, inputs, return_loss_only=False):
-        """predict step"""
-
-    def predict_loop(self):
-        """predict loop"""
-
-    def save_model(self, output_dir, model_name=None):
-        """save model to specify dir."""
-        assert output_dir, "`output_dir` is None, please input a real path."
-        if hasattr(self.network, 'config') and isinstance(self.network.config, PretrainedConfig):
-            self.network.config.to_file(output_dir)
-        if model_name:
-            model_path = os.path.join(output_dir, f'{model_name}.ckpt')
+                        self.state.num_input_tokens_seen += self.accelerator.gather(inputs[main_input_name]).numel()
+                if rng_to_sync:
+                    # self._load_rng_state(resume_from_checkpoint)
+                    rng_to_sync = False
+
+                # Skip past any already trained steps if resuming training
+                if steps_trained_in_current_epoch > 0:
+                    steps_trained_in_current_epoch -= 1
+                    if steps_trained_progress_bar is not None:
+                        steps_trained_progress_bar.update(1)
+                    if steps_trained_in_current_epoch == 0:
+                        self._load_rng_state(resume_from_checkpoint)
+                    continue
+                if steps_trained_progress_bar is not None:
+                    steps_trained_progress_bar.close()
+                    steps_trained_progress_bar = None
+
+                if step % args.gradient_accumulation_steps == 0:
+                    self.control = self.callback_handler.on_step_begin(args, self.state, self.control)
+
+                tr_loss_step, grads = self.training_step(model, inputs)
+                if (
+                    args.logging_nan_inf_filter
+                    and (ops.isnan(tr_loss_step) or ops.isinf(tr_loss_step))
+                ):
+                    # if loss is nan or inf simply add the average of previous logged losses
+                    tr_loss += tr_loss / (1 + self.state.global_step - self._globalstep_last_logged)
+                else:
+                    tr_loss += tr_loss_step
+
+                self.current_flos += float(self.floating_point_ops(inputs))
+
+                is_last_step_and_steps_less_than_grad_acc = (
+                    steps_in_epoch <= args.gradient_accumulation_steps and (step + 1) == steps_in_epoch
+                )
+                if (
+                    total_batched_samples % args.gradient_accumulation_steps == 0
+                    or
+                    # last step in epoch but step is always smaller than gradient_accumulation_steps
+                    is_last_step_and_steps_less_than_grad_acc
+                ):
+                    # Gradient clipping
+                    if args.max_grad_norm is not None and args.max_grad_norm > 0:
+                        # deepspeed does its own clipping
+                        grads = ops.clip_by_global_norm(grads, args.max_grad_norm)
+
+                    # Optimizer step
+                    self.optimizer(grads)
+
+                    self.state.global_step += 1
+                    self.state.epoch = epoch + (step + 1 + steps_skipped) / steps_in_epoch
+                    self.control = self.callback_handler.on_step_end(args, self.state, self.control)
+                    self._maybe_log_save_evaluate(tr_loss, grad_norm, model, epoch, ignore_keys_for_eval)
+                else:
+                    self.control = self.callback_handler.on_substep_end(args, self.state, self.control)
+
+                if self.control.should_epoch_stop or self.control.should_training_stop:
+                    break
+            if step < 0:
+                logger.warning(
+                    "There seems to be not a single sample in your epoch_iterator, stopping training at step"
+                    f" {self.state.global_step}! This is expected if you're using an IterableDataset and set"
+                    f" num_steps ({max_steps}) higher than the number of available samples."
+                )
+                self.control.should_training_stop = True
+
+            self.control = self.callback_handler.on_epoch_end(args, self.state, self.control)
+            self._maybe_log_save_evaluate(tr_loss, grad_norm, model, epoch, ignore_keys_for_eval)
+
+            if self.control.should_training_stop:
+                break
+
+        if args.past_index and hasattr(self, "_past"):
+            # Clean the state at the end of training
+            delattr(self, "_past")
+
+        logger.info("\n\nTraining completed. Do not forget to share your model on huggingface.co/models =)\n\n")
+        if args.load_best_model_at_end and self.state.best_model_checkpoint is not None:
+            # Wait for everyone to get here so we are sure the model has been saved by process 0.
+            self._load_best_model()
+
+        # add remaining tr_loss
+        self._total_loss_scalar += tr_loss.item()
+        train_loss = self._total_loss_scalar / self.state.global_step
+
+        metrics = speed_metrics(
+            "train",
+            start_time,
+            num_samples=num_train_samples,
+            num_steps=self.state.max_steps,
+            num_tokens=num_train_tokens,
+        )
+        self.store_flos()
+        metrics["total_flos"] = self.state.total_flos
+        metrics["train_loss"] = train_loss
+
+        self.is_in_train = False
+
+        self.log(metrics)
+
+        checkpoints_sorted = self._sorted_checkpoints(use_mtime=False, output_dir=self.args.output_dir)
+
+        # Delete the last checkpoint when save_total_limit=1 if it's different from the best checkpoint and process allowed to save.
+        if self.args.should_save and self.state.best_model_checkpoint is not None and self.args.save_total_limit == 1:
+            for checkpoint in checkpoints_sorted:
+                if not os.path.samefile(checkpoint, self.state.best_model_checkpoint):
+                    logger.info(f"Deleting older checkpoint [{checkpoint}] due to args.save_total_limit")
+                    shutil.rmtree(checkpoint)
+
+        self.control = self.callback_handler.on_train_end(args, self.state, self.control)
+
+        # After training we make sure to retrieve back the original forward pass method
+        # for the embedding layer by removing the forward post hook.
+        if self.neftune_noise_alpha is not None:
+            self._deactivate_neftune(self.model)
+
+        return TrainOutput(self.state.global_step, train_loss, metrics)
+
+
+    def _load_from_checkpoint(self, resume_from_checkpoint, model=None):
+        if model is None:
+            model = self.model
+
+        config_file = os.path.join(resume_from_checkpoint, CONFIG_NAME)
+        adapter_weights_file = os.path.join(resume_from_checkpoint, ADAPTER_WEIGHTS_NAME)
+        adapter_safe_weights_file = os.path.join(resume_from_checkpoint, ADAPTER_SAFE_WEIGHTS_NAME)
+        weights_file = os.path.join(resume_from_checkpoint, WEIGHTS_NAME)
+        weights_index_file = os.path.join(resume_from_checkpoint, WEIGHTS_INDEX_NAME)
+        safe_weights_file = os.path.join(resume_from_checkpoint, SAFE_WEIGHTS_NAME)
+        safe_weights_index_file = os.path.join(resume_from_checkpoint, SAFE_WEIGHTS_INDEX_NAME)
+
+        if not (
+            any(
+                os.path.isfile(f)
+                for f in [
+                    weights_file,
+                    safe_weights_file,
+                    weights_index_file,
+                    safe_weights_index_file,
+                    adapter_weights_file,
+                    adapter_safe_weights_file,
+                ]
+            )
+        ):
+            raise ValueError(f"Can't find a valid checkpoint at {resume_from_checkpoint}")
+
+        logger.info(f"Loading model from {resume_from_checkpoint}.")
+
+        if os.path.isfile(config_file):
+            config = PretrainedConfig.from_json_file(config_file)
+
+        if os.path.isfile(weights_file) or os.path.isfile(safe_weights_file):
+            # If the model is on the GPU, it still works!
+            # We load the model state dict on the CPU to avoid an OOM error.
+            if self.args.save_safetensors and os.path.isfile(safe_weights_file):
+                state_dict = safe_load_file(safe_weights_file)
+            else:
+                state_dict = mindspore.load_checkpoint(
+                    weights_file,
+                )
+
+            # workaround for FSDP bug https://github.com/pytorch/pytorch/issues/82963
+            # which takes *args instead of **kwargs
+            load_result = model.load_state_dict(state_dict, False)
+            # release memory
+            del state_dict
+            self._issue_warnings_after_load(load_result)
+
+        # Load adapters following PR # 24096
+        # elif _is_peft_model(model):
+        #     # If train a model using PEFT & LoRA, assume that adapter have been saved properly.
+        #     if hasattr(model, "active_adapter") and hasattr(model, "load_adapter"):
+        #         if os.path.exists(resume_from_checkpoint):
+        #             model.load_adapter(resume_from_checkpoint, model.active_adapter, is_trainable=True)
+        #         else:
+        #             logger.warning(
+        #                 "The intermediate checkpoints of PEFT may not be saved correctly, "
+        #                 f"consider using a custom callback to save {ADAPTER_WEIGHTS_NAME} in corresponding saving folders. "
+        #                 "Check some examples here: https://github.com/huggingface/peft/issues/96"
+        #             )
+        #     else:
+        #         logger.warning("Could not load adapter model, make sure to have `peft>=0.3.0` installed")
+        else:
+            # We load the sharded checkpoint
+            load_result = load_sharded_checkpoint(
+                model, resume_from_checkpoint, prefer_safe=self.args.save_safetensors
+            )
+            self._issue_warnings_after_load(load_result)
+
+
+    def _load_optimizer_and_scheduler(self, checkpoint):
+        """If optimizer and scheduler states exist, load them."""
+        if checkpoint is None:
+            return
+
+
+        checkpoint_file_exists = (
+            os.path.isfile(os.path.join(checkpoint, OPTIMIZER_NAME))
+        )
+        if checkpoint_file_exists and os.path.isfile(os.path.join(checkpoint, SCHEDULER_NAME)):
+            # Load in optimizer and scheduler states
+            mindspore.load_param_into_net(self.optimizer, mindspore.load_checkpoint(os.path.join(checkpoint, OPTIMIZER_NAME)))
+            # with warnings.catch_warnings(record=True) as caught_warnings:
+            with open(os.path.join(checkpoint, SCHEDULER_NAME), 'r') as fp:
+                self.lr_scheduler.load_state_dict(json.load(fp))
+
+            # reissue_pt_warnings(caught_warnings)
+
+    def _prepare_inputs(self, inputs: Dict[str, Union[mindspore.Tensor, Any]]) -> Dict[str, Union[mindspore.Tensor, Any]]:
+        """
+        Prepare `inputs` before feeding them to the model, converting them to tensors if they are not already and
+        handling potential state.
+        """
+        if len(inputs) == 0:
+            raise ValueError(
+                "The batch received was empty, your model won't be able to train on it. Double-check that your "
+                f"training dataset contains keys expected by the model: {','.join(self._signature_columns)}."
+            )
+        if self.args.past_index >= 0 and self._past is not None:
+            inputs["mems"] = self._past
+
+        return inputs
+
+    def training_step(self, model: nn.Cell, inputs: Dict[str, Union[mindspore.Tensor, Any]]) -> Tuple[List[mindspore.Tensor], mindspore.Tensor]:
+        """
+        Perform a training step on a batch of inputs.
+
+        Subclass and override to inject custom behavior.
+
+        Args:
+            model (`nn.Cell`):
+                The model to train.
+            inputs (`Dict[str, Union[mindspore.Tensor, Any]]`):
+                The inputs and targets of the model.
+
+                The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
+                argument `labels`. Check your model's documentation for all accepted arguments.
+
+        Return:
+            `mindspore.Tensor`: The tensor with training loss on this batch.
+        """
+        model.set_train()
+        inputs = self._prepare_inputs(inputs)
+
+        def forward(inputs):
+            return self.compute_loss(model, inputs)
+
+        if getattr(self, 'grad_fn', None) is None or self.model_reload:
+            self.grad_fn = mindspore.value_and_grad(forward, None, self.optimizer.parameters)
+
+        loss, grads = self.grad_fn(inputs)
+
+        return loss / self.args.gradient_accumulation_steps, grads
+
+    def compute_loss(self, model, inputs, return_outputs=False):
+        """
+        How the loss is computed by Trainer. By default, all models return the loss in the first element.
+
+        Subclass and override for custom behavior.
+        """
+        if self.label_smoother is not None and "labels" in inputs:
+            labels = inputs.pop("labels")
+        else:
+            labels = None
+        outputs = model(**inputs)
+        # Save past state if it exists
+        # TODO: this needs to be fixed and made cleaner later.
+        if self.args.past_index >= 0:
+            self._past = outputs[self.args.past_index]
+
+        if labels is not None:
+            # if _is_peft_model(unwrapped_model):
+            #     model_name = unwrapped_model.base_model.model._get_name()
+            # else:
+            model_name = model._get_name()
+            if model_name in MODEL_FOR_CAUSAL_LM_MAPPING_NAMES.values():
+                loss = self.label_smoother(outputs, labels, shift_labels=True)
+            else:
+                loss = self.label_smoother(outputs, labels)
         else:
-            model_path = os.path.join(output_dir, 'model.ckpt')
-        save_checkpoint(self.network, model_path)
+            if isinstance(outputs, dict) and "loss" not in outputs:
+                raise ValueError(
+                    "The model did not return a loss from the inputs, only the following keys: "
+                    f"{','.join(outputs.keys())}. For reference, the inputs it received are {','.join(inputs.keys())}."
+                )
+            # We don't use .loss here since the model may return tuples instead of ModelOutput.
+            loss = outputs["loss"] if isinstance(outputs, dict) else outputs[0]
+
+        return (loss, outputs) if return_outputs else loss
+
+
+    def is_local_process_zero(self) -> bool:
+        """
+        Whether or not this process is the local (e.g., on one machine if training in a distributed fashion on several
+        machines) main process.
+        """
+        return self.args.local_process_index == 0
+
+    def is_world_process_zero(self) -> bool:
+        """
+        Whether or not this process is the global main process (when training in a distributed fashion on several
+        machines, this is only going to be `True` for one process).
+        """
+        # Special case for SageMaker ModelParallel since there process_index is dp_process_index, not the global
+        # process index.
+        return self.args.process_index == 0
+
+    def floating_point_ops(self, inputs: Dict[str, Union[mindspore.Tensor, Any]]):
+        """
+        For models that inherit from [`PreTrainedModel`], uses that method to compute the number of floating point
+        operations for every backward + forward pass. If using another model, either implement such a method in the
+        model or subclass and override this method.
+
+        Args:
+            inputs (`Dict[str, Union[mindspore.Tensor, Any]]`):
+                The inputs and targets of the model.
+
+        Returns:
+            `int`: The number of floating-point operations.
+        """
+        if hasattr(self.model, "floating_point_ops"):
+            return self.model.floating_point_ops(inputs)
+        else:
+            return 0
+
+    def _issue_warnings_after_load(self, load_result):
+        if len(load_result[0]) != 0:
+            if self.model._keys_to_ignore_on_save is not None and set(load_result[0]) == set(
+                self.model._keys_to_ignore_on_save
+            ):
+                self.model.tie_weights()
+            else:
+                logger.warning(f"There were missing keys in the checkpoint model loaded: {load_result[0]}.")
+        if len(load_result[1]) != 0:
+            logger.warning(
+                f"There were unexpected keys in the checkpoint model loaded: {load_result[1]}."
+            )
+
+    def _maybe_log_save_evaluate(self, tr_loss, grad_norm, model, epoch, ignore_keys_for_eval):
+        if self.control.should_log and self.state.global_step > self._globalstep_last_logged:
+            logs: Dict[str, float] = {}
+
+            # # all_gather + mean() to get average loss over all processes
+            # tr_loss_scalar = self._nested_gather(tr_loss).mean().item()
+            tr_loss_scalar = tr_loss.item()
+
+            # reset tr_loss to zero
+            ops.assign(tr_loss, 0)
+
+            logs["loss"] = round(tr_loss_scalar / (self.state.global_step - self._globalstep_last_logged), 4)
+            if grad_norm is not None:
+                logs["grad_norm"] = grad_norm
+            logs["learning_rate"] = self._get_learning_rate()
+
+            self._total_loss_scalar += tr_loss_scalar
+            self._globalstep_last_logged = self.state.global_step
+            self.store_flos()
+            self.log(logs)
+
+        metrics = None
+
+        if self.control.should_evaluate:
+            metrics = self.evaluate(ignore_keys=ignore_keys_for_eval)
+            # self._report_to_hp_search(trial, self.state.global_step, metrics)
+
+            # Run delayed LR scheduler now that metrics are populated
+            if isinstance(self.lr_scheduler, mindspore.experimental.optim.lr_scheduler.ReduceLROnPlateau):
+                metric_to_check = self.args.metric_for_best_model
+                if not metric_to_check.startswith("eval_"):
+                    metric_to_check = f"eval_{metric_to_check}"
+                self.lr_scheduler.step(metrics[metric_to_check])
+
+        if self.control.should_save:
+            self._save_checkpoint(model, metrics=metrics)
+            self.control = self.callback_handler.on_save(self.args, self.state, self.control)
+
+    def save_model(self, output_dir: Optional[str] = None, _internal_call: bool = False):
+        """
+        Will save the model, so you can reload it using `from_pretrained()`.
+
+        Will only save from the main process.
+        """
+
+        if output_dir is None:
+            output_dir = self.args.output_dir
+
+        if self.args.should_save:
+            self._save(output_dir)
+
+    def _save(self, output_dir: Optional[str] = None, state_dict=None):
+        # If we are executing this function, we are the process zero, so we don't check for that.
+        output_dir = output_dir if output_dir is not None else self.args.output_dir
+        os.makedirs(output_dir, exist_ok=True)
+        logger.info(f"Saving model checkpoint to {output_dir}")
+
+        supported_classes = (PreTrainedModel,) #if not is_peft_available() else (PreTrainedModel, PeftModel)
+        # Save a trained model and configuration using `save_pretrained()`.
+        # They can then be reloaded using `from_pretrained()`
+        if not isinstance(self.model, supported_classes):
+            if state_dict is None:
+                state_dict = self.model.parameters_dict()
+
+            if isinstance(self.model, supported_classes):
+                self.model.save_pretrained(
+                    output_dir, state_dict=state_dict, safe_serialization=self.args.save_safetensors
+                )
+            else:
+                logger.info("Trainer.model is not a `PreTrainedModel`, only saving its state dict.")
+                if self.args.save_safetensors:
+                    safe_save_file(
+                        state_dict, os.path.join(output_dir, SAFE_WEIGHTS_NAME), metadata={"format": "np"}
+                    )
+                else:
+                    mindspore.save_checkpoint(self.model, os.path.join(output_dir, WEIGHTS_NAME))
+        else:
+            self.model.save_pretrained(
+                output_dir, state_dict=state_dict, safe_serialization=self.args.save_safetensors
+            )
+
+        if self.tokenizer is not None:
+            self.tokenizer.save_pretrained(output_dir)
+
+        # # Good practice: save your training arguments together with the trained model
+        # torch.save(self.args, os.path.join(output_dir, TRAINING_ARGS_NAME))
+
+    def _save_optimizer_and_scheduler(self, output_dir):
+        if self.args.should_save:
+            # deepspeed.save_checkpoint above saves model/optim/sched
+            mindspore.save_checkpoint(self.optimizer, os.path.join(output_dir, OPTIMIZER_NAME))
+
+        # Save SCHEDULER & SCALER
+        if self.args.should_save:
+            # with warnings.catch_warnings(record=True) as caught_warnings:
+            lr_scheduler_state_dict = copy.deepcopy(self.lr_scheduler.state_dict())
+            with open(os.path.join(output_dir, SCHEDULER_NAME), 'w') as fp:
+                json.dump(convert_tensor_to_scalar(lr_scheduler_state_dict), fp)
+            # reissue_pt_warnings(caught_warnings)
+
+    def _save_checkpoint(self, model, metrics=None):
+        # In all cases, including ddp/dp/deepspeed, self.model is always a reference to the model we
+        # want to save except FullyShardedDDP.
+        # assert unwrap_model(model) is self.model, "internal model should be a reference to self.model"
+
+        # Save model checkpoint
+        checkpoint_folder = f"{PREFIX_CHECKPOINT_DIR}-{self.state.global_step}"
+
+        # self.store_flos()
+
+        run_dir = self._get_output_dir()
+        output_dir = os.path.join(run_dir, checkpoint_folder)
+        self.save_model(output_dir, _internal_call=True)
+
+        if not self.args.save_only_model:
+            # Save optimizer and scheduler
+            self._save_optimizer_and_scheduler(output_dir)
+            # Save RNG state
+            # self._save_rng_state(output_dir)
+
+        # Determine the new best metric / best model checkpoint
+        if metrics is not None and self.args.metric_for_best_model is not None:
+            metric_to_check = self.args.metric_for_best_model
+            if not metric_to_check.startswith("eval_"):
+                metric_to_check = f"eval_{metric_to_check}"
+            metric_value = metrics[metric_to_check]
+
+            operator = np.greater if self.args.greater_is_better else np.less
+            if (
+                self.state.best_metric is None
+                or self.state.best_model_checkpoint is None
+                or operator(metric_value, self.state.best_metric)
+            ):
+                self.state.best_metric = metric_value
+                self.state.best_model_checkpoint = output_dir
+
+        # Save the Trainer state
+        if self.args.should_save:
+            self.state.save_to_json(os.path.join(output_dir, TRAINER_STATE_NAME))
+
+        # Maybe delete some older checkpoints.
+        if self.args.should_save:
+            # Solely rely on numerical checkpoint id for rotation.
+            # mtime is not reliable especially on some fuse fs in cloud environments.
+            self._rotate_checkpoints(use_mtime=False, output_dir=run_dir)
+
+    def _rotate_checkpoints(self, use_mtime=False, output_dir=None) -> None:
+        if self.args.save_total_limit is None or self.args.save_total_limit <= 0:
+            return
+
+        # Check if we should delete older checkpoint(s)
+        checkpoints_sorted = self._sorted_checkpoints(use_mtime=use_mtime, output_dir=output_dir)
+        if len(checkpoints_sorted) <= self.args.save_total_limit:
+            return
+
+        # If save_total_limit=1 with load_best_model_at_end=True, we could end up deleting the last checkpoint, which
+        # we don't do to allow resuming.
+        save_total_limit = self.args.save_total_limit
+        if (
+            self.state.best_model_checkpoint is not None
+            and self.args.save_total_limit == 1
+            and checkpoints_sorted[-1] != self.state.best_model_checkpoint
+        ):
+            save_total_limit = 2
+
+        number_of_checkpoints_to_delete = max(0, len(checkpoints_sorted) - save_total_limit)
+        checkpoints_to_be_deleted = checkpoints_sorted[:number_of_checkpoints_to_delete]
+        for checkpoint in checkpoints_to_be_deleted:
+            logger.info(f"Deleting older checkpoint [{checkpoint}] due to args.save_total_limit")
+            shutil.rmtree(checkpoint, ignore_errors=True)
+
+
+    def store_flos(self):
+        # Storing the number of floating-point operations that went into the model
+        # if self.args.parallel_mode == ParallelMode.DISTRIBUTED:
+        #     self.state.total_flos += (
+        #         distributed_broadcast_scalars([self.current_flos], device=self.args.device).sum().item()
+        #     )
+        #     self.current_flos = 0
+        # else:
+        self.state.total_flos += self.current_flos
+        self.current_flos = 0
+
+    def evaluate(
+        self,
+        eval_dataset: Optional[Union[Dataset, Dict[str, Dataset]]] = None,
+        ignore_keys: Optional[List[str]] = None,
+        metric_key_prefix: str = "eval",
+    ) -> Dict[str, float]:
+        """
+        Run evaluation and returns metrics.
+
+        The calling script will be responsible for providing a method to compute metrics, as they are task-dependent
+        (pass it to the init `compute_metrics` argument).
+
+        You can also subclass and override this method to inject custom behavior.
+
+        Args:
+            eval_dataset (Union[`Dataset`, Dict[str, `Dataset`]), *optional*):
+                Pass a dataset if you wish to override `self.eval_dataset`. If it is a [`~datasets.Dataset`], columns
+                not accepted by the `model.forward()` method are automatically removed. If it is a dictionary, it will
+                evaluate on each dataset, prepending the dictionary key to the metric name. Datasets must implement the
+                `__len__` method.
+
+                <Tip>
+
+                If you pass a dictionary with names of datasets as keys and datasets as values, evaluate will run
+                separate evaluations on each dataset. This can be useful to monitor how training affects other
+                datasets or simply to get a more fine-grained evaluation.
+                When used with `load_best_model_at_end`, make sure `metric_for_best_model` references exactly one
+                of the datasets. If you, for example, pass in `{"data1": data1, "data2": data2}` for two datasets
+                `data1` and `data2`, you could specify `metric_for_best_model="eval_data1_loss"` for using the
+                loss on `data1` and `metric_for_best_model="eval_data1_loss"` for the loss on `data2`.
+
+                </Tip>
+
+            ignore_keys (`List[str]`, *optional*):
+                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
+                gathering predictions.
+            metric_key_prefix (`str`, *optional*, defaults to `"eval"`):
+                An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
+                "eval_bleu" if the prefix is "eval" (default)
+
+        Returns:
+            A dictionary containing the evaluation loss and the potential metrics computed from the predictions. The
+            dictionary also contains the epoch number which comes from the training state.
+        """
+        # handle multipe eval datasets
+        eval_dataset = eval_dataset if eval_dataset is not None else self.eval_dataset
+        if isinstance(eval_dataset, dict):
+            metrics = {}
+            for eval_dataset_name, _eval_dataset in eval_dataset.items():
+                dataset_metrics = self.evaluate(
+                    eval_dataset=_eval_dataset,
+                    ignore_keys=ignore_keys,
+                    metric_key_prefix=f"{metric_key_prefix}_{eval_dataset_name}",
+                )
+                metrics.update(dataset_metrics)
+            return metrics
+
+        eval_dataset = self.get_eval_dataset(eval_dataset)
+
+
+        start_time = time.time()
+
+        eval_loop = self.evaluation_loop
+        output = eval_loop(
+            eval_dataset,
+            description="Evaluation",
+            # No point gathering the predictions if there are no metrics, otherwise we defer to
+            # self.args.prediction_loss_only
+            prediction_loss_only=True if self.compute_metrics is None else None,
+            ignore_keys=ignore_keys,
+            metric_key_prefix=metric_key_prefix,
+        )
+
+        total_batch_size = self.args.eval_batch_size * self.args.world_size
+        if f"{metric_key_prefix}_jit_compilation_time" in output.metrics:
+            start_time += output.metrics[f"{metric_key_prefix}_jit_compilation_time"]
+        output.metrics.update(
+            speed_metrics(
+                metric_key_prefix,
+                start_time,
+                num_samples=output.num_samples,
+                num_steps=math.ceil(output.num_samples / total_batch_size),
+            )
+        )
+
+        self.log(output.metrics)
+
+        self.control = self.callback_handler.on_evaluate(self.args, self.state, self.control, output.metrics)
+
+        return output.metrics
+
+    def predict(
+        self, test_dataset: Dataset, ignore_keys: Optional[List[str]] = None, metric_key_prefix: str = "test"
+    ) -> PredictionOutput:
+        """
+        Run prediction and returns predictions and potential metrics.
+
+        Depending on the dataset and your use case, your test dataset may contain labels. In that case, this method
+        will also return metrics, like in `evaluate()`.
+
+        Args:
+            test_dataset (`Dataset`):
+                Dataset to run the predictions on. If it is an `datasets.Dataset`, columns not accepted by the
+                `model.forward()` method are automatically removed. Has to implement the method `__len__`
+            ignore_keys (`List[str]`, *optional*):
+                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
+                gathering predictions.
+            metric_key_prefix (`str`, *optional*, defaults to `"test"`):
+                An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
+                "test_bleu" if the prefix is "test" (default)
+
+        <Tip>
+
+        If your predictions or labels have different sequence length (for instance because you're doing dynamic padding
+        in a token classification task) the predictions will be padded (on the right) to allow for concatenation into
+        one array. The padding index is -100.
+
+        </Tip>
+
+        Returns: *NamedTuple* A namedtuple with the following keys:
+
+            - predictions (`np.ndarray`): The predictions on `test_dataset`.
+            - label_ids (`np.ndarray`, *optional*): The labels (if the dataset contained some).
+            - metrics (`Dict[str, float]`, *optional*): The potential dictionary of metrics (if the dataset contained
+              labels).
+        """
+        # memory metrics - must set up as early as possible
+        # self._memory_tracker.start()
+
+        test_dataloader = self.get_test_dataset(test_dataset)
+        start_time = time.time()
+
+        eval_loop = self.evaluation_loop
+        output = eval_loop(
+            test_dataloader, description="Prediction", ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix
+        )
+        total_batch_size = self.args.eval_batch_size * self.args.world_size
+        # if f"{metric_key_prefix}_jit_compilation_time" in output.metrics:
+        #     start_time += output.metrics[f"{metric_key_prefix}_jit_compilation_time"]
+        output.metrics.update(
+            speed_metrics(
+                metric_key_prefix,
+                start_time,
+                num_samples=output.num_samples,
+                num_steps=math.ceil(output.num_samples / total_batch_size),
+            )
+        )
+
+        self.control = self.callback_handler.on_predict(self.args, self.state, self.control, output.metrics)
+
+        return PredictionOutput(predictions=output.predictions, label_ids=output.label_ids, metrics=output.metrics)
+
+    def evaluation_loop(
+        self,
+        dataset,
+        description: str,
+        prediction_loss_only: Optional[bool] = None,
+        ignore_keys: Optional[List[str]] = None,
+        metric_key_prefix: str = "eval",
+    ) -> EvalLoopOutput:
+        """
+        Prediction/evaluation loop, shared by `Trainer.evaluate()` and `Trainer.predict()`.
+
+        Works both with or without labels.
+        """
+        args = self.args
+
+        prediction_loss_only = prediction_loss_only if prediction_loss_only is not None else args.prediction_loss_only
+
+        model = self.model
+        # if full fp16 or bf16 eval is wanted and this ``evaluation`` or ``predict`` isn't called
+        # while ``train`` is running, cast it to the right dtype first and then put on device
+        if not self.is_in_train:
+            if args.fp16_full_eval:
+                model = model.to(dtype=mindspore.float16)
+            elif args.bf16_full_eval:
+                model = model.to(dtype=mindspore.bfloat16)
+
+        batch_size = self.args.eval_batch_size
+
+        logger.info(f"***** Running {description} *****")
+        if has_length(dataset):
+            logger.info(f"  Num examples = {self.num_examples(dataset)}")
+        else:
+            logger.info("  Num examples: Unknown")
+        logger.info(f"  Batch size = {batch_size}")
+
+        model.set_train(False)
+
+        self.callback_handler.eval_dataset = dataset
+
+        if args.past_index >= 0:
+            self._past = None
+
+        # Initialize containers
+        # losses/preds/labels on GPU/TPU (accumulated for eval_accumulation_steps)
+        losses_host = None
+        preds_host = None
+        labels_host = None
+        inputs_host = None
+
+        # losses/preds/labels on CPU (final containers)
+        all_losses = None
+        all_preds = None
+        all_labels = None
+        all_inputs = None
+        # Will be useful when we have an iterable dataset so don't know its length.
+
+        observed_num_examples = 0
+        # Main evaluation loop
+        for step, inputs in enumerate(dataset.create_dict_iterator()):
+            # Update the observed num examples
+            observed_batch_size = find_batch_size(inputs)
+
+            if observed_batch_size is not None:
+                observed_num_examples += observed_batch_size
+                # For batch samplers, batch_size is not known by the dataloader in advance.
+                if batch_size is None:
+                    batch_size = observed_batch_size
+
+            # Prediction step
+            loss, logits, labels = self.prediction_step(model, inputs, prediction_loss_only, ignore_keys=ignore_keys)
+            main_input_name = getattr(self.model, "main_input_name", "input_ids")
+            inputs_decode = self._prepare_input(inputs[main_input_name]) if args.include_inputs_for_metrics else None
+
+            # Update containers on host
+            if loss is not None:
+                losses = loss.repeat(observed_batch_size)
+                # losses = loss.repeat(batch_size)
+                losses_host = losses if losses_host is None else nested_concat(losses_host, losses, padding_index=-100)
+            # if labels is not None:
+            #     labels = self.accelerator.pad_across_processes(labels, dim=1, pad_index=-100)
+            if inputs_decode is not None:
+                # inputs_decode = self.accelerator.pad_across_processes(inputs_decode, dim=1, pad_index=-100)
+                # inputs_decode = self.gather_function((inputs_decode))
+                inputs_host = (
+                    inputs_decode
+                    if inputs_host is None
+                    else nested_concat(inputs_host, inputs_decode, padding_index=-100)
+                )
+
+            if logits is not None:
+                # logits = self.accelerator.pad_across_processes(logits, dim=1, pad_index=-100)
+                if self.preprocess_logits_for_metrics is not None:
+                    logits = self.preprocess_logits_for_metrics(logits, labels)
+                # logits = self.gather_function((logits))
+                preds_host = logits if preds_host is None else nested_concat(preds_host, logits, padding_index=-100)
+
+            if labels is not None:
+                # labels = self.gather_function((labels))
+                labels_host = labels if labels_host is None else nested_concat(labels_host, labels, padding_index=-100)
+
+            self.control = self.callback_handler.on_prediction_step(args, self.state, self.control)
+
+            # Gather all tensors and put them back on the CPU if we have done enough accumulation steps.
+            if args.eval_accumulation_steps is not None and (step + 1) % args.eval_accumulation_steps == 0:
+                if losses_host is not None:
+                    losses = nested_numpify(losses_host)
+                    all_losses = losses if all_losses is None else np.concatenate((all_losses, losses), axis=0)
+                if preds_host is not None:
+                    logits = nested_numpify(preds_host)
+                    all_preds = logits if all_preds is None else nested_concat(all_preds, logits, padding_index=-100)
+                if inputs_host is not None:
+                    inputs_decode = nested_numpify(inputs_host)
+                    all_inputs = (
+                        inputs_decode
+                        if all_inputs is None
+                        else nested_concat(all_inputs, inputs_decode, padding_index=-100)
+                    )
+                if labels_host is not None:
+                    labels = nested_numpify(labels_host)
+                    all_labels = (
+                        labels if all_labels is None else nested_concat(all_labels, labels, padding_index=-100)
+                    )
+
+                # Set back to None to begin a new accumulation
+                losses_host, preds_host, inputs_host, labels_host = None, None, None, None
+
+        if args.past_index and hasattr(self, "_past"):
+            # Clean the state at the end of the evaluation loop
+            delattr(self, "_past")
+
+        # Gather all remaining tensors and put them back on the CPU
+        if losses_host is not None:
+            losses = nested_numpify(losses_host)
+            all_losses = losses if all_losses is None else np.concatenate((all_losses, losses), axis=0)
+
+        if preds_host is not None:
+            logits = nested_numpify(preds_host)
+            all_preds = logits if all_preds is None else nested_concat(all_preds, logits, padding_index=-100)
+        if inputs_host is not None:
+            inputs_decode = nested_numpify(inputs_host)
+            all_inputs = (
+                inputs_decode if all_inputs is None else nested_concat(all_inputs, inputs_decode, padding_index=-100)
+            )
+        if labels_host is not None:
+            labels = nested_numpify(labels_host)
+            all_labels = labels if all_labels is None else nested_concat(all_labels, labels, padding_index=-100)
+
+        # Number of samples
+        if has_length(dataset):
+            num_samples = len(dataset)
+        if num_samples == 0 and observed_num_examples > 0:
+            num_samples = observed_num_examples
+
+        # Metrics!
+        if self.compute_metrics is not None and all_preds is not None and all_labels is not None:
+            if args.include_inputs_for_metrics:
+                metrics = self.compute_metrics(
+                    EvalPrediction(predictions=all_preds, label_ids=all_labels, inputs=all_inputs)
+                )
+            else:
+                metrics = self.compute_metrics(EvalPrediction(predictions=all_preds, label_ids=all_labels))
+        else:
+            metrics = {}
+
+        # To be JSON-serializable, we need to remove numpy types or zero-d tensors
+        metrics = denumpify_detensorize(metrics)
+
+        if all_losses is not None:
+            metrics[f"{metric_key_prefix}_loss"] = all_losses.mean().item()
+
+        # Prefix all keys with metric_key_prefix + '_'
+        for key in list(metrics.keys()):
+            if not key.startswith(f"{metric_key_prefix}_"):
+                metrics[f"{metric_key_prefix}_{key}"] = metrics.pop(key)
+
+        return EvalLoopOutput(predictions=all_preds, label_ids=all_labels, metrics=metrics, num_samples=num_samples)
+
+    def _nested_gather(self, tensors, name=None):
+        """
+        Gather value of `tensors` (tensor or list/tuple of nested tensors) and convert them to numpy before
+        concatenating them to `gathered`
+        """
+        if tensors is None:
+            return
+        return tensors
+
+    def prediction_step(
+        self,
+        model: nn.Cell,
+        inputs: Dict[str, Union[mindspore.Tensor, Any]],
+        prediction_loss_only: bool,
+        ignore_keys: Optional[List[str]] = None,
+    ) -> Tuple[Optional[mindspore.Tensor], Optional[mindspore.Tensor], Optional[mindspore.Tensor]]:
+        """
+        Perform an evaluation step on `model` using `inputs`.
+
+        Subclass and override to inject custom behavior.
+
+        Args:
+            model (`nn.Module`):
+                The model to evaluate.
+            inputs (`Dict[str, Union[mindspore.Tensor, Any]]`):
+                The inputs and targets of the model.
+
+                The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
+                argument `labels`. Check your model's documentation for all accepted arguments.
+            prediction_loss_only (`bool`):
+                Whether or not to return the loss only.
+            ignore_keys (`List[str]`, *optional*):
+                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
+                gathering predictions.
+
+        Return:
+            Tuple[Optional[mindspore.Tensor], Optional[mindspore.Tensor], Optional[mindspore.Tensor]]: A tuple with the loss,
+            logits and labels (each being optional).
+        """
+        has_labels = False if len(self.label_names) == 0 else all(inputs.get(k) is not None for k in self.label_names)
+        # For CLIP-like models capable of returning loss values.
+        # If `return_loss` is not specified or being `None` in `inputs`, we check if the default value of `return_loss`
+        # is `True` in `model.forward`.
+        return_loss = inputs.get("return_loss", None)
+        if return_loss is None:
+            return_loss = self.can_return_loss
+        loss_without_labels = len(self.label_names) == 0 and return_loss
+
+        inputs = self._prepare_inputs(inputs)
+        if ignore_keys is None:
+            if hasattr(self.model, "config"):
+                ignore_keys = getattr(self.model.config, "keys_to_ignore_at_inference", [])
+            else:
+                ignore_keys = []
+
+        # labels may be popped when computing the loss (label smoothing for instance) so we grab them first.
+        if has_labels or loss_without_labels:
+            labels = tuple(inputs.get(name) for name in self.label_names)
+            # labels = nested_detach(tuple(inputs.get(name) for name in self.label_names))
+            if len(labels) == 1:
+                labels = labels[0]
+        else:
+            labels = None
+
+        if has_labels or loss_without_labels:
+            loss, outputs = self.compute_loss(model, inputs, return_outputs=True)
+            loss = loss.mean()
+
+            if isinstance(outputs, dict):
+                logits = tuple(v for k, v in outputs.items() if k not in ignore_keys + ["loss"])
+            else:
+                logits = outputs[1:]
+        else:
+            loss = None
+            outputs = model(**inputs)
+            if isinstance(outputs, dict):
+                logits = tuple(v for k, v in outputs.items() if k not in ignore_keys)
+            else:
+                logits = outputs
+            # TODO: this needs to be fixed and made cleaner later.
+            if self.args.past_index >= 0:
+                self._past = outputs[self.args.past_index - 1]
+
+        if prediction_loss_only:
+            return (loss, None, None)
+
+        # logits = nested_detach(logits)
+        if len(logits) == 1:
+            logits = logits[0]
+
+        return (loss, logits, labels)
+
+
+    def log(self, logs: Dict[str, float]) -> None:
+        """
+        Log `logs` on the various objects watching training.
+
+        Subclass and override this method to inject custom behavior.
+
+        Args:
+            logs (`Dict[str, float]`):
+                The values to log.
+        """
+        if self.state.epoch is not None:
+            logs["epoch"] = round(self.state.epoch, 2)
+        if self.args.include_num_input_tokens_seen:
+            logs["num_input_tokens_seen"] = self.state.num_input_tokens_seen
+
+        output = {**logs, **{"step": self.state.global_step}}
+        self.state.log_history.append(output)
+        self.control = self.callback_handler.on_log(self.args, self.state, self.control, logs)
+
+    def _sorted_checkpoints(
+        self, output_dir=None, checkpoint_prefix=PREFIX_CHECKPOINT_DIR, use_mtime=False
+    ) -> List[str]:
+        ordering_and_checkpoint_path = []
+
+        glob_checkpoints = [str(x) for x in Path(output_dir).glob(f"{checkpoint_prefix}-*") if os.path.isdir(x)]
+
+        for path in glob_checkpoints:
+            if use_mtime:
+                ordering_and_checkpoint_path.append((os.path.getmtime(path), path))
+            else:
+                regex_match = re.match(f".*{checkpoint_prefix}-([0-9]+)", path)
+                if regex_match is not None and regex_match.groups() is not None:
+                    ordering_and_checkpoint_path.append((int(regex_match.groups()[0]), path))
+
+        checkpoints_sorted = sorted(ordering_and_checkpoint_path)
+        checkpoints_sorted = [checkpoint[1] for checkpoint in checkpoints_sorted]
+        # Make sure we don't delete the best model.
+        if (
+            self.state.best_model_checkpoint is not None
+            and str(Path(self.state.best_model_checkpoint)) in checkpoints_sorted
+        ):
+            best_model_index = checkpoints_sorted.index(str(Path(self.state.best_model_checkpoint)))
+            for i in range(best_model_index, len(checkpoints_sorted) - 2):
+                checkpoints_sorted[i], checkpoints_sorted[i + 1] = checkpoints_sorted[i + 1], checkpoints_sorted[i]
+        return checkpoints_sorted
+
+def load_sharded_checkpoint(model, folder, strict=True, prefer_safe=True):
+    """
+    This is the same as
+    [`torch.nn.Module.load_state_dict`](https://pytorch.org/docs/stable/generated/torch.nn.Module.html?highlight=load_state_dict#torch.nn.Module.load_state_dict)
+    but for a sharded checkpoint.
+
+    This load is performed efficiently: each checkpoint shard is loaded one by one in RAM and deleted after being
+    loaded in the model.
+
+    Args:
+        model (`torch.nn.Module`): The model in which to load the checkpoint.
+        folder (`str` or `os.PathLike`): A path to a folder containing the sharded checkpoint.
+        strict (`bool`, *optional`, defaults to `True`):
+            Whether to strictly enforce that the keys in the model state dict match the keys in the sharded checkpoint.
+        prefer_safe (`bool`, *optional*, defaults to `False`)
+            If both safetensors and PyTorch save files are present in checkpoint and `prefer_safe` is True, the
+            safetensors files will be loaded. Otherwise, PyTorch files are always loaded when possible.
+
+    Returns:
+        `NamedTuple`: A named tuple with `missing_keys` and `unexpected_keys` fields
+            - `missing_keys` is a list of str containing the missing keys
+            - `unexpected_keys` is a list of str containing the unexpected keys
+    """
+    # Load the index
+    index_file = os.path.join(folder, WEIGHTS_INDEX_NAME)
+    safe_index_file = os.path.join(folder, SAFE_WEIGHTS_INDEX_NAME)
+
+    index_present = os.path.isfile(index_file)
+    safe_index_present = os.path.isfile(safe_index_file)
+
+    if not index_present and not (safe_index_present and is_safetensors_available()):
+        filenames = (
+            (WEIGHTS_INDEX_NAME, SAFE_WEIGHTS_INDEX_NAME) if is_safetensors_available() else (WEIGHTS_INDEX_NAME,)
+        )
+        raise ValueError(f"Can't find a checkpoint index ({' or '.join(filenames)}) in {folder}.")
+
+    load_safe = False
+    if safe_index_present:
+        if prefer_safe:
+            if is_safetensors_available():
+                load_safe = True  # load safe due to preference
+            else:
+                logger.warning(
+                    f"Cannot load sharded checkpoint at {folder} safely since safetensors is not installed!"
+                )
+        elif not index_present:
+            load_safe = True  # load safe since we have no other choice
+
+    load_index = safe_index_file if load_safe else index_file
+
+    with open(load_index, "r", encoding="utf-8") as f:
+        index = json.load(f)
+
+    shard_files = list(set(index["weight_map"].values()))
+
+    # If strict=True, error before loading any of the state dicts.
+    loaded_keys = index["weight_map"].keys()
+    model_keys = model.parameters_dict().keys()
+    missing_keys = [key for key in model_keys if key not in loaded_keys]
+    unexpected_keys = [key for key in loaded_keys if key not in model_keys]
+    if strict and (len(missing_keys) > 0 or len(unexpected_keys) > 0):
+        error_message = f"Error(s) in loading state_dict for {model.__class__.__name__}"
+        if len(missing_keys) > 0:
+            str_missing_keys = ",".join([f'"{k}"' for k in missing_keys])
+            error_message += f"\nMissing key(s): {str_missing_keys}."
+        if len(unexpected_keys) > 0:
+            str_unexpected_keys = ",".join([f'"{k}"' for k in unexpected_keys])
+            error_message += f"\nMissing key(s): {str_unexpected_keys}."
+        raise RuntimeError(error_message)
+
+    loader = safe_load_file if load_safe else mindspore.load_checkpoint
+
+    for shard_file in shard_files:
+        state_dict = loader(os.path.join(folder, shard_file))
+        model.load_state_dict(state_dict, strict=False)
+
+        # Make sure memory is freed before we load the next state dict.
+        del state_dict
+        gc.collect()
+
+    # Return the same thing as PyTorch load_state_dict function.
+    return missing_keys, unexpected_keys
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## mindnlp/parallel/tensor_parallel/layers.py

```diff
@@ -16,15 +16,14 @@
 
 from typing import Optional, Union
 
 import mindspore
 from mindspore import nn, ops
 from mindspore import Parameter, Tensor
 from mindspore.common.initializer import Initializer, Zero
-from mindspore.ops._tracefunc import trace
 from .mappings import _get_rank, _get_group_size
 
 
 from .mappings import (
     copy_to_model_parallel_region,
     gather_from_model_parallel_region,
     reduce_from_model_parallel_region,
@@ -67,15 +66,14 @@
         self.vocab_size_per_partition = self.vocab_end_index - self.vocab_start_index
 
         # Allocate weights.
         self.weight = Parameter(Tensor(shape=(self.vocab_size_per_partition, self.embedding_size),
                                        dtype=dtype, init=init_method),
                                 "weight")
 
-    @trace
     def construct(self, input_: Tensor) -> Tensor:  # type: ignore
         # Build the mask.
         input_mask = (input_ < self.vocab_start_index) | (
             input_ >= self.vocab_end_index
         )
         # Mask the input.
         masked_input = input_ - self.vocab_start_index
@@ -125,15 +123,14 @@
         )
 
         # Allocate weights.
         self.weight = Parameter(Tensor(shape=(self.vocab_size, self.embedding_size_per_partition),
                                        dtype=dtype, init=init_method),
                                 "weight")
 
-    @trace
     def construct(self, input_: Tensor) -> Tensor:  # type: ignore
         input_parallel = copy_to_model_parallel_region(input_)
         ori_shape = input_parallel.shape
         output_parallel = ops.gather(self.weight, input_parallel.view(-1), 0).view(
             ori_shape + (self.embedding_size_per_partition, )
         )
         output = gather_from_model_parallel_region(output_parallel)
@@ -196,15 +193,14 @@
         else:
             self.bias = None
 
     def get_master_weight(self) -> Tensor:
         """get master weight of ColumnParallelLinear"""
         return gather_from_model_parallel_region(self.weight).swapaxes(0, 1)
 
-    @trace
     def construct(self, input_: Tensor) -> Tensor:  # type: ignore
         # Set up backprop all-reduce.
         input_parallel = copy_to_model_parallel_region(input_)
         # Matrix multiply.
         output_parallel = ops.matmul(input_parallel, self.weight)
         if self.bias is not None:
             output_parallel = output_parallel + self.bias
@@ -277,15 +273,14 @@
         else:
             self.bias = None
 
     def get_master_weight(self) -> Tensor:
         """get master weight of RowParallelLinear"""
         return gather_from_model_parallel_region(self.weight).swapaxes(0, 1)
 
-    @trace
     def construct(self, input_: Tensor) -> Tensor:  # type:ignore
         # Set up backprop all-reduce.
         if self.input_is_parallel:
             input_parallel = input_
         else:
             input_parallel = scatter_to_model_parallel_region(input_)
         # Matrix multiply.
```

## mindnlp/peft/__init__.py

```diff
@@ -27,16 +27,22 @@
     # PeftModelForQuestionAnswering,
     PeftModelForSeq2SeqLM,
     PeftModelForSequenceClassification,
     PeftModelForTokenClassification,
 )
 
 from .tuners import (
+    AdaptionPromptConfig,
+    AdaptionPromptModel,
     LoraConfig,
     LoraModel,
+    IA3Config,
+    IA3Model,
+    AdaLoraConfig,
+    AdaLoraModel,
 )
 
 from .utils import (
     # TRANSFORMERS_MODELS_TO_PREFIX_TUNING_POSTPROCESS_MAPPING,
     PeftType,
     TaskType,
     # bloom_model_postprocess_past_key_value,
```

## mindnlp/peft/config.py

```diff
@@ -55,15 +55,19 @@
                 [`~transformers.utils.PushToHubMixin.push_to_hub`] method.
         """
         if os.path.isfile(save_directory):
             raise AssertionError(f"Provided path ({save_directory}) should be a directory, not a file")
 
         os.makedirs(save_directory, exist_ok=True)
 
-        output_dict = self.__dict__
+        output_dict = asdict(self)
+        # converting set type to list
+        for key, value in output_dict.items():
+            if isinstance(value, set):
+                output_dict[key] = list(value)
         output_path = os.path.join(save_directory, CONFIG_NAME)
 
         # save it
         with open(output_path, "w", encoding='utf-8') as writer:
             writer.write(json.dumps(output_dict, indent=2, sort_keys=True))
```

## mindnlp/peft/mapping.py

```diff
@@ -24,16 +24,21 @@
     # PeftModelForFeatureExtraction,
     # PeftModelForQuestionAnswering,
     PeftModelForSeq2SeqLM,
     PeftModelForSequenceClassification,
     PeftModelForTokenClassification,
 )
 from .tuners import (
+    AdaLoraConfig,
+    AdaLoraModel,
     LoraConfig,
-    LoraModel
+    LoraModel,
+    AdaptionPromptConfig,
+    IA3Config,
+    IA3Model,
 )
 
 MODEL_TYPE_TO_PEFT_MODEL_MAPPING = {
     "SEQ_CLS": PeftModelForSequenceClassification,
     "SEQ_2_SEQ_LM": PeftModelForSeq2SeqLM,
     "CAUSAL_LM": PeftModelForCausalLM,
     "TOKEN_CLS": PeftModelForTokenClassification,
@@ -43,23 +48,24 @@
 
 
 PEFT_TYPE_TO_CONFIG_MAPPING = {
     # "ADAPTION_PROMPT": AdaptionPromptConfig,
     # "PROMPT_TUNING": PromptTuningConfig,
     # "PREFIX_TUNING": PrefixTuningConfig,
     # "P_TUNING": PromptEncoderConfig,
+    "ADAPTION_PROMPT": AdaptionPromptConfig,
     "LORA": LoraConfig,
-    # "ADALORA": AdaLoraConfig,
-    # "IA3": IA3Config,
+    "ADALORA": AdaLoraConfig,
+    "IA3": IA3Config,
 }
 
 PEFT_TYPE_TO_TUNER_MAPPING = {
     "LORA": LoraModel,
-    # "ADALORA": AdaLoraModel,
-    # "IA3": IA3Model,
+    "ADALORA": AdaLoraModel,
+    "IA3": IA3Model,
 }
 
 
 def get_peft_config(config_dict: Dict[str, Any]):
     """
     Returns a Peft config object from a dictionary.
```

## mindnlp/peft/peft_model.py

```diff
@@ -23,15 +23,18 @@
 from mindspore import nn, ops
 from mindspore.train.serialization import  _exec_save
 from mindspore.nn import CrossEntropyLoss
 
 from .config import PeftConfig, PromptLearningConfig
 
 from .tuners import (
+    AdaLoraModel,
+    AdaptionPromptModel,
     LoraModel,
+    IA3Model,
     # LoraConfig
 )
 from .utils import (
     # SAFETENSORS_WEIGHTS_NAME,
     # TRANSFORMERS_MODELS_TO_PREFIX_TUNING_POSTPROCESS_MAPPING,
     WEIGHTS_NAME,
     PeftType,
@@ -48,14 +51,17 @@
     shift_tokens_right,
     # _get_batch_size, # will be used for prompt learning methods
 )
 
 
 PEFT_TYPE_TO_MODEL_MAPPING = {
     PeftType.LORA: LoraModel,
+    PeftType.ADAPTION_PROMPT: AdaptionPromptModel,
+    PeftType.IA3: IA3Model,
+    PeftType.ADALORA: AdaLoraModel,
 }
 class PeftModel(nn.Cell):
     """
     Base model encompassing various Peft methods.
 
     Args:
         model ([`~mindnlp.models.PreTrainedModel`]): The base transformer model used for Peft.
```

## mindnlp/peft/tuners/__init__.py

```diff
@@ -11,7 +11,10 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Tuners"""
 
 from .lora import LoraConfig, LoraModel
+from .ia3 import IA3Config, IA3Model
+from .adaption_prompt import AdaptionPromptConfig, AdaptionPromptModel
+from .adalora import AdaLoraConfig, AdaLoraModel
```

## mindnlp/peft/tuners/lora.py

```diff
@@ -37,15 +37,15 @@
     ModulesToSaveWrapper,
     PeftType,
     # _freeze_adapter,
     _get_submodules,
     transpose,
 )
 
-from .tuners_utils import BaseTuner, BaseTunerLayer
+from .tuners_utils import BaseTuner
 
 # if is_bnb_available():
 #     import bitsandbytes as bnb
 
 
 @dataclass
 class LoraConfig(PeftConfig):
@@ -435,32 +435,32 @@
 
         if active_adapter is None:
             raise ValueError(
                 "Something went wrong, no active adapter could be found, please report the issue on GitHub"
             )
         return active_adapter
 
-    def _mark_only_adapters_as_trainable(self) -> None:
+    def _mark_only_adapters_as_trainable(self,model) -> None:
         """mark_only_lora_as_trainable"""
         # get bias
         active_adapter = self._get_active_adapter()
         bias = self.peft_config[active_adapter].bias
 
-        for n, p in self.model.parameters_and_names():  # named_parameters() -> parameters_and_names()
+        for n, p in model.parameters_and_names():  # named_parameters() -> parameters_and_names()
             if "lora_" not in n:
                 p.requires_grad = False
                 # print(n, p, "requires_grad = False")
         if bias == "none":
             return
         elif bias == "all":
-            for n, p in self.model.parameters_and_names():
+            for n, p in model.parameters_and_names():
                 if "bias" in n:
                     p.requires_grad = True
         elif bias == "lora_only":
-            for m in self.model.cells():  # .cells() for modules()
+            for m in model.cells():  # .cells() for modules()
                 if isinstance(m, LoraLayer) and hasattr(m, "bias") and m.bias is not None:
                     m.bias.requires_grad = True
         else:
             raise NotImplementedError
 
 
     @staticmethod
@@ -537,15 +537,15 @@
                     f"Currently, only `torch.nn.Linear` and `Conv1D` are supported."
                 )
             new_module = Linear(adapter_name, in_features, out_features, has_bias=bias, **kwargs)
 
         return new_module
 
 
-class LoraLayer(BaseTunerLayer):
+class LoraLayer():
     """Lora Layer"""
     # TODO add CellDict Support
     def __init__(self, in_features: int, out_features: int, **kwargs):
         self.r = {}
         self.lora_alpha = {}
         self.scaling = {}
         # TODO: there is no nn.CellDict() in mindspore
```

## mindnlp/peft/tuners/tuners_utils.py

```diff
@@ -11,21 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 BaseTuner class and BaseTunerLayer class.
 """
+# pylint: disable=line-too-long
+# pylint: disable=missing-function-docstring
+# pylint: disable=unused-argument
+# pylint: disable=too-many-arguments
+# pylint: disable=too-many-function-args
+# pylint: disable=no-member
+# pylint: disable=function-redefined
 from __future__ import annotations
-
+import re
 import logging
-
-from typing import Any, Union
-
-from mindspore import nn
+import warnings
+from typing import Any, Optional, Union
+from abc import ABC
+from mindspore import nn, Tensor
 
 from ..config import PeftConfig
 from ..utils import _get_submodules
 
 logger = logging.getLogger(__name__)
 
 
@@ -85,19 +92,27 @@
                 # user is adding a dict of PeftConfigs
                 self.peft_config.update(peft_config)
 
         # transformers models have a .config attribute, whose presence is assumed later on
         # if not hasattr(self, "config"):
         #     self.config = {"model_type": "custom"}
 
+        self.active_adapter: str | list[str] = adapter_name
         self.inject_adapter(self.model, adapter_name)
 
         # Copy the peft_config in the injected model.
         self.model.peft_config = self.peft_config
 
+    @property
+    def active_adapters(self) -> list[str]:
+        if isinstance(self.active_adapter, str):
+            return [self.active_adapter]
+        # is already a list of str
+        return self.active_adapter
+
     def construct(self, *args: Any, **kwargs: Any):
         return self.model.construct(*args, **kwargs)
 
     def _prepare_adapter_config(self, peft_config: PeftConfig, model_config: dict) -> PeftConfig:
         r"""
         A private method to eventually prepare the adapter config. For transformers based models, if
         `peft_config.target_modules` is None, we can automatically infer the target modules from the
@@ -236,15 +251,15 @@
 
         if not is_target_modules_in_base_model:
             raise ValueError(
                 f"Target modules {peft_config.target_modules} not found in the base model. "
                 f"Please check the target modules and try again."
             )
 
-        self._mark_only_adapters_as_trainable()
+        self._mark_only_adapters_as_trainable(model)
 
         if self.peft_config[adapter_name].inference_mode:
             for name, param in self.model.parameters_and_names():
                 if adapter_name in name:
                     param.requires_grad = False
 
     def merge_adapter(self):
@@ -260,26 +275,257 @@
         This method unmerges the LoRa layers from the base model.
         """
         for module in self.model.modules():
             if isinstance(module, BaseTunerLayer):
                 module.unmerge()
 
 
-class BaseTunerLayer():
+class BaseTunerLayer(ABC):
     r"""
     A tuner layer mixin that provides the common methods and attributes for all tuners.
 
     Args:
-        is_plugable (`bool`, *optional*):
+        is_pluggable (`bool`, *optional*):
             Whether the adapter layer can be plugged to any pytorch module
-        active_adapter (`str`, *optional*):
+        active_adapters (Union[List[`str`], `str`], *optional*):
             The name of the active adapter.
     """
+
     active_adapter = None
 
-    def merge(self):
-        """megre layer."""
+    # All names of layers that may contain adapter (trainable) weights
+    adapter_layer_names: tuple[str] = ()
+    # All names of other parameters that may contain adapter-related parameters
+    other_param_names: tuple[str] = ()
+
+    # indicates whether all adapters should be disabled
+    _disable_adapters: bool = False
+
+    # the currently active adapter(s)
+    _active_adapter: str | list[str] = "default"
+
+    # List all merged adapters
+    merged_adapters: list[str] = []
+
+    def get_base_layer(self) -> nn.Cell:
+        """
+        (Recursively) get the base_layer.
+
+        This is necessary for the case that the tuner layer wraps another tuner layer.
+
+        """
+        base_layer = self
+        while hasattr(base_layer, "base_layer"):
+            base_layer = base_layer.base_layer
+        return base_layer
+
+    @property
+    def weight(self) -> Tensor:
+        # This is required for some transformers code, e.g. for T5, weight is accessed as:
+        #     self.wo.weight
+        # where "wo" is the adapter layer.
+        # https://github.com/huggingface/transformers/blob/78f6ed6c70b29c1560780e3869a7ad4c6b3d2710/src/transformers
+        # /models/t5/modeling_t5.py#L292
+        base_layer = self.get_base_layer()
+        weight = base_layer.weight
+        return weight
+
+    @property
+    def bias(self) -> Tensor:
+        base_layer = self.get_base_layer()
+        return base_layer.bias
+
+    def merge(self, safe_merge: bool = False, adapter_names: Optional[list[str]] = None) -> None:
         raise NotImplementedError
 
-    def unmerge(self):
-        """unmerge layer."""
+    def unmerge(self) -> None:
         raise NotImplementedError
+
+    @property
+    def merged(self) -> bool:
+        return bool(self.merged_adapters)
+
+    @property
+    def disable_adapters(self) -> bool:
+        # use a property to ensure that disable_adapters is not set directly, instead use the enable_adapters method
+        return self._disable_adapters
+
+    @property
+    def active_adapter(self) -> str | list[str]:
+        # use a property to ensure that active_adapter is not set directly, instead use the set_adapter method
+        return self._active_adapter
+
+    @property
+    def active_adapters(self):
+        if isinstance(self.active_adapter, str):
+            return [self.active_adapter]
+        # is already a list of str
+        return self.active_adapter
+
+    def enable_adapters(self, enabled: bool) -> None:
+        """Toggle the enabling and disabling of adapters
+
+        Takes care of setting the requires_grad flag for the adapter weights.
+
+        Args:
+            enabled (bool): True to enable adapters, False to disable adapters
+        """
+        if enabled:
+            self.set_adapter(self.active_adapters)
+            self._disable_adapters = False
+        else:
+            # disable grads on all adapter layers
+            for layer_name in self.adapter_layer_names:
+                layer = getattr(self, layer_name)
+                layer.set_grad(requires_grad=False)
+            self._disable_adapters = True
+
+    def set_adapter(self, adapter_names: str | list[str]) -> None:
+        """Set the active adapter(s).
+
+        Additionally, this function will set the specified adapters to trainable (i.e., requires_grad=True). If this is
+        not desired, use the following code.
+
+        ```py
+        >>> for name, param in model_peft.named_parameters():
+        ...     if ...:  # some check on name (ex. if 'lora' in name)
+        ...         param.requires_grad = False
+        ```
+
+        Args:
+            adapter_name (`str` or `List[str]`): Name of the adapter(s) to be activated.
+        """
+        if isinstance(adapter_names, str):
+            adapter_names = [adapter_names]
+
+        # Deactivate grads on the inactive adapter and activate grads on the active adapter
+        for layer_name in self.adapter_layer_names:
+            module_dict = getattr(self, layer_name)
+            for key, layer in module_dict.items():
+                if key in adapter_names:
+                    # Note: It is possible that not a single layer is called with requires_grad_(True) here. This may
+                    # happen if a completely different adapter layer is being activated.
+                    layer.requires_grad = True
+                else:
+                    layer.requires_grad = False
+
+        self._active_adapter = adapter_names
+
+    def _all_available_adapter_names(self) -> list[str]:
+        """Return a sorted list of all available adapter names"""
+        adapter_names = set()
+        for name in self.adapter_layer_names + self.other_param_names:
+            # we check each possible attribute and if it's a dict or ModuleDict, we assume that the keys are the adapter
+            # names
+            attr = getattr(self, name)
+            if hasattr(attr, "keys"):
+                adapter_names.update(attr.keys())
+        return sorted(adapter_names)
+
+    def delete_adapter(self, adapter_name: str) -> None:
+        """
+        Delete an adapter from the layer
+
+        This should be called on all adapter layers, or else we will get an inconsistent state.
+
+        This method will also set a new active adapter if the deleted adapter was an active adapter. It is important
+        that the new adapter is chosen in a deterministic way, so that the same adapter is chosen on all layers.
+
+        Args:
+            adapter_name (`str`): The name of the adapter to delete
+
+        """
+        for attr in self.adapter_layer_names + self.other_param_names:
+            if adapter_name in getattr(self, attr):
+                del getattr(self, attr)[adapter_name]
+
+        if adapter_name in self.active_adapters:
+            # choose a new active adapter
+            active_adapters = self.active_adapters[:]
+            active_adapters.remove(adapter_name)
+            if active_adapters:
+                self.set_adapter(active_adapters)
+            else:
+                # no active adapters left, set a new default adapter
+                # here we get the list of all adapters existing adapter names and choose the first one
+                remaining_adapters = self._all_available_adapter_names()
+                if not remaining_adapters:
+                    self.set_adapter([])
+                else:
+                    new_active_adapter = remaining_adapters[0]
+                    warnings.warn(
+                        f"Adapter {adapter_name} was active which is now deleted. Setting active adapter to "
+                        f"{new_active_adapter}."
+                    )
+                    self.set_adapter(remaining_adapters[0])
+
+def check_adapters_to_merge(module: BaseTunerLayer, adapter_names: Optional[list[str]] = None) -> list[str]:
+    """
+    Helper function to check which adapters should be merged.
+
+    Only return those adapters that are not already merged. Give a warning if some or all of the adapters are already
+    merged.
+
+    """
+    if adapter_names is None:
+        adapter_names = module.active_adapters
+
+    if module.merged:
+        merged_adapters = set(module.merged_adapters)
+        adapter_names = [name for name in adapter_names if name not in merged_adapters]
+
+        if adapter_names:
+            warnings.warn(
+                f"Already following adapters were merged {','.join(module.merged_adapters)}. "
+                f"You are now additionally merging {','.join(adapter_names)}."
+            )
+        else:
+            warnings.warn("All adapters are already merged, nothing to do.")
+
+    return adapter_names
+
+def check_target_module_exists(config, key: str) -> bool | re.Match[str] | None:
+    """A helper method to check if the passed module's key name matches any of the target modules in the adapter_config.
+
+    Args:
+        config (`LoraConfig` | `LycorisConfig`): A config to match target modules from
+        key (`str`): A key to search any matches in config
+
+    Returns:
+        `bool` | `re.Match[str]` | `None`: True of match object if key matches any target modules from config, False or
+        None if no match found
+    """
+    if isinstance(config.target_modules, str):
+        target_module_found = re.fullmatch(config.target_modules, key)
+    elif key in config.target_modules:
+        # this module is specified directly in target_modules
+        target_module_found = True
+    else:
+        target_module_found = any(key.endswith(f".{target_key}") for target_key in config.target_modules)
+
+        layer_indexes = getattr(config, "layers_to_transform", None)
+        layers_pattern = getattr(config, "layers_pattern", None)
+
+        is_using_layer_indexes = layer_indexes is not None and (
+            len(layer_indexes) != 0 if isinstance(layer_indexes, list) else True
+        )
+        if is_using_layer_indexes and target_module_found:
+            layer_index = None
+            if layers_pattern is None or len(layers_pattern) == 0:
+                layer_index = re.match(r".*\.[^.]*\.(\d+)\.", key)
+            else:
+                layers_pattern = [layers_pattern] if isinstance(layers_pattern, str) else layers_pattern
+                for pattern in layers_pattern:
+                    layer_index = re.match(rf".*\.{pattern}\.(\d+)\.", key)
+                    if layer_index is not None:
+                        break
+
+            if layer_index is None:
+                target_module_found = False
+            else:
+                layer_index = int(layer_index.group(1))
+                if isinstance(layer_indexes, int):
+                    target_module_found = layer_index == layer_indexes
+                else:
+                    target_module_found = layer_index in layer_indexes
+
+    return target_module_found
```

## mindnlp/peft/utils/__init__.py

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 # ============================================================================
 """utils for peft"""
 from .peft_types import PeftType, TaskType
 from .other import (
     # TRANSFORMERS_MODELS_TO_PREFIX_TUNING_POSTPROCESS_MAPPING,
     TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING,
-    # TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING,
-    # TRANSFORMERS_MODELS_TO_IA3_TARGET_MODULES_MAPPING,
-    # TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING,
+    TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING,
+    TRANSFORMERS_MODELS_TO_IA3_TARGET_MODULES_MAPPING,
+    TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING,
     COMMON_LAYERS_PATTERN,
     CONFIG_NAME,
     WEIGHTS_NAME,
     # SAFETENSORS_WEIGHTS_NAME,
     CLAMP_QUANTILE,
     _set_trainable,
     # add_library_to_model_card,
```

## mindnlp/peft/utils/other.py

```diff
@@ -144,15 +144,15 @@
 
 
 
 def _freeze_adapter(model, adapter_name):
     """
     freeze adapter
     """
-    for n, p in model.named_parameters():
+    for n, p in model.parameters_and_names():
         if adapter_name in n:
             p.requires_grad = False
 
 
 def _set_adapter(model, adapter_name):
     for module in model.modules():
         if isinstance(module, ModulesToSaveWrapper):
@@ -279,17 +279,84 @@
     # "RefinedWebModel": ["query_key_value"],
     # "RefinedWeb": ["query_key_value"],
     "falcon": ["query_key_value"],
     # "btlm": ["c_proj", "c_attn"],
     # "codegen": ["qkv_proj"],
 }
 
-TRANSFORMERS_MODELS_TO_IA3_TARGET_MODULES_MAPPING = {}
-TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING = {}
+TRANSFORMERS_MODELS_TO_IA3_TARGET_MODULES_MAPPING = {
+    "t5": ["k", "v", "wo"],
+    "mt5": ["k", "v", "wi_1"],
+    "gpt2": ["c_attn", "mlp.c_proj"],
+    "bloom": ["query_key_value", "mlp.dense_4h_to_h"],
+    "roberta": ["key", "value", "output.dense"],
+    "opt": ["q_proj", "k_proj", "fc2"],
+    "gptj": ["q_proj", "v_proj", "fc_out"],
+    "gpt_neox": ["query_key_value", "dense_4h_to_h"],
+    "gpt_neo": ["q_proj", "v_proj", "c_proj"],
+    "bart": ["q_proj", "v_proj", "fc2"],
+    "gpt_bigcode": ["c_attn", "mlp.c_proj"],
+    "llama": ["k_proj", "v_proj", "down_proj"],
+    "mistral": ["k_proj", "v_proj", "down_proj"],
+    "mixtral": ["k_proj", "v_proj", "w2"],
+    "bert": ["key", "value", "output.dense"],
+    "deberta-v2": ["key_proj", "value_proj", "output.dense"],
+    "deberta": ["in_proj", "output.dense"],
+    "RefinedWebModel": ["query_key_value", "dense_4h_to_h"],
+    "RefinedWeb": ["query_key_value", "dense_4h_to_h"],
+    "falcon": ["query_key_value", "dense_4h_to_h"],
+    "phi": ["q_proj", "v_proj", "fc2"],
+    "gemma": ["q_proj", "v_proj", "down_proj"],
+}
+
+TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING = {
+    "t5": ["wo"],
+    "mt5": [],
+    "gpt2": ["mlp.c_proj"],
+    "bloom": ["mlp.dense_4h_to_h"],
+    "roberta": ["output.dense"],
+    "opt": ["fc2"],
+    "gptj": ["fc_out"],
+    "gpt_neox": ["dense_4h_to_h"],
+    "gpt_neo": ["c_proj"],
+    "bart": ["fc2"],
+    "gpt_bigcode": ["mlp.c_proj"],
+    "llama": ["down_proj"],
+    "mistral": ["down_proj"],
+    "mixtral": ["w2"],
+    "bert": ["output.dense"],
+    "deberta-v2": ["output.dense"],
+    "deberta": ["output.dense"],
+    "RefinedWeb": ["dense_4h_to_h"],
+    "RefinedWebModel": ["dense_4h_to_h"],
+    "falcon": ["dense_4h_to_h"],
+    "phi": ["fc2"],
+    "gemma": ["down_proj"],
+}
 COMMON_LAYERS_PATTERN = ["layers", "h", "block", "blocks", "layer"]
-TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING = {}
+TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING = {
+    "t5": ["q", "k", "v", "o", "wi", "wo"],
+    # "mt5": ["q", "k", "v", "o", "wi_0", "wi_1", "wo"],
+    "bart": ["q_proj", "k_proj", "v_proj", "out_proj", "fc1", "fc2"],
+    "gpt2": ["c_attn"],
+    "bloom": ["query_key_value"],
+    "opt": ["q_proj", "k_proj", "v_proj", "out_proj", "fc1", "fc2"],
+    # "gptj": ["q_proj", "v_proj"],
+    # "gpt_neox": ["query_key_value"],
+    "gpt_neo": ["q_proj", "v_proj"],
+    "llama": ["q_proj", "v_proj"],
+    "bert": ["query", "value"],
+    "roberta": ["query", "key", "value", "dense"],
+    # "xlm-roberta": ["query", "value"],
+    # "electra": ["query", "value"],
+    "deberta-v2": ["query_proj", "key_proj", "value_proj", "dense"],
+    "gpt_bigcode": ["c_attn"],
+    "deberta": ["in_proj"],
+    # "layoutlm": ["query", "value"],
+    "falcon": ["query_key_value"],
+}
 
 
 WEIGHTS_NAME = "adapter_model.ckpt"
 CONFIG_NAME = "adapter_config.json"
 
 CLAMP_QUANTILE = 0.99
```

## mindnlp/peft/utils/peft_types.py

```diff
@@ -21,17 +21,17 @@
     """
     PeftType.
     """
     # PROMPT_TUNING = "PROMPT_TUNING"
     # P_TUNING = "P_TUNING"
     # PREFIX_TUNING = "PREFIX_TUNING"
     LORA = "LORA"
-    # ADALORA = "ADALORA"
-    # ADAPTION_PROMPT = "ADAPTION_PROMPT"
-    # IA3 = "IA3"
+    ADALORA = "ADALORA"
+    ADAPTION_PROMPT = "ADAPTION_PROMPT"
+    IA3 = "IA3"
 
 
 class TaskType(str, enum.Enum):
     """
     TaskType
     """
     SEQ_CLS = "SEQ_CLS"
```

## mindnlp/peft/utils/save_and_load.py

```diff
@@ -51,15 +51,15 @@
         model ([`PeftModel`]): The Peft model. 
     """
 
     config = model.peft_config[adapter_name]
     if state_dict is None:
         # NOTE: state_dict = model.state_dict()
         state_dict = get_data_list(model)
-    if config.peft_type == PeftType.LORA:
+    if config.peft_type in (PeftType.LORA, PeftType.ADALORA):
         # to_return = lora_state_dict(model, bias=model.peft_config.bias)
         # adapted from `https://github.com/microsoft/LoRA/blob/main/loralib/utils.py`
         # to be used directly with the state dict which is necessary when using DeepSpeed or FSDP
         bias = config.bias
         if bias == "none":
             to_return = {k: state_dict[k] for k in state_dict if "lora_" in k}
         elif bias == "all":
@@ -71,14 +71,24 @@
                     to_return[k] = state_dict[k]
                     bias_name = k.split("lora_")[0] + "bias"
                     if bias_name in state_dict:
                         to_return[bias_name] = state_dict[bias_name]
         else:
             raise NotImplementedError
         to_return = {k: v for k, v in to_return.items() if (("lora_" in k and adapter_name in k) or ("bias" in k))}
+        if config.peft_type == PeftType.ADALORA:
+            rank_pattern = config.rank_pattern
+            if rank_pattern is not None:
+                rank_pattern = {k.replace(f".{adapter_name}", ""): v for k, v in rank_pattern.items()}
+                config.rank_pattern = rank_pattern
+                to_return = model.resize_state_dict_by_rank_pattern(rank_pattern, to_return, adapter_name)
+    elif config.peft_type == PeftType.ADAPTION_PROMPT:
+        to_return = {k: state_dict[k] for k in state_dict if k.split(".")[-1].startswith("adaption_")}
+    elif config.peft_type == PeftType.IA3:
+        to_return = {k: state_dict[k] for k in state_dict if "ia3_" in k}
     else:
         raise NotImplementedError
 
     if model.modules_to_save is not None:
         for key, value in state_dict.items():
             if any(f"{module_name}.modules_to_save.{adapter_name}" in key for module_name in model.modules_to_save):
                 to_return[key.replace("modules_to_save.", "")] = value
@@ -93,42 +103,58 @@
 
     Args:
         model ([`PeftModel`]): The Peft model.
         peft_model_state_dict (`dict`): The state dict of the Peft model.
     """
     config = model.peft_config[adapter_name]
     state_dict = {}
+    strict_load = False
     if model.modules_to_save is not None:
         for key, value in peft_model_state_dict.items():
             if any(module_name in key for module_name in model.modules_to_save):
                 for module_name in model.modules_to_save:
                     if module_name in key:
                         key = key.replace(module_name, f"{module_name}.modules_to_save.{adapter_name}")
                         break
             state_dict[key] = value
     else:
         state_dict = peft_model_state_dict
 
-    if config.peft_type == PeftType.LORA:
+    if config.peft_type in (
+        PeftType.LORA,
+        PeftType.IA3,
+        PeftType.ADALORA,
+    ):
         peft_model_state_dict = {}
+        parameter_prefix = {
+            PeftType.IA3: "ia3_",
+            PeftType.LORA: "lora_",
+            PeftType.ADALORA: "lora_",
+        }[config.peft_type]
         for k, v in state_dict.items():
-            if "lora_" in k:
-                suffix = k.split("lora_")[1]
+            if parameter_prefix in k:
+                suffix = k.split(parameter_prefix)[1]
                 if "." in suffix:
                     suffix_to_replace = ".".join(suffix.split(".")[1:])
                     k = k.replace(suffix_to_replace, f"{adapter_name}.{suffix_to_replace}")
                 else:
                     k = f"{k}.{adapter_name}"
                 peft_model_state_dict[k] = v
             else:
                 peft_model_state_dict[k] = v
+        if config.peft_type == PeftType.ADALORA:
+            strict_load = True
+            rank_pattern = config.rank_pattern
+            if rank_pattern is not None:
+                model.resize_modules_by_rank_pattern(rank_pattern, adapter_name)
+    elif config.peft_type == PeftType.ADAPTION_PROMPT:
+        peft_model_state_dict = state_dict
     else:
         raise NotImplementedError
-
-    param_not_load, ckpt_not_load = mindspore.load_param_into_net(model, peft_model_state_dict)
+    param_not_load, ckpt_not_load = mindspore.load_param_into_net(model, peft_model_state_dict, strict_load=strict_load)
 
     return (param_not_load, ckpt_not_load)
 
 
 def load_peft_weights(model_id: str,) -> dict:
     r"""
     A helper method to load the PEFT weights from local storage. Add download logic later.
```

## mindnlp/transformers/__init__.py

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """MindNLP Transformers"""
 from . import models, pipelines
 from .models import *
 from .pipelines import *
+from .generation import *
 from .configuration_utils import PretrainedConfig
 from .modeling_utils import PreTrainedModel
 from .tokenization_utils_base import PreTrainedTokenizerBase, SpecialTokensMixin
 from .tokenization_utils import PreTrainedTokenizer
 from .tokenization_utils_fast import PreTrainedTokenizerFast
 
 __all__ = ['PretrainedConfig', 'PreTrainedModel', 'PreTrainedTokenizerBase',
```

## mindnlp/transformers/configuration_utils.py

```diff
@@ -248,14 +248,15 @@
     @classmethod
     def from_pretrained(
         cls,
         pretrained_model_name_or_path: Union[str, os.PathLike],
         cache_dir: Optional[Union[str, os.PathLike]] = None,
         force_download: bool = False,
         local_files_only: bool = False,
+        mirror: str = 'huggingface',
         **kwargs,
     ) -> "PretrainedConfig":
         r"""
         Instantiate a [`PretrainedConfig`] (or a derived class) from a pretrained model configuration.
 
         Args:
             pretrained_model_name_or_path (`str` or `os.PathLike`):
@@ -329,14 +330,15 @@
         )
         assert config.output_attentions == True
         assert unused_kwargs == {"foo": False}
         ```"""
         kwargs["cache_dir"] = cache_dir
         kwargs["force_download"] = force_download
         kwargs["local_files_only"] = local_files_only
+        kwargs['mirror'] = mirror
 
         config_dict, kwargs = cls.get_config_dict(pretrained_model_name_or_path, **kwargs)
         if "model_type" in config_dict and hasattr(cls, "model_type") and config_dict["model_type"] != cls.model_type:
             logger.warning(
                 f"You are using a model of type {config_dict['model_type']} to instantiate a model of type "
                 f"{cls.model_type}. This is not supported for all configurations of models and can yield errors."
             )
@@ -392,14 +394,15 @@
         force_download = kwargs.pop("force_download", False)
         resume_download = kwargs.pop("resume_download", False)
         proxies = kwargs.pop("proxies", None)
         local_files_only = kwargs.pop("local_files_only", False)
         subfolder = kwargs.pop("subfolder", "")
         token = kwargs.pop('token', None)
         revision = kwargs.pop('revision', 'main')
+        mirror = kwargs.pop('mirror', 'huggingface')
 
         pretrained_model_name_or_path = str(pretrained_model_name_or_path)
 
         is_local = os.path.isdir(pretrained_model_name_or_path)
         if os.path.isfile(os.path.join(subfolder, pretrained_model_name_or_path)):
             # Special case when pretrained_model_name_or_path is a local file
             resolved_config_file = pretrained_model_name_or_path
@@ -421,14 +424,15 @@
                     force_download=force_download,
                     proxies=proxies,
                     resume_download=resume_download,
                     local_files_only=local_files_only,
                     revision=revision,
                     token=token,
                     subfolder=subfolder,
+                    mirror=mirror
                 )
             except EnvironmentError:
                 # Raise any environment error raise by `cached_file`. It will have a helpful error message adapted to
                 # the original exception.
                 raise
             except Exception as exc:
                 # For any other exception, we throw a generic error.
```

## mindnlp/transformers/image_processing_utils.py

```diff
@@ -711,7 +711,44 @@
         size_dict = size
 
     if not is_valid_size_dict(size_dict):
         raise ValueError(
             f"{param_name} must have one of the following set of keys: {VALID_SIZE_DICT_KEYS}, got {size_dict.keys()}"
         )
     return size_dict
+
+def select_best_resolution(original_size: tuple, possible_resolutions: list) -> tuple:
+    """
+    Selects the best resolution from a list of possible resolutions based on the original size.
+
+    This is done by calculating the effective and wasted resolution for each possible resolution.
+
+    The best fit resolution is the one that maximizes the effective resolution and minimizes the wasted resolution.
+
+    Args:
+        original_size (tuple):
+            The original size of the image in the format (height, width).
+        possible_resolutions (list):
+            A list of possible resolutions in the format [(height1, width1), (height2, width2), ...].
+
+    Returns:
+        tuple: The best fit resolution in the format (height, width).
+    """
+    original_height, original_width = original_size
+    best_fit = None
+    max_effective_resolution = 0
+    min_wasted_resolution = float("inf")
+
+    for height, width in possible_resolutions:
+        scale = min(width / original_width, height / original_height)
+        downscaled_width, downscaled_height = int(original_width * scale), int(original_height * scale)
+        effective_resolution = min(downscaled_width * downscaled_height, original_width * original_height)
+        wasted_resolution = (width * height) - effective_resolution
+
+        if effective_resolution > max_effective_resolution or (
+            effective_resolution == max_effective_resolution and wasted_resolution < min_wasted_resolution
+        ):
+            max_effective_resolution = effective_resolution
+            min_wasted_resolution = wasted_resolution
+            best_fit = (height, width)
+
+    return best_fit
```

## mindnlp/transformers/modeling_utils.py

```diff
@@ -33,22 +33,23 @@
 from mindspore._c_expression import Tensor as Tensor_ # pylint: disable=no-name-in-module
 
 from mindnlp.configs import PT_WEIGHTS_NAME, WEIGHTS_NAME, WEIGHTS_INDEX_NAME, PT_WEIGHTS_INDEX_NAME, \
     SAFE_WEIGHTS_NAME, SAFE_WEIGHTS_INDEX_NAME
 from mindnlp.utils.download import is_remote_url, download_url, cached_file, get_checkpoint_shard_files
 from mindnlp.utils import convert_file_size_to_int, logging, ModelOutput, is_safetensors_available
 from mindnlp._legacy.functional import arange
-from mindnlp.utils.serialization import load
+from mindnlp.utils.serialization import load, safe_save_file
 from mindnlp.injection import set_global_fp16
 
 from .generation import GenerationMixin
 from .configuration_utils import PretrainedConfig
 from .generation.configuration_utils import GenerationConfig
 from .activations import get_activation
 
+
 logger = logging.get_logger(__name__)
 
 _init_weights = True
 init_func = mindspore.common.initializer.initializer
 
 
 @contextmanager
@@ -779,14 +780,15 @@
         config: Optional[Union[PretrainedConfig, str, os.PathLike]] = None,
         cache_dir: Optional[Union[str, os.PathLike]] = None,
         ignore_mismatched_sizes: bool = False,
         force_download: bool = False,
         local_files_only: bool = False,
         token: Optional[Union[str, bool]] = None,
         use_safetensors: bool = None,
+        mirror: str = 'huggingface',
         **kwargs,
     ):
         """from_pretrained"""
         state_dict = kwargs.pop("state_dict", None)
         cache_dir = kwargs.pop("cache_dir", None)
         _ = kwargs.pop("from_pt", True)
         force_download = kwargs.pop("force_download", False)
@@ -813,14 +815,15 @@
                 *model_args,
                 cache_dir=cache_dir,
                 return_unused_kwargs=True,
                 force_download=force_download,
                 resume_download=resume_download,
                 proxies=proxies,
                 local_files_only=local_files_only,
+                mirror=mirror,
                 **kwargs,
             )
         else:
             model_kwargs = kwargs
 
         # Load model
         if pretrained_model_name_or_path is not None:
@@ -902,15 +905,16 @@
                         "force_download": force_download,
                         "proxies": proxies,
                         "resume_download": resume_download,
                         "local_files_only": local_files_only,
                         "subfolder": subfolder,
                         "_raise_exceptions_for_missing_entries": False,
                         'revision': revision,
-                        "token": token
+                        "token": token,
+                        'mirror': mirror
                     }
                     # try safetensors
                     resolved_archive_file = cached_file(pretrained_model_name_or_path, filename, **cached_file_kwargs)
                     use_safetensors = resolved_archive_file is not None
 
                     # Since we set _raise_exceptions_for_missing_entries=False, we don't get an exception but a None
                     # result when internet is up, the repo and revision exist, but the file does not.
@@ -988,15 +992,16 @@
                 cache_dir=cache_dir,
                 force_download=force_download,
                 proxies=proxies,
                 resume_download=resume_download,
                 local_files_only=local_files_only,
                 token=token,
                 subfolder=subfolder,
-                revision=revision
+                revision=revision,
+                mirror=mirror,
             )
 
         if pretrained_model_name_or_path is None and state_dict is None:
             raise ValueError("the argument 'pretrained_model_name_or_path' should be "
                              "a string of model name or checkpoint path, but got 'None'.")
 
         config.name_or_path = pretrained_model_name_or_path
@@ -1045,38 +1050,37 @@
         for name, tensor in model.parameters_dict().items():
             id_tensor = id(tensor)
             ptrs[id_tensor].append(name)
 
         # These are all the pointers of shared tensors.
         tied_params = [names for _, names in ptrs.items() if len(names) > 1]
         def load_ckpt(resolved_archive_file):
-            if 'ckpt' not in resolved_archive_file:
+            if not resolved_archive_file.endswith('ckpt'):
                 if use_safetensors or 'safetensors' in resolved_archive_file:
                     from safetensors.numpy import load_file
                     origin_state_dict = load_file(resolved_archive_file)
                     if use_fp16:
                         logger.warning_once("MindSpore do not support bfloat16 dtype, we will automaticlly convert to float16")
-                    new_state_dict = {k: Parameter(Tensor.from_numpy(v.astype(usage_dtype))) for k, v in origin_state_dict.items()}
+                    state_dict = {k: Parameter(Tensor.from_numpy(v.astype(usage_dtype))) for k, v in origin_state_dict.items()}
                 else:
-                    new_state_dict = load(resolved_archive_file)
+                    state_dict = load(resolved_archive_file)
             else:
                 try:
                     state_dict = load_checkpoint(str(resolved_archive_file))
                 except Exception as exc:
                     raise OSError(
                         f"Unable to load weights from mindspore checkpoint file '{resolved_archive_file}'. "
                     ) from exc
 
-                new_state_dict = {}
-                for key, value in state_dict.items():
-                    key = key.replace('gamma', 'weight').replace('beta', 'bias').replace('embedding_table', 'weight')
-                    value.name = value.name.replace('gamma', 'weight').replace('beta', 'bias')\
-                        .replace('embedding_table', 'weight')
-                    new_state_dict[key] = value
-            return new_state_dict
+            state_keys = list(state_dict.keys())
+            for key in state_keys:
+                new_key = key.replace('gamma', 'weight').replace('beta', 'bias').replace('embedding_table', 'weight')
+                if new_key != key:
+                    state_dict[new_key] = state_dict.pop(key)
+            return state_dict
 
         keys_missing = list(model.parameters_dict().keys())
         param_id_set = set()
 
         use_keep_in_fp32_modules = False
         if model._keep_in_fp32_modules:
             use_keep_in_fp32_modules = True
@@ -1385,14 +1389,15 @@
     def save_pretrained(
         self,
         save_directory: Union[str, os.PathLike],
         is_main_process: bool = True,
         state_dict: Optional[dict] = None,
         save_function: Callable = mindspore.save_checkpoint,
         max_shard_size: Union[int, str] = "5GB",
+        safe_serialization: bool = True,
         variant: Optional[str] = None,
         **kwargs,
     ):
         """
         Save a model and its configuration file to a directory, so that it can be re-loaded using the
         [`~PreTrainedModel.from_pretrained`] class method.
 
@@ -1464,15 +1469,16 @@
         # Handle the case where some state_dict keys shouldn't be saved
         if self._keys_to_ignore_on_save is not None:
             for ignore_key in self._keys_to_ignore_on_save:
                 if ignore_key in state_dict.keys():
                     del state_dict[ignore_key]
 
         # Shard the model if it is too big.
-        weights_name = _add_variant(WEIGHTS_NAME, variant)
+        # weights_name = _add_variant(WEIGHTS_NAME, variant)
+        weights_name = SAFE_WEIGHTS_NAME if safe_serialization else WEIGHTS_NAME
 
         shards, index = shard_checkpoint(state_dict, max_shard_size=max_shard_size, weights_name=weights_name)
 
         # Clean the folder from a previous save
         for filename in os.listdir(save_directory):
             full_filename = os.path.join(save_directory, filename)
             # If we have a shard file that is not going to be replaced, we delete it, but only from the main process
@@ -1490,21 +1496,26 @@
                 and is_main_process
                 and reg.fullmatch(filename_no_suffix) is not None
             ):
                 os.remove(full_filename)
 
         # Save the model
         for shard_file, shard in shards.items():
-            save_function(shard, os.path.join(save_directory, shard_file))
+            if safe_serialization:
+                # At some point we will need to deal better with save_function (used for TPU and other distributed
+                # joyfulness), but for now this enough.
+                safe_save_file(shard, os.path.join(save_directory, shard_file), metadata={"format": "np"})
+            else:
+                save_function(shard, os.path.join(save_directory, shard_file))
 
         if index is None:
             path_to_weights = os.path.join(save_directory, _add_variant(WEIGHTS_NAME, variant))
             logger.info(f"Model weights saved in {path_to_weights}")
         else:
-            save_index_file = WEIGHTS_INDEX_NAME
+            save_index_file = SAFE_WEIGHTS_INDEX_NAME if safe_serialization else WEIGHTS_INDEX_NAME
             save_index_file = os.path.join(save_directory, _add_variant(save_index_file, variant))
             # Save the index as well
             with open(save_index_file, "w", encoding="utf-8") as f:
                 content = json.dumps(index, indent=2, sort_keys=True) + "\n"
                 f.write(content)
             logger.info(
                 f"The model is bigger than the maximum size per checkpoint ({max_shard_size}) and is going to be "
@@ -1520,56 +1531,14 @@
         for _, cell in self.cells_and_names():
             if hasattr(cell, "_set_recompute"):
                 cell._set_recompute()
 
     def check_names(self):
         pass
 
-
-    def load_state_dict(self, parameter_dict, strict=False):
-        """
-        Load parameters into network, return parameter list that are not loaded in the network.
-        """
-        if not isinstance(parameter_dict, dict):
-            logger.critical("Failed to combine the net and the parameters.")
-            msg = ("For 'load_param_into_net', the argument 'parameter_dict' should be a dict, "
-                "but got {}.".format(type(parameter_dict)))
-            raise TypeError(msg)
-
-        for key, value in parameter_dict.items():
-            if not isinstance(key, str) or not isinstance(value, (Parameter, str, list)):
-                logger.critical("Load parameters into net failed.")
-                msg = ("For 'parameter_dict', the element in the argument 'parameter_dict' should be a "
-                    "'str' and 'Parameter' , but got {} and {}.".format(type(key), type(value)))
-                raise TypeError(msg)
-
-        param_not_load = []
-        ckpt_not_load = list(parameter_dict.keys())
-        for name, param in self.parameters_and_names():
-            if param.name in parameter_dict:
-                new_param = parameter_dict[name]
-                param.set_data(new_param)
-                ckpt_not_load.remove(name)
-            else:
-                param_not_load.append(name)
-
-        logger.debug("Params not matched(in net but not in parameter_dict):")
-        for param_name in param_not_load:
-            logger.debug("%s", param_name)
-
-        logger.info("Loading parameters into net is finished.")
-        if param_not_load:
-            logger.warning("For 'load_param_into_net', "
-                        "{} parameters in the 'net' are not loaded, because they are not in the "
-                        "'parameter_dict', please check whether the network structure is consistent "
-                        "when training and loading checkpoint.".format(len(param_not_load)))
-            for param_name in param_not_load:
-                logger.warning("{} is not loaded.".format(param_name))
-        return param_not_load, ckpt_not_load
-
 def get_parameter_dtype(parameter: Union[nn.Cell, GenerationMixin, "ModuleUtilsMixin"]):
     """
     Returns the first found floating dtype in parameters if there is one, otherwise returns the last dtype it found.
     """
     last_dtype = None
     for t in parameter.get_parameters():
         last_dtype = t.dtype
```

## mindnlp/transformers/tokenization_utils_base.py

```diff
@@ -1522,14 +1522,15 @@
         cls,
         pretrained_model_name_or_path: Union[str, os.PathLike],
         *init_inputs,
         cache_dir: Optional[Union[str, os.PathLike]] = None,
         force_download: bool = False,
         local_files_only: bool = False,
         token: str = None,
+        mirror: str = 'huggingface',
         **kwargs,
     ):
         r"""
         Instantiate a [`~tokenization_utils_base.PreTrainedTokenizerBase`] (or a derived class) from a predefined
         tokenizer.
 
         Args:
@@ -1654,14 +1655,15 @@
                     force_download=force_download,
                     resume_download=resume_download,
                     proxies=proxies,
                     local_files_only=local_files_only,
                     token=token,
                     subfolder=subfolder,
                     revision=revision,
+                    mirror=mirror,
                     _raise_exceptions_for_missing_entries=False,
                     _raise_exceptions_for_connection_errors=False,
                 )
                 if resolved_config_file is not None:
                     with open(resolved_config_file, encoding="utf-8") as reader:
                         tokenizer_config = json.load(reader)
                         if "fast_tokenizer_files" in tokenizer_config:
@@ -1687,14 +1689,15 @@
                     force_download=force_download,
                     proxies=proxies,
                     resume_download=resume_download,
                     local_files_only=local_files_only,
                     token=token,
                     subfolder=subfolder,
                     revision=revision,
+                    mirror=mirror,
                     _raise_exceptions_for_missing_entries=False,
                     _raise_exceptions_for_connection_errors=False,
                 )
         if len(unresolved_files) > 0:
             logger.info(
                 f"Can't load following files from cache: {unresolved_files} and cannot check if these "
                 "files are necessary for the tokenizer to operate."
```

## mindnlp/transformers/generation/__init__.py

```diff
@@ -16,7 +16,8 @@
 Generation
 """
 from .beam_constraints import *
 from .beam_search import *
 from .logits_process import *
 from .stopping_criteria import *
 from .utils import *
+from .streamers import *
```

## mindnlp/transformers/generation/logits_process.py

```diff
@@ -437,19 +437,21 @@
         if not all(isinstance(i, int) for i in eos_token_id) or any(i < 0 for i in eos_token_id):
             raise ValueError(f"`eos_token_id` has to be a list of positive integers, but is {eos_token_id}")
 
         self.min_length = min_length
         self.eos_token_id = eos_token_id
 
     def __call__(self, input_ids: mindspore.Tensor, scores: mindspore.Tensor) -> mindspore.Tensor:
-        cur_len = input_ids.shape[-1]
-        if cur_len < self.min_length:
-            for i in self.eos_token_id:
-                scores[:, i] = -float("inf")
-        return scores
+        vocab_tensor = ops.arange(scores.shape[-1])
+        eos_token_id = mindspore.tensor(self.eos_token_id)
+        eos_token_mask = vocab_tensor == eos_token_id
+        scores_processed = scores.copy()
+        if input_ids.shape[-1] < self.min_length:
+            scores_processed = ops.where(eos_token_mask, -math.inf, scores)
+        return scores_processed
 
 
 class MinNewTokensLengthLogitsProcessor(LogitsProcessor):
     r"""
     [`LogitsProcessor`] enforcing a min-length of new tokens by setting EOS (End-Of-Sequence) token probability to 0.
 
     Args:
@@ -547,15 +549,16 @@
             eos_token_id = [eos_token_id]
         self.eos_token_id = eos_token_id
 
     def __call__(self, input_ids: mindspore.Tensor, scores: mindspore.Tensor) -> mindspore.Tensor:
         cur_len = input_ids.shape[-1]
         if cur_len == self.max_length - 1:
             num_tokens = scores.shape[1]
-            scores[:, [i for i in range(num_tokens) if i not in self.eos_token_id]] = -float("inf")
+            scores[:, [i for i in range(num_tokens) if i not in self.eos_token_id]] = \
+                float(np.finfo(mindspore.dtype_to_nptype(scores.dtype)).min)
             for i in self.eos_token_id:
                 scores[:, i] = 0
         return scores
 
 
 class InfNanRemoveLogitsProcessor(LogitsProcessor):
     r"""
```

## mindnlp/transformers/generation/utils.py

```diff
@@ -646,42 +646,14 @@
             inputs, input_name = model_kwargs["inputs_embeds"], "inputs_embeds"
 
         # 4. if `inputs` is still None, try to create `input_ids` from BOS token
         inputs = self._maybe_initialize_input_ids_for_generation(inputs, bos_token_id, model_kwargs)
         return inputs, input_name, model_kwargs
 
     def _maybe_initialize_input_ids_for_generation(
-        self,
-        inputs: Optional[mindspore.Tensor] = None,
-        bos_token_id: Optional[int] = None,
-        model_kwargs: Optional[Dict[str, mindspore.Tensor]] = None,
-    ) -> mindspore.Tensor:
-        """Initializes input ids for generation, if necessary."""
-        if inputs is not None:
-            return inputs
-
-        encoder_outputs = model_kwargs.get("encoder_outputs")
-        if self.config.is_encoder_decoder and encoder_outputs is not None:
-            # make dummy input_ids with value -100, as a sanity check ensuring that they won't be used for encoding
-            shape = encoder_outputs.last_hidden_state.shape[:-1]
-            return ops.ones(shape, dtype=mindspore.int64) * -100
-
-        if bos_token_id is None:
-            raise ValueError("`bos_token_id` has to be defined when no `input_ids` are provided.")
-
-        # If there is some tensor in `model_kwargs`, we can infer the batch size from it. This is helpful with
-        # soft-prompting or in multimodal implementations built on top of decoder-only language models.
-        batch_size = 1
-        for value in model_kwargs.values():
-            if isinstance(value, mindspore.Tensor):
-                batch_size = value.shape[0]
-                break
-        return ops.ones((batch_size, 1), dtype=mindspore.int64) * bos_token_id
-
-    def _maybe_initialize_input_ids_for_generation(
             self,
             inputs: Optional[mindspore.Tensor] = None,
             bos_token_id: Optional[int] = None,
             model_kwargs: Optional[Dict[str, mindspore.Tensor]] = None,
         ) -> mindspore.Tensor:
         """Initializes input ids for generation, if necessary."""
         if inputs is not None:
@@ -689,24 +661,28 @@
 
         encoder_outputs = model_kwargs.get("encoder_outputs")
         if self.config.is_encoder_decoder and encoder_outputs is not None:
             # make dummy input_ids with value -100, as a sanity check ensuring that they won't be used for encoding
             shape = encoder_outputs.last_hidden_state.shape[:-1]
             return ops.ones(shape, dtype=mindspore.int64) * -100
 
-        if bos_token_id is None:
-            raise ValueError("`bos_token_id` has to be defined when no `input_ids` are provided.")
-
         # If there is some tensor in `model_kwargs`, we can infer the batch size from it. This is helpful with
         # soft-prompting or in multimodal implementations built on top of decoder-only language models.
         batch_size = 1
         for value in model_kwargs.values():
             if isinstance(value, mindspore.Tensor):
                 batch_size = value.shape[0]
                 break
+
+        if "inputs_embeds" in model_kwargs:
+            return ops.ones((batch_size, 0), dtype=mindspore.int64)
+
+        if bos_token_id is None:
+            raise ValueError("`bos_token_id` has to be defined when no `input_ids` are provided.")
+
         return ops.ones((batch_size, 1), dtype=mindspore.int64) * bos_token_id
 
     def _can_retrieve_inputs_from_name(
         self, inputs: Optional[mindspore.Tensor], name: str, model_kwargs: Dict[str, mindspore.Tensor]
     ) -> mindspore.Tensor:
         """
         If `inputs` is None and `name` is in both forward function and keyword arguments, then inputs can be retrieved
```

## mindnlp/transformers/models/__init__.py

```diff
@@ -44,17 +44,19 @@
     bloom,
     bridgetower,
     bros,
     byt5,
     clip,
     codegen,
     convbert,
+    convnext,
     cpm,
     cpmant,
     cpmbee,
+    cvt,
     deberta,
     distilbert,
     efficientnet,
     electra,
     encodec,
     esm,
     ernie,
@@ -71,40 +73,52 @@
     gpt_pangu,
     graphormer,
     hubert,
     jetmoe,
     layoutlm,
     layoutlmv2,
     llama,
+    llava,
+    llava_next,
     longformer,
     luke,
     mamba,
     mbart,
     megatron_bert,
     minicpm,
     mistral,
     mixtral,
     mobilebert,
+    mpnet,
+    mpt,
     musicgen,
     musicgen_melody,
     nezha,
+    olmo,
+    openelm,
     opt,
     pegasus,
     phi,
+    phi3,
     pop2piano,
     qwen2,
     qwen2_moe,
     reformer,
+    resnet,
     roberta,
     rwkv,
+    sam,
     seamless_m4t,
     seamless_m4t_v2,
+    segformer,
     starcoder2,
     t5,
+    timesformer,
     tinybert,
+    vipllava,
     wav2vec2,
     wav2vec2_with_lm,
     whisper,
     xlm,
     xlm_roberta,
     xlnet
 )
@@ -137,17 +151,19 @@
 from .bloom import *
 from .bridgetower import *
 from .bros import *
 from .byt5 import *
 from .clip import *
 from .codegen import *
 from .convbert import *
+from .convnext import *
 from .cpm import *
 from .cpmant import *
 from .cpmbee import *
+from .cvt import *
 from .deberta import *
 from .distilbert import *
 from .efficientnet import *
 from .electra import *
 from .encodec import *
 from .esm import *
 from .ernie import *
@@ -164,40 +180,52 @@
 from .gpt2 import *
 from .graphormer import *
 from .hubert import *
 from .jetmoe import *
 from .layoutlm import *
 from .layoutlmv2 import *
 from .llama import *
+from .llava import *
+from .llava_next import *
 from .longformer import *
 from .luke import *
 from .mamba import *
 from .mbart import *
 from .megatron_bert import *
 from .minicpm import *
 from .mistral import *
 from .mixtral import *
 from .mobilebert import *
+from .mpnet import *
+from .mpt import *
 from .musicgen import *
 from .musicgen_melody import *
 from .nezha import *
+from .olmo import *
+from .openelm import *
 from .opt import *
 from .pegasus import *
 from .phi import *
+from .phi3 import *
 from .pop2piano import *
 from .qwen2 import *
 from .qwen2_moe import *
 from .reformer import *
+from .resnet import *
 from .roberta import *
 from .rwkv import *
+from .sam import *
 from .seamless_m4t import *
 from .seamless_m4t_v2 import *
+from .segformer import *
 from .starcoder2 import *
 from .tinybert import *
 from .t5 import *
+from .timesformer import *
+from .vipllava import *
 from .whisper import *
 from .wav2vec2 import *
 from .wav2vec2_with_lm import *
 from .xlm import *
 from .xlm_roberta import *
 from .xlnet import *
 
@@ -230,17 +258,19 @@
 __all__.extend(bloom.__all__)
 __all__.extend(bridgetower.__all__)
 __all__.extend(bros.__all__)
 __all__.extend(byt5.__all__)
 __all__.extend(clip.__all__)
 __all__.extend(codegen.__all__)
 __all__.extend(convbert.__all__)
+__all__.extend(convnext.__all__)
 __all__.extend(cpm.__all__)
 __all__.extend(cpmant.__all__)
 __all__.extend(cpmbee.__all__)
+__all__.extend(cvt.__all__)
 __all__.extend(deberta.__all__)
 __all__.extend(distilbert.__all__)
 __all__.extend(efficientnet.__all__)
 __all__.extend(electra.__all__)
 __all__.extend(encodec.__all__)
 __all__.extend(ernie.__all__)
 __all__.extend(ernie_m.__all__)
@@ -257,39 +287,51 @@
 __all__.extend(gpt2.__all__)
 __all__.extend(graphormer.__all__)
 __all__.extend(hubert.__all__)
 __all__.extend(jetmoe.__all__)
 __all__.extend(layoutlm.__all__)
 __all__.extend(layoutlmv2.__all__)
 __all__.extend(llama.__all__)
+__all__.extend(llava.__all__)
+__all__.extend(llava_next.__all__)
 __all__.extend(longformer.__all__)
 __all__.extend(luke.__all__)
 __all__.extend(mamba.__all__)
 __all__.extend(mbart.__all__)
 __all__.extend(megatron_bert.__all__)
 __all__.extend(minicpm.__all__)
 __all__.extend(mistral.__all__)
 __all__.extend(mixtral.__all__)
 __all__.extend(mobilebert.__all__)
+__all__.extend(mpnet.__all__)
+__all__.extend(mpt.__all__)
 __all__.extend(musicgen.__all__)
 __all__.extend(musicgen_melody.__all__)
 __all__.extend(nezha.__all__)
+__all__.extend(olmo.__all__)
+__all__.extend(openelm.__all__)
 __all__.extend(opt.__all__)
 __all__.extend(pegasus.__all__)
 __all__.extend(phi.__all__)
+__all__.extend(phi3.__all__)
 __all__.extend(pop2piano.__all__)
 __all__.extend(qwen2.__all__)
 __all__.extend(qwen2_moe.__all__)
 __all__.extend(reformer.__all__)
+__all__.extend(resnet.__all__)
 __all__.extend(roberta.__all__)
 __all__.extend(rwkv.__all__)
+__all__.extend(sam.__all__)
 __all__.extend(seamless_m4t.__all__)
 __all__.extend(seamless_m4t_v2.__all__)
+__all__.extend(segformer.__all__)
 __all__.extend(starcoder2.__all__)
-__all__.extend(tinybert.__all__)
 __all__.extend(t5.__all__)
+__all__.extend(timesformer.__all__)
+__all__.extend(tinybert.__all__)
+__all__.extend(vipllava.__all__)
 __all__.extend(whisper.__all__)
 __all__.extend(wav2vec2.__all__)
 __all__.extend(wav2vec2_with_lm.__all__)
 __all__.extend(xlm.__all__)
 __all__.extend(xlm_roberta.__all__)
 __all__.extend(xlnet.__all__)
```

## mindnlp/transformers/models/auto/auto_factory.py

```diff
@@ -65,37 +65,40 @@
             f"Model type should be one of {', '.join(c.__name__ for c in cls._model_mapping.keys())}."
         )
 
     @classmethod
     def from_pretrained(cls, pretrained_model_name_or_path, *model_args, **kwargs):
         config = kwargs.pop("config", None)
         _ = kwargs.get('from_pt', True)
+        mirror = kwargs.get('mirror', 'huggingface')
+        revision = kwargs.get('revision', 'main')
         token = kwargs.get('token', None)
         if not isinstance(config, PretrainedConfig):
             kwargs_orig = copy.deepcopy(kwargs)
             # ensure not to pollute the config object with torch_dtype="auto" - since it's
             # meaningless in the context of the config object - torch.dtype values are acceptable
             if kwargs.get("ms_dtype", None) == "auto":
                 _ = kwargs.pop("ms_dtype")
             # to not overwrite the quantization_config if config has a quantization_config
             if kwargs.get("quantization_config", None) is not None:
                 _ = kwargs.pop("quantization_config")
-
             config, kwargs = AutoConfig.from_pretrained(
                 pretrained_model_name_or_path,
                 return_unused_kwargs=True,
                 **kwargs,
             )
             # if torch_dtype=auto was passed here, ensure to pass it on
             if kwargs_orig.get("torch_dtype", None) == "auto":
                 kwargs["torch_dtype"] = "auto"
             if kwargs_orig.get("quantization_config", None) is not None:
                 kwargs["quantization_config"] = kwargs_orig["quantization_config"]
 
         kwargs['token'] = token
+        kwargs['mirror'] = mirror
+        kwargs['revision'] = revision
         if type(config) in cls._model_mapping.keys():
             model_class = _get_model_class(config, cls._model_mapping)
             return model_class.from_pretrained(
                 pretrained_model_name_or_path, *model_args, config=config, **kwargs
             )
         raise ValueError(
             f"Unrecognized configuration class {config.__class__} for this kind of AutoModel: {cls.__name__}.\n"
```

## mindnlp/transformers/models/auto/configuration_auto.py

```diff
@@ -19,14 +19,15 @@
 import warnings
 from collections import OrderedDict
 from typing import List, Union
 
 from mindnlp.configs import CONFIG_NAME
 from mindnlp.utils import logging
 from mindnlp.transformers.configuration_utils import PretrainedConfig
+
 logger = logging.get_logger(__name__)
 
 CONFIG_MAPPING_NAMES = OrderedDict(
     [
         # Add configs here
         ("albert", "AlbertConfig"),
         ("align", "AlignConfig"),
@@ -46,62 +47,81 @@
         ("blenderbot", "BlenderbotConfig"),
         ("blenderbot-small", "BlenderbotSmallConfig"),
         ("blip", "BlipConfig"),
         ("blip-2", "Blip2Config"),
         ("bloom", "BloomConfig"),
         ("bridgetower", "BridgeTowerConfig"),
         ("bros", "BrosConfig"),
-        ('chatglm', 'ChatGLMConfig'),
+        ("chatglm", "ChatGLMConfig"),
         ("clip", "CLIPConfig"),
         ("clip_vision_model", "CLIPVisionConfig"),
         ("codegen", "CodeGenConfig"),
+        ("convbert", "ConvBertConfig"),
+        ("convnext", "ConvNextConfig"),
         ("cpmant", "CpmAntConfig"),
         ("cpmbee", "CpmBeeConfig"),
+        ("cvt", "CvtConfig"),
         ("deberta", "DebertaConfig"),
         ("distilbert", "DistilBertConfig"),
         ("encodec", "EncodecConfig"),
         ("esm", "EsmConfig"),
         ("falcon", "FalconConfig"),
         ("gemma", "GemmaConfig"),
         ("gpt2", "GPT2Config"),
-        ('gpt_bigcode', 'GPTBigCodeConfig'),
+        ("gpt_bigcode", "GPTBigCodeConfig"),
+        ("gpt_neox", "GPTNeoXConfig"),
         ("gpt_pangu", "GPTPanguConfig"),
-        ('hubert', 'HubertConfig'),
-        ('jetmoe', 'JetMoEConfig'),
+        ("hubert", "HubertConfig"),
+        ("jetmoe", "JetMoEConfig"),
+        ("llama", "LlamaConfig"),
+        ("llava", "LlavaConfig"),
+        ("llava_next", "LlavaNextConfig"),
         ("mamba", "MambaConfig"),
         ("mbart", "MBartConfig"),
-        ('minicpm', 'MiniCPMConfig'),
+        ("minicpm", "MiniCPMConfig"),
         ("mistral", "MistralConfig"),
         ("mixtral", "MixtralConfig"),
         ("musicgen", "MusicgenConfig"),
         ("musicgen_melody", "MusicgenMelodyConfig"),
-        ('mt5', 'MT5Config'),
-        ("opt", 'OPTConfig'),
+        ("mt5", "MT5Config"),
+        ("olmo", "OlmoConfig"),
+        ("openelm", "OpenELMConfig"),
+        ("opt", "OPTConfig"),
+        ("pegasus", "PegasusConfig"),
         ("phi", "PhiConfig"),
+        ("phi3", "Phi3Config"),
         ("qwen2", "Qwen2Config"),
         ("qwen2_moe", "Qwen2MoeConfig"),
         ("reformer", "ReformerConfig"),
+        ("resnet", "ResNetConfig"),
         ("roberta", "RobertaConfig"),
+        ("sam", "SamConfig"),
+        ("segformer", "SegformerConfig"),
         ("starcoder2", "Starcoder2Config"),
-        ('t5', 'T5Config'),
-        ('wav2vec2', 'Wav2Vec2Config'),
+        ("t5", "T5Config"),
+        ("timesformer", "TimesformerConfig"),
+        ("vipllava", "VipLlavaConfig"),
+        ("wav2vec2", "Wav2Vec2Config"),
         ("whisper", "WhisperConfig"),
-        ('xlm-roberta', 'XLMRobertaConfig'),
+        ("xlm-roberta", "XLMRobertaConfig"),
         ("layoutlmv2", "LayoutLMv2Config"),
         ("xlnet", "XLNetConfig"),
     ]
 )
 
 CONFIG_ARCHIVE_MAP_MAPPING_NAMES = OrderedDict(
     [
         # Add archive maps here)
         ("albert", "ALBERT_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("align", "ALIGN_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("altclip", "ALTCLIP_PRETRAINED_CONFIG_ARCHIVE_MAP"),
-        ("audio-spectrogram-transformer", "AUDIO_SPECTROGRAM_TRANSFORMER_PRETRAINED_CONFIG_ARCHIVE_MAP"),
+        (
+            "audio-spectrogram-transformer",
+            "AUDIO_SPECTROGRAM_TRANSFORMER_PRETRAINED_CONFIG_ARCHIVE_MAP",
+        ),
         ("autoformer", "AUTOFORMER_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("bark", "BARK_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("bart", "BART_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("beit", "BEIT_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("bert", "BERT_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("big_bird", "BIG_BIRD_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("bigbird_pegasus", "BIGBIRD_PEGASUS_PRETRAINED_CONFIG_ARCHIVE_MAP"),
@@ -261,15 +281,18 @@
         ("swin", "SWIN_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("swin2sr", "SWIN2SR_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("swinv2", "SWINV2_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("switch_transformers", "SWITCH_TRANSFORMERS_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("t5", "T5_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("table-transformer", "TABLE_TRANSFORMER_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("tapas", "TAPAS_PRETRAINED_CONFIG_ARCHIVE_MAP"),
-        ("time_series_transformer", "TIME_SERIES_TRANSFORMER_PRETRAINED_CONFIG_ARCHIVE_MAP"),
+        (
+            "time_series_transformer",
+            "TIME_SERIES_TRANSFORMER_PRETRAINED_CONFIG_ARCHIVE_MAP",
+        ),
         ("timesformer", "TIMESFORMER_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("transfo-xl", "TRANSFO_XL_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("tvlt", "TVLT_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("unispeech", "UNISPEECH_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("unispeech-sat", "UNISPEECH_SAT_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("van", "VAN_PRETRAINED_CONFIG_ARCHIVE_MAP"),
         ("videomae", "VIDEOMAE_PRETRAINED_CONFIG_ARCHIVE_MAP"),
@@ -414,14 +437,16 @@
         ("layoutlmv3", "LayoutLMv3"),
         ("layoutxlm", "LayoutXLM"),
         ("led", "LED"),
         ("levit", "LeViT"),
         ("lilt", "LiLT"),
         ("llama", "LLaMA"),
         ("llama2", "Llama2"),
+        ("llava", "LLaVa"),
+        ("llava_next", "LLaVA-NeXT"),
         ("longformer", "Longformer"),
         ("longt5", "LongT5"),
         ("luke", "LUKE"),
         ("lxmert", "LXMERT"),
         ("m2m_100", "M2M100"),
         ("mamba", "Mamba"),
         ("marian", "Marian"),
@@ -456,25 +481,28 @@
         ("mvp", "MVP"),
         ("nat", "NAT"),
         ("nezha", "Nezha"),
         ("nllb", "NLLB"),
         ("nllb-moe", "NLLB-MOE"),
         ("nougat", "Nougat"),
         ("nystromformer", "Nyströmformer"),
+        ("olmo", "OLMo"),
+        ("openelm", "OpenELM"),
         ("oneformer", "OneFormer"),
         ("open-llama", "OpenLlama"),
         ("openai-gpt", "OpenAI GPT"),
         ("opt", "OPT"),
         ("owlv2", "OWLv2"),
         ("owlvit", "OWL-ViT"),
         ("pegasus", "Pegasus"),
         ("pegasus_x", "PEGASUS-X"),
         ("perceiver", "Perceiver"),
         ("persimmon", "Persimmon"),
         ("phi", "Phi"),
+        ("phi3", "Phi3"),
         ("phobert", "PhoBERT"),
         ("pix2struct", "Pix2Struct"),
         ("plbart", "PLBart"),
         ("poolformer", "PoolFormer"),
         ("pop2piano", "Pop2Piano"),
         ("prophetnet", "ProphetNet"),
         ("pvt", "PVT"),
@@ -526,14 +554,15 @@
         ("umt5", "UMT5"),
         ("unispeech", "UniSpeech"),
         ("unispeech-sat", "UniSpeechSat"),
         ("upernet", "UPerNet"),
         ("van", "VAN"),
         ("videomae", "VideoMAE"),
         ("vilt", "ViLT"),
+        ("vipllava", "VipLlava"),
         ("vision-encoder-decoder", "Vision Encoder decoder"),
         ("vision-text-dual-encoder", "VisionTextDualEncoder"),
         ("visual_bert", "VisualBERT"),
         ("vit", "ViT"),
         ("vit_hybrid", "ViT Hybrid"),
         ("vit_mae", "ViTMAE"),
         ("vit_msn", "ViTMSN"),
@@ -559,22 +588,22 @@
         ("xmod", "X-MOD"),
         ("yolos", "YOLOS"),
         ("yoso", "YOSO"),
     ]
 )
 
 DEPRECATED_MODELS = [
-    "bort",
-    "mctct",
-    "mmbt",
-    "open_llama",
-    "retribert",
-    "tapex",
-    "trajectory_transformer",
-    "van",
+    # "bort",
+    # "mctct",
+    # "mmbt",
+    # "open_llama",
+    # "retribert",
+    # "tapex",
+    # "trajectory_transformer",
+    # "van",
 ]
 
 SPECIAL_MODEL_TYPE_TO_MODULE_NAME = OrderedDict(
     [
         ("openai-gpt", "openai"),
         ("data2vec-audio", "data2vec"),
         ("data2vec-text", "data2vec"),
@@ -627,44 +656,52 @@
         if key in self._extra_content:
             return self._extra_content[key]
         if key not in self._mapping:
             raise KeyError(key)
         value = self._mapping[key]
         module_name = model_type_to_module_name(key)
         if module_name not in self._modules:
-            self._modules[module_name] = importlib.import_module(f".{module_name}", "mindnlp.transformers.models")
+            self._modules[module_name] = importlib.import_module(
+                f".{module_name}", "mindnlp.transformers.models"
+            )
         if hasattr(self._modules[module_name], value):
             return getattr(self._modules[module_name], value)
 
         # Some of the mappings have entries model_type -> config of another model type. In that case we try to grab the
         # object at the top level.
         transformers_module = importlib.import_module("mindnlp.transformers")
         return getattr(transformers_module, value)
 
     def keys(self):
         return list(self._mapping.keys()) + list(self._extra_content.keys())
 
     def values(self):
-        return [self[k] for k in self._mapping.keys()] + list(self._extra_content.values())
+        return [self[k] for k in self._mapping.keys()] + list(
+            self._extra_content.values()
+        )
 
     def items(self):
-        return [(k, self[k]) for k in self._mapping.keys()] + list(self._extra_content.items())
+        return [(k, self[k]) for k in self._mapping.keys()] + list(
+            self._extra_content.items()
+        )
 
     def __iter__(self):
         return iter(list(self._mapping.keys()) + list(self._extra_content.keys()))
 
     def __contains__(self, item):
         return item in self._mapping or item in self._extra_content
 
     def register(self, key, value, exist_ok=False):
         """
         Register a new configuration in this mapping.
         """
         if key in self._mapping.keys() and not exist_ok:
-            raise ValueError(f"'{key}' is already used by a Transformers config, pick another name.")
+            raise ValueError(
+                f"'{key}' is already used by a Transformers config, pick another name."
+            )
         self._extra_content[key] = value
 
 
 CONFIG_MAPPING = _LazyConfigMapping(CONFIG_MAPPING_NAMES)
 
 
 class _LazyLoadAllMappings(OrderedDict):
@@ -719,29 +756,36 @@
         return iter(self._data)
 
     def __contains__(self, item):
         self._initialize()
         return item in self._data
 
 
-ALL_PRETRAINED_CONFIG_ARCHIVE_MAP = _LazyLoadAllMappings(CONFIG_ARCHIVE_MAP_MAPPING_NAMES)
+ALL_PRETRAINED_CONFIG_ARCHIVE_MAP = _LazyLoadAllMappings(
+    CONFIG_ARCHIVE_MAP_MAPPING_NAMES
+)
 
 
 def _get_class_name(model_class: Union[str, List[str]]):
     if isinstance(model_class, (list, tuple)):
         return " or ".join([f"[`{c}`]" for c in model_class if c is not None])
     return f"[`{model_class}`]"
 
 
 def _list_model_options(indent, config_to_class=None, use_model_types=True):
     if config_to_class is None and not use_model_types:
-        raise ValueError("Using `use_model_types=False` requires a `config_to_class` dictionary.")
+        raise ValueError(
+            "Using `use_model_types=False` requires a `config_to_class` dictionary."
+        )
     if use_model_types:
         if config_to_class is None:
-            model_type_to_name = {model_type: f"[`{config}`]" for model_type, config in CONFIG_MAPPING_NAMES.items()}
+            model_type_to_name = {
+                model_type: f"[`{config}`]"
+                for model_type, config in CONFIG_MAPPING_NAMES.items()
+            }
         else:
             model_type_to_name = {
                 model_type: _get_class_name(model_class)
                 for model_type, model_class in config_to_class.items()
                 if model_type in MODEL_NAMES_MAPPING
             }
         lines = [
@@ -751,15 +795,16 @@
     else:
         config_to_name = {
             CONFIG_MAPPING_NAMES[config]: _get_class_name(clas)
             for config, clas in config_to_class.items()
             if config in CONFIG_MAPPING_NAMES
         }
         config_to_model_name = {
-            config: MODEL_NAMES_MAPPING[model_type] for model_type, config in CONFIG_MAPPING_NAMES.items()
+            config: MODEL_NAMES_MAPPING[model_type]
+            for model_type, config in CONFIG_MAPPING_NAMES.items()
         }
         lines = [
             f"{indent}- [`{config_name}`] configuration class:"
             f" {config_to_name[config_name]} ({config_to_model_name[config_name]} model)"
             for config_name in sorted(config_to_name.keys())
         ]
     return "\n".join(lines)
@@ -772,15 +817,17 @@
         i = 0
         while i < len(lines) and re.search(r"^(\s*)List options\s*$", lines[i]) is None:
             i += 1
         if i < len(lines):
             indent = re.search(r"^(\s*)List options\s*$", lines[i]).groups()[0]
             if use_model_types:
                 indent = f"{indent}    "
-            lines[i] = _list_model_options(indent, config_to_class=config_to_class, use_model_types=use_model_types)
+            lines[i] = _list_model_options(
+                indent, config_to_class=config_to_class, use_model_types=use_model_types
+            )
             docstrings = "\n".join(lines)
         else:
             raise ValueError(
                 f"The function {fn} should have an empty 'List options' in its docstring as placeholder, current"
                 f" docstring is:\n{docstrings}"
             )
         fn.__doc__ = docstrings
@@ -895,15 +942,17 @@
         True
 
         >>> unused_kwargs
         {'foo': False}
         ```"""
         kwargs["name_or_path"] = pretrained_model_name_or_path
 
-        config_dict, unused_kwargs = PretrainedConfig.get_config_dict(pretrained_model_name_or_path, **kwargs)
+        config_dict, unused_kwargs = PretrainedConfig.get_config_dict(
+            pretrained_model_name_or_path, **kwargs
+        )
         if "model_type" in config_dict:
             config_class = CONFIG_MAPPING[config_dict["model_type"]]
             return config_class.from_dict(config_dict, **unused_kwargs)
         # Fallback: use pattern matching on the string.
         # We go from longer names to shorter names to catch roberta before bert (for instance)
         for pattern in sorted(CONFIG_MAPPING.keys(), key=len, reverse=True):
             if pattern in str(pretrained_model_name_or_path).lower():
```

## mindnlp/transformers/models/auto/image_processing_auto.py

```diff
@@ -378,14 +378,15 @@
                 logger.warning(
                     "Could not find image processor auto map in the image processor config or the model config. "
                     "Loading based on pattern matching with the model's feature extractor configuration. Please open a "
                     "PR/issue to update `preprocessor_config.json` to use `AutoImageProcessor` instead of "
                     "`AutoFeatureExtractor`. This warning will be removed in v4.40."
                 )
 
+        print(image_processor_class)
         # If we don't find the image processor class in the image processor config, let's try the model config.
         if image_processor_class is None and image_processor_auto_map is None:
             if not isinstance(config, PretrainedConfig):
                 config = AutoConfig.from_pretrained(pretrained_model_name_or_path, **kwargs)
             # It could be in `config.image_processor_type``
             image_processor_class = getattr(config, "image_processor_type", None)
             if hasattr(config, "auto_map") and "AutoImageProcessor" in config.auto_map:
```

## mindnlp/transformers/models/auto/modeling_auto.py

```diff
@@ -55,42 +55,53 @@
         ("codegen", "CodeGenModel"),
         ("cpmant", "CpmAntModel"),
         ("cpmbee", "CpmBeeModel"),
         ("chatglm", "ChatGLMModel"),
         ("clip", "CLIPModel"),
         ("clip_vision_model", "CLIPVisionModel"),
         ("convbert", "ConvBertModel"),
+        ("convnext", "ConvNextModel"),
+        ("cvt", "CvtModel"),
         ("deberta", "DebertaModel"),
         ('encodec', 'EncodecModel'),
         ("esm", "EsmModel"),
         ("ernie", "ErnieModel"),
         ("ernie_m", "ErnieMModel"),
         ("falcon", "FalconModel"),
         ("gemma", "GemmaModel"),
         ("gpt_bigcode", "GPTBigCodeModel"),
         ("gpt", "GPTModel"),
         ("gpt2", "GPT2Model"),
         ("gpt_pangu", "GPTPanguModel"),
         ("layoutlmv2", "LayoutLMv2Model"),
         ("longformer", "LongformerModel"),
         ("jetmoe", "JetMoEModel"),
+        ("llama", "LlamaModel"),
         ("mamba", "MambaModel"),
         ('mbart', 'MBartModel'),
         ('minicpm', 'MiniCPMModel'),
         ("mistral", "MistralModel"),
         ("mixtral", "MixtralModel"),
+        ("olmo", "OlmoModel"),
+        ("openelm", "OpenELMModel"),
         ("opt", "OPTModel"),
+        ("pegasus", "PegasusModel"),
         ("phi", "PhiModel"),
+        ("phi3", "Phi3Model"),
         ("qwen2", "Qwen2Model"),
         ("qwen2_moe", "Qwen2MoeModel"),
         ("reformer", "ReformerModel"),
+        ("resnet", "ResNetModel"),
         ("roberta", "RobertaModel"),
         ("rwkv", "RwkvModel"),
+        ("sam", "SamModel"),
+        ("segformer", "SegformerModel"),
         ("starcoder2", "Starcoder2Model"),
         ("t5", "T5Model"),
+        ("timesformer", "TimesformerModel"),
         ("whisper", "WhisperModel"),
         ("xlm-roberta", "XLMRobertaModel"),
 	("xlnet", "XLNetModel"),
     ]
 )
 
 MODEL_FOR_PRETRAINING_MAPPING_NAMES = OrderedDict(
@@ -147,28 +158,33 @@
         ("biogpt", "BioGptForCausalLM"),
         ("blenderbot", "BlenderbotForCausalLM"),
         ("blenderbot-small", "BlenderbotSmallForCausalLM"),
         ("bloom", "BloomForCausalLM"),
         ("codegen", "CodeGenForCausalLM"),
         ("cpmant", "CpmAntForCausalLM"),
         ("cpmbee", "CpmBeeForCausalLM"),
+        ("falcon", "FalconForCausalLM"),
         ("gemma", "GemmaForCausalLM"),
         ("gpt2", "GPT2LMHeadModel"),
         ("gpt_pangu", "GPTPanguForCausalLM"),
-        ("falcon", "FalconForCausalLM"),
         ("gpt_bigcode", "GPTBigCodeForCausalLM"),
         ("jetmoe", "JetMoEForCausalLM"),
+        ("llama", "LlamaForCausalLM"),
         ("mamba", "MambaForCausalLM"),
         ('minicpm', 'MiniCPMForCausalLM'),
         ("mistral", "MistralForCausalLM"),
         ("mixtral", "MixtralForCausalLM"),
         ("musicgen", "MusicgenForCausalLM"),
         ("musicgen_melody", "MusicgenMelodyForCausalLM"),
+        ("olmo", "OlmoForCausalLM"),
+        ("openelm", "OpenELMForCausalLM"),
         ("opt", "OPTForCausalLM"),
+        ("pegasus", "PegasusForCausalLM"),
         ("phi", "PhiForCausalLM"),
+        ("phi3", "Phi3ForCausalLM"),
         ("qwen2", "Qwen2ForCausalLM"),
         ("qwen2_moe", "Qwen2MoeForCausalLM"),
         ("reformer", "ReformerModelWithLMHead"),
         ("roberta", "RobertaLMHeadModel"),
         ("rwkv", "RwkvForCausalLM"),
         ("starcoder2", "Starcoder2ForCausalLM"),
         ("whisper", "WhisperForCausalLM"),
@@ -374,14 +390,15 @@
         ("layoutlmv2", "LayoutLMv2ForSequenceClassification"),
         ("jetmoe", "JetMoEForSequenceClassification"),
         ('minicpm', 'MiniCPMForSequenceClassification'),
         ("mistral", "MistralForSequenceClassification"),
         ("mixtral", "MixtralForSequenceClassification"),
         ("opt", "OPTForSequenceClassification"),
         ("phi", "PhiForSequenceClassification"),
+        ("phi3", "Phi3ForSequenceClassification"),
         ("qwen2", "Qwen2ForSequenceClassification"),
         ("qwen2_moe", "Qwen2MoeForSequenceClassification"),
         ("reformer", "ReformerForSequenceClassification"),
         ("starcoder2", "Starcoder2ForSequenceClassification"),
         ("xlm-roberta", "XLMRobertaForSequenceClassification"),
 	("xlnet", "XLNetForSequenceClassification"),
     ]
@@ -520,14 +537,15 @@
         ("mobilebert", "MobileBertForTokenClassification"),
         ("mpnet", "MPNetForTokenClassification"),
         ("mpt", "MptForTokenClassification"),
         ("mra", "MraForTokenClassification"),
         ("nezha", "NezhaForTokenClassification"),
         ("nystromformer", "NystromformerForTokenClassification"),
         ("phi", "PhiForTokenClassification"),
+        ("phi3", "Phi3ForTokenClassification"),
         ("qdqbert", "QDQBertForTokenClassification"),
         ("rembert", "RemBertForTokenClassification"),
         ("roberta", "RobertaForTokenClassification"),
         ("roberta-prelayernorm", "RobertaPreLayerNormForTokenClassification"),
         ("roc_bert", "RoCBertForTokenClassification"),
         ("roformer", "RoFormerForTokenClassification"),
         ("squeezebert", "SqueezeBertForTokenClassification"),
```

## mindnlp/transformers/models/auto/tokenization_auto.py

```diff
@@ -213,14 +213,16 @@
         (
             "llama",
             (
                 "LlamaTokenizer" if is_sentencepiece_available() else None,
                 "LlamaTokenizerFast" if is_tokenizers_available() else None,
             ),
         ),
+        ("llava", ("LlamaTokenizer", "LlamaTokenizerFast" if is_tokenizers_available() else None)),
+        ("llava_next", ("LlamaTokenizer", "LlamaTokenizerFast" if is_tokenizers_available() else None)),
         ("longformer", ("LongformerTokenizer", "LongformerTokenizerFast" if is_tokenizers_available() else None)),
         (
             "longt5",
             (
                 "T5Tokenizer" if is_sentencepiece_available() else None,
                 "T5TokenizerFast" if is_tokenizers_available() else None,
             ),
@@ -300,14 +302,22 @@
         (
             "nystromformer",
             (
                 "AlbertTokenizer" if is_sentencepiece_available() else None,
                 "AlbertTokenizerFast" if is_tokenizers_available() else None,
             ),
         ),
+        ("olmo", (None, "GPTNeoXTokenizerFast" if is_tokenizers_available() else None)),
+        (
+            "openelm",
+            (
+                "LlamaTokenizer" if is_sentencepiece_available() else None,
+                "LlamaTokenizerFast" if is_tokenizers_available() else None,
+            ),
+        ),
         ("oneformer", ("CLIPTokenizer", "CLIPTokenizerFast" if is_tokenizers_available() else None)),
         ("opt", ("GPT2Tokenizer", "GPT2TokenizerFast" if is_tokenizers_available() else None)),
         ("owlv2", ("CLIPTokenizer", "CLIPTokenizerFast" if is_tokenizers_available() else None)),
         ("owlvit", ("CLIPTokenizer", "CLIPTokenizerFast" if is_tokenizers_available() else None)),
         ("gpt_pangu", ("GPTPanguTokenizer", None)),
         (
             "pegasus",
@@ -333,14 +343,15 @@
         (
             "persimmon",
             (
                 "LlamaTokenizer" if is_sentencepiece_available() else None,
                 "LlamaTokenizerFast" if is_tokenizers_available() else None,
             ),
         ),
+        ("phi3", ("LlamaTokenizer", "LlamaTokenizerFast" if is_tokenizers_available() else None)),
         ("phi", ("CodeGenTokenizer", "CodeGenTokenizerFast" if is_tokenizers_available() else None)),
         ("phobert", ("PhobertTokenizer", None)),
         # ("pix2struct", ("T5Tokenizer", "T5TokenizerFast" if is_tokenizers_available() else None)),
         ("plbart", ("PLBartTokenizer" if is_sentencepiece_available() else None, None)),
         ("prophetnet", ("ProphetNetTokenizer", None)),
         ("qdqbert", ("BertTokenizer", "BertTokenizerFast" if is_tokenizers_available() else None)),
         (
@@ -419,14 +430,15 @@
             "umt5",
             (
                 "T5Tokenizer" if is_sentencepiece_available() else None,
                 "T5TokenizerFast" if is_tokenizers_available() else None,
             ),
         ),
         ("vilt", ("BertTokenizer", "BertTokenizerFast" if is_tokenizers_available() else None)),
+        ("vipllava", ("LlamaTokenizer", "LlamaTokenizerFast" if is_tokenizers_available() else None)),
         ("visual_bert", ("BertTokenizer", "BertTokenizerFast" if is_tokenizers_available() else None)),
         ("vits", ("VitsTokenizer", None)),
         ("wav2vec2", ("Wav2Vec2CTCTokenizer", None)),
         ("wav2vec2-conformer", ("Wav2Vec2CTCTokenizer", None)),
         ("wav2vec2_phoneme", ("Wav2Vec2PhonemeCTCTokenizer", None)),
         ("whisper", ("WhisperTokenizer", "WhisperTokenizerFast" if is_tokenizers_available() else None)),
         ("xclip", ("CLIPTokenizer", "CLIPTokenizerFast" if is_tokenizers_available() else None)),
```

## mindnlp/transformers/models/beit/configuration_beit.py

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """ BEiT model configuration"""
 from mindnlp.utils import logging
-from mindnlp.utils.backbone_utils import BackboneConfigMixin, get_aligned_output_features_output_indices
+from ...backbone_utils import BackboneConfigMixin, get_aligned_output_features_output_indices
 from ...configuration_utils import PretrainedConfig
 
 
 logger = logging.get_logger(__name__)
 
 BEIT_PRETRAINED_CONFIG_ARCHIVE_MAP = {
     "microsoft/beit-base-patch16-224-pt22k": (
```

## mindnlp/transformers/models/beit/modeling_beit.py

```diff
@@ -23,15 +23,15 @@
 
 import numpy as np
 import mindspore
 from mindspore import nn, ops, Tensor, Parameter
 from mindspore.common.initializer import initializer, Normal
 
 from mindnlp.utils import logging
-from mindnlp.utils.backbone_utils import BackboneMixin
+from ...backbone_utils import BackboneMixin
 from ...activations import ACT2FN
 from ...modeling_outputs import (
     BackboneOutput,
     BaseModelOutput,
     BaseModelOutputWithPooling,
     ImageClassifierOutput,
     MaskedLMOutput,
```

## mindnlp/transformers/models/bit/configuration_bit.py

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ BiT model configuration"""
 
 from ...configuration_utils import PretrainedConfig
 from ....utils import logging
-from ....utils.backbone_utils import BackboneConfigMixin, get_aligned_output_features_output_indices
+from ...backbone_utils import BackboneConfigMixin, get_aligned_output_features_output_indices
 
 
 logger = logging.get_logger(__name__)
 
 
 class BitConfig(BackboneConfigMixin, PretrainedConfig):
     r"""
```

## mindnlp/transformers/models/bit/modeling_bit.py

```diff
@@ -28,15 +28,15 @@
     BackboneOutput,
     BaseModelOutputWithNoAttention,
     BaseModelOutputWithPoolingAndNoAttention,
     ImageClassifierOutputWithNoAttention,
 )
 from ...modeling_utils import PreTrainedModel
 from ....utils import logging
-from ....utils.backbone_utils import BackboneMixin
+from ...backbone_utils import BackboneMixin
 from .configuration_bit import BitConfig
 
 
 logger = logging.get_logger(__name__)
 
 # General docstring
 _CONFIG_FOR_DOC = "BitConfig"
```

## mindnlp/transformers/models/convbert/__init__.py

```diff
@@ -11,18 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 ConvBert Model.
 """
-from . import convbert, convbert_config, convbert_tokenizer, convbert_tokenizer_fast
+from . import (
+    convbert,
+    convbert_config,
+    convbert_tokenizer,
+    convbert_tokenizer_fast,
+    graph_convbert,
+)
 from .convbert import *
 from .convbert_config import *
 from .convbert_tokenizer import *
 from .convbert_tokenizer_fast import *
+from .graph_convbert import *
 
 __all__ = []
 __all__.extend(convbert.__all__)
 __all__.extend(convbert_config.__all__)
 __all__.extend(convbert_tokenizer.__all__)
 __all__.extend(convbert_tokenizer_fast.__all__)
+__all__.extend(graph_convbert.__all__)
```

## mindnlp/transformers/models/convbert/convbert.py

```diff
@@ -15,60 +15,67 @@
 """ ConvBERT model."""
 
 from typing import Optional, Tuple, Union
 import math
 import mindspore as ms
 from mindspore import nn
 from mindspore import ops
-from mindspore.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 from mindspore.common.initializer import initializer, Normal
 
 from ...activations import ACT2FN, get_activation
 from ...modeling_outputs import (
     BaseModelOutputWithCrossAttentions,
     MaskedLMOutput,
     MultipleChoiceModelOutput,
     QuestionAnsweringModelOutput,
     SequenceClassifierOutput,
     TokenClassifierOutput,
 )
 from ...modeling_utils import PreTrainedModel, SequenceSummary
 from .convbert_config import ConvBertConfig
-from ...ms_utils import apply_chunking_to_forward, find_pruneable_heads_and_indices, prune_linear_layer
+from ...ms_utils import (
+    apply_chunking_to_forward,
+    find_pruneable_heads_and_indices,
+    prune_linear_layer,
+)
 
 CONVBERT_PRETRAINED_MODEL_ARCHIVE_LIST = [
     "conv-bert-base",
     "conv-bert-medium-small",
     "conv-bert-small",
 ]
 
 
 class ConvBertEmbeddings(nn.Cell):
     """Construct the embeddings from word, position and token_type embeddings."""
 
     def __init__(self, config):
         super().__init__()
         self.word_embeddings = nn.Embedding(
-            config.vocab_size, config.embedding_size, padding_idx=config.pad_token_id)
+            config.vocab_size, config.embedding_size, padding_idx=config.pad_token_id
+        )
         self.position_embeddings = nn.Embedding(
-            config.max_position_embeddings, config.embedding_size)
+            config.max_position_embeddings, config.embedding_size
+        )
         self.token_type_embeddings = nn.Embedding(
-            config.type_vocab_size, config.embedding_size)
+            config.type_vocab_size, config.embedding_size
+        )
 
         # self.LayerNorm is not snake-cased to stick with TensorFlow model variable name and be able to load
         # any TensorFlow checkpoint file
         self.LayerNorm = nn.LayerNorm(
-            config.embedding_size, epsilon=config.layer_norm_eps)
+            config.embedding_size, epsilon=config.layer_norm_eps
+        )
         self.dropout = nn.Dropout(p=config.hidden_dropout_prob)
         # position_ids (1, len position emb) is contiguous in memory and exported when serialized
-        self.position_ids = ops.arange(
-            config.max_position_embeddings).broadcast_to((1, -1))
+        self.position_ids = ops.arange(config.max_position_embeddings).broadcast_to(
+            (1, -1)
+        )
 
-        self.token_type_ids = ops.zeros(
-            self.position_ids.shape, dtype=ms.int64)
+        self.token_type_ids = ops.zeros(self.position_ids.shape, dtype=ms.int64)
 
     def construct(
         self,
         input_ids: Optional[ms.Tensor] = None,
         token_type_ids: Optional[ms.Tensor] = None,
         position_ids: Optional[ms.Tensor] = None,
         inputs_embeds: Optional[ms.Tensor] = None,
@@ -86,15 +93,16 @@
         # Setting the token_type_ids to the registered buffer in constructor where it is all zeros, which usually occurs
         # when its auto-generated, registered buffer helps users when tracing the model without passing token_type_ids, solves
         # issue #5664
         if token_type_ids is None:
             if hasattr(self, "token_type_ids"):
                 buffered_token_type_ids = self.token_type_ids[:, :seq_length]
                 buffered_token_type_ids_expanded = buffered_token_type_ids.broadcast_to(
-                    input_shape[0], seq_length)
+                    input_shape[0], seq_length
+                )
                 token_type_ids = buffered_token_type_ids_expanded
             else:
                 token_type_ids = ops.zeros(input_shape, dtype=ms.int64)
 
         if inputs_embeds is None:
             inputs_embeds = self.word_embeddings(input_ids)
         position_embeddings = self.position_embeddings(position_ids)
@@ -115,74 +123,81 @@
     config_class = ConvBertConfig
     base_model_prefix = "convbert"
     supports_gradient_checkpointing = True
 
     def _init_weights(self, cell):
         """Initialize the weights"""
         if isinstance(cell, nn.Dense):
-            cell.weight = ms.Parameter(initializer(
-                Normal(sigma=self.config.initializer_range, mean=0.0),
-                cell.weight.shape,
-                cell.weight.dtype
-            ))
+            cell.weight = ms.Parameter(
+                initializer(
+                    Normal(sigma=self.config.initializer_range, mean=0.0),
+                    cell.weight.shape,
+                    cell.weight.dtype,
+                )
+            )
             if cell.bias is not None:
-                cell.bias = ms.Parameter(initializer(
-                    'zeros', cell.bias.shape, cell.bias.dtype))
+                cell.bias = ms.Parameter(
+                    initializer("zeros", cell.bias.shape, cell.bias.dtype)
+                )
         elif isinstance(cell, nn.Embedding):
-            cell.weight = ms.Parameter(initializer(Normal(mean=0.0, sigma=self.config.initializer_range),
-                                                   cell.weight.shape, cell.weight.dtype))
+            cell.weight = ms.Parameter(
+                initializer(
+                    Normal(mean=0.0, sigma=self.config.initializer_range),
+                    cell.weight.shape,
+                    cell.weight.dtype,
+                )
+            )
             # if cell.padding_idx is not None:
             #     cell.weight.data[cell.padding_idx].set_data(
             #         initializer('zeros',
             #                     cell.weight.data[cell.padding_idx].shape,
             #                     cell.weight.data[cell.padding_idx].dtype)
             #     )
         elif isinstance(cell, nn.LayerNorm):
             cell.bias = ms.Parameter(
-                initializer(
-                    'zeros', cell.bias.shape, cell.bias.dtype)
+                initializer("zeros", cell.bias.shape, cell.bias.dtype)
             )
             cell.weight = ms.Parameter(
-                initializer(
-                    'ones', cell.weight.shape, cell.weight.dtype)
+                initializer("ones", cell.weight.shape, cell.weight.dtype)
             )
 
 
 class SeparableConv1D(nn.Cell):
     """This class implements separable convolution, i.e. a depthwise and a pointwise layer"""
 
     def __init__(self, config, input_filters, output_filters, kernel_size):
         super().__init__()
         self.depthwise = nn.Conv1d(
             input_filters,
             input_filters,
             kernel_size=kernel_size,
             group=input_filters,
-            pad_mode='pad',
+            pad_mode="pad",
             padding=kernel_size // 2,
-            has_bias=False
+            has_bias=False,
         )
         self.pointwise = nn.Conv1d(
-            input_filters,
-            output_filters,
-            kernel_size=1,
-            has_bias=False
+            input_filters, output_filters, kernel_size=1, has_bias=False
         )
         self.bias = ms.Parameter(ops.zeros((output_filters, 1)))
 
-        self.depthwise.weight = ms.Parameter(initializer(
-            Normal(sigma=config.initializer_range, mean=0.0),
-            self.depthwise.weight.shape,
-            self.depthwise.weight.dtype
-        ))
-        self.pointwise.weight = ms.Parameter(initializer(
-            Normal(sigma=config.initializer_range, mean=0.0),
-            self.pointwise.weight.shape,
-            self.depthwise.weight.dtype
-        ))
+        self.depthwise.weight = ms.Parameter(
+            initializer(
+                Normal(sigma=config.initializer_range, mean=0.0),
+                self.depthwise.weight.shape,
+                self.depthwise.weight.dtype,
+            )
+        )
+        self.pointwise.weight = ms.Parameter(
+            initializer(
+                Normal(sigma=config.initializer_range, mean=0.0),
+                self.pointwise.weight.shape,
+                self.depthwise.weight.dtype,
+            )
+        )
 
     def construct(self, hidden_states: ms.Tensor) -> ms.Tensor:
         x = self.depthwise(hidden_states)
         x = self.pointwise(x)
         x += self.bias
         return x
 
@@ -190,15 +205,17 @@
 class ConvBertSelfAttention(nn.Cell):
     """
     ConvBertSelfAttention
     """
 
     def __init__(self, config):
         super().__init__()
-        if config.hidden_size % config.num_attention_heads != 0 and not hasattr(config, "embedding_size"):
+        if config.hidden_size % config.num_attention_heads != 0 and not hasattr(
+            config, "embedding_size"
+        ):
             raise ValueError(
                 f"The hidden size ({config.hidden_size}) is not a multiple of the number of attention "
                 f"heads ({config.num_attention_heads})"
             )
 
         new_num_attention_heads = config.num_attention_heads // config.head_ratio
         if new_num_attention_heads < 1:
@@ -206,43 +223,44 @@
             self.num_attention_heads = 1
         else:
             self.num_attention_heads = new_num_attention_heads
             self.head_ratio = config.head_ratio
 
         self.conv_kernel_size = config.conv_kernel_size
         if config.hidden_size % self.num_attention_heads != 0:
-            raise ValueError(
-                "hidden_size should be divisible by num_attention_heads")
+            raise ValueError("hidden_size should be divisible by num_attention_heads")
 
-        self.attention_head_size = (
-            config.hidden_size // self.num_attention_heads) // 2
+        self.attention_head_size = (config.hidden_size // self.num_attention_heads) // 2
         self.all_head_size = self.num_attention_heads * self.attention_head_size
 
         self.query = nn.Dense(config.hidden_size, self.all_head_size)
         self.key = nn.Dense(config.hidden_size, self.all_head_size)
         self.value = nn.Dense(config.hidden_size, self.all_head_size)
 
         self.key_conv_attn_layer = SeparableConv1D(
             config, config.hidden_size, self.all_head_size, self.conv_kernel_size
         )
         self.conv_kernel_layer = nn.Dense(
-            self.all_head_size, self.num_attention_heads * self.conv_kernel_size)
+            self.all_head_size, self.num_attention_heads * self.conv_kernel_size
+        )
         self.conv_out_layer = nn.Dense(config.hidden_size, self.all_head_size)
         self.unfold = nn.Unfold(
             ksizes=[1, self.conv_kernel_size, 1, 1],
             rates=[1, 1, 1, 1],
             strides=[1, 1, 1, 1],
-            padding="same"
+            padding="same",
         )
         self.dropout = nn.Dropout(p=config.attention_probs_dropout_prob)
 
     def swapaxes_for_scores(self, x):
         """swapaxes for scores"""
-        new_x_shape = x.shape[:-1] + \
-            (self.num_attention_heads, self.attention_head_size)
+        new_x_shape = x.shape[:-1] + (
+            self.num_attention_heads,
+            self.attention_head_size,
+        )
         x = x.view(*new_x_shape)
         return x.permute(0, 2, 1, 3)
 
     def construct(
         self,
         hidden_states: ms.Tensor,
         attention_mask: Optional[ms.Tensor] = None,
@@ -259,51 +277,53 @@
             mixed_key_layer = self.key(encoder_hidden_states)
             mixed_value_layer = self.value(encoder_hidden_states)
         else:
             mixed_key_layer = self.key(hidden_states)
             mixed_value_layer = self.value(hidden_states)
 
         mixed_key_conv_attn_layer = self.key_conv_attn_layer(
-            hidden_states.swapaxes(1, 2))
+            hidden_states.swapaxes(1, 2)
+        )
         mixed_key_conv_attn_layer = mixed_key_conv_attn_layer.swapaxes(1, 2)
 
         query_layer = self.swapaxes_for_scores(mixed_query_layer)
         key_layer = self.swapaxes_for_scores(mixed_key_layer)
         value_layer = self.swapaxes_for_scores(mixed_value_layer)
-        conv_attn_layer = ops.multiply(
-            mixed_key_conv_attn_layer, mixed_query_layer)
+        conv_attn_layer = ops.multiply(mixed_key_conv_attn_layer, mixed_query_layer)
 
         conv_kernel_layer = self.conv_kernel_layer(conv_attn_layer)
         conv_kernel_layer = ops.reshape(
-            conv_kernel_layer, [-1, self.conv_kernel_size, 1])
+            conv_kernel_layer, [-1, self.conv_kernel_size, 1]
+        )
         conv_kernel_layer = ops.softmax(conv_kernel_layer, axis=1)
 
         conv_out_layer = self.conv_out_layer(hidden_states)
         conv_out_layer = ops.reshape(
-            conv_out_layer, [batch_size, -1, self.all_head_size])
+            conv_out_layer, [batch_size, -1, self.all_head_size]
+        )
         conv_out_layer = conv_out_layer.swapaxes(1, 2).unsqueeze(-1)
         conv_out_layer = ops.unfold(
             conv_out_layer,
             kernel_size=[self.conv_kernel_size, 1],
             dilation=1,
             padding=[(self.conv_kernel_size - 1) // 2, 0],
             stride=1,
         )
         conv_out_layer = conv_out_layer.swapaxes(1, 2).reshape(
             batch_size, -1, self.all_head_size, self.conv_kernel_size
         )
         conv_out_layer = ops.reshape(
-            conv_out_layer, [-1, self.attention_head_size, self.conv_kernel_size])
+            conv_out_layer, [-1, self.attention_head_size, self.conv_kernel_size]
+        )
         conv_out_layer = ops.matmul(conv_out_layer, conv_kernel_layer)
         conv_out_layer = ops.reshape(conv_out_layer, [-1, self.all_head_size])
 
         # Take the dot product between "query" and "key" to get the raw attention scores.
         attention_scores = ops.matmul(query_layer, key_layer.swapaxes(-1, -2))
-        attention_scores = attention_scores / \
-            math.sqrt(self.attention_head_size)
+        attention_scores = attention_scores / math.sqrt(self.attention_head_size)
         if attention_mask is not None:
             # Apply the attention mask is (precomputed for all layers in ConvBertModel forward() function)
             attention_scores = attention_scores + attention_mask
 
         # Normalize the attention scores to probabilities.
         attention_probs = ops.softmax(attention_scores, axis=-1)
 
@@ -314,39 +334,41 @@
         # Mask heads if we want to
         if head_mask is not None:
             attention_probs = attention_probs * head_mask
 
         context_layer = ops.matmul(attention_probs, value_layer)
         context_layer = context_layer.permute(0, 2, 1, 3)
 
-        conv_out = ops.reshape(conv_out_layer, [
-                               batch_size, -1, self.num_attention_heads, self.attention_head_size])
+        conv_out = ops.reshape(
+            conv_out_layer,
+            [batch_size, -1, self.num_attention_heads, self.attention_head_size],
+        )
         context_layer = ops.cat([context_layer, conv_out], 2)
 
         # conv and context
         new_context_layer_shape = context_layer.shape[:-2] + (
             self.num_attention_heads * self.attention_head_size * 2,
         )
         context_layer = context_layer.view(*new_context_layer_shape)
 
-        outputs = (context_layer, attention_probs) if output_attentions else (
-            context_layer,)
+        outputs = (
+            (context_layer, attention_probs) if output_attentions else (context_layer,)
+        )
         return outputs
 
 
 class ConvBertSelfOutput(nn.Cell):
     """
     ConvBertSelfOutput
     """
 
     def __init__(self, config):
         super().__init__()
         self.dense = nn.Dense(config.hidden_size, config.hidden_size)
-        self.LayerNorm = nn.LayerNorm(
-            config.hidden_size, epsilon=config.layer_norm_eps)
+        self.LayerNorm = nn.LayerNorm(config.hidden_size, epsilon=config.layer_norm_eps)
         self.dropout = nn.Dropout(p=config.hidden_dropout_prob)
 
     def construct(self, hidden_states: ms.Tensor, input_tensor: ms.Tensor) -> ms.Tensor:
         hidden_states = self.dense(hidden_states)
         hidden_states = self.dropout(hidden_states)
         hidden_states = self.LayerNorm(hidden_states + input_tensor)
         return hidden_states
@@ -360,33 +382,35 @@
     def __init__(self, config):
         super().__init__()
         self.self = ConvBertSelfAttention(config)
         self.output = ConvBertSelfOutput(config)
         self.pruned_heads = set()
 
     def prune_heads(self, heads):
-        """ prune heads """
+        """prune heads"""
         if len(heads) == 0:
             return
         heads, index = find_pruneable_heads_and_indices(
-            heads, self.self.num_attention_heads, self.self.attention_head_size, self.pruned_heads
+            heads,
+            self.self.num_attention_heads,
+            self.self.attention_head_size,
+            self.pruned_heads,
         )
 
         # Prune linear layers
         self.self.query = prune_linear_layer(self.self.query, index)
         self.self.key = prune_linear_layer(self.self.key, index)
         self.self.value = prune_linear_layer(self.self.value, index)
-        self.output.dense = prune_linear_layer(
-            self.output.dense, index, axis=1)
+        self.output.dense = prune_linear_layer(self.output.dense, index, axis=1)
 
         # Update hyper params and store pruned heads
-        self.self.num_attention_heads = self.self.num_attention_heads - \
-            len(heads)
-        self.self.all_head_size = self.self.attention_head_size * \
-            self.self.num_attention_heads
+        self.self.num_attention_heads = self.self.num_attention_heads - len(heads)
+        self.self.all_head_size = (
+            self.self.attention_head_size * self.self.num_attention_heads
+        )
         self.pruned_heads = self.pruned_heads.union(heads)
 
     def construct(
         self,
         hidden_states: ms.Tensor,
         attention_mask: Optional[ms.Tensor] = None,
         head_mask: Optional[ms.Tensor] = None,
@@ -415,21 +439,21 @@
         super().__init__()
         self.input_size = input_size
         self.output_size = output_size
         self.num_groups = num_groups
         self.group_in_dim = self.input_size // self.num_groups
         self.group_out_dim = self.output_size // self.num_groups
         self.weight = nn.Parameter(
-            ops.zeros((self.num_groups, self.group_in_dim, self.group_out_dim)))
+            ops.zeros((self.num_groups, self.group_in_dim, self.group_out_dim))
+        )
         self.bias = nn.Parameter(ops.zeros(output_size))
 
     def construct(self, hidden_states: ms.Tensor) -> ms.Tensor:
         batch_size = list(hidden_states.shape)[0]
-        x = ops.reshape(
-            hidden_states, [-1, self.num_groups, self.group_in_dim])
+        x = ops.reshape(hidden_states, [-1, self.num_groups, self.group_in_dim])
         x = x.permute(1, 0, 2)
         x = ops.matmul(x, self.weight)
         x = x.permute(1, 0, 2)
         x = ops.reshape(x, [batch_size, -1, self.output_size])
         x = x + self.bias
         return x
 
@@ -441,15 +465,17 @@
 
     def __init__(self, config):
         super().__init__()
         if config.num_groups == 1:
             self.dense = nn.Dense(config.hidden_size, config.intermediate_size)
         else:
             self.dense = GroupedLinearLayer(
-                input_size=config.hidden_size, output_size=config.intermediate_size, num_groups=config.num_groups
+                input_size=config.hidden_size,
+                output_size=config.intermediate_size,
+                num_groups=config.num_groups,
             )
         if isinstance(config.hidden_act, str):
             self.intermediate_act_fn = ACT2FN[config.hidden_act]
         else:
             self.intermediate_act_fn = config.hidden_act
 
     def construct(self, hidden_states: ms.Tensor) -> ms.Tensor:
@@ -465,18 +491,19 @@
 
     def __init__(self, config):
         super().__init__()
         if config.num_groups == 1:
             self.dense = nn.Dense(config.intermediate_size, config.hidden_size)
         else:
             self.dense = GroupedLinearLayer(
-                input_size=config.intermediate_size, output_size=config.hidden_size, num_groups=config.num_groups
+                input_size=config.intermediate_size,
+                output_size=config.hidden_size,
+                num_groups=config.num_groups,
             )
-        self.LayerNorm = nn.LayerNorm(
-            config.hidden_size, epsilon=config.layer_norm_eps)
+        self.LayerNorm = nn.LayerNorm(config.hidden_size, epsilon=config.layer_norm_eps)
         self.dropout = nn.Dropout(p=config.hidden_dropout_prob)
 
     def construct(self, hidden_states: ms.Tensor, input_tensor: ms.Tensor) -> ms.Tensor:
         hidden_states = self.dense(hidden_states)
         hidden_states = self.dropout(hidden_states)
         hidden_states = self.LayerNorm(hidden_states + input_tensor)
         return hidden_states
@@ -493,15 +520,16 @@
         self.seq_len_dim = 1
         self.attention = ConvBertAttention(config)
         self.is_decoder = config.is_decoder
         self.add_cross_attention = config.add_cross_attention
         if self.add_cross_attention:
             if not self.is_decoder:
                 raise TypeError(
-                    f"{self} should be used as a decoder model if cross attention is added")
+                    f"{self} should be used as a decoder model if cross attention is added"
+                )
             self.crossattention = ConvBertAttention(config)
         self.intermediate = ConvBertIntermediate(config)
         self.output = ConvBertOutput(config)
 
     def construct(
         self,
         hidden_states: ms.Tensor,
@@ -535,15 +563,18 @@
                 output_attentions,
             )
             attention_output = cross_attention_outputs[0]
             # add cross attentions if we output attention weights
             outputs = outputs + cross_attention_outputs[1:]
 
         layer_output = apply_chunking_to_forward(
-            self.feed_forward_chunk, self.chunk_size_feed_forward, self.seq_len_dim, attention_output
+            self.feed_forward_chunk,
+            self.chunk_size_feed_forward,
+            self.seq_len_dim,
+            attention_output,
         )
         outputs = (layer_output,) + outputs
         return outputs
 
     def feed_forward_chunk(self, attention_output):
         """feed forward chunk"""
         intermediate_output = self.intermediate(attention_output)
@@ -555,16 +586,17 @@
     """
     ConvBertEncoder
     """
 
     def __init__(self, config):
         super().__init__()
         self.config = config
-        self.layer = nn.CellList([ConvBertLayer(config)
-                                 for _ in range(config.num_hidden_layers)])
+        self.layer = nn.CellList(
+            [ConvBertLayer(config) for _ in range(config.num_hidden_layers)]
+        )
         self.gradient_checkpointing = False
 
     def construct(
         self,
         hidden_states: ms.Tensor,
         attention_mask: Optional[ms.Tensor] = None,
         head_mask: Optional[ms.Tensor] = None,
@@ -572,15 +604,17 @@
         encoder_attention_mask: Optional[ms.Tensor] = None,
         output_attentions: Optional[bool] = False,
         output_hidden_states: Optional[bool] = False,
         return_dict: Optional[bool] = True,
     ) -> Union[Tuple, BaseModelOutputWithCrossAttentions]:
         all_hidden_states = () if output_hidden_states else None
         all_self_attentions = () if output_attentions else None
-        all_cross_attentions = () if output_attentions and self.config.add_cross_attention else None
+        all_cross_attentions = (
+            () if output_attentions and self.config.add_cross_attention else None
+        )
         for i, layer_cell in enumerate(self.layer):
             if output_hidden_states:
                 all_hidden_states = all_hidden_states + (hidden_states,)
 
             layer_head_mask = head_mask[i] if head_mask is not None else None
 
             if self.gradient_checkpointing and self.training:
@@ -602,24 +636,28 @@
                     encoder_attention_mask,
                     output_attentions,
                 )
             hidden_states = layer_outputs[0]
             if output_attentions:
                 all_self_attentions = all_self_attentions + (layer_outputs[1],)
                 if self.config.add_cross_attention:
-                    all_cross_attentions = all_cross_attentions + \
-                        (layer_outputs[2],)
+                    all_cross_attentions = all_cross_attentions + (layer_outputs[2],)
 
         if output_hidden_states:
             all_hidden_states = all_hidden_states + (hidden_states,)
 
         if not return_dict:
             return tuple(
                 v
-                for v in [hidden_states, all_hidden_states, all_self_attentions, all_cross_attentions]
+                for v in [
+                    hidden_states,
+                    all_hidden_states,
+                    all_self_attentions,
+                    all_cross_attentions,
+                ]
                 if v is not None
             )
         return BaseModelOutputWithCrossAttentions(
             last_hidden_state=hidden_states,
             hidden_states=all_hidden_states,
             attentions=all_self_attentions,
             cross_attentions=all_cross_attentions,
@@ -634,36 +672,36 @@
     def __init__(self, config):
         super().__init__()
         self.dense = nn.Dense(config.hidden_size, config.hidden_size)
         if isinstance(config.hidden_act, str):
             self.transform_act_fn = ACT2FN[config.hidden_act]
         else:
             self.transform_act_fn = config.hidden_act
-        self.LayerNorm = nn.LayerNorm(
-            config.hidden_size, epsilon=config.layer_norm_eps)
+        self.LayerNorm = nn.LayerNorm(config.hidden_size, epsilon=config.layer_norm_eps)
 
     def construct(self, hidden_states: ms.Tensor) -> ms.Tensor:
         hidden_states = self.dense(hidden_states)
         hidden_states = self.transform_act_fn(hidden_states)
         hidden_states = self.LayerNorm(hidden_states)
         return hidden_states
 
 
 class ConvBertModel(ConvBertPreTrainedModel):
     """
-    ConvBertEncoder
+    ConvBertModel
     """
 
     def __init__(self, config):
         super().__init__(config)
         self.embeddings = ConvBertEmbeddings(config)
 
         if config.embedding_size != config.hidden_size:
             self.embeddings_project = nn.Dense(
-                config.embedding_size, config.hidden_size)
+                config.embedding_size, config.hidden_size
+            )
 
         self.encoder = ConvBertEncoder(config)
         self.config = config
         # Initialize weights and apply final processing
         self.post_init()
 
     def get_input_embeddings(self):
@@ -688,53 +726,64 @@
         position_ids: Optional[ms.Tensor] = None,
         head_mask: Optional[ms.Tensor] = None,
         inputs_embeds: Optional[ms.Tensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple, BaseModelOutputWithCrossAttentions]:
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        output_attentions = (
+            output_attentions
+            if output_attentions is not None
+            else self.config.output_attentions
+        )
         output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+            output_hidden_states
+            if output_hidden_states is not None
+            else self.config.output_hidden_states
+        )
+        return_dict = (
+            return_dict if return_dict is not None else self.config.use_return_dict
         )
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         if input_ids is not None and inputs_embeds is not None:
             raise ValueError(
-                "You cannot specify both input_ids and inputs_embeds at the same time")
+                "You cannot specify both input_ids and inputs_embeds at the same time"
+            )
         if input_ids is not None:
-            self.warn_if_padding_and_no_attention_mask(
-                input_ids, attention_mask)
+            self.warn_if_padding_and_no_attention_mask(input_ids, attention_mask)
             input_shape = input_ids.shape
         elif inputs_embeds is not None:
             input_shape = inputs_embeds.shape[:-1]
         else:
-            raise ValueError(
-                "You have to specify either input_ids or inputs_embeds")
+            raise ValueError("You have to specify either input_ids or inputs_embeds")
 
         batch_size, seq_length = input_shape
 
         if attention_mask is None:
             attention_mask = ops.ones(input_shape)
         if token_type_ids is None:
             if hasattr(self.embeddings, "token_type_ids"):
                 buffered_token_type_ids = self.embeddings.token_type_ids[:, :seq_length]
                 buffered_token_type_ids_expanded = buffered_token_type_ids.expand(
-                    batch_size, seq_length)
+                    batch_size, seq_length
+                )
                 token_type_ids = buffered_token_type_ids_expanded
             else:
                 token_type_ids = ops.zeros(input_shape, dtype=ms.int64)
 
         extended_attention_mask = self.get_extended_attention_mask(
-            attention_mask, input_shape)
-        head_mask = self.get_head_mask(
-            head_mask, self.config.num_hidden_layers)
+            attention_mask, input_shape
+        )
+        head_mask = self.get_head_mask(head_mask, self.config.num_hidden_layers)
 
         hidden_states = self.embeddings(
-            input_ids=input_ids, position_ids=position_ids, token_type_ids=token_type_ids, inputs_embeds=inputs_embeds
+            input_ids=input_ids,
+            position_ids=position_ids,
+            token_type_ids=token_type_ids,
+            inputs_embeds=inputs_embeds,
         )
 
         if hasattr(self, "embeddings_project"):
             hidden_states = self.embeddings_project(hidden_states)
 
         hidden_states = self.encoder(
             hidden_states,
@@ -752,39 +801,40 @@
     """Prediction cell for the generator, made up of two dense layers."""
 
     def __init__(self, config):
         super().__init__()
 
         self.activation = get_activation("gelu")
         self.LayerNorm = nn.LayerNorm(
-            config.embedding_size, epsilon=config.layer_norm_eps)
+            config.embedding_size, epsilon=config.layer_norm_eps
+        )
         self.dense = nn.Dense(config.hidden_size, config.embedding_size)
 
     def construct(self, generator_hidden_states: ms.Tensor) -> ms.Tensor:
         hidden_states = self.dense(generator_hidden_states)
         hidden_states = self.activation(hidden_states)
         hidden_states = self.LayerNorm(hidden_states)
 
         return hidden_states
 
 
 class ConvBertForMaskedLM(ConvBertPreTrainedModel):
     """
-    ConvBertEncoder
+    ConvBertForMaskedLM
     """
+
     _tied_weights_keys = ["generator.lm_head.weight"]
 
     def __init__(self, config):
         super().__init__(config)
 
         self.convbert = ConvBertModel(config)
         self.generator_predictions = ConvBertGeneratorPredictions(config)
 
-        self.generator_lm_head = nn.Dense(
-            config.embedding_size, config.vocab_size)
+        self.generator_lm_head = nn.Dense(config.embedding_size, config.vocab_size)
         # Initialize weights and apply final processing
         self.post_init()
 
     def get_output_embeddings(self):
         return self.generator_lm_head
 
     def set_output_embeddings(self, new_embeddings):
@@ -805,40 +855,41 @@
     ) -> Union[Tuple, MaskedLMOutput]:
         r"""
         labels (`ms.Tensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the masked language modeling loss. Indices should be in `[-100, 0, ...,
             config.vocab_size]` (see `input_ids` docstring) Tokens with indices set to `-100` are ignored (masked), the
             loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`
         """
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+        return_dict = (
+            return_dict if return_dict is not None else self.config.use_return_dict
+        )
 
         generator_hidden_states = self.convbert(
             input_ids,
             attention_mask,
             token_type_ids,
             position_ids,
             head_mask,
             inputs_embeds,
             output_attentions,
             output_hidden_states,
             return_dict,
         )
         generator_sequence_output = generator_hidden_states[0]
 
-        prediction_scores = self.generator_predictions(
-            generator_sequence_output)
+        prediction_scores = self.generator_predictions(generator_sequence_output)
         prediction_scores = self.generator_lm_head(prediction_scores)
 
         loss = None
         # Masked language modeling softmax layer
         if labels is not None:
             labels = labels.to(ms.int32)
-            loss_fct = nn.CrossEntropyLoss()  # -100 index = padding token
-            loss = loss_fct(prediction_scores.view(-1,
-                            self.config.vocab_size), labels.view(-1))
+            loss = ops.cross_entropy(
+                prediction_scores.view(-1, self.config.vocab_size), labels.view(-1)
+            )
 
         if not return_dict:
             output = (prediction_scores,) + generator_hidden_states[1:]
             return ((loss,) + output) if loss is not None else output
 
         return MaskedLMOutput(
             loss=loss,
@@ -851,15 +902,17 @@
 class ConvBertClassificationHead(nn.Cell):
     """Head for sentence-level classification tasks."""
 
     def __init__(self, config):
         super().__init__()
         self.dense = nn.Dense(config.hidden_size, config.hidden_size)
         classifier_dropout = (
-            config.classifier_dropout if config.classifier_dropout is not None else config.hidden_dropout_prob
+            config.classifier_dropout
+            if config.classifier_dropout is not None
+            else config.hidden_dropout_prob
         )
         self.dropout = nn.Dropout(p=classifier_dropout)
         self.out_proj = nn.Dense(config.hidden_size, config.num_labels)
 
         self.config = config
 
     def construct(self, hidden_states: ms.Tensor, **kwargs) -> ms.Tensor:
@@ -870,15 +923,15 @@
         x = self.dropout(x)
         x = self.out_proj(x)
         return x
 
 
 class ConvBertForSequenceClassification(ConvBertPreTrainedModel):
     """
-    ConvBertEncoder
+    ConvBertForSequenceClassification
     """
 
     def __init__(self, config):
         super().__init__(config)
         self.num_labels = config.num_labels
         self.config = config
         self.convbert = ConvBertModel(config)
@@ -902,15 +955,17 @@
     ) -> Union[Tuple, SequenceClassifierOutput]:
         r"""
         labels (`ms.Tensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+        return_dict = (
+            return_dict if return_dict is not None else self.config.use_return_dict
+        )
 
         outputs = self.convbert(
             input_ids,
             attention_mask=attention_mask,
             token_type_ids=token_type_ids,
             position_ids=position_ids,
             head_mask=head_mask,
@@ -931,26 +986,22 @@
                     self.config.problem_type = "regression"
                 elif self.num_labels > 1 and labels.dtype in [ms.int64, ms.int32]:
                     self.config.problem_type = "single_label_classification"
                 else:
                     self.config.problem_type = "multi_label_classification"
 
             if self.config.problem_type == "regression":
-                loss_fct = MSELoss()
                 if self.num_labels == 1:
-                    loss = loss_fct(logits.squeeze(), labels.squeeze())
+                    loss = ops.mse_loss(logits.squeeze(), labels.squeeze())
                 else:
-                    loss = loss_fct(logits, labels)
+                    loss = ops.mse_loss(logits, labels)
             elif self.config.problem_type == "single_label_classification":
-                loss_fct = CrossEntropyLoss()
-                loss = loss_fct(
-                    logits.view(-1, self.num_labels), labels.view(-1))
+                loss = ops.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
             elif self.config.problem_type == "multi_label_classification":
-                loss_fct = BCEWithLogitsLoss()
-                loss = loss_fct(logits, labels)
+                loss = ops.binary_cross_entropy_with_logits(logits, labels)
 
         if not return_dict:
             output = (logits,) + outputs[1:]
             return ((loss,) + output) if loss is not None else output
 
         return SequenceClassifierOutput(
             loss=loss,
@@ -990,28 +1041,41 @@
     ) -> Union[Tuple, MultipleChoiceModelOutput]:
         r"""
         labels (`ms.Tensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the multiple choice classification loss. Indices should be in `[0, ...,
             num_choices-1]` where `num_choices` is the size of the second dimension of the input tensors. (See
             `input_ids` above)
         """
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-        num_choices = input_ids.shape[1] if input_ids is not None else inputs_embeds.shape[1]
+        return_dict = (
+            return_dict if return_dict is not None else self.config.use_return_dict
+        )
+        num_choices = (
+            input_ids.shape[1] if input_ids is not None else inputs_embeds.shape[1]
+        )
 
-        input_ids = input_ids.view(-1,
-                                   input_ids.shape[-1]) if input_ids is not None else None
-        attention_mask = attention_mask.view(
-            -1, attention_mask.shape[-1]) if attention_mask is not None else None
-        token_type_ids = token_type_ids.view(
-            -1, token_type_ids.shape[-1]) if token_type_ids is not None else None
-        position_ids = position_ids.view(
-            -1, position_ids.shape[-1]) if position_ids is not None else None
+        input_ids = (
+            input_ids.view(-1, input_ids.shape[-1]) if input_ids is not None else None
+        )
+        attention_mask = (
+            attention_mask.view(-1, attention_mask.shape[-1])
+            if attention_mask is not None
+            else None
+        )
+        token_type_ids = (
+            token_type_ids.view(-1, token_type_ids.shape[-1])
+            if token_type_ids is not None
+            else None
+        )
+        position_ids = (
+            position_ids.view(-1, position_ids.shape[-1])
+            if position_ids is not None
+            else None
+        )
         inputs_embeds = (
-            inputs_embeds.view(-1,
-                               inputs_embeds.shape[-2], inputs_embeds.shape[-1])
+            inputs_embeds.view(-1, inputs_embeds.shape[-2], inputs_embeds.shape[-1])
             if inputs_embeds is not None
             else None
         )
 
         outputs = self.convbert(
             input_ids,
             attention_mask=attention_mask,
@@ -1029,16 +1093,15 @@
         pooled_output = self.sequence_summary(sequence_output)
         logits = self.classifier(pooled_output)
         reshaped_logits = logits.view(-1, num_choices)
 
         loss = None
         if labels is not None:
             labels = labels.to(ms.int32)
-            loss_fct = CrossEntropyLoss()
-            loss = loss_fct(reshaped_logits, labels)
+            loss = ops.cross_entropy(reshaped_logits, labels)
 
         if not return_dict:
             output = (reshaped_logits,) + outputs[1:]
             return ((loss,) + output) if loss is not None else output
 
         return MultipleChoiceModelOutput(
             loss=loss,
@@ -1055,15 +1118,17 @@
 
     def __init__(self, config):
         super().__init__(config)
         self.num_labels = config.num_labels
 
         self.convbert = ConvBertModel(config)
         classifier_dropout = (
-            config.classifier_dropout if config.classifier_dropout is not None else config.hidden_dropout_prob
+            config.classifier_dropout
+            if config.classifier_dropout is not None
+            else config.hidden_dropout_prob
         )
         self.dropout = nn.Dropout(p=classifier_dropout)
         self.classifier = nn.Dense(config.hidden_size, config.num_labels)
 
         # Initialize weights and apply final processing
         self.post_init()
 
@@ -1080,15 +1145,17 @@
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple, TokenClassifierOutput]:
         r"""
         labels (`ms.Tensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the token classification loss. Indices should be in `[0, ..., config.num_labels - 1]`.
         """
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+        return_dict = (
+            return_dict if return_dict is not None else self.config.use_return_dict
+        )
 
         outputs = self.convbert(
             input_ids,
             attention_mask=attention_mask,
             token_type_ids=token_type_ids,
             position_ids=position_ids,
             head_mask=head_mask,
@@ -1102,16 +1169,15 @@
 
         sequence_output = self.dropout(sequence_output)
         logits = self.classifier(sequence_output)
 
         loss = None
         if labels is not None:
             labels = labels.to(ms.int32)
-            loss_fct = CrossEntropyLoss()
-            loss = loss_fct(logits.view(-1, self.num_labels), labels.view(-1))
+            loss = ops.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
 
         if not return_dict:
             output = (logits,) + outputs[1:]
             return ((loss,) + output) if loss is not None else output
 
         return TokenClassifierOutput(
             loss=loss,
@@ -1146,51 +1212,49 @@
         inputs_embeds: Optional[ms.Tensor] = None,
         start_positions: Optional[ms.Tensor] = None,
         end_positions: Optional[ms.Tensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple, QuestionAnsweringModelOutput]:
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+        return_dict = (
+            return_dict if return_dict is not None else self.config.use_return_dict
+        )
 
         outputs = self.convbert(
             input_ids,
             attention_mask=attention_mask,
             token_type_ids=token_type_ids,
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-
         sequence_output = outputs[0]
-
         logits = self.qa_outputs(sequence_output)
         start_logits, end_logits = logits.split(1, axis=-1)
         start_logits = start_logits.squeeze(-1)
         end_logits = end_logits.squeeze(-1)
 
         total_loss = None
         if start_positions is not None and end_positions is not None:
             # If we are on multi-GPU, split add a dimension
             if len(start_positions.shape) > 1:
                 start_positions = start_positions.squeeze(-1)
             if len(end_positions.shape) > 1:
                 end_positions = end_positions.squeeze(-1)
             # sometimes the start/end positions are outside our model inputs, we ignore these terms
             ignored_index = start_logits.shape[1]
-            start_positions = start_positions.clamp(
-                0, ignored_index).to(ms.int32)
+            start_positions = start_positions.clamp(0, ignored_index).to(ms.int32)
             end_positions = end_positions.clamp(0, ignored_index).to(ms.int32)
 
-            loss_fct = CrossEntropyLoss(ignore_index=ignored_index)
-            start_loss = loss_fct(start_logits, start_positions)
-            end_loss = loss_fct(end_logits, end_positions)
+            start_loss = ops.cross_entropy(start_logits, start_positions, ignore_index=ignored_index)
+            end_loss = ops.cross_entropy(end_logits, end_positions, ignore_index=ignored_index)
             total_loss = (start_loss + end_loss) / 2
 
         if not return_dict:
             output = (start_logits, end_logits) + outputs[1:]
             return ((total_loss,) + output) if total_loss is not None else output
 
         return QuestionAnsweringModelOutput(
```

## mindnlp/transformers/models/gpt_neox/modeling_gpt_neox.py

```diff
@@ -15,15 +15,15 @@
 """ MindNLP  GPTNeoX model."""
 
 from typing import Optional, Tuple, Union
 
 from functools import partial
 import numpy as np
 import mindspore
-from mindspore import nn, Tensor, ops
+from mindspore import nn, ops
 from mindspore.common.initializer import initializer, Normal
 from mindnlp.utils import logging, get_default_dtype
 
 from ...modeling_outputs import (
     BaseModelOutputWithPast,
     CausalLMOutputWithPast,
     QuestionAnsweringModelOutput,
@@ -69,14 +69,15 @@
     models.
     """
 
     config_class = GPTNeoXConfig
     base_model_prefix = "gpt_neox"
     supports_gradient_checkpointing = True
     _no_split_modules = ["GPTNeoXLayer"]
+    _keys_to_ignore_on_load_unexpected = [r'masked_bias', r'attention.bias', r'inv_freq']
     _skip_keys_device_placement = "past_key_values"
     _supports_flash_attn_2 = False
 
     def _init_weights(self, cell):
         """Initialize the weights"""
         if isinstance(cell, nn.Dense):
             cell.weight.set_data(initializer(Normal(sigma=self.config.initializer_range, mean=0.0),
@@ -139,16 +140,16 @@
         self.norm_factor = self.head_size ** -0.5
         self.query_key_value = nn.Dense(config.hidden_size, 3 * config.hidden_size, has_bias=config.attention_bias)
         self.dense = nn.Dense(config.hidden_size, config.hidden_size, has_bias=config.attention_bias)
         self.attention_dropout = nn.Dropout(p=config.attention_dropout)
         self.is_causal = True
 
     def _init_bias(self, max_positions):
-        self.bias = Tensor.tril(ops.ones((max_positions, max_positions), dtype=mindspore.dtype.bool_)).view(
-                1, 1, max_positions, max_positions)
+        self.bias = ops.tril(ops.ones((max_positions, max_positions))).view(
+                1, 1, max_positions, max_positions).astype(mindspore.bool_)
 
     def _init_rope(self):
         if self.config.rope_scaling is None:
             self.rotary_emb = GPTNeoXRotaryEmbedding(
                 self.rotary_ndims, self.config.max_position_embeddings, base=self.config.rotary_emb_base
             )
         else:
@@ -206,16 +207,16 @@
 
         # Compute token offset for rotary embeddings (when decoding)
         seq_len = key.shape[-2]
         if has_layer_past:
             seq_len += layer_past[0].shape[-2]
         cos, sin = self.rotary_emb(value, seq_len=seq_len)
         query, key = apply_rotary_pos_emb(query_rot, key_rot, cos, sin, position_ids)
-        query = ops.cat((query, query_pass), axis=-1)
-        key = ops.cat((key, key_pass), axis=-1)
+        query = ops.cat((query, query_pass.type_as(query)), axis=-1)
+        key = ops.cat((key, key_pass.type_as(key)), axis=-1)
 
         # Cache QKV values
         if has_layer_past:
             past_key = layer_past[0]
             past_value = layer_past[1]
             key = ops.cat((past_key, key), axis=-2)
             value = ops.cat((past_value, value), axis=-2)
@@ -272,21 +273,18 @@
         key = key.view(batch_size * num_attention_heads, key_length, attn_head_size)
         attn_scores = ops.zeros((
             batch_size * num_attention_heads,
             query_length,
             key_length),
             dtype=query.dtype
         )
-        attn_scores = Tensor.baddbmm(
-            attn_scores,
+        attn_scores = ops.bmm(
             query,
             key.swapaxes(1, 2),
-            beta=1.0,
-            alpha=self.norm_factor,
-        )
+        ) * self.norm_factor
         attn_scores = attn_scores.view(batch_size, num_attention_heads, query_length, key_length)
 
         mask_value = np.finfo(mindspore.dtype_to_nptype(attn_scores.dtype)).min
         # Need to be a tensor, otherwise we get error: `RuntimeError: expected scalar type float but found double`.
         # Need to be on the same device, otherwise `RuntimeError: ..., x and y to be on the same device`
         mask_value = mindspore.tensor(mask_value, dtype=attn_scores.dtype)
         attn_scores = ops.where(causal_mask, attn_scores, mask_value)
@@ -319,61 +317,60 @@
     """GPTNeoXRotaryEmbedding"""
     def __init__(self, dim, max_position_embeddings=2048, base=10000):
         super().__init__()
 
         self.dim = dim
         self.max_position_embeddings = max_position_embeddings
         self.base = base
-        inv_freq = 1.0 / (self.base ** (ops.arange(0, self.dim, 2, dtype=mindspore.int64).float() / self.dim))
+        inv_freq = 1.0 / (self.base ** (ops.arange(0, self.dim, 2).float() / self.dim))
         self.inv_freq = inv_freq
 
-        # Build here to make `torch.jit.trace` work.
         self._set_cos_sin_cache(
             seq_len=max_position_embeddings, dtype=get_default_dtype()
         )
 
     def _set_cos_sin_cache(self, seq_len, dtype):
         self.max_seq_len_cached = seq_len
         t = ops.arange(self.max_seq_len_cached, dtype=self.inv_freq.dtype).type_as(self.inv_freq)
 
         freqs = ops.outer(t, self.inv_freq)
         # Different from paper, but it uses a different permutation in order to obtain the same calculation
         emb = ops.cat((freqs, freqs), axis=-1)
-        self.cos_cached = emb.cos().to(dtype)
-        self.sin_cached = emb.sin().to(dtype)
+        self.cos_cached = emb.cos()
+        self.sin_cached = emb.sin()
 
     def construct(self, x, seq_len=None):
         # x: [bs, num_attention_heads, seq_len, head_size]
         if seq_len > self.max_seq_len_cached:
             self._set_cos_sin_cache(seq_len=seq_len, dtype=x.dtype)
 
         return (
-            self.cos_cached[:seq_len].to(dtype=x.dtype),
-            self.sin_cached[:seq_len].to(dtype=x.dtype),
+            self.cos_cached[:seq_len],
+            self.sin_cached[:seq_len],
         )
 
 
 # copied from transformers.models.llama.modeling_llama.LlamaLinearScalingRotaryEmbedding.__init__
 class GPTNeoXLinearScalingRotaryEmbedding(GPTNeoXRotaryEmbedding):
     """GPTNeoXRotaryEmbedding extended with linear scaling. Credits to the Reddit user /u/kaiokendev"""
 
     def __init__(self, dim, max_position_embeddings=2048, base=10000, scaling_factor=1.0):
         self.scaling_factor = scaling_factor
         super().__init__(dim, max_position_embeddings, base)
 
     def _set_cos_sin_cache(self, seq_len, dtype):
         self.max_seq_len_cached = seq_len
-        t = ops.arange(self.max_seq_len_cached, dtype=mindspore.int64).type_as(self.inv_freq)
+        t = ops.arange(self.max_seq_len_cached, dtype=mindspore.float32).type_as(self.inv_freq)
         t = t / self.scaling_factor
 
         freqs = ops.outer(t, self.inv_freq)
         # Different from paper, but it uses a different permutation in order to obtain the same calculation
         emb = ops.cat((freqs, freqs), axis=-1)
-        self.cos_cached = emb.cos().to(dtype)
-        self.sin_cached = emb.sin().to(dtype)
+        self.cos_cached = emb.cos()
+        self.sin_cached = emb.sin()
 
 
 class GPTNeoXDynamicNTKScalingRotaryEmbedding(GPTNeoXRotaryEmbedding):
     """GPTNeoXRotaryEmbedding extended with Dynamic NTK scaling. Credits to the Reddit users /u/bloc97 and /u/emozilla"""
 
     def __init__(self, dim, max_position_embeddings=2048, base=10000, scaling_factor=1.0):
         self.scaling_factor = scaling_factor
@@ -390,16 +387,16 @@
             self.inv_freq = inv_freq
 
         t = ops.arange(self.max_seq_len_cached, dtype=mindspore.int64).type_as(self.inv_freq)
 
         freqs = ops.outer(t, self.inv_freq)
         # Different from paper, but it uses a different permutation in order to obtain the same calculation
         emb = ops.cat((freqs, freqs), axis=-1)
-        self.cos_cached = emb.cos().to(dtype)
-        self.sin_cached = emb.sin().to(dtype)
+        self.cos_cached = emb.cos()
+        self.sin_cached = emb.sin()
 
 
 def rotate_half(x):
     """Rotates half the hidden dims of the input."""
     # x1 = x[..., : x.shape[-1] // 2]
     # x2 = x[..., x.shape[-1] // 2:]
     x1, x2 = x.tensor_split(2, -1)
```

## mindnlp/transformers/models/gpt_neox/tokenization_gpt_neox_fast.py

```diff
@@ -1,58 +1,48 @@
 # coding=utf-8
-# Copyright 2024 Huawei Technologies Co., Ltd
+# Copyright 2022 EleutherAI and The HuggingFace Inc. team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tokenization classes for GPTNeoX."""
 import json
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
-from tokenizers import pre_tokenizers
+from tokenizers import pre_tokenizers, processors
 
-from mindnlp.utils import logging
 from ...tokenization_utils_fast import PreTrainedTokenizerFast
+from ....utils import logging
 
 
 logger = logging.get_logger(__name__)
 
 VOCAB_FILES_NAMES = {"vocab_file": "vocab.json", "merges_file": "merges.txt", "tokenizer_file": "tokenizer.json"}
 
-PRETRAINED_VOCAB_FILES_MAP = {
-    "tokenizer_file": {
-        "EleutherAI/gpt-neox-20b": "https://hf-mirror.com/EleutherAI/gpt-neox-20b/resolve/main/tokenizer.json",
-    },
-}
-
-PRETRAINED_POSITIONAL_EMBEDDINGS_SIZES = {
-    "gpt-neox-20b": 2048,
-}
-
 
 class GPTNeoXTokenizerFast(PreTrainedTokenizerFast):
     """
     Construct a "fast" GPT-NeoX-20B tokenizer (backed by HuggingFace's *tokenizers* library). Based on byte-level
     Byte-Pair-Encoding.
 
     This tokenizer has been trained to treat spaces like parts of the tokens (a bit like sentencepiece) so a word will
     be encoded differently whether it is at the beginning of the sentence (without space) or not:
 
     ```python
     >>> from transformers import GPTNeoXTokenizerFast
 
-    >>> tokenizer = GPTNeoXTokenizerFast.from_pretrained("gpt2")
+    >>> tokenizer = GPTNeoXTokenizerFast.from_pretrained("openai-community/gpt2")
     >>> tokenizer("Hello world")["input_ids"]
     [15496, 995]
 
     >>> tokenizer(" Hello world")["input_ids"]
     [18435, 995]
     ```
 
@@ -79,68 +69,178 @@
         unk_token (`str`, *optional*, defaults to `<|endoftext|>`):
             The unknown token. A token that is not in the vocabulary cannot be converted to an ID and is set to be this
             token instead.
         bos_token (`str`, *optional*, defaults to `<|endoftext|>`):
             The beginning of sequence token.
         eos_token (`str`, *optional*, defaults to `<|endoftext|>`):
             The end of sequence token.
+        pad_token (`str`, *optional*):
+            Token for padding a sequence.
         add_prefix_space (`bool`, *optional*, defaults to `False`):
             Whether or not to add an initial space to the input. This allows to treat the leading word just as any
             other word. (GPTNeoX tokenizer detect beginning of words by the preceding space).
+        add_bos_token (`bool`, *optional*, defaults to `False`):
+            Whether or not to add a `bos_token` at the start of sequences.
+        add_eos_token (`bool`, *optional*, defaults to `False`):
+            Whether or not to add an `eos_token` at the end of sequences.
         trim_offsets (`bool`, *optional*, defaults to `True`):
             Whether or not the post-processing step should trim offsets to avoid including whitespaces.
     """
 
     vocab_files_names = VOCAB_FILES_NAMES
-    pretrained_vocab_files_map = PRETRAINED_VOCAB_FILES_MAP
-    max_model_input_sizes = PRETRAINED_POSITIONAL_EMBEDDINGS_SIZES
     model_input_names = ["input_ids", "attention_mask"]
 
     def __init__(
         self,
         vocab_file=None,
         merges_file=None,
         tokenizer_file=None,
         unk_token="<|endoftext|>",
         bos_token="<|endoftext|>",
         eos_token="<|endoftext|>",
+        pad_token=None,
+        add_bos_token=False,
+        add_eos_token=False,
         add_prefix_space=False,
         **kwargs,
     ):
         super().__init__(
             vocab_file,
             merges_file,
             tokenizer_file=tokenizer_file,
             unk_token=unk_token,
             bos_token=bos_token,
             eos_token=eos_token,
+            pad_token=pad_token,
+            add_bos_token=add_bos_token,
+            add_eos_token=add_eos_token,
             add_prefix_space=add_prefix_space,
             **kwargs,
         )
 
+        self._add_bos_token = add_bos_token
+        self._add_eos_token = add_eos_token
+        self.update_post_processor()
+
         pre_tok_state = json.loads(self.backend_tokenizer.pre_tokenizer.__getstate__())
         if pre_tok_state.get("add_prefix_space", add_prefix_space) != add_prefix_space:
             pre_tok_class = getattr(pre_tokenizers, pre_tok_state.pop("type"))
             pre_tok_state["add_prefix_space"] = add_prefix_space
             self.backend_tokenizer.pre_tokenizer = pre_tok_class(**pre_tok_state)
 
         self.add_prefix_space = add_prefix_space
 
+    @property
+    def add_eos_token(self):
+        return self._add_eos_token
+
+    @property
+    def add_bos_token(self):
+        return self._add_bos_token
+
+    @add_eos_token.setter
+    def add_eos_token(self, value):
+        self._add_eos_token = value
+        self.update_post_processor()
+
+    @add_bos_token.setter
+    def add_bos_token(self, value):
+        self._add_bos_token = value
+        self.update_post_processor()
+
+    # Copied from transformers.models.llama.tokenization_llama_fast.LlamaTokenizerFast.update_post_processor
+    def update_post_processor(self):
+        """
+        Updates the underlying post processor with the current `bos_token` and `eos_token`.
+        """
+        bos = self.bos_token
+        bos_token_id = self.bos_token_id
+        if bos is None and self.add_bos_token:
+            raise ValueError("add_bos_token = True but bos_token = None")
+
+        eos = self.eos_token
+        eos_token_id = self.eos_token_id
+        if eos is None and self.add_eos_token:
+            raise ValueError("add_eos_token = True but eos_token = None")
+
+        single = f"{(bos+':0 ') if self.add_bos_token else ''}$A:0{(' '+eos+':0') if self.add_eos_token else ''}"
+        pair = f"{single}{(' '+bos+':1') if self.add_bos_token else ''} $B:1{(' '+eos+':1') if self.add_eos_token else ''}"
+
+        special_tokens = []
+        if self.add_bos_token:
+            special_tokens.append((bos, bos_token_id))
+        if self.add_eos_token:
+            special_tokens.append((eos, eos_token_id))
+        self._tokenizer.post_processor = processors.TemplateProcessing(
+            single=single, pair=pair, special_tokens=special_tokens
+        )
+
+    # Copied from transformers.models.llama.tokenization_llama.LlamaTokenizer.get_special_tokens_mask
+    def get_special_tokens_mask(
+        self, token_ids_0: List[int], token_ids_1: Optional[List[int]] = None, already_has_special_tokens: bool = False
+    ) -> List[int]:
+        """
+        Retrieve sequence ids from a token list that has no special tokens added. This method is called when adding
+        special tokens using the tokenizer `prepare_for_model` method.
+
+        Args:
+            token_ids_0 (`List[int]`):
+                List of IDs.
+            token_ids_1 (`List[int]`, *optional*):
+                Optional second list of IDs for sequence pairs.
+            already_has_special_tokens (`bool`, *optional*, defaults to `False`):
+                Whether or not the token list is already formatted with special tokens for the model.
+
+        Returns:
+            `List[int]`: A list of integers in the range [0, 1]: 1 for a special token, 0 for a sequence token.
+        """
+        if already_has_special_tokens:
+            return super().get_special_tokens_mask(
+                token_ids_0=token_ids_0, token_ids_1=token_ids_1, already_has_special_tokens=True
+            )
+
+        bos_token_id = [1] if self.add_bos_token else []
+        eos_token_id = [1] if self.add_eos_token else []
+
+        if token_ids_1 is None:
+            return bos_token_id + ([0] * len(token_ids_0)) + eos_token_id
+        return (
+            bos_token_id
+            + ([0] * len(token_ids_0))
+            + eos_token_id
+            + bos_token_id
+            + ([0] * len(token_ids_1))
+            + eos_token_id
+        )
+
+    # Copied from transformers.models.llama.tokenization_llama_fast.LlamaTokenizerFast.build_inputs_with_special_tokens
+    def build_inputs_with_special_tokens(self, token_ids_0, token_ids_1=None):
+        bos_token_id = [self.bos_token_id] if self.add_bos_token else []
+        eos_token_id = [self.eos_token_id] if self.add_eos_token else []
+
+        output = bos_token_id + token_ids_0 + eos_token_id
+
+        if token_ids_1 is not None:
+            output = output + bos_token_id + token_ids_1 + eos_token_id
+
+        return output
+
     def save_vocabulary(self, save_directory: str, filename_prefix: Optional[str] = None) -> Tuple[str]:
         files = self._tokenizer.model.save(save_directory, name=filename_prefix)
         return tuple(files)
 
     @property
     # Copied from transformers.models.gpt2.tokenization_gpt2.GPT2Tokenizer.default_chat_template
     def default_chat_template(self):
         """
         A simple chat template that ignores role information and just concatenates messages with EOS tokens.
         """
         logger.warning_once(
-            "\nNo chat template is defined for this tokenizer - using the default template "
-            f"for the {self.__class__.__name__} class. If the default is not appropriate for "
-            "your model, please set `tokenizer.chat_template` to an appropriate template. "
-            "See https://hf-mirror.com/docs/transformers/main/chat_templating for more information.\n"
+            "No chat template is set for this tokenizer, falling back to a default class-level template. "
+            "This is very error-prone, because models are often trained with templates different from the class "
+            "default! Default chat templates are a legacy feature and will be removed in Transformers v4.43, at which "
+            "point any code depending on them will stop working. We recommend setting a valid chat template before "
+            "then to ensure that this model continues working without issues."
         )
         return "{% for message in messages %}" "{{ message.content }}{{ eos_token }}" "{% endfor %}"
 
 __all__ = ['GPTNeoXTokenizerFast']
```

## mindnlp/transformers/models/mbart/modeling_mbart.py

```diff
@@ -441,19 +441,19 @@
         if isinstance(cell, nn.Dense):
             cell.weight.set_data(initializer(Normal(self.config.init_std),
                                                cell.weight.shape, cell.weight.dtype))
             if cell.bias is not None:
                 cell.bias.set_data(initializer('zeros',
                                                cell.bias.shape, cell.bias.dtype))
         elif isinstance(cell, nn.Embedding):
-            cell.weight.set_data(initializer(Normal(
-                sigma=std, mean=0.0), cell.weight.shape, cell.weight.dtype))
-            if cell.padding_idx is not None:
-                cell.weight.data[cell.padding_idx] = ops.zeros_like(
-                    cell.weight.data[cell.padding_idx])
+            weight = np.random.normal(0.0, std, cell.weight.shape)
+            if cell.padding_idx:
+                weight[cell.padding_idx] = 0
+
+            cell.weight.set_data(Tensor(weight, cell.weight.dtype))
 
     @property
     def dummy_inputs(self):
         """dummy_inputs"""
         pad_token = self.config.pad_token_id
         input_ids = Tensor([[0, 6, 10, 4, 2], [0, 8, 12, 2, pad_token]])
         dummy_inputs = {
```

## mindnlp/transformers/models/pegasus/__init__.py

```diff
@@ -11,14 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 Pegasus Models init
 """
-from . import tokenization_pegasus, tokenization_pegasus_fast
+from . import tokenization_pegasus, tokenization_pegasus_fast, configuration_pegasus, modeling_pegasus
 from .tokenization_pegasus import *
 from .tokenization_pegasus_fast import *
+from .configuration_pegasus import *
+from .modeling_pegasus import *
 
 __all__ = []
 __all__.extend(tokenization_pegasus.__all__)
 __all__.extend(tokenization_pegasus_fast.__all__)
+__all__.extend(configuration_pegasus.__all__)
+__all__.extend(modeling_pegasus.__all__)
```

## mindnlp/transformers/models/pegasus/tokenization_pegasus.py

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 # Copyright 2020 Google and The HuggingFace Inc. team.
+# Copyright 2024 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## mindnlp/transformers/models/pegasus/tokenization_pegasus_fast.py

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 # Copyright 2020 Google and The HuggingFace Inc. team.
+# Copyright 2024 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## mindnlp/transformers/models/timesformer/__init__.py

```diff
@@ -0,0 +1,67 @@
+00000000: 2320 436f 7079 7269 6768 7420 3230 3234  # Copyright 2024
+00000010: 2048 7561 7765 6920 5465 6368 6e6f 6c6f   Huawei Technolo
+00000020: 6769 6573 2043 6f2e 2c20 4c74 640a 230a  gies Co., Ltd.#.
+00000030: 2320 4c69 6365 6e73 6564 2075 6e64 6572  # Licensed under
+00000040: 2074 6865 2041 7061 6368 6520 4c69 6365   the Apache Lice
+00000050: 6e73 652c 2056 6572 7369 6f6e 2032 2e30  nse, Version 2.0
+00000060: 2028 7468 6520 224c 6963 656e 7365 2229   (the "License")
+00000070: 3b0a 2320 796f 7520 6d61 7920 6e6f 7420  ;.# you may not 
+00000080: 7573 6520 7468 6973 2066 696c 6520 6578  use this file ex
+00000090: 6365 7074 2069 6e20 636f 6d70 6c69 616e  cept in complian
+000000a0: 6365 2077 6974 6820 7468 6520 4c69 6365  ce with the Lice
+000000b0: 6e73 652e 0a23 2059 6f75 206d 6179 206f  nse..# You may o
+000000c0: 6274 6169 6e20 6120 636f 7079 206f 6620  btain a copy of 
+000000d0: 7468 6520 4c69 6365 6e73 6520 6174 0a23  the License at.#
+000000e0: 0a23 2068 7474 703a 2f2f 7777 772e 6170  .# http://www.ap
+000000f0: 6163 6865 2e6f 7267 2f6c 6963 656e 7365  ache.org/license
+00000100: 732f 4c49 4345 4e53 452d 322e 300a 230a  s/LICENSE-2.0.#.
+00000110: 2320 556e 6c65 7373 2072 6571 7569 7265  # Unless require
+00000120: 6420 6279 2061 7070 6c69 6361 626c 6520  d by applicable 
+00000130: 6c61 7720 6f72 2061 6772 6565 6420 746f  law or agreed to
+00000140: 2069 6e20 7772 6974 696e 672c 2073 6f66   in writing, sof
+00000150: 7477 6172 650a 2320 6469 7374 7269 6275  tware.# distribu
+00000160: 7465 6420 756e 6465 7220 7468 6520 4c69  ted under the Li
+00000170: 6365 6e73 6520 6973 2064 6973 7472 6962  cense is distrib
+00000180: 7574 6564 206f 6e20 616e 2022 4153 2049  uted on an "AS I
+00000190: 5322 2042 4153 4953 2c0a 2320 5749 5448  S" BASIS,.# WITH
+000001a0: 4f55 5420 5741 5252 414e 5449 4553 204f  OUT WARRANTIES O
+000001b0: 5220 434f 4e44 4954 494f 4e53 204f 4620  R CONDITIONS OF 
+000001c0: 414e 5920 4b49 4e44 2c20 6569 7468 6572  ANY KIND, either
+000001d0: 2065 7870 7265 7373 206f 7220 696d 706c   express or impl
+000001e0: 6965 642e 0a23 2053 6565 2074 6865 204c  ied..# See the L
+000001f0: 6963 656e 7365 2066 6f72 2074 6865 2073  icense for the s
+00000200: 7065 6369 6669 6320 6c61 6e67 7561 6765  pecific language
+00000210: 2067 6f76 6572 6e69 6e67 2070 6572 6d69   governing permi
+00000220: 7373 696f 6e73 2061 6e64 0a23 206c 696d  ssions and.# lim
+00000230: 6974 6174 696f 6e73 2075 6e64 6572 2074  itations under t
+00000240: 6865 204c 6963 656e 7365 2e0a 2320 3d3d  he License..# ==
+00000250: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000260: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000270: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000280: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000290: 3d3d 3d3d 3d3d 3d3d 3d3d 0a22 2222 0a54  ==========.""".T
+000002a0: 696d 6573 666f 726d 6572 204d 6f64 656c  imesformer Model
+000002b0: 2e0a 2222 220a 6672 6f6d 202e 2069 6d70  ..""".from . imp
+000002c0: 6f72 7420 636f 6e66 6967 7572 6174 696f  ort configuratio
+000002d0: 6e5f 7469 6d65 7366 6f72 6d65 722c 206d  n_timesformer, m
+000002e0: 6f64 656c 696e 675f 7469 6d65 7366 6f72  odeling_timesfor
+000002f0: 6d65 722c 2069 6d61 6765 5f70 726f 6365  mer, image_proce
+00000300: 7373 696e 675f 7669 6465 6f6d 6165 0a66  ssing_videomae.f
+00000310: 726f 6d20 2e63 6f6e 6669 6775 7261 7469  rom .configurati
+00000320: 6f6e 5f74 696d 6573 666f 726d 6572 2069  on_timesformer i
+00000330: 6d70 6f72 7420 2a0a 6672 6f6d 202e 6d6f  mport *.from .mo
+00000340: 6465 6c69 6e67 5f74 696d 6573 666f 726d  deling_timesform
+00000350: 6572 2069 6d70 6f72 7420 2a0a 6672 6f6d  er import *.from
+00000360: 202e 696d 6167 655f 7072 6f63 6573 7369   .image_processi
+00000370: 6e67 5f76 6964 656f 6d61 6520 696d 706f  ng_videomae impo
+00000380: 7274 202a 0a0a 0a5f 5f61 6c6c 5f5f 203d  rt *...__all__ =
+00000390: 205b 5d0a 5f5f 616c 6c5f 5f2e 6578 7465   [].__all__.exte
+000003a0: 6e64 2863 6f6e 6669 6775 7261 7469 6f6e  nd(configuration
+000003b0: 5f74 696d 6573 666f 726d 6572 2e5f 5f61  _timesformer.__a
+000003c0: 6c6c 5f5f 290a 5f5f 616c 6c5f 5f2e 6578  ll__).__all__.ex
+000003d0: 7465 6e64 286d 6f64 656c 696e 675f 7469  tend(modeling_ti
+000003e0: 6d65 7366 6f72 6d65 722e 5f5f 616c 6c5f  mesformer.__all_
+000003f0: 5f29 0a5f 5f61 6c6c 5f5f 2e65 7874 656e  _).__all__.exten
+00000400: 6428 696d 6167 655f 7072 6f63 6573 7369  d(image_processi
+00000410: 6e67 5f76 6964 656f 6d61 652e 5f5f 616c  ng_videomae.__al
+00000420: 6c5f 5f29 0a                             l__).
```

## mindnlp/transformers/models/wav2vec2/configuration_wav2vec2.py

```diff
@@ -82,15 +82,15 @@
             convolutional layers.
         feat_proj_dropout (`float`, *optional*, defaults to 0.0):
             The dropout probability for output of the feature encoder.
         feat_extract_activation (`str, `optional`, defaults to `"gelu"`):
             The non-linear activation function (function or string) in the 1D convolutional layers of the feature
             extractor. If string, `"gelu"`, `"relu"`, `"selu"` and `"gelu_new"` are supported.
         feat_quantizer_dropout (`float`, *optional*, defaults to 0.0):
-            The dropout probabilitiy for quantized feature encoder states.
+            The dropout probability for quantized feature encoder states.
         conv_dim (`Tuple[int]` or `List[int]`, *optional*, defaults to `(512, 512, 512, 512, 512, 512, 512)`):
             A tuple of integers defining the number of input and output channels of each 1D convolutional layer in the
             feature encoder. The length of *conv_dim* defines the number of 1D convolutional layers.
         conv_stride (`Tuple[int]` or `List[int]`, *optional*, defaults to `(5, 2, 2, 2, 2, 2, 2)`):
             A tuple of integers defining the stride of each 1D convolutional layer in the feature encoder. The length
             of *conv_stride* defines the number of convolutional layers and has to match the length of *conv_dim*.
         conv_kernel (`Tuple[int]` or `List[int]`, *optional*, defaults to `(10, 3, 3, 3, 3, 3, 3)`):
@@ -140,15 +140,15 @@
         num_codevectors_per_group (`int`, *optional*, defaults to 320):
             Number of entries in each quantization codebook (group).
         num_codevector_groups (`int`, *optional*, defaults to 2):
             Number of codevector groups for product codevector quantization.
         contrastive_logits_temperature (`float`, *optional*, defaults to 0.1):
             The temperature *kappa* in the contrastive loss.
         feat_quantizer_dropout (`float`, *optional*, defaults to 0.0):
-            The dropout probabilitiy for the output of the feature encoder that's used by the quantizer.
+            The dropout probability for the output of the feature encoder that's used by the quantizer.
         num_negatives (`int`, *optional*, defaults to 100):
             Number of negative samples for the contrastive loss.
         codevector_dim (`int`, *optional*, defaults to 256):
             Dimensionality of the quantized feature vectors.
         proj_codevector_dim (`int`, *optional*, defaults to 256):
             Dimensionality of the final projection of both the quantized and the transformer features.
         diversity_loss_weight (`int`, *optional*, defaults to 0.1):
```

## mindnlp/transformers/models/xlm_roberta/modeling_xlm_roberta.py

```diff
@@ -20,15 +20,14 @@
 import math
 import logging
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import mindspore
 from mindspore import nn, ops, Parameter, Tensor
-from mindspore.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 from mindspore.common.initializer import initializer, Normal
 from mindnlp.utils import logging
 from .configuration_xlm_roberta import XLMRobertaConfig
 from ...activations import ACT2FN
 from ...modeling_utils import PreTrainedModel
 from ...ms_utils import apply_chunking_to_forward, find_pruneable_heads_and_indices, prune_linear_layer
 from ...modeling_outputs import (
@@ -859,16 +858,15 @@
         prediction_scores = self.lm_head(sequence_output)
 
         lm_loss = None
         if labels is not None:
             # we are doing next-token prediction; shift prediction scores and input ids by one
             shifted_prediction_scores = prediction_scores[:, :-1, :]
             labels = labels[:, 1:]
-            loss_fct = CrossEntropyLoss()
-            lm_loss = loss_fct(shifted_prediction_scores.view(-1, self.config.vocab_size), labels.view(-1))
+            lm_loss = ops.cross_entropy(shifted_prediction_scores.view(-1, self.config.vocab_size), labels.view(-1))
 
         if not return_dict:
             output = (prediction_scores,) + outputs[2:]
             return ((lm_loss,) + output) if lm_loss is not None else output
 
         return CausalLMOutputWithCrossAttentions(
             loss=lm_loss,
@@ -891,15 +889,15 @@
 
         return {"input_ids": input_ids, "attention_mask": attention_mask, "past_key_values": past_key_values}
 
     def _reorder_cache(self, past_key_values, beam_idx):
         reordered_past = ()
         for layer_past in past_key_values:
             reordered_past += (
-                tuple(past_state.index_select(0, beam_idx.to(past_state.device)) for past_state in layer_past),
+                tuple(past_state.index_select(0, beam_idx) for past_state in layer_past),
             )
         return reordered_past
 
 
 class XLMRobertaForMaskedLM(XLMRobertaPreTrainedModel):
     """XLMRobertaForMaskedLM"""
     _tied_weights_keys = ["lm_head.decoder.weight", "lm_head.decoder.bias"]
@@ -965,17 +963,15 @@
         )
         sequence_output = outputs[0]
         prediction_scores = self.lm_head(sequence_output)
 
         masked_lm_loss = None
         if labels is not None:
             # move labels to correct device to enable model parallelism
-            labels = labels.to(prediction_scores.device)
-            loss_fct = CrossEntropyLoss()
-            masked_lm_loss = loss_fct(prediction_scores.view(-1, self.config.vocab_size), labels.view(-1))
+            masked_lm_loss = ops.cross_entropy(prediction_scores.view(-1, self.config.vocab_size), labels.view(-1))
 
         if not return_dict:
             output = (prediction_scores,) + outputs[2:]
             return ((masked_lm_loss,) + output) if masked_lm_loss is not None else output
 
         return MaskedLMOutput(
             loss=masked_lm_loss,
@@ -1005,20 +1001,16 @@
 
         # project back to size of vocabulary with bias
         x = self.decoder(x)
 
         return x
 
     def _tie_weights(self):
-        # To tie those two weights if they get disconnected (on TPU or when the bias is resized)
-        # For accelerate compatibility and to not break backward compatibility
-        if self.decoder.bias.device.type == "meta":
-            self.decoder.bias = self.bias
-        else:
-            self.bias = self.decoder.bias
+        # To tie those two weights if they get disconnected
+        self.bias = self.decoder.bias
 
 
 class XLMRobertaForSequenceClassification(XLMRobertaPreTrainedModel):
     """XLMRobertaForSequenceClassification"""
     def __init__(self, config):
         super().__init__(config)
         self.num_labels = config.num_labels
@@ -1064,35 +1056,31 @@
         )
         sequence_output = outputs[0]
         logits = self.classifier(sequence_output)
 
         loss = None
         if labels is not None:
             # move labels to correct device to enable model parallelism
-            labels = labels.to(logits.device)
             if self.config.problem_type is None:
                 if self.num_labels == 1:
                     self.config.problem_type = "regression"
                 elif self.num_labels > 1 and labels.dtype in (mindspore.int64, mindspore.int32):
                     self.config.problem_type = "single_label_classification"
                 else:
                     self.config.problem_type = "multi_label_classification"
 
             if self.config.problem_type == "regression":
-                loss_fct = MSELoss()
                 if self.num_labels == 1:
-                    loss = loss_fct(logits.squeeze(), labels.squeeze())
+                    loss = ops.mse_loss(logits.squeeze(), labels.squeeze())
                 else:
-                    loss = loss_fct(logits, labels)
+                    loss = ops.mse_loss(logits, labels)
             elif self.config.problem_type == "single_label_classification":
-                loss_fct = CrossEntropyLoss()
-                loss = loss_fct(logits.view(-1, self.num_labels), labels.view(-1))
+                loss = ops.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
             elif self.config.problem_type == "multi_label_classification":
-                loss_fct = BCEWithLogitsLoss()
-                loss = loss_fct(logits, labels)
+                loss = ops.binary_cross_entropy_with_logits(logits, labels)
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return SequenceClassifierOutput(
             loss=loss,
@@ -1162,17 +1150,15 @@
         pooled_output = self.dropout(pooled_output)
         logits = self.classifier(pooled_output)
         reshaped_logits = logits.view(-1, num_choices)
 
         loss = None
         if labels is not None:
             # move labels to correct device to enable model parallelism
-            labels = labels.to(reshaped_logits.device)
-            loss_fct = CrossEntropyLoss()
-            loss = loss_fct(reshaped_logits, labels)
+            loss = ops.cross_entropy(reshaped_logits, labels)
 
         if not return_dict:
             output = (reshaped_logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return MultipleChoiceModelOutput(
             loss=loss,
@@ -1232,18 +1218,15 @@
         sequence_output = outputs[0]
 
         sequence_output = self.dropout(sequence_output)
         logits = self.classifier(sequence_output)
 
         loss = None
         if labels is not None:
-            # move labels to correct device to enable model parallelism
-            labels = labels.to(logits.device)
-            loss_fct = CrossEntropyLoss()
-            loss = loss_fct(logits.view(-1, self.num_labels), labels.view(-1))
+            loss = ops.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return TokenClassifierOutput(
             loss=loss,
@@ -1341,17 +1324,16 @@
             if len(end_positions.shape) > 1:
                 end_positions = end_positions.squeeze(-1)
             # sometimes the start/end positions are outside our model inputs, we ignore these terms
             ignored_index = start_logits.size(1)
             start_positions = start_positions.clamp(0, ignored_index)
             end_positions = end_positions.clamp(0, ignored_index)
 
-            loss_fct = CrossEntropyLoss(ignore_index=ignored_index)
-            start_loss = loss_fct(start_logits, start_positions)
-            end_loss = loss_fct(end_logits, end_positions)
+            start_loss = ops.cross_entropy(start_logits, start_positions, ignore_index=ignored_index)
+            end_loss = ops.cross_entropy(end_logits, end_positions, ignore_index=ignored_index)
             total_loss = (start_loss + end_loss) / 2
 
         if not return_dict:
             output = (start_logits, end_logits) + outputs[2:]
             return ((total_loss,) + output) if total_loss is not None else output
 
         return QuestionAnsweringModelOutput(
```

## mindnlp/transformers/models/xlnet/modeling_xlnet.py

```diff
@@ -20,15 +20,15 @@
 from dataclasses import dataclass
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 from mindspore.common.initializer import initializer, Normal
 
 import mindspore
-from mindspore import nn, Parameter, Tensor
+from mindspore import nn, ops, Parameter, Tensor
 from mindspore.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 
 from mindnlp. transformers. ms_utils import apply_chunking_to_forward
 from mindnlp. transformers. activations import ACT2FN
 from mindnlp. transformers. modeling_utils import PoolerAnswerClass, PoolerEndLogits, PoolerStartLogits, PreTrainedModel, SequenceSummary
 from mindnlp.utils import (ModelOutput, logging)
 from .configuration_xlnet import XLNetConfig
@@ -56,24 +56,24 @@
             )
 
         self.n_head = config.n_head
         self.d_head = config.d_head
         self.d_model = config.d_model
         self.scale = 1 / (config.d_head ** 0.5)
 
-        self.q = Parameter(mindspore.ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
-        self.k = Parameter(mindspore.ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
-        self.v = Parameter(mindspore.ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
-        self.o = Parameter(mindspore.ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
-        self.r = Parameter(mindspore.ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
-
-        self.r_r_bias = Parameter(mindspore.ops.zeros((self.n_head, self.d_head), dtype=mindspore.float32))
-        self.r_s_bias = Parameter(mindspore.ops.zeros((self.n_head, self.d_head), dtype=mindspore.float32))
-        self.r_w_bias = Parameter(mindspore.ops.zeros((self.n_head, self.d_head), dtype=mindspore.float32))
-        self.seg_embed = Parameter(mindspore.ops.zeros((2, self.n_head, self.d_head), dtype=mindspore.float32))
+        self.q = Parameter(ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
+        self.k = Parameter(ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
+        self.v = Parameter(ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
+        self.o = Parameter(ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
+        self.r = Parameter(ops.zeros((config.d_model, self.n_head, self.d_head), dtype=mindspore.float32))
+
+        self.r_r_bias = Parameter(ops.zeros((self.n_head, self.d_head), dtype=mindspore.float32))
+        self.r_s_bias = Parameter(ops.zeros((self.n_head, self.d_head), dtype=mindspore.float32))
+        self.r_w_bias = Parameter(ops.zeros((self.n_head, self.d_head), dtype=mindspore.float32))
+        self.seg_embed = Parameter(ops.zeros((2, self.n_head, self.d_head), dtype=mindspore.float32))
 
         self.layer_norm = nn.LayerNorm(config.d_model, epsilon=config.layer_norm_eps)
         self.dropout = nn.Dropout(p=config.dropout)
 
     def prune_heads(self, heads):
         raise NotImplementedError
 
@@ -82,29 +82,29 @@
         """perform relative shift to form the relative attention score."""
         x_size = x.shape
 
         x = x.reshape(x_size[1], x_size[0], x_size[2], x_size[3])
         x = x[1:, ...]
         x = x.reshape(x_size[0], x_size[1] - 1, x_size[2], x_size[3])
         # x = x[:, 0:klen, :, :]
-        x = mindspore.ops.index_select(x, 1, mindspore.ops.arange(klen, dtype=mindspore.int64))
+        x = ops.index_select(x, 1, ops.arange(klen, dtype=mindspore.int64))
 
         return x
 
     @staticmethod
     def rel_shift_bnij(x, klen=-1):
         x_size = x.shape
 
         x = x.reshape(x_size[0], x_size[1], x_size[3], x_size[2])
         x = x[:, :, 1:, :]
         x = x.reshape(x_size[0], x_size[1], x_size[2], x_size[3] - 1)
         # Note: the tensor-slice form was faster in my testing than torch.index_select
         #       However, tracing doesn't like the nature of the slice, and if klen changes
         #       during the run then it'll fail, whereas index_select will be fine.
-        x = mindspore.ops.index_select(x, 3, mindspore.ops.arange(klen, dtype=mindspore.int64))
+        x = ops.index_select(x, 3, ops.arange(klen, dtype=mindspore.int64))
         # x = x[:, :, :, :klen]
 
         return x
 
     def rel_attn_core(
             self,
             q_head,
@@ -115,56 +115,56 @@
             attn_mask=None,
             head_mask=None,
             output_attentions=False,
     ):
         """Core relative positional attention operations."""
 
         # content based attention score
-        ac = mindspore.ops.einsum("ibnd,jbnd->bnij", q_head + self.r_w_bias, k_head_h)
+        ac = ops.einsum("ibnd,jbnd->bnij", q_head + self.r_w_bias, k_head_h)
 
         # position based attention score
-        bd = mindspore.ops.einsum("ibnd,jbnd->bnij", q_head + self.r_r_bias, k_head_r)
+        bd = ops.einsum("ibnd,jbnd->bnij", q_head + self.r_r_bias, k_head_r)
         bd = self.rel_shift_bnij(bd, klen=ac.shape[3])
 
         # segment based attention score
         if seg_mat is None:
             ef = 0
         else:
-            ef = mindspore.ops.einsum("ibnd,snd->ibns", q_head + self.r_s_bias, self.seg_embed)
-            ef = mindspore.ops.einsum("ijbs,ibns->bnij", seg_mat, ef)
+            ef = ops.einsum("ibnd,snd->ibns", q_head + self.r_s_bias, self.seg_embed)
+            ef = ops.einsum("ijbs,ibns->bnij", seg_mat, ef)
 
         # merge attention scores and perform masking
         attn_score = (ac + bd + ef) * self.scale
         if attn_mask is not None:
             # attn_score = attn_score * (1 - attn_mask) - 1e30 * attn_mask
             if attn_mask.dtype == mindspore.float16:
-                attn_score = attn_score - 65500 * mindspore.ops.einsum("ijbn->bnij", attn_mask)
+                attn_score = attn_score - 65500 * ops.einsum("ijbn->bnij", attn_mask)
             else:
-                attn_score = attn_score - 1e30 * mindspore.ops.einsum("ijbn->bnij", attn_mask)
+                attn_score = attn_score - 1e30 * ops.einsum("ijbn->bnij", attn_mask)
 
         # attention probability
-        attn_prob = mindspore.ops.softmax(attn_score, axis=3)
+        attn_prob = ops.softmax(attn_score, axis=3)
         attn_prob = self.dropout(attn_prob)
 
         # Mask heads if we want to
         if head_mask is not None:
-            attn_prob = attn_prob * mindspore.ops.einsum("ijbn->bnij", head_mask)
+            attn_prob = attn_prob * ops.einsum("ijbn->bnij", head_mask)
 
         # attention output
-        attn_vec = mindspore.ops.einsum("bnij,jbnd->ibnd", attn_prob, v_head_h)
+        attn_vec = ops.einsum("bnij,jbnd->ibnd", attn_prob, v_head_h)
 
         if output_attentions:
-            return attn_vec, mindspore.ops.einsum("bnij->ijbn", attn_prob)
+            return attn_vec, ops.einsum("bnij->ijbn", attn_prob)
 
         return attn_vec
 
     def post_attention(self, h, attn_vec, residual=True):
         """Post-attention processing."""
         # post-attention projection (back to `d_model`)
-        attn_out = mindspore.ops.einsum("ibnd,hnd->ibh", attn_vec, self.o)
+        attn_out = ops.einsum("ibnd,hnd->ibh", attn_vec, self.o)
 
         attn_out = self.dropout(attn_out)
         if residual:
             attn_out = attn_out + h
         output = self.layer_norm(attn_out)
 
         return output
@@ -182,30 +182,30 @@
             head_mask=None,
             output_attentions=False,
     ):
         if g is not None:
             # Two-stream attention with relative positional encoding.
             # content based attention score
             if mems is not None and mems.dim() > 1:
-                cat = mindspore.ops.cat([mems, h], axis=0)
+                cat = ops.cat([mems, h], axis=0)
             else:
                 cat = h
 
             # content-based key head
-            k_head_h = mindspore.ops.einsum("ibh,hnd->ibnd", cat, self.k)
+            k_head_h = ops.einsum("ibh,hnd->ibnd", cat, self.k)
 
             # content-based value head
-            v_head_h = mindspore.ops.einsum("ibh,hnd->ibnd", cat, self.v)
+            v_head_h = ops.einsum("ibh,hnd->ibnd", cat, self.v)
 
             # position-based key head
-            k_head_r = mindspore.ops.einsum("ibh,hnd->ibnd", r, self.r)
+            k_head_r = ops.einsum("ibh,hnd->ibnd", r, self.r)
 
             # h-stream
             # content-stream query head
-            q_head_h = mindspore.ops.einsum("ibh,hnd->ibnd", h, self.q)
+            q_head_h = ops.einsum("ibh,hnd->ibnd", h, self.q)
 
             # core attention ops
             attn_vec_h = self.rel_attn_core(
                 q_head_h,
                 k_head_h,
                 v_head_h,
                 k_head_r,
@@ -219,34 +219,34 @@
                 attn_vec_h, attn_prob_h = attn_vec_h
 
             # post processing
             output_h = self.post_attention(h, attn_vec_h)
 
             # g-stream
             # query-stream query head
-            q_head_g = mindspore.ops.einsum("ibh,hnd->ibnd", g, self.q)
+            q_head_g = ops.einsum("ibh,hnd->ibnd", g, self.q)
 
             # core attention ops
             if target_mapping is not None:
-                q_head_g = mindspore.ops.einsum("mbnd,mlb->lbnd", q_head_g, target_mapping)
+                q_head_g = ops.einsum("mbnd,mlb->lbnd", q_head_g, target_mapping)
                 attn_vec_g = self.rel_attn_core(
                     q_head_g,
                     k_head_h,
                     v_head_h,
                     k_head_r,
                     seg_mat=seg_mat,
                     attn_mask=attn_mask_g,
                     head_mask=head_mask,
                     output_attentions=output_attentions,
                 )
 
                 if output_attentions:
                     attn_vec_g, attn_prob_g = attn_vec_g
 
-                attn_vec_g = mindspore.ops.einsum("lbnd,mlb->mbnd", attn_vec_g, target_mapping)
+                attn_vec_g = ops.einsum("lbnd,mlb->mbnd", attn_vec_g, target_mapping)
             else:
                 attn_vec_g = self.rel_attn_core(
                     q_head_g,
                     k_head_h,
                     v_head_h,
                     k_head_r,
                     seg_mat=seg_mat,
@@ -263,26 +263,26 @@
 
             if output_attentions:
                 attn_prob = attn_prob_h, attn_prob_g
 
         else:
             # Multi-head attention with relative positional encoding
             if mems is not None and mems.dim() > 1:
-                cat = mindspore.ops.cat([mems, h], axis=0)
+                cat = ops.cat([mems, h], axis=0)
             else:
                 cat = h
 
             # content heads
-            q_head_h = mindspore.ops.einsum("ibh,hnd->ibnd", h, self.q)
-            k_head_h = mindspore.ops.einsum("ibh,hnd->ibnd", cat, self.k)
-            v_head_h = mindspore.ops.einsum("ibh,hnd->ibnd", cat, self.v)
+            q_head_h = ops.einsum("ibh,hnd->ibnd", h, self.q)
+            k_head_h = ops.einsum("ibh,hnd->ibnd", cat, self.k)
+            v_head_h = ops.einsum("ibh,hnd->ibnd", cat, self.v)
 
             # positional heads
             # type casting for fp16 support
-            k_head_r = mindspore.ops.einsum("ibh,hnd->ibnd", r.type(self.r.dtype), self.r)
+            k_head_r = ops.einsum("ibh,hnd->ibnd", r.type(self.r.dtype), self.r)
 
             # core attention ops
             attn_vec = self.rel_attn_core(
                 q_head_h,
                 k_head_h,
                 v_head_h,
                 k_head_r,
@@ -679,120 +679,29 @@
     end_top_index: Optional[mindspore.Tensor] = None
     cls_logits: Optional[mindspore.Tensor] = None
     mems: Optional[List[mindspore.Tensor]] = None
     hidden_states: Optional[Tuple[mindspore.Tensor, ...]] = None
     attentions: Optional[Tuple[mindspore.Tensor, ...]] = None
 
 
-XLNET_START_DOCSTRING = r"""
-
-    This model inherits from [`PreTrainedModel`]. Check the superclass documentation for the generic methods the
-    library implements for all its model (such as downloading or saving, resizing the input embeddings, pruning heads
-    etc.)
-
-    This model is also a PyTorch [torch.nn.Module](https://pytorch.org/docs/stable/nn.html#torch.nn.Module) subclass.
-    Use it as a regular PyTorch Module and refer to the PyTorch documentation for all matter related to general usage
-    and behavior.
-
-    Parameters:
-        config ([`XLNetConfig`]): Model configuration class with all the parameters of the model.
-            Initializing with a config file does not load the weights associated with the model, only the
-            configuration. Check out the [`~PreTrainedModel.from_pretrained`] method to load the model weights.
-"""
-
-XLNET_INPUTS_DOCSTRING = r"""
-    Args:
-        input_ids (`torch.LongTensor` of shape `({0})`):
-            Indices of input sequence tokens in the vocabulary.
-
-            Indices can be obtained using [`AutoTokenizer`]. See [`PreTrainedTokenizer.encode`] and
-            [`PreTrainedTokenizer.__call__`] for details.
-
-            [What are input IDs?](../glossary#input-ids)
-        attention_mask (`torch.FloatTensor` of shape `({0})`, *optional*):
-            Mask to avoid performing attention on padding token indices. Mask values selected in `[0, 1]`:
-
-            - 1 for tokens that are **not masked**,
-            - 0 for tokens that are **masked**.
-
-            [What are attention masks?](../glossary#attention-mask)
-        mems (`List[torch.FloatTensor]` of length `config.n_layers`):
-            Contains pre-computed hidden-states (see `mems` output below) . Can be used to speed up sequential
-            decoding. The token ids which have their past given to this model should not be passed as `input_ids` as
-            they have already been computed.
-
-            `use_mems` has to be set to `True` to make use of `mems`.
-        perm_mask (`torch.FloatTensor` of shape `(batch_size, sequence_length, sequence_length)`, *optional*):
-            Mask to indicate the attention pattern for each input token with values selected in `[0, 1]`:
-
-            - if `perm_mask[k, i, j] = 0`, i attend to j in batch k;
-            - if `perm_mask[k, i, j] = 1`, i does not attend to j in batch k.
-
-            If not set, each token attends to all the others (full bidirectional attention). Only used during
-            pretraining (to define factorization order) or for sequential decoding (generation).
-        target_mapping (`torch.FloatTensor` of shape `(batch_size, num_predict, sequence_length)`, *optional*):
-            Mask to indicate the output tokens to use. If `target_mapping[k, i, j] = 1`, the i-th predict in batch k is
-            on the j-th token. Only used during pretraining for partial prediction or for sequential decoding
-            (generation).
-        token_type_ids (`torch.LongTensor` of shape `({0})`, *optional*):
-            Segment token indices to indicate first and second portions of the inputs. Indices are selected in `[0,
-            1]`:
-
-            - 0 corresponds to a *sentence A* token,
-            - 1 corresponds to a *sentence B* token.
-
-            [What are token type IDs?](../glossary#token-type-ids)
-        input_mask (`torch.FloatTensor` of shape `{0}`, *optional*):
-            Mask to avoid performing attention on padding token indices. Negative of `attention_mask`, i.e. with 0 for
-            real tokens and 1 for padding which is kept for compatibility with the original code base.
-
-            Mask values selected in `[0, 1]`:
-
-            - 1 for tokens that are **masked**,
-            - 0 for tokens that are **not masked**.
-
-            You can only uses one of `input_mask` and `attention_mask`.
-        head_mask (`torch.FloatTensor` of shape `(num_heads,)` or `(num_layers, num_heads)`, *optional*):
-            Mask to nullify selected heads of the self-attention modules. Mask values selected in `[0, 1]`:
-
-            - 1 indicates the head is **not masked**,
-            - 0 indicates the head is **masked**.
-
-        inputs_embeds (`torch.FloatTensor` of shape `({0}, hidden_size)`, *optional*):
-            Optionally, instead of passing `input_ids` you can choose to directly pass an embedded representation. This
-            is useful if you want more control over how to convert `input_ids` indices into associated vectors than the
-            model's internal embedding lookup matrix.
-        output_attentions (`bool`, *optional*):
-            Whether or not to return the attentions tensors of all attention layers. See `attentions` under returned
-            tensors for more detail.
-        output_hidden_states (`bool`, *optional*):
-            Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors for
-            more detail.
-        return_dict (`bool`, *optional*):
-            Whether or not to return a [`~utils.ModelOutput`] instead of a plain tuple.
-"""
-
-
 class XLNetModel(XLNetPreTrainedModel):
     def __init__(self, config):
         super().__init__(config)
 
-        mindspore.set_context(pynative_synchronize=True)
-
         self.mem_len = config.mem_len
         self.reuse_len = config.reuse_len
         self.d_model = config.d_model
         self.same_length = config.same_length
         self.attn_type = config.attn_type
         self.bi_data = config.bi_data
         self.clamp_len = config.clamp_len
         self.n_layer = config.n_layer
 
         self.word_embedding = nn.Embedding(config.vocab_size, config.d_model)
-        self.mask_emb = mindspore.Parameter(mindspore.ops.zeros((1, 1, config.d_model),dtype=mindspore.float32))
+        self.mask_emb = mindspore.Parameter(ops.zeros((1, 1, config.d_model),dtype=mindspore.float32))
         self.layer = nn.CellList([XLNetLayer(config) for _ in range(config.n_layer)])
         self.dropout = nn.Dropout(p=config.dropout)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def get_input_embeddings(self):
@@ -818,15 +727,15 @@
                ^ [0 0 0 0 0 1 1 1 1] [0 0 0 0 0 1 1 1 1]
                  [0 0 0 0 0 0 1 1 1] [1 0 0 0 0 0 1 1 1]
             qlen [0 0 0 0 0 0 0 1 1] [1 1 0 0 0 0 0 1 1]
                  [0 0 0 0 0 0 0 0 1] [1 1 1 0 0 0 0 0 1]
                v [0 0 0 0 0 0 0 0 0] [1 1 1 1 0 0 0 0 0]
 
         """
-        mask = mindspore.ops.ones((qlen, qlen + mlen))
+        mask = ops.ones((qlen, qlen + mlen))
         if self.same_length:
             mask_lo = mask[:, :qlen].tril(-1)
             mask.triu_(mlen + 1)
             mask[:, :qlen] += mask_lo
         else:
             mask.triu_(mlen + 1)
 
@@ -845,61 +754,61 @@
             # If `use_mems` is active and `mem_len` is defined, the model returns the last `mem_len` hidden
             # states. This is the preferred setting for training and long-form generation.
             cutoff = -self.mem_len
         if prev_mem is None:
             # if `use_mems` is active and `mem_len` is defined, the model
             new_mem = curr_out[cutoff:]
         else:
-            new_mem = mindspore.ops.cat([prev_mem, curr_out], axis=0)[cutoff:]
+            new_mem = ops.cat([prev_mem, curr_out], axis=0)[cutoff:]
 
         return new_mem
 
     @staticmethod
     def positional_embedding(pos_seq, inv_freq, bsz=None):
-        sinusoid_inp = mindspore.ops.einsum("i,d->id", pos_seq, inv_freq)
-        pos_emb = mindspore.ops.cat([mindspore.ops.sin(sinusoid_inp), mindspore.ops.cos(sinusoid_inp)], axis=-1)
+        sinusoid_inp = ops.einsum("i,d->id", pos_seq, inv_freq)
+        pos_emb = ops.cat([ops.sin(sinusoid_inp), ops.cos(sinusoid_inp)], axis=-1)
         pos_emb = pos_emb[:, None, :]
 
         if bsz is not None:
             pos_emb = pos_emb.expand(-1, bsz, -1)
 
         return pos_emb
 
     def relative_positional_encoding(self, qlen, klen, bsz=None):
         # create relative positional encoding.
-        freq_seq = mindspore.ops.arange(0, self.d_model, 2.0, dtype=mindspore.int64).float()
-        inv_freq = 1 / mindspore.ops.pow(10000, (freq_seq / self.d_model))
+        freq_seq = ops.arange(0, self.d_model, 2.0, dtype=mindspore.int64).float()
+        inv_freq = 1 / ops.pow(10000, (freq_seq / self.d_model))
 
         if self.attn_type == "bi":
             # beg, end = klen - 1, -qlen
             beg, end = klen, -qlen
         elif self.attn_type == "uni":
             # beg, end = klen - 1, -1
             beg, end = klen, -1
         else:
             raise ValueError(f"Unknown `attn_type` {self.attn_type}.")
 
         if self.bi_data:
-            fwd_pos_seq = mindspore.ops.arange(beg, end, -1.0, dtype=mindspore.int64).float()
-            bwd_pos_seq = mindspore.ops.arange(-beg, -end, 1.0, dtype=mindspore.int64).float()
+            fwd_pos_seq = ops.arange(beg, end, -1.0, dtype=mindspore.int64).float()
+            bwd_pos_seq = ops.arange(-beg, -end, 1.0, dtype=mindspore.int64).float()
 
             if self.clamp_len > 0:
                 fwd_pos_seq = fwd_pos_seq.clamp(-self.clamp_len, self.clamp_len)
                 bwd_pos_seq = bwd_pos_seq.clamp(-self.clamp_len, self.clamp_len)
 
             if bsz is not None:
                 fwd_pos_emb = self.positional_embedding(fwd_pos_seq, inv_freq, bsz // 2)
                 bwd_pos_emb = self.positional_embedding(bwd_pos_seq, inv_freq, bsz // 2)
             else:
                 fwd_pos_emb = self.positional_embedding(fwd_pos_seq, inv_freq)
                 bwd_pos_emb = self.positional_embedding(bwd_pos_seq, inv_freq)
 
-            pos_emb = mindspore.ops.cat([fwd_pos_emb, bwd_pos_emb], axis=1)
+            pos_emb = ops.cat([fwd_pos_emb, bwd_pos_emb], axis=1)
         else:
-            fwd_pos_seq = mindspore.ops.arange(beg, end, -1.0, dtype=mindspore.int64).float()
+            fwd_pos_seq = ops.arange(beg, end, -1.0, dtype=mindspore.int64).float()
             if self.clamp_len > 0:
                 fwd_pos_seq = fwd_pos_seq.clamp(-self.clamp_len, self.clamp_len)
             pos_emb = self.positional_embedding(fwd_pos_seq, inv_freq, bsz)
 
         return pos_emb
 
     def construct(
@@ -940,27 +849,27 @@
 
         # the original code for XLNet uses shapes [len, bsz] with the batch dimension at the end
         # but we want a unified interface in the library with the batch size on the first dimension
         # so we move here the first dimension (batch) to the end
         if input_ids is not None and inputs_embeds is not None:
             raise ValueError("You cannot specify both input_ids and inputs_embeds at the same time")
         elif input_ids is not None:
-            input_ids = input_ids.transpose(1, 0).contiguous()
+            input_ids = input_ids.swapaxes(1, 0)
             qlen, bsz = input_ids.shape[0], input_ids.shape[1]
         elif inputs_embeds is not None:
-            inputs_embeds = inputs_embeds.transpose(1, 0, 2).contiguous()
+            inputs_embeds = inputs_embeds.transpose(1, 0, 2)
             qlen, bsz = inputs_embeds.shape[0], inputs_embeds.shape[1]
         else:
             raise ValueError("You have to specify either input_ids or inputs_embeds")
 
-        token_type_ids = token_type_ids.transpose(1, 0).contiguous() if token_type_ids is not None else None
-        input_mask = input_mask.transpose(1, 0).contiguous() if input_mask is not None else None
-        attention_mask = attention_mask.transpose(1, 0).contiguous() if attention_mask is not None else None
-        perm_mask = perm_mask.permute(1, 2, 0).contiguous() if perm_mask is not None else None
-        target_mapping = target_mapping.permute(1, 2, 0).contiguous() if target_mapping is not None else None
+        token_type_ids = token_type_ids.swapaxes(1, 0) if token_type_ids is not None else None
+        input_mask = input_mask.swapaxes(1, 0) if input_mask is not None else None
+        attention_mask = attention_mask.swapaxes(1, 0) if attention_mask is not None else None
+        perm_mask = perm_mask.permute(1, 2, 0) if perm_mask is not None else None
+        target_mapping = target_mapping.permute(1, 2, 0) if target_mapping is not None else None
 
         mlen = mems[0].shape[0] if mems is not None and mems[0] is not None else 0
         klen = mlen + qlen
 
         dtype_float = self.dtype
 
         # Attention mask
@@ -986,28 +895,28 @@
             data_mask = perm_mask
         else:
             data_mask = None
 
         if data_mask is not None:
             # all mems can be attended to
             if mlen > 0:
-                mems_mask = mindspore.ops.zeros((data_mask.shape[0], mlen, bsz)).to(dtype=data_mask.dtype)
-                data_mask = mindspore.ops.cat([mems_mask, data_mask], axis=1)
+                mems_mask = ops.zeros((data_mask.shape[0], mlen, bsz)).to(dtype=data_mask.dtype)
+                data_mask = ops.cat([mems_mask, data_mask], axis=1)
             if attn_mask is None:
                 attn_mask = data_mask[:, :, :, None]
             else:
                 attn_mask += data_mask[:, :, :, None]
 
         if attn_mask is not None:
             attn_mask = (attn_mask > 0).to(dtype_float)
 
         if attn_mask is not None:
-            non_tgt_mask = -mindspore.ops.eye(qlen).to(dtype=attn_mask.dtype)
+            non_tgt_mask = -ops.eye(qlen).to(dtype=attn_mask.dtype)
             if mlen > 0:
-                non_tgt_mask = mindspore.ops.cat([mindspore.ops.zeros((qlen, mlen)).to(dtype=attn_mask.dtype), non_tgt_mask],
+                non_tgt_mask = ops.cat([ops.zeros((qlen, mlen)).to(dtype=attn_mask.dtype), non_tgt_mask],
                                                  axis=-1)
             non_tgt_mask = ((attn_mask + non_tgt_mask[:, :, None, None]) > 0).to(dtype=attn_mask.dtype)
         else:
             non_tgt_mask = None
 
         # Word embeddings and prepare h & g hidden states
         if inputs_embeds is not None:
@@ -1024,22 +933,22 @@
         else:
             output_g = None
 
         # Segment embedding
         if token_type_ids is not None:
             # Convert `token_type_ids` to one-hot `seg_mat`
             if mlen > 0:
-                mem_pad = mindspore.ops.zeros((mlen, bsz), dtype=mindspore.int64)
-                cat_ids = mindspore.ops.cat([mem_pad, token_type_ids], axis=0)
+                mem_pad = ops.zeros((mlen, bsz), dtype=mindspore.int64)
+                cat_ids = ops.cat([mem_pad, token_type_ids], axis=0)
             else:
                 cat_ids = token_type_ids
 
             # `1` indicates not in the same segment [qlen x klen x bsz]
             seg_mat = (token_type_ids[:, None] != cat_ids[None, :]).long()
-            seg_mat = mindspore.ops.one_hot(seg_mat, depth=2).to(dtype_float)
+            seg_mat = ops.one_hot(seg_mat, depth=2).to(dtype_float)
         else:
             seg_mat = None
 
         # Positional encoding
         pos_emb = self.relative_positional_encoding(qlen, klen, bsz=bsz)
         pos_emb = self.dropout(pos_emb)
 
@@ -1090,34 +999,34 @@
 
         # Add last hidden state
         if output_hidden_states:
             hidden_states.append((output_h, output_g) if output_g is not None else output_h)
 
         output = self.dropout(output_g if output_g is not None else output_h)
 
-        # Prepare outputs, we transpose back here to shape [bsz, len, hidden_dim] (cf. beginning of forward() method)
-        output = output.permute(1, 0, 2).contiguous()
+        # Prepare outputs, we swapaxes back here to shape [bsz, len, hidden_dim] (cf. beginning of forward() method)
+        output = output.permute(1, 0, 2)
 
         if not use_mems:
             new_mems = None
 
         if output_hidden_states:
             if output_g is not None:
-                hidden_states = tuple(h.permute(1, 0, 2).contiguous() for hs in hidden_states for h in hs)
+                hidden_states = tuple(h.permute(1, 0, 2) for hs in hidden_states for h in hs)
             else:
-                hidden_states = tuple(hs.permute(1, 0, 2).contiguous() for hs in hidden_states)
+                hidden_states = tuple(hs.permute(1, 0, 2) for hs in hidden_states)
 
         if output_attentions:
             if target_mapping is not None:
                 # when target_mapping is provided, there are 2-tuple of attentions
                 attentions = tuple(
-                    tuple(att_stream.permute(2, 3, 0, 1).contiguous() for att_stream in t) for t in attentions
+                    tuple(att_stream.permute(2, 3, 0, 1) for att_stream in t) for t in attentions
                 )
             else:
-                attentions = tuple(t.permute(2, 3, 0, 1).contiguous() for t in attentions)
+                attentions = tuple(t.permute(2, 3, 0, 1) for t in attentions)
 
         if not return_dict:
             return tuple(v for v in [output, new_mems, hidden_states, attentions] if v is not None)
 
         return XLNetModelOutput(
             last_hidden_state=output, mems=new_mems, hidden_states=hidden_states, attentions=attentions
         )
@@ -1143,35 +1052,35 @@
     def set_output_embeddings(self, new_embeddings):
         self.lm_loss = new_embeddings
 
     def prepare_inputs_for_generation(self, input_ids, past_key_values=None, use_mems=None, **kwargs):
         # Add dummy token at the end (no attention on this one)
 
         effective_batch_size = input_ids.shape[0]
-        dummy_token = mindspore.ops.zeros((effective_batch_size, 1), dtype=mindspore.int64)
+        dummy_token = ops.zeros((effective_batch_size, 1), dtype=mindspore.int64)
 
         # At every pass, the attention values for the new token and the two last generated tokens
         # are computed, the rest is reloaded from the `past` cache. A purely auto-regressive model would have
         # offset = 1; offset = 2 seems to have slightly better computation.
         offset = 2
 
         if past_key_values:
-            input_ids = mindspore.ops.cat([input_ids[:, -offset:], dummy_token], axis=1)
+            input_ids = ops.cat([input_ids[:, -offset:], dummy_token], axis=1)
         else:
-            input_ids = mindspore.ops.cat([input_ids, dummy_token], axis=1)
+            input_ids = ops.cat([input_ids, dummy_token], axis=1)
 
         # Build permutation mask so that previous tokens don't see last token
         sequence_length = input_ids.shape[1]
-        perm_mask = mindspore.ops.zeros(
+        perm_mask = ops.zeros(
             (effective_batch_size, sequence_length, sequence_length), dtype=mindspore.float32
         )
         perm_mask[:, :, -1] = 1.0
 
         # We'll only predict the last token
-        target_mapping = mindspore.ops.zeros(
+        target_mapping = ops.zeros(
             (effective_batch_size, 1, sequence_length), dtype=mindspore.float32
         )
         target_mapping[:, 0, -1] = 1.0
 
         inputs = {
             "input_ids": input_ids,
             "perm_mask": perm_mask,
@@ -1642,16 +1551,16 @@
             **kwargs,
         )
 
         sequence_output = outputs[0]
 
         logits = self.qa_outputs(sequence_output)
         start_logits, end_logits = logits.split(1, axis=-1)
-        start_logits = start_logits.squeeze(-1).contiguous()
-        end_logits = end_logits.squeeze(-1).contiguous()
+        start_logits = start_logits.squeeze(-1)
+        end_logits = end_logits.squeeze(-1)
 
         total_loss = None
         if start_positions is not None and end_positions is not None:
             # If we are on multi-GPU, split add a dimension
             if len(start_positions.shape) > 1:
                 start_positions = start_positions.squeeze(-1)
             if len(end_positions.shape) > 1:
@@ -1814,37 +1723,37 @@
                     hidden_states=transformer_outputs.hidden_states,
                     attentions=transformer_outputs.attentions,
                 )
 
         else:
             # during inference, compute the end logits based on beam search
             bsz, slen, hsz = hidden_states.shape
-            start_log_probs = mindspore.ops.softmax(start_logits, axis=-1)  # shape (bsz, slen)
+            start_log_probs = ops.softmax(start_logits, axis=-1)  # shape (bsz, slen)
 
-            start_top_log_probs, start_top_index = mindspore.ops.topk(
+            start_top_log_probs, start_top_index = ops.topk(
                 start_log_probs, self.start_n_top, dim=-1
             )  # shape (bsz, start_n_top)
             start_top_index_exp = start_top_index.unsqueeze(-1).expand(-1, -1, hsz)  # shape (bsz, start_n_top, hsz)
-            start_states = mindspore.ops.gather_elements(hidden_states, -2, start_top_index_exp)  # shape (bsz, start_n_top, hsz)
+            start_states = ops.gather_elements(hidden_states, -2, start_top_index_exp)  # shape (bsz, start_n_top, hsz)
             start_states = start_states.unsqueeze(1).expand(-1, slen, -1, -1)  # shape (bsz, slen, start_n_top, hsz)
 
             hidden_states_expanded = hidden_states.unsqueeze(2).expand_as(
                 start_states
             )  # shape (bsz, slen, start_n_top, hsz)
             p_mask = p_mask.unsqueeze(-1) if p_mask is not None else None
             end_logits = self.end_logits(hidden_states_expanded, start_states=start_states, p_mask=p_mask)
-            end_log_probs = mindspore.ops.softmax(end_logits, axis=1)  # shape (bsz, slen, start_n_top)
+            end_log_probs = ops.softmax(end_logits, axis=1)  # shape (bsz, slen, start_n_top)
 
-            end_top_log_probs, end_top_index = mindspore.ops.topk(
+            end_top_log_probs, end_top_index = ops.topk(
                 end_log_probs, self.end_n_top, dim=1
             )  # shape (bsz, end_n_top, start_n_top)
             end_top_log_probs = end_top_log_probs.view(-1, self.start_n_top * self.end_n_top)
             end_top_index = end_top_index.view(-1, self.start_n_top * self.end_n_top)
 
-            start_states = mindspore.ops.einsum(
+            start_states = ops.einsum(
                 "blh,bl->bh", hidden_states, start_log_probs
             )  # get the representation of START as weighted sum of hidden states
             cls_logits = self.answer_class(
                 hidden_states, start_states=start_states, cls_index=cls_index
             )  # Shape (batch size,): one single `cls_logits` for each sample
 
             if not return_dict:
```

## mindnlp/utils/download.py

```diff
@@ -29,15 +29,15 @@
 from pathlib import Path
 from urllib.parse import urlparse, parse_qs
 from tqdm.autonotebook import tqdm
 import requests
 from requests.exceptions import ProxyError, SSLError, HTTPError
 
 from mindnlp.configs import DEFAULT_ROOT, ENV_VARS_TRUE_VALUES, MINDNLP_CACHE, REPO_TYPES, HF_URL_BASE, \
-    HF_TOKEN
+    HF_TOKEN, MS_URL_BASE
 from .errors import (
     EntryNotFoundError,
     LocalEntryNotFoundError,
     RepositoryNotFoundError,
     ModelNotFoundError,
     GatedRepoError
 )
@@ -148,15 +148,15 @@
         ('{home}\.text', '{home}\aclImdb_v1.tar.gz')
 
     """
     if not os.path.exists(path):
         os.makedirs(path)
 
     retry_cnt = 0
-    retry_limit = 3
+    retry_limit = 5
 
     if download_file_name is None:
         name = extract_filename_from_url(url)
     else:
         name = download_file_name
 
     file_path = os.path.join(path, name)
@@ -167,41 +167,45 @@
 
     while not (os.path.exists(file_path) and check_md5(file_path, md5sum)):
         if retry_cnt < retry_limit:
             retry_cnt += 1
         else:
             raise HTTPError(
                 f"Download from {url} failed. " "Retry limit reached")
+
+        # get downloaded size
+        tmp_file_path = file_path + "_tmp"
+        if os.path.exists(tmp_file_path) and retry_cnt != 0:
+            file_size = os.path.getsize(tmp_file_path)
+            headers['Range'] = f'bytes={file_size}-'
+        else:
+            file_size = 0
         req = requests.get(url, stream=True, timeout=10, proxies=proxies, headers=headers)
 
         status = req.status_code
         if status == 404:
             raise EntryNotFoundError(f"Can not found url: {url}")
         if status == 401:
             raise GatedRepoError('You should have authorization to access the model.')
         if status == 429:
             raise HTTPError('Too many requests.')
         try:
-            tmp_file_path = file_path + "_tmp"
-            total_size = req.headers.get("content-length")
-            with open(tmp_file_path, "wb") as file:
-                if total_size:
-                    with tqdm(
-                        total=int(total_size), unit="B", unit_scale=True, unit_divisor=1024
-                    ) as pbar:
-                        for chunk in req.iter_content(chunk_size=1024):
-                            file.write(chunk)
-                            pbar.update(len(chunk))
-                else:
+            total_size = int(req.headers.get('content-length', 0)) + file_size
+            with open(tmp_file_path, "ab") as file:
+                with tqdm(
+                    total=int(total_size), unit="B", initial=file_size, unit_scale=True, unit_divisor=1024
+                ) as pbar:
                     for chunk in req.iter_content(chunk_size=1024):
                         if chunk:
                             file.write(chunk)
+                            pbar.update(len(chunk))
+
             shutil.move(tmp_file_path, file_path)
         except requests.exceptions.RequestException as e:
-            if retry_cnt >= retry_limit:
+            if retry_cnt > retry_limit:
                 raise
             print(f"Failed to download: {e}")
             print(f"Retrying... (attempt {retry_cnt}/{retry_limit})")
             time.sleep(1)  # Add a small delay before retrying
 
     return file_path
 
@@ -363,14 +367,15 @@
     force_download: bool = False,
     resume_download: bool = False,
     proxies: Optional[Dict[str, str]] = None,
     local_files_only: bool = False,
     revision = 'main',
     token = None,
     subfolder: str = "",
+    mirror: str = 'huggingface',
     repo_type: Optional[str] = None,
     user_agent: Optional[Union[str, Dict[str, str]]] = None,
     _raise_exceptions_for_gated_repo: bool = True,
     _raise_exceptions_for_missing_entries: bool = True,
     _raise_exceptions_for_connection_errors: bool = True,
 ):
     """
@@ -472,24 +477,24 @@
             cache_dir=cache_dir,
             user_agent=user_agent,
             force_download=force_download,
             proxies=proxies,
             resume_download=resume_download,
             local_files_only=local_files_only,
             revision=revision,
-            token=token
+            token=token,
+            mirror=mirror
         )
     except GatedRepoError as e:
         if not _raise_exceptions_for_missing_entries:
             return None
         if resolved_file is not None or not _raise_exceptions_for_gated_repo:
             return resolved_file
         raise EnvironmentError(
-            "You are trying to access a gated repo.\nMake sure to have access to it at "
-            f"https://hf-mirror.com/{path_or_repo_id}.\n{str(e)}"
+            "You are trying to access a gated repo.\nMake sure to have access to it."
         ) from e
     except RepositoryNotFoundError as e:
         raise EnvironmentError(
             f"{path_or_repo_id} is not a local folder and is nost a valid model identifier "
         ) from e
     except LocalEntryNotFoundError as e:
         # We try to see if we have a cached version (not up to date):
@@ -534,14 +539,15 @@
     user_agent: Union[Dict, str, None] = None,
     force_download: bool = False,
     proxies: Optional[Dict] = None,
     resume_download: bool = False,
     local_files_only: bool = False,
     revision: str = 'main',
     token: str = None,
+    mirror: str = 'huggingface'
 ) -> str:
     """Download a given file if it's not already present in the local cache.
     """
     if cache_dir is None:
         cache_dir = MINDNLP_CACHE
     if isinstance(cache_dir, Path):
         cache_dir = str(cache_dir)
@@ -572,30 +578,26 @@
             )
 
     pointer_path = os.path.join(storage_folder, relative_filename)
 
     if os.path.exists(pointer_path) and not force_download:
         return pointer_path
 
-    url = build_download_url(repo_id, filename, revision, repo_type=repo_type)
-    # check model whether exist
-    model_url = url[: url.rfind(repo_id) + len(repo_id)]
+    url = build_download_url(repo_id, filename, revision, repo_type=repo_type, mirror=mirror)
 
     token = HF_TOKEN if not token else token
 
     headers = None
     if token:
         headers = {
-            'authorization': f"Bearer {token}"
+            'authorization': f"Bearer {token}",
         }
-
+    else:
+        headers = {}
     try:
-        req = requests.head(model_url, timeout=3, proxies=proxies, headers=headers)
-        if req.status_code >= 400:
-            raise RepositoryNotFoundError(f"Can not found model: {repo_id}")
         pointer_path = http_get(url, storage_folder, download_file_name=relative_filename, proxies=proxies, headers=headers)
     except (requests.exceptions.SSLError,
             requests.exceptions.ProxyError,
             requests.exceptions.ConnectionError,
             requests.exceptions.Timeout):
         # Otherwise, our Internet connection is down.
         # etag is None
@@ -773,14 +775,15 @@
     proxies=None,
     resume_download=False,
     local_files_only=False,
     revision='main',
     token=None,
     user_agent=None,
     subfolder="",
+    mirror='huggingface'
 ):
     """
     For a given model:
 
     - download and cache all the shards of a sharded checkpoint if `pretrained_model_name_or_path` is a model ID on the
       Hub
     - returns the list of paths to all the shards, as well as some metadata.
@@ -823,15 +826,16 @@
                 force_download=force_download,
                 proxies=proxies,
                 resume_download=resume_download,
                 local_files_only=local_files_only,
                 user_agent=user_agent,
                 subfolder=subfolder,
                 revision=revision,
-                token=token
+                token=token,
+                mirror=mirror
             )
         # We have already dealt with RepositoryNotFoundError and RevisionNotFoundError when getting the index, so
         # we don't have to catch them here.
         except EntryNotFoundError as exc:
             raise EnvironmentError(
                 f"{pretrained_model_name_or_path} does not appear to have a file named {shard_filename} which is "
                 "required according to the checkpoint index."
@@ -842,19 +846,35 @@
                 " again after checking your internet connection."
             ) from exc
 
         cached_filenames.append(cached_filename)
 
     return cached_filenames, sharded_metadata
 
+MIRROR_MAP = {
+    'huggingface': HF_URL_BASE,
+    'modelscope': MS_URL_BASE,
+    'wisemodel': "https://awsdownload.wisemodel.cn/file-proxy/{}/-/raw/{}/{}",
+    'gitee': "https://ai.gitee.com/huggingface/{}/resolve/{}/{}",
+    'aifast': "https://aifasthub.com/models/{}/{}",
+}
 
 def build_download_url(
     repo_id: str,
     filename: str,
     revision: str,
     *,
     subfolder: Optional[str] = None,
     repo_type: Optional[str] = None,
+    mirror: str = 'huggingface'
 ) -> str:
     """Construct the URL of a file from the given information.
     """
-    return HF_URL_BASE.format(repo_id, revision, filename)
+    if mirror not in MIRROR_MAP:
+        raise ValueError('The mirror name not support, please use one of the mirror website below: '
+                         '["huggingface", "modelscope", "wisemodel", "gitee", "aifast"]')
+    if mirror in ('huggingface', 'gitee', 'modelscope', 'wisemodel'):
+        return MIRROR_MAP[mirror].format(repo_id, revision, filename)
+    if revision is not None and revision != 'main':
+        logger.warning(f'`revision` is not support when use "{mirror}" website. '
+                    f'If you want use specific revision, please use "modelscope", "huggingface" or "gitee".')
+    return MIRROR_MAP[mirror].format(repo_id, filename)
```

## mindnlp/utils/generic.py

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 Generic utils.
 """
+import inspect
 from enum import Enum
 from collections import OrderedDict, UserDict
 from dataclasses import fields
 from typing import Any, Tuple, ContextManager, List
 from contextlib import ExitStack
 
 import numpy as np
@@ -335,7 +336,37 @@
     """no grad wrapper"""
     def wrapper(*args, **kwargs):
         _pynative_executor.set_enable_grad(False)
         outputs = func(*args, **kwargs)
         _pynative_executor.set_enable_grad(True)
         return outputs
     return wrapper
+
+def find_labels(model_class):
+    """
+    Find the labels used by a given model.
+
+    Args:
+        model_class (`type`): The class of the model.
+    """
+    model_name = model_class.__name__
+    signature = inspect.signature(model_class.construct)  # TensorFlow models
+
+    if "QuestionAnswering" in model_name:
+        return [p for p in signature.parameters if "label" in p or p in ("start_positions", "end_positions")]
+    else:
+        return [p for p in signature.parameters if "label" in p]
+
+def can_return_loss(model_class):
+    """
+    Check if a given model can return loss.
+
+    Args:
+        model_class (`type`): The class of the model.
+    """
+    signature = inspect.signature(model_class.construct)  # TensorFlow models
+
+    for p in signature.parameters:
+        if p == "return_loss" and signature.parameters[p].default is True:
+            return True
+
+    return False
```

## mindnlp/utils/logging.py

```diff
@@ -10,25 +10,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
+# pylint: disable=unused-import
 """ Logging utilities."""
 
 import functools
 import logging
 import os
 import sys
 import threading
 from logging import (
+    CRITICAL,  # NOQA
     DEBUG,  # NOQA
     ERROR,  # NOQA
+    FATAL,  # NOQA
     INFO,  # NOQA
+    NOTSET,  # NOQA
+    WARN,  # NOQA
     WARNING,  # NOQA
 )
 from logging import captureWarnings as _captureWarnings
 from typing import Optional
 
 from tqdm import auto as tqdm_lib
```

## mindnlp/utils/serialization.py

```diff
@@ -33,14 +33,16 @@
 from functools import reduce
 from dataclasses import dataclass
 from ml_dtypes import bfloat16
 
 import numpy as np
 import mindspore
 from mindspore import Tensor
+import safetensors
+import safetensors.numpy
 
 from . import logging
 
 logger = logging.get_logger(__name__)
 
 MAGIC_NUMBER = 0x1950a86a20f9469cfc6c
 PROTOCOL_VERSION = 1001
@@ -593,7 +595,15 @@
     try:
         mindspore.save_checkpoint(ms_ckpt, ms_ckpt_path)
     except Exception as exc:
         raise RuntimeError(f'Save checkpoint to {ms_ckpt_path} failed, '
                             f'please checkout the path.') from exc
 
     return ms_ckpt_path
+
+def safe_load_file(filename):
+    state_dict = safetensors.numpy.load_file(filename)
+    return {k: mindspore.Parameter(v) for k, v in state_dict.items()}
+
+def safe_save_file(tensor_dict, filename, metadata=None):
+    tensor_dict = {k: v.asnumpy() for k, v in tensor_dict.items()}
+    return safetensors.numpy.save_file(tensor_dict, filename, metadata)
```

## mindnlp/utils/testing_utils.py

```diff
@@ -49,18 +49,19 @@
     is_pytest_available,
     is_mindspore_available,
     is_essentia_available,
     is_librosa_available,
     is_pretty_midi_available,
     is_scipy_available,
     is_pyctcdecode_available,
-    is_vision_available,
+    is_safetensors_available,
     is_sentencepiece_available,
     is_tokenizers_available,
     is_pytesseract_available,
+    is_vision_available
 )
 from .generic import strtobool
 
 if is_pytest_available():
     from _pytest.doctest import (
         Module,
         _get_checker,
@@ -146,14 +147,21 @@
     else:
         try:
             _value = int(value)
         except ValueError as exc:
             raise ValueError(f"If set, {key} must be a int.") from exc
     return _value
 
+def require_vision(test_case):
+    """
+    Decorator marking a test that requires the vision dependencies. These tests are skipped when torchaudio isn't
+    installed.
+    """
+    return unittest.skipUnless(is_vision_available(), "test requires vision")(test_case)
+
 def require_tokenizers(test_case):
     """
     Decorator marking a test that requires 🤗 Tokenizers. These tests are skipped when 🤗 Tokenizers isn't installed.
     """
     return unittest.skipUnless(is_tokenizers_available(), "test requires tokenizers")(test_case)
 
 def require_sentencepiece(test_case):
@@ -206,20 +214,19 @@
 
 def require_pyctcdecode(test_case):
     """
     Decorator marking a test that requires pyctcdecode
     """
     return unittest.skipUnless(is_pyctcdecode_available(), "test requires pyctcdecode")(test_case)
 
-def require_vision(test_case):
+def require_safetensors(test_case):
     """
-    Decorator marking a test that requires the vision dependencies. These tests are skipped when torchaudio isn't
-    installed.
+    Decorator marking a test that requires safetensors. These tests are skipped when safetensors isn't installed.
     """
-    return unittest.skipUnless(is_vision_available(), "test requires vision")(test_case)
+    return unittest.skipUnless(is_safetensors_available(), "test requires safetensors")(test_case)
 
 def require_pytesseract(test_case):
     """
     Decorator marking a test that requires pytesseract
     """
     return unittest.skipUnless(is_pytesseract_available(), "test requires pytesseract")(test_case)
 
@@ -1413,7 +1420,25 @@
             assert len(lines) >= 3
             # each key one line, ident should be 2, min length is 3
             assert lines[0].strip() == "{"
             for _ in lines[1:-1]:
                 left_indent = len(lines[1]) - len(lines[1].lstrip())
                 assert left_indent == 2
             assert lines[-1].strip() == "}"
+
+_run_staging = parse_flag_from_env("MINDNLP_CO_STAGING", default=False)
+
+def is_staging_test(test_case):
+    """
+    Decorator marking a test as a staging test.
+
+    Those tests will run using the staging environment of huggingface.co instead of the real model hub.
+    """
+    if not _run_staging:
+        return unittest.skip("test is staging test")(test_case)
+    else:
+        try:
+            import pytest  # We don't need a hard dependency on pytest in the main library
+        except ImportError:
+            return test_case
+        else:
+            return pytest.mark.is_staging_test()(test_case)
```

## tests/ut/engine/test_trainer.py

```diff
@@ -1,173 +1,2104 @@
-# Copyright 2022 Huawei Technologies Co., Ltd
+# coding=utf-8
+# Copyright 2018 the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ============================================================================
-"""Test Trainer run function"""
-# pylint: disable=C0103
-# pylint: disable=W0621
+
+import dataclasses
+import gc
+import json
+import math
+import os
+import random
+import re
+import subprocess
+import sys
+import tempfile
 import unittest
+from itertools import product
+from pathlib import Path
+from typing import Dict, List
+from unittest.mock import Mock, patch
+import pytest
+
 import numpy as np
-from ddt import ddt, data
-from mindspore import nn, Tensor
-import mindspore.dataset as ds
-
-from mindnlp.engine.trainer import Trainer
-from mindnlp.metrics import Accuracy
-from mindnlp.engine.callbacks.timer_callback import TimerCallback
-from mindnlp.engine.callbacks.earlystop_callback import EarlyStopCallback
-from mindnlp.engine.callbacks.best_model_callback import BestModelCallback
-from mindnlp.engine.callbacks.checkpoint_callback import CheckpointCallback
-
-np.random.seed(1)
-
-class MyDataset:
-    """Dataset"""
-    def __init__(self):
-        self.data = np.random.randn(20, 3).astype(np.float32)
-        self.label = list(np.random.choice([0, 1]).astype(np.float32) for i in range(20))
-        self.length = list(np.random.choice([0, 1]).astype(np.float32) for i in range(20))
+from parameterized import parameterized
+from requests.exceptions import HTTPError
+
+from mindnlp.engine import (
+    IntervalStrategy,
+    TrainerCallback,
+    TrainingArguments
+)
+from mindnlp.transformers import (
+    AutoTokenizer,
+    PretrainedConfig,
+)
+from mindnlp.modules.optimization import get_polynomial_decay_schedule_with_warmup
+from mindnlp.utils import is_mindspore_available, logging
+from mindnlp.utils.serialization import safe_load_file, safe_save_file
+from mindnlp.utils.testing_utils import (
+    # ENDPOINT_STAGING,
+    # TOKEN,
+    # USER,
+    CaptureLogger,
+    LoggingLevel,
+    TestCasePlus,
+    execute_subprocess_async,
+    get_tests_dir,
+    is_staging_test,
+    require_safetensors,
+    require_sentencepiece,
+    require_tokenizers,
+    require_mindspore,
+    slow,
+)
+from mindnlp.transformers.tokenization_utils_base import PreTrainedTokenizerBase
+from mindnlp.engine.utils import PREFIX_CHECKPOINT_DIR, get_last_checkpoint
+from mindnlp.engine.train_args import OptimizerNames
+from mindnlp.utils import (
+    is_safetensors_available,
+)
+from mindnlp.configs import (
+    SAFE_WEIGHTS_INDEX_NAME,
+    SAFE_WEIGHTS_NAME,
+    WEIGHTS_INDEX_NAME,
+    WEIGHTS_NAME,
+)
+
+if is_mindspore_available():
+    import mindspore
+    from mindspore import nn, ops
+    from mindspore.dataset import GeneratorDataset
+
+    # import transformers.optimization
+    from mindnlp.engine.callbacks import (
+        EarlyStoppingCallback
+    )
+    from mindnlp.transformers import (
+        AutoModelForCausalLM,
+        AutoModelForSequenceClassification,
+        # GlueDataset,
+        # GlueDataTrainingArguments,
+        GPT2Config,
+        GPT2LMHeadModel,
+        # LineByLineTextDataset,
+        PreTrainedModel,
+    )
+    from mindnlp.engine import Trainer, TrainerState
+    # from mindnlp.transformers.modeling_utils import unwrap_model
+
+
+PATH_SAMPLE_TEXT = f"{get_tests_dir()}/fixtures/sample_text.txt"
+
+
+class RegressionDataset:
+    def __init__(self, a=2, b=3, length=64, seed=42, label_names=None):
+        np.random.seed(seed)
+        self.label_names = ["labels"] if label_names is None else label_names
+        self.length = length
+        self.x = np.random.normal(size=(length,)).astype(np.float32)
+        self.ys = [a * self.x + b + np.random.normal(scale=0.1, size=(length,)) for _ in self.label_names]
+        self.ys = [y.astype(np.float32) for y in self.ys]
+
+    def __len__(self):
+        return self.length
+
+    def __getitem__(self, i):
+        result = [self.x[i]]
+        for y in self.ys:
+            result.append(y[i])
+        return tuple(result)
+
+@dataclasses.dataclass
+class RegressionTrainingArguments(TrainingArguments):
+    a: float = 0.0
+    b: float = 0.0
+    keep_report_to: bool = False
+
+    def __post_init__(self):
+        super().__post_init__()
+        # save resources not dealing with reporting unless specified (also avoids the warning when it's not set)
+        # can be explicitly disabled via `keep_report_to`
+        if not self.keep_report_to:
+            self.report_to = []
+
+
+class RepeatDataset:
+    def __init__(self, x, length=64):
+        self.x = x
+        self.length = length
+
+    def __len__(self):
+        return self.length
 
-    def __getitem__(self, index):
-        return self.data[index], self.label[index], self.length[index]
+    def __getitem__(self, i):
+        return self.x, self.x
+
+
+class DynamicShapesDataset:
+    def __init__(self, length=64, seed=42, batch_size=8):
+        self.length = length
+        np.random.seed(seed)
+        sizes = np.random.randint(1, 20, (length // batch_size,))
+        # For easy batching, we make every batch_size consecutive samples the same size.
+        self.xs = [np.random.normal(size=(s,)).astype(np.float32) for s in sizes.repeat(batch_size)]
+        self.ys = [np.random.normal(size=(s,)).astype(np.float32) for s in sizes.repeat(batch_size)]
 
     def __len__(self):
-        return len(self.data)
+        return self.length
+
+    def __getitem__(self, i):
+        return self.xs[i], self.ys[i]
+
 
-class MyModel(nn.Cell):
-    """Model"""
-    def __init__(self):
-        super().__init__()
-        self.fc = nn.Dense(3, 1)
-
-    def construct(self, data):
-        output = self.fc(data)
-        return output
-
-class MyModel2(nn.Cell):
-    """Model2"""
-    def __init__(self):
-        super().__init__()
-        self.fc = nn.Dense(3, 1)
-
-    def construct(self, data, label, length):
-        output = self.fc(data)
-        label = label + label + length
-        return output
-
-
-class MyModelWithLoss(nn.Cell):
-    """Model"""
-    def __init__(self):
-        super().__init__()
-        self.fc = nn.Dense(3, 1)
-        self.loss = nn.MSELoss()
-    def construct(self, data, label) -> Tensor:
-        output = self.fc(data)
-        loss = self.loss(output, label)
-        return loss
-
-@ddt
-class TestTrainerRun(unittest.TestCase):
-    r"""
-    Test Trainer Run
+class AlmostAccuracy:
+    def __init__(self, thresh=0.25):
+        self.thresh = thresh
+
+    def __call__(self, eval_pred):
+        predictions, labels = eval_pred
+        true = np.abs(predictions - labels) <= self.thresh
+        return {"accuracy": true.astype(np.float32).mean().item()}
+
+
+class RegressionModelConfig(PretrainedConfig):
+    def __init__(self, a=0, b=0, double_output=False, random_ms=True, **kwargs):
+        super().__init__(**kwargs)
+        self.a = a
+        self.b = b
+        self.double_output = double_output
+        self.random_ms = random_ms
+        self.hidden_size = 1
+
+
+if is_mindspore_available():
+
+    class SampleIterableDataset:
+        def __init__(self, a=2, b=3, length=64, seed=42, label_names=None):
+            self.dataset = RegressionDataset(a=a, b=b, length=length, seed=seed, label_names=label_names)
+
+        def __iter__(self):
+            for i in range(len(self.dataset)):
+                yield self.dataset[i]
+
+    class FiniteIterableDataset(SampleIterableDataset):
+        def __init__(self, a=2, b=3, length=64, seed=42, label_names=None):
+            super().__init__(a, b, length, seed, label_names)
+            self.current_sample = 0
+
+        def __iter__(self):
+            while self.current_sample < len(self.dataset):
+                yield self.dataset[self.current_sample]
+                self.current_sample += 1
+
+    class MultiLoader:
+        def __init__(self, loaders):
+            self.loaders = loaders
+
+        def __len__(self):
+            return sum(len(loader) for loader in self.loaders)
+
+        def __iter__(self):
+            for loader in self.loaders:
+                yield from loader
+
+    class RegressionModel(nn.Cell):
+        def __init__(self, a=0, b=0, double_output=False):
+            super().__init__()
+            self.a = mindspore.Parameter(mindspore.tensor([a]).float())
+            self.b = mindspore.Parameter(mindspore.tensor([b]).float())
+            self.double_output = double_output
+            self.config = None
+
+        def construct(self, input_x, labels=None, **kwargs):
+            y = input_x * self.a + self.b
+            if labels is None:
+                return (y, y) if self.double_output else (y,)
+            loss = ops.mse_loss(y, labels)
+            return (loss, y, y) if self.double_output else (loss, y)
+
+    class RegressionDictModel(nn.Cell):
+        def __init__(self, a=0, b=0):
+            super().__init__()
+            self.a = mindspore.Parameter(mindspore.tensor([a]).float())
+            self.b = mindspore.Parameter(mindspore.tensor([b]).float())
+            self.config = None
+
+        def construct(self, input_x, labels=None, **kwargs):
+            y = input_x * self.a + self.b
+            result = {"output": y}
+            if labels is not None:
+                result["loss"] = ops.mse_loss(y, labels)
+            return result
+
+    class RegressionPreTrainedModel(PreTrainedModel):
+        config_class = RegressionModelConfig
+        base_model_prefix = "regression"
+
+        def __init__(self, config):
+            super().__init__(config)
+            self.a = mindspore.Parameter(mindspore.tensor([config.a]).float())
+            self.b = mindspore.Parameter(mindspore.tensor([config.b]).float())
+            self.double_output = config.double_output
+
+        def construct(self, input_x, labels=None, **kwargs):
+            y = input_x * self.a + self.b
+            if labels is None:
+                return (y, y) if self.double_output else (y,)
+            loss = ops.mse_loss(y, labels)
+            return (loss, y, y) if self.double_output else (loss, y)
+
+    class RegressionRandomPreTrainedModel(PreTrainedModel):
+        config_class = RegressionModelConfig
+        base_model_prefix = "regression"
+
+        def __init__(self, config):
+            super().__init__(config)
+            self.a = mindspore.Parameter(mindspore.tensor([config.a]).float())
+            self.b = mindspore.Parameter(mindspore.tensor([config.b]).float())
+            self.random_ms = config.random_ms
+
+        def construct(self, input_x, labels=None, **kwargs):
+            y = input_x * self.a + self.b
+            if self.random_ms:
+                torch_rand = ops.randn(1).squeeze()
+            np_rand = np.random.rand()
+            rand_rand = random.random()
+
+            if self.random_ms:
+                y += 0.05 * torch_rand
+            y += 0.05 * mindspore.tensor(np_rand + rand_rand)
+
+            if labels is None:
+                return (y,)
+            loss = ops.mse_loss(y, labels)
+            return (loss, y)
+
+    class TstLayer(nn.Cell):
+        def __init__(self, hidden_size):
+            super().__init__()
+            self.linear1 = nn.Dense(hidden_size, hidden_size)
+            self.ln1 = nn.LayerNorm(hidden_size)
+            self.linear2 = nn.Dense(hidden_size, hidden_size)
+            self.ln2 = nn.LayerNorm(hidden_size)
+            self.bias = mindspore.Parameter(ops.zeros(hidden_size))
+
+        def construct(self, x):
+            h = self.ln1(ops.relu(self.linear1(x)))
+            h = ops.relu(self.linear2(x))
+            return self.ln2(x + h + self.bias)
+
+    def get_regression_trainer(
+        a=0, b=0, double_output=False, train_len=64, eval_len=64, pretrained=True, keep_report_to=False, **kwargs
+    ):
+        label_names = kwargs.get("label_names", None)
+
+        column_names = ['input_x']
+        if label_names is None:
+            column_names.append('labels')
+        else:
+            column_names.extend(label_names)
+        gradient_checkpointing = kwargs.get("gradient_checkpointing", False)
+        train_dataset = GeneratorDataset(RegressionDataset(length=train_len, label_names=label_names), column_names=column_names)
+        eval_dataset = GeneratorDataset(RegressionDataset(length=eval_len, label_names=label_names), column_names=column_names, shuffle=False)
+
+        model_init = kwargs.pop("model_init", None)
+        if model_init is not None:
+            model = None
+        else:
+            if pretrained:
+                config = RegressionModelConfig(a=a, b=b, double_output=double_output)
+                # We infer the correct model class if one uses gradient_checkpointing or not
+                target_cls = (
+                    RegressionPreTrainedModel
+                )
+                model = target_cls(config)
+            else:
+                model = RegressionModel(a=a, b=b, double_output=double_output)
+
+        compute_metrics = kwargs.pop("compute_metrics", None)
+        optimizers = kwargs.pop("optimizers", (None, None))
+        output_dir = kwargs.pop("output_dir", "./regression")
+        preprocess_logits_for_metrics = kwargs.pop("preprocess_logits_for_metrics", None)
+
+        args = RegressionTrainingArguments(output_dir, a=a, b=b, keep_report_to=keep_report_to, **kwargs)
+        return Trainer(
+            model,
+            args,
+            train_dataset=train_dataset,
+            eval_dataset=eval_dataset,
+            compute_metrics=compute_metrics,
+            optimizers=optimizers,
+            model_init=model_init,
+            preprocess_logits_for_metrics=preprocess_logits_for_metrics,
+        )
+
+
+class TrainerIntegrationCommon:
+    def check_saved_checkpoints(self, output_dir, freq, total, is_pretrained=True, safe_weights=True):
+        weights_file = WEIGHTS_NAME if not safe_weights else SAFE_WEIGHTS_NAME
+        file_list = [weights_file]#, "training_args.bin", "optimizer.ckpt", "scheduler.json", "trainer_state.json"]
+        if is_pretrained:
+            file_list.append("config.json")
+        for step in range(freq, total, freq):
+            checkpoint = os.path.join(output_dir, f"checkpoint-{step}")
+            self.assertTrue(os.path.isdir(checkpoint))
+            for filename in file_list:
+                self.assertTrue(os.path.isfile(os.path.join(checkpoint, filename)))
+
+    def check_best_model_has_been_loaded(
+        self, output_dir, freq, total, trainer, metric, greater_is_better=False, is_pretrained=True, safe_weights=True
+    ):
+        checkpoint = os.path.join(output_dir, f"checkpoint-{(total // freq) * freq}")
+        log_history = TrainerState.load_from_json(os.path.join(checkpoint, "trainer_state.json")).log_history
+
+        values = [d[metric] for d in log_history]
+        best_value = max(values) if greater_is_better else min(values)
+        best_checkpoint = (values.index(best_value) + 1) * freq
+        checkpoint = os.path.join(output_dir, f"checkpoint-{best_checkpoint}")
+        if is_pretrained:
+            best_model = RegressionPreTrainedModel.from_pretrained(checkpoint)
+        else:
+            best_model = RegressionModel()
+            if not safe_weights:
+                state_dict = mindspore.load_checkpoint(os.path.join(checkpoint, WEIGHTS_NAME))
+            else:
+                state_dict = safe_load_file(os.path.join(checkpoint, SAFE_WEIGHTS_NAME))
+            best_model.load_state_dict(state_dict)
+        self.assertTrue(np.allclose(best_model.a.asnumpy(), trainer.model.a.asnumpy()))
+        self.assertTrue(np.allclose(best_model.b.asnumpy(), trainer.model.b.asnumpy()))
+
+        metrics = trainer.evaluate()
+        self.assertEqual(metrics[metric], best_value)
+
+    def check_trainer_state_are_the_same(self, trainer_state, trainer_state1):
+        # We'll pop things so operate on copies.
+        state = trainer_state.copy()
+        state1 = trainer_state1.copy()
+        # Log history main contain different logs for the time metrics (after resuming a training).
+        log_history = state.pop("log_history", None)
+        log_history1 = state1.pop("log_history", None)
+        self.assertEqual(state, state1)
+        skip_log_keys = ["train_runtime", "train_samples_per_second", "train_steps_per_second", "train_loss"]
+        for log, log1 in zip(log_history, log_history1):
+            for key in skip_log_keys:
+                _ = log.pop(key, None)
+                _ = log1.pop(key, None)
+            self.assertEqual(log, log1)
+
+    def convert_to_sharded_checkpoint(self, folder, save_safe=True, load_safe=True):
+        # Converts a checkpoint of a regression model to a sharded checkpoint.
+        if load_safe:
+            loader = safe_load_file
+            weights_file = os.path.join(folder, SAFE_WEIGHTS_NAME)
+        else:
+            loader = mindspore.load_checkpoint
+            weights_file = os.path.join(folder, WEIGHTS_NAME)
+
+        if save_safe:
+            extension = "safetensors"
+            saver = safe_save_file
+            index_file = os.path.join(folder, SAFE_WEIGHTS_INDEX_NAME)
+            shard_name = SAFE_WEIGHTS_NAME
+        else:
+            extension = "ckpt"
+            saver = mindspore.save_checkpoint
+            index_file = os.path.join(folder, WEIGHTS_INDEX_NAME)
+            shard_name = WEIGHTS_NAME
+
+        state_dict = loader(weights_file)
+
+        os.remove(weights_file)
+        keys = list(state_dict.keys())
+
+        shard_files = [
+            shard_name.replace(f".{extension}", f"-{idx+1:05d}-of-{len(keys):05d}.{extension}")
+            for idx in range(len(keys))
+        ]
+        index = {"metadata": {}, "weight_map": {key: shard_files[i] for i, key in enumerate(keys)}}
+
+        with open(index_file, "w", encoding="utf-8") as f:
+            content = json.dumps(index, indent=2, sort_keys=True) + "\n"
+            f.write(content)
+
+        for param_name, shard_file in zip(keys, shard_files):
+            saver({param_name: state_dict[param_name]}, os.path.join(folder, shard_file))
+
+@require_mindspore
+@require_sentencepiece
+@require_tokenizers
+class TrainerIntegrationPrerunTest(TestCasePlus, TrainerIntegrationCommon):
     """
+    Only tests that want to tap into the auto-pre-run 2 trainings:
+    - self.default_trained_model
+    - self.alternate_trained_model
+    directly, or via check_trained_model
+    """
+
     def setUp(self):
-        self.input = None
-        # 1. define dataset
-        self.dataset_generator = MyDataset()
-        train_dataset = ds.GeneratorDataset(self.dataset_generator, ["data", "label", "length"], shuffle=False)
-        eval_dataset = ds.GeneratorDataset(self.dataset_generator, ["data", "label", "length"], shuffle=False)
-        self.train_dataset = train_dataset.batch(4)
-        self.eval_dataset = eval_dataset.batch(4)
-        # 2. define Models & Loss & Optimizer
-        self.net = MyModel()
-        self.net_2 = MyModel2()
-        self.net.update_parameters_name('net.')
-        self.net_2.update_parameters_name('net_2.')
-
-        self.loss_fn = nn.MSELoss()
-        self.optimizer = nn.Adam(self.net.trainable_params(), learning_rate=0.01)
-        # 3. define callbacks
-        self.timer_callback_epochs = TimerCallback(print_steps=2)
-        self.earlystop_callback = EarlyStopCallback(patience=2)
-        self.bestmodel_callback = BestModelCallback(save_path='save/callback/best_model', auto_load=True)
-        self.checkpoint_callback = CheckpointCallback(save_path='save/callback/ckpt_files', epochs=2,\
-                                                      keep_checkpoint_max=2)
-        self.callbacks = [self.timer_callback_epochs, self.earlystop_callback, self.bestmodel_callback]
-        # 4. define metrics
-        self.metric = Accuracy()
-        # 5. define trainer
-
-
-    def test_pure_trainer(self):
-        """test_pure_trainer"""
-        # 6. trainer run
-        pure_trainer = Trainer(network=self.net, train_dataset=self.train_dataset, eval_dataset=self.eval_dataset,
-                                metrics=self.metric, epochs=2, optimizer=self.optimizer,
-                                loss_fn=self.loss_fn)
-        pure_trainer.run(tgt_columns='label')
-
-
-    def test_trainer_timer(self):
-        """test_trainer_timer"""
-        trainer = Trainer(network=self.net, train_dataset=self.train_dataset, eval_dataset=self.eval_dataset,
-                          metrics=self.metric, epochs=2, optimizer=self.optimizer, loss_fn=self.loss_fn,
-                          callbacks=self.timer_callback_epochs)
-        trainer.run(tgt_columns='label')
-
-
-    def test_trainer_earlystop(self):
-        """test_trainer_earlystop"""
-        trainer = Trainer(network=self.net, train_dataset=self.train_dataset, eval_dataset=self.eval_dataset,
-                          metrics=self.metric, epochs=6, optimizer=self.optimizer, loss_fn=self.loss_fn,
-                          callbacks=self.earlystop_callback)
-        trainer.run(tgt_columns='label')
-
-
-    def test_trainer_bestmodel(self):
-        """test_trainer_bestmodel"""
-        trainer = Trainer(network=self.net, train_dataset=self.train_dataset, eval_dataset=self.eval_dataset,
-                          metrics=self.metric, epochs=4, optimizer=self.optimizer, loss_fn=self.loss_fn,
-                          callbacks=self.bestmodel_callback)
-        trainer.run(tgt_columns='label')
-
-
-    def test_trainer_checkpoint(self):
-        """test_trainer_checkpoint"""
-        trainer = Trainer(network=self.net, train_dataset=self.train_dataset, eval_dataset=self.eval_dataset,
-                          metrics=self.metric, epochs=7, optimizer=self.optimizer, loss_fn=self.loss_fn,
-                          callbacks=self.checkpoint_callback)
-        trainer.run(tgt_columns='label')
-
-
-    def test_different_model(self):
-        """test_different_model"""
-        trainer = Trainer(network=self.net_2, train_dataset=self.train_dataset, eval_dataset=self.eval_dataset,
-                          metrics=self.metric, epochs=2, optimizer=self.optimizer,
-                          loss_fn=self.loss_fn)
-        trainer.run(tgt_columns='length')
-
-
-    def test_no_eval_in_trainer(self):
-        """test_eval_in_trainer"""
-        trainer = Trainer(network=self.net, train_dataset=self.train_dataset, epochs=2,
-                          optimizer=self.optimizer, loss_fn=self.loss_fn)
-        trainer.run(tgt_columns='length')
-
-
-    def test_train_object_netword(self):
-        """test_eval_in_trainer"""
-        net = MyModelWithLoss()
-        trainer = Trainer(network=net, train_dataset=self.train_dataset, epochs=2,
-                          optimizer=self.optimizer)
-        trainer.run()
+        super().setUp()
+        args = TrainingArguments("..")
+        self.n_epochs = args.num_train_epochs
+        self.batch_size = args.train_batch_size
+        trainer = get_regression_trainer(learning_rate=0.1)
+        trainer.train()
+        self.default_trained_model = (trainer.model.a, trainer.model.b)
+
+        trainer = get_regression_trainer(learning_rate=0.1, seed=314)
+        trainer.train()
+        self.alternate_trained_model = (trainer.model.a, trainer.model.b)
+
+    def check_trained_model(self, model, alternate_seed=False):
+        # Checks a training seeded with learning_rate = 0.1
+        (a, b) = self.alternate_trained_model if alternate_seed else self.default_trained_model
+        self.assertTrue(np.allclose(model.a.asnumpy(), a.asnumpy()))
+        self.assertTrue(np.allclose(model.b.asnumpy(), b.asnumpy()))
+
+    def test_reproducible_training(self):
+        # Checks that training worked, model trained and seed made a reproducible training.
+        trainer = get_regression_trainer(learning_rate=0.1)
+        trainer.train()
+        self.check_trained_model(trainer.model)
+
+        # Checks that a different seed gets different (reproducible) results.
+        trainer = get_regression_trainer(learning_rate=0.1, seed=314)
+        trainer.train()
+        self.check_trained_model(trainer.model, alternate_seed=True)
+
+    def test_trainer_with_datasets(self):
+        import datasets
+
+        np.random.seed(42)
+        class MyAccessible:
+            def __init__(self):
+                self._data = np.random.normal(size=(64,)).astype(np.float32)
+                self._label = 2.0 * self._data + 3.0 + np.random.normal(scale=0.1, size=(64,)).astype(np.float32)
+
+            def __getitem__(self, index):
+                return self._data[index], self._label[index]
+
+            def __len__(self):
+                return len(self._data)
+
+        train_dataset = GeneratorDataset(MyAccessible(), column_names=["input_x", "labels"])
+
+        # Base training. Should have the same results as test_reproducible_training
+        model = RegressionModel()
+        args = TrainingArguments("./regression", learning_rate=0.1)
+        trainer = Trainer(model, args, train_dataset=train_dataset)
+        trainer.train()
+        self.check_trained_model(trainer.model)
+
+        # # Can return tensors.
+        # model = RegressionModel()
+        # trainer = Trainer(model, args, train_dataset=train_dataset)
+        # trainer.train()
+        # self.check_trained_model(trainer.model)
+
+        # Adding one column not used by the model should have no impact
+        
+        class MyAccessible:
+            def __init__(self):
+                self._data = np.random.normal(size=(64,)).astype(np.float32)
+                self._label = 2.0 * self._data + 3.0 + np.random.normal(scale=0.1, size=(64,)).astype(np.float32)
+                self._extra = np.random.normal(size=(64,)).astype(np.float32)
+
+            def __getitem__(self, index):
+                return self._data[index], self._label[index], self._extra[index]
+
+            def __len__(self):
+                return len(self._data)
+
+        train_dataset = GeneratorDataset(MyAccessible(), column_names=["input_x", "labels", "extra"])
+        model = RegressionModel()
+        trainer = Trainer(model, args, train_dataset=train_dataset)
+        trainer.train()
+        self.check_trained_model(trainer.model)
+
+    def test_model_init(self):
+        train_dataset = GeneratorDataset(RegressionDataset(), column_names=['input_x', 'labels'])
+
+        args = TrainingArguments("./regression", learning_rate=0.1)
+        trainer = Trainer(args=args, train_dataset=train_dataset, model_init=lambda: RegressionModel())
+        trainer.train()
+        self.check_trained_model(trainer.model)
+
+        # Re-training should restart from scratch, thus lead the same results.
+        trainer.train()
+        self.check_trained_model(trainer.model)
+
+        # Re-training should restart from scratch, thus lead the same results and new seed should be used.
+        trainer.args.seed = 314
+        trainer.train()
+        self.check_trained_model(trainer.model, alternate_seed=True)
+
+    # TODO: support gradient accumulation
+    # def test_gradient_accumulation(self):
+    #     # Training with half the batch size but accumulation steps as 2 should give the same results.
+    #     trainer = get_regression_trainer(
+    #         gradient_accumulation_steps=2, per_device_train_batch_size=4, learning_rate=0.1
+    #     )
+    #     trainer.train()
+    #     self.check_trained_model(trainer.model)
+
+    # def test_gradient_checkpointing(self):
+    #     trainer = get_regression_trainer(
+    #         per_device_train_batch_size=1,
+    #         learning_rate=0.1,
+    #         gradient_checkpointing=True,
+    #         gradient_checkpointing_kwargs={"use_reentrant": False},
+    #     )
+    #     previous_params = {k: v.detach().clone() for k, v in trainer.model.named_parameters()}
+
+    #     trainer.train()
+
+    #     # Check if model weights have been updated
+    #     for k, v in trainer.model.named_parameters():
+    #         self.assertFalse(
+    #             np.allclose(previous_params[k], v, rtol=1e-4, atol=1e-4),
+    #             f"Model weights for {k} have not been updated",
+    #         )
+
+    def test_training_loss(self):
+        # With even logs
+        trainer = get_regression_trainer(logging_steps=8)
+        trainer.train()
+        log_history = trainer.state.log_history
+
+        losses = [log["loss"] for log in log_history if "loss" in log]
+        train_loss = log_history[-1]["train_loss"]
+        self.assertAlmostEqual(sum(losses) / len(losses), train_loss, places=4)
+
+        # With uneven logs
+        trainer = get_regression_trainer(logging_steps=5*8)
+        trainer.train()
+        log_history = trainer.state.log_history
+
+        # Training loss should be the same as before
+        new_train_loss = log_history[-1]["train_loss"]
+        self.assertAlmostEqual(train_loss, new_train_loss, places=4)
+
+    def test_custom_optimizer(self):
+        train_dataset = GeneratorDataset(RegressionDataset(), column_names=['input_x', 'labels'])
+        args = TrainingArguments("./regression")
+        model = RegressionModel()
+        from mindspore.experimental import optim
+
+        optimizer = optim.SGD(model.trainable_params(), lr=1.0)
+        lr_scheduler = optim.lr_scheduler.LambdaLR(optimizer, lr_lambda=lambda x: 1.0)
+        trainer = Trainer(model, args, train_dataset=train_dataset, optimizers=(optimizer, lr_scheduler))
+        trainer.train()
+
+        (a, b) = self.default_trained_model
+        self.assertFalse(np.allclose(trainer.model.a.asnumpy(), a.asnumpy()))
+        self.assertFalse(np.allclose(trainer.model.b.asnumpy(), b.asnumpy()))
+        self.assertEqual(trainer.optimizer.param_groups[0]["lr"], 1.0)
+
+    def test_lr_scheduler_kwargs(self):
+        # test scheduler kwargs passed via TrainingArguments
+        train_dataset = RegressionDataset()
+        model = RegressionModel()
+        num_steps, num_warmup_steps = 10, 2
+        extra_kwargs = {"power": 5.0, "lr_end": 1e-5}  # Non-default arguments
+        args = TrainingArguments(
+            "./regression",
+            lr_scheduler_type="polynomial",
+            lr_scheduler_kwargs=extra_kwargs,
+            learning_rate=0.2,
+            warmup_steps=num_warmup_steps,
+        )
+        trainer = Trainer(model, args, train_dataset=train_dataset)
+        trainer.create_optimizer_and_scheduler(num_training_steps=num_steps)
+
+        # Checking that the scheduler was created
+        self.assertIsNotNone(trainer.lr_scheduler)
+
+        # Checking that the correct args were passed
+        sched1 = trainer.lr_scheduler
+        sched2 = get_polynomial_decay_schedule_with_warmup(
+            trainer.optimizer, num_warmup_steps=num_warmup_steps, num_training_steps=num_steps, **extra_kwargs
+        )
+        self.assertEqual(sched1.lr_lambdas[0].args, sched2.lr_lambdas[0].args)
+        self.assertEqual(sched1.lr_lambdas[0].keywords, sched2.lr_lambdas[0].keywords)
+
+    def test_reduce_lr_on_plateau_args(self):
+        # test passed arguments for a custom ReduceLROnPlateau scheduler
+        train_dataset = GeneratorDataset(RegressionDataset(length=64), column_names=['input_x', 'labels'])
+        eval_dataset = GeneratorDataset(RegressionDataset(length=64), column_names=['input_x', 'labels'])
+
+        args = TrainingArguments(
+            "./regression",
+            evaluation_strategy="epoch",
+            metric_for_best_model="eval_loss",
+        )
+        model = RegressionModel()
+        optimizer = mindspore.experimental.optim.SGD(model.trainable_params(), lr=1.0)
+        lr_scheduler = mindspore.experimental.optim.lr_scheduler.ReduceLROnPlateau(optimizer, factor=0.2, patience=5, cooldown=2)
+        trainer = Trainer(
+            model, args, train_dataset=train_dataset, eval_dataset=eval_dataset, optimizers=(optimizer, lr_scheduler)
+        )
+        trainer.train()
+
+        self.assertIsInstance(trainer.lr_scheduler, mindspore.experimental.optim.lr_scheduler.ReduceLROnPlateau)
+        self.assertEqual(trainer.lr_scheduler.factor, 0.2)
+        self.assertEqual(trainer.lr_scheduler.patience, 5)
+        self.assertEqual(trainer.lr_scheduler.cooldown, 2)
+
+    def test_reduce_lr_on_plateau(self):
+        # test the ReduceLROnPlateau scheduler
+
+        class TrainerWithLRLogs(Trainer):
+            def log(self, logs):
+                # the LR is computed after metrics and does not exist for the first epoch
+                if hasattr(self.lr_scheduler, "_last_lr"):
+                    logs["learning_rate"] = self.lr_scheduler._last_lr[0]
+                super().log(logs)
+
+        train_dataset = GeneratorDataset(RegressionDataset(length=64), column_names=['input_x', 'labels'])
+        eval_dataset = GeneratorDataset(RegressionDataset(length=64), column_names=['input_x', 'labels'])
+
+        args = TrainingArguments(
+            "./regression",
+            lr_scheduler_type="reduce_lr_on_plateau",
+            evaluation_strategy="epoch",
+            metric_for_best_model="eval_loss",
+            num_train_epochs=10,
+            learning_rate=0.2,
+        )
+        model = RegressionModel()
+        trainer = TrainerWithLRLogs(model, args, train_dataset=train_dataset, eval_dataset=eval_dataset)
+        trainer.train()
+
+        self.assertIsInstance(trainer.lr_scheduler, mindspore.experimental.optim.lr_scheduler.ReduceLROnPlateau)
+        patience = trainer.lr_scheduler.patience
+
+        logs = trainer.state.log_history[1:]
+        best_loss = logs[0]["eval_loss"]
+        bad_epochs = 0
+        for i, log in enumerate(logs[:-1]):  # Compare learning rate to next epoch's
+            loss = log["eval_loss"]
+            just_decreased = False
+            if loss > best_loss:
+                bad_epochs += 1
+                if bad_epochs > patience:
+                    self.assertLess(logs[i + 1]["learning_rate"], log["learning_rate"])
+                    just_decreased = True
+                    bad_epochs = 0
+            else:
+                best_loss = loss
+                bad_epochs = 0
+            if not just_decreased:
+                self.assertEqual(logs[i + 1]["learning_rate"], log["learning_rate"])
+
+    # def test_adafactor_lr_none(self):
+    #     # test the special case where lr=None, since Trainer can't not have lr_scheduler
+    #     from mindspore.nn import AdaFactor
+    #     # from transformers.optimization import Adafactor, AdafactorSchedule
+
+    #     train_dataset = RegressionDataset()
+    #     args = TrainingArguments("./regression")
+    #     model = RegressionModel()
+    #     optimizer = AdaFactor(model.trainable_params(), scale_parameter=True, relative_step=True, warmup_init=True, lr=None)
+    #     lr_scheduler = AdafactorSchedule(optimizer)
+    #     trainer = Trainer(model, args, train_dataset=train_dataset, optimizers=(optimizer, lr_scheduler))
+    #     trainer.train()
+
+    #     (a, b) = self.default_trained_model
+    #     self.assertFalse(np.allclose(trainer.model.a, a))
+    #     self.assertFalse(np.allclose(trainer.model.b, b))
+    #     self.assertGreater(trainer.optimizer.state_dict()["param_groups"][0]["lr"], 0)
+
+    # TODO: support bf16
+    # def test_mixed_bf16(self):
+    #     # very basic test
+    #     trainer = get_regression_trainer(learning_rate=0.1, bf16=True)
+    #     trainer.train()
+    #     self.check_trained_model(trainer.model)
+
+    #     # --bf16 --half_precision_backend apex can't be used together
+    #     with self.assertRaises(ValueError):
+    #         trainer = get_regression_trainer(learning_rate=0.1, bf16=True, half_precision_backend="apex")
+
+    #     # will add more specific tests once there are some bugs to fix
+
+
+@require_mindspore
+@require_sentencepiece
+@require_tokenizers
+class TrainerIntegrationTest(TestCasePlus, TrainerIntegrationCommon):
+    def setUp(self):
+        super().setUp()
+        args = TrainingArguments("..")
+        self.n_epochs = args.num_train_epochs
+        self.batch_size = args.train_batch_size
+
+    def test_trainer_works_with_dict(self):
+        # Edge case because Apex with mode O2 will change our models to return dicts. This test checks it doesn't break
+        # anything.
+        train_dataset = GeneratorDataset(RegressionDataset(), column_names=['input_x', 'labels'])
+        eval_dataset = GeneratorDataset(RegressionDataset(), column_names=['input_x', 'labels'])
+        model = RegressionDictModel()
+        args = TrainingArguments("./regression")
+        trainer = Trainer(model, args, train_dataset=train_dataset, eval_dataset=eval_dataset)
+        trainer.train()
+        _ = trainer.evaluate()
+        _ = trainer.predict(GeneratorDataset(RegressionDataset(), column_names=['input_x', 'labels']))
+
+    def test_evaluation_with_keys_to_drop(self):
+        config = GPT2Config(vocab_size=100, n_positions=128, n_embd=32, n_layer=3, n_head=4)
+        tiny_gpt2 = GPT2LMHeadModel(config)
+        x = ops.randint(0, 100, (128,))
+        eval_dataset = GeneratorDataset(RepeatDataset(x), column_names=['input_ids', 'labels'])
+        args = TrainingArguments("./test")
+        trainer = Trainer(tiny_gpt2, args, eval_dataset=eval_dataset)
+        # By default the past_key_values are removed
+        result = trainer.predict(eval_dataset)
+        self.assertTrue(isinstance(result.predictions, np.ndarray))
+        # We can still get them by setting ignore_keys to []
+        result = trainer.predict(eval_dataset, ignore_keys=[])
+        self.assertTrue(isinstance(result.predictions, tuple))
+        self.assertEqual(len(result.predictions), 2)
+
+    def test_training_arguments_are_left_untouched(self):
+        trainer = get_regression_trainer()
+        trainer.train()
+        args = TrainingArguments("./regression")
+        dict1, dict2 = args.to_dict(), trainer.args.to_dict()
+        for key in dict1.keys():
+            # Logging dir can be slightly different as they default to something with the time.
+            if key != "logging_dir":
+                self.assertEqual(dict1[key], dict2[key])
+
+    def test_number_of_steps_in_training(self):
+        # Regular training has n_epochs * len(train_dl) steps
+        trainer = get_regression_trainer(learning_rate=0.1)
+        train_output = trainer.train()
+        self.assertEqual(train_output.global_step, self.n_epochs * 64 / self.batch_size)
+
+        # Check passing num_train_epochs works (and a float version too):
+        trainer = get_regression_trainer(learning_rate=0.1, num_train_epochs=1.5)
+        train_output = trainer.train()
+        self.assertEqual(train_output.global_step, int(1.5 * 64 / self.batch_size))
+
+        # If we pass a max_steps, num_train_epochs is ignored
+        trainer = get_regression_trainer(learning_rate=0.1, max_steps=10)
+        train_output = trainer.train()
+        self.assertEqual(train_output.global_step, 10)
+
+    def test_neftune(self):
+        config = GPT2Config(vocab_size=100, n_positions=128, n_embd=32, n_layer=3, n_head=4)
+        tiny_gpt2 = GPT2LMHeadModel(config)
+        x = np.random.randint(0, 100, (128,))
+        train_dataset = GeneratorDataset(RepeatDataset(x), column_names=['input_ids', 'labels'])
+
+        # Trainer without inf/nan filter
+        args = TrainingArguments(
+            "./test", learning_rate=1e-9, logging_steps=5, logging_nan_inf_filter=False, neftune_noise_alpha=0.4
+        )
+        trainer = Trainer(tiny_gpt2, args, train_dataset=train_dataset)
+
+        trainer.model = trainer._activate_neftune(trainer.model)
+
+        dummy_input = mindspore.Tensor([[1, 0, 1]])
+        emb1 = trainer.model.get_input_embeddings()(dummy_input)
+        emb2 = trainer.model.get_input_embeddings()(dummy_input)
+
+        self.assertFalse(np.allclose(emb1.asnumpy(), emb2.asnumpy()), "Neftune noise is not applied!")
+
+        # redefine the model
+        tiny_gpt2 = GPT2LMHeadModel(config)
+        # Trainer without inf/nan filter
+        args = TrainingArguments(
+            "./test", learning_rate=1e-9, logging_steps=5, logging_nan_inf_filter=False, neftune_noise_alpha=0.4
+        )
+        trainer = Trainer(tiny_gpt2, args, train_dataset=train_dataset)
+
+        # Check that it trains without errors
+        trainer.train()
+
+        # Make sure forward pass works fine
+        _ = trainer.model(dummy_input)
+        self.assertTrue(len(trainer.model.get_input_embeddings()._forward_hook) == 0)
+
+        trainer.model.set_train(False)
+
+        # Check that we get identical embeddings just in case
+        emb1 = trainer.model.get_input_embeddings()(dummy_input)
+        emb2 = trainer.model.get_input_embeddings()(dummy_input)
+
+        self.assertTrue(np.allclose(emb1.asnumpy(), emb2.asnumpy()), "Neftune noise is still applied!")
+
+    def test_logging_inf_nan_filter(self):
+        config = GPT2Config(vocab_size=100, n_positions=128, n_embd=32, n_layer=3, n_head=4)
+        tiny_gpt2 = GPT2LMHeadModel(config)
+        x = ops.randint(0, 100, (128,))
+        train_dataset = GeneratorDataset(RepeatDataset(x), column_names=['input_ids', 'labels'])
+
+        # Trainer without inf/nan filter
+        args = TrainingArguments("./test", learning_rate=1e9, logging_steps=5, logging_nan_inf_filter=False)
+        trainer = Trainer(tiny_gpt2, args, train_dataset=train_dataset)
+        trainer.train()
+        log_history_no_filter = trainer.state.log_history
+
+        # Trainer with inf/nan filter
+        args = TrainingArguments("./test", learning_rate=1e9, logging_steps=5, logging_nan_inf_filter=True)
+        trainer = Trainer(tiny_gpt2, args, train_dataset=train_dataset)
+        trainer.train()
+        log_history_filter = trainer.state.log_history
+
+        def is_any_loss_nan_or_inf(log_history):
+            losses = [l["loss"] for l in log_history[:-1]]
+            return any(math.isnan(x) for x in losses) or any(math.isinf(x) for x in losses)
+
+        self.assertTrue(is_any_loss_nan_or_inf(log_history_no_filter))
+        self.assertFalse(is_any_loss_nan_or_inf(log_history_filter))
+
+    def test_train_and_eval_dataloaders(self):
+        n_gpu = 1
+        trainer = get_regression_trainer(learning_rate=0.1, per_device_train_batch_size=16)
+        self.assertEqual(trainer.get_train_dataset().get_batch_size(), 16 * n_gpu)
+        trainer = get_regression_trainer(learning_rate=0.1, per_device_eval_batch_size=16)
+        self.assertEqual(trainer.get_eval_dataset().get_batch_size(), 16 * n_gpu)
+
+        # Check drop_last works
+        trainer = get_regression_trainer(
+            train_len=66, eval_len=74, learning_rate=0.1, per_device_train_batch_size=16, per_device_eval_batch_size=32
+        )
+        self.assertEqual(len(trainer.get_train_dataset()), 66 // (16 * n_gpu) + 1)
+        self.assertEqual(len(trainer.get_eval_dataset()), 74 // (32 * n_gpu) + 1)
+
+        trainer = get_regression_trainer(
+            train_len=66,
+            eval_len=74,
+            learning_rate=0.1,
+            per_device_train_batch_size=16,
+            per_device_eval_batch_size=32,
+            dataset_drop_last=True,
+        )
+        self.assertEqual(len(trainer.get_train_dataset()), 66 // (16 * n_gpu))
+        self.assertEqual(len(trainer.get_eval_dataset()), 74 // (32 * n_gpu))
+
+        # Check passing a new dataset for evaluation works
+        new_eval_dataset = GeneratorDataset(RegressionDataset(length=128), column_names=['input_x', 'labels'])
+        self.assertEqual(len(trainer.get_eval_dataset(new_eval_dataset)), 128 // (32 * n_gpu))
+
+    # tests that we do not require mindspore.dataset.Dataset
+    def test_data_without_dataset(self):
+        pass
+
+    def test_evaluate(self):
+        trainer = get_regression_trainer(a=1.5, b=2.5, compute_metrics=AlmostAccuracy())
+        results = trainer.evaluate()
+
+        x, y = trainer.eval_dataset.source.x, trainer.eval_dataset.source.ys[0]
+        pred = 1.5 * x + 2.5
+        expected_loss = ((pred - y) ** 2).mean()
+        self.assertAlmostEqual(results["eval_loss"], expected_loss)
+        expected_acc = AlmostAccuracy()((pred, y))["accuracy"]
+        self.assertAlmostEqual(results["eval_accuracy"], expected_acc)
+
+        # With a number of elements not a round multiple of the batch size
+        trainer = get_regression_trainer(a=1.5, b=2.5, eval_len=66, compute_metrics=AlmostAccuracy())
+        results = trainer.evaluate()
+
+        x, y = trainer.eval_dataset.source.x, trainer.eval_dataset.source.ys[0]
+        pred = 1.5 * x + 2.5
+        expected_loss = ((pred - y) ** 2).mean()
+        self.assertAlmostEqual(results["eval_loss"], expected_loss)
+        expected_acc = AlmostAccuracy()((pred, y))["accuracy"]
+        self.assertAlmostEqual(results["eval_accuracy"], expected_acc)
+
+        # With logits preprocess
+        trainer = get_regression_trainer(
+            a=1.5,
+            b=2.5,
+            compute_metrics=AlmostAccuracy(),
+            preprocess_logits_for_metrics=lambda logits, labels: logits + 1,
+        )
+        results = trainer.evaluate()
+
+        x, y = trainer.eval_dataset.source.x, trainer.eval_dataset.source.ys[0]
+        pred = 1.5 * x + 2.5
+        expected_loss = ((pred - y) ** 2).mean()
+        self.assertAlmostEqual(results["eval_loss"], expected_loss)
+        expected_acc = AlmostAccuracy()((pred + 1, y))["accuracy"]
+        self.assertAlmostEqual(results["eval_accuracy"], expected_acc)
+
+    def test_evaluate_with_jit(self):
+        trainer = get_regression_trainer(a=1.5, b=2.5, compute_metrics=AlmostAccuracy(), jit_mode_eval=True)
+        results = trainer.evaluate()
+
+        x, y = trainer.eval_dataset.source.x, trainer.eval_dataset.source.ys[0]
+        pred = 1.5 * x + 2.5
+        expected_loss = ((pred - y) ** 2).mean()
+        self.assertAlmostEqual(results["eval_loss"], expected_loss)
+        expected_acc = AlmostAccuracy()((pred, y))["accuracy"]
+        self.assertAlmostEqual(results["eval_accuracy"], expected_acc)
+
+        # With a number of elements not a round multiple of the batch size
+        trainer = get_regression_trainer(
+            a=1.5, b=2.5, eval_len=66, compute_metrics=AlmostAccuracy(), jit_mode_eval=True
+        )
+        results = trainer.evaluate()
+
+        x, y = trainer.eval_dataset.source.x, trainer.eval_dataset.source.ys[0]
+        pred = 1.5 * x + 2.5
+        expected_loss = ((pred - y) ** 2).mean()
+        self.assertAlmostEqual(results["eval_loss"], expected_loss)
+        expected_acc = AlmostAccuracy()((pred, y))["accuracy"]
+        self.assertAlmostEqual(results["eval_accuracy"], expected_acc)
+
+        # With logits preprocess
+        trainer = get_regression_trainer(
+            a=1.5,
+            b=2.5,
+            compute_metrics=AlmostAccuracy(),
+            preprocess_logits_for_metrics=lambda logits, labels: logits + 1,
+            jit_mode_eval=True,
+        )
+        results = trainer.evaluate()
+
+        x, y = trainer.eval_dataset.source.x, trainer.eval_dataset.source.ys[0]
+        pred = 1.5 * x + 2.5
+        expected_loss = ((pred - y) ** 2).mean()
+        self.assertAlmostEqual(results["eval_loss"], expected_loss)
+        expected_acc = AlmostAccuracy()((pred + 1, y))["accuracy"]
+        self.assertAlmostEqual(results["eval_accuracy"], expected_acc)
+
+    def test_predict(self):
+        trainer = get_regression_trainer(a=1.5, b=2.5)
+        preds = trainer.predict(trainer.eval_dataset).predictions
+        x = trainer.eval_dataset.source.x
+        print(preds, 1.5 * x + 2.5)
+        self.assertTrue(np.allclose(preds, 1.5 * x + 2.5))
+
+        # With a number of elements not a round multiple of the batch size
+        trainer = get_regression_trainer(a=1.5, b=2.5, eval_len=66)
+        preds = trainer.predict(trainer.eval_dataset).predictions
+        x = trainer.eval_dataset.source.x
+        self.assertTrue(np.allclose(preds, 1.5 * x + 2.5))
+
+        # With more than one output of the model
+        trainer = get_regression_trainer(a=1.5, b=2.5, double_output=True)
+        preds = trainer.predict(trainer.eval_dataset).predictions
+        x = trainer.eval_dataset.source.x
+        self.assertEqual(len(preds), 2)
+        self.assertTrue(np.allclose(preds[0], 1.5 * x + 2.5))
+        self.assertTrue(np.allclose(preds[1], 1.5 * x + 2.5))
+
+        # With more than one output/label of the model
+        trainer = get_regression_trainer(a=1.5, b=2.5, double_output=True, label_names=["labels", "labels_2"])
+        outputs = trainer.predict(trainer.eval_dataset)
+        preds = outputs.predictions
+        labels = outputs.label_ids
+        x = trainer.eval_dataset.source.x
+        self.assertEqual(len(preds), 2)
+        self.assertTrue(np.allclose(preds[0], 1.5 * x + 2.5))
+        self.assertTrue(np.allclose(preds[1], 1.5 * x + 2.5))
+        self.assertTrue(np.array_equal(labels[0], trainer.eval_dataset.source.ys[0]))
+        self.assertTrue(np.array_equal(labels[1], trainer.eval_dataset.source.ys[1]))
+
+    def test_predict_with_jit(self):
+        trainer = get_regression_trainer(a=1.5, b=2.5, jit_mode_eval=True)
+        preds = trainer.predict(trainer.eval_dataset).predictions
+        x = trainer.eval_dataset.source.x
+        self.assertTrue(np.allclose(preds, 1.5 * x + 2.5))
+
+        # With a number of elements not a round multiple of the batch size
+        trainer = get_regression_trainer(a=1.5, b=2.5, eval_len=66, jit_mode_eval=True)
+        preds = trainer.predict(trainer.eval_dataset).predictions
+        x = trainer.eval_dataset.source.x
+        self.assertTrue(np.allclose(preds, 1.5 * x + 2.5))
+
+        # With more than one output of the model
+        trainer = get_regression_trainer(a=1.5, b=2.5, double_output=True, jit_mode_eval=True)
+        preds = trainer.predict(trainer.eval_dataset).predictions
+        x = trainer.eval_dataset.source.x
+        self.assertEqual(len(preds), 2)
+        self.assertTrue(np.allclose(preds[0], 1.5 * x + 2.5))
+        self.assertTrue(np.allclose(preds[1], 1.5 * x + 2.5))
+
+        # With more than one output/label of the model
+        trainer = get_regression_trainer(
+            a=1.5, b=2.5, double_output=True, label_names=["labels", "labels_2"], jit_mode_eval=True
+        )
+        outputs = trainer.predict(trainer.eval_dataset)
+        preds = outputs.predictions
+        labels = outputs.label_ids
+        x = trainer.eval_dataset.source.x
+        self.assertEqual(len(preds), 2)
+        self.assertTrue(np.allclose(preds[0], 1.5 * x + 2.5))
+        self.assertTrue(np.allclose(preds[1], 1.5 * x + 2.5))
+        self.assertTrue(np.array_equal(labels[0], trainer.eval_dataset.source.ys[0]))
+        self.assertTrue(np.array_equal(labels[1], trainer.eval_dataset.source.ys[1]))
+
+    @pytest.mark.skip('not support dynamic shape')
+    def test_dynamic_shapes(self):
+        eval_dataset = GeneratorDataset(DynamicShapesDataset(batch_size=self.batch_size), column_names=['input_x', 'labels'])
+        model = RegressionModel(a=2, b=1)
+        args = TrainingArguments("./regression")
+        trainer = Trainer(model, args, eval_dataset=eval_dataset)
+
+        # Check evaluation can run to completion
+        _ = trainer.evaluate()
+
+        # Check predictions
+        preds = trainer.predict(eval_dataset)
+        for expected, seen in zip(eval_dataset.ys, preds.label_ids):
+            self.assertTrue(np.array_equal(expected, seen[: expected.shape[0]]))
+            self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
+
+        for expected, seen in zip(eval_dataset.xs, preds.predictions):
+            self.assertTrue(np.array_equal(2 * expected + 1, seen[: expected.shape[0]]))
+            self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
+
+        # Same tests with eval accumulation
+        args = TrainingArguments("./regression", eval_accumulation_steps=2)
+        trainer = Trainer(model, args, eval_dataset=eval_dataset)
+
+        # Check evaluation can run to completion
+        _ = trainer.evaluate()
+
+        # Check predictions
+        preds = trainer.predict(eval_dataset)
+        for expected, seen in zip(eval_dataset.ys, preds.label_ids):
+            self.assertTrue(np.array_equal(expected, seen[: expected.shape[0]]))
+            self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
+
+        for expected, seen in zip(eval_dataset.xs, preds.predictions):
+            self.assertTrue(np.array_equal(2 * expected + 1, seen[: expected.shape[0]]))
+            self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
+
+    def test_log_level(self):
+        # testing only --log_level (--log_level_replica requires multiple gpus and DDP and is tested elsewhere)
+        logger = logging.get_logger()
+        log_info_string = "Running training"
+
+        # test with the default log_level - should be the same as before and thus we test depending on is_info
+        is_info = logging.get_verbosity() <= 20
+        with CaptureLogger(logger) as cl:
+            trainer = get_regression_trainer()
+            trainer.train()
+        if is_info:
+            self.assertIn(log_info_string, cl.out)
+        else:
+            self.assertNotIn(log_info_string, cl.out)
+
+        with LoggingLevel(logging.INFO):
+            # test with low log_level - lower than info
+            with CaptureLogger(logger) as cl:
+                trainer = get_regression_trainer(log_level="debug")
+                trainer.train()
+            self.assertIn(log_info_string, cl.out)
+
+        with LoggingLevel(logging.INFO):
+            # test with high log_level - should be quiet
+            with CaptureLogger(logger) as cl:
+                trainer = get_regression_trainer(log_level="error")
+                trainer.train()
+            self.assertNotIn(log_info_string, cl.out)
+
+    def test_save_checkpoints(self):
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(output_dir=tmpdir, save_steps=5)
+            trainer.train()
+            self.check_saved_checkpoints(tmpdir, 5, int(self.n_epochs * 64 / self.batch_size))
+
+        # With a regular model that is not a PreTrainedModel
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(output_dir=tmpdir, save_steps=5, pretrained=False)
+            trainer.train()
+            self.check_saved_checkpoints(tmpdir, 5, int(self.n_epochs * 64 / self.batch_size), False)
+
+    def test_save_checkpoints_is_atomic(self):
+        class UnsaveableTokenizer(PreTrainedTokenizerBase):
+            def save_pretrained(self, *args, **kwargs):
+                raise OSError("simulated file write error")
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(output_dir=tmpdir, save_steps=5)
+            # Attach unsaveable tokenizer to partially fail checkpointing
+            trainer.tokenizer = UnsaveableTokenizer()
+            with self.assertRaises(OSError) as _context:
+                trainer.train()
+            # assert get_last_checkpoint(tmpdir) is None
+
+    @require_safetensors
+    def test_safe_checkpoints(self):
+        for save_safetensors in [True, False]:
+            with tempfile.TemporaryDirectory() as tmpdir:
+                trainer = get_regression_trainer(output_dir=tmpdir, save_steps=5, save_safetensors=save_safetensors)
+                trainer.train()
+                self.check_saved_checkpoints(
+                    tmpdir, 5, int(self.n_epochs * 64 / self.batch_size), safe_weights=save_safetensors
+                )
+
+            # With a regular model that is not a PreTrainedModel
+            with tempfile.TemporaryDirectory() as tmpdir:
+                trainer = get_regression_trainer(
+                    output_dir=tmpdir, save_steps=5, pretrained=False, save_safetensors=save_safetensors
+                )
+                trainer.train()
+                self.check_saved_checkpoints(
+                    tmpdir, 5, int(self.n_epochs * 64 / self.batch_size), False, safe_weights=save_safetensors
+                )
+
+    def test_run_seq2seq_double_train_wrap_once(self):
+        # test that we don't wrap the model more than once
+        # since wrapping primarily happens on multi-gpu setup we want multiple gpus to test for
+        # example DataParallel(DataParallel(model))
+
+        trainer = get_regression_trainer()
+        trainer.train()
+        model_wrapped_before = trainer.model
+        trainer.train()
+        model_wrapped_after = trainer.model
+        self.assertIs(model_wrapped_before, model_wrapped_after, "should be not wrapped twice")
+
+    def test_can_resume_training(self):
+        # This test will fail for more than 2 GPUs since the batch size will get bigger and with the number of
+        # save_steps, the checkpoint will resume training at epoch 2 or more (so the data seen by the model
+        # won't be the same since the training dataloader is shuffled).
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            kwargs = {
+                "output_dir": tmpdir,
+                "train_len": 128,
+                "save_steps": 16,
+                "learning_rate": 0.1,
+                "logging_steps": 16,
+            }
+            trainer = get_regression_trainer(**kwargs)
+            trainer.train()
+            (a, b) = trainer.model.a.item(), trainer.model.b.item()
+            state = dataclasses.asdict(trainer.state)
+
+            checkpoint = os.path.join(tmpdir, "checkpoint-16")
+
+            # Reinitialize trainer
+            trainer = get_regression_trainer(**kwargs)
+
+            trainer.train(resume_from_checkpoint=checkpoint)
+            (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+            state1 = dataclasses.asdict(trainer.state)
+            self.assertEqual(a, a1)
+            self.assertEqual(b, b1)
+            self.check_trainer_state_are_the_same(state, state1)
+
+            # Now check with a later checkpoint that it also works when we span over one epoch
+            checkpoint = os.path.join(tmpdir, "checkpoint-48")
+
+            # Reinitialize trainer and load model
+            trainer = get_regression_trainer(**kwargs)
+
+            trainer.train(resume_from_checkpoint=checkpoint)
+            (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+            state1 = dataclasses.asdict(trainer.state)
+            self.assertEqual(a, a1)
+            self.assertEqual(b, b1)
+            self.check_trainer_state_are_the_same(state, state1)
+
+        # With a regular model that is not a PreTrainedModel
+        with tempfile.TemporaryDirectory() as tmpdir:
+            kwargs = {
+                "output_dir": tmpdir,
+                "train_len": 128,
+                "save_steps": 16,
+                "learning_rate": 0.1,
+                "pretrained": False,
+            }
+
+            trainer = get_regression_trainer(**kwargs)
+            trainer.train()
+            (a, b) = trainer.model.a.item(), trainer.model.b.item()
+            state = dataclasses.asdict(trainer.state)
+
+            checkpoint = os.path.join(tmpdir, "checkpoint-16")
+
+            # Reinitialize trainer and load model
+            trainer = get_regression_trainer(**kwargs)
+
+            trainer.train(resume_from_checkpoint=checkpoint)
+            (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+            state1 = dataclasses.asdict(trainer.state)
+            self.assertEqual(a, a1)
+            self.assertEqual(b, b1)
+            self.check_trainer_state_are_the_same(state, state1)
+
+            # Now check with a later checkpoint that it also works when we span over one epoch
+            checkpoint = os.path.join(tmpdir, "checkpoint-48")
+
+            # Reinitialize trainer and load model
+            trainer = get_regression_trainer(**kwargs)
+
+            trainer.train(resume_from_checkpoint=checkpoint)
+            (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+            state1 = dataclasses.asdict(trainer.state)
+            self.assertEqual(a, a1)
+            self.assertEqual(b, b1)
+            self.check_trainer_state_are_the_same(state, state1)
+
+        # Now check failures
+
+        # 1. fail to find a bogus checkpoint
+        trainer = get_regression_trainer()
+        with self.assertRaises(Exception) as context:
+            trainer.train(resume_from_checkpoint=f"{checkpoint}-bogus")
+        self.assertTrue("Can't find a valid checkpoint at" in str(context.exception))
+
+        # 2. fail to find any checkpoint - due a fresh output_dir
+        output_dir2 = self.get_auto_remove_tmp_dir()
+        trainer = get_regression_trainer(output_dir=output_dir2)
+        with self.assertRaises(Exception) as context:
+            trainer.train(resume_from_checkpoint=True)
+        self.assertTrue("No valid checkpoint found in output directory" in str(context.exception))
+
+    @unittest.skip(
+        reason="@muellerzr: Fix once Trainer can take an accelerate configuration. Need to set `seedable_sampler=True`."
+    )
+    def test_resume_training_with_randomness(self):
+        # For more than 1 GPUs, since the randomness is introduced in the model and with DataParallel (which is used
+        # in this test for more than 2 GPUs), the calls to the torch RNG will happen in a random order (sometimes
+        # GPU 0 will call first and sometimes GPU 1).
+        train_dataset = RegressionDataset(length=128)
+        eval_dataset = RegressionDataset()
+
+        with self.subTest("Test every step"):
+            config = RegressionModelConfig(a=0, b=2, random_ms=random_ms)
+            model = RegressionRandomPreTrainedModel(config)
+
+            tmp_dir = self.get_auto_remove_tmp_dir()
+            args = RegressionTrainingArguments(tmp_dir, save_steps=5, learning_rate=0.1)
+            trainer = Trainer(model, args, train_dataset=train_dataset, eval_dataset=eval_dataset)
+
+            trainer.train()
+            (a, b) = trainer.model.a.item(), trainer.model.b.item()
+
+            model = RegressionRandomPreTrainedModel(config)
+            trainer = Trainer(model, args, train_dataset=train_dataset, eval_dataset=eval_dataset)
+            trainer.train(resume_from_checkpoint=os.path.join(tmp_dir, "checkpoint-15"))
+            (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+
+            self.assertAlmostEqual(a, a1, delta=1e-5)
+            self.assertAlmostEqual(b, b1, delta=1e-5)
+
+        with self.subTest("Test every epoch"):
+            config = RegressionModelConfig(a=0, b=2)
+            model = RegressionRandomPreTrainedModel(config)
+
+            tmp_dir = self.get_auto_remove_tmp_dir()
+            args = RegressionTrainingArguments(tmp_dir, save_strategy="epoch", learning_rate=0.1)
+            trainer = Trainer(model, args, train_dataset=train_dataset, eval_dataset=eval_dataset)
+
+            trainer.train()
+            (a, b) = trainer.model.a.item(), trainer.model.b.item()
+
+            model = RegressionRandomPreTrainedModel(config)
+            trainer = Trainer(model, args, train_dataset=train_dataset, eval_dataset=eval_dataset)
+
+            checkpoints = [d for d in os.listdir(tmp_dir) if d.startswith("checkpoint-")]
+            # There should be one checkpoint per epoch.
+            self.assertEqual(len(checkpoints), 3)
+            checkpoint_dir = sorted(checkpoints, key=lambda x: int(x.replace("checkpoint-", "")))[0]
+
+            trainer.train(resume_from_checkpoint=os.path.join(tmp_dir, checkpoint_dir))
+            (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+
+            self.assertAlmostEqual(a, a1, delta=1e-5)
+            self.assertAlmostEqual(b, b1, delta=1e-5)
+
+    @slow
+    def test_auto_batch_size_finder(self):
+        SRC_DIR = os.path.abspath(
+            os.path.join(os.path.dirname(__file__), "..", "..", "examples", "pytorch", "text-classification")
+        )
+        sys.path.append(SRC_DIR)
+        import run_glue
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            testargs = f"""
+                run_glue.py
+                --model_name_or_path distilbert/distilbert-base-uncased
+                --task_name mrpc
+                --do_train
+                --do_eval
+                --max_seq_len 128
+                --per_device_train_batch_size 4096
+                --learning_rate 2e-5
+                --num_train_epochs 1
+                --output_dir {tmpdir}
+                --auto_find_batch_size 0
+                """.split()
+            with self.assertRaises(RuntimeError):
+                with patch.object(sys, "argv", testargs):
+                    run_glue.main()
+
+        testargs[-1] = "1"
+        with patch.object(sys, "argv", testargs):
+            run_glue.main()
+
+    @pytest.mark.skip('not support auto batch size now')
+    def test_auto_batch_size_with_resume_from_checkpoint(self):
+        train_dataset = GeneratorDataset(RegressionDataset(length=128), column_names=['input_x', 'labels'])
+
+        config = RegressionModelConfig(a=0, b=2)
+        model = RegressionRandomPreTrainedModel(config)
+
+        tmp_dir = self.get_auto_remove_tmp_dir()
+
+        class MockCudaOOMCallback(TrainerCallback):
+            def on_step_end(self, args, state, control, **kwargs):
+                # simulate OOM on the first step
+                if state.train_batch_size >= 16:
+                    raise RuntimeError("CUDA out of memory.")
+
+        args = RegressionTrainingArguments(
+            tmp_dir,
+            do_train=True,
+            max_steps=2,
+            save_steps=1,
+            per_device_train_batch_size=16,
+            auto_find_batch_size=True,
+        )
+        trainer = Trainer(model, args, train_dataset=train_dataset, callbacks=[MockCudaOOMCallback()])
+        trainer.train()
+        # After `auto_find_batch_size` is ran we should now be at 8
+        self.assertEqual(trainer._train_batch_size, 8)
+
+        # We can then make a new Trainer
+        trainer = Trainer(model, args, train_dataset=train_dataset)
+        # Check we are at 16 to start
+        self.assertEqual(trainer._train_batch_size, 16 * max(trainer.args.n_gpu, 1))
+        trainer.train(resume_from_checkpoint=True)
+        # We should be back to 8 again, picking up based upon the last ran Trainer
+        self.assertEqual(trainer._train_batch_size, 8)
+
+    # regression for this issue: https://github.com/huggingface/transformers/issues/12970
+    def test_training_with_resume_from_checkpoint_false(self):
+        train_dataset = GeneratorDataset(RegressionDataset(length=128), column_names=['input_x', 'labels'])
+        eval_dataset = GeneratorDataset(RegressionDataset(), column_names=['input_x', 'labels'])
+
+        config = RegressionModelConfig(a=0, b=2)
+        model = RegressionRandomPreTrainedModel(config)
+
+        tmp_dir = self.get_auto_remove_tmp_dir()
+        args = RegressionTrainingArguments(tmp_dir, save_steps=5, learning_rate=0.1)
+        trainer = Trainer(model, args, train_dataset=train_dataset, eval_dataset=eval_dataset)
+
+        trainer.train(resume_from_checkpoint=False)
+
+    def test_resume_training_with_shard_checkpoint(self):
+        # This test will fail for more than 2 GPUs since the batch size will get bigger and with the number of
+        # save_steps, the checkpoint will resume training at epoch 2 or more (so the data seen by the model
+        # won't be the same since the training dataloader is shuffled).
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(output_dir=tmpdir, train_len=128, save_steps=16, learning_rate=0.1)
+            trainer.train()
+            (a, b) = trainer.model.a.item(), trainer.model.b.item()
+            state = dataclasses.asdict(trainer.state)
+
+            checkpoint = os.path.join(tmpdir, "checkpoint-16")
+            self.convert_to_sharded_checkpoint(checkpoint)
+
+            # Reinitialize trainer
+            trainer = get_regression_trainer(output_dir=tmpdir, train_len=128, save_steps=5, learning_rate=0.1)
+
+            trainer.train(resume_from_checkpoint=checkpoint)
+            (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+            state1 = dataclasses.asdict(trainer.state)
+            self.assertEqual(a, a1)
+            self.assertEqual(b, b1)
+            self.check_trainer_state_are_the_same(state, state1)
+
+    @require_safetensors
+    def test_resume_training_with_safe_checkpoint(self):
+        # This test will fail for more than 2 GPUs since the batch size will get bigger and with the number of
+        # save_steps, the checkpoint will resume training at epoch 2 or more (so the data seen by the model
+        # won't be the same since the training dataloader is shuffled).
+
+        for initial_safe in [False, True]:
+            for loaded_safe in [False, True]:
+                with tempfile.TemporaryDirectory() as tmpdir:
+                    trainer = get_regression_trainer(
+                        output_dir=tmpdir,
+                        train_len=128,
+                        save_steps=16,
+                        learning_rate=0.1,
+                        save_safetensors=initial_safe,
+                    )
+                    trainer.train()
+                    (a, b) = trainer.model.a.item(), trainer.model.b.item()
+                    state = dataclasses.asdict(trainer.state)
+
+                    checkpoint = os.path.join(tmpdir, "checkpoint-16")
+                    self.convert_to_sharded_checkpoint(checkpoint, load_safe=initial_safe, save_safe=loaded_safe)
+
+                    # Reinitialize trainer
+                    trainer = get_regression_trainer(
+                        output_dir=tmpdir, train_len=128, save_steps=16, learning_rate=0.1, save_safetensors=loaded_safe
+                    )
+
+                    trainer.train(resume_from_checkpoint=checkpoint)
+                    (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+                    state1 = dataclasses.asdict(trainer.state)
+                    self.assertEqual(a, a1)
+                    self.assertEqual(b, b1)
+                    self.check_trainer_state_are_the_same(state, state1)
+
+    def test_resume_training_with_gradient_accumulation(self):
+        # This test will fail for more than 2 GPUs since the batch size will get bigger and with the number of
+        # save_steps, the checkpoint will resume training at epoch 2 or more (so the data seen by the model
+        # won't be the same since the training dataloader is shuffled).
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(
+                output_dir=tmpdir,
+                train_len=128,
+                gradient_accumulation_steps=2,
+                per_device_train_batch_size=4,
+                save_steps=16,
+                learning_rate=0.1,
+            )
+            trainer.train()
+            (a, b) = trainer.model.a.item(), trainer.model.b.item()
+            state = dataclasses.asdict(trainer.state)
+
+            checkpoint = os.path.join(tmpdir, "checkpoint-16")
+
+            # Reinitialize trainer
+            trainer = get_regression_trainer(
+                output_dir=tmpdir,
+                train_len=128,
+                gradient_accumulation_steps=2,
+                per_device_train_batch_size=4,
+                save_steps=16,
+                learning_rate=0.1,
+            )
+
+            trainer.train(resume_from_checkpoint=checkpoint)
+            (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+            state1 = dataclasses.asdict(trainer.state)
+            self.assertEqual(a, a1)
+            self.assertEqual(b, b1)
+            self.check_trainer_state_are_the_same(state, state1)
+
+    def test_resume_training_with_frozen_params(self):
+        # This test will fail for more than 2 GPUs since the batch size will get bigger and with the number of
+        # save_steps, the checkpoint will resume training at epoch 2 or more (so the data seen by the model
+        # won't be the same since the training dataloader is shuffled).
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(
+                output_dir=tmpdir,
+                train_len=128,
+                per_device_train_batch_size=4,
+                save_steps=32,
+                learning_rate=0.1,
+            )
+            trainer.model.a.requires_grad = False
+            trainer.train()
+            (a, b) = trainer.model.a.item(), trainer.model.b.item()
+            state = dataclasses.asdict(trainer.state)
+
+            checkpoint = os.path.join(tmpdir, "checkpoint-32")
+
+            # Reinitialize trainer
+            trainer = get_regression_trainer(
+                output_dir=tmpdir,
+                train_len=128,
+                per_device_train_batch_size=4,
+                save_steps=32,
+                learning_rate=0.1,
+            )
+            trainer.model.a.requires_grad = False
+
+            trainer.train(resume_from_checkpoint=checkpoint)
+
+            self.assertFalse(trainer.model.a.requires_grad)
+            (a1, b1) = trainer.model.a.item(), trainer.model.b.item()
+            state1 = dataclasses.asdict(trainer.state)
+            self.assertEqual(a, a1)
+            self.assertEqual(b, b1)
+            self.check_trainer_state_are_the_same(state, state1)
+
+    def test_load_best_model_at_end(self):
+        total = int(self.n_epochs * 64 / self.batch_size)
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(
+                a=1.5,
+                b=2.5,
+                output_dir=tmpdir,
+                learning_rate=0.1,
+                eval_steps=5,
+                evaluation_strategy="steps",
+                save_steps=5,
+                load_best_model_at_end=True,
+            )
+            self.assertFalse(trainer.args.greater_is_better)
+            trainer.train()
+            self.check_saved_checkpoints(tmpdir, 5, total)
+            self.check_best_model_has_been_loaded(tmpdir, 5, total, trainer, "eval_loss")
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(
+                a=1.5,
+                b=2.5,
+                output_dir=tmpdir,
+                learning_rate=0.1,
+                eval_steps=5,
+                evaluation_strategy="steps",
+                save_steps=5,
+                load_best_model_at_end=True,
+                metric_for_best_model="accuracy",
+                compute_metrics=AlmostAccuracy(),
+            )
+            self.assertTrue(trainer.args.greater_is_better)
+            trainer.train()
+            self.check_saved_checkpoints(tmpdir, 5, total)
+            self.check_best_model_has_been_loaded(tmpdir, 5, total, trainer, "eval_accuracy", greater_is_better=True)
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(
+                a=1.5,
+                b=2.5,
+                output_dir=tmpdir,
+                learning_rate=0.1,
+                evaluation_strategy="epoch",
+                save_strategy="epoch",
+                load_best_model_at_end=True,
+                metric_for_best_model="accuracy",
+                compute_metrics=AlmostAccuracy(),
+            )
+            self.assertTrue(trainer.args.greater_is_better)
+            trainer.train()
+            self.check_saved_checkpoints(tmpdir, 64 // self.batch_size, total)
+            self.check_best_model_has_been_loaded(
+                tmpdir, 64 // self.batch_size, total, trainer, "eval_accuracy", greater_is_better=True
+            )
+
+        # Test this works with a non PreTrainedModel
+        with tempfile.TemporaryDirectory() as tmpdir:
+            trainer = get_regression_trainer(
+                output_dir=tmpdir,
+                learning_rate=0.1,
+                eval_steps=5,
+                evaluation_strategy="steps",
+                save_steps=5,
+                load_best_model_at_end=True,
+                pretrained=False,
+            )
+            self.assertFalse(trainer.args.greater_is_better)
+            trainer.train()
+            self.check_saved_checkpoints(tmpdir, 5, total, is_pretrained=False)
+            self.check_best_model_has_been_loaded(tmpdir, 5, total, trainer, "eval_loss", is_pretrained=False)
+
+    @require_safetensors
+    def test_load_best_model_from_safetensors(self):
+        total = int(self.n_epochs * 64 / self.batch_size)
+        for save_safetensors, pretrained in product([False, True], [False, True]):
+            with tempfile.TemporaryDirectory() as tmpdir:
+                trainer = get_regression_trainer(
+                    a=1.5,
+                    b=2.5,
+                    output_dir=tmpdir,
+                    learning_rate=0.1,
+                    eval_steps=5,
+                    evaluation_strategy="steps",
+                    save_steps=5,
+                    load_best_model_at_end=True,
+                    save_safetensors=save_safetensors,
+                    pretrained=pretrained,
+                )
+                self.assertFalse(trainer.args.greater_is_better)
+                trainer.train()
+                self.check_saved_checkpoints(tmpdir, 5, total, is_pretrained=pretrained, safe_weights=save_safetensors)
+                self.check_best_model_has_been_loaded(
+                    tmpdir, 5, total, trainer, "eval_loss", is_pretrained=pretrained, safe_weights=save_safetensors
+                )
+
+    @slow
+    def test_trainer_eval_mrpc(self):
+        MODEL_ID = "google-bert/bert-base-cased-finetuned-mrpc"
+        tokenizer = AutoTokenizer.from_pretrained(MODEL_ID)
+        model = AutoModelForSequenceClassification.from_pretrained(MODEL_ID)
+        data_args = GlueDataTrainingArguments(
+            task_name="mrpc", data_dir=f"{get_tests_dir()}/fixtures/tests_samples/MRPC", overwrite_cache=True
+        )
+        eval_dataset = GlueDataset(data_args, tokenizer=tokenizer, mode="dev")
+
+        training_args = TrainingArguments(output_dir="./examples", use_cpu=True)
+        trainer = Trainer(model=model, args=training_args, eval_dataset=eval_dataset)
+        result = trainer.evaluate()
+        self.assertLess(result["eval_loss"], 0.2)
+
+    @slow
+    def test_trainer_eval_multiple(self):
+        MODEL_ID = "openai-community/gpt2"
+        tokenizer = AutoTokenizer.from_pretrained(MODEL_ID)
+        model = AutoModelForCausalLM.from_pretrained(MODEL_ID)
+        dataset = LineByLineTextDataset(
+            tokenizer=tokenizer,
+            file_path=PATH_SAMPLE_TEXT,
+            block_size=tokenizer.max_len_single_sentence,
+        )
+        for example in dataset.examples:
+            example["labels"] = example["input_ids"]
+        training_args = TrainingArguments(
+            output_dir="./examples",
+            use_cpu=True,
+            per_device_eval_batch_size=1,
+        )
+        trainer = Trainer(
+            model=model,
+            args=training_args,
+            eval_dataset={
+                "data1": dataset,
+                "data2": dataset,
+            },
+        )
+        result = trainer.evaluate()
+        self.assertIn("eval_data1_loss", result)
+        self.assertIn("eval_data2_loss", result)
+
+    @slow
+    def test_trainer_eval_lm(self):
+        MODEL_ID = "distilbert/distilroberta-base"
+        tokenizer = AutoTokenizer.from_pretrained(MODEL_ID)
+        dataset = LineByLineTextDataset(
+            tokenizer=tokenizer,
+            file_path=PATH_SAMPLE_TEXT,
+            block_size=tokenizer.max_len_single_sentence,
+        )
+        self.assertEqual(len(dataset), 31)
+
+    def test_training_iterable_dataset(self):
+        config = RegressionModelConfig()
+        model = RegressionPreTrainedModel(config)
+        # Adding one column not used by the model should have no impact
+        train_dataset = GeneratorDataset(SampleIterableDataset(label_names=["labels", "extra"]), column_names=['input_x', "labels", "extra"])
+
+        args = RegressionTrainingArguments(output_dir="./examples", max_steps=4)
+        trainer = Trainer(model=model, args=args, train_dataset=train_dataset)
+        trainer.train()
+        self.assertEqual(trainer.state.global_step, 4)
+
+        loader = trainer.get_train_dataset()
+        self.assertIsInstance(loader, mindspore.dataset.Dataset)
+
+    def test_evaluation_iterable_dataset(self):
+        config = RegressionModelConfig(a=1.5, b=2.5)
+        model = RegressionPreTrainedModel(config)
+        # Adding one column not used by the model should have no impact
+        eval_dataset = GeneratorDataset(SampleIterableDataset(label_names=["labels", "extra"]),
+                                        column_names=['input_x', "labels", "extra"], shuffle=False)
+
+        args = RegressionTrainingArguments(output_dir="./examples", per_device_eval_batch_size=64)
+        trainer = Trainer(model=model, args=args, eval_dataset=eval_dataset, compute_metrics=AlmostAccuracy())
+        results = trainer.evaluate()
+
+        x, y = trainer.eval_dataset.source.dataset.x, trainer.eval_dataset.source.dataset.ys[0]
+        pred = 1.5 * x + 2.5
+        expected_loss = ((pred - y) ** 2).mean()
+        self.assertAlmostEqual(results["eval_loss"], expected_loss)
+        expected_acc = AlmostAccuracy()((pred, y))["accuracy"]
+        self.assertAlmostEqual(results["eval_accuracy"], expected_acc)
+
+        # With a number of elements not a round multiple of the batch size
+        eval_dataset = GeneratorDataset(SampleIterableDataset(length=66),
+                                        column_names=['input_x', "labels"], shuffle=False)
+        results = trainer.evaluate(eval_dataset)
+
+        x, y = eval_dataset.source.dataset.x, eval_dataset.source.dataset.ys[0]
+        pred = 1.5 * x + 2.5
+        expected_loss = ((pred - y) ** 2).mean()
+        self.assertAlmostEqual(results["eval_loss"], expected_loss)
+        expected_acc = AlmostAccuracy()((pred, y))["accuracy"]
+        self.assertAlmostEqual(results["eval_accuracy"], expected_acc)
+
+    def test_predict_iterable_dataset(self):
+        config = RegressionModelConfig(a=1.5, b=2.5)
+        model = RegressionPreTrainedModel(config)
+        eval_dataset = GeneratorDataset(SampleIterableDataset(), column_names=['input_x', 'labels'])
+
+        args = RegressionTrainingArguments(output_dir="./examples")
+        trainer = Trainer(model=model, args=args, eval_dataset=eval_dataset, compute_metrics=AlmostAccuracy())
+
+        preds = trainer.predict(trainer.eval_dataset).predictions
+        x = eval_dataset.source.dataset.x
+        self.assertTrue(np.allclose(preds, 1.5 * x + 2.5))
+
+        # With a number of elements not a round multiple of the batch size
+        # Adding one column not used by the model should have no impact
+        test_dataset = GeneratorDataset(SampleIterableDataset(length=66, label_names=["labels", "extra"]),
+                                        column_names=['input_x', 'labels', "extra"])
+        preds = trainer.predict(test_dataset).predictions
+        x = test_dataset.source.dataset.x
+        self.assertTrue(np.allclose(preds, 1.5 * x + 2.5))
+
+    def test_num_train_epochs_in_training(self):
+        # len(train_dl) < gradient_accumulation_steps shouldn't give ``ZeroDivisionError`` when ``max_steps`` is given.
+        # It should give 1 update step for each epoch.
+        trainer = get_regression_trainer(
+            max_steps=3, train_len=64, per_device_train_batch_size=16, gradient_accumulation_steps=5
+        )
+        train_output = trainer.train()
+        self.assertEqual(train_output.global_step, 3)
+
+        # Even ``max_steps`` is not specified, we still expect 1 update step for each epoch if
+        # len(train_dl) < gradient_accumulation_steps.
+        trainer = get_regression_trainer(train_len=64, per_device_train_batch_size=16, gradient_accumulation_steps=5)
+        train_output = trainer.train()
+        self.assertEqual(train_output.global_step, int(self.n_epochs))
+
+    def test_early_stopping_callback(self):
+        # early stopping stops training before num_training_epochs
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            trainer = get_regression_trainer(
+                output_dir=tmp_dir,
+                num_train_epochs=20,
+                gradient_accumulation_steps=1,
+                per_device_train_batch_size=16,
+                load_best_model_at_end=True,
+                evaluation_strategy=IntervalStrategy.EPOCH,
+                save_strategy=IntervalStrategy.EPOCH,
+                compute_metrics=AlmostAccuracy(),
+                metric_for_best_model="accuracy",
+            )
+            trainer.add_callback(EarlyStoppingCallback(1, 0.0001))
+            train_output = trainer.train()
+            self.assertLess(train_output.global_step, 20 * 64 / 16)
+
+        # Invalid inputs to trainer with early stopping callback result in assertion error
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            trainer = get_regression_trainer(
+                output_dir=tmp_dir,
+                num_train_epochs=20,
+                gradient_accumulation_steps=1,
+                per_device_train_batch_size=16,
+                evaluation_strategy=IntervalStrategy.EPOCH,
+                compute_metrics=AlmostAccuracy(),
+                metric_for_best_model="accuracy",
+            )
+            trainer.add_callback(EarlyStoppingCallback(1))
+            self.assertEqual(trainer.state.global_step, 0)
+            try:
+                trainer.train()
+            except AssertionError:
+                self.assertEqual(trainer.state.global_step, 0)
+
+    def test_flos_extraction(self):
+        trainer = get_regression_trainer(learning_rate=0.1)
+
+        def assert_flos_extraction(trainer, wrapped_model_to_check):
+            self.assertEqual(trainer.model, wrapped_model_to_check)
+            self.assertGreaterEqual(getattr(wrapped_model_to_check.config, "total_flos", 0), 0)
+
+        # with plain model
+        assert_flos_extraction(trainer, trainer.model)
+
+        # # with enforced DataParallel
+        # assert_flos_extraction(trainer, nn.DataParallel(trainer.model))
+
+        trainer.train()
+        self.assertTrue(isinstance(trainer.state.total_flos, float))
+
+    def check_checkpoint_deletion(self, trainer, output_dir, expected):
+        # Make fake checkpoints
+        for n in [5, 10, 15, 20, 25]:
+            os.makedirs(os.path.join(output_dir, f"{PREFIX_CHECKPOINT_DIR}-{n}"), exist_ok=True)
+        trainer._rotate_checkpoints(output_dir=output_dir)
+        glob_checkpoints = [str(x) for x in Path(output_dir).glob(f"{PREFIX_CHECKPOINT_DIR}-*")]
+        values = [int(re.match(f".*{PREFIX_CHECKPOINT_DIR}-([0-9]+)", d).groups()[0]) for d in glob_checkpoints]
+        self.assertSetEqual(set(values), set(expected))
+
+    def test_checkpoint_rotation(self):
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            # Without best model at end
+            trainer = get_regression_trainer(output_dir=tmp_dir, save_total_limit=2)
+            self.check_checkpoint_deletion(trainer, tmp_dir, [20, 25])
+
+            # With best model at end
+            trainer = get_regression_trainer(
+                output_dir=tmp_dir, evaluation_strategy="steps", load_best_model_at_end=True, save_total_limit=2
+            )
+            trainer.state.best_model_checkpoint = os.path.join(tmp_dir, "checkpoint-5")
+            self.check_checkpoint_deletion(trainer, tmp_dir, [5, 25])
+
+            # Edge case: we don't always honor save_total_limit=1 if load_best_model_at_end=True to be able to resume
+            # from checkpoint
+            trainer = get_regression_trainer(
+                output_dir=tmp_dir, evaluation_strategy="steps", load_best_model_at_end=True, save_total_limit=1
+            )
+            trainer.state.best_model_checkpoint = os.path.join(tmp_dir, "checkpoint-25")
+            self.check_checkpoint_deletion(trainer, tmp_dir, [25])
+
+            trainer.state.best_model_checkpoint = os.path.join(tmp_dir, "checkpoint-5")
+            self.check_checkpoint_deletion(trainer, tmp_dir, [5, 25])
+
+    def check_mem_metrics(self, trainer, check_func):
+        metrics = trainer.train().metrics
+        check_func("init_mem_cpu_alloc_delta", metrics)
+        check_func("train_mem_cpu_alloc_delta", metrics)
+        if backend_device_count(torch_device) > 0:
+            check_func("init_mem_gpu_alloc_delta", metrics)
+            check_func("train_mem_gpu_alloc_delta", metrics)
+
+        metrics = trainer.evaluate()
+        check_func("eval_mem_cpu_alloc_delta", metrics)
+        if backend_device_count(torch_device) > 0:
+            check_func("eval_mem_gpu_alloc_delta", metrics)
+
+        metrics = trainer.predict(RegressionDataset()).metrics
+        check_func("test_mem_cpu_alloc_delta", metrics)
+        if backend_device_count(torch_device) > 0:
+            check_func("test_mem_gpu_alloc_delta", metrics)
+
+    # def test_mem_metrics(self):
+    #     # with mem metrics enabled
+    #     trainer = get_regression_trainer(skip_memory_metrics=False)
+    #     self.check_mem_metrics(trainer, self.assertIn)
+
+    #     # with mem metrics disabled
+    #     trainer = get_regression_trainer(skip_memory_metrics=True)
+    #     self.check_mem_metrics(trainer, self.assertNotIn)
+
+    @pytest.mark.skip('skip_memory_metrics not support')
+    def test_fp16_full_eval(self):
+        # this is a sensitive test so let's keep debugging printouts in place for quick diagnosis.
+        # it's using pretty large safety margins, but small enough to detect broken functionality.
+        debug = 0
+        n_gpus = 1
+
+        bs = 8
+        eval_len = 16 * n_gpus
+        # make the params somewhat big so that there will be enough RAM consumed to be able to
+        # measure things. We should get about 64KB for a+b in fp32
+        a = np.ones((1000, bs), np.float32) + 0.001
+        b = np.ones((1000, bs), np.float32) - 0.001
+
+        # 1. with fp16_full_eval disabled
+        trainer = get_regression_trainer(a=a, b=b, eval_len=eval_len, skip_memory_metrics=False)
+        metrics = trainer.evaluate()
+        del trainer
+        gc.collect()
+
+        fp32_init = metrics["init_mem_gpu_alloc_delta"]
+        fp32_eval = metrics["eval_mem_gpu_alloc_delta"]
+
+        if debug:
+            print(f"fp32_init {fp32_init}")
+            print(f"fp32_eval {fp32_eval}")
+
+        # here we expect the model to be preloaded in trainer.__init__ and consume around 64K gpu ram.
+        # perfect world: fp32_init == 64<<10
+        self.assertGreater(fp32_init, 59_000)
+        # after eval should be no extra memory allocated - with a small margin (other than the peak
+        # memory consumption for the forward calculation that gets recovered)
+        # perfect world: fp32_eval == close to zero
+        self.assertLess(fp32_eval, 5_000)
+
+        # 2. with fp16_full_eval enabled
+        trainer = get_regression_trainer(a=a, b=b, eval_len=eval_len, fp16_full_eval=True, skip_memory_metrics=False)
+        metrics = trainer.evaluate()
+        fp16_init = metrics["init_mem_gpu_alloc_delta"]
+        fp16_eval = metrics["eval_mem_gpu_alloc_delta"]
+
+        if debug:
+            print(f"fp16_init {fp16_init}")
+            print(f"fp16_eval {fp16_eval}")
+
+        # here we expect the model to not be preloaded in trainer.__init__, so with a small margin it should be close to 0
+        # perfect world: fp16_init == close to zero
+        self.assertLess(fp16_init, 5_000)
+        # here we put the model on device in eval and only `half()` of it, i.e. about 32K,(again we ignore the peak margin which gets returned back)
+        # perfect world: fp32_init == 32<<10
+        self.assertGreater(fp16_eval, 27_000)
+
+        # 3. relative comparison fp32 vs full fp16
+        # should be about half of fp16_init
+        # perfect world: fp32_init/2 == fp16_eval
+        self.assertAlmostEqual(fp16_eval, fp32_init / 2, delta=5_000)
+
+
+    @pytest.mark.skip('not support bf16')
+    @require_mindspore
+    def test_bf16_full_eval(self):
+        # note: most of the logic is the same as test_fp16_full_eval
+
+        # this is a sensitive test so let's keep debugging printouts in place for quick diagnosis.
+        # it's using pretty large safety margins, but small enough to detect broken functionality.
+        debug = 0
+        n_gpus = 1
+
+        bs = 8
+        eval_len = 16 * n_gpus
+        # make the params somewhat big so that there will be enough RAM consumed to be able to
+        # measure things. We should get about 64KB for a+b in fp32
+        a = ops.ones(1000, bs) + 0.001
+        b = ops.ones(1000, bs) - 0.001
+
+        # 1. with bf16_full_eval disabled
+        trainer = get_regression_trainer(a=a, b=b, eval_len=eval_len, skip_memory_metrics=False)
+        metrics = trainer.evaluate()
+        del trainer
+        gc.collect()
+
+        fp32_init = metrics["init_mem_gpu_alloc_delta"]
+        fp32_eval = metrics["eval_mem_gpu_alloc_delta"]
+
+        if debug:
+            print(f"fp32_init {fp32_init}")
+            print(f"fp32_eval {fp32_eval}")
+
+        # here we expect the model to be preloaded in trainer.__init__ and consume around 64K gpu ram.
+        # perfect world: fp32_init == 64<<10
+        self.assertGreater(fp32_init, 59_000)
+        # after eval should be no extra memory allocated - with a small margin (other than the peak
+        # memory consumption for the forward calculation that gets recovered)
+        # perfect world: fp32_eval == close to zero
+        self.assertLess(fp32_eval, 5_000)
+
+        # 2. with bf16_full_eval enabled
+        trainer = get_regression_trainer(a=a, b=b, eval_len=eval_len, bf16_full_eval=True, skip_memory_metrics=False)
+        metrics = trainer.evaluate()
+        bf16_init = metrics["init_mem_gpu_alloc_delta"]
+        bf16_eval = metrics["eval_mem_gpu_alloc_delta"]
+
+        if debug:
+            print(f"bf16_init {bf16_init}")
+            print(f"bf16_eval {bf16_eval}")
+
+        # here we expect the model to not be preloaded in trainer.__init__, so with a small margin it should be close to 0
+        # perfect world: bf16_init == close to zero
+        self.assertLess(bf16_init, 5_000)
+        # here we put the model on device in eval and only `half()` of it, i.e. about 32K,(again we ignore the peak margin which gets returned back)
+        # perfect world: fp32_init == 32<<10
+        self.assertGreater(bf16_eval, 27_000)
+
+        # 3. relative comparison fp32 vs full bf16
+        # should be about half of bf16_init
+        # perfect world: fp32_init/2 == bf16_eval
+        self.assertAlmostEqual(bf16_eval, fp32_init / 2, delta=5_000)
+
+    def test_no_wd_param_group(self):
+        model = nn.SequentialCell(TstLayer(128), nn.CellList([TstLayer(128), TstLayer(128)]))
+        trainer = Trainer(model=model)
+        trainer.create_optimizer_and_scheduler(10)
+        wd_names = ['0.linear1.weight', '0.linear2.weight', '1.0.linear1.weight', '1.0.linear2.weight', '1.1.linear1.weight', '1.1.linear2.weight']  # fmt: skip
+        wd_params = [p for n, p in model.parameters_and_names() if n in wd_names]
+        no_wd_params = [p for n, p in model.parameters_and_names() if n not in wd_names]
+        self.assertListEqual(trainer.optimizer.param_groups[0]["params"], wd_params)
+        self.assertListEqual(trainer.optimizer.param_groups[1]["params"], no_wd_params)
+
+    @slow
+    def test_end_to_end_example(self):
+        # Tests that `translation.py` will run without issues
+        script_path = os.path.abspath(
+            os.path.join(
+                os.path.dirname(__file__), "..", "..", "examples", "pytorch", "translation", "run_translation.py"
+            )
+        )
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            command = [
+                "accelerate",
+                "launch",
+                script_path,
+                "--model_name_or_path",
+                "google-t5/t5-small",
+                "--per_device_train_batch_size",
+                "1",
+                "--output_dir",
+                tmpdir,
+                "--overwrite_output_dir",
+                "--do_train",
+                "--max_train_samples",
+                "64",
+                "--num_train_epochs",
+                "1",
+                "--dataset_name",
+                "wmt16",
+                "--dataset_config",
+                "ro-en",
+                "--source_lang",
+                "en",
+                "--target_lang",
+                "ro",
+                "--do_predict",
+                "--max_predict_samples",
+                "64",
+                "--predict_with_generate",
+                "--ddp_timeout",
+                "60",
+            ]
+            execute_subprocess_async(command)
+            # successful return here == success - any errors would have caused an error or a timeout in the sub-call
+
+optim_test_params = []
+if is_mindspore_available():
+    default_adam_kwargs = {
+        "betas": (TrainingArguments.adam_beta1, TrainingArguments.adam_beta2),
+        "eps": TrainingArguments.adam_epsilon,
+        "lr": TrainingArguments.learning_rate,
+    }
+
+    default_lion_kwargs = {
+        "betas": (TrainingArguments.adam_beta1, TrainingArguments.adam_beta2),
+        "lr": TrainingArguments.learning_rate,
+    }
+
+    default_anyprecision_kwargs = {
+        "use_kahan_summation": False,
+        "momentum_dtype": mindspore.float32,
+        "variance_dtype": mindspore.float32,
+        "compensation_buffer_dtype": mindspore.bfloat16,
+    }
+
+    optim_test_params = [
+        (
+            TrainingArguments(optim=OptimizerNames.ADAMW, output_dir="None"),
+            mindspore.experimental.optim.AdamW,
+            default_adam_kwargs,
+        ),
+        # (
+        #     TrainingArguments(optim=OptimizerNames.ADAFACTOR, output_dir="None"),
+        #     transformers.optimization.Adafactor,
+        #     {
+        #         "scale_parameter": False,
+        #         "relative_step": False,
+        #         "lr": TrainingArguments.learning_rate,
+        #     },
+        # ),
+    ]
+
+
+@require_mindspore
+class TrainerOptimizerChoiceTest(unittest.TestCase):
+    def check_optim_and_kwargs(self, training_args: TrainingArguments, expected_cls, expected_kwargs):
+        actual_cls, optim_kwargs = Trainer.get_optimizer_cls_and_kwargs(training_args)
+        self.assertEqual(expected_cls, actual_cls)
+        self.assertIsNotNone(optim_kwargs)
+
+        for p, v in expected_kwargs.items():
+            self.assertTrue(p in optim_kwargs)
+            actual_v = optim_kwargs[p]
+            self.assertTrue(actual_v == v, f"Failed check for {p}. Expected {v}, but got {actual_v}.")
+
+    @parameterized.expand(optim_test_params, skip_on_empty=True)
+    def test_optim_supported(self, training_args: TrainingArguments, expected_cls, expected_kwargs):
+        # exercises all the valid --optim options
+        self.check_optim_and_kwargs(training_args, expected_cls, expected_kwargs)
+
+        trainer = get_regression_trainer(**training_args.to_dict())
+        trainer.train()
```

## tests/ut/modules/test_flashattention.py

```diff
@@ -9,76 +9,165 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Test FlashAttention-v2-FP32"""
-from math import sqrt
 import unittest
 import numpy as np
 import pytest
 
 import mindspore as ms
 from mindspore import ops, Tensor
 from mindnlp.transformers.kernel_utils import compile_kernel
 from mindnlp.utils.testing_utils import require_mindspore_gpu
 
+
 class TestFlashAttention(unittest.TestCase):
     r"""
     Test module flashattention
     """
 
-    def load_flash_cuda_kernel(self, func_name, context_length):
-        """load flash cuda kernel"""
-        device_target = ms.get_context("device_target")
-        if device_target != "GPU":
-            raise RuntimeError("FlashAttention operator only support GPU currently.")
-
-        so_path = compile_kernel(kernel_name="flash", Tmax=context_length)
-        flash_op = ops.Custom(
-            f"{str(so_path)}:{func_name}",
-            out_shape=lambda q, k, v, l, m: q,
-            out_dtype=lambda q, k, v, l, m: q,
-            func_type="aot",
-        )
-        flash_op.add_prim_attr("primitive_target", device_target)
-        return flash_op
-
-    def manual_attn(self, query, key, value):
+    def manual_attn_forward(self, query, key, value):
         r"""
         manual attention
         """
         embed_size = query.shape[-1]
-        scaling_factor = sqrt(sqrt(Tensor(embed_size, ms.float32)))
+        scaling_factor = ops.sqrt(ops.sqrt(Tensor(embed_size, ms.float32)))
         query = query / scaling_factor
+        attn_mask = ops.ones((query.shape[-2], key.shape[-2]), ms.bool_).tril()
         attn = ops.matmul(query, key.swapaxes(-2, -1) / scaling_factor)
+        attn = attn.masked_fill(attn_mask == 0, float("-inf"))
         attn = ops.softmax(attn, -1)
         output = ops.matmul(attn, value)
         return output
 
+    def manual_attn_backward(self, query, key, value):
+        return ms.grad(self.manual_attn_forward, grad_position=(0, 1, 2))(
+            query, key, value
+        )
+
     @require_mindspore_gpu
-    def test_flashattention2_forward_FP32(self):
+    def test_flashattention2_fp32(self):
         r"""
         Unit test for flashattention forward.
         """
         # 加载flash cuda kernel
-        op = self.load_flash_cuda_kernel("flash_forward", 512)
+        device_target = ms.get_context("device_target")
+        if device_target != "GPU":
+            raise RuntimeError("FlashAttention operator only support GPU currently.")
 
+        so_path = compile_kernel(kernel_name="flash", Tmax=1024)
+        flash_1_fwd_op = ops.Custom(
+            f"{str(so_path)}:flash_attn_1_fwd_f32",
+            out_shape=lambda q, k, v: (q, (q[0], q[1], q[2]), (q[0], q[1], q[2])),
+            out_dtype=lambda q, k, v: (q, q, q),
+            func_type="aot",
+        )
+        flash_1_fwd_op.add_prim_attr("primitive_target", device_target)
+
+        flash_2_fwd_op = ops.Custom(
+            f"{str(so_path)}:flash_attn_2_fwd_f32",
+            out_shape=lambda q, k, v,: (q, (q[0], q[1], q[2])),
+            out_dtype=lambda q, k, v,: (q, q),
+            func_type="aot",
+        )
+        flash_2_fwd_op.add_prim_attr("primitive_target", device_target)
         profiler = ms.Profiler()
 
-        # 定义输入数据
-        Q = np.random.randn(16, 12, 64, 64).astype(np.float32)
-        K = np.random.randn(16, 12, 64, 64).astype(np.float32)
-        V = np.random.randn(16, 12, 64, 64).astype(np.float32)
-        l = np.zeros((16, 12, 64), dtype=np.float32)
-        m = np.ones((16, 12, 64), dtype=np.float32) * (-np.inf)
-        print("=== profiling MindSpore manual-attention === ")
-        output_manual = self.manual_attn(ms.Tensor(Q), ms.Tensor(K), ms.Tensor(V))
-        # profiler.analyse()
-        print("=== profiling MindSpore flash-attention === ")
-        output = op(
-            ms.Tensor(Q), ms.Tensor(K), ms.Tensor(V), ms.Tensor(l), ms.Tensor(m)
+        # seq_len must be multiple of Br
+        Q = np.random.randn(8, 12, 1024, 64).astype(np.float32)
+        K = np.random.randn(8, 12, 1024, 64).astype(np.float32)
+        V = np.random.randn(8, 12, 1024, 64).astype(np.float32)
+        print("====== profiling forward pass ======")
+        print("=== profiling MindSpore manual-attention(forward) === ")
+        output_manual_fwd = self.manual_attn_forward(
+            ms.Tensor(Q), ms.Tensor(K), ms.Tensor(V)
+        )
+        print("=== profiling MindSpore flash-attention-v1(forward) === ")
+        output1_fwd, l, m = flash_1_fwd_op(
+            ms.Tensor(Q),
+            ms.Tensor(K),
+            ms.Tensor(V),
+        )
+        print(output1_fwd)
+        assert np.allclose(
+            output1_fwd[0].asnumpy(), output_manual_fwd[0].asnumpy(), atol=1e-02
+        )
+        print("=== profiling MindSpore flash-attention-v2(forward) === ")
+        output2_fwd, L = flash_2_fwd_op(
+            ms.Tensor(Q),
+            ms.Tensor(K),
+            ms.Tensor(V),
+        )
+
+        assert np.allclose(
+            output2_fwd[0].asnumpy(), output_manual_fwd[0].asnumpy(), atol=1e-02
+        )
+        print("=== MindSpore flash-attention(forward) pass === \n")
+
+        print("====== profiling backward pass ======")
+
+        flash_1_bwd_op = ops.Custom(
+            f"{str(so_path)}:flash_attn_1_bwd_f32",
+            out_shape=lambda q, k, v, do, o, l, m: (q, q, q),
+            out_dtype=lambda q, k, v, do, o, l, m: (q, q, q),
+            func_type="aot",
+        )
+        flash_1_bwd_op.add_prim_attr("primitive_target", device_target)
+
+        flash_2_bwd_op = ops.Custom(
+            f"{str(so_path)}:flash_attn_2_bwd_f32",
+            out_shape=lambda q, k, v, o, do, l: (q, q, q),
+            out_dtype=lambda q, k, v, o, do, l: (q, q, q),
+            func_type="aot",
+        )
+        flash_2_bwd_op.add_prim_attr("primitive_target", device_target)
+
+        y_grad = np.ones_like(output_manual_fwd.asnumpy(), dtype=np.float32)
+
+        print("=== profiling MindSpore manual-attention(backward) === ")
+        (
+            output_manual_bwd_dq,
+            output_manual_bwd_dk,
+            output_manual_bwd_dv,
+        ) = self.manual_attn_backward(
+            ms.Tensor(Q),
+            ms.Tensor(K),
+            ms.Tensor(V),
+        )
+        print("=== profiling MindSpore flash-attention-v1(backward) === ")
+        (
+            output1_bwd_dq,
+            output1_bwd_dk,
+            output1_bwd_dv,
+        ) = flash_1_bwd_op(
+            ms.Tensor(Q),
+            ms.Tensor(K),
+            ms.Tensor(V),
+            ms.Tensor(output1_fwd),
+            ms.Tensor(y_grad),
+            ms.Tensor(l),
+            ms.Tensor(m),
+        )
+        assert np.allclose(
+            output1_bwd_dq[0].asnumpy(), output_manual_bwd_dq[0].asnumpy(), atol=1e-02
+        )
+        print("=== profiling MindSpore flash-attention-v2(backward) === ")
+        (
+            output2_bwd_dq,
+            output2_bwd_dk,
+            output2_bwd_dv,
+        ) = flash_2_bwd_op(
+            ms.Tensor(Q),
+            ms.Tensor(K),
+            ms.Tensor(V),
+            ms.Tensor(output2_fwd),
+            ms.Tensor(y_grad),
+            ms.Tensor(L),
         )
         profiler.analyse()
-        # print(output)
-        assert np.allclose(output[0].asnumpy(), output_manual[0].asnumpy(), atol=1e-03)
+        assert np.allclose(
+            output2_bwd_dq[0].asnumpy(), output_manual_bwd_dq[0].asnumpy(), atol=1e-02
+        )
+        print("=== MindSpore flash-attention(backward) pass === ")
```

## tests/ut/transformers/test_backbone_common.py

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 
 import copy
 import inspect
 import tempfile
 
 from mindnlp.utils.testing_utils import require_mindspore
-from mindnlp.utils.backbone_utils import BackboneType
+from mindnlp.transformers.backbone_utils import BackboneType
 
 
 @require_mindspore
 class BackboneTesterMixin:
     all_model_classes = ()
     has_attentions = True
```

## tests/ut/transformers/test_modeling_common.py

```diff
@@ -932,22 +932,22 @@
             model(**self._prepare_for_class(inputs_dict, model_class))
 
             # Check that adding and removing tokens has not modified the first part of the embedding matrix.
             models_equal = True
 
             if model.config.is_encoder_decoder:
                 for p1, p2 in zip(encoder_cloned_embeddings, encoder_model_embed.weight):
-                    if p1.data.ne(p2.data).sum() > 0:
+                    if p1.ne(p2).sum() > 0:
                         models_equal = False
                 for p1, p2 in zip(decoder_cloned_embeddings, decoder_model_embed.weight):
-                    if p1.data.ne(p2.data).sum() > 0:
+                    if p1.ne(p2).sum() > 0:
                         models_equal = False
             else:
                 for p1, p2 in zip(cloned_embeddings, model_embed.weight):
-                    if p1.data.ne(p2.data).sum() > 0:
+                    if p1.ne(p2).sum() > 0:
                         models_equal = False
 
             self.assertTrue(models_equal)
 
     def test_resize_tokens_embeddings(self):
         (
             original_config,
```

## tests/ut/transformers/generation/test_utils.py

```diff
@@ -1801,17 +1801,18 @@
             with self.assertRaises(AssertionError):
                 self.assertListEqual(outputs_from_rand_embeds.tolist(), outputs_from_embeds.tolist())
 
             # input_ids is not a required input -- if we don't pass it, the newly generated tokens will be the same
             outputs_from_embeds_wo_ids = model.generate(
                 inputs_embeds=inputs_embeds, max_new_tokens=20 - inputs_embeds.shape[1]
             )
+
             self.assertListEqual(
                 outputs_from_embeds[:, inputs_embeds.shape[1] :].tolist(),
-                outputs_from_embeds_wo_ids[:, 1:].tolist(),
+                outputs_from_embeds_wo_ids.tolist(),
             )
 
     def _check_outputs(self, output, input_ids, config, use_cache=False, num_return_sequences=1):
         batch_size, seq_length = input_ids.shape
         num_sequences_in_output = batch_size * num_return_sequences
         gen_len = (
             output.sequences.shape[-1] - 1 if config.is_encoder_decoder else output.sequences.shape[-1] - seq_length
```

## tests/ut/transformers/models/chatglm/test_modeling_chatglm.py

```diff
@@ -35,17 +35,17 @@
     for _ in range(total_dims):
         values.append(random.randint(0, vocab_size - 1))
 
     return mindspore.tensor(data=values, dtype=mindspore.int64).view(shape)
 
 
 def get_model_and_tokenizer():
-    model = AutoModelForSeq2SeqLM.from_pretrained("THUDM/chatglm-6b").half()
+    model = AutoModelForSeq2SeqLM.from_pretrained("THUDM/chatglm-6b", mirror='aifast').half()
     model.set_train(False)
-    tokenizer = AutoTokenizer.from_pretrained("THUDM/chatglm-6b")
+    tokenizer = AutoTokenizer.from_pretrained("THUDM/chatglm-6b", mirror='gitee')
     return model, tokenizer
 
 def get_model_and_tokenizer_random_init():
     config = AutoConfig.from_pretrained("THUDM/chatglm-6b")
     model = AutoModelForSeq2SeqLM.from_config(config).half()
     model.set_train(False)
     tokenizer = AutoTokenizer.from_pretrained("THUDM/chatglm-6b")
```

## tests/ut/transformers/models/convbert/test_modeling_convbert.py

```diff
@@ -32,15 +32,14 @@
         ConvBertForMaskedLM,
         ConvBertForMultipleChoice,
         ConvBertForQuestionAnswering,
         ConvBertForSequenceClassification,
         ConvBertForTokenClassification,
         ConvBertModel,
     )
-    mindspore.set_context(pynative_synchronize=True)
 
 
 class ConvBertModelTester:
     def __init__(
         self,
         parent,
         batch_size=13,
```

## tests/ut/transformers/models/xlnet/test_modeling_xlnet.py

```diff
@@ -90,15 +90,14 @@
         self.seed = 1
         self.type_vocab_size = 2
         self.bos_token_id = 1
         self.eos_token_id = 2
         self.pad_token_id = 5
         self.num_choices = 4
 
-        mindspore.set_context(pynative_synchronize=True)
 
     def prepare_config_and_inputs(self):
 
         input_ids_1 = ids_tensor([self.batch_size, self.seq_length], self.vocab_size)
         input_ids_2 = ids_tensor([self.batch_size, self.seq_length], self.vocab_size)
         segment_ids = ids_tensor([self.batch_size, self.seq_length], self.type_vocab_size)
         input_mask = random_attention_mask([self.batch_size, self.seq_length])
```

## Comparing `mindnlp/engine/evaluator.py` & `mindnlp/_legacy/engine/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 """
 Evaluator for testing.
 """
 from inspect import signature
 from tqdm.autonotebook import tqdm
 from mindnlp import ms_jit
 from mindnlp.abc import Metric
-from mindnlp.engine.callbacks.callback_manager import CallbackManager, RunContext
-from mindnlp.utils import ModelOutput, logging
+from .callbacks.callback_manager import CallbackManager, RunContext
+from ...utils import ModelOutput, logging
 
 logger = logging.get_logger(__name__)
 
 class Evaluator:
     r"""
     Evaluator to test the model.
```

## Comparing `mindnlp/engine/train_args.py` & `mindnlp/_legacy/engine/train_args.py`

 * *Files identical despite different names*

## Comparing `mindnlp/engine/callbacks/__init__.py` & `mindnlp/_legacy/engine/callbacks/__init__.py`

 * *Files identical despite different names*

## Comparing `mindnlp/engine/callbacks/best_model_callback.py` & `mindnlp/_legacy/engine/callbacks/best_model_callback.py`

 * *Files identical despite different names*

## Comparing `mindnlp/engine/callbacks/callback_manager.py` & `mindnlp/_legacy/engine/callbacks/callback_manager.py`

 * *Files identical despite different names*

## Comparing `mindnlp/engine/callbacks/checkpoint_callback.py` & `mindnlp/_legacy/engine/callbacks/checkpoint_callback.py`

 * *Files identical despite different names*

## Comparing `mindnlp/engine/callbacks/earlystop_callback.py` & `mindnlp/_legacy/engine/callbacks/earlystop_callback.py`

 * *Files identical despite different names*

## Comparing `mindnlp/engine/callbacks/timer_callback.py` & `mindnlp/_legacy/engine/callbacks/timer_callback.py`

 * *Files identical despite different names*

## Comparing `mindnlp/engine/trainer/utils.py` & `mindnlp/_legacy/engine/trainer/utils.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/__init__.py` & `mindnlp/_legacy/metrics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 Callbacks.
 """
-from mindnlp.metrics import accuracy, bleu, confusion_matrix, distinct, em_score, \
+from . import accuracy, bleu, confusion_matrix, distinct, em_score, \
     f1, matthews, pearson, perplexity, precision, recall, rouge, spearman
 
 from .perplexity import *
 from .bleu import *
 from .rouge import *
 from .distinct import *
 from .accuracy import *
```

## Comparing `mindnlp/metrics/accuracy.py` & `mindnlp/_legacy/metrics/accuracy.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/bleu.py` & `mindnlp/_legacy/metrics/bleu.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/confusion_matrix.py` & `mindnlp/_legacy/metrics/confusion_matrix.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/distinct.py` & `mindnlp/_legacy/metrics/distinct.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/em_score.py` & `mindnlp/_legacy/metrics/em_score.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/f1.py` & `mindnlp/_legacy/metrics/f1.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/matthews.py` & `mindnlp/_legacy/metrics/matthews.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/pearson.py` & `mindnlp/_legacy/metrics/pearson.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/perplexity.py` & `mindnlp/_legacy/metrics/perplexity.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/precision.py` & `mindnlp/_legacy/metrics/precision.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/recall.py` & `mindnlp/_legacy/metrics/recall.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/rouge.py` & `mindnlp/_legacy/metrics/rouge.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/spearman.py` & `mindnlp/_legacy/metrics/spearman.py`

 * *Files identical despite different names*

## Comparing `mindnlp/metrics/utils.py` & `mindnlp/_legacy/metrics/utils.py`

 * *Files identical despite different names*

## Comparing `mindnlp/text2vec/__init__.py` & `mindnlp/_legacy/engine/export.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-# Copyright 2024 Huawei Technologies Co., Ltd
+# Copyright 2022 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""MindNLP Text2vec"""
-from .sentence_model import SentenceModel
-from .word2vec import Word2Vec
+"""
+export models to other IR format
+"""
+
+# TODO: use `mindspore.export` api to achieve such function.
```

## Comparing `mindnlp/utils/backbone_utils.py` & `mindnlp/transformers/backbone_utils.py`

 * *Files identical despite different names*

## Comparing `tests/ut/metrics/test_metrics_class.py` & `tests/ut/legacy/metrics/test_metrics_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Test Classes for Metrics"""
 
 
 import unittest
 import numpy as np
 import mindspore
 from mindspore import Tensor
-from mindnlp.metrics import (Perplexity, BleuScore, RougeN, RougeL, Distinct, Accuracy,
+from mindnlp._legacy.metrics import (Perplexity, BleuScore, RougeN, RougeL, Distinct, Accuracy,
                              Precision, Recall, F1Score, ConfusionMatrix,
                              MatthewsCorrelation, PearsonCorrelation,
                              SpearmanCorrelation, EmScore)
 
 
 class TestClassPerplexity(unittest.TestCase):
     r"""
```

## Comparing `tests/ut/metrics/test_metrics_fn.py` & `tests/ut/legacy/metrics/test_metrics_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Test the Functions for Metrics"""
 
 
 import unittest
 import numpy as np
 import mindspore
 from mindspore import Tensor
-from mindnlp.metrics import (perplexity_fn, bleu_fn, rouge_n_fn, rouge_l_fn, distinct_fn, accuracy_fn,
+from mindnlp._legacy.metrics import (perplexity_fn, bleu_fn, rouge_n_fn, rouge_l_fn, distinct_fn, accuracy_fn,
                              precision_fn, recall_fn, f1_score_fn, confusion_matrix_fn,
                              matthews_correlation_fn, pearson_correlation_fn,
                              spearman_correlation_fn, em_score_fn)
 
 class TestPerplexity(unittest.TestCase):
     r"""
     Test perplexity
```

## Comparing `tests/ut/transformers/models/gpt_neox/test_gpt_neox.py` & `tests/ut/transformers/models/gpt_neox/test_modeling_gpt_neox.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,8 +351,9 @@
             if isinstance(value, list) and isinstance(value[0], np.ndarray):
                 return mindspore.tensor(np.array(value), dtype)
             if isinstance(value, np.ndarray) and value.shape == (0,):
                 return mindspore.tensor(mindspore._c_expression.Tensor(value, dtype)) # pylint: disable=c-extension-no-member
             return mindspore.tensor(value, dtype)
         input_ids = as_tensor(input_ids)[None]
         outputs = model(input_ids)["logits"][:, -1][0, :30]
+        print(EXPECTED_LOGITS.asnumpy(), outputs.asnumpy())
         self.assertTrue(np.allclose(EXPECTED_LOGITS.asnumpy(), outputs.asnumpy(), atol=1e-5))
```

## Comparing `mindnlp-0.2.4.dist-info/LICENSE` & `mindnlp-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mindnlp-0.2.4.dist-info/METADATA` & `mindnlp-0.3.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: mindnlp
-Version: 0.2.4
-Summary: An open source natural language processing research tool box. Git version: [sha1]:caca912, [branch]: (HEAD -> clip, origin/clip)
+Version: 0.3.0
+Summary: An open source natural language processing research tool box. Git version: [sha1]:18acd45, [branch]: (HEAD -> master, ms/master)
 Home-page: https://github.com/mindlab-ai/mindnlp/tree/master/
 Author: MindSpore Team
 License: Apache 2.0
 Project-URL: Sources, https://github.com/mindlab-ai/mindnlp
 Project-URL: Issue Tracker, https://github.com/mindlab-ai/mindnlp/issues
 Classifier: License :: OSI Approved :: Apache Software License
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: mindspore
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: datasets
+Requires-Dist: evaluate
 Requires-Dist: tokenizers
+Requires-Dist: safetensors
 Requires-Dist: sentencepiece
 Requires-Dist: regex
 Requires-Dist: addict
-Requires-Dist: safetensors
 Requires-Dist: ml-dtypes
 Requires-Dist: pyctcdecode
+Requires-Dist: jieba
```

## Comparing `mindnlp-0.2.4.dist-info/RECORD` & `mindnlp-0.3.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,35 @@
 mindnlp/__init__.py,sha256=zN8WkA5xfrlykU1ubuW85EGUnb7R9dH5P4TACcQI17M,1162
-mindnlp/configs.py,sha256=gFz3hmr14cJZdpqvJZqaAasa3yFcwnCkg4KWueMjPQw,2170
-mindnlp/injection.py,sha256=O3_H5tfhAAPGq7v5vjmVrkprFU3pugKQ7sGZ4d66jPI,37726
-mindnlp/readme.md,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/_csrc/cuda/flash.cu,sha256=fuOhLHgN5m-BPVVmMqOZZd0nD4jTNywTZsx-NpCUJOc,5132
+mindnlp/amp.py,sha256=50_-YR7mmAiiF3k6_7R7abcnjNivHpdYQxz51QLhejs,2099
+mindnlp/configs.py,sha256=0aMBrU_fXVLqe2mfYqlns1uNkXDpGEqP8DX2RujWteg,2302
+mindnlp/injection.py,sha256=tLq-yiOkZgnExGPH0CkCRq5CdOcZ6LWNameO-LT8PgQ,44332
+mindnlp/_csrc/cuda/flash.cu,sha256=SGkPnD7EtijC44oRl1CC99x-ESD-KlKXpuC_dZKn8M0,29929
 mindnlp/_csrc/cuda/wkv.cu,sha256=Sbgw3Sd6mYoyy8M9DwtcW0CjDtq-d6FxvlskViSv7xA,7940
 mindnlp/_legacy/__init__.py,sha256=RPO-lfdXFzTdUTiIlkM0hjlVovkCspDhG7u5p9q1QR0,707
 mindnlp/_legacy/amp.py,sha256=5h55oV-Jw_Fab-vGc_AkX98aIGXa4ntDPUw0O6rgCcg,7978
-mindnlp/_legacy/functional.py,sha256=cVr4ugcow96nFQqlmHmXwFMe2AZ05prIoUa4xTWL9Pk,67590
+mindnlp/_legacy/functional.py,sha256=9JVbn9_sInXyjfwAWP8758yr6mItyu57RZOcjpTcrHI,67596
 mindnlp/_legacy/initializer.py,sha256=GvBTOWfCoXZJw61x2rp_nB3bauw2j7-l5SYgPHGl7bg,2633
 mindnlp/_legacy/utils.py,sha256=L9lp1u3CNEsKdCMYzw2earOGQ4McGRv9Ap6YhInfEpg,3284
+mindnlp/_legacy/engine/__init__.py,sha256=cFr_jRrFiqi15P1zKqazG1IQBeP_wETrSuz9v2leGGI,779
+mindnlp/_legacy/engine/evaluator.py,sha256=Ok9f7eKAWu4vVv2rOHe8U-9lb8s96GWnXtuTd6Yf5d8,8087
+mindnlp/_legacy/engine/export.py,sha256=fGF3DEKz7LuStbtSsrzBKVCr7RozgnnHM_2jm4f4rJg,770
+mindnlp/_legacy/engine/train_args.py,sha256=Y_csPQd4XAN5SziYEATatYenr7O40SwvJsSMzUm9yRM,807
+mindnlp/_legacy/engine/utils.py,sha256=lnpkLWbeOMqPwJFwwp5YjYL-aO1JWhixsJ0vKSB1xeY,1120
+mindnlp/_legacy/engine/callbacks/__init__.py,sha256=2e2ObWOpnFC56VYNI8qOLmdtJ27sCJLpbKTmTLF0KNY,927
+mindnlp/_legacy/engine/callbacks/best_model_callback.py,sha256=jn0w-l2g9v_nt1JuNhQi8HGpD7dGm7_VrMD4xf955-0,5118
+mindnlp/_legacy/engine/callbacks/callback_manager.py,sha256=VIoDN-zZjgIDlF_uLdU55nsXDZf0l_vxhXx57nY6kis,4086
+mindnlp/_legacy/engine/callbacks/checkpoint_callback.py,sha256=G6_tXgsQPBntTCs6JPksGEIkilSFolQo7C1ZIFzXHZA,4156
+mindnlp/_legacy/engine/callbacks/earlystop_callback.py,sha256=LothxjyR_q4a_yAZGVaf19nNxeTY7Qk7LhjSQWFa0yY,2464
+mindnlp/_legacy/engine/callbacks/timer_callback.py,sha256=V5fhYX0O_3TDd2CIGoXUmQXRnPB5GpUj-mofTbq6Cu0,6079
+mindnlp/_legacy/engine/trainer/__init__.py,sha256=dW7MTfGG5MJw2lQfEuxpTD0C3wh8wgxQvx3ThHZcPRY,753
+mindnlp/_legacy/engine/trainer/base.py,sha256=smXet9SRyD6A2g5vI3Hb2PFZhOVDeCJza0NpwyFU0ow,16871
+mindnlp/_legacy/engine/trainer/ppo.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/_legacy/engine/trainer/rm.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/_legacy/engine/trainer/sft.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/_legacy/engine/trainer/utils.py,sha256=qz9sfAbH0HJff3NxjpWojeqsvNdwnvZwIX9bhZ5NNr4,3704
 mindnlp/_legacy/hypercomplex/__init__.py,sha256=OmaMN7P1RO8LK7QHvAYtwF5Aluaijv107v9uMH7TkvQ,883
 mindnlp/_legacy/hypercomplex/utils.py,sha256=sKYW_RQTdUBsGI6HpqVXCG9KGJdh5R2zxEzaLp8t4x8,1755
 mindnlp/_legacy/hypercomplex/complex/__init__.py,sha256=1TQK3Tl1XpohRK9fXtcMA1OpXd4bAIrxb2lyfwjyS4o,882
 mindnlp/_legacy/hypercomplex/complex/_complex_bn_impl.py,sha256=i9JoEpTiCfqcJT9yn5oScrB2sEP9CsLiQVk93wAXFuk,6981
 mindnlp/_legacy/hypercomplex/complex/_complex_conv_impl.py,sha256=yVfjYD70brGitKR0h6Oabh98lMMrIu6K6tt3Kq_2HvI,11071
 mindnlp/_legacy/hypercomplex/complex/_complex_dense_impl.py,sha256=fCIiS0VBOFzxnVOEiamppY09QIU_CW4CNFVZgm1o610,5878
 mindnlp/_legacy/hypercomplex/complex/_complex_relu.py,sha256=Tqx40I42TIWpnIw6q-FGHs--jo_uSy_3Ws7pC7WILRM,2146
@@ -35,130 +52,95 @@
 mindnlp/_legacy/hypercomplex/hypercomplex/_hc_conv_impl.py,sha256=xZSpRch6w7OOKxaA8IrdZB4oKaIusQ0pGwXQrZ9f9Ok,5893
 mindnlp/_legacy/hypercomplex/hypercomplex/_hc_dense_impl.py,sha256=jda1wqlGqTCw-u-XYD2G9QTA_zWdOjqOcFPJGoVOmWw,5140
 mindnlp/_legacy/hypercomplex/hypercomplex/hc_bn.py,sha256=PCnh_b2kDMMSD8W94sxtN5cbvmRnGudA7kV3i_hG5Fw,36029
 mindnlp/_legacy/hypercomplex/hypercomplex/hc_conv.py,sha256=GQ7-VBTcBvGxGkY4KpnMf6114AXxPFV2EX_rZMkx_O0,49241
 mindnlp/_legacy/hypercomplex/hypercomplex/hc_dense.py,sha256=wKXz8u7nwpjt76GDV9UnkLDGkiXkgnuc9gFUUZeLUzI,11082
 mindnlp/_legacy/hypercomplex/hypercomplex/hc_pool.py,sha256=7ccf1Mnjr0t6s7xHtMJS908eQo3JaxjwCxAPkPF4e9Y,44353
 mindnlp/_legacy/hypercomplex/hypercomplex/uniform_operator.py,sha256=g4Df6538nK54qO3VVuOKs9ltK3lDXpGxVixATWziHF0,1691
-mindnlp/_legacy/hypercomplex/tensor_decomposition/hypercomplex_td.py,sha256=iTIzMvgbARLgIqIF-1RBdvQXgyTLd0E6nFCpb8wXYRE,2915
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/dual_svd.py,sha256=OW1VriE2bU3HZWw0iGzNb5IGfQnJDPHYohplbCKQzTY,4383
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/qr.py,sha256=CXzG8YVCM55gA2bDaQTROmw17nXUlB_tsHBJFqUTMFQ,4886
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/star_svd.py,sha256=LyMi4CNyuoznug3zC3UVRfQQI2IYMI5zUR_smuz6sNs,802
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/svd.py,sha256=2cpAY7HE3HNDiB7rv-NYXoPIlXBKSnit2iFy5Sbp1Rg,3728
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/algorithm/t_svd.py,sha256=Ol7Vkj52zm88HohuSnbtsheM4hIsji7vSF2_B35kyhs,800
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/matrix.py,sha256=FKRizlMDkc57TL2L8lAiGHm58RhAAB6ehqvb-rfrrSE,6592
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/scalar.py,sha256=-owkKrFa9EGJ17pr1iFkaAaHTCBuq5FJZnyhjrUY46U,1431
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/scalar_visitor.py,sha256=usNdk7g1Dv6vCI69uGk4WhU8AsLgpnBGsdT9xDHlqR0,593
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/vector.py,sha256=XnC9iNifMmjWuzxbUEjmrNnG68KTXQbcl1dNlawQBSQ,4859
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/complex/_complex_algebra_impl.py,sha256=rHmlPdhyFg6pYwIDHsHW1KeHa0AZqjLsJe9p2SMAewg,3088
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/complex/complex_algebra_factory.py,sha256=jrwavQimWlaBMjNihevkmxfY3d24Ay0nSrtkeRbsGUE,894
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/dual/_dual_algebra_impl.py,sha256=Ztg46J9sTgl6LWtSGw1LfpMckEM4jSJNtjfiinyZ2yg,2640
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/dual/dual_algebra_factory.py,sha256=BYARgw14ePI0NYtRUXywxkHpHX4e3x0a-5YToGk8AqA,873
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_math_obj_impl.py,sha256=VTpuGtd3nwLS04WuwJJ305pcVxLYsLLUFhKkXmHeJeY,594
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_matrix_impl.py,sha256=rF_MT31x7dNGQfvywfNdICqPht0hEQuh8PPVlBVFvC4,456
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_scalar_impl.py,sha256=aInHM4INYCLCZ1hVhriKnHXOIOv4NeMIAhFPLXVtcCQ,858
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/_hc_vector_impl.py,sha256=BqdzlItny1Pq_nZ7ws2Sc1QGlr_gOEg2ZA6MYSx9_P8,481
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_algebra_factory.py,sha256=L7Qhga9yxPutzczjNoFDJYzzPVaJjaWatE_tKUVKmO0,653
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_matrix.py,sha256=RXl53f4hP1yEcQZ2EGkNxHJLufvn-ILz2JPGHoOoz2o,13424
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_scalar.py,sha256=vq7DzynVoMITWPFz-bsW6DD9hTxWRMD3pZLMMP23zm0,3020
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/hypercomplex/hc_vector.py,sha256=hf-Q2fEJ19ZhIX00TpXOFhvYAuwsxETIeDA3SV04gQk,9501
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/real/real_matrix.py,sha256=KLJNz1CZ7-yF2Tl901YNFZzwcl9Qnf1wnk68Pq-cFxY,6240
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/real/real_scalar.py,sha256=9jWJ8SoAIFm6ovzvfpK3rLMA6SPQ1CV48TuzapZrzeU,1650
-mindnlp/_legacy/hypercomplex/tensor_decomposition/linal/basics/real/real_vector.py,sha256=PpOGrYceiSbZ0ure1vao6LKiYQVeuVphQqAQKIX2PHM,4089
+mindnlp/_legacy/metrics/__init__.py,sha256=SzLkEzfuh3rG_ATqrSJ0oX7BNxZ1RNQwpkCYmmp0dSk,1576
+mindnlp/_legacy/metrics/accuracy.py,sha256=iTm2KdSrqk1ZpTibjOwd2Zw_l1earl4y3M2_tSUuWe8,7525
+mindnlp/_legacy/metrics/bleu.py,sha256=PL6apPQF1BGNEcD83wCdDjtCn6DqvzlDpzJTFBgYlno,10364
+mindnlp/_legacy/metrics/confusion_matrix.py,sha256=vbsRGBcjyZIAqgwENF0-JX6lPASAVpBvbJlWBj64FJM,6201
+mindnlp/_legacy/metrics/distinct.py,sha256=qkdyDwbRJ0YxlJCltCszrW_jQj-93wTpM5u7x7wa-0c,4231
+mindnlp/_legacy/metrics/em_score.py,sha256=27xO_n6dZCICsAgv4dDUAeXzD9d4QJJLDl8h04nV2tA,6130
+mindnlp/_legacy/metrics/f1.py,sha256=b9dxTetVJpBvzXRQKIkfmuEwwnCH3XP97WtYa2__74w,8006
+mindnlp/_legacy/metrics/matthews.py,sha256=XSTLBqcuU0rV5O96vrGb-zoPy5Dyk6hMLLkz29yUWNI,7665
+mindnlp/_legacy/metrics/pearson.py,sha256=eMCBUZMBff8syheTNMfvEcJfEtHtxi_kTZX4qVeIrs8,7280
+mindnlp/_legacy/metrics/perplexity.py,sha256=3M-3ERae6o8JsW7bb9wH_9kXqwjKq4stq3pFgSxT2GU,9898
+mindnlp/_legacy/metrics/precision.py,sha256=stIppEdcOqcBgrIKMRnlssC8f8T29zyMakVrr8qdbgE,7040
+mindnlp/_legacy/metrics/recall.py,sha256=3b9XZB4pTEm-vLsvPf5JWhUBJ9MNbMJiM_2WdnrKnz4,6746
+mindnlp/_legacy/metrics/rouge.py,sha256=6HzBuoKsGn_tQIfZ3urx6LADU1uR7Tw_Vofm4ak3SKg,12329
+mindnlp/_legacy/metrics/spearman.py,sha256=vk-L0mFnVzHOmKRHq_3-KboYrmfbDXTx4hWw-_RQWNA,6735
+mindnlp/_legacy/metrics/utils.py,sha256=Pycmys4mwc8m6GpiIKoSvRZcpDWgBWDWHULIOz4buug,4407
 mindnlp/_legacy/nn/__init__.py,sha256=k_nbrmE1VeUrnLdlpknWRlgXGM64HoE699t2y9FoY0s,1092
 mindnlp/_legacy/nn/dropout.py,sha256=N5rtog27z3KVYDlYfr1OFaJlThvoprbAiTGWY1V6NlI,3367
 mindnlp/_legacy/nn/half_op.py,sha256=QtJDhpj0EBgzCS0UhklQ7z0TbUd9FF8zGMLZQp8F9yQ,896
 mindnlp/_legacy/nn/transformer.py,sha256=hT0xpPfJZtBfpTvhzICpyNObZ7W76LixF-7oMc7mAz0,33081
 mindnlp/_legacy/ops/__init__.py,sha256=psCypTLtIAHU56ad6wbRKquJT6lqYgywmetFYfRsJPw,797
 mindnlp/_legacy/ops/parallel.py,sha256=SWcFYeNOa-9XN8A0IlUFMLLQ7xJz73RTGqbuuRP7MxI,1196
 mindnlp/_legacy/transforms/__init__.py,sha256=aj5PQDyvcYuBbNqh8aO2ps1i5MkWUJyXKlrCWfjDev4,872
 mindnlp/_legacy/transforms/add_token.py,sha256=ZFeF5LRgBiTzKO9YiWMXuutqdIQnJlff0vlgQcDqpXs,2110
 mindnlp/_legacy/transforms/truncate.py,sha256=_5KjHZtG-8rI6DuGVdO7FaBaVD8FC4yYqHg6GJa0eLM,1880
 mindnlp/abc/__init__.py,sha256=hHcc3DyEDk_MSga2H7l4LCBnqqVy-bTEjcwoEkChH0E,822
 mindnlp/abc/callback.py,sha256=cxJdFzkfphK9Pa-LmDkKs-vQ265R1C5cy4x9d2_b0OU,2926
-mindnlp/abc/container.py,sha256=XKXzhG8PCUdtDI-zdmsAdzgxno_bYgfJgzp3t3DwFcY,5945
+mindnlp/abc/container.py,sha256=24o48z5dL0_wVpOxJkfp9r-I7a1K_6eEK7JCUKkaMaY,8313
 mindnlp/abc/metric.py,sha256=rnzWKC2sYa6eEG-Q4dTTUb49oO2lelNxkGqCu6aJtqM,2870
 mindnlp/abc/register.py,sha256=SJvfq2cvR5y_cyzTHMyWZ0iNuIex8-2oLPEblCMOgqo,1466
 mindnlp/abc/models/__init__.py,sha256=PQozoDVuNZq9pH68XppPStmn2Y7mOT5BI7tgcVqg13U,823
 mindnlp/abc/models/base_model.py,sha256=ALbTIaovycpxqyl056O6EVy49VPi7nDH9KWAR0VFDhc,6023
 mindnlp/abc/models/seq2seq_model.py,sha256=PdN6deP9A2IU_vk9GVZWgOCDpyVQ8LZwIXAqz5FsyOY,3414
 mindnlp/abc/models/seq2vec_model.py,sha256=0wsMaP0GbiX4IwGPoDRyJhUvPTCEot2cAywEG8nhSdE,2934
 mindnlp/abc/modules/__init__.py,sha256=mSSBTGPH4gCq6PVFgnqkB0gGGDlP7iWhdSDv4pkaez0,811
 mindnlp/abc/modules/decoder.py,sha256=ki7LY8-tj5P2Exr2ZxtWN6AGF7-FF8IiCcDqCVSYa64,2816
 mindnlp/abc/modules/embedding.py,sha256=_EibCZq9paxLXLvQyHVFh4kN_deZVcEs4HQkMn__dQA,2408
 mindnlp/abc/modules/encoder.py,sha256=t4BXKE9qKgw2oxB8perXF7-FKMCLCvugC9d5vorEDB0,2360
 mindnlp/abc/modules/generator.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/accelerate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/accelerate/accelerator.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/accelerate/inference.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/data/__init__.py,sha256=j4RrOJsPko6ds6O82aPI773vTlauoD11BHXblnrL_2c,790
 mindnlp/data/io/__init__.py,sha256=UfsVFnx2S5r1SMZ_OWCohz7nncoh3oyaXspgJ4d2LZU,736
 mindnlp/data/io/audio.py,sha256=M-0IXCsx-JP0RU8A1IoJZOq5IdNlv3wtaTaC7SRvjwM,34595
 mindnlp/data/processors/__init__.py,sha256=_c2YLOgkf0ONf07sFzphIUiggUjfR6iDc7oQHKOsT-0,768
 mindnlp/data/processors/squad.py,sha256=OPx6DLo4oM-zv5lM8wv_r3yUkyuqUKRTcdO7HVxjmoY,20407
-mindnlp/dataset/__init__.py,sha256=scyJLq-6z8vC1lxOL7lkCd73ZgokL_owgCMtq6-gNLQ,720
+mindnlp/dataset/__init__.py,sha256=OMWmMIobk1oloyid5bLQwwLXghM-xq6VBVIpjudTTr0,755
 mindnlp/dataset/load.py,sha256=NcWwtYE1LknWJZucyfiX26nQdincpWb9BKygLBGE-JU,13264
+mindnlp/dataset/map_fn.py,sha256=JcMgBXpR8a51GZFIeanYozr3ZYhPYmxbHAc2oucCh9E,907
 mindnlp/dataset/utils.py,sha256=OLw6rwxpJmkWX11Hai1H2lF2ZwuLUNUWvf1i296g0cI,1921
 mindnlp/dataset/transforms/__init__.py,sha256=ib-XL8MQPr1fdmA7utmKp-yh1DDImBcW-WWxYyyTfwE,1211
 mindnlp/dataset/transforms/basic_tokenizer.py,sha256=EllLR6ee01UrMcJFY5Z8QhNTf8mUoRz8AeDPpdnZ8uM,9716
 mindnlp/dataset/transforms/jieba_tokenizer.py,sha256=cipFmFHH5XTOaiHHfRUVgOrbCdKjih7UfBIHA6vEsWQ,1608
 mindnlp/dataset/transforms/lookup.py,sha256=mzd8JtwJkCuzq-_wVqg2rFp5nVwisBXkrHOG7uyORnA,2508
 mindnlp/dataset/transforms/pad_transform.py,sha256=oEoCuo4ZBas16G07e5Fz9bGST0pgnYKbg1l_uXP86kM,2548
-mindnlp/diffusers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/diffusers/loaders/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/diffusers/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/diffusers/pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/diffusers/schedulers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/diffusers/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/engine/__init__.py,sha256=cFr_jRrFiqi15P1zKqazG1IQBeP_wETrSuz9v2leGGI,779
-mindnlp/engine/evaluator.py,sha256=xh8vOAzen6jkJZHhy_iSujauVWuSCIub4KZNp2Xv2JQ,8106
+mindnlp/engine/__init__.py,sha256=Ej-0L31vyPx46SoW-5cqMCiPVnDU0l-Usns1TxGcgMc,787
+mindnlp/engine/callbacks.py,sha256=36mHnEzjumWmW3Fck1dfYGt2sq7c6xXfHE1fqy3WlfA,24684
 mindnlp/engine/export.py,sha256=fGF3DEKz7LuStbtSsrzBKVCr7RozgnnHM_2jm4f4rJg,770
-mindnlp/engine/train_args.py,sha256=Y_csPQd4XAN5SziYEATatYenr7O40SwvJsSMzUm9yRM,807
-mindnlp/engine/utils.py,sha256=pNIDTw78s5IuWcs07idGv7VLbHOuQWcYWOuQLQ4nA5c,1125
-mindnlp/engine/callbacks/__init__.py,sha256=2e2ObWOpnFC56VYNI8qOLmdtJ27sCJLpbKTmTLF0KNY,927
-mindnlp/engine/callbacks/best_model_callback.py,sha256=jn0w-l2g9v_nt1JuNhQi8HGpD7dGm7_VrMD4xf955-0,5118
-mindnlp/engine/callbacks/callback_manager.py,sha256=VIoDN-zZjgIDlF_uLdU55nsXDZf0l_vxhXx57nY6kis,4086
-mindnlp/engine/callbacks/checkpoint_callback.py,sha256=G6_tXgsQPBntTCs6JPksGEIkilSFolQo7C1ZIFzXHZA,4156
-mindnlp/engine/callbacks/earlystop_callback.py,sha256=LothxjyR_q4a_yAZGVaf19nNxeTY7Qk7LhjSQWFa0yY,2464
-mindnlp/engine/callbacks/timer_callback.py,sha256=V5fhYX0O_3TDd2CIGoXUmQXRnPB5GpUj-mofTbq6Cu0,6079
+mindnlp/engine/utils.py,sha256=7vGxnxR_D2QWVn8tQbFUthpe0lAtWAkUqKYWoUgya7I,19087
+mindnlp/engine/train_args/__init__.py,sha256=7ALRr8RHhgr4Iw2QT_NKBC5Ov3r6TFp3molvbTqPCoI,39
+mindnlp/engine/train_args/base.py,sha256=Wr4cANXVh8EOyXGyWOEA6VKTqoovAdOTzNSXnsMxxe4,94202
+mindnlp/engine/train_args/ddpo.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/engine/train_args/kto.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/engine/train_args/ppo.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/engine/train_args/reward.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/engine/train_args/seq2seq.py,sha256=-a8GkIqwN_oqjYZTnvzjAnoxCg8ZaS-lNkPjCLApGk8,4248
 mindnlp/engine/trainer/__init__.py,sha256=dW7MTfGG5MJw2lQfEuxpTD0C3wh8wgxQvx3ThHZcPRY,753
-mindnlp/engine/trainer/base.py,sha256=BoCSX28L6IFjH1lmZLJihAavfaN2-XE-k82PrH8GEvg,16949
-mindnlp/engine/trainer/ppo.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/engine/trainer/base.py,sha256=XS1X9LDDjMNyK1ReBwNJHXKfS6xLlLP20I90mIn_eUU,93556
+mindnlp/engine/trainer/default_func.py,sha256=8toWbTBUh8_ijbn_u1gOfKOtu9tnsLdF_8qBXSVGGT0,3703
+mindnlp/engine/trainer/ppo_trainer.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/engine/trainer/reward_trainer.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/engine/trainer/rl_base.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/engine/trainer/rm.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/engine/trainer/sft.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/engine/trainer/utils.py,sha256=qz9sfAbH0HJff3NxjpWojeqsvNdwnvZwIX9bhZ5NNr4,3704
-mindnlp/evaluate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/suite.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/audio_classification.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/automatic_speech_recognition.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/base.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/image_classification.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/question_answering.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/text2text_generation.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/text_classification.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/text_generation.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/evaluate/evaluator/token_classification.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindnlp/metrics/__init__.py,sha256=eSbM_PQ96E3pN_Dz7KM-WcHGxWSvLL7OJWjao2h91go,1590
-mindnlp/metrics/accuracy.py,sha256=iTm2KdSrqk1ZpTibjOwd2Zw_l1earl4y3M2_tSUuWe8,7525
-mindnlp/metrics/bleu.py,sha256=PL6apPQF1BGNEcD83wCdDjtCn6DqvzlDpzJTFBgYlno,10364
-mindnlp/metrics/confusion_matrix.py,sha256=vbsRGBcjyZIAqgwENF0-JX6lPASAVpBvbJlWBj64FJM,6201
-mindnlp/metrics/distinct.py,sha256=qkdyDwbRJ0YxlJCltCszrW_jQj-93wTpM5u7x7wa-0c,4231
-mindnlp/metrics/em_score.py,sha256=27xO_n6dZCICsAgv4dDUAeXzD9d4QJJLDl8h04nV2tA,6130
-mindnlp/metrics/f1.py,sha256=b9dxTetVJpBvzXRQKIkfmuEwwnCH3XP97WtYa2__74w,8006
-mindnlp/metrics/matthews.py,sha256=XSTLBqcuU0rV5O96vrGb-zoPy5Dyk6hMLLkz29yUWNI,7665
-mindnlp/metrics/pearson.py,sha256=eMCBUZMBff8syheTNMfvEcJfEtHtxi_kTZX4qVeIrs8,7280
-mindnlp/metrics/perplexity.py,sha256=3M-3ERae6o8JsW7bb9wH_9kXqwjKq4stq3pFgSxT2GU,9898
-mindnlp/metrics/precision.py,sha256=stIppEdcOqcBgrIKMRnlssC8f8T29zyMakVrr8qdbgE,7040
-mindnlp/metrics/recall.py,sha256=3b9XZB4pTEm-vLsvPf5JWhUBJ9MNbMJiM_2WdnrKnz4,6746
-mindnlp/metrics/rouge.py,sha256=6HzBuoKsGn_tQIfZ3urx6LADU1uR7Tw_Vofm4ak3SKg,12329
-mindnlp/metrics/spearman.py,sha256=vk-L0mFnVzHOmKRHq_3-KboYrmfbDXTx4hWw-_RQWNA,6735
-mindnlp/metrics/utils.py,sha256=Pycmys4mwc8m6GpiIKoSvRZcpDWgBWDWHULIOz4buug,4407
+mindnlp/engine/trainer/seq2seq_trainer.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/engine/trainer/sft_trainer.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/modules/__init__.py,sha256=F4kJ17bhyCauXK8KOULTNe0CZ_mX-p08QoWFp434Dks,2229
 mindnlp/modules/accumulator.py,sha256=ySal1DQovq2XS8jd4sjNmj9sbfXpFJQtEIJ1rR94O5M,1966
 mindnlp/modules/attentions.py,sha256=ROvYft2AjZ4LhXzwlUIIczSWzueW5Nu-ZeyofUE78eE,22547
 mindnlp/modules/crf.py,sha256=zBZ0opZ8XI1ngsWgmrWnBGyqGmJlTKbd9JaLsY6lb-U,13033
 mindnlp/modules/loss.py,sha256=1bNP98aScwV5vEGYw4sOQxbzvIUVuqWQ08k5xEHRxkY,6458
+mindnlp/modules/optimization.py,sha256=LFaqNNuv9B4BPgez2SdTvfHmQ6vlvBRrN3QhMjKtTkQ,22616
 mindnlp/modules/rnns.py,sha256=EmpSu6T6b6YsMIx0Oqr-KZmUVjRJiyE2PHbgYqZ4s2k,22885
 mindnlp/modules/weight_norm.py,sha256=IlODsU6wfguwza_KQ7Wb3yFd2egZ-zUI3lqRNKysBvg,7136
 mindnlp/modules/custom/__init__.py,sha256=La-dV9qOD9ib2pV3ot47dOFSOxRtnCTYZajlpvF_LIo,702
 mindnlp/modules/decoder/__init__.py,sha256=PN_Jzr19TMpxirSH80MVovkxIl6TJa8HZ52PI9P7J28,773
 mindnlp/modules/decoder/rnn_decoder.py,sha256=EtcmbVPNq_G5uCmjd_etZRcIBZe_74Cwo3YiOBahX5Q,10869
 mindnlp/modules/embeddings/__init__.py,sha256=hO-yEUA5WdRhLgYbDZd49C5gvBYZwK1wfSNfE1xkgkE,801
 mindnlp/modules/embeddings/fasttext_embedding.py,sha256=SG-A0wxBFS7V_g5xmh1Q37oA3DRH_i3M70jByKPhChs,8276
@@ -170,61 +152,73 @@
 mindnlp/modules/functional/graph_func.py,sha256=5e69qOeIlEhqxw0pKmS4MU2OOrMTYM1M77m0g0g7E6g,2705
 mindnlp/modules/functional/neural_network.py,sha256=Pf_MIFL-ZFf57tuPGCNQv-hW69bA7k5PjwyFjbPy0kw,985
 mindnlp/modules/functional/normalize.py,sha256=3atvFVH59AxPi2lo3h6lhdUIuVRJ2_Z7i8KLwL_a09g,838
 mindnlp/modules/functional/weight_norm.py,sha256=aKXYPxFkHFCwKqyew8xxL322Gsknh3T9dpY3QT7HdOQ,3298
 mindnlp/parallel/__init__.py,sha256=aUXrEICNTzyZLPD7IIs9J-neiRAJ47a7ypjni_0lqdU,846
 mindnlp/parallel/pipeline_parallel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/parallel/tensor_parallel/__init__.py,sha256=qW1fLvXW8FyfP8ZNhY8llemXEds8sDNEf-l2UiSgjtw,818
-mindnlp/parallel/tensor_parallel/layers.py,sha256=pkfNDj-0ucrbdMYMoShqr7EZ1FJi8jh44bwJByv4oZ4,11750
+mindnlp/parallel/tensor_parallel/layers.py,sha256=TQ655i8drzwCDLH198VpgK9nX6GtpS41AkU6Sd_szbg,11658
 mindnlp/parallel/tensor_parallel/mappings.py,sha256=nErGGVRND7ssEX4gWwuzEaxBW36f-ImQZ-42cT4VSU0,4587
 mindnlp/parallel/tensor_parallel/utils.py,sha256=7j9VVlFJcS0BtoHdAsz8WnX7cB4POHrd3MwcecCRCPk,3369
-mindnlp/peft/__init__.py,sha256=JeA0ORJJpssJUCdfywfsQoPXhhE9xuVojqfA4lVIkQ8,1594
-mindnlp/peft/config.py,sha256=wdE3GEFguv3rzZfYgSUGYemIgcuqreoSuGqAODn5lgA,6758
-mindnlp/peft/mapping.py,sha256=W1M_RcsUjF_q-adQWL2iAVFjEIQIsehPObILMnQDyOY,3322
-mindnlp/peft/peft_model.py,sha256=fyShaUdaaOKlG8qJTy7m5xBwIEyY86HrusNI8Luw_Nc,37352
-mindnlp/peft/tuners/__init__.py,sha256=X7H4NvAHmBkLIPMArfe72n1eCE1QsX212uImU7tytOY,738
-mindnlp/peft/tuners/lora.py,sha256=XvHzVD3vSUN49AlZxnNRwbxLezH9gAjnbUh9elA0JbM,37392
-mindnlp/peft/tuners/tuners_utils.py,sha256=RApfuINIoWSxqYP8fZrLl3piyzYqLJ2W5j6sMNPjILU,11619
-mindnlp/peft/utils/__init__.py,sha256=9Sj2W5-v3pMhc0iUV6PZnQLuDKgBHiPEs8LlotZY0hI,1756
-mindnlp/peft/utils/other.py,sha256=cO_Gq1AxqDavrriM3JGfWUaQQ6beoiCORxh33H0XQQU,11128
-mindnlp/peft/utils/peft_types.py,sha256=U5GcTifIt7-DvIkTO--3sAuWSflmguSR6v1G_9edq1U,1242
-mindnlp/peft/utils/save_and_load.py,sha256=vzFYbUz82I8B5LpsJR3jdwbT5Wb7mmrwKJlAYSAxjSY,5767
-mindnlp/text2vec/__init__.py,sha256=5txdPGVtJz_iMTM3C4yVCCo_1_SxQ-6Po7e8L1KmRPU,763
-mindnlp/text2vec/sentence_model.py,sha256=6oDeltBvsUmQqHigLGcAEYMf575a5KKc-5_AfRQ3C7g,8215
-mindnlp/text2vec/word2vec.py,sha256=HGygGq7Y34IlgJhu1rtRgrDWZkINyC5iW_OPJN_Bu6A,6109
-mindnlp/transformers/__init__.py,sha256=Qu8PvCl1bZ5IPo-_7BtrTxLWwHirS556wA6peJ-aQqQ,1287
+mindnlp/peft/__init__.py,sha256=Q1xNycZ8P9x_UKkVbFCcEi6XY7dI766ZyiXc-jE2XR0,1711
+mindnlp/peft/config.py,sha256=1Hv8jXCFFXtj4Qx7oDnH8BBojFLUmJWpn6nGXDKjCz0,6932
+mindnlp/peft/mapping.py,sha256=Xw9UzKud5c2dw-z8ea3tuxkJtpmcmZaRPCxK9Nl3ATs,3458
+mindnlp/peft/peft_model.py,sha256=fu9YwM6F-HvOJuxyszikppUIH91XH2mYaXlRav7scdk,37530
+mindnlp/peft/tuners/__init__.py,sha256=TtR_YbIuouDvvSPdg6KRjTMGw6niCWGFF12G2w9TkUU,898
+mindnlp/peft/tuners/lora.py,sha256=bF3h0-iFXybVJ5nXFGUnMl_5Vb92SC24iX0PSzfjnmY,37353
+mindnlp/peft/tuners/tuners_utils.py,sha256=tOE8o_VoXPnYB8jnOd77oMMmBb-J7B0WJTiwJixx88E,21709
+mindnlp/peft/tuners/adalora/__init__.py,sha256=RJfJXzMym82Qdp03EiE7foQTcusN3FhliR9dyzRXg40,908
+mindnlp/peft/tuners/adalora/config.py,sha256=pTAT8T3CbRNX9qqINfdi27fJzZJEf4sPilKTdCtMlwI,2875
+mindnlp/peft/tuners/adalora/layer.py,sha256=ZUGa43wClHpwppJxEBKZVr9Nu19KK87d_Crf_GMcS8E,16835
+mindnlp/peft/tuners/adalora/model.py,sha256=K46uOIAI9CPBCcowQ4xz0QlNFIM0j5BQZSaThqyGxpE,17645
+mindnlp/peft/tuners/adaption_prompt/__init__.py,sha256=vPCNDBbuuGJ5rwhrDXAUq7jm6JA6RvyL80Od8llLSvQ,817
+mindnlp/peft/tuners/adaption_prompt/config.py,sha256=LPGC4Nm1wVWDllFM_va0p4iurEsQVoyxf3dJ9GWGlSo,2999
+mindnlp/peft/tuners/adaption_prompt/layer.py,sha256=4hT-3lvVNU2uHZBHZ-oEcXtBjmaE6FllS6jl1sNAqvo,5026
+mindnlp/peft/tuners/adaption_prompt/model.py,sha256=ByfvuQfL3AKwLwSZ3rFxRCP-3l6caJzvsiKXq5wrkw0,6652
+mindnlp/peft/tuners/adaption_prompt/utils.py,sha256=K-Gowu-l-fjcS0tvxg8Ehtis-DLjzi7rVz3_ubzW990,4004
+mindnlp/peft/tuners/ia3/__init__.py,sha256=x5eG79TWHxQDgjSNYTByoPy070xIM3FGXfFWrj8L3qU,860
+mindnlp/peft/tuners/ia3/config.py,sha256=S4bQURSGJjAy8QtI7KrF2QvPrqVivf-9u4e461Vcm3Q,5283
+mindnlp/peft/tuners/ia3/layer.py,sha256=y6WPlOIgNW_kIF0PZ_B3qVnin6_c2OK2GmPXbFb8trI,13778
+mindnlp/peft/tuners/ia3/model.py,sha256=EGquqMSdQBNGpli8mM-U6iPMrMhBcOYaMA7WTr8cpzg,16862
+mindnlp/peft/utils/__init__.py,sha256=L1QO_2D1PmTRkBhoGB5Dks2cuSKzis543ZOxaBcBg8g,1750
+mindnlp/peft/utils/other.py,sha256=V8G2QYWgOw9AQQkjkgaN9xUycsvLP1-P91utVNSeYn0,13664
+mindnlp/peft/utils/peft_types.py,sha256=6SHwyopYPJy6gZWrl1-6PXSLnzouxbzo5bp--nfkHM4,1236
+mindnlp/peft/utils/save_and_load.py,sha256=VeEOlOehKj-R-w4v6rLKcU_ihPfN8IvdO26ttSVwQn8,7130
+mindnlp/sentence/__init__.py,sha256=Zf6D3-zWrbdrGmI-Askf3JiAYWm9fKJrU6ePR7VCLyo,690
+mindnlp/transformers/__init__.py,sha256=cVGusml-_NmwJQBzcx1WIUwfQQ8jb7rzQLimqMC5T20,1313
 mindnlp/transformers/activations.py,sha256=vv5oOMKbxT-M03SHCe2Sd01BZ7Ll-IhHWWdCClygqT4,5438
 mindnlp/transformers/audio_utils.py,sha256=w3h2rxRXtFwtoyWBSKHwz7ifHgBjVwonswnNfOxDNsI,33460
+mindnlp/transformers/backbone_utils.py,sha256=i6D55KHDT2o_Ejvdv5voNv4tUSdbC3bSuVvcu6qj82o,16335
 mindnlp/transformers/cache_utils.py,sha256=PwstaYZe7xNWZ_fu4wjNMdswBnavC9da3jeWM4HJMpY,20239
-mindnlp/transformers/configuration_utils.py,sha256=vivC604nF8ev15aGs4QluSL5LLO-igFQYjhVo3TWJI0,35706
+mindnlp/transformers/configuration_utils.py,sha256=YaIkKFC3vElm7AzuZj7_35X9Y8E6rXRy1vK2N4iW0WU,35864
 mindnlp/transformers/convert_slow_tokenizer.py,sha256=jhorBivmFT5WbTzzeds9xQ2FgOFl27XJ2rJeaCA5lH4,53285
 mindnlp/transformers/feature_extraction_sequence_utils.py,sha256=Imxuuu1Jrgq-Gfv4CdavzJcH4Feis1lHRKNvv1SXZpg,18222
 mindnlp/transformers/feature_extraction_utils.py,sha256=l_lxwuYqUsTWXRR_4ypFHMGv8Uh78_jqCQlYK4JntOc,26772
-mindnlp/transformers/image_processing_utils.py,sha256=1P-BO1Hp1hmKiWRs6HB79CkJkvWmCU1xQk5R5XlaMaE,33187
+mindnlp/transformers/image_processing_utils.py,sha256=ahbLEV2PcR-gGIXkLAw3koj7M58eQ7HDDbZ56y0qWg4,34842
 mindnlp/transformers/image_transforms.py,sha256=XAPVvn5puJjymEsEDgtibTkVE-u7tEtVtmBC9foKbJA,32924
 mindnlp/transformers/image_utils.py,sha256=frXrghYl-qR-za86WKvV7vViW5SzSCU_mOTTMOR9meI,29937
 mindnlp/transformers/kernel_utils.py,sha256=EbqQghbUjXweEY6jpaUpSuCu0h5Fuhz3pt6ilwRUdHQ,3025
 mindnlp/transformers/modeling_attn_mask_utils.py,sha256=A2OYYNl6CABjR-NGMWkqx-q1d_RLbxaPgBCD22rOJbg,10957
 mindnlp/transformers/modeling_outputs.py,sha256=EuYy4AB87Qu7U50OZLP61vDmoP1rkODjqjBXyiXi7Fg,111179
-mindnlp/transformers/modeling_utils.py,sha256=9LsRLnXRnX4mNfnDlseJqdeFbpAB2j6vjagF4y04s88,96613
+mindnlp/transformers/modeling_utils.py,sha256=ysh1j7sogrvUs6MAyBpnTfLgonLMlDR1ScJqcPq7R48,95069
 mindnlp/transformers/ms_utils.py,sha256=N7IRToelae2hmwz83fcVg44D_JMwA9ZrEhHdUzl6AdU,8657
 mindnlp/transformers/processing_utils.py,sha256=FdONMo8FHR-imvIpFjK1rwzw7wxuH4mZ6jUERNC0E64,10219
 mindnlp/transformers/time_series_utils.py,sha256=Lq_FOUpKksA0JjkNqoSZ8zjrInHo-fnw-f1rWnQcuIk,6636
 mindnlp/transformers/tokenization_utils.py,sha256=7N7dtuhR0WP4I0_ARGkYZY8XEYPSgCVBS5i5wJNtrZs,44063
-mindnlp/transformers/tokenization_utils_base.py,sha256=5HpfBkwPAaDOLNHWpCPgsI7aiUPKGueS0ikm6FKrCq8,175003
+mindnlp/transformers/tokenization_utils_base.py,sha256=pDNHDwhVv5QDuvUJtY5Nqfs4g-dBvZw5sE5FSURrbXI,175110
 mindnlp/transformers/tokenization_utils_fast.py,sha256=iCnx9OddrLa2umbQ3KMHxmr7VotUbkrh4dMPzxrlgps,37089
-mindnlp/transformers/generation/__init__.py,sha256=b5_aMiadea3qZtn3gXN2WNLyBAGWJSPmv7HunK7T1Nk,829
+mindnlp/transformers/generation/__init__.py,sha256=_ryB6pYlS91CzWdxWdBS3Usa4d3m8xNpYc_izRx6POk,854
 mindnlp/transformers/generation/beam_constraints.py,sha256=uqF7dR6m0sETAXRktv-tsnWubLRLAHWfMpiF-lCxlVw,19732
 mindnlp/transformers/generation/beam_search.py,sha256=22XZl1LNtKMilC7_HYuoO4hOf_7kYhF80s3ZAezLye0,43463
 mindnlp/transformers/generation/configuration_utils.py,sha256=d35ZPNxywHVx75OeqaISmTFN_NqBKtsmn820toourLY,32343
-mindnlp/transformers/generation/logits_process.py,sha256=Am0_Bh-zz3wK6RyzGefCxDefP4dE5mI_p36W3vydJ_o,66891
+mindnlp/transformers/generation/logits_process.py,sha256=nJVdT0yLj55PJGS4Et7mGCGe1SMjKxWVUlxGXDZ_zIQ,67137
 mindnlp/transformers/generation/stopping_criteria.py,sha256=ctgIzoyD3Njf8hZGwfM1HMrCxaaNRPvNJMtvGqB76gM,5067
 mindnlp/transformers/generation/streamers.py,sha256=nfNWWJrnInIDUklA7oX44R9V3Wak2ipHCULVwbT79_A,9287
-mindnlp/transformers/generation/utils.py,sha256=f8k0RkIw2mOnRRUhhX5SCyLv3IgVQf-6M0q8dDIKBCs,252173
-mindnlp/transformers/models/__init__.py,sha256=nSvm60J2ciXj_jgY_MU-sCTl3B7iLYrrf_ADC6rrR14,7060
+mindnlp/transformers/generation/utils.py,sha256=t90vC5oiMEoO6hLPqwMXPpj_ymt6bfBxKScYKyg1cHs,250910
+mindnlp/transformers/models/__init__.py,sha256=yJZ8VF717L5jFrC5o9HnWn9YNbkcursZHyHsO7YqXFs,7976
 mindnlp/transformers/models/albert/__init__.py,sha256=kvD7gpaI2cvbB9GcyoDciROxpWbnbk9-fF0QD9YfOy0,1120
 mindnlp/transformers/models/albert/configuration_albert.py,sha256=vqiWcAlgEShzjGy3qdmjM8C4Vwcj6B57_fpQeY9V-qE,8303
 mindnlp/transformers/models/albert/modeling_albert.py,sha256=Ipttkzs18lFxgyH3BFXqTvu-7WPpDpdUVdW0opn9ZRU,48840
 mindnlp/transformers/models/albert/tokenization_albert.py,sha256=S3tKRWcrOhazlQIpRK6u6puqF6Bz_lcROMWB9FOvTRE,15804
 mindnlp/transformers/models/albert/tokenization_albert_fast.py,sha256=yIM4e2czojHW0JBQoymgzbhpUEidWrrouSik4IkEOdA,11024
 mindnlp/transformers/models/align/__init__.py,sha256=EmzW8tqvGOMH5fO5mQLm_VZqDHdMEOQgaBug6LVc4c0,989
 mindnlp/transformers/models/align/configuration_align.py,sha256=c--Hgtcs46dk85NkSvbwLc312BqZi1xhRiPRpP2XK5g,18320
@@ -235,22 +229,22 @@
 mindnlp/transformers/models/altclip/modeling_altclip.py,sha256=ke3svp38x0ijZx33Z7oorCJ8LRaW2jFJ25HqqmdrQYk,73075
 mindnlp/transformers/models/altclip/processing_altclip.py,sha256=aib4leZrb2IqqUWkSs8e8yNORtx3H46S9j5TaQWETjg,6589
 mindnlp/transformers/models/audio_spectrogram_transformer/__init__.py,sha256=PG0vCiX0VI6m4EIIbY3ELzD9PxEwHF7amsMPoFpYfXw,1252
 mindnlp/transformers/models/audio_spectrogram_transformer/configuration_audio_spectrogram_transformer.py,sha256=2guyWTnmxhejYBmF442WqZIPAUMU58fO7HUJRSOZ_Do,5830
 mindnlp/transformers/models/audio_spectrogram_transformer/feature_extraction_audio_spectrogram_transformer.py,sha256=caBkZhXHWBjqsQjhcRTwAwex82tRWjk1LXQRipxG9io,9478
 mindnlp/transformers/models/audio_spectrogram_transformer/modeling_audio_spectrogram_transformer.py,sha256=Zabej1cLRJWgrCXxubYaF-rcC45rbuTjXpeyqnIuBNo,22723
 mindnlp/transformers/models/auto/__init__.py,sha256=fKMToR-STo2xkAYZtsC_GG8dDMSXu-ZJeM0JBUaYACc,6545
-mindnlp/transformers/models/auto/auto_factory.py,sha256=eMkT0aaz-MOQj8mfoeF3hHgMUK8dP1YDNMUk3uX_OPw,10729
-mindnlp/transformers/models/auto/configuration_auto.py,sha256=VqxrL_XG3G7GOnsQCavO5amqdMa51sQsflRKCZJPp9E,40590
+mindnlp/transformers/models/auto/auto_factory.py,sha256=gnRfwWg-H1hITgIOHaobTW-7EskFomKkeVTw-cVw2mc,10903
+mindnlp/transformers/models/auto/configuration_auto.py,sha256=3iZlNw2BesW0WnRnsNRxa7JdaAob0sDSuQRysLnW_yI,41697
 mindnlp/transformers/models/auto/feature_extraction_auto.py,sha256=P7B2exnsLcIpVPnGQbIIn5atUiRZbDeSbK2XdX2DFzA,18666
-mindnlp/transformers/models/auto/image_processing_auto.py,sha256=WdYE546D6XXbtRu138vgNrYgzoHCE51JqVbDWqhbsrU,20881
-mindnlp/transformers/models/auto/modeling_auto.py,sha256=hIeBeGHZub6hBOw98gqZ6G0h9Cx7QcRyHbIVCj6Ow0k,41547
+mindnlp/transformers/models/auto/image_processing_auto.py,sha256=6NQeRsMCJ_juP5JT4PGwPkDlymSg-Ym7H7Sc1USIdAM,20918
+mindnlp/transformers/models/auto/modeling_auto.py,sha256=Y1eqTBfj_zKRpIPPI9dOTSTX7PgmUyGD_BrxWLiEX14,42232
 mindnlp/transformers/models/auto/modeling_graph_auto.py,sha256=jGgbSmmj1b51_HeHs-LX1067i_Zx8eOd1ZUPIV301G8,12314
 mindnlp/transformers/models/auto/processing_auto.py,sha256=q17nktmWTRcuVT87tBKZIDGx0-wtXnNipCEuvRArZlE,15357
-mindnlp/transformers/models/auto/tokenization_auto.py,sha256=Av1NcuX-CnS5ATDb3dmdQZYl5dJyo0JExhihT6pxZ3U,39882
+mindnlp/transformers/models/auto/tokenization_auto.py,sha256=1gfSmIc0Kacojn5haK2eFM-E2mDUscdGae7l9Xu8gj8,40604
 mindnlp/transformers/models/autoformer/__init__.py,sha256=Ar0f-8Bpn6TP3aUrQ5WTMyyEljWXgwMOZPhs9FwqTnE,935
 mindnlp/transformers/models/autoformer/configuration_autoformer.py,sha256=AsP3cPlPlc_jAveSkE-H9Nic3uKz3ozZcY3I1OPih14,12462
 mindnlp/transformers/models/autoformer/modeling_autoformer.py,sha256=XTJLmXghHmxdvKxkTR1H4ARbTxRZoAsl5GCldvA5rfA,97091
 mindnlp/transformers/models/baichuan/__init__.py,sha256=Xws2zEDi9pKhUg7bZ4zIaEVgaesEevEyF6iV45UBgmg,1028
 mindnlp/transformers/models/baichuan/configuration_baichuan.py,sha256=-MchRqVjs7rH25FoLtBh9QNdGCzsYdGR9unhyxiih6A,2461
 mindnlp/transformers/models/baichuan/modeling_baichuan.py,sha256=2-sgpj9NaCaZFYKVCKQsyv46iKM3Ji3-RdyVHKalbAQ,43284
 mindnlp/transformers/models/baichuan/tokenization_baichuan.py,sha256=lXrSixuRRGZ5_An0WKoaix4UejppaU16PHRQwZ8v5Z4,9639
@@ -266,17 +260,17 @@
 mindnlp/transformers/models/bart/tokenization_bart_fast.py,sha256=9lS92y8JaUA4UBQvgrc8d1KPyOscCvBdjUsT2td-yUo,14266
 mindnlp/transformers/models/barthez/__init__.py,sha256=OHsFgDmFQ2FpRsbPNfe0JF3NmYbsHYH_v_9S6LziGwc,940
 mindnlp/transformers/models/barthez/tokenization_barthez.py,sha256=uaHUNyQpve89ltsCRsahoqyMt7fvjnk-62Q0Lv05gl0,12831
 mindnlp/transformers/models/barthez/tokenization_barthez_fast.py,sha256=V7uSVCsrfu_kQ3wRCg5s6JkWpZvGuuEMdS3j1yBaDEE,8996
 mindnlp/transformers/models/bartpho/__init__.py,sha256=S8rHegymJ-G13xPwHcXotbCID9Cr3-1PoXmQqVFlwrQ,822
 mindnlp/transformers/models/bartpho/tokenization_bartpho.py,sha256=O69zBZqUybJ_SSpy0mfLiOZChqtZ2SFMPQ1RXgLU3fw,14087
 mindnlp/transformers/models/beit/__init__.py,sha256=JI1KTOgr7zSAmvRUAsCcvVwabBoNL-HGrRp-bpVR0zs,999
-mindnlp/transformers/models/beit/configuration_beit.py,sha256=q-wFneOZ4pS1T0kInJUb30VHPf9APJy66CiKgW7NHl4,11381
+mindnlp/transformers/models/beit/configuration_beit.py,sha256=SdCPgZaLbldOmjHVdh4bvbHtXrYvkZFCe56MDQ814nI,11370
 mindnlp/transformers/models/beit/image_processing_beit.py,sha256=K6sQn3gmCdxuLiMS-Nld95WQy11P823O7yrMkyYV564,25144
-mindnlp/transformers/models/beit/modeling_beit.py,sha256=-wqWZt4mOTOLnhkZ4BwYiUZ5cbs6qO-hr4hwwOAShsY,56500
+mindnlp/transformers/models/beit/modeling_beit.py,sha256=3ewqB5F0--SYrxARvwIFAJEWXH0sujkmCmg2OSExLrs,56489
 mindnlp/transformers/models/bert/__init__.py,sha256=JERpcNgqgnLUZmImDBkbEzOlkrHrjssR-wtYTc5ZHMo,1196
 mindnlp/transformers/models/bert/configuration_bert.py,sha256=lLHijn951YQtGhvp7iMNex5YrUyfOUDlCjiPU1nbVE0,2598
 mindnlp/transformers/models/bert/modeling_bert.py,sha256=TnkxM6yABCVzUjIYsw-cAilptZcf81oazsZ2rNw8sqQ,93194
 mindnlp/transformers/models/bert/modeling_graph_bert.py,sha256=9xCeoTYu3pF2NnzI53w07D_Z-bGP1zBAqeYbOE9kYmQ,24981
 mindnlp/transformers/models/bert/tokenization_bert.py,sha256=nUI1W4OJZN5j2PV7f0czwpBMsxkwACMXlJefEwhaqwE,25179
 mindnlp/transformers/models/bert/tokenization_bert_fast.py,sha256=C26fkVpw29fgfzuOqnzG7YdXEodbswGhpKipbRR89vY,14885
 mindnlp/transformers/models/bert_generation/__init__.py,sha256=0gRx9b9OmhUX6xIQ57F-1k2591Lsp3WaTuswUrm0CkU,1086
@@ -299,17 +293,17 @@
 mindnlp/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py,sha256=HZRSfY1FZgJ_IkToYWSOlP2ncOr44vTKC3bPBbPyMLI,8577
 mindnlp/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py,sha256=3dcjB5qs8za4cqgccTr0hXjGFi95cPKKGZKXjpC202Y,134691
 mindnlp/transformers/models/biogpt/__init__.py,sha256=jzfar9P7hYKySKNYNxa7fBWrJvNq9as_-ST5tFXS0Xo,1007
 mindnlp/transformers/models/biogpt/configuration_biogpt.py,sha256=NbAre1ddPv1yxZCwnj3DJxcTJxYyfZQyTkjS0LUsoCA,6499
 mindnlp/transformers/models/biogpt/modeling_biogpt.py,sha256=JPq95S5Fa2xIQMN39fa6lHlSCJgKNSNHu-IIt61xbSM,34793
 mindnlp/transformers/models/biogpt/tokenization_biogpt.py,sha256=gjdHulzti_30uH-o_NKILxwLCWY9Ik-W1B7_rt1HJUQ,13838
 mindnlp/transformers/models/bit/__init__.py,sha256=j3BxO5PLjCnJcs3HpLg8bqtF-A2uV3-MqynsRQxOrzk,989
-mindnlp/transformers/models/bit/configuration_bit.py,sha256=KzJeGU3lm8vAAb2cKBRpTK3wYRDNd07HwLettL_hFto,6297
+mindnlp/transformers/models/bit/configuration_bit.py,sha256=DLZEcaYvoykz8WD27U5htbU_DoMfNitipluUJbJwNLw,6290
 mindnlp/transformers/models/bit/image_processing_bit.py,sha256=SdlSYDfzNvInq4Hw0HcaNbSXfi3OKAmWgMoMSZbim3s,16448
-mindnlp/transformers/models/bit/modeling_bit.py,sha256=haNxYwXtOBfbK6xMrW_i_9YWxrRXKQnsGegZb-T26co,29567
+mindnlp/transformers/models/bit/modeling_bit.py,sha256=V9-6h2fSV0or-Y2XVmk3to46nwFuZr-CkqPJBA2qLV4,29560
 mindnlp/transformers/models/blenderbot/__init__.py,sha256=nVdCXAIJ28xukWT_2daVaiY-CzpQsvlFkTRbdJZ61qU,1174
 mindnlp/transformers/models/blenderbot/configuration_blenderbot.py,sha256=xiF6Dy6uNdiozP2e1Q0EWStbv_tVQazW5SXeVqI-QXM,7560
 mindnlp/transformers/models/blenderbot/modeling_blenderbot.py,sha256=6sZuUnmz0R8oKGBhUh9xvEP1VIVyQkgepQXXoPo7Trw,64667
 mindnlp/transformers/models/blenderbot/tokenization_blenderbot.py,sha256=fRxHPO20rfX_oGTZCWyaVpVsKRgK9KqsP51Q15ns8xI,19111
 mindnlp/transformers/models/blenderbot/tokenization_blenderbot_fast.py,sha256=fRxHPO20rfX_oGTZCWyaVpVsKRgK9KqsP51Q15ns8xI,19111
 mindnlp/transformers/models/blenderbot_small/__init__.py,sha256=c_85gqZjbyENwSRiFNnF4FQCMsAfM0w55PsD1Gi7sbQ,1252
 mindnlp/transformers/models/blenderbot_small/configuration_blenderbot_small.py,sha256=zqmfx-83kwECL8oWB2gG6KHJndLGGDJOh7xiH9gpRjI,7547
@@ -361,30 +355,38 @@
 mindnlp/transformers/models/clip/tokenization_clip.py,sha256=ByfdfLXXm4L9JAjbeWJ5OSRU8S2uPd45dBBc861Equs,21283
 mindnlp/transformers/models/clip/tokenization_clip_fast.py,sha256=d8jQNnEpMyuVXolZ5_rjEhxQU7YfmOxTWyP0DXRmyyE,7387
 mindnlp/transformers/models/codegen/__init__.py,sha256=LFcuhSJcria7XEpEiPiztQYpjmpeoYlOx1_OVFp5xN4,1239
 mindnlp/transformers/models/codegen/configuration_codegen.py,sha256=v_sCH5wjQDvsjblKcx84qxcxi3vi-92iXogTXGT3BFk,7710
 mindnlp/transformers/models/codegen/modeling_codegen.py,sha256=AW2myqA-VtHBXMJjriPL_X3xfze9Bvf_BLAvcAYG8uU,26987
 mindnlp/transformers/models/codegen/tokenization_codegen.py,sha256=_hRtr9UGMbVxmswsj7zDL6jngcv5Oy1UFpUqsHdoVm4,15302
 mindnlp/transformers/models/codegen/tokenization_codegen_fast.py,sha256=xE_wVf-zwGDaqVENYn4RU6aP2bQWdfK2VPUaISOvLTk,10395
-mindnlp/transformers/models/convbert/__init__.py,sha256=Iu5oTT0oUxggtzokfWhIbaS6d9NjsiWOlXVD433StB4,1082
-mindnlp/transformers/models/convbert/convbert.py,sha256=ZMvqx3dbq1s0upQSBSA3H7W5N5l-CnYZo_oH5LqNeC0,47131
+mindnlp/transformers/models/convbert/__init__.py,sha256=JTHuHs4c0JpgtXTv8VoFzpBWHsY_LAVFCB5FBCy51Dg,1192
+mindnlp/transformers/models/convbert/convbert.py,sha256=_EoAWv0kjbbB53tNo6jz_BfuHySbaLvuRTsnuGx5ZO0,47625
 mindnlp/transformers/models/convbert/convbert_config.py,sha256=mh-aos4NRGwA5s8e1R-OFdYvVL4bKzqdu-4ud4w-yZU,3138
 mindnlp/transformers/models/convbert/convbert_tokenizer.py,sha256=Sj4tqPv5rpPEw3PL8_7AKXQrAFdSqR3BzfrZGVTRnH0,21854
 mindnlp/transformers/models/convbert/convbert_tokenizer_fast.py,sha256=7o_J7kWIWI9BAqkLtUOtRDPZhPM7jlazP2bQ31E1Cdo,8790
+mindnlp/transformers/models/convbert/graph_convbert.py,sha256=a3qPltQ-HzTwzjA0Fqd3pThUTAy17bCFFyY2Sa3hwJo,20684
+mindnlp/transformers/models/convnext/__init__.py,sha256=F2Rf2ebe0yOOmK9YeBHFeYR9XTR2DDVljobzNxftOXA,1038
+mindnlp/transformers/models/convnext/configuration_convnext.py,sha256=m1Wc6ZVlxl6-K0s45MMXyklL9-h7SYmuciA1ayN4Smw,5622
+mindnlp/transformers/models/convnext/image_processing_convnext.py,sha256=J4tiJK6o0HqxT7cXOcm4Q_zcrqAe2PV2_9huf7aKXX4,16342
+mindnlp/transformers/models/convnext/modeling_convnext.py,sha256=MVdZL4UhjJepwp_aWa7kGH4AiQUgDkvgcRwWtPDn_Uk,19441
 mindnlp/transformers/models/cpm/__init__.py,sha256=pvKlCDjSWg9cKZ6S6H1Xs8sqlJp3vvIqsqn7IFP41iU,1013
 mindnlp/transformers/models/cpm/tokenization_cpm.py,sha256=t794D8DuhEHnlptM8wX0VYqkYij8etGY-4Sb5qy9DHU,15403
 mindnlp/transformers/models/cpm/tokenization_cpm_fast.py,sha256=7Rz4OfUCmkIMFhVA0Ek_IRoWrrmDxJy7UpHCQtK679w,10855
 mindnlp/transformers/models/cpmant/__init__.py,sha256=inHmfIXlqC803ewRm45j5ZrP49s3Qv8lZiqNcD8Y-Pg,1110
 mindnlp/transformers/models/cpmant/configuration_cpmant.py,sha256=oAh5wLZwRuWnsGHvAMy8wcaUhfByioRoLwf9ILxjwvE,5439
 mindnlp/transformers/models/cpmant/modeling_cpmant.py,sha256=tqmeb2uxb_6drgtBYW0NlwY8OSdswtGkKAN6VgJPCWE,35004
 mindnlp/transformers/models/cpmant/tokenization_cpmant.py,sha256=Ag5DQYU0u13JmkPly7-P6SBPxsqGASDUDpJD4pkkf1c,10166
 mindnlp/transformers/models/cpmbee/__init__.py,sha256=0fDsZnAigndfAignhmNr1hLIQUrXAr2NLU5PcNZw09o,1110
 mindnlp/transformers/models/cpmbee/configuration_cpmbee.py,sha256=Y8Bd_WxfVqpiLhUC6GVnhmlhv-POfirx865u0XrBCvE,6080
 mindnlp/transformers/models/cpmbee/modeling_cpmbee.py,sha256=4DOnDpU4nz379pQei4iGjBmQfWsl0jWEs96913ffoKA,92050
 mindnlp/transformers/models/cpmbee/tokenization_cpmbee.py,sha256=HXD1x0L3FRc0L2jHTZLQIc4uBbr-UHJGNxdISBmdiG4,39889
+mindnlp/transformers/models/cvt/__init__.py,sha256=bszSdB8eJKe3EbWRErm8KZ_bOLku9VcWVXoEEyLe7dQ,890
+mindnlp/transformers/models/cvt/configuration_cvt.py,sha256=g3otIqkJaL1viME0tGMbFj97eW-kN4VaxyZVfm38sqk,6686
+mindnlp/transformers/models/cvt/modeling_cvt.py,sha256=d02BLtOUk2IuHP0Y_goD5hiUfUCLHjo8PtovYpp5ntc,26387
 mindnlp/transformers/models/deberta/__init__.py,sha256=AP2vuCNeHVTicMcE8JSomO2LI4PaA2smyACLoM10dd8,1139
 mindnlp/transformers/models/deberta/configuration_deberta.py,sha256=dgKAPhqMr5rwhrxPAwefsCsLFayw0L5dKl5_RNb7AqE,7765
 mindnlp/transformers/models/deberta/modeling_deberta.py,sha256=myfnYcx2EU-1EQhuM5K83rce-jC4au1rlmrvN0pYTtY,50218
 mindnlp/transformers/models/deberta/tokenization_deberta.py,sha256=0vUwSoxMN6gMJusc_8Hzqv_rv1ocRX-vS3CgKJxYSYU,19193
 mindnlp/transformers/models/deberta/tokenization_deberta_fast.py,sha256=SiAjbT7wz32BvvOHqu9C2XCw4QMd3qMPPXYzVGtXAE8,12810
 mindnlp/transformers/models/distilbert/__init__.py,sha256=9UOCyRL1AGP1WBNrHndMvdy1--XLx6tFSxr88sj_3i0,1168
 mindnlp/transformers/models/distilbert/configuration_distilbert.py,sha256=Ewc6S8J-mq-aHoO5C-gD8rffribh0U75EXoTwTPlO88,6538
@@ -446,16 +448,16 @@
 mindnlp/transformers/models/gpt_bigcode/gpt_bigcode_config.py,sha256=QK0vS0UmyyWbFLq0jQODzM4dBQ3D6Gl5D7qL07D_4KI,2866
 mindnlp/transformers/models/gpt_bigcode/gpt_bigcode_tokenizer.py,sha256=qclCAgzEhozUtPK-uDNm2c3JbwNN7M97UHPqXbdgE4s,3451
 mindnlp/transformers/models/gpt_neo/__init__.py,sha256=QuLl0Obrzen2o8jm8XWEZTlvRJE2oWnrxAa7ntSF0lo,893
 mindnlp/transformers/models/gpt_neo/gpt_neo.py,sha256=BitjfUTlEFXYY9HS13KXdVQByau-PL6wquQrn4HBAfw,31296
 mindnlp/transformers/models/gpt_neo/gpt_neo_config.py,sha256=0Qz7FJuZ3MqTq-QczN2vhY5R9S8x28kIZoBcAKV8tYk,3658
 mindnlp/transformers/models/gpt_neox/__init__.py,sha256=KfxiVAe_PpiRyGWaEW49uqZqSXanfZKmk5iKVoCG_jE,989
 mindnlp/transformers/models/gpt_neox/configuration_gpt_neox.py,sha256=vhqkznrxZlTDajphUo3qgiYlhY17GMMOxQl8DHwXavM,4201
-mindnlp/transformers/models/gpt_neox/modeling_gpt_neox.py,sha256=wGf_YZXtSRN3oxiQg_UKu0rGM-EBk2JG0FAqfRVK1r0,47248
-mindnlp/transformers/models/gpt_neox/tokenization_gpt_neox_fast.py,sha256=luTJMlBdjcLTLudaoQJDzzM3y9zh4gYtoI-vFcIuEms,6036
+mindnlp/transformers/models/gpt_neox/modeling_gpt_neox.py,sha256=mvHzMFhVFvGryelf51S3mAInfNsHcyp8nlqz7kE2Lxk,47109
+mindnlp/transformers/models/gpt_neox/tokenization_gpt_neox_fast.py,sha256=IWoNXhV--f_DCKe-ppFiE-X9jtagol1s_uBtjgPpoOE,10401
 mindnlp/transformers/models/gpt_pangu/__init__.py,sha256=UvGd_s5XbId7sBW_gnm1F3NdvAh1Pl1xmof1u0ayoW4,1035
 mindnlp/transformers/models/gpt_pangu/configuration_gptpangu.py,sha256=UjVnQJh4hR3tOZbUDQmQQkV_WKvhDYQ_VflJrPkdXjA,2478
 mindnlp/transformers/models/gpt_pangu/modeling_gptpangu.py,sha256=hgloqswOUlDIHNamLdXoUPZtZkkYXAVqoqs_ZuIJdkM,22225
 mindnlp/transformers/models/gpt_pangu/tokenization_gptpangu.py,sha256=PI13Fd5ZRpKXJLSL9Cdvrh_7jmEDBgJaKPnS4ZKk0zk,5069
 mindnlp/transformers/models/graphormer/__init__.py,sha256=I_pSp5a91Dgua9d53ufUpZ51lRoO4WsioPJX8jEluqk,1105
 mindnlp/transformers/models/graphormer/algos_graphormer.pyx,sha256=8pF5MRII8qey7iDSBf4V1_vfA6W9DJxMa_NpP9Gc7uM,3633
 mindnlp/transformers/models/graphormer/collating_graphormer.py,sha256=EYQkdGVUm6Bq5X35dJkDuqF00GJva1uoxxtOe1x2n4M,7817
@@ -495,14 +497,23 @@
 mindnlp/transformers/models/llama/__init__.py,sha256=sxwX9nMivuBJzHUCOAhPYfkEedUi-YApLRNl4D-bR8E,1457
 mindnlp/transformers/models/llama/configuration_llama.py,sha256=anVkJSIHloAQb_UyBBR0veTnX9J9iG6456J8elX02Ew,9417
 mindnlp/transformers/models/llama/modeling_llama.py,sha256=3CqxH8AgnqiSTpttRukubftZmqRxtlc0Bj6dCx83uk0,37351
 mindnlp/transformers/models/llama/tokenization_code_llama.py,sha256=l1hq4QigwZqep9PhJjh-2joDMXXVfRJ2a5eYC9D8McE,23580
 mindnlp/transformers/models/llama/tokenization_code_llama_fast.py,sha256=WbxDOF2DwfyDk994nC-ZldFfxXQu0E8o5QoxyjyLZa0,19760
 mindnlp/transformers/models/llama/tokenization_llama.py,sha256=aMMY74eYIdr0IhEXbdTN0s1py9wLP9v86PdzeJ_xWao,22019
 mindnlp/transformers/models/llama/tokenization_llama_fast.py,sha256=YWTYbxgWRhPB4P7-eJeOuomzvHMGqFefew7nBCp3qBg,13087
+mindnlp/transformers/models/llava/__init__.py,sha256=VXpuuNfQpRxlNnAuJ-oisQeqzlVUAdk1ja8jW9zQPDU,916
+mindnlp/transformers/models/llava/configuration_llava.py,sha256=M-7Lz3-zkRGQkaBQn27qwSsDAHzo3b4h69cBUAjyJIw,6068
+mindnlp/transformers/models/llava/modeling_llava.py,sha256=G565xpPjoUlZpXQ93i-H0ybs4ajxsHWMfW2m_-QLvgs,22649
+mindnlp/transformers/models/llava/processing_llava.py,sha256=GXsoj6M2gdtTW8s0OeR2IKZTisKsagsiDZj-Tc7et98,7201
+mindnlp/transformers/models/llava_next/__init__.py,sha256=ttAffiLCgvzVT2q1KkzuqaGzOAAbQzrpq2i-9uM_7zQ,1137
+mindnlp/transformers/models/llava_next/configuration_llava_next.py,sha256=Y1L8jjw2OzGGYw9wct-OTP6DGaXjL5Qi3KOOKhcxcLY,6131
+mindnlp/transformers/models/llava_next/image_processing_llava_next.py,sha256=UvGzGoLIoZHCL-EKn1Y9zqN-EpoqB3XS1HwXDK11mEQ,29344
+mindnlp/transformers/models/llava_next/modeling_llava_next.py,sha256=J-uDT6-HxY_wmj6UOvEGcx-OjzVpF5rXjvWOJInGAAk,29418
+mindnlp/transformers/models/llava_next/processing_llava_next.py,sha256=a78ZUkc9diIX7RxHme3ed2ED4YsU0ebsxY6aTiR_zzA,7269
 mindnlp/transformers/models/longformer/__init__.py,sha256=fjkvVNWfTlZ5pO9aduvYMWqILKU1f3bmcdpJ8WYwTuM,1173
 mindnlp/transformers/models/longformer/configuration_longformer.py,sha256=dwI_L48K_mLI23zKb1pxFJUbodPGjAxAKxfFlKxzsjA,7354
 mindnlp/transformers/models/longformer/modeling_longformer.py,sha256=kftPze-bnseOYG_Ahlx5OaZofoiOhwUE5dXJwS3ESvw,107905
 mindnlp/transformers/models/longformer/tokenization_longformer.py,sha256=3LFybwCZRCzua2s4LxUI9JZrtIR5gj1pjvp5RtLZVoA,19034
 mindnlp/transformers/models/longformer/tokenization_longformer_fast.py,sha256=U2aV-cPPqabRiR6C3jqdhzWINSFuU8rzb_IM_pBFGto,14789
 mindnlp/transformers/models/longt5/__init__.py,sha256=2OVatgQU5Wgf65oVfaLGGdmpLK0RqR1-urnp7rvnO5M,1012
 mindnlp/transformers/models/longt5/configuration_longt5.py,sha256=8qYDDg3-kCc3FWO9M0d67z_h9IrCHBo_MO8GhDxupWg,7520
@@ -517,15 +528,15 @@
 mindnlp/transformers/models/mamba/modeling_graph_mamba.py,sha256=XfpStwzW92fdZ6IzHltHOxz_dyONeBB9zu5E8fbJBeY,20727
 mindnlp/transformers/models/mamba/modeling_mamba.py,sha256=qDrVFKY01aatFTbNr-DERNOhWFNwuV21NJGbixP7Sjk,22627
 mindnlp/transformers/models/maskformer/__init__.py,sha256=b6RZtQQG1fZLGzOGE_ZetHnS5iAeM2Mvpf6REVMF_H0,891
 mindnlp/transformers/models/maskformer/maskformer.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/transformers/models/maskformer/maskformer_config.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/transformers/models/mbart/__init__.py,sha256=_ssqvuKRZ44sFWS3sHcsZpqQi3yQwgc0UWeBDNk79yw,1109
 mindnlp/transformers/models/mbart/configuration_mbart.py,sha256=cy75fQzKnt0dSZpiVwPss99TJxELwFIFoEdpxBTx0NA,3514
-mindnlp/transformers/models/mbart/modeling_mbart.py,sha256=LPtGLZDpKuoFGRoRYzsR1Hkz940tpn6XiYWIn2MOtZg,60039
+mindnlp/transformers/models/mbart/modeling_mbart.py,sha256=I_eEW0EMy5IpZvkJaXh0E-VLeaNvM_WKhkhniAbBAJE,59953
 mindnlp/transformers/models/mbart/tokenization_mbart.py,sha256=oJS5JnmJQ2USccdk2tqjFnc54biDmipZlhWo5MlH0Lc,13994
 mindnlp/transformers/models/mbart/tokenization_mbart_fast.py,sha256=f0AXS8OaeWH-ahEzqQtK6Q0JdTKQQbLS6B58zRlsUno,12171
 mindnlp/transformers/models/megatron_bert/__init__.py,sha256=TMnJuv_NFyKBwrSDF-p9cLKKXTlgx1WnEgfcJR6P8Ng,1044
 mindnlp/transformers/models/megatron_bert/configuration_megatron_bert.py,sha256=S9VH4F8UsHrZX7oRillZKVbeQp_sqx5GJOIIestoKU4,6610
 mindnlp/transformers/models/megatron_bert/modeling_megatron_bert.py,sha256=el0yAszEjAW9dR_YgUIlG8G2pt8Q-s7jTPcc7hY1R4M,72730
 mindnlp/transformers/models/megatron_gpt2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/transformers/models/megatron_gpt2/megatron_gpt2.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -545,14 +556,22 @@
 mindnlp/transformers/models/mobilebert/mobilebert.py,sha256=OVBpkLo3D-f_EQqOo4UGyCSdevAYij54HkfVgn6Ldzk,57813
 mindnlp/transformers/models/mobilebert/mobilebert_config.py,sha256=LaxUPS2K5uIV8vyQHglnKN49I2j0-O5ocQ1ABpYzMHo,3205
 mindnlp/transformers/models/mobilebert/mobilebert_tokenizer.py,sha256=qSVUPDwnKI-0_ijjA-U0PuycIWABc0-9Xtn_-VS7rUc,5687
 mindnlp/transformers/models/moss/__init__.py,sha256=D5pmZF7e8BEl_hR0mDN10hxwltaN8CmVwPf2I9cBC3k,778
 mindnlp/transformers/models/moss/moss.py,sha256=-34YPzU1OnPHhHh6zeIcKxyEj3M7hPmEd2N4VIfwLqA,32778
 mindnlp/transformers/models/moss/moss_configuration.py,sha256=OGS4aHeHZrSJ7yYxBA-ytWbrRFjr5gWCWsiS_y6HkAU,2838
 mindnlp/transformers/models/moss/moss_tokenization.py,sha256=C-9m-aTGYRMkO5D2yWxFgK1laX-miuO0Imf5SU1LCn0,867
+mindnlp/transformers/models/mpnet/__init__.py,sha256=rkVREpIWbAM8Jj7i5_gVJBqMuCk4YMH7ZZe3L2yBeqo,997
+mindnlp/transformers/models/mpnet/configuration_mpnet.py,sha256=g9arRcn22q6MXQ6QNwrpQPM00hRVWbGxwK0ja6mGL3Y,2795
+mindnlp/transformers/models/mpnet/modeling_mpnet.py,sha256=DDdRvN_se-nfmN5r5mkOpNKAOBJMy3aeMwhlne53BuU,39308
+mindnlp/transformers/models/mpnet/tokenization_mpnet.py,sha256=6JtG_8njERZxNpeyvjAtyYWQaTR5FOsw3w2xQrLsors,22784
+mindnlp/transformers/models/mpnet/tokenization_mpnet_fast.py,sha256=ZBKYTumtlvaJWO2Eorf3bQvF4l5_OjwvpvBR_WloR-Q,9861
+mindnlp/transformers/models/mpt/__init__.py,sha256=wIYwmu4BnNtuMrseWKhm-yIGPupcic9h6DG9EdMWNYY,886
+mindnlp/transformers/models/mpt/configuration_mpt.py,sha256=DrggQkD64c6GZB6sazN2z7sPUN8R0OceU6q4tIeNlEY,12049
+mindnlp/transformers/models/mpt/modeling_mpt.py,sha256=AF0w-Sa_kCiolS1jkGhMkudLJDAP79GaOHUQdztAFoE,33852
 mindnlp/transformers/models/mt5/__init__.py,sha256=h8w7lBquHC_xwuAVhC5d6WBZZCk2UL-wY1Yy0Rv8now,889
 mindnlp/transformers/models/mt5/configuration_mt5.py,sha256=9ZuBxldxcEJJ71WEiwdrx2mLNxJhNU0HS6BSeiLZEEo,6755
 mindnlp/transformers/models/mt5/modeling_mt5.py,sha256=rBAmjR1FIWC01CYCYAWn9LyGXAwjQibpX8fhj0dCcw8,81209
 mindnlp/transformers/models/musicgen/__init__.py,sha256=9wmRbv8p6xPKq3-kHmFyVqaedPTrB_zHvEwXSiUKotE,1025
 mindnlp/transformers/models/musicgen/configuration_musicgen.py,sha256=ENhNHSLRFmKUFtReJiNveFXiMu4b8Ht-3H4NrpBszdU,10700
 mindnlp/transformers/models/musicgen/modeling_musicgen.py,sha256=3fClvekkyNTlmlnUdiSBM5y05f8i_dyRwSgdfWO8ll8,110242
 mindnlp/transformers/models/musicgen/processing_musicgen.py,sha256=UFEzkU38C-MhDxiuzIwLK3s9pQtEhHp6OwyNAw5W3bM,5684
@@ -561,23 +580,34 @@
 mindnlp/transformers/models/musicgen_melody/feature_extraction_musicgen_melody.py,sha256=fLU-tCK1FlHF-W6krv04SGnUb4LOpKJ_d7c5k780wHI,15630
 mindnlp/transformers/models/musicgen_melody/modeling_musicgen_melody.py,sha256=2K6RAWadxkJiia0HdC_BirNrrTll6RL0tgh6knK-k4s,106734
 mindnlp/transformers/models/musicgen_melody/processing_musicgen_melody.py,sha256=IX8c1hYh6DHBHuQEm--ngHJXKooWHjbGRERr6oAMtrc,8653
 mindnlp/transformers/models/nezha/__init__.py,sha256=_PkPAyzLAz9gselRav5O46DRJEdVw8sN9-g_BrB_D6o,945
 mindnlp/transformers/models/nezha/nezha.py,sha256=W1bNLGgwpnhT9OvXvTiMLbw-00pTn3c37fdkwPLTTOA,47907
 mindnlp/transformers/models/nezha/nezha_config.py,sha256=O7mIAPzbQESMi06n4Pc59NE6i2TfhUIDPcZ-IIkH5T0,2431
 mindnlp/transformers/models/nezha/nezha_tokenizer.py,sha256=NaXJS5yVYSp5OYLb64eXEwHGOd-NLVVaq7EEPM1ONDU,2953
+mindnlp/transformers/models/olmo/__init__.py,sha256=JV2n43X_V7Suxhkcdz5Po9y-MkJnfgaMtJhjc56A6Wc,897
+mindnlp/transformers/models/olmo/configuration_olmo.py,sha256=BoQJBgPYCzF0HpyI7D8fwXe-7CmptfvG0pUI8s36hP4,8938
+mindnlp/transformers/models/olmo/modeling_olmo.py,sha256=PyuMb-VPrHoL6PQkDsBYwYa0rx15UpluscW0PZnWPrM,39292
+mindnlp/transformers/models/openelm/__init__.py,sha256=1dzlvBCBA7UykNy2-vew5wHVLULC8JUJd9TjoAnc-38,915
+mindnlp/transformers/models/openelm/configuration_openelm.py,sha256=0ZZzlUEntmj9mqDhVgbI2gtbMU6ErTh2VXTiBUfCkm4,12715
+mindnlp/transformers/models/openelm/modeling_openelm.py,sha256=ynS-ilAmtG71Mk8vxs7C0tigxK2hMG8AIzlTncilXCw,35961
 mindnlp/transformers/models/opt/__init__.py,sha256=9hRJbyk3_rziUsPgFBO8BqgUDAfL0rjGOsFqwIeARpA,891
 mindnlp/transformers/models/opt/configuration_opt.py,sha256=Mtj7zDkDq2-bgiMmHCVOCn7VUUvNv9ANuQ73MaSWHgw,7373
 mindnlp/transformers/models/opt/modeling_opt.py,sha256=Si8x61l-I_uLbhFwR1uAciJ8iWS2JViiBJA38zoeI4A,47645
-mindnlp/transformers/models/pegasus/__init__.py,sha256=XAldIk1mOYXQhEDfYmb8pSHjlqkhlmF1G23I1HXWItk,943
-mindnlp/transformers/models/pegasus/tokenization_pegasus.py,sha256=_HPDggI4GPETopxDOi2-3iJJXocgQ-zJ-0KOT6n8jG0,13184
-mindnlp/transformers/models/pegasus/tokenization_pegasus_fast.py,sha256=32YFI9xO2RzIf0Y0RxNoEjIHvc9s7Z37ftaGrbQM3Lk,9982
+mindnlp/transformers/models/pegasus/__init__.py,sha256=ei5L0SaREC23P38zOfpXb5X7ERZHvJzdwon5ihDNbjo,1140
+mindnlp/transformers/models/pegasus/configuration_pegasus.py,sha256=Lcc-lqUjY2WXho6CTmuqgainni8YR8a45c0_io7MJ6g,7830
+mindnlp/transformers/models/pegasus/modeling_pegasus.py,sha256=CLiqR8m1beQJ7iTe5ERlzB4s3l68DLTMlq0nMhRtjVY,71916
+mindnlp/transformers/models/pegasus/tokenization_pegasus.py,sha256=9tKiXVJeU58FFs0ETK4873Kx9IFyVyQ57O_SzdLvRlc,13230
+mindnlp/transformers/models/pegasus/tokenization_pegasus_fast.py,sha256=GT5o58Q2qj9bqq071NEYC1vLrKiSEykgPy1vJVSLGqo,10028
 mindnlp/transformers/models/phi/__init__.py,sha256=xohCbnuGA1QJyRO-fYzlkT1Ky3D4LmUavD9UlBTuvZc,892
 mindnlp/transformers/models/phi/configuration_phi.py,sha256=nK-f7kqmAzlYekcHGP-GpnBAetJWCPx6QEXxjQPNg5M,9266
 mindnlp/transformers/models/phi/modeling_phi.py,sha256=9SQkQvBZHRvw6tfY7PMoc4NOCIMkuKxU-I-6tODTWxQ,42961
+mindnlp/transformers/models/phi3/__init__.py,sha256=3jQzJ5_Kp-XzGsJyv6TY7m4xNYoykFeO_afpr9cZVQs,898
+mindnlp/transformers/models/phi3/configuration_phi3.py,sha256=oN2PyPayDRhMwhavD2SLZxvHmiEcx-EoC9e0DdsiJD4,10417
+mindnlp/transformers/models/phi3/modeling_phi3.py,sha256=tukzOI1Lh26ZyT1P2qI5yI93C23MrC0KrtY5fdU2cIQ,44874
 mindnlp/transformers/models/pop2piano/__init__.py,sha256=7lKCKxlIOeKmVIYCC5puHZx48LaV1wbsGzr9WA7JtDs,600
 mindnlp/transformers/models/pop2piano/configuration_pop2piano.py,sha256=FyLM2DbPqGbD9ny0WAUi0ZrInV8Apj7H9_cLYDmhRiY,6241
 mindnlp/transformers/models/pop2piano/feature_extraction_pop2piano.py,sha256=vuj6syO2M0XmKPXz074vsN7m9m7J9ZPwow8w8Gh_jsY,20121
 mindnlp/transformers/models/pop2piano/modeling_pop2piano.py,sha256=Jax5wTpgipJ5l2LOhUsjagSuTVciF9ViuNHdVO30cFE,60570
 mindnlp/transformers/models/pop2piano/processing_pop2piano.py,sha256=NTaPAYCArR2vkfmN2tse4TzJfcSi9OcMokTpCAOqexY,5589
 mindnlp/transformers/models/pop2piano/tokenization_pop2piano.py,sha256=ddr8rAIYIT0nnW58Rpb7kvvvFcKGUlTPQVhgvVCOdKY,32281
 mindnlp/transformers/models/qwen2/__init__.py,sha256=A1z40XNhUWVouukydmYIEMkJiQ5R8-VA6v2VMjmIYzw,1108
@@ -590,52 +620,73 @@
 mindnlp/transformers/models/qwen2_moe/modeling_qwen2_moe.py,sha256=j_SgqoVZHRz-GITnXV6RZNcRXFx9xhlQwVaH9D01RzM,45282
 mindnlp/transformers/models/reformer/__init__.py,sha256=JBrlkdAEhjZnqSzlb0Nj3UiRt4SvdO5KdI-r4c3P7yU,1148
 mindnlp/transformers/models/reformer/configuration_reformer.py,sha256=EcUSxvfhD8iyg7EP4wV08QwvT04zn0TxWAfaB2o1Dzg,13575
 mindnlp/transformers/models/reformer/modeling_reformer.py,sha256=n9FZ9p3UgLkMuTsJYtE5RySMW1eWGKC2cOnG-0LueJg,107482
 mindnlp/transformers/models/reformer/tokenization_reformer.py,sha256=aWODuAwaFX3ri0JbmuUB7iGhd1ozIEFxqg6IUhMYnnA,7289
 mindnlp/transformers/models/reformer/tokenization_reformer_fast.py,sha256=yE9t0rpSvJj8Gxu5luAqnllqzBQXAmDREqJg6pTnXSM,5004
 mindnlp/transformers/models/regnet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/transformers/models/resnet/__init__.py,sha256=uTd9LprQ8zZiifq9MgRcKKkVeB-5wEJ8WmR6Js3kw9I,905
+mindnlp/transformers/models/resnet/configuration_resnet.py,sha256=9fGe4nEr56eLX-50umxhG0ZIj5Di3aYESgJX34JW9CQ,5515
+mindnlp/transformers/models/resnet/modeling_resnet.py,sha256=JfJL7EDD-tlWJ-G8-2XSMtwsvuY08I57k-OMmN4BWLc,16938
 mindnlp/transformers/models/roberta/__init__.py,sha256=-1uT5s_1QvcBVwoIuzH5noh8Oqam58A-kjy-wR5yjFk,1133
 mindnlp/transformers/models/roberta/configuration_roberta.py,sha256=lRytCf4bsbixEKecY5I0YNQVEwHGk-U0g_VJk_HKDg4,2420
 mindnlp/transformers/models/roberta/modeling_graph_roberta.py,sha256=TaOJIrjGwIhMNjdr85m4sljIerCQCBXPKT7OuI-FYSI,12078
 mindnlp/transformers/models/roberta/modeling_roberta.py,sha256=5pDEbF56D9u-g41czcg5qM2qiUI9NyKWHEY3GcGqT1E,60971
 mindnlp/transformers/models/roberta/tokenization_roberta.py,sha256=sybkJ_yNIKtwp2U9R_A-CweayEPSLKaFHZSUM06XmUg,18177
 mindnlp/transformers/models/roberta/tokenization_roberta_fast.py,sha256=c8TYS3H45EJNOrf1_QtaxTlwVW4__5jLU6ZnjTJXFC4,13885
 mindnlp/transformers/models/rwkv/__init__.py,sha256=CBnS5dn5eB0mgBcvieMr7GQxArgiy-52btb6g81r5k0,995
 mindnlp/transformers/models/rwkv/configuration_rwkv.py,sha256=NpAYyaOA9hjJAoMSkZXRz60ktjc8GF2PFfniWfG47Lg,6303
 mindnlp/transformers/models/rwkv/modeling_rwkv.py,sha256=GKQjWxzpAXErvyHprCW64WMz2bQZ-aechPN8-BFcRPk,28881
+mindnlp/transformers/models/sam/__init__.py,sha256=6KwjpG8CrQv5lOLNkY9LLBtXOztTXU1tOsaw71azmLg,1078
+mindnlp/transformers/models/sam/configuration_sam.py,sha256=rgQL3R4SU-JlIqD-K8Qe-68lpx1TIkTY4C6YMrq4ekQ,13877
+mindnlp/transformers/models/sam/image_processing_sam.py,sha256=LWv1HLRZEVpROwAf3gnGMqQQan0Zxgu2V4X675x2wqI,57684
+mindnlp/transformers/models/sam/modeling_sam.py,sha256=_QsGvY-GNVcmsGXCFBHLkgVLIByO2Z4ZSTyitIf50Wc,58327
+mindnlp/transformers/models/sam/processing_sam.py,sha256=WG_jthrk5ShaXPR25xX8qA6_KQ3rDk5q56lcdFKVj-A,10115
 mindnlp/transformers/models/seamless_m4t/__init__.py,sha256=wrRuR7nef-nJIQ11iw25TJyexjmJ9cs7gslhgs3EdVw,1459
 mindnlp/transformers/models/seamless_m4t/configuration_seamless_m4t.py,sha256=c9srxtlsDzYks60TQYnHrK2KIVQmPSMalZZ7Nh7kCPk,23758
 mindnlp/transformers/models/seamless_m4t/feature_extraction_seamless_m4t.py,sha256=3RUmWcSJ-V36M6bsGh9NynfhFVZGy7ERG-kONR-9NhQ,13061
 mindnlp/transformers/models/seamless_m4t/modeling_seamless_m4t.py,sha256=ghzAbj8OL1mCDeXTZutM0cMc61HA3R7UfM_eU6iVooM,189385
 mindnlp/transformers/models/seamless_m4t/processing_seamless_m4t.py,sha256=rrcs8-mM1ryX-YrLEzTcBEwyHh23vGwv0lhYCJTerjY,5891
 mindnlp/transformers/models/seamless_m4t/tokenization_seamless_m4t.py,sha256=EjBcevEuM149D8RFk9Uzg5dXElhM8GkzaAlymG8McCg,25979
 mindnlp/transformers/models/seamless_m4t/tokenization_seamless_m4t_fast.py,sha256=8FMa3pyqY7-sfLFbCMJfK1GXyGKcvF3Pec-mdubCOZ0,20489
 mindnlp/transformers/models/seamless_m4t_v2/__init__.py,sha256=N2Ms8MaxxzdAJh4Lf3p6LCiyZ3_C6g2MfPcj-G0qq28,974
 mindnlp/transformers/models/seamless_m4t_v2/configuration_seamless_m4t_v2.py,sha256=cStoJictXdLbsAcXT3qeSMcxXj7fEPAlPEE0vFsmj4I,24474
 mindnlp/transformers/models/seamless_m4t_v2/modeling_seamless_m4t_v2.py,sha256=4X8IJD4bj5jVKmafHWTgfa1kx3QanvjaphcKdTUrNss,211331
+mindnlp/transformers/models/segformer/__init__.py,sha256=5twTi2lBtLZBfrYw7pzvTJYGwGEg_U74nQhkES2macM,1053
+mindnlp/transformers/models/segformer/configuration_segformer.py,sha256=UC8qCDjedGlt4vkeq6c1p_g-1ELAsxE_H3KkMQMmWV8,6793
+mindnlp/transformers/models/segformer/image_processing_segformer.py,sha256=ZDEfWuVeSnMVzq_D7iQZxpBajIwTItvKxU2F5b8r83s,23450
+mindnlp/transformers/models/segformer/modeling_segformer.py,sha256=911964BuCTa9ls-bh1K6tclsn8jyoCxUEmvDt9ICLT0,32442
 mindnlp/transformers/models/starcoder2/__init__.py,sha256=UmUL0F8INx05ja3CIuZecYzsi3GpMUiVuFali50rQzA,934
 mindnlp/transformers/models/starcoder2/configuration_starcoder2.py,sha256=sLcdqFcpaE_PvgXPcJxyjiXOJhQKOav7JgM1CGLicP8,6919
 mindnlp/transformers/models/starcoder2/modeling_starcoder2.py,sha256=cTee3GkO-x_nPvVt2oiW4F6kMfeRGtTSgbGpKpHsVvI,36584
 mindnlp/transformers/models/t5/__init__.py,sha256=rCYTY2eSH1OB8f5feb4MoyVwyyDyq1qgMG-GqfMojYk,1171
 mindnlp/transformers/models/t5/chatyuan_tokenizer.py,sha256=mshANadj5d4B4XDeYPBYuxk_nN0J_Y7hdsDG2ZHl0-I,4419
 mindnlp/transformers/models/t5/configuration_t5.py,sha256=AQA-VvnksX6N0zFwM9qBP-JdvVQv8syqgQCddnVb3ZI,6772
 mindnlp/transformers/models/t5/modeling_t5.py,sha256=zEWDVtRutUKsLWsJV8umlYUlz6WRfdF0Hn5eRVgQ3Ws,70759
 mindnlp/transformers/models/t5/tokenization_t5.py,sha256=Jh6Y25FoHsguu2t5I19KQxu6B8Coc0EIKKlE7_0mk8A,20403
 mindnlp/transformers/models/t5/tokenization_t5_fast.py,sha256=OYiqM4eQwKrICF5SXwZtgD0MtPZZkF2WMJPRssLZC90,10806
 mindnlp/transformers/models/table_transformer/__init__.py,sha256=pENDaP1fNav394vPX685cEL23ZbqSYV2l4wp_Yud0kY,694
-mindnlp/transformers/models/timesformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/transformers/models/timesformer/__init__.py,sha256=SdjrssZNLRnLKIn0qWpE8ng-YvNtfvr9AOVGVYeT2sw,1061
+mindnlp/transformers/models/timesformer/configuration_timesformer.py,sha256=J3KHoRvHv3A_yTh8PMOmdPnWfFVH4i_5UbMMHP59Tmw,5818
+mindnlp/transformers/models/timesformer/image_processing_videomae.py,sha256=VdK3jWMIaUQ6DcawmcWCepfgoFSLcI6Czy6t7ZiVQgo,17146
+mindnlp/transformers/models/timesformer/modeling_timesformer.py,sha256=5-vyxFwnaPR4hEBxuZPjjqpeQNZK-mKb9W1pGNE8NdA,33020
 mindnlp/transformers/models/tinybert/__init__.py,sha256=e3pPmmiTOu7_rHm_rJb8diDwW8pvQuv5feDcOjmR_bg,879
 mindnlp/transformers/models/tinybert/tinybert.py,sha256=3bhOQFWOp01sFGs1J5KqSCQnp8GHe8B1KFvOJ-bbuNU,25866
 mindnlp/transformers/models/tinybert/tinybert_config.py,sha256=509kbrtOtD_x02BXWoBzg5Ey7dNrg1klkeX8EN1Jg8Q,3520
 mindnlp/transformers/models/transformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/transformers/models/transformer/transformer.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/transformers/models/transformer/transformer_config.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/transformers/models/van/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/transformers/models/van/configuration_van.py,sha256=PKEpz4jEmbgZX_2jU_IP8OHXZH6XwVSreo29EsOq1jI,4682
+mindnlp/transformers/models/van/modeling_van.py,sha256=2uHDTE8NVfYP9E03fdayV2_PJmCqKpA7hd5xj-aLxNU,18894
+mindnlp/transformers/models/vipllava/__init__.py,sha256=WbT-Z8eV4gGp8LPFFssa1B0_UY0Y9ueA1Fce2RGSzgc,895
+mindnlp/transformers/models/vipllava/configuration_vipllava.py,sha256=-_Wc-D1a2RfSHP9QNDzzHNAssQEHH8IojwhyGoV_kVw,5740
+mindnlp/transformers/models/vipllava/modeling_vipllava.py,sha256=pYRO6RsWWcU8r4zpKnDm2AwFKNVlhiY6EgtevkT5yb0,29912
 mindnlp/transformers/models/wav2vec2/__init__.py,sha256=TtgrXpRT-Zm_FBVBs20dazrP8FdETRav4DLYM-rNtak,1598
-mindnlp/transformers/models/wav2vec2/configuration_wav2vec2.py,sha256=NOnTCmQJHnoLqmzmaCX8mJxhfmQXiMD_KFcGtnDnj9w,20372
+mindnlp/transformers/models/wav2vec2/configuration_wav2vec2.py,sha256=udbqhV1iDwzJ4FANXgPnn7f57MNPc0BZkeJJYtZAA-4,20370
 mindnlp/transformers/models/wav2vec2/feature_extraction_wav2vec2.py,sha256=gR2mB2UkETEp-PnDhSfs9QTefdaiHL3mJi98gpq1_Zw,11553
 mindnlp/transformers/models/wav2vec2/modeling_wav2vec2.py,sha256=VcrLl69Uj80QaqFDVHB3843qtO1jx-0IvF2ZwcC_VHU,97015
 mindnlp/transformers/models/wav2vec2/processing_wav2vec2.py,sha256=g9Qxk1gjmF75hI9HBUh8SL2lPB0cFYuOnJ0tat_fr5Y,7177
 mindnlp/transformers/models/wav2vec2/tokenization_wav2vec2.py,sha256=bIoLwyb3h4H2iY1YSApCmk3ZpPHMaA8vM1dIFYCLhQs,36485
 mindnlp/transformers/models/wav2vec2_with_lm/__init__.py,sha256=K4OXZaw6n4DMy_QRa4qH3RGtuEaMuDzgummotpikmTs,860
 mindnlp/transformers/models/wav2vec2_with_lm/processing_wav2vec2_with_lm.py,sha256=QQ3mfOYdW_cfcivaYG8VzkYOUGtBLqy7ryf7z3iySuo,29591
 mindnlp/transformers/models/whisper/__init__.py,sha256=AHkRyPcVBavgLNHAjwAStTlcG8PaITgua4GXNBTe44s,1356
@@ -649,104 +700,65 @@
 mindnlp/transformers/models/whisper/tokenization_whisper_fast.py,sha256=apolzLRPay-9NGwkZMi3dNtlI5-A3PlWgoz2vhXbpAs,32375
 mindnlp/transformers/models/xlm/__init__.py,sha256=CYV99yz0jJAQRrdwPEgjFtB4X7i5ThOfOqtS8ZTKviE,983
 mindnlp/transformers/models/xlm/configuration_xlm.py,sha256=3XC1OGueoW8LVPkRLZFa_eYPELvwTrrnJmLUSyRwElo,11328
 mindnlp/transformers/models/xlm/modeling_xlm.py,sha256=Tv6HsmwkjoCZ_fjSKN1Rad0zrmMkw0QoR_mnJ5_D00Y,46629
 mindnlp/transformers/models/xlm/tokenization_xlm.py,sha256=6bqkoiJQvurtOtZzQ7G0RgJm5eKkghVk-5Cw9Ekqnuo,34991
 mindnlp/transformers/models/xlm_roberta/__init__.py,sha256=19WdzbQ85JEp76zYsqyq7629mKrtPZFk1h-9OdkvghE,1192
 mindnlp/transformers/models/xlm_roberta/configuration_xlm_roberta.py,sha256=zWack7GDUw-p_H_jvhtFyPYhS2RvniTU-0fvJAiVz0E,6980
-mindnlp/transformers/models/xlm_roberta/modeling_xlm_roberta.py,sha256=QjWiEK_mtbqu-sHFbn0q7rVoojaznGAnOxFBehyITog,63314
+mindnlp/transformers/models/xlm_roberta/modeling_xlm_roberta.py,sha256=IpS1gkTwyuQqUMehgxtGsXg-nDGqubl0SPugpqm6yJQ,62507
 mindnlp/transformers/models/xlm_roberta/tokenization_xlm_roberta.py,sha256=UCy_KMjTgBUzlDrx94Il8TtL7kQ8hCV2WnKVbsrp5Y4,14289
 mindnlp/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py,sha256=4vGn2z6bOySEgXfhViM1QPthAc-tfOs4pHkJOCN3z0U,10433
 mindnlp/transformers/models/xlnet/__init__.py,sha256=u8gHvTfnYGl7gAHlr6kwZSoT4tihza8PoGdIBpOTSlY,1109
 mindnlp/transformers/models/xlnet/configuration_xlnet.py,sha256=Xq9aQYkwwbCFWzs_yBVi03lVG0yCk7UjfX38KDjxtVI,4735
-mindnlp/transformers/models/xlnet/modeling_xlnet.py,sha256=0si1Htl5IOaxM6A-4gmyBPNY24drEhZ9m26SfBo2pcE,85973
+mindnlp/transformers/models/xlnet/modeling_xlnet.py,sha256=zIMi8owbhCzk35TYSKvEuapACnWvxUMQEFk3MV5R9yE,79968
 mindnlp/transformers/models/xlnet/tokenization_xlnet.py,sha256=ZzFVVMz7W93XAtiSS4nPDZm-aT6WsL6tpg1rQjY-JUs,16395
 mindnlp/transformers/models/xlnet/tokenization_xlnet_fast.py,sha256=JEEfMSrnxbb9XzQRVooLW1oek63CgTuak0h8Nx6Kt9g,10222
 mindnlp/transformers/pipelines/__init__.py,sha256=f_l_LRhYEAZnvj39ulSyuSVUPIDHI0M-qavu9RBNIoY,26016
 mindnlp/transformers/pipelines/audio_utils.py,sha256=yDcbQLkIoZTQUuPXXuAPaIUQeFnIexJOqQe_DR-enig,9793
 mindnlp/transformers/pipelines/automatic_speech_recognition.py,sha256=e5C0iMGYB8V6y0zeWvwdkcw3A6FH_DEDuV0c27mhSeE,37518
 mindnlp/transformers/pipelines/base.py,sha256=bZV_FGWncZJry29bkhA5x-GIeurTNy8UVmi9EmdAuDU,35984
 mindnlp/transformers/pipelines/document_question_answering.py,sha256=5_Nim0IhGVUOjw2sdVEASmfNzmsAdPvU69s10uwe0Ls,27144
 mindnlp/transformers/pipelines/question_answering.py,sha256=UFDwjxbU_k1opZ6Ep5ifQxbhQpDjXSjRDdXSvVJMAZs,28511
 mindnlp/transformers/pipelines/text2text_generation.py,sha256=xbOlhrXcdm_6mG1N1tRr6nCMrVajbEXJJJOAHpf37zo,17651
 mindnlp/transformers/pipelines/text_classification.py,sha256=IGwVFY_ViW3tiNsiLJA2tVkfBr_yZkis7_u72O0mPvk,9640
 mindnlp/transformers/pipelines/text_generation.py,sha256=zoHFHgWZ-UPrX_2FZcfylVfth2zd6JIszAcHaev5q-U,15366
 mindnlp/transformers/pipelines/zero_shot_classification.py,sha256=rDtCJmMD-o5yaShFssyokSwRhk_4gggr38wLzXQtN4g,13013
+mindnlp/trl/__init__.py,sha256=-HpIKoAAyC83jWs6__D560rrrzIlZrE2V9rBbimXW8E,717
+mindnlp/trl/core.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/trl/environment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/trl/extras/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mindnlp/trl/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/utils/__init__.py,sha256=Q1yo5WvMBnr_PPQeiTvVsaevg9cvdNF7mfsw7afxgQQ,1510
-mindnlp/utils/backbone_utils.py,sha256=i6D55KHDT2o_Ejvdv5voNv4tUSdbC3bSuVvcu6qj82o,16335
 mindnlp/utils/compatibility.py,sha256=NIPsQaQQtunubod3VEKk5u9yvEvqORCsUtSv6qUoSls,1458
 mindnlp/utils/decompress.py,sha256=luC41yt5cms2LgnrTxRDKoTzG7tjBxRwFZhhx8fi1vY,2916
-mindnlp/utils/download.py,sha256=c532Tso8Hc0gRsv6Vk1CbPjAAYxmxko9YCUMUpDLqfs,32202
+mindnlp/utils/download.py,sha256=lcVlyYcg1VdocfVvQwu_2GEq8RtWcEjBWfu1rwPs6ZI,33061
 mindnlp/utils/errors.py,sha256=EL0gCowHpOXiei23tOTRMMbTOVEoxKW1-ZDIb7BGXhk,12029
-mindnlp/utils/generic.py,sha256=hyHbSGz5fxBy5Ur5kjYPpUGODEWatNpaxrvCGFq22QI,11747
+mindnlp/utils/generic.py,sha256=BZqrzEYJLy3Cm31kpZzWjTsPTU3ZDGBtWnT1JeSpJpI,12652
 mindnlp/utils/import_utils.py,sha256=SJvtG0td-4M_s-ajBeCO7MiXsbKQoBFtGdqkBEmBTlA,14008
-mindnlp/utils/logging.py,sha256=podm3st4jOwTcQ7H1O2fuHvh93XNECauu11MaNXdFoE,11478
+mindnlp/utils/logging.py,sha256=bIb5z9TdKKDzsrG2ugkcOKNw7_9va_7fG3vJN_oW0Y4,11589
 mindnlp/utils/peft_utils.py,sha256=baZaj7HcDBkvCYK3A9cEpjjR07VexYEisFRbonmFBtg,4451
 mindnlp/utils/save.py,sha256=EtnCwtbFWfrBGtlPo1UK-F5IZinp98Pc8RhyGoR5T3A,1898
-mindnlp/utils/serialization.py,sha256=RLhILVf_CrRFJOjs-D2eDVABRyvRsgIQ5XM73BgmrZE,21582
-mindnlp/utils/testing_utils.py,sha256=xezyGUublDJSOQr97Zx86hDS08BHDpZiBudpISBM0T0,50268
+mindnlp/utils/serialization.py,sha256=OgkpNmDqxAN3RBdDJpAjvEm8aJOUUChD1nGgwBcxK4M,21980
+mindnlp/utils/testing_utils.py,sha256=H1ODIqkzlAjp-ARwkYEX5HkQv8c9XNWxmppiAWc2yL8,51172
 mindnlp/vocab/__init__.py,sha256=gs-jacpF3faHAH3SmDh9OqguGI14yVHHCFbKJI3vbi8,712
 mindnlp/vocab/vocab.py,sha256=DFK0c508tVTGjs1Tlc0BxN-VdULS-XLjTHm-2w3PG0E,11522
 mindnlp/workflow/__init__.py,sha256=xh07UUH2_UWGmuy8sGt__xC1pZqEGegnyjK17PKfHks,768
 mindnlp/workflow/utils.py,sha256=pAykV-PnUlQISmBFn-9HttI3mK77DU4Z8nUUGKL9VC4,5813
 mindnlp/workflow/work.py,sha256=Ukrvx7lYYZf2v2qPmPJ5Ug_mKAH7-hwQYLTMvqYLb1E,7577
 mindnlp/workflow/workflow.py,sha256=3Z6rq8tKdHL1j3ggzZ78U7YHQYRrBRC8ubZwxDRbpVQ,7103
 mindnlp/workflow/downstream/__init__.py,sha256=oSZxbB24ULf2vzEpwUrGU3Ufe1rBSVs9O4pY1HvU2Ug,757
 mindnlp/workflow/downstream/sentiment_analysis_model.py,sha256=2arUbL4sv96uybretuy8YZhUGyUxVp296eceNELUn7k,1557
 mindnlp/workflow/works/__init__.py,sha256=qRcg5U1kyjt91rsSTIEczV9h75jMONpFdlRDMC8H5G4,780
 mindnlp/workflow/works/classification.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/workflow/works/information_extraction.py,sha256=qu3woCpgaWgSLTjuPe5tNZUiaelv7AzjCS1gqb2iujk,26028
 mindnlp/workflow/works/ner.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/workflow/works/qa.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindnlp/workflow/works/sentiment_analysis.py,sha256=t6J1OV83_PYH6ZLwXi5-KnPkVAkhvjMVFC_LJq76ooQ,6032
-tests/README.md,sha256=7ko9b5GA-TbkaZ6KC4F1o6RAhVioX6p9yIfwq17VyxY,65
 tests/__init__.py,sha256=lwey9xjqqTeDK1QXjlJjsMNPpVGJsHa192sadlzh7vY,708
 tests/common.py,sha256=t8sKSFL-uq-6P8abw6vbqT6IGOKuUa3cW_DFe596ztI,147
-tests/pytest.ini,sha256=mwKd8Rw5A7TcFvEPZyIny2EN5a1ijYa3y2Y2NRL4u_A,129
-tests/fixtures/add_distilbert_like_config.json,sha256=7OalygSPuWJc1_jeWSm6ffSP6e1BqXovduWdUm0oBm8,504
-tests/fixtures/dummy-config.json,sha256=rAoPGa_mBX5B3J9exnOu2Cbt1TIvVf_cx_pWKoJdRcI,29
-tests/fixtures/dummy_feature_extractor_config.json,sha256=CSr4ZqiObQiBe8mDiRy8P0Q1xcPpa-maSW5FsqugMgU,101
-tests/fixtures/empty.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/fixtures/input.txt,sha256=wKHIThBAG0BjPeoEcJki4Wt2IuJyMXzXdBRc0gmKGZM,52
-tests/fixtures/merges.txt,sha256=1MC_s0hAEZon430exLBJpm3I51vfI82CtO8OyCEb8QA,36
-tests/fixtures/preprocessor_config.json,sha256=twMYYFdVbijNESQlAQJPawUpHfFy764mtojqayOliwg,100
-tests/fixtures/sample_text.txt,sha256=UgWq-pCvsIQbJLBctGE0XjaSqF2OqAJ9iTWvED_VxhM,4394
-tests/fixtures/sample_text_no_unicode.txt,sha256=X3DKBj6or4bg6RhHjSDMempmgjpLB4xLWaA9-X-gBUE,4284
-tests/fixtures/spiece.model,sha256=_vsCtmemxcL-J2AtKOX7NCj2aricfW84jnyNRKAtAzY,760289
-tests/fixtures/test_entity_vocab.json,sha256=qlR-IoRgUgkJ3nMJoenEfn2hMxQFhbCg-g7bFJ1wyvA,76
-tests/fixtures/test_sentencepiece.model,sha256=jf0erkUiKBsbg56rh3p5G-_sehZjpByBTHfZyJx0jy0,253154
-tests/fixtures/test_sentencepiece_bpe.model,sha256=xN549dEe4JFBFl0x2n2tl-gJ3W7ntSoMvG12qXMCgoY,251527
-tests/fixtures/test_sentencepiece_bpe_char.model,sha256=f8xI8-Il9iexZB20EM6wyGSb0rDJguFQsD-L43KKtWA,238473
-tests/fixtures/test_sentencepiece_no_bos.model,sha256=bzr5fC57xR14HnRAqjPe7n9ILqyBnSP9JK-A57TOJkY,253134
-tests/fixtures/test_sentencepiece_with_bytefallback.model,sha256=xh7M5DNp_DurlWZGTw5x86113CMZparcKlYePjElAuM,270096
-tests/fixtures/vocab.json,sha256=7dBmkVu-INEOyc18aPhE6sXzWm00sAST2GDDYibElRw,228
-tests/fixtures/vocab.txt,sha256=hZD_VOmhXhbYhOY9GKbKh1sztsF1_-dsbgtVwvTcmp8,85
-tests/fixtures/tests_samples/.gitignore,sha256=gTH85GETNNiO8zZ8BZ5PTOAZlzTtucwxtGfu70Tb4uU,52
-tests/fixtures/tests_samples/COCO/000000039769.png,sha256=z288S--hSHMsdFPg3lr6sA9oJCdDX-rS2IsHqWFc2sI,694498
-tests/fixtures/tests_samples/COCO/coco_annotations.txt,sha256=WLXasf4Pi7SX5-TDY7tlNN7Qv9mIO9hEm-T8Eut2imM,4075
-tests/fixtures/tests_samples/COCO/coco_panoptic_annotations.txt,sha256=dqssr0ea90JJ3yr3nVaAaIMNLUu0krmgwGMD-2IYlaU,555
-tests/fixtures/tests_samples/COCO/coco_panoptic/000000039769.png,sha256=H-kPhvunQs6E6UcQo8EJU4BUS-5VvIJGNFLV9XRcTE0,8269
-tests/fixtures/tests_samples/GermEval/dev.txt,sha256=cu52g0mtyio5ZLSeWAYjqXDUjS1BePZpwGT0kmQwLJU,1718
-tests/fixtures/tests_samples/GermEval/labels.txt,sha256=t8fVkXdl_YbaRkvrlMTFaLs4mRCwc0oTSL8fcEKSnPg,218
-tests/fixtures/tests_samples/GermEval/train.txt,sha256=hrbCXqbemOYT5qh7nsuv8X9cWv-XSqlvrMGgZ37yGno,1779
-tests/fixtures/tests_samples/MRPC/dev.csv,sha256=RWZKRXC4o81DvmZR1heEJj1uUd7n1byM2aUD1qSfNoE,1354
-tests/fixtures/tests_samples/MRPC/dev.tsv,sha256=SqkXUw5tyIuoNgFiqPjOvb-lX2gHc7CB04TIKtr1Jok,1386
-tests/fixtures/tests_samples/MRPC/train.csv,sha256=RWZKRXC4o81DvmZR1heEJj1uUd7n1byM2aUD1qSfNoE,1354
-tests/fixtures/tests_samples/MRPC/train.tsv,sha256=SqkXUw5tyIuoNgFiqPjOvb-lX2gHc7CB04TIKtr1Jok,1386
-tests/fixtures/tests_samples/SQUAD/sample.json,sha256=F83am-XRiXLSg0d2c0NV_3rzcjCG_RPAZRg6BdvtRro,17233
-tests/fixtures/tests_samples/STS-B/dev.tsv,sha256=Mi3M0aZut7cc6nG4O6lOb1tG2SJji6pWuy5YIasIoVM,1126
-tests/fixtures/tests_samples/STS-B/train.tsv,sha256=1xSYqJDffO8n5Do40J85VWUj5B2jizgc39SohcgVzDg,1121
-tests/fixtures/tests_samples/conll/sample.json,sha256=Mf_53uEhd74JUHenSwIh8_kX4KB5rf0TnFo85vvvl9Y,3001
-tests/fixtures/tests_samples/swag/sample.json,sha256=njXm4XXdxYxVz7vJiucpkjBRs7VwhkW6lpxHbeeNnGc,3522
-tests/fixtures/tests_samples/wiki_text/wiki_00,sha256=qWGIX9pcn8TfFneaZ6cIyMstVJdmsj7Sn_oVQFQTwUc,79924
-tests/fixtures/tests_samples/wmt16/sample.json,sha256=PSH1usabsIumFlZv9BBrjkfFuEA4bVMEP_Qm8ZjHSrY,1423
-tests/fixtures/tests_samples/wmt_en_ro/test.json,sha256=cQ--FKyjLllS8WCvbJ541GZm_3-gdEHp6ZpPiUSpov4,27417
-tests/fixtures/tests_samples/wmt_en_ro/train.json,sha256=CzC4ogZSWGx8q0MTOxksuIJcQ6IGUEYs6-BvoHsjsjk,11234
-tests/fixtures/tests_samples/wmt_en_ro/val.json,sha256=rHKGPfMHUEba0OOab49H5Sm-OUtj_qeDGyQLlawG5xY,21699
-tests/fixtures/tests_samples/xsum/sample.json,sha256=2J_OT9Ea0CQH4VNS46-ab5Dv1TMnV2TVA5sy3FP1WaE,15601
 tests/st/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/st/test_bilstm_imdb.py,sha256=xRSKJkpI-fKDcA7YZZ2f8ipKPVN4HajdcgkNQbUvFCM,2834
 tests/st/test_longformer.py,sha256=2nOLV7RCRK8J85AinfcRxJlZB9LxHUm8zN_eECFp7Ao,2110
 tests/test_module/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_module/custom_configuration.py,sha256=7OqOEZxuJ2qshW25cPjz976chbK6hl_5zKr9G_JQ1gQ,387
 tests/test_module/custom_modeling.py,sha256=zhTelUtzaewXJPr3XpZO2Gn5as7TWsDllTAdC2tXCcc,777
 tests/test_module/custom_pipeline.py,sha256=ELI8p05HEFFdw35cQMUNp0g0r_99gU2DEWziU12jn9s,1117
@@ -754,28 +766,26 @@
 tests/ut/dataset/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/dataset/test_imdb.py,sha256=98si2jYjyug8Ag5MhuPrgCqKhMhAnY7XDca9gYHGuA4,2423
 tests/ut/dataset/transforms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/dataset/transforms/test_add_token.py,sha256=HY8sWbuOCR7Iwfu0VJU4MEch0r7RiSsjUb2HI8j2H7c,2555
 tests/ut/dataset/transforms/test_lookup.py,sha256=K4nWn92jafVGG4uXNcOP_6zvsNB8vcTJysbCzubRgT0,1235
 tests/ut/dataset/transforms/test_pad_transform.py,sha256=DeIGSzLiwH4OLb5GNCPJox1yR70WiLXbYFvASKDHvUw,2560
 tests/ut/engine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/ut/engine/test_callback.py,sha256=Nvxw09OWYrNHOdsub8RalQ5KXAH2PBZoclzixHKhsFU,2248
-tests/ut/engine/test_evaluator.py,sha256=dxRUfmnoS6j5DnNEm0Hlr2GL8mKEtFP_piPSMu_l1xI,2352
-tests/ut/engine/test_trainer.py,sha256=O6VTxj1RBVXMcthOxmpvD-joq9URchzYfwRSTJDaPco,6878
+tests/ut/engine/test_trainer.py,sha256=gI2NK7ecOUzH6PuahnUpnOC-duDxakr3sfRTpuNXBVs,92214
 tests/ut/legacy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/legacy/test_einsum.py,sha256=tNP-76eygMopj42M-2LGuVgkyDY4l7jmK5Ii8UXIDH4,845
-tests/ut/metrics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/ut/metrics/test_metrics_class.py,sha256=70z3xy9DQpahVTzQz6POD9GgVa6uvr5h56ikg57P_-0,32965
-tests/ut/metrics/test_metrics_fn.py,sha256=bGzR_dG3GuDgkTmvYk8jHqaSXjf37m_LViXpgCfgHrQ,19939
+tests/ut/legacy/metrics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/legacy/metrics/test_metrics_class.py,sha256=9-B6LWUShE_inG879frhs7knmhjNEirRIfwJ60oE97E,32973
+tests/ut/legacy/metrics/test_metrics_fn.py,sha256=YNOtxtxsSqKjDEZOH_wkjToH2qNgUV7JbpjF6cpJ6ag,19947
 tests/ut/modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/modules/test_crf.py,sha256=tB2srz7-ZHarCMtkC3J_yfoIJ89Yg5F1_7mMa-1HY4s,13357
 tests/ut/modules/test_decoder.py,sha256=MIsy98u8pgJjWi-VDe48GE7stXqBk541qebT9GdcPS8,5675
 tests/ut/modules/test_encoder.py,sha256=iFPDlI1log0sMdKzPg1G4pGguGXm_ggRE7UNxWgyl8M,4267
 tests/ut/modules/test_fasttext_embedding.py,sha256=RV9oJCcPGm1OGpIVKCdiy9MQEvJs73Zu6VbDpxpmFAw,1422
-tests/ut/modules/test_flashattention.py,sha256=YaVIrT43kDXh0SBveD-PEesWZPdN3E09CC8KVcoDYcw,3216
+tests/ut/modules/test_flashattention.py,sha256=TxvMHR2FveN3ORdk0oJWHm2k5j-atFVNnlx4J1oRP6g,6300
 tests/ut/modules/test_glove_embedding.py,sha256=ftppFF6AHXAdomdHbjGHu6_3nHFy_pqdbJX2dBU6wPA,1356
 tests/ut/modules/attentions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/modules/attentions/test_additive_attention.py,sha256=2k4nNAwc014C0vYrPcgBpa8lx0PMKG6e-qdsmOF1NTQ,1809
 tests/ut/modules/attentions/test_binary_attention.py,sha256=5BN6g8m3E_4y6gF5tsZdpf8gehiHk_urdnpMd_wyUAE,1784
 tests/ut/modules/attentions/test_cosine_attention.py,sha256=4yVUditrbV2h8CX477ZbD7t2iUZU4_6lydyfUwKFEn0,1779
 tests/ut/modules/attentions/test_linear_attention.py,sha256=62VWsEEu2c4Gi9khgSZNmIoLAL3H9vAPuTcw_WUAWbE,1831
 tests/ut/modules/attentions/test_scaled_dot_attention.py,sha256=eaMHF5bRKq7G9NXxBsBQPKv7I0G2vA4U5qusIDUKlxA,1540
@@ -790,28 +800,26 @@
 tests/ut/modules/rnns/test_lstm.py,sha256=mhOECKJuGGunkCI0HsHgKPTODY26xgIY3apiEgzSFbM,5180
 tests/ut/modules/transformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/modules/transformer/test_multi_head_attention.py,sha256=QzrRd0bVaTZ5igMtLvWrbByTui0_WcHJqwJ7PXCm-rM,3775
 tests/ut/modules/transformer/test_transformer_encoder.py,sha256=zAgME-8psLPxg8BQtJitYYKxN9YCSb7XhRZbvUmqI0k,2187
 tests/ut/modules/transformer/test_transformer_encoder_layer.py,sha256=K-kmSIMo_woyQI8EeE6puu80WoVX4dcWcpk7O3jztOI,1434
 tests/ut/peft/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/peft/test_config.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/ut/text2vec/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/ut/text2vec/test_sbert_embeddings.py,sha256=8tQMVm2_OuttPfdZdCzQkr29k4wwY_iBtcli7aAY9TQ,2756
-tests/ut/text2vec/test_w2v_embeddings.py,sha256=CDM-UuhKSfYL2wbfA9qd7qyi7K1X_r2_uBZUcWqMgDI,2078
 tests/ut/transformers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/ut/transformers/test_backbone_common.py,sha256=txxEgoTMKhv-Dy7n9Xn4CmFHinn9uJcstgzGAxKHl6c,10140
+tests/ut/transformers/test_backbone_common.py,sha256=DoCO8qRYeX4bxozju_W2XrQVdhXlftOvR3YqwBAboz4,10147
 tests/ut/transformers/test_configuration_common.py,sha256=gvvrWUeo6bDrb1_SmoM1INjpXFaKk0lveeZmLCAlVsc,8097
 tests/ut/transformers/test_feature_extraction_common.py,sha256=kWbdOsVnhh1ASYqwUpL0nwmklXl-FyaDKNSI9xHSSVI,2231
-tests/ut/transformers/test_modeling_common.py,sha256=QxNaOVSiymQm5RzvJSb2AOWKHnqUR2-maUyWsbDPHKc,73183
+tests/ut/transformers/test_image_processing_common.py,sha256=f9v5G8MSvrlI1GS4SR5GVVQ1tuaEzWA_Ee8o__HzSEY,15893
+tests/ut/transformers/test_modeling_common.py,sha256=VdlUrF5HF78er1APbqEcogUnINhp1qUuIC6yz6UFdLI,73153
 tests/ut/transformers/test_pipeline_mixin.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/test_sequence_feature_extraction_common.py,sha256=vxiKuoq2UiL_kG_D_SeMgQw3KwwJTVWHSaxTd0br7U0,16663
 tests/ut/transformers/test_tokenization_common.py,sha256=XrAn3Ti7YjSyEVodbcJm3sCOzl9fm7EH7ugTFYnpq6o,206613
 tests/ut/transformers/generation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/generation/test_framework_agnostic.py,sha256=MZ2dJM_D5Kwjgq8dZikZig2u6Ot--KQRbs04wyfFg5c,28522
-tests/ut/transformers/generation/test_utils.py,sha256=CodMjYzfrrxRSfiFaqCBuB2TdY8qaVUJYDH_BTWGoio,123394
+tests/ut/transformers/generation/test_utils.py,sha256=eeYBE6vB22ry6Vs3q1mbC5G4mEcsj6J055JYaSCNc18,123388
 tests/ut/transformers/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/albert/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/albert/test_modeling_albert.py,sha256=ODQALKRaFylnsN7Cj9kas21NGgGVJ7xvgvgMgGphwv8,14176
 tests/ut/transformers/models/albert/test_tokenization_albert.py,sha256=Cjx6OOihR3SK9v3J6Dz8Tj-7eZmZAuDi2EMBvwdbEsk,8039
 tests/ut/transformers/models/align/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/align/test_modeling_align.py,sha256=EslcA9n-2S6IexBZmO7yYCXWb-jBdj5R2F3rv6tmuQk,21247
 tests/ut/transformers/models/altclip/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -857,26 +865,30 @@
 tests/ut/transformers/models/bloom/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/bloom/test_modeling_bloom.py,sha256=VqftlJT94ESm6lqIacbQvAidYuyysKg74aUo5j-Tfqk,35152
 tests/ut/transformers/models/bridgetower/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/bridgetower/test_modeling_bridgetower.py,sha256=9ex0ainAcrDZ7J7u0pTbM754BzuPlpOEbaW9TNfmLcI,23014
 tests/ut/transformers/models/bros/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/bros/test_modeling_bros.py,sha256=qSM0LvtOy2kxVsOtkk9yhM6hMGYKBdLie0W8GadKVE4,16094
 tests/ut/transformers/models/chatglm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/ut/transformers/models/chatglm/test_modeling_chatglm.py,sha256=ccIUgeWIOHUi8ILkrIupWpanUNpVnfmXr62dwplTbx8,13895
+tests/ut/transformers/models/chatglm/test_modeling_chatglm.py,sha256=3WY4uoa43XlkhgtFmY-3vkxvKZWyqrvPzLYm7QTm-RY,13928
 tests/ut/transformers/models/chatglm/test_modeling_graph_chatglm.py,sha256=FYD3uXuxvbib86psxKqBMNQFeXuChNFGnwDZmjV6u6Y,13970
 tests/ut/transformers/models/clip/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/clip/test_modeling_clip.py,sha256=MJsXqSThGloO4Z5U6pQBFVE3Z1RJzBNw1qJh8ITXTtM,25666
 tests/ut/transformers/models/codegen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/codegen/test_modeling_codegen.py,sha256=3DTQcST5zay01pU2rr6vBUKYUr_UKgcjrRBDNuYX-uo,23368
 tests/ut/transformers/models/convbert/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/ut/transformers/models/convbert/test_modeling_convbert.py,sha256=mZWx8gl7TNhtHZRSGwYMEtgIYjti1BTpIr9pduTHijM,19793
+tests/ut/transformers/models/convbert/test_modeling_convbert.py,sha256=0k_YWZxsfxdxiFPlSsPoxZcRCa8SJVCDUZFmBZzo-O0,19740
+tests/ut/transformers/models/convnext/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/convnext/test_modeling_convnext.py,sha256=tIu_DZTP31bE5vQiJlGFF6fXEaEla_jBHZCLI7dqDHU,11121
 tests/ut/transformers/models/cpmant/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/cpmant/test_modeling_cpmant.py,sha256=WPfF8Tg7v57RM22n8FbzpQnoAjHwNRkAjQVVN0tKhEg,9906
 tests/ut/transformers/models/cpmbee/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/cpmbee/test_modeling_cpmbee.py,sha256=uxzfNbGikpwmno2iE3KSVPu369VcHsqouRvzdwNcG4w,8443
+tests/ut/transformers/models/cvt/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/cvt/test_modeling_cvt.py,sha256=_A2m8D1-ykbL8Tm1hMSVdw4vug1BMwOoGydTjnxkcbM,10006
 tests/ut/transformers/models/deberta/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/deberta/test_modeling_deberta.py,sha256=mFKfMkt7Ptc0SY3t77UwpF0y8HrPW_3FiZVCSBhhyvQ,12019
 tests/ut/transformers/models/encodec/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/encodec/test_modeling_encodec.py,sha256=xoHn4lgxTIPHfAG_i2pruPXurHtcA7KzS_Y2b8fM8mg,20901
 tests/ut/transformers/models/ernie/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/ernie/test_modeling_ernie.py,sha256=mAcgEL4IJlqkiFFETUKDyRqsffi1gsbV08GN80YXooo,22370
 tests/ut/transformers/models/ernie_m/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -893,28 +905,33 @@
 tests/ut/transformers/models/gpt2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/gpt2/test_modeling_gpt2.py,sha256=rg_xky2j9R1t5Tg6fisw8bY7ItnEVrVTg-Y4vtu7e1c,36548
 tests/ut/transformers/models/gpt_bigcode/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/gpt_bigcode/test_modeling_gpt_bigcode.py,sha256=jMi6ngGadDo3D2biZsgk8A8D5WWMJ01V8zmylJ9xPic,25963
 tests/ut/transformers/models/gpt_neo/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/gpt_neo/test_gpt_neo.py,sha256=UQ0oyrizu5dJtArW8vsen7JBx5ZXwGVfDflcAbxE9ow,4504
 tests/ut/transformers/models/gpt_neox/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/ut/transformers/models/gpt_neox/test_gpt_neox.py,sha256=r9YZH80NwCus3yNPxRWKpyR8uhO61nLY8gmGSR4I1Zc,16620
+tests/ut/transformers/models/gpt_neox/test_modeling_gpt_neox.py,sha256=nkxybSwQZtk_BLD7UQ-P2oYGgzOs8Il1CHgwcDqj2IQ,16680
 tests/ut/transformers/models/graphormer/__init__.py,sha256=ayDtxj7vzQvwz3DHSpzZ9XTxA3_06Ib35TBWLTIr_Co,691
 tests/ut/transformers/models/graphormer/test_graphormer_cells.py,sha256=nnNYekGpS76JjWSeM53fTgpbQ1kmRYC59Ice7KDTcQM,6947
 tests/ut/transformers/models/graphormer/test_modeling_graphormer.py,sha256=cNBKMMP2C2csvD5vdveRwTLN7wTynkW221A5Z-i8nVc,65804
 tests/ut/transformers/models/hubert/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/hubert/test_modeling_hubert.py,sha256=NSGOr7pKSD4LzgkvIfgJqv3NrueiQU2eIqsvbGhkiWY,29210
 tests/ut/transformers/models/internlm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/internlm/test_modeling_internlm.py,sha256=83if4Eor_TFuyeB9ggR4wcaj6Lp4volyFPW9Kej_dZM,1601
 tests/ut/transformers/models/layoutlm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/layoutlm/test_modeling_layoutlm.py,sha256=EQGuXCeuXeu5YV-3ddBmlUjNTO6_23aiwN-2H5K3gBY,17742
 tests/ut/transformers/models/layoutlmv2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/layoutlmv2/test_modeling_layoutlmv2.py,sha256=T73YyoVlZZULRX_Pllo5i8Og0dNF_9K3ZY3Zfc1PJOo,28358
 tests/ut/transformers/models/llama/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/llama/test_modeling_llama.py,sha256=mSLZgKEsVbb3o6xQbYa5VG0CmrHKF4DBdDFLTK1ce8s,27045
+tests/ut/transformers/models/llava/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/llava/test_modeling_llava.py,sha256=0_GDD4GDEox40v-v6n7i8GMWlPHFu7CBQ3VnxhYpSco,29866
+tests/ut/transformers/models/llava_next/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/llava_next/test_image_processor_llava_next.py,sha256=kGt2yU7BIyorHjF9ogiSS9z4ag1sjR9TReSkPIUeeEI,8896
+tests/ut/transformers/models/llava_next/test_modeling_llava_next.py,sha256=kripTnlGofyL40zVvI53gQ1aGkO5H3QN3hDm35ss49M,20537
 tests/ut/transformers/models/longformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/longformer/test_modeling_longformer.py,sha256=sqDvmuPzfVhzkYyUyDy2rqw5IDf7m7RkrQP4bWcTmQM,31552
 tests/ut/transformers/models/luke/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/luke/test_modeling_luke.py,sha256=EMbgSS8PV72tcsis4RnzVyeut7yPMNwA6t5RTLKEucI,11176
 tests/ut/transformers/models/mamba/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/mamba/test_modeling_graph_mamba.py,sha256=uXfVfbgO1HqigZwrlYOm2Vm_3a3W_AaUHsaRYn0pqKE,5356
 tests/ut/transformers/models/mamba/test_modeling_mamba.py,sha256=V-tfNvGvxtL8Nb5NjLZiq-k4vjZ6UMSxXRwaHXxP4Vc,19188
@@ -926,77 +943,94 @@
 tests/ut/transformers/models/mistral/test_modeling_mistral.py,sha256=yQpfWW0y0YUADQ2C1RWXayOik0kog98sQ6W8gab_Hg8,17577
 tests/ut/transformers/models/mixtral/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/mixtral/test_modeling_mixtral.py,sha256=OKLID3jo2OmJDkgiDaKXHOAuzLeVKFbrAFndKEcbiCk,19377
 tests/ut/transformers/models/mobilebert/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/mobilebert/test_mobilebert.py,sha256=f7Bth7WCncPadgDx8CXeO6zBAHGdm735om0SYbq47yU,12087
 tests/ut/transformers/models/moss/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/moss/test_modeling_moss.py,sha256=foFaNzkB8Xh3s_Hhxmj4Ob4RoqF5G_jHcInAY4d7REk,3681
+tests/ut/transformers/models/mpnet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/mpnet/test_modeling_mpnet.py,sha256=4rrZZ997TU-8eiQnlgQv7vSDYY1ZqSwpa_DwmVH6GHY,10618
+tests/ut/transformers/models/mpt/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/mpt/test_modeling_mpt.py,sha256=2H4mWWnvZrlQwl1dUlrWomgxJ_T0UGmAKgZy9Jqedfg,20662
 tests/ut/transformers/models/mt5/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/mt5/test_modeling_mt5.py,sha256=aCVi8rduOhn-5JzvvSBt0GgyMwn9rwU5CPpRDWMIO6k,2095
 tests/ut/transformers/models/musicgen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/musicgen/test_modeling_musicgen.py,sha256=oFzhHexhOfKXxvwjYD_4aaMmzBTwarEcoGzHIUg3U8M,45746
 tests/ut/transformers/models/musicgen_melody/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/musicgen_melody/test_feature_extraction_musicgen_melody.py,sha256=wZvtFaECJO36ZW0I9w8uBW4x71AGwrzNgON7eti4w8k,9926
 tests/ut/transformers/models/musicgen_melody/test_modeling_musicgen_melody.py,sha256=QB5yHOOKbNTyuoDVq6X4PICKmjRfLED-Zegsx1vxokc,46150
 tests/ut/transformers/models/musicgen_melody/test_processor_musicgen_melody.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/nezha/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/nezha/test_modeling_nezha.py,sha256=U7UCXu4YOd8RT3iD8k9XvWTN3Hp_wbAsjeoeV9LjnAc,10126
+tests/ut/transformers/models/olmo/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/olmo/test_modeling_olmo.py,sha256=t8bhLGsaTC8i-jxqTHds1NKKI0XtZm6ISE7NUzZUZxQ,19188
 tests/ut/transformers/models/opt/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/opt/test_modeling_opt.py,sha256=LO923ROHNf6TeN1OCPsw8V3QeXPbtcPzCETnxom7eyE,23125
+tests/ut/transformers/models/pegasus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/pegasus/test_modeling_pegasus.py,sha256=wsK8ElFQlV1j0BNc_I8UMxybiDyC-5jYLDz2qsgce1g,25878
 tests/ut/transformers/models/phi/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/phi/test_modeling_phi.py,sha256=eFR-QlBwwtlTB8mFtzVPcKX-Qg4PGSZOV4MXZFl_fVk,18965
 tests/ut/transformers/models/pop2piano/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/pop2piano/test_modeling_pop2piano.py,sha256=EvePTcU7D7Pt4Ee6uVn1JKfIDflE3QsnQDyKvvxs_YI,31317
 tests/ut/transformers/models/qwen2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/qwen2/test_modeling_qwen2.py,sha256=VdRe5Q3IWydnCzEKOH9YVjTPyniUroTnz6H_Vx-9IUM,19480
 tests/ut/transformers/models/qwen2_moe/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/qwen2_moe/test_modeling_qwen2_moe.py,sha256=e_eHCDEbyi8MootJfg6eDyng4kzo6qtAqjwJprHn3Bk,22239
 tests/ut/transformers/models/reformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/reformer/test_modeling_reformer.py,sha256=XZaA82pb49KWjvtx5dfnb6PpfOTArttEjf5P8BOIWpQ,43606
+tests/ut/transformers/models/resnet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/resnet/test_modeling_resnet.py,sha256=luWGArNvZVOsQbGySLk5QIbJ-IG5GxeJXNB5gj9umAI,11827
 tests/ut/transformers/models/roberta/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/roberta/test_modeling_roberta.py,sha256=TR_saviShLNur9UYnkZD5zuRVja5chC8ST7ECYXhE2M,22751
 tests/ut/transformers/models/rwkv/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/rwkv/test_modeling_rwkv.py,sha256=YlaBUd0rdkG85SXlUy6Pc34HqXMaei2dSLzNaqq5_Bc,17034
+tests/ut/transformers/models/sam/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/sam/test_modeling_sam.py,sha256=Rz6sKpbSBlt_T9eM0_8xIKModi9LTfU8s0ObmgDuglA,27308
 tests/ut/transformers/models/seamless_m4t/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/seamless_m4t/test_modeling_seamless_m4t.py,sha256=Gil-MNuBmPc8m6AKVyu445ueauNy2iaoQmk75V9LB48,45139
 tests/ut/transformers/models/seamless_m4t_v2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/seamless_m4t_v2/test_modeling_seamless_m4t_v2.py,sha256=b4SaNrF4fKLjVTTFoojk7W7SkYkqxE-9_Hhc525E9Dg,48018
+tests/ut/transformers/models/segformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/segformer/test_modeling_segformer.py,sha256=DPWi2B62IRxz5k9yKgVkiqMIRqz-v2Snm90IqvLlE0E,16779
 tests/ut/transformers/models/starcoder2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/starcoder2/test_modeling_starcoder2.py,sha256=PlIhH_s2qU0d3edPpIBGYEoa5b7Uy_X3-9h8K_pyeCo,16333
 tests/ut/transformers/models/t5/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/t5/test_modeling_t5.py,sha256=GaSM5GVB5CSMzWrYN3Hdkr5o4F3Q1OTQQ1kbdtITBJM,74031
+tests/ut/transformers/models/timesformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/timesformer/test_modeling_timesformer.py,sha256=nAl5r1u-zNKJ-oWeBVPlholZ9fAgv-2oS6JYjxLNjAA,13192
 tests/ut/transformers/models/tinybert/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/tinybert/test_tinybert.py,sha256=xths0lfNz8gPAqlVtO8ckV0Z29rZGcXa-YCtzvrz7eU,15357
+tests/ut/transformers/models/vipllava/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/ut/transformers/models/vipllava/test_modeling_vipllava.py,sha256=3HI4fplH0qDQ1bzNSvtMJ5gr6cU2DPjo6gEQd55vJ1U,18077
 tests/ut/transformers/models/wav2vec2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/wav2vec2/test_feature_extraction_wav2vec2.py,sha256=917cwLWq8Iw2iWdLYia4MmcxqT8dDQDGC6aY-FtOw-0,10497
 tests/ut/transformers/models/wav2vec2/test_modeling_wav2vec2.py,sha256=RnPXCE9Idguw_ui2MqIKkKx6nBOobtOfKbwZBheMh1c,72157
 tests/ut/transformers/models/wav2vec2/test_processor_wav2vec2.py,sha256=kKHXth8VqAYe2_Z6U5c7Uvfc6hqrYahx_inunTav26Y,6366
 tests/ut/transformers/models/wav2vec2/test_tokenization_wav2vec2.py,sha256=n2TXQBrbCioD0-c1I3ZjH_no5rHAiawyceFaG9Aolnc,40919
 tests/ut/transformers/models/whisper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/whisper/test_modeling_whisper.py,sha256=AcPz5rT1YIqSSCwF_pScW-z9Dph7YHWgKGuHzuMdq8A,77595
 tests/ut/transformers/models/xlm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/xlm/test_modeling_xlm.py,sha256=Y9GZuTbDjIwi7Kp6on47NtVDBPxbkFcqolAKoROxzLs,19441
 tests/ut/transformers/models/xlm/test_tokenization_xlm.py,sha256=0ono8j4uLPxFXtfSy9EI5ibdELLQbLYF_s7C_1Rmbms,3300
 tests/ut/transformers/models/xlm_roberta/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/models/xlm_roberta/test_modeling_xlm_roberta.py,sha256=w6aiGWIah3nRr1TtF2VDdcl_hBfyaI0-vPqEhJDmNOw,2827
 tests/ut/transformers/models/xlnet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/ut/transformers/models/xlnet/test_modeling_xlnet.py,sha256=n52pQ0ItsYPNYiO1zgbwls-pnN4E58EEQgVKWaCQMuE,28446
+tests/ut/transformers/models/xlnet/test_modeling_xlnet.py,sha256=Pp0YnUHS76BroJxiAWU0WQfG4O1z_nYZoOEPCVtuJDY,28389
 tests/ut/transformers/models/xlnet/test_tokenization_xlnet.py,sha256=3UW4vUoOEiWluXj4Je8Pap4pQskutFOP7uSgfyqWCmc,12729
 tests/ut/transformers/pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/transformers/pipelines/test_pipelines_common.py,sha256=1Dl8xZEhGqFR0AJ7VITQ-zfFhf6Y6n0fTl23S_sGEWY,18027
 tests/ut/transformers/pipelines/test_pipelines_document_question_answering.py,sha256=EkDtCyLlHJtGp59Af77yDaLkz3iCfz5Z9FIWT4-MVSc,12486
 tests/ut/transformers/pipelines/test_pipelines_question_answering.py,sha256=1yqGSZhgvLYxtT7t1Vu0Xa2FF0UQyk_noT8FNwpfCR4,25446
 tests/ut/transformers/pipelines/test_pipelines_text2text_generation.py,sha256=sMUS8KFuhOFVdcVNCMvARsCiVhmF5oNh6i3UIS7TE84,3661
 tests/ut/transformers/pipelines/test_pipelines_text_classification.py,sha256=-yPz84FUYWnsILGGdM12k6D8-ByGSGMhGqhxsVU9K_0,6805
 tests/ut/transformers/pipelines/test_pipelines_text_generation.py,sha256=1Ag3I_OezzmvjOldhnBVcZfJu9FyeIMtdTndGv3h794,13706
 tests/ut/transformers/pipelines/test_pipelines_zero_shot_classification.py,sha256=aR_vnyb08KzHYLopYJILAUVC_Ge3oVz2N7exSNTj4z0,11105
-tests/ut/utils/test_download.py,sha256=qwgNAeqs_KDBMS6xK4kKNssfLPkTk0G-q9IAZJMStss,1996
 tests/ut/vocab/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/ut/vocab/test_vocab.py,sha256=nNUuXh4xwHRSBXUCMcX24hHeuzYDuOB00jlNvvWcJKI,2076
 tests/ut/vocab/test_vocab_fasttext.py,sha256=ofhi_ruA_oGHqyZhJb1iFeFpHqKoAbpGyzeb9jdqfTg,1029
 tests/ut/vocab/test_vocab_glove.py,sha256=03WRCJDPdWcMazhbjJ88WBnlLCoRkuG5Qm5ccrsVICU,1238
-mindnlp-0.2.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mindnlp-0.2.4.dist-info/METADATA,sha256=XCCafZ2zs2ll_HbIxX1sp8GEQcgsttkPyIjZKhFdJlA,804
-mindnlp-0.2.4.dist-info/NOTICE,sha256=WMUrehXyktO2Y7n7-wX_4ODWQ6v0RNQqYNcpO8tdj-A,57
-mindnlp-0.2.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-mindnlp-0.2.4.dist-info/top_level.txt,sha256=TxwFWW5fBi37a5G0OYTMGr42mW2sYvTk9hcQlhfuzaY,14
-mindnlp-0.2.4.dist-info/RECORD,,
+mindnlp-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mindnlp-0.3.0.dist-info/METADATA,sha256=BFuvLaoqLJkIJZ2nUyHxHlf-zc68L0gcTkhzvFzpdQY,849
+mindnlp-0.3.0.dist-info/NOTICE,sha256=WMUrehXyktO2Y7n7-wX_4ODWQ6v0RNQqYNcpO8tdj-A,57
+mindnlp-0.3.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+mindnlp-0.3.0.dist-info/top_level.txt,sha256=TxwFWW5fBi37a5G0OYTMGr42mW2sYvTk9hcQlhfuzaY,14
+mindnlp-0.3.0.dist-info/RECORD,,
```

