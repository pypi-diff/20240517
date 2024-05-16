# Comparing `tmp/lamini-2.1.8-123-py3-none-any.whl.zip` & `tmp/lamini-2.2.0a1-124-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,58 +1,59 @@
-Zip file size: 689452 bytes, number of entries: 56
--rw-r--r--  2.0 unx     1363 b- defN 24-Apr-18 20:53 lamini/__init__.py
--rw-r--r--  2.0 unx     2200 b- defN 24-Apr-18 20:52 lamini/api/classifier.py
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-18 20:52 lamini/api/embedding.py
--rw-r--r--  2.0 unx    12631 b- defN 24-Apr-18 20:52 lamini/api/lamini.py
--rw-r--r--  2.0 unx     2369 b- defN 24-Apr-18 20:52 lamini/api/lamini_config.py
--rw-r--r--  2.0 unx     2518 b- defN 24-Apr-18 20:52 lamini/api/precise_trainer.py
--rw-r--r--  2.0 unx     6208 b- defN 24-Apr-18 20:52 lamini/api/rest_requests.py
--rw-r--r--  2.0 unx     6824 b- defN 24-Apr-18 20:52 lamini/api/streaming_completion.py
--rw-r--r--  2.0 unx     1547 b- defN 24-Apr-18 20:52 lamini/api/synchronize.py
--rw-r--r--  2.0 unx     6617 b- defN 24-Apr-18 20:52 lamini/api/train.py
--rw-r--r--  2.0 unx     4605 b- defN 24-Apr-18 20:52 lamini/api/utils/async_inference_queue.py
--rw-r--r--  2.0 unx     5930 b- defN 24-Apr-18 20:52 lamini/api/utils/async_inference_queue_3_10.py
--rw-r--r--  2.0 unx     1494 b- defN 24-Apr-18 20:52 lamini/api/utils/base_async_inference_queue.py
--rw-r--r--  2.0 unx     1343 b- defN 24-Apr-18 20:52 lamini/api/utils/completion.py
--rw-r--r--  2.0 unx     2865 b- defN 24-Apr-18 20:52 lamini/api/utils/process_batch.py
--rw-r--r--  2.0 unx     5959 b- defN 24-Apr-18 20:52 lamini/api/utils/reservations.py
--rw-r--r--  2.0 unx      413 b- defN 24-Apr-18 20:52 lamini/api/utils/shutdown.py
--rw-r--r--  2.0 unx     1393 b- defN 24-Apr-18 20:52 lamini/api/utils/upload_client.py
--rw-r--r--  2.0 unx    24530 b- defN 24-Apr-18 20:52 lamini/classify/lamini_classifier.py
--rw-r--r--  2.0 unx      896 b- defN 24-Apr-18 20:52 lamini/error/error.py
--rw-r--r--  2.0 unx     2906 b- defN 24-Apr-18 20:52 lamini/evaluators/benchmark.py
--rw-r--r--  2.0 unx     2820 b- defN 24-Apr-18 20:52 lamini/evaluators/custom/custom_evaluator.py
--rw-r--r--  2.0 unx     9671 b- defN 24-Apr-18 20:52 lamini/evaluators/custom/earnings_call_evaluator.py
--rw-r--r--  2.0 unx     9770 b- defN 24-Apr-18 20:52 lamini/evaluators/custom/ecommerce_evaluator.py
--rw-r--r--  2.0 unx     9121 b- defN 24-Apr-18 20:52 lamini/evaluators/custom/icd_evaluator.py
--rw-r--r--  2.0 unx  1298418 b- defN 24-Apr-18 20:52 lamini/evaluators/custom/datasets/earnings_calls.jsonl
--rw-r--r--  2.0 unx  5527615 b- defN 24-Apr-18 20:52 lamini/evaluators/custom/datasets/icd11.jsonl
--rw-r--r--  2.0 unx   732222 b- defN 24-Apr-18 20:52 lamini/evaluators/custom/datasets/shopping.jsonl
--rw-r--r--  2.0 unx     5413 b- defN 24-Apr-18 20:52 lamini/evaluators/helm/harness_evaluator.py
--rw-r--r--  2.0 unx      775 b- defN 24-Apr-18 20:52 lamini/evaluators/helm/mmlu_evaluator.py
--rw-r--r--  2.0 unx      861 b- defN 24-Apr-18 20:52 lamini/evaluators/helm/truthfulqa_evaluator.py
--rw-r--r--  2.0 unx     2441 b- defN 24-Apr-18 20:52 lamini/evaluators/utils/utils.py
--rw-r--r--  2.0 unx     1273 b- defN 24-Apr-18 20:52 lamini/generation/base_generation_queue.py
--rw-r--r--  2.0 unx      594 b- defN 24-Apr-18 20:52 lamini/generation/base_node_object.py
--rw-r--r--  2.0 unx      797 b- defN 24-Apr-18 20:52 lamini/generation/base_prompt_object.py
--rw-r--r--  2.0 unx     2154 b- defN 24-Apr-18 20:52 lamini/generation/classifier_node.py
--rw-r--r--  2.0 unx     1418 b- defN 24-Apr-18 20:52 lamini/generation/embedding_node.py
--rw-r--r--  2.0 unx     5101 b- defN 24-Apr-18 20:52 lamini/generation/generation_node.py
--rw-r--r--  2.0 unx     3868 b- defN 24-Apr-18 20:52 lamini/generation/generation_pipeline.py
--rw-r--r--  2.0 unx     6615 b- defN 24-Apr-18 20:52 lamini/generation/generation_queue_3_10.py
--rw-r--r--  2.0 unx     2014 b- defN 24-Apr-18 20:52 lamini/generation/index_node.py
--rw-r--r--  2.0 unx      965 b- defN 24-Apr-18 20:52 lamini/generation/modify_node.py
--rw-r--r--  2.0 unx     3448 b- defN 24-Apr-18 20:52 lamini/generation/process_generation_batch.py
--rw-r--r--  2.0 unx     1390 b- defN 24-Apr-18 20:52 lamini/generation/split_response_node.py
--rw-r--r--  2.0 unx      557 b- defN 24-Apr-18 20:52 lamini/generation/token_optimizer.py
--rw-r--r--  2.0 unx     3413 b- defN 24-Apr-18 20:52 lamini/index/lamini_index.py
--rw-r--r--  2.0 unx     9354 b- defN 24-Apr-18 20:52 lamini/runners/base_runner.py
--rw-r--r--  2.0 unx      720 b- defN 24-Apr-18 20:52 lamini/runners/basic_model_runner.py
--rw-r--r--  2.0 unx     3062 b- defN 24-Apr-18 20:52 lamini/runners/llama_v2_runner.py
--rw-r--r--  2.0 unx     2625 b- defN 24-Apr-18 20:52 lamini/runners/mistral_runner.py
--rw-r--r--  2.0 unx       21 b- defN 24-Apr-18 20:52 llama/__init__.py
--rw-r--r--  2.0 unx    11340 b- defN 24-Apr-18 20:53 lamini-2.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1507 b- defN 24-Apr-18 20:53 lamini-2.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 20:53 lamini-2.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-18 20:53 lamini-2.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5067 b- defN 24-Apr-18 20:53 lamini-2.1.8.dist-info/RECORD
-56 files, 7762275 bytes uncompressed, 681308 bytes compressed:  91.2%
+Zip file size: 690663 bytes, number of entries: 57
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-16 22:24 lamini/__init__.py
+-rw-r--r--  2.0 unx     2200 b- defN 24-May-16 22:24 lamini/api/classifier.py
+-rw-r--r--  2.0 unx     1129 b- defN 24-May-16 22:24 lamini/api/embedding.py
+-rw-r--r--  2.0 unx    13018 b- defN 24-May-16 22:24 lamini/api/lamini.py
+-rw-r--r--  2.0 unx     2369 b- defN 24-May-16 22:24 lamini/api/lamini_config.py
+-rw-r--r--  2.0 unx     2404 b- defN 24-May-16 22:24 lamini/api/precise_trainer.py
+-rw-r--r--  2.0 unx     6208 b- defN 24-May-16 22:24 lamini/api/rest_requests.py
+-rw-r--r--  2.0 unx     6827 b- defN 24-May-16 22:24 lamini/api/streaming_completion.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-16 22:24 lamini/api/synchronize.py
+-rw-r--r--  2.0 unx     6999 b- defN 24-May-16 22:24 lamini/api/train.py
+-rw-r--r--  2.0 unx     4605 b- defN 24-May-16 22:24 lamini/api/utils/async_inference_queue.py
+-rw-r--r--  2.0 unx     5930 b- defN 24-May-16 22:24 lamini/api/utils/async_inference_queue_3_10.py
+-rw-r--r--  2.0 unx     1494 b- defN 24-May-16 22:24 lamini/api/utils/base_async_inference_queue.py
+-rw-r--r--  2.0 unx     1343 b- defN 24-May-16 22:24 lamini/api/utils/completion.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-16 22:24 lamini/api/utils/process_batch.py
+-rw-r--r--  2.0 unx     5959 b- defN 24-May-16 22:24 lamini/api/utils/reservations.py
+-rw-r--r--  2.0 unx      413 b- defN 24-May-16 22:24 lamini/api/utils/shutdown.py
+-rw-r--r--  2.0 unx     1394 b- defN 24-May-16 22:24 lamini/api/utils/upload_client.py
+-rw-r--r--  2.0 unx    24599 b- defN 24-May-16 22:24 lamini/classify/lamini_classifier.py
+-rw-r--r--  2.0 unx      896 b- defN 24-May-16 22:24 lamini/error/error.py
+-rw-r--r--  2.0 unx     2906 b- defN 24-May-16 22:24 lamini/evaluators/benchmark.py
+-rw-r--r--  2.0 unx     2820 b- defN 24-May-16 22:24 lamini/evaluators/custom/custom_evaluator.py
+-rw-r--r--  2.0 unx     9671 b- defN 24-May-16 22:24 lamini/evaluators/custom/earnings_call_evaluator.py
+-rw-r--r--  2.0 unx     9770 b- defN 24-May-16 22:24 lamini/evaluators/custom/ecommerce_evaluator.py
+-rw-r--r--  2.0 unx     9121 b- defN 24-May-16 22:24 lamini/evaluators/custom/icd_evaluator.py
+-rw-r--r--  2.0 unx  1298418 b- defN 24-May-16 22:24 lamini/evaluators/custom/datasets/earnings_calls.jsonl
+-rw-r--r--  2.0 unx  5527615 b- defN 24-May-16 22:24 lamini/evaluators/custom/datasets/icd11.jsonl
+-rw-r--r--  2.0 unx   732222 b- defN 24-May-16 22:24 lamini/evaluators/custom/datasets/shopping.jsonl
+-rw-r--r--  2.0 unx     5413 b- defN 24-May-16 22:24 lamini/evaluators/helm/harness_evaluator.py
+-rw-r--r--  2.0 unx      775 b- defN 24-May-16 22:24 lamini/evaluators/helm/mmlu_evaluator.py
+-rw-r--r--  2.0 unx      861 b- defN 24-May-16 22:24 lamini/evaluators/helm/truthfulqa_evaluator.py
+-rw-r--r--  2.0 unx     2441 b- defN 24-May-16 22:24 lamini/evaluators/utils/utils.py
+-rw-r--r--  2.0 unx     1273 b- defN 24-May-16 22:24 lamini/generation/base_generation_queue.py
+-rw-r--r--  2.0 unx      594 b- defN 24-May-16 22:24 lamini/generation/base_node_object.py
+-rw-r--r--  2.0 unx      797 b- defN 24-May-16 22:24 lamini/generation/base_prompt_object.py
+-rw-r--r--  2.0 unx     2154 b- defN 24-May-16 22:24 lamini/generation/classifier_node.py
+-rw-r--r--  2.0 unx     1418 b- defN 24-May-16 22:24 lamini/generation/embedding_node.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-16 22:24 lamini/generation/generation_node.py
+-rw-r--r--  2.0 unx     3868 b- defN 24-May-16 22:24 lamini/generation/generation_pipeline.py
+-rw-r--r--  2.0 unx     6615 b- defN 24-May-16 22:24 lamini/generation/generation_queue_3_10.py
+-rw-r--r--  2.0 unx     2014 b- defN 24-May-16 22:24 lamini/generation/index_node.py
+-rw-r--r--  2.0 unx      965 b- defN 24-May-16 22:24 lamini/generation/modify_node.py
+-rw-r--r--  2.0 unx     3454 b- defN 24-May-16 22:24 lamini/generation/process_generation_batch.py
+-rw-r--r--  2.0 unx     1390 b- defN 24-May-16 22:24 lamini/generation/split_response_node.py
+-rw-r--r--  2.0 unx      557 b- defN 24-May-16 22:24 lamini/generation/token_optimizer.py
+-rw-r--r--  2.0 unx     3413 b- defN 24-May-16 22:24 lamini/index/lamini_index.py
+-rw-r--r--  2.0 unx     9354 b- defN 24-May-16 22:24 lamini/runners/base_runner.py
+-rw-r--r--  2.0 unx      720 b- defN 24-May-16 22:24 lamini/runners/basic_model_runner.py
+-rw-r--r--  2.0 unx     3068 b- defN 24-May-16 22:24 lamini/runners/llama_v2_runner.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-16 22:24 lamini/runners/llama_v3_runner.py
+-rw-r--r--  2.0 unx     2625 b- defN 24-May-16 22:24 lamini/runners/mistral_runner.py
+-rw-r--r--  2.0 unx       21 b- defN 24-May-16 22:24 llama/__init__.py
+-rw-r--r--  2.0 unx    11340 b- defN 24-May-16 22:24 lamini-2.2.0a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1509 b- defN 24-May-16 22:24 lamini-2.2.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 22:24 lamini-2.2.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-16 22:24 lamini-2.2.0a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5167 b- defN 24-May-16 22:24 lamini-2.2.0a1.dist-info/RECORD
+57 files, 7766380 bytes uncompressed, 682357 bytes compressed:  91.2%
```

## zipnote {}

```diff
@@ -141,29 +141,32 @@
 
 Filename: lamini/runners/basic_model_runner.py
 Comment: 
 
 Filename: lamini/runners/llama_v2_runner.py
 Comment: 
 
+Filename: lamini/runners/llama_v3_runner.py
+Comment: 
+
 Filename: lamini/runners/mistral_runner.py
 Comment: 
 
 Filename: llama/__init__.py
 Comment: 
 
-Filename: lamini-2.1.8.dist-info/LICENSE
+Filename: lamini-2.2.0a1.dist-info/LICENSE
 Comment: 
 
-Filename: lamini-2.1.8.dist-info/METADATA
+Filename: lamini-2.2.0a1.dist-info/METADATA
 Comment: 
 
-Filename: lamini-2.1.8.dist-info/WHEEL
+Filename: lamini-2.2.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: lamini-2.1.8.dist-info/top_level.txt
+Filename: lamini-2.2.0a1.dist-info/top_level.txt
 Comment: 
 
-Filename: lamini-2.1.8.dist-info/RECORD
+Filename: lamini-2.2.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lamini/__init__.py

```diff
@@ -1,13 +1,14 @@
 # Turn of isort, because alphabetic order for the following imports causes circular dependency issues
 
 # isort: off
 from lamini.error import error
 
 from lamini.runners.llama_v2_runner import LlamaV2Runner
+from lamini.runners.llama_v3_runner import LlamaV3Runner
 from lamini.runners.basic_model_runner import BasicModelRunner
 from lamini.runners.mistral_runner import MistralRunner
 from lamini.api.lamini import Lamini
 from lamini.classify.lamini_classifier import LaminiClassifier, BinaryLaminiClassifier
 from lamini.api.classifier import Classifier
 from lamini.api.embedding import Embedding
 from lamini.generation.generation_node import GenerationNode
```

## lamini/api/lamini.py

```diff
@@ -134,16 +134,20 @@
         return results
 
     def upload_data(
         self,
         data: Iterable[Dict[str, Union[int, float, str, bool, Dict, List]]],
         is_public: Optional[bool] = None,
     ):
+        num_datapoints = 0
+
         def get_data_str(d):
+            nonlocal num_datapoints
             for item in d:
+                num_datapoints += 1
                 yield json.dumps(item) + "\n"
 
         if not data:
             raise ValueError("Data pairs cannot be empty.")
 
         output = self.trainer.get_upload_base_path()
         self.upload_base_path = output["upload_base_path"]
@@ -154,14 +158,17 @@
             if self.upload_base_path == "azure":
                 data_str = get_data_str(data)
                 output = self.trainer.create_blob_dataset_location(
                     self.upload_base_path, dataset_id, is_public
                 )
                 self.upload_file_path = output["dataset_location"]
                 upload_to_blob(data_str, self.upload_file_path)
+                self.trainer.update_blob_dataset_num_datapoints(
+                    dataset_id, num_datapoints
+                )
                 print("Data pairs uploaded to blob.")
             else:
                 output = self.trainer.upload_dataset_locally(
                     self.upload_base_path, dataset_id, is_public, data
                 )
                 self.upload_file_path = output["dataset_location"]
                 print("Data pairs uploaded to local.")
@@ -224,74 +231,71 @@
             raise Exception(
                 "Upload of only csv and jsonlines file supported at the moment."
             )
         return items
 
     def train(
         self,
-        data: Optional[
-            Iterable[Dict[str, Union[int, float, str, bool, Dict, List]]]
-        ] = None,
+        data_or_dataset_id: Union[
+            str, Iterable[Dict[str, Union[int, float, str, bool, Dict, List]]]
+        ],
         finetune_args: Optional[dict] = None,
+        gpu_config: Optional[dict] = None,
         enable_peft: Optional[bool] = None,
         peft_args: Optional[dict] = None,
         is_public: Optional[bool] = None,
         use_cached_model: Optional[bool] = None,
-        dataset_id: Optional[str] = None,
         multi_node: Optional[bool] = None,
     ):
-        if dataset_id:
-            output = self.trainer.get_upload_base_path()
-            self.upload_base_path = output["upload_base_path"]
-            output = self.trainer.get_existing_dataset(
-                dataset_id, self.upload_base_path, is_public
-            )
-            self.upload_file_path = output["dataset_location"]
-            data = None
-
-        elif not dataset_id and data:
-            dataset_id = self.upload_data(data, is_public)
-            data = None
-
+        if isinstance(data_or_dataset_id, str):
+            dataset_id = data_or_dataset_id
         else:
-            raise ValueError(
-                "Data pairs can not be empty. Either data or dataset_id must be provided."
-            )
+            dataset_id = self.upload_data(data_or_dataset_id, is_public=is_public)
+        assert dataset_id is not None
+        output = self.trainer.get_upload_base_path()
+        self.upload_base_path = output["upload_base_path"]
+        output = self.trainer.get_existing_dataset(
+            dataset_id, self.upload_base_path, is_public
+        )
+        self.upload_file_path = output["dataset_location"]
 
-        # TODO: remove passing `data` completely.
         job = self.trainer.train(
-            data,
-            self.model_name,
-            self.upload_file_path,
-            finetune_args,
-            enable_peft,
-            peft_args,
-            is_public,
-            use_cached_model,
-            dataset_id,
-            multi_node,
+            model_name=self.model_name,
+            dataset_id=dataset_id,
+            upload_file_path=self.upload_file_path,
+            finetune_args=finetune_args,
+            gpu_config=gpu_config,
+            enable_peft=enable_peft,
+            peft_args=peft_args,
+            is_public=is_public,
+            use_cached_model=use_cached_model,
+            multi_node=multi_node,
         )
         job["dataset_id"] = dataset_id
         return job
 
     # continuously poll until the job is completed
     def train_and_wait(
         self,
-        data: Optional[List] = None,
+        data_or_dataset_id: Union[
+            str, Iterable[Dict[str, Union[int, float, str, bool, Dict, List]]]
+        ],
         finetune_args: Optional[dict] = None,
+        gpu_config: Optional[dict] = None,
         enable_peft: Optional[bool] = None,
         peft_args: Optional[dict] = None,
         is_public: Optional[bool] = None,
         use_cached_model: Optional[bool] = None,
         multi_node: Optional[bool] = None,
         **kwargs,
     ):
         job = self.train(
-            data,
+            data_or_dataset_id,
             finetune_args=finetune_args,
+            gpu_config=gpu_config,
             enable_peft=enable_peft,
             peft_args=peft_args,
             is_public=is_public,
             use_cached_model=use_cached_model,
             multi_node=multi_node,
         )
 
@@ -353,14 +357,14 @@
         output_type,
         max_tokens,
         max_new_tokens,
     ):
         req_data = {}
         req_data["model_name"] = model_name
         req_data["prompt"] = prompt
-        req_data["out_type"] = output_type
+        req_data["output_type"] = output_type
         req_data["max_tokens"] = max_tokens
         if max_new_tokens is not None:
             req_data["max_new_tokens"] = max_new_tokens
         if self.model_config:
             req_data["model_config"] = self.model_config.as_dict()
         return req_data
```

## lamini/api/precise_trainer.py

```diff
@@ -27,48 +27,45 @@
         self.model_config = self.config.get("model_config", None)
 
     def upload_file(
         self, file_path, input_key: str = "input", output_key: str = "output"
     ):
         items = self.lamini_api._upload_file_impl(file_path, input_key, output_key)
         try:
-            self.lamini_api.upload_data(items)
+            return self.lamini_api.upload_data(items)
         except Exception as e:
             print(f"Error reading data file: {e}")
             raise e
 
     def train(
         self,
-        data: Optional[
-            Iterable[Dict[str, Union[int, float, str, bool, Dict, List]]]
-        ] = None,
+        data_or_dataset_id: Union[
+            str, Iterable[Dict[str, Union[int, float, str, bool, Dict, List]]]
+        ],
         finetune_args: Optional[dict] = None,
+        gpu_config: Optional[dict] = None,
         is_public: Optional[bool] = None,
         use_cached_model: Optional[bool] = None,
-        dataset_id: Optional[str] = None,
     ):
-        if dataset_id:
-            self.upload_base_path = self.trainer.get_upload_base_path()[
-                "upload_base_path"
-            ]
-            output = self.trainer.get_existing_dataset(
-                dataset_id, self.upload_base_path, is_public
+        if isinstance(data_or_dataset_id, str):
+            dataset_id = data_or_dataset_id
+        else:
+            dataset_id = self.lamini_api.upload_data(
+                data_or_dataset_id, is_public=is_public
             )
-            self.upload_file_path = output["dataset_location"]
+        self.upload_base_path = self.trainer.get_upload_base_path()["upload_base_path"]
+        output = self.trainer.get_existing_dataset(
+            dataset_id, self.upload_base_path, is_public
+        )
+        self.upload_file_path = output["dataset_location"]
 
-        if dataset_id is None and data is not None:
-            dataset_id = self.lamini_api.upload_data(data, is_public)
-            if (
-                self.upload_base_path == "azure"
-            ):  # if data is uploaded to azure, dont send it with the request
-                data = None
         job = self.trainer.precise_train(
-            data,
             self.model_name,
+            dataset_id,
             self.upload_file_path or self.lamini_api.upload_file_path,
             finetune_args,
+            gpu_config,
             is_public,
             use_cached_model,
-            dataset_id,
         )
         job["dataset_id"] = dataset_id
         return job
```

## lamini/api/streaming_completion.py

```diff
@@ -200,14 +200,14 @@
 
     def make_llm_req_map(
         self, model_name, prompt, output_type, max_tokens, max_new_tokens, server
     ):
         req_data = {}
         req_data["model_name"] = model_name
         req_data["prompt"] = prompt
-        req_data["out_type"] = output_type
+        req_data["output_type"] = output_type
         req_data["max_tokens"] = max_tokens
         if max_new_tokens is not None:
             req_data["max_new_tokens"] = max_new_tokens
         if server is not None:
             req_data["server"] = server
         return req_data
```

## lamini/api/train.py

```diff
@@ -21,81 +21,79 @@
         self.api_url = api_url or lamini.api_url or get_configured_url(self.config)
         self.api_prefix = self.api_url + "/v1/"
         self.ui_url = "https://app.lamini.ai"
         self.model_config = self.config.get("model_config", None)
 
     def train(
         self,
-        data: list,
         model_name: str,
+        dataset_id: str,
         upload_file_path: Optional[str] = None,
         finetune_args: Optional[dict] = None,
+        gpu_config: Optional[dict] = None,
         enable_peft: Optional[bool] = None,
         peft_args: Optional[dict] = None,
         is_public: Optional[bool] = None,
         use_cached_model: Optional[bool] = None,
-        dataset_id: Optional[str] = None,
         multi_node: Optional[bool] = None,
     ):
         req_data = {"model_name": model_name}
-        if data is not None:
-            req_data["data"] = data
+        req_data["dataset_id"] = dataset_id
         if upload_file_path is not None:
             req_data["upload_file_path"] = upload_file_path
         if finetune_args is not None:
             req_data["finetune_args"] = finetune_args
+        if gpu_config is not None:
+            req_data["gpu_config"] = gpu_config
         if enable_peft is not None:
             req_data["enable_peft"] = enable_peft
         if peft_args is not None:
             req_data["peft_args"] = peft_args
         if is_public is not None:
             req_data["is_public"] = is_public
         if use_cached_model is not None:
             req_data["use_cached_model"] = use_cached_model
         if self.model_config:
             req_data["model_config"] = self.model_config.as_dict()
-        if dataset_id is not None:
-            req_data["dataset_id"] = dataset_id
         if multi_node is not None:
             req_data["multi_node"] = multi_node
         url = self.api_prefix + "train"
 
         job = make_web_request(self.api_key, url, "post", req_data)
         self.job_id = job["job_id"]
         print(
             f"Training job submitted! Check status of job {self.job_id} here: {self.ui_url}/train/{self.job_id}"
         )
 
         return job
 
     def precise_train(
         self,
-        data: list,
         model_name: str,
+        dataset_id: str,
         upload_file_path: Optional[str] = None,
         finetune_args: Optional[dict] = None,
+        gpu_config: Optional[dict] = None,
         is_public: Optional[bool] = None,
         use_cached_model: Optional[bool] = None,
-        dataset_id: Optional[str] = None,
     ):
         req_data = {"model_name": model_name}
-        if data is not None:
-            req_data["data"] = data
+        req_data["dataset_id"] = dataset_id
         if upload_file_path is not None:
             req_data["upload_file_path"] = upload_file_path
         if finetune_args is not None:
             req_data["finetune_args"] = finetune_args
+        if gpu_config is not None:
+            req_data["gpu_config"] = gpu_config
         if is_public is not None:
             req_data["is_public"] = is_public
         if use_cached_model is not None:
             req_data["use_cached_model"] = use_cached_model
         if self.model_config:
             req_data["model_config"] = self.model_config.as_dict()
-        if dataset_id is not None:
-            req_data["dataset_id"] = dataset_id
         url = self.api_prefix + "precise_train"
 
         job = make_web_request(self.api_key, url, "post", req_data)
         self.job_id = job["job_id"]
         print(
             f"Training job submitted! Check status of job {self.job_id} here: {self.ui_url}/train/{self.job_id}"
         )
@@ -142,28 +140,45 @@
 
         return make_web_request(self.api_key, url, "get")
 
     def create_blob_dataset_location(
         self, upload_base_path, dataset_id, is_public, data=None
     ):
         url = self.api_prefix + "data"
-        req_data = {"upload_base_path": upload_base_path, "dataset_id": dataset_id}
+        req_data = {
+            "upload_base_path": upload_base_path,
+            "dataset_id": dataset_id,
+        }
 
         if is_public is not None:
             req_data["is_public"] = is_public
 
         if data is not None:
             req_data["data"] = data
 
         return make_web_request(
             self.api_key,
             url,
             "post",
             req_data,
         )
+
+    def update_blob_dataset_num_datapoints(self, dataset_id, num_datapoints):
+        url = self.api_prefix + "data/num-datapoints"
+        req_data = {
+            "num_datapoints": num_datapoints,
+            "dataset_id": dataset_id,
+        }
+
+        return make_web_request(
+            self.api_key,
+            url,
+            "post",
+            req_data,
+        )
 
     def get_upload_base_path(self):
         url = self.api_prefix + "get-upload-base-path"
         return make_web_request(self.api_key, url, "get")
 
     def upload_dataset_locally(self, upload_base_path, dataset_id, is_public, data):
         url = self.api_prefix + "local-data"
```

## lamini/api/utils/upload_client.py

```diff
@@ -1,12 +1,13 @@
 import hashlib
+import itertools
 import os
 import time
 from typing import Dict, Iterable, List, Union
-import itertools
+
 import jsonlines
 from azure.storage.blob import BlobClient
 
 
 def upload_to_blob(data: Iterable[str], sas_url: str):
     blob_client_sas = BlobClient.from_blob_url(blob_url=sas_url)
```

## lamini/classify/lamini_classifier.py

```diff
@@ -20,15 +20,15 @@
     examples from prompts and then uses a logistic regression to classify
     the examples.
     """
 
     def __init__(
         self,
         config: dict = {},
-        model_name: str = "meta-llama/Llama-2-7b-chat-hf",
+        model_name: str = "meta-llama/Meta-Llama-3-8B-Instruct",
         augmented_example_count: int = 10,
         generator_from_prompt=None,
         example_modifier=None,
         example_expander=None,
     ):
         self.classifier = LaminiClassifier(
             config=config,
@@ -93,15 +93,15 @@
     examples from prompts and then trains a final logistic regression on top
     of an LLM to classify the examples.
     """
 
     def __init__(
         self,
         config: dict = {},
-        model_name: str = "meta-llama/Llama-2-7b-chat-hf",
+        model_name: str = "meta-llama/Meta-Llama-3-8B-Instruct",
         augmented_example_count: int = 10,
         batch_size: int = 10,
         threads: int = 1,
         saved_examples_path: str = "/tmp/saved_examples.jsonl",
         generator_from_prompt=None,
         example_modifier=None,
         example_expander=None,
@@ -457,15 +457,15 @@
 
 
 class DefaultExampleGenerator:
     def __init__(
         self,
         prompt,
         config=None,
-        model_name="meta-llama/Llama-2-7b-chat-hf",
+        model_name="meta-llama/Meta-Llama-3-8B-Instruct",
         batch_size=10,
     ):
         self.prompt = prompt
         self.config = config
         self.example_count = 5
         self.model_name = model_name
         self.batch_size = batch_size
@@ -566,15 +566,18 @@
             ]
 
         return all_examples
 
 
 class DefaultExampleModifier:
     def __init__(
-        self, config=None, model_name="meta-llama/Llama-2-7b-chat-hf", batch_size=10
+        self,
+        config=None,
+        model_name="meta-llama/Meta-Llama-3-8B-Instruct",
+        batch_size=10,
     ):
         self.config = config
         self.model_name = model_name
         self.required_examples = 5
         self.batch_size = batch_size
 
     def modify_examples(self, examples):
@@ -660,15 +663,17 @@
                 result["example_5"],
             ]
 
         return all_examples
 
 
 class DefaultExampleExpander:
-    def __init__(self, prompt, config=None, model_name="meta-llama/Llama-2-7b-chat-hf"):
+    def __init__(
+        self, prompt, config=None, model_name="meta-llama/Meta-Llama-3-8B-Instruct"
+    ):
         self.prompt = prompt
         self.config = config
         self.model_name = model_name
 
     def expand_example(self, example_batch):
         runner = LlamaV2Runner(config=self.config, model_name=self.model_name)
```

## lamini/generation/generation_node.py

```diff
@@ -70,15 +70,15 @@
         output_type,
         max_tokens,
         max_new_tokens,
     ):
         req_data = {}
         req_data["model_name"] = model_name
         req_data["prompt"] = prompt
-        req_data["out_type"] = output_type
+        req_data["output_type"] = output_type
         req_data["max_tokens"] = max_tokens
         if max_new_tokens is not None:
             req_data["max_new_tokens"] = max_new_tokens
         if self.model_config:
             req_data["model_config"] = self.model_config.as_dict()
         req_data["type"] = "completion"
         return req_data
```

## lamini/generation/process_generation_batch.py

```diff
@@ -87,13 +87,13 @@
             "prompt": [p.get_prompt() for p in batch["prompt"]],
         }
     else:
         json = {
             "reservation_id": reservation_id,
             "model_name": batch["model_name"],
             "prompt": [p.get_prompt() for p in batch["prompt"]],
-            "out_type": batch["out_type"],
+            "output_type": batch["output_type"],
             "max_tokens": batch["max_tokens"],
             "max_new_tokens": batch.get("max_new_tokens", None),
             "model_config": batch.get("model_config", None),
         }
     return json
```

## lamini/runners/llama_v2_runner.py

```diff
@@ -10,15 +10,15 @@
 
 
 class LlamaV2Runner(BaseRunner):
     """A class for running and training a Llama V2 model, using system and user prompts"""
 
     def __init__(
         self,
-        model_name: str = "meta-llama/Llama-2-7b-chat-hf",
+        model_name: str = "meta-llama/Meta-Llama-3-8B-Instruct",
         system_prompt: str = None,
         prompt_template="<s>[INST] <<SYS>>\n{system}\n<</SYS>>\n\n{user} [/INST]",
         api_key=None,
         api_url=None,
         config={},
         local_cache_file=None,
     ):
```

## lamini/runners/mistral_runner.py

```diff
@@ -5,15 +5,15 @@
 
 DEFAULT_SYSTEM_PROMPT = "Always assist with care, respect, and truth. Respond with utmost utility yet securely. Avoid harmful, unethical, prejudiced, or negative content. Ensure replies promote fairness and positivity."
 
 
 class MistralRunner(BaseRunner):
     def __init__(
         self,
-        model_name="mistralai/Mistral-7B-Instruct-v0.1",
+        model_name="mistralai/Mistral-7B-Instruct-v0.2",
         system_prompt: str = None,
         prompt_template="<s>[INST] {system} {user} [/INST]",
         api_key=None,
         api_url=None,
         config={},
         local_cache_file=None,
     ):
```

## Comparing `lamini-2.1.8.dist-info/LICENSE` & `lamini-2.2.0a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lamini-2.1.8.dist-info/METADATA` & `lamini-2.2.0a1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamini
-Version: 2.1.8
+Version: 2.2.0a1
 Summary: Build on large language models faster
 Author-email: PowerML <info@powerml.co>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

## Comparing `lamini-2.1.8.dist-info/RECORD` & `lamini-2.2.0a1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-lamini/__init__.py,sha256=kRVJzhJ0UKa9ScKEO81jcPWffi-x4IzhLExH07MeEm8,1363
+lamini/__init__.py,sha256=Sx_94ell5ny8qL40VBM22omxf5u49-YjGR_eMAt3d8Y,1420
 lamini/api/classifier.py,sha256=Xv8EwtyLD4n5M5N7tW33wmKFBhXI5OV6uMT7DYqxBX4,2200
 lamini/api/embedding.py,sha256=jbfbNmS7jyBYO_Nylp3kw7L-Zb0GrZa1owoRAtgFmNY,1129
-lamini/api/lamini.py,sha256=_GPyCZeqT1qvwj2qvhF-jKEMcIvlFowNkX9gZa_6q7E,12631
+lamini/api/lamini.py,sha256=o7BcUXF1zgWgx62IsimKxxG0ryUqhx3GmwYGmaMb3ik,13018
 lamini/api/lamini_config.py,sha256=LcPqdlaMAdoahFNlH1ig1NYfMK_z0nQMneafhcZWuu4,2369
-lamini/api/precise_trainer.py,sha256=cO02f9asuFQumcTKxYNXzWNVutBZSgTKKb6BlZfC0yQ,2518
+lamini/api/precise_trainer.py,sha256=-30qzyw7AAcnU8QhQo1iaU8YQrGDuFdWXGhBHhT3ffc,2404
 lamini/api/rest_requests.py,sha256=i1nIcAOrtE4zvs0le4mPz37NUq1_Hrty4f5zl0D446w,6208
-lamini/api/streaming_completion.py,sha256=HS9bB_4Onwbs7oQ8UonMClD8eEnFmt6e1acVTuS0kHA,6824
+lamini/api/streaming_completion.py,sha256=cSiU80XgOj1p9nOPh6j_N-z8T9Zp1CM6yZN4R7hncCA,6827
 lamini/api/synchronize.py,sha256=Uo6-lQToa-42zVdQ4Qlefvf0Mi3i2He_W1S9yciMMNk,1547
-lamini/api/train.py,sha256=WOtuMceFrvE-aAmYwif3xliuOxkDdzwEYKXG0AIWlXQ,6617
+lamini/api/train.py,sha256=t6tN7pC88iWQIc_lPwsrBTAgnsmHigo-DtyvFiaJz-U,6999
 lamini/api/utils/async_inference_queue.py,sha256=M-7RMyMIFcMS47Z2l9-8W05SafuJnnYiQvLUTgWWfdw,4605
 lamini/api/utils/async_inference_queue_3_10.py,sha256=Itmn1E9bfotiVmnO-k1dznAP87sY-EKRUC-zuZkkLtQ,5930
 lamini/api/utils/base_async_inference_queue.py,sha256=4JvyjGSQfxcSAvV5hQ2-VqbN_1diqLW_nJzNUsEXXnU,1494
 lamini/api/utils/completion.py,sha256=37vn81fvpGR7HMuGQy1Cwz2ozIj0aZQTcxHzXl-cVpI,1343
 lamini/api/utils/process_batch.py,sha256=nNWu80NSeYig_MoO1GQs_JOiJMQgpts0F5Y-xQMDmG8,2865
 lamini/api/utils/reservations.py,sha256=yXnGPM1eQXgzRdQ1rjtoHMSxn4DhDPetxJfPl5221_4,5959
 lamini/api/utils/shutdown.py,sha256=oznFdh3JsE3CDH4Fx30c8_pVGBlIF0iPlFCFpoTE4iU,413
-lamini/api/utils/upload_client.py,sha256=n4VpSgg5n17NUr6PL7eT_aQESPz7GyrJb3x9jG-o1Kw,1393
-lamini/classify/lamini_classifier.py,sha256=k8QM40qbmnooIUQfjN8SoBwdwlJqj0ybs4gskDs3IDo,24530
+lamini/api/utils/upload_client.py,sha256=nTossvV58LSVvdny1iuTO6PPomE3HlPxjt2_xkmw0V8,1394
+lamini/classify/lamini_classifier.py,sha256=HW6yRQxjcApX2DeG4EAgZSR1t3ucgbXd1tlb65qYV18,24599
 lamini/error/error.py,sha256=C4SbfG3obNYGH8onkUkhUc61XRTwejCBlsG1QBNaEQI,896
 lamini/evaluators/benchmark.py,sha256=sXEmTgEKMvKng-4FjEZZB_AFKd5__KQSalKvdB_qFQs,2906
 lamini/evaluators/custom/custom_evaluator.py,sha256=XvNSIznP_3gNN7sbXOryOCWor7I7tO3Tsy6bOgJRpGA,2820
 lamini/evaluators/custom/earnings_call_evaluator.py,sha256=S_mE6X5UgpXKm97DnfhcnYkmVA3BfmVqDBAgsfnAq-w,9671
 lamini/evaluators/custom/ecommerce_evaluator.py,sha256=zsMSuZ2DtrBuEzvahI3khd_j9nNRNUX2Whe1UHoqK18,9770
 lamini/evaluators/custom/icd_evaluator.py,sha256=jt98RxQIWrz6yV8t67O3TJEhP9fFfMn0_cOmat57n5o,9121
 lamini/evaluators/custom/datasets/earnings_calls.jsonl,sha256=x4Rr_ds8vMQDBWZWlRcF0vVrF54X3eoDQKGEALkFe6M,1298418
@@ -31,26 +31,27 @@
 lamini/evaluators/helm/truthfulqa_evaluator.py,sha256=xS8hpoKudf3K99eaEnbM5EShB_QTDOPffhFEOYntGww,861
 lamini/evaluators/utils/utils.py,sha256=DRevBVPgYChc46r3vpA_FXzfTFO0S976MI6mfyjpaic,2441
 lamini/generation/base_generation_queue.py,sha256=D_gav4v76N9Oo2r0dWYNuho2A8nKdr0Q-0xMjZMmyPk,1273
 lamini/generation/base_node_object.py,sha256=Q_t8eqCnf5HnLOHQTMpFaIq-_I2_YhXUhi64FeRF5-M,594
 lamini/generation/base_prompt_object.py,sha256=nC5VTLoiNzYoQquA2nPeqAvWY_zeSJlDtQnb5iuutSk,797
 lamini/generation/classifier_node.py,sha256=EPD1eQyyu3M_tbjPfOzL5Ejg6LQjOh1pUWbbJwhkkc0,2154
 lamini/generation/embedding_node.py,sha256=Iq2PlnI6yMTpwxG67w07029VDp_aJjKNbHhAgN4utnk,1418
-lamini/generation/generation_node.py,sha256=62X4Bm_qcdPd0J4Z6AyYWDOMNeiQgkT8EpIs77BZaWQ,5101
+lamini/generation/generation_node.py,sha256=xEtEio0GdFY7bh03hU3J7DwHV2rX4Iv0EcB_o3frwz0,5104
 lamini/generation/generation_pipeline.py,sha256=jbBYbVV4w8Tmrdzo84c-0GpSfM9a_ZIqJ6yqiXyWvks,3868
 lamini/generation/generation_queue_3_10.py,sha256=sm33jtLqN7HpIhWvJYX6v9pNPq3IXLWlYv068dOFK-k,6615
 lamini/generation/index_node.py,sha256=A2y__ukKaZotXM1kqBOZAS5mxfpyq-h6tnmlsUvj5D0,2014
 lamini/generation/modify_node.py,sha256=OKH1dmJmptteccspAxS3sgyP4NvFyix3HTnzaGyb7DI,965
-lamini/generation/process_generation_batch.py,sha256=siVQuzJMX0x5xesyzUucUzX6nJ-Y8jFgs3csfbUoP6I,3448
+lamini/generation/process_generation_batch.py,sha256=3ohOioemMjAnhbNOAlLgphMGwPZwHyCeFsxtxk5Ziow,3454
 lamini/generation/split_response_node.py,sha256=sZJaPj_4mdf-m-c4CAQ22O6nzA53fsHKzI5P7Irw7Do,1390
 lamini/generation/token_optimizer.py,sha256=LI7-APb8XM_Jg1WNL2DuQV4NcoY3y1FL-B3KlDPNe0E,557
 lamini/index/lamini_index.py,sha256=Hdc3pNxdGHwz10hUlR9frBluDBOe9l45_nS9UnIR6vk,3413
 lamini/runners/base_runner.py,sha256=VYPlMdx2sR9BLXrO_jsyp-p0_3IQUXwPkVta8g6xFPE,9354
 lamini/runners/basic_model_runner.py,sha256=7e4xTotKGdmC0PH-ynAlOtXxHDvhH8HInqWCggG5DOA,720
-lamini/runners/llama_v2_runner.py,sha256=T2OjiJTC0goNpZebD1iKOKkuL5aAjfdrTvxss-d5ezM,3062
-lamini/runners/mistral_runner.py,sha256=uHS2ptK01JMGnvSi4zH6bcWquuZYjc3eIFgzWnFeg1Q,2625
+lamini/runners/llama_v2_runner.py,sha256=UWzd4P2zV0qSC9Id72CqH68vGF9w69y48ldx0-mJSFY,3068
+lamini/runners/llama_v3_runner.py,sha256=negM9Eiv6qnrWH_knEf6FHVWW6HF6eWED2eBqNp21Hc,3203
+lamini/runners/mistral_runner.py,sha256=q-MhkotBc1Y9y57Uym9k4ONBkGn9mRBLhJue3M9uMd8,2625
 llama/__init__.py,sha256=E77xncFEWyRrg-MsjkiLrCkNJBIYIxr111hLd7WpgjY,21
-lamini-2.1.8.dist-info/LICENSE,sha256=-alRIf0b5B1SavU0njHUTAanPUn6GHxH9a2Q_ACz1HM,11340
-lamini-2.1.8.dist-info/METADATA,sha256=VNnVz9kN3wZDHVTi_z7V40_WKwfo9hSb61KwJ2haIv8,1507
-lamini-2.1.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-lamini-2.1.8.dist-info/top_level.txt,sha256=5h0-n2aeXxQUxmNPPJ0AnsKIBAZV_qWqU0JIpA6Q2zo,13
-lamini-2.1.8.dist-info/RECORD,,
+lamini-2.2.0a1.dist-info/LICENSE,sha256=-alRIf0b5B1SavU0njHUTAanPUn6GHxH9a2Q_ACz1HM,11340
+lamini-2.2.0a1.dist-info/METADATA,sha256=SdsCJcgYg4ohrtif_8YDTeZb36yzDbbE1fD-p38MjFo,1509
+lamini-2.2.0a1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+lamini-2.2.0a1.dist-info/top_level.txt,sha256=5h0-n2aeXxQUxmNPPJ0AnsKIBAZV_qWqU0JIpA6Q2zo,13
+lamini-2.2.0a1.dist-info/RECORD,,
```

